# Comparing `tmp/pipeline-telemetry-0.9.4.tar.gz` & `tmp/pipeline_telemetry-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline-telemetry-0.9.4.tar", last modified: Thu Nov  3 22:11:48 2022, max compression
+gzip compressed data, was "pipeline_telemetry-1.0.0.tar", last modified: Wed May  8 13:22:19 2024, max compression
```

## Comparing `pipeline-telemetry-0.9.4.tar` & `pipeline_telemetry-1.0.0.tar`

### file list

```diff
@@ -1,131 +1,112 @@
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.467711 pipeline-telemetry-0.9.4/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      642 2022-11-03 22:02:53.000000 pipeline-telemetry-0.9.4/.bumpversion.cfg
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3006 2021-10-06 14:03:48.000000 pipeline-telemetry-0.9.4/.cookiecutterrc
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      334 2021-10-25 11:35:17.000000 pipeline-telemetry-0.9.4/.coveragerc
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      353 2021-10-06 14:03:48.000000 pipeline-telemetry-0.9.4/.editorconfig
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       30 2021-10-14 08:35:23.000000 pipeline-telemetry-0.9.4/.isort.cfg
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      554 2021-10-06 14:03:48.000000 pipeline-telemetry-0.9.4/.pre-commit-config.yaml
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      284 2021-10-14 12:50:04.000000 pipeline-telemetry-0.9.4/.readthedocs.yml
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      822 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/.travis.yml
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       38 2021-10-14 09:01:58.000000 pipeline-telemetry-0.9.4/AUTHORS.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     5778 2022-11-03 22:07:44.000000 pipeline-telemetry-0.9.4/CHANGELOG.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2787 2021-10-06 14:03:48.000000 pipeline-telemetry-0.9.4/CONTRIBUTING.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)    43679 2021-10-06 14:03:48.000000 pipeline-telemetry-0.9.4/LICENSE
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      428 2022-09-09 20:11:33.000000 pipeline-telemetry-0.9.4/MANIFEST.in
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     7853 2022-11-03 22:11:48.467903 pipeline-telemetry-0.9.4/PKG-INFO
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2928 2022-05-16 11:19:15.000000 pipeline-telemetry-0.9.4/README.rst
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:47.964541 pipeline-telemetry-0.9.4/ci/
--rwxr-xr-x   0 maartenderuyter   (501) staff       (20)     2811 2021-10-25 11:35:17.000000 pipeline-telemetry-0.9.4/ci/bootstrap.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       70 2021-10-06 20:05:29.000000 pipeline-telemetry-0.9.4/ci/requirements.txt
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.021347 pipeline-telemetry-0.9.4/ci/templates/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     1557 2021-10-06 14:03:48.000000 pipeline-telemetry-0.9.4/ci/templates/.appveyor.yml
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     1014 2021-10-06 14:03:48.000000 pipeline-telemetry-0.9.4/ci/templates/.travis.yml
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.200142 pipeline-telemetry-0.9.4/docs/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     4039 2022-05-16 10:43:09.000000 pipeline-telemetry-0.9.4/docs/adding telemetry.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       28 2021-10-06 14:03:49.000000 pipeline-telemetry-0.9.4/docs/authors.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       30 2021-10-06 14:03:49.000000 pipeline-telemetry-0.9.4/docs/changelog.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     1303 2022-11-03 22:02:58.000000 pipeline-telemetry-0.9.4/docs/conf.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       33 2021-10-06 14:03:48.000000 pipeline-telemetry-0.9.4/docs/contributing.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     6523 2022-05-12 20:32:43.000000 pipeline-telemetry-0.9.4/docs/decorators.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      381 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/docs/index.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     5964 2022-05-13 11:45:26.000000 pipeline-telemetry-0.9.4/docs/process_type.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       27 2021-10-06 14:03:49.000000 pipeline-telemetry-0.9.4/docs/readme.rst
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.202490 pipeline-telemetry-0.9.4/docs/reference/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       70 2021-10-06 14:03:49.000000 pipeline-telemetry-0.9.4/docs/reference/index.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      142 2021-10-06 14:03:49.000000 pipeline-telemetry-0.9.4/docs/reference/pipeline_telemetry.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       63 2021-11-05 22:58:40.000000 pipeline-telemetry-0.9.4/docs/requirements.txt
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      109 2021-10-06 14:03:49.000000 pipeline-telemetry-0.9.4/docs/spelling_wordlist.txt
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      337 2022-05-15 20:22:43.000000 pipeline-telemetry-0.9.4/docs/storage class.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3417 2022-11-03 22:08:45.000000 pipeline-telemetry-0.9.4/docs/telemetry aggregation.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2243 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/docs/telemetry counters.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     5847 2022-06-09 19:46:24.000000 pipeline-telemetry-0.9.4/docs/telemetry mixin.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2303 2022-05-13 08:56:37.000000 pipeline-telemetry-0.9.4/docs/telemetry object.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2889 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/docs/usage.rst
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      553 2022-11-03 22:11:48.469362 pipeline-telemetry-0.9.4/setup.cfg
--rwxr-xr-x   0 maartenderuyter   (501) staff       (20)     3028 2022-11-03 22:02:41.000000 pipeline-telemetry-0.9.4/setup.py
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:47.789061 pipeline-telemetry-0.9.4/src/
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.221801 pipeline-telemetry-0.9.4/src/pipeline_telemetry/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2778 2022-11-03 21:55:44.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/__init__.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      405 2021-10-06 14:03:49.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/__main__.py
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.273113 pipeline-telemetry-0.9.4/src/pipeline_telemetry/aggregator/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      192 2022-11-03 21:58:10.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/aggregator/__init__.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     7778 2022-11-03 22:04:48.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/aggregator/aggregator.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2203 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/aggregator/helper.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2356 2022-11-03 22:00:14.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/aggregator/mongo_aggregator.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      843 2021-10-06 14:03:49.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/cli.py
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.279499 pipeline-telemetry-0.9.4/src/pipeline_telemetry/data_classes/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       68 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/data_classes/__init__.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     8188 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/data_classes/telemetry_models.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     5915 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/decorator.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3585 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/helper.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)    14126 2022-10-05 16:09:27.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/main.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2874 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/mixin.py
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.304399 pipeline-telemetry-0.9.4/src/pipeline_telemetry/settings/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      297 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/settings/__init__.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3060 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/settings/data_class.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3421 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/settings/date_ranges.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     5656 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/settings/exceptions.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     1864 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/settings/process_type.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3045 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/settings/settings.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     1328 2022-01-31 13:50:13.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/settings/telemetry_errors.py
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.360647 pipeline-telemetry-0.9.4/src/pipeline_telemetry/storage/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      103 2022-03-25 10:38:03.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/storage/__init__.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     6143 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/storage/generic.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     6136 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/storage/memory.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     6002 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/storage/mongo.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      940 2022-10-07 13:52:49.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/storage/mongo_connection.py
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.372589 pipeline-telemetry-0.9.4/src/pipeline_telemetry/validators/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      169 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/validators/__init__.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2212 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/validators/abstract_validator_instruction.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3434 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/validators/dict_validator.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     4837 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/validators/entries_have_key.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     1259 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/validators/has_key.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2612 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry/validators/validate_entries.py
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.266012 pipeline-telemetry-0.9.4/src/pipeline_telemetry.egg-info/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     7853 2022-11-03 22:11:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3707 2022-11-03 22:11:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 maartenderuyter   (501) staff       (20)        1 2022-11-03 22:11:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       68 2022-11-03 22:11:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry.egg-info/entry_points.txt
--rw-r--r--   0 maartenderuyter   (501) staff       (20)        1 2021-10-06 19:31:23.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry.egg-info/not-zip-safe
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       38 2022-11-03 22:11:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry.egg-info/requires.txt
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       19 2022-11-03 22:11:47.000000 pipeline-telemetry-0.9.4/src/pipeline_telemetry.egg-info/top_level.txt
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.405500 pipeline-telemetry-0.9.4/tests/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2562 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/tests/test_add_telemetry.py
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.422938 pipeline-telemetry-0.9.4/tests/test_aggregator/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      775 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/tests/test_aggregator/test_aggregator.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     1869 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/tests/test_aggregator/test_aggregator_data.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     4194 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/tests/test_aggregator/test_daily_aggregator.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     5887 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/tests/test_aggregator/test_helper.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      761 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/tests/test_aggregator/test_mongo_aggregator.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     1289 2022-11-03 22:04:30.000000 pipeline-telemetry-0.9.4/tests/test_aggregator/test_partial_aggregator.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3642 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/tests/test_data.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     6395 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/tests/test_decorator.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     7866 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/tests/test_helpers.py
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.428911 pipeline-telemetry-0.9.4/tests/test_integration/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3485 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/tests/test_integration/test_int_telemetry.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3350 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/tests/test_integration/test_integration_data.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2804 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/tests/test_mixin.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)       85 2021-10-06 14:03:48.000000 pipeline-telemetry-0.9.4/tests/test_pipeline_telemetry.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2570 2021-10-25 11:35:17.000000 pipeline-telemetry-0.9.4/tests/test_process_types.py
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.435896 pipeline-telemetry-0.9.4/tests/test_settings/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)        0 2021-09-29 18:55:19.000000 pipeline-telemetry-0.9.4/tests/test_settings/__init__.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     5882 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/tests/test_settings/test_date_time_ranges.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     6445 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/tests/test_settings/test_exceptions.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      459 2022-01-31 13:50:24.000000 pipeline-telemetry-0.9.4/tests/test_settings_module.py
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.448535 pipeline-telemetry-0.9.4/tests/test_storage/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     4205 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/tests/test_storage/test_mongo_storage.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)    14427 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/tests/test_storage/test_sqllite_storage.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)      200 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/tests/test_storage/test_storage_data.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     1462 2022-01-31 13:50:19.000000 pipeline-telemetry-0.9.4/tests/test_telemetry_class_methods.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     9263 2022-10-04 18:39:14.000000 pipeline-telemetry-0.9.4/tests/test_telemetry_counter.py
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.453958 pipeline-telemetry-0.9.4/tests/test_telemetry_models/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)    17026 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/tests/test_telemetry_models/test_telemetry_class.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2826 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/tests/test_telemetry_models/test_telemetry_data.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     6873 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/tests/test_telemetry_models/test_telemetry_model.py
-drwxr-xr-x   0 maartenderuyter   (501) staff       (20)        0 2022-11-03 22:11:48.466191 pipeline-telemetry-0.9.4/tests/test_validators/
--rw-r--r--   0 maartenderuyter   (501) staff       (20)        0 2021-09-29 18:55:06.000000 pipeline-telemetry-0.9.4/tests/test_validators/__init__.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3165 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/tests/test_validators/test_dict_validator.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     6513 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/tests/test_validators/test_entries_have_key.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     3142 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/tests/test_validators/test_has_key_instruction.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     4741 2022-09-09 19:39:49.000000 pipeline-telemetry-0.9.4/tests/test_validators/test_validate_entries.py
--rw-r--r--   0 maartenderuyter   (501) staff       (20)     2017 2022-10-26 16:24:47.000000 pipeline-telemetry-0.9.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    43679 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.115273 pipeline_telemetry-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/adding telemetry.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/process_type.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.115273 pipeline_telemetry-1.0.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/reference/pipeline_telemetry.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/storage class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/telemetry aggregation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/telemetry counters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/telemetry mixin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/telemetry object.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-08 13:22:19.131273 pipeline_telemetry-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.111273 pipeline_telemetry-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.115273 pipeline_telemetry-1.0.0/src/pipeline_telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.119273 pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/mongo_aggregator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.119273 pipeline_telemetry-1.0.0/src/pipeline_telemetry/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/data_classes/telemetry_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14116 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.119273 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/data_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/date_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/process_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/telemetry_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.119273 pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/mongo_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.123273 pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/abstract_validator_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/entries_have_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/has_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/validate_entries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-08 13:22:19.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-08 13:22:19.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:22:19.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 13:22:19.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 13:22:19.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.123273 pipeline_telemetry-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_add_telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.123273 pipeline_telemetry-1.0.0/tests/test_aggregator/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_aggregator/test_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_aggregator/test_aggregator_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_aggregator/test_daily_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_aggregator/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_aggregator/test_mongo_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_aggregator/test_partial_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_integration/test_int_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_integration/test_integration_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_process_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/tests/test_settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_settings/test_date_time_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_settings/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_settings_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/tests/test_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_storage/test_mongo_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_storage/test_sqllite_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_storage/test_storage_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_telemetry_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_telemetry_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/tests/test_telemetry_models/
+-rw-r--r--   0 runner    (1001) docker     (127)    16966 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_telemetry_models/test_telemetry_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_telemetry_models/test_telemetry_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_telemetry_models/test_telemetry_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/tests/test_validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_validators/test_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_validators/test_entries_have_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_validators/test_has_key_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_validators/test_validate_entries.py
```

### Comparing `pipeline-telemetry-0.9.4/CHANGELOG.rst` & `pipeline_telemetry-1.0.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 
 Changelog
 =========
+1.0.0 (2024-05-08)
+-------------------
+* Added python 3.12 support
 
 0.9.4 (2022-11-03)
 -------------------
 * Added ``PartialToSingleMongoAggregator`` and ``PartialToSingleAggregator``
   classes to allow automated aggregation of multiple partial telemetry objects to a single telemetry object.
```

### Comparing `pipeline-telemetry-0.9.4/CONTRIBUTING.rst` & `pipeline_telemetry-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pipeline-telemetry-0.9.4/LICENSE` & `pipeline_telemetry-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline-telemetry-0.9.4/PKG-INFO` & `pipeline_telemetry-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,88 @@
 Metadata-Version: 2.1
 Name: pipeline-telemetry
-Version: 0.9.4
-Summary: Create and store data pipeline telemetry data
+Version: 1.0.0
+Summary: Measure your data pipelines with easy to use telemetry logic
 Home-page: https://github.com/MaartendeRuyter/pipeline-telemetry
 Author: Maarten de Ruyter
-Author-email: maarten@geodatagarden.com
-License: LGPL-3.0-or-later
-Project-URL: Documentation, https://pipeline-telemetry.readthedocs.io/
-Project-URL: Changelog, https://pipeline-telemetry.readthedocs.io/en/latest/changelog.html
-Project-URL: Issue Tracker, https://github.com/MaartendeRuyter/pipeline-telemetry/issues
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
+Author-email: "Maarten de Ruyter" <maarten@geodatagarden.com>
+License: GNU
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Utilities
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.rst
+Requires-Dist: error-manager
+Requires-Dist: mongoengine
+Requires-Dist: jmespath
 
 ========
 Overview
 ========
 
+.. start-badges
+
+.. list-table::
+    :stub-columns: 1
+
+    * - docs
+      - |docs|
+    * - tests
+      - | |travis| |requires|
+        | |codecov|
+    * - package
+      - | |version| |wheel|
+        | |supported-versions|
+        | |supported-implementations|
+        | |commits-since|
+.. |docs| image:: https://readthedocs.org/projects/pipeline-telemetry/badge/?style=flat
+    :target: https://pipeline-telemetry.readthedocs.io/
+    :alt: Documentation Status
+
+.. |travis| image:: https://api.travis-ci.com/MaartendeRuyter/pipeline-telemetry.svg?branch=master
+    :alt: Travis-CI Build Status
+    :target: https://travis-ci.com/github/MaartendeRuyter/pipeline-telemetry
+
+.. |requires| image:: https://requires.io/github/MaartendeRuyter/pipeline-telemetry/requirements.svg?branch=master
+    :alt: Requirements Status
+    :target: https://requires.io/github/MaartendeRuyter/pipeline-telemetry/requirements/?branch=master
+
+.. |codecov| image:: https://codecov.io/gh/MaartendeRuyter/pipeline-telemetry/branch/master/graphs/badge.svg?branch=master
+    :alt: Coverage Status
+    :target: https://codecov.io/github/MaartendeRuyter/pipeline-telemetry
+
+.. |version| image:: https://img.shields.io/pypi/v/pipeline-telemetry.svg
+    :alt: PyPI Package latest release
+    :target: https://pypi.org/project/pipeline-telemetry
+
+.. |wheel| image:: https://img.shields.io/pypi/wheel/pipeline-telemetry.svg
+    :alt: PyPI Wheel
+    :target: https://pypi.org/project/pipeline-telemetry
+
+.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/pipeline-telemetry.svg
+    :alt: Supported versions
+    :target: https://pypi.org/project/pipeline-telemetry
+
+.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pipeline-telemetry.svg
+    :alt: Supported implementations
+    :target: https://pypi.org/project/pipeline-telemetry
+
+.. |commits-since| image:: https://img.shields.io/github/commits-since/MaartendeRuyter/pipeline-telemetry/v0.0.1.svg
+    :alt: Commits since latest release
+    :target: https://github.com/MaartendeRuyter/pipeline-telemetry/compare/v0.0.1...master
 
 
+
+.. end-badges
+
 Create and store data pipeline telemetry data
 
 * Free software: GNU Lesser General Public License v3 or later (LGPLv3+)
 
 Installing pipeline-telemetry
 =============================
 
@@ -79,14 +125,17 @@
       - ::
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
+1.0.0 (2024-05-08)
+-------------------
+* Added python 3.12 support
 
 0.9.4 (2022-11-03)
 -------------------
 * Added ``PartialToSingleMongoAggregator`` and ``PartialToSingleAggregator``
   classes to allow automated aggregation of multiple partial telemetry objects to a single telemetry object.
 
 
@@ -277,9 +326,7 @@
 * Added MongoDb storage class
 * Started with documentation
 
 
 0.0.1 (2021-10-06)
 ------------------
 * First release on PyPI.
-
-
```

### Comparing `pipeline-telemetry-0.9.4/README.rst` & `pipeline_telemetry-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pipeline-telemetry-0.9.4/docs/adding telemetry.rst` & `pipeline_telemetry-1.0.0/docs/adding telemetry.rst`

 * *Files identical despite different names*

### Comparing `pipeline-telemetry-0.9.4/docs/decorators.rst` & `pipeline_telemetry-1.0.0/docs/decorators.rst`

 * *Files identical despite different names*

### Comparing `pipeline-telemetry-0.9.4/docs/process_type.rst` & `pipeline_telemetry-1.0.0/docs/process_type.rst`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
       - Sub process to convert the data to a form in which it can be uploaded
     * - DATA_UPLOAD
       - Sub process to upload the data to a specific target
 
 
 Creating your own process types and subtypes
 --------------------------------------------
-The package allows for custom process types and subtypes to be defined. This can easily be done with the ``ProcessType`` class. Be aware that your custom process types need to be :ref:`registered<Registering process types>` with the ``Telemetry`` class before they can be used. In the example below the process type CUSTOM_GET_WEATHER_DATA is defined with 5 sub process types.:: 
+The package allows for custom process types and subtypes to be defined. This can easily be done with the ``ProcessType`` class. Be aware that your custom process types need to be registered with the ``Telemetry`` class before they can be used. In the example below the process type CUSTOM_GET_WEATHER_DATA is defined with 5 sub process types.:: 
 
     from pipeline_telemetry import ProcessType, Telemetry
 
     GET_WEATHER_DATA = ProcessType(
         process_type = 'CUSTOM_GET_WEATHER_DATA',
         subtypes = [
             'RETRIEVE_WEATHER_OBJECT_FROM_API',
@@ -148,9 +148,9 @@
         'source_name': 'SOME_WEATHER_API',
         'process_type': ProcessTypes.GET_CLIMATE_DATA,
         'telemetry_rules': {}
         }
     
     telemetry_obj = Telemetry(**TELEMETRY_LOAD_CLIMATE_DATA)
 
-You can now :ref:`add telemetry<Adding telemetry datapoints>` to this telemetry object using subprocess, 'RETRIEVE_CLIMATE_OBJECT_FROM_API', 'CONVERT_TO_YEARLY_CLIMATE_OBJECT' and 
+You can now add telemetry to this telemetry object using subprocess, 'RETRIEVE_CLIMATE_OBJECT_FROM_API', 'CONVERT_TO_YEARLY_CLIMATE_OBJECT' and 
 'STORE_YEARLY_CLIMATE'.
```

### Comparing `pipeline-telemetry-0.9.4/docs/telemetry aggregation.rst` & `pipeline_telemetry-1.0.0/docs/telemetry aggregation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,19 @@
     # run daily aggregations for period from 10 days agon till 5 days ago.
     aggregator.aggeregate(start_date, end_date)
 
     # run a daily aggregation for yesterdays telemertry.
     aggregator.aggeregat_yesterda()
 
 
-PartialToDailyAggregator
-------------------------
-This aggregetor creates single aggregations (with telemetry_type 'SINGLE AGGREGATION') from selected telemetry objects with telemetry_type 'PARTIAL TELEMETRY'. PartialToDailyAggregators can be used when data jobs are split into sepreate jobs each creating their own partial telemetry. PartialToDailyAggregator can then be used to merge all the Partial telemetry object into a single aggregation object.
+PartialToSingleAggregator
+-------------------------
+This aggregetor creates single aggregations (with telemetry_type 'SINGLE AGGREGATION') from selected telemetry objects with telemetry_type 'PARTIAL TELEMETRY'. PartialToSingleAggregators can be used when data jobs are split into sepreate jobs each creating their own partial telemetry. PartialToSingleAggregator can then be used to merge all the Partial telemetry object into a single aggregation object.
 
 
 MongoDB Aggregator
 ------------------
 A mongo DB version of the aggregator classes have been made such that you no longer have to provide the MongoDB storage class yourself.
 
 Available MongoDB aggregators.
 ``DailyMongoAggregator``
-``PartialToDailyMongoAggregator``
+``PartialToSingleyMongoAggregator``
```

### Comparing `pipeline-telemetry-0.9.4/docs/telemetry counters.rst` & `pipeline_telemetry-1.0.0/docs/telemetry counters.rst`

 * *Files identical despite different names*

### Comparing `pipeline-telemetry-0.9.4/docs/telemetry mixin.rst` & `pipeline_telemetry-1.0.0/docs/telemetry mixin.rst`

 * *Files identical despite different names*

### Comparing `pipeline-telemetry-0.9.4/docs/telemetry object.rst` & `pipeline_telemetry-1.0.0/docs/telemetry object.rst`

 * *Files 11% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     * - process_type
       - ProcessType
       - Mandatory
       - Object that defines which data pipeline the telemetry is about
     * - telemetry_type
       - str
       - Optional
-      - Value from predefined set of :ref:`telemetry types<Telemetry types>`.
+      - Value from predefined telemetry types.
 
 
 These 3 identifiers allow you to find and group your telemetry data for a
 specific pipeline.
```

### Comparing `pipeline-telemetry-0.9.4/docs/usage.rst` & `pipeline_telemetry-1.0.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/aggregator/aggregator.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/aggregator.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,44 +10,50 @@
 >>> telemetry_object = Telemetry(**telemtry_params)
 >>> # create aggregator
 >>> aggregator = TelemetryAggregator(telemetry_object)
 >>> # aggregate a telemetry queryset and return the result
 >>> aggregated_telemetry = aggregator.aggregate(telemetry_queryset)
 
 """
+
 from abc import ABC
 from datetime import date, datetime, timedelta
 from typing import Iterator, Protocol, Type
 
 from pipeline_telemetry.data_classes import TelemetryModel
 from pipeline_telemetry.settings import exceptions
 from pipeline_telemetry.settings import settings as st
-from pipeline_telemetry.settings.date_ranges import DateTimeRange, \
-    get_daily_date_ranges
+from pipeline_telemetry.settings.date_ranges import DateTimeRange, get_daily_date_ranges
 
 from .helper import TelemetryAggregator, TelemetryListArgs, TelemetrySelector
 
 DATE_TIME_RANGE_GENERATOR = {
     st.DAILY_AGGR_TELEMETRY_TYPE: get_daily_date_ranges,
 }
 
 
 class TelemetryStorage(Protocol):
-
     def telemetry_list(
-            self, telemetry_type: str, category: str, sub_category: str,
-            source_name: str, process_type: str, from_date_time: datetime,
-            to_date_time: datetime) -> Iterator[TelemetryModel]:
+        self,
+        telemetry_type: str,
+        category: str,
+        sub_category: str,
+        source_name: str,
+        process_type: str,
+        from_date_time: datetime,
+        to_date_time: datetime,
+    ) -> Iterator[TelemetryModel]:
         """
-        Method to return an iteraror TelemetryModel instances retrieved from a database query with the provided arguments.
+        Method to return an iteraror TelemetryModel instances retrieved from a
+        database query with the provided arguments.
         """
         ...
 
     def store_telemetry(self, telemetry: TelemetryModel) -> None:
-        """ public method to persist telemetry object"""
+        """public method to persist telemetry object"""
         ...
 
 
 class AbstractAggregator(ABC):
     """
     Aggregator to aggregate all SINGLE TELEMETRY objects for a single day
     into a telemetry objetc of type DAILY AGGREGATION.
@@ -65,72 +71,72 @@
 
     __telemetry_selector: TelemetrySelector
     __target_telemetry: TelemetryModel
     __telemetry_storage: TelemetryStorage
     __aggregator: Type[TelemetryAggregator] = TelemetryAggregator
 
     def __init__(
-            self, telemetry_selector: TelemetrySelector,
-            telemetry_storage: TelemetryStorage) -> None:
+        self, telemetry_selector: TelemetrySelector, telemetry_storage: TelemetryStorage
+    ) -> None:
         self.__telemetry_selector = telemetry_selector
         self.__telemetry_storage = telemetry_storage
         self._set_target_telemetry_model()
 
     @property
     def target_telemetry(self):
         return self.__target_telemetry
 
     @property
     def storage_class(self):
         return self.__telemetry_storage
 
     def aggregate(self, start_date: date, end_date: date) -> None:
-        """Method to run all aggregations in the given time period.
-        """
+        """Method to run all aggregations in the given time period."""
         date_time_ranges = self._get_date_ranges(
-            start_date=start_date, end_date=end_date)
+            start_date=start_date, end_date=end_date
+        )
         for date_time_range in date_time_ranges:
             aggregated_telemetry = self._run_aggregation(date_time_range)
             self.__telemetry_storage.store_telemetry(aggregated_telemetry)
 
     def _get_date_ranges(
-            self, start_date: date, end_date: date) -> Iterator[DateTimeRange]:
+        self, start_date: date, end_date: date
+    ) -> Iterator[DateTimeRange]:
         """
         Method to return the list of date ranges based upon start and end
         date.
         """
         generator = DATE_TIME_RANGE_GENERATOR.get(self.TO_TELEMETRY_TYPE)
         if not generator:
             raise exceptions.UnknownTelemetryType(self.TO_TELEMETRY_TYPE)
 
-        return generator(
-            start_date=start_date, end_date=end_date)
+        return generator(start_date=start_date, end_date=end_date)
 
-    def _run_aggregation(
-            self, date_time_range: DateTimeRange) -> TelemetryModel:
+    def _run_aggregation(self, date_time_range: DateTimeRange) -> TelemetryModel:
         """
         Method to run the actual aggregation and return the aggregated telemetry model.
         """
         # gather the database instances to be aggregated
-        telemetry_list_params = \
-            self._telememtry_list_params(date_time_range)._asdict()
+        telemetry_list_params = self._telememtry_list_params(date_time_range)._asdict()
         telemetry_objects = self.__telemetry_storage.telemetry_list(
-            **telemetry_list_params)
+            **telemetry_list_params
+        )
 
         initial_telemetry_obj = self.__target_telemetry.copy()
         aggregator = self.__aggregator(initial_telemetry_obj)
         aggregated_telemetry = aggregator.aggregate(telemetry_objects)
 
         return self._set_start_date_time_for_aggregated_telemetry(
-            aggregated_telemetry, date_time_range)
+            aggregated_telemetry, date_time_range
+        )
 
     @staticmethod
     def _set_start_date_time_for_aggregated_telemetry(
-            telemetry_obj: TelemetryModel,
-            date_time_range: DateTimeRange) -> TelemetryModel:
+        telemetry_obj: TelemetryModel, date_time_range: DateTimeRange
+    ) -> TelemetryModel:
         """
         Method to set the telemetry start_date_time attribute to the date_time
         for which the aggregation was run as start_date_time is set to now() by
         default.
         """
         # For daily telemetry aggregation the date of the aggregated object
         # is the from_date attribute in the date_time_range
@@ -143,31 +149,33 @@
         model.
         """
         self.__target_telemetry = TelemetryModel(
             telemetry_type=self.TO_TELEMETRY_TYPE,
             source_name=self.__telemetry_selector.source_name,
             process_type=self.__telemetry_selector.process_type,
             category=self.__telemetry_selector.category,
-            sub_category=self.__telemetry_selector.sub_category)
+            sub_category=self.__telemetry_selector.sub_category,
+        )
 
-    def _telememtry_list_params(self, date_time_range: DateTimeRange) \
-            -> TelemetryListArgs:
+    def _telememtry_list_params(
+        self, date_time_range: DateTimeRange
+    ) -> TelemetryListArgs:
         """
         Method to return telemetry_list_params that can be used to retrieve a
         list of TelemetryModel objects from the storage model.
 
         i.e. these params serve as input to the telemetry_list method of the
         storage_class
         """
         telemetry_list_params = self.__telemetry_selector._asdict()
         return TelemetryListArgs(
             telemetry_type=self.FROM_TELEMETRY_TYPE,
             from_date_time=date_time_range.from_date,
             to_date_time=date_time_range.to_date,
-            **telemetry_list_params
+            **telemetry_list_params,
         )
 
 
 class DailyAggregator(AbstractAggregator):
     """
     Aggregator to aggregate all SINGLE TELEMETRY objects for a single day
     into a telemetry objetc of type DAILY AGGREGATION.
@@ -181,16 +189,15 @@
     - aggregate_yesterday: makes daily aggregation for yesterday
     """
 
     FROM_TELEMETRY_TYPE = st.SINGLE_TELEMETRY_TYPE
     TO_TELEMETRY_TYPE = st.DAILY_AGGR_TELEMETRY_TYPE
 
     def aggregate_yesterday(self) -> None:
-        """Method to run the aggregation for yesterday.
-        """
+        """Method to run the aggregation for yesterday."""
         start_date = date.today()
         end_date = date.today() - timedelta(days=1)
         self.aggregate(start_date=start_date, end_date=end_date)
 
 
 class PartialToSingleAggregator(AbstractAggregator):
     """
@@ -200,9 +207,10 @@
     When initializig the class a TelemetrySelector should provided that
     determine which telemnetry objects are in scope
 
     The following methods are available to run the actual aggregations
 
     - aggregate: makes daily aggregations from start_date to end_date
     """
+
     FROM_TELEMETRY_TYPE = st.PARTIAL_AGGR_TELEMETRY_TYPE
     TO_TELEMETRY_TYPE = st.SINGLE_TELEMETRY_TYPE
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/aggregator/helper.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 Single day date range generators.
 - get_daily_date_ranges: free choice of start and end date
 - get_daily_date_range_till_yesterday: from start date till yesterday
 - get_daily_date_range_yesterday: date range for yesterday
 
 
 """
+
 from datetime import datetime
 from typing import NamedTuple, Protocol
 
 from pipeline_telemetry.data_classes import TelemetryModel
 
 
 class TelemetrySelector(NamedTuple):
@@ -37,14 +38,15 @@
         )
 
     The `telemtry_selector` defines what telemetry objects are in scope.
     The `aggregator` object defines what kind of aggregation is done (by
     selecting the AggregatorClass) and provides you with metods to run the
     aggergation for a specific period.
     """
+
     category: str
     sub_category: str
     source_name: str
     process_type: str
 
 
 class TelemetryListArgs(NamedTuple):
@@ -54,26 +56,22 @@
     source_name: str
     process_type: str
     from_date_time: datetime
     to_date_time: datetime
 
 
 class TelemetryList(Protocol):
-    def __next__(self) -> TelemetryModel:
-        ...
-
-    def __iter__(self) -> 'TelemetryList':
-        ...
+    def __next__(self) -> TelemetryModel: ...
 
+    def __iter__(self) -> "TelemetryList": ...
 
-class TelemetryAggregator():
 
+class TelemetryAggregator:
     __telemetry: TelemetryModel
 
     def __init__(self, telemetry: TelemetryModel) -> None:
         self.__telemetry = telemetry
 
-    def aggregate(
-            self, telemetry_list: TelemetryList) -> TelemetryModel:
+    def aggregate(self, telemetry_list: TelemetryList) -> TelemetryModel:
         for telemetry in telemetry_list:
             self.__telemetry += telemetry
         return self.__telemetry
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/aggregator/mongo_aggregator.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/mongo_aggregator.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,20 @@
             telemetry_selector=telemetry_selector
         )
 
 available classes:
 - DailyMongoAggregator
 
 """
+
 from abc import ABC
 
 from pipeline_telemetry.storage import TelemetryMongoStorage
 
-from .aggregator import AbstractAggregator, DailyAggregator, \
-    PartialToSingleAggregator
+from .aggregator import AbstractAggregator, DailyAggregator, PartialToSingleAggregator
 from .helper import TelemetrySelector
 
 
 class AbstractMongoAggregator(ABC):
     """Class to return a DailyAggregator class with TelemetryMongoStorage.
 
     When using this aggregator class the storage_class is automatically set
@@ -39,15 +39,15 @@
     """
 
     AGGREGATOR_CLASS: type[AbstractAggregator]
 
     def __new__(cls, telemetry_selector: TelemetrySelector):
         return cls.AGGREGATOR_CLASS(
             telemetry_selector=telemetry_selector,
-            telemetry_storage=TelemetryMongoStorage()
+            telemetry_storage=TelemetryMongoStorage(),
         )
 
 
 class DailyMongoAggregator(AbstractMongoAggregator):
     """Class to return a DailyAggregator class with TelemetryMongoStorage.
 
     When using this aggregator class the storage_class is automatically set
@@ -55,19 +55,21 @@
 
     >>> telemetry_selector = TelemetrySelector(
         category, sub_category, source_name, process_type)
     >>> aggeregator = DailyMongoAggregator(
             telemetry_selector=telemetry_selector
         )
     """
+
     AGGREGATOR_CLASS = DailyAggregator
 
 
 class PartialToSingleMongoAggregator(AbstractMongoAggregator):
     """
     Class to return a PartialToSingleAggregator class with
     TelemetryMongoStorage.
 
     When using this aggregator class the storage_class is automatically set
     to TelemetryMongoStorage and can not be provided as argument.
     """
+
     AGGREGATOR_CLASS = PartialToSingleAggregator
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/data_classes/telemetry_models.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/data_classes/telemetry_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 - TelemetryData: Data class to hold the actual (error)counters in a
                  TelemetryModel object
 
 - TelemetryModel: Data class to define the Telemetry object category, type,
                   source etc. Holds the reference to the actual counters defined
                   in TelemetryData dataclass.
 """
+
 from collections import defaultdict
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import DefaultDict, Dict, Optional
 
 from errors import ErrorCode
 
 from pipeline_telemetry.settings import exceptions
 from pipeline_telemetry.settings import settings as st
 
 
 @dataclass
-class TelemetryData():
+class TelemetryData:
     """
     Class to define the telemetry (error)counters.
 
     attributes:
     - base_counter (int): counter for the TelemetryData object.
     - fail_counter (int): fail counter for the TelemetryData object.
     - counters (dict): dict of sub (custom) counters [str: int]
@@ -38,114 +39,109 @@
     - increase_custom_count
     - increase_error_count
 
     counters can be added in which case base, fail, custom and error counters
     will be summed up seperately. Add method will return self with added
     TelemetryData object.
     """
+
     base_counter: int = 0
     fail_counter: int = 0
-    counters: DefaultDict[str, int] = field(
-        default_factory=lambda: defaultdict(int))
-    errors: DefaultDict[str, int] = field(
-        default_factory=lambda: defaultdict(int))
+    counters: DefaultDict[str, int] = field(default_factory=lambda: defaultdict(int))
+    errors: DefaultDict[str, int] = field(default_factory=lambda: defaultdict(int))
 
     def increase_base_count(self, increment: int) -> None:
         """Increase the base counter with a given increment."""
         self.base_counter += increment
 
     def increase_fail_count(self, increment: int) -> None:
         """Increase the fail counter with a given increment."""
         self.fail_counter += increment
 
-    def increase_error_count(
-            self, increment: int, error_code: ErrorCode) -> None:
+    def increase_error_count(self, increment: int, error_code: ErrorCode) -> None:
         """Increase an error counter with a given increment."""
 
         error_code_key = error_code.code
-        self._increase_error_count(
-            increment=increment, error_code_key=error_code_key)
+        self._increase_error_count(increment=increment, error_code_key=error_code_key)
 
-    def _increase_error_count(
-            self, increment: int, error_code_key: str) -> None:
+    def _increase_error_count(self, increment: int, error_code_key: str) -> None:
         self.errors[error_code_key] += increment
 
     def increase_custom_count(self, increment: int, counter: str) -> None:
         """Increase a custom counter with a given increment."""
         self.counters[counter] += increment
 
-    def __add__(self, telemetry_data: 'TelemetryData') -> 'TelemetryData':
+    def __add__(self, telemetry_data: "TelemetryData") -> "TelemetryData":
         """
         Add telemetry_data object to self by adding up all counters seperately.
         """
         self.increase_base_count(telemetry_data.base_counter)
         self.increase_fail_count(telemetry_data.fail_counter)
         for error_code_key, increment in telemetry_data.errors.items():
             self._increase_error_count(
-                increment=increment, error_code_key=error_code_key)
+                increment=increment, error_code_key=error_code_key
+            )
         for counter, increment in telemetry_data.counters.items():
-            self.increase_custom_count(
-                increment=increment, counter=counter)
+            self.increase_custom_count(increment=increment, counter=counter)
         return self
 
 
 @dataclass
-class TelemetryModel():
+class TelemetryModel:
     telemetry_type: str
     category: str
     sub_category: str
     source_name: str
     process_type: str
     start_date_time: datetime = datetime.now()
     run_time_in_seconds: Optional[float] = None
     io_time_in_seconds: float = 0
     traffic_light: str = st.DEFAULT_TRAFIC_LIGHT_COLOR
     telemetry: Dict[str, TelemetryData] = field(default_factory=dict)
 
     def validate(self) -> None:
         self._check_telemetry_type()
 
-    def copy(self) -> 'TelemetryModel':
+    def copy(self) -> "TelemetryModel":
         """
         Method to return a copy of the telemetry model. In a telemetry copy
         only the attributes telemetry_type, categroy, sub_category, source_name
         and process_type are copied.
         """
         return TelemetryModel(
             telemetry_type=self.telemetry_type,
             category=self.category,
             sub_category=self.sub_category,
             source_name=self.source_name,
-            process_type=self.process_type)
+            process_type=self.process_type,
+        )
 
     def _check_telemetry_type(self) -> None:
         """Check validaty of provided telemetry type.
 
         Raises exception if not valid. Returns non if telemetry type is valid.
 
         Args:
             telemetry_type (str): [description]
 
         Raises:
             exceptions.InvalidTelemetryType: When telemetry type is not valid.
         """
         if self.telemetry_type not in st.TELEMETRY_TYPES:
-            raise exceptions.InvalidTelemetryType(
-                st.TELEMETRY_TYPES)
+            raise exceptions.InvalidTelemetryType(st.TELEMETRY_TYPES)
 
     def set_orange_traffic_light(self) -> None:
         """Sets traffic light attribute to orange."""
         self.traffic_light = st.TRAFIC_LIGHT_COLOR_ORANGE
 
     def set_red_traffic_light(self) -> None:
         """Sets traffic light attribute to red."""
         self.traffic_light = st.TRAFIC_LIGHT_COLOR_RED
 
-    def __add__(
-            self, telemetry_model_to_add: 'TelemetryModel') -> 'TelemetryModel':
+    def __add__(self, telemetry_model_to_add: "TelemetryModel") -> "TelemetryModel":
         """
         Method to add to telementry model instances.
         Adding a 2 telemetry model instances implies adding all telemetry data
         objects and adding iotime, run time and traffic light attributes to a
         specific counter.
         """
         self.__add_base_count()
@@ -156,56 +152,55 @@
         return self
 
     def __add_base_count(self) -> None:
         """
         Sub method for the __add__ method to increase base_counter of the
         aggregation sub_process when adding TelemetryModel instances.
         """
-        self.get_sub_process_data(
-            sub_process=st.AGGREGATION_KEY).increase_base_count(increment=1)
+        self.get_sub_process_data(sub_process=st.AGGREGATION_KEY).increase_base_count(
+            increment=1
+        )
 
-    def __add_traffic_light(
-            self, telemetry_model_to_add: 'TelemetryModel') -> None:
+    def __add_traffic_light(self, telemetry_model_to_add: "TelemetryModel") -> None:
         """
         Sub method for the __add__ method to add the traffic_light value of the
         TelemetryModel instance to be added to the aggregation sub_process.
         """
-        self.get_sub_process_data(
-            sub_process=st.AGGREGATION_KEY).increase_custom_count(
-                increment=1, counter=telemetry_model_to_add.traffic_light)
+        self.get_sub_process_data(sub_process=st.AGGREGATION_KEY).increase_custom_count(
+            increment=1, counter=telemetry_model_to_add.traffic_light
+        )
 
-    def __add_sub_process(
-            self, telemetry_model_to_add: 'TelemetryModel') -> None:
+    def __add_sub_process(self, telemetry_model_to_add: "TelemetryModel") -> None:
         """
         Sub method for the __add__ method to add the sub_processes of the two
         TelemetryModel instances.
         """
         for sub_process in telemetry_model_to_add.telemetry:
             sub_pr = self.get_sub_process_data(sub_process)
             sub_pr += telemetry_model_to_add.get_sub_process_data(
-                sub_process=sub_process)
+                sub_process=sub_process
+            )
 
-    def __add_io_time(self, telemetry_model_to_add: 'TelemetryModel') -> None:
+    def __add_io_time(self, telemetry_model_to_add: "TelemetryModel") -> None:
         """
         Sub method for the __add__ method to add the rounded io_time of the
         TelemetryModel instance to be added to the aggregation sub_process.
         """
-        self.get_sub_process_data(
-            sub_process=st.AGGREGATION_KEY).increase_custom_count(
-                increment=round(telemetry_model_to_add.io_time_in_seconds),
-                counter=st.IO_TIME_KEY)
+        self.get_sub_process_data(sub_process=st.AGGREGATION_KEY).increase_custom_count(
+            increment=round(telemetry_model_to_add.io_time_in_seconds),
+            counter=st.IO_TIME_KEY,
+        )
 
-    def __add_run_time(self, telemetry_model_to_add: 'TelemetryModel') -> None:
+    def __add_run_time(self, telemetry_model_to_add: "TelemetryModel") -> None:
         """
         Sub method for the __add__ method to add the rounded run_time of the
         TelemetryModel instance to be added to the aggregation sub_process.
         """
         run_time_in_seconds = telemetry_model_to_add.run_time_in_seconds or 0
-        self.get_sub_process_data(
-            sub_process=st.AGGREGATION_KEY).increase_custom_count(
-                increment=round(run_time_in_seconds),
-                counter=st.RUN_TIME)
+        self.get_sub_process_data(sub_process=st.AGGREGATION_KEY).increase_custom_count(
+            increment=round(run_time_in_seconds), counter=st.RUN_TIME
+        )
 
     def get_sub_process_data(self, sub_process: str) -> TelemetryData:
         if not self.telemetry.get(sub_process):
             self.telemetry[sub_process] = TelemetryData()
         return self.telemetry[sub_process]
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/decorator.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 decorators:
     - add_telemetry
     - add_mongo_telemetry
     - add_single_usage_telemetry
     - add_mongo_single_usage_telemetry
 """
+
 from functools import wraps
-from typing import Type
+from typing import Callable, Optional, Type
 
 from .main import Telemetry
 from .settings import exceptions
 from .storage import AbstractTelemetryStorage, TelemetryMongoStorage
 
 
-def add_telemetry(telemetry_params: dict) -> object:
+def add_telemetry(telemetry_params: dict) -> Callable:
     """
     Decorator method to add a telemetry to the class from which the
     decorator was called. When using this decorator the storage
     class can be set as wanted but defaults to TelemetryInMemoryStorage.
 
     Args:
         telemetry_params (dict:
@@ -47,15 +48,15 @@
             return result
 
         return wrapped_method
 
     return wrapper
 
 
-def add_mongo_telemetry(telemetry_params: dict) -> object:
+def add_mongo_telemetry(telemetry_params: dict) -> Callable:
     """
     Decorator method to add a telemetry to the class from which the
     decorator was called. When using this decorator the mongo storage
     class will used.
 
     Args:
         telemetry_params (dict:
@@ -67,30 +68,31 @@
     def wrapper(method):
         @wraps(method)
         def wrapped_method(self, *args, **kwargs):
             """
             Wrapper for method where result log should be added
             """
             if (not hasattr(self, "_telemetry")) or (not self._telemetry):
-                tel_params = telemetry_params.copy() | \
-                    {'storage_class': TelemetryMongoStorage}
+                tel_params = telemetry_params.copy() | {
+                    "storage_class": TelemetryMongoStorage
+                }
                 self._telemetry = Telemetry(**tel_params)
                 result = method(self, *args, **kwargs)
                 self._telemetry.save_and_close()
                 self._telemetry = None
             else:
                 result = method(self, *args, **kwargs)
             return result
 
         return wrapped_method
 
     return wrapper
 
 
-def add_mongo_single_usage_telemetry(sub_process: str = None) -> object:
+def add_mongo_single_usage_telemetry(sub_process: Optional[str] = None) -> object:
     """
     Decorator method to add a telemetry to the class from which the
     decorator was called. The telemetry object will be reset each the method
     initiating the telemetry object will be called. This method should be used
     for stand alone telemetry measurements like for example external API calls.
     It can be used to easily store a single event telemetry object.
 
@@ -100,22 +102,22 @@
         - sub_process (str, Optional):
             one of the sub_processes defined with the process_type. A
             counter with value 1 will be created for this sub_process.
             This field is optional, if not provided no counter will be
             added to the telemetry object
     """
     return add_single_usage_telemetry(
-        sub_process=sub_process,
-        storage_class=TelemetryMongoStorage
+        sub_process=sub_process, storage_class=TelemetryMongoStorage
     )
 
 
 def add_single_usage_telemetry(
-        sub_process: str = None,
-        storage_class: Type[AbstractTelemetryStorage] = None) -> object:
+    sub_process: Optional[str] = None,
+    storage_class: Optional[Type[AbstractTelemetryStorage]] = None,
+) -> object:
     """
     Decorator method to add a telemetry to the class from which the
     decorator was called. The telemetry object will be reset each the method
     initiating the telemetry object will be called. This method should be used
     for stand alone telemetry measurements like for example external API calls.
     It can be used to easily store a single event telemetry object.
 
@@ -131,29 +133,32 @@
 
     def wrapper(method):
         @wraps(method)
         def wrapped_method(self, *args, **kwargs):
             """
             Wrapper for method where result log should be added
             """
-            telemetry_params = getattr(self, 'TELEMETRY_PARAMS', False)
+            telemetry_params = getattr(self, "TELEMETRY_PARAMS", False)
             if not telemetry_params:
                 raise exceptions.ClassTelemetryParamsNotDefined(self)
 
-            storage_class_params = \
-                {'storage_class': storage_class} if storage_class else {}
+            if not isinstance(telemetry_params, dict):
+                raise exceptions.ClassTelemetryParamsNotOfTypeDict(self)
+
+            storage_class_params = (
+                {"storage_class": storage_class} if storage_class else {}
+            )
 
             tel_params = telemetry_params | storage_class_params
             self._telemetry = Telemetry(**tel_params)
 
             # only if sub_process was defined set the base count for that
             # subprocess
             if sub_process:
-                self._telemetry.increase_sub_process_base_count(
-                    sub_process=sub_process)
+                self._telemetry.increase_sub_process_base_count(sub_process=sub_process)
             result = method(self, *args, **kwargs)
             self._telemetry.save_and_close()
             self._telemetry = None
 
             return result
 
         return wrapped_method
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/helper.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/helper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""Helper module for pipeline_telemetry
-"""
+"""Helper module for pipeline_telemetry"""
+
 from typing import Any, List, Union
 
 from errors import ReturnValueWithStatus
 
 from .settings import exceptions
 from .settings import settings as st
 from .settings.data_class import TelemetryCounter
@@ -11,28 +11,28 @@
 
 def is_telemetry_counter(counter: Union[TelemetryCounter, Any]) -> bool:
     """Method to check in object is an instance of TelemetryCounter."""
     return issubclass(counter.__class__, TelemetryCounter)
 
 
 def add_errors_from_return_value(
-        object_with_telemetry: Any, sub_process: str,
-        return_value: ReturnValueWithStatus) -> None:
+    object_with_telemetry: Any, sub_process: str, return_value: ReturnValueWithStatus
+) -> None:
     """
     Helper method to add the errors from a ReturnValueWithStatus instance to the
     telemetry instance of the object_with_telemetry.
     """
     object_with_telemetry._telemetry.add(
-        sub_process=sub_process,
-        data=[], errors=return_value.errors)
+        sub_process=sub_process, data=[], errors=return_value.errors
+    )
 
 
 def add_telemetry_counters_from_return_value(
-        object_with_telemetry: Any,
-        return_value: ReturnValueWithStatus) -> List[Any]:
+    object_with_telemetry: Any, return_value: ReturnValueWithStatus
+) -> List[Any]:
     """
     Helper method to add the TelemetryCounters from a ReturnValueWithStatus
     instance to the telemetry instance of the object_with_telemetry.
     """
     result_without_telemetry_counters = []
     for item in return_value.result:
         if is_telemetry_counter(item):
@@ -40,35 +40,33 @@
         else:
             result_without_telemetry_counters.append(item)
 
     return result_without_telemetry_counters
 
 
 def process_return_value(
-        object_with_telemetry: Any, sub_process: str,
-        return_value: ReturnValueWithStatus) -> List[Any]:
+    object_with_telemetry: Any, sub_process: str, return_value: ReturnValueWithStatus
+) -> List[Any]:
     """Processes a return value object.
     All errors and telemetry counters in return_value errors and result list
     will be processed and added to the telemetry object in
     object_with_telemetry. All the other values in the result list are then
     returned as a list.
 
     Args:
         object_with_telemetry (Any): _description_
         sub_process (str): _description_
         return_value (ReturnValueWithStatus): _description_
 
     Returns:
         List[Any]: _description_
     """
-    add_errors_from_return_value(
-        object_with_telemetry, sub_process, return_value)
+    add_errors_from_return_value(object_with_telemetry, sub_process, return_value)
 
-    return add_telemetry_counters_from_return_value(
-        object_with_telemetry, return_value)
+    return add_telemetry_counters_from_return_value(object_with_telemetry, return_value)
 
 
 def increase_base_count(
     object_with_telemetry: Any, sub_process: str, increment: int = 1
 ) -> None:
     """
     Helper method to increase base count for a sub_process
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/main.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Module to provide Telemetry class as public class to be accessed
 
 classes
     - Telemetry
 
 """
+
 from datetime import datetime
 from typing import Dict, List, Optional, Type
 
 from errors import ErrorCode
 
 from .data_classes.telemetry_models import TelemetryData, TelemetryModel
 from .helper import _raise_exception_if_telemetry_closed
@@ -17,48 +18,47 @@
 from .settings.data_class import ProcessType, TelemetryCounter
 from .settings.process_type import ProcessTypes
 from .storage.generic import AbstractTelemetryStorage
 from .storage.memory import TelemetryInMemoryStorage
 from .validators.dict_validator import DictValidator
 
 
-class Telemetry():
+class Telemetry:
     _telemetry: TelemetryModel
     _telemetry_rules: dict
     _storage_class: Type[AbstractTelemetryStorage]
     _available_process_types: Type[ProcessTypes] = ProcessTypes
     _process_type: ProcessType
     _available_telemetry_types = st.TELEMETRY_TYPES
 
     def __init__(
         self,
         category: str,
         sub_category: str,
         source_name: str,
         process_type: ProcessType,
         telemetry_type: str = st.DEFAULT_TELEMETRY_TYPE,
-        telemetry_rules: dict = dict(),
-        storage_class:
-            Type[AbstractTelemetryStorage] = TelemetryInMemoryStorage,
+        telemetry_rules: Optional[dict] = None,
+        storage_class: Type[AbstractTelemetryStorage] = TelemetryInMemoryStorage,
     ):
         self._process_type = process_type
         self._validate_process_type()
         self._storage_class = storage_class
-        self._telemetry_rules = telemetry_rules
+        self._telemetry_rules = telemetry_rules or {}
         self._telemetry = TelemetryModel(
             telemetry_type=telemetry_type,
             category=category,
             sub_category=sub_category,
             source_name=source_name,
-            process_type=process_type.name)
+            process_type=process_type.name,
+        )
         self._telemetry.validate()
 
     @classmethod
-    def add_process_type(cls, process_type_key: str, process_type: ProcessType
-                         ) -> None:
+    def add_process_type(cls, process_type_key: str, process_type: ProcessType) -> None:
         """
         Add a custom process type to the available process types to the
         already registered process types.
 
         Args:
             process_type (ProcessType): Process type that needs to be added
             process_type_key (str): key that should be used when calling this
@@ -145,16 +145,16 @@
             raise exceptions.TelemetryObjectAlreadyClosed()
         self._set_runtime()
         self._storage_class().store_telemetry(self.telemetry)
 
         return self.telemetry
 
     def add_telemetry_counter(
-            self, telemetry_counter: TelemetryCounter,
-            increment: Optional[int] = None) -> None:
+        self, telemetry_counter: TelemetryCounter, increment: Optional[int] = None
+    ) -> None:
         """
         Method to process a TelemetryCounter object with predefined counters.
 
         Args:
             telemetry_counter (TelemetryCounter): [description]
             increment (int, None):
                 when not None overules the increment setting from
@@ -179,16 +179,15 @@
             self.increase_sub_process_custom_count(
                 sub_process=sub_process,
                 custom_counter=counter_name,
                 increment=increment,
             )
 
     @_raise_exception_if_telemetry_closed
-    def add(self, sub_process: str, data: dict, errors: List[ErrorCode]
-            ) -> None:
+    def add(self, sub_process: str, data: dict, errors: List[ErrorCode]) -> None:
         """
         Add data validation errors and/or errors from data process to a
         telemetry sub process.
         Data validation errors are retrieved from data validation defined in
         telemetry rules.
 
         Method does not update BASE_COUNT.
@@ -233,15 +232,16 @@
         :typesub_process: str
         :param errors: errors to be processed
         :type errors: list of Errorcodes
         :returns: None
         """
         for error_code in errors:
             self.increase_sub_process_error_count(
-                error_code=error_code, sub_process=sub_process)
+                error_code=error_code, sub_process=sub_process
+            )
 
     @_raise_exception_if_telemetry_closed
     def set_orange_traffic_light(self) -> None:
         """Sets traffic light attribute to orange."""
         self.telemetry.set_orange_traffic_light()
 
     @_raise_exception_if_telemetry_closed
@@ -282,29 +282,31 @@
         """
         current_io_time = getattr(self._telemetry, st.IO_TIME_KEY)
         increased_io_time = current_io_time + incremental_io_time
         setattr(self._telemetry, st.IO_TIME_KEY, increased_io_time)
 
     @_raise_exception_if_telemetry_closed
     def increase_sub_process_base_count(
-            self, sub_process: str, increment: int = 1) -> None:
+        self, sub_process: str, increment: int = 1
+    ) -> None:
         """
         Increases the base count for a subprocess.
 
         Args:
             sub_process (str): name of subprocess
         """
         if self._sub_process_not_yet_initialized(sub_process):
             self._initialize_sub_process(sub_process)
 
         self.get(sub_process).increase_base_count(increment)
 
     @_raise_exception_if_telemetry_closed
     def increase_sub_process_fail_count(
-            self, sub_process: str, increment: int = 1) -> None:
+        self, sub_process: str, increment: int = 1
+    ) -> None:
         """
         Increases the fail count for a subprocess.
 
         Args:
             sub_process (str): name of subprocess
         """
         if self._sub_process_not_yet_initialized(sub_process):
@@ -328,19 +330,20 @@
             BaseCountForSubProcessNotAdded: if subprocess has not yet been
                                             created
         """
         if self._sub_process_not_yet_initialized(sub_process):
             raise exceptions.BaseCountForSubProcessNotAdded(sub_process)
 
         self.get(sub_process).increase_error_count(
-            increment=increment, error_code=error_code)
+            increment=increment, error_code=error_code
+        )
 
     @_raise_exception_if_telemetry_closed
     def increase_sub_process_custom_count(
-            self, custom_counter: str, sub_process: str, increment: int = 1
+        self, custom_counter: str, sub_process: str, increment: int = 1
     ) -> None:
         """
         Increases a custom counter for a subprocess.
 
         Args:
             sub_process (str): name of subprocess
             custom_counter (str): name of custom counter
@@ -350,15 +353,16 @@
             BaseCountForSubProcessNotAdded: if subprocess has not yet been
                                             created
         """
         if self._sub_process_not_yet_initialized(sub_process):
             self._initialize_sub_process(sub_process)
 
         self.get(sub_process).increase_custom_count(
-            increment=increment, counter=custom_counter)
+            increment=increment, counter=custom_counter
+        )
 
     def _sub_process_is_initialized(self, sub_process: str) -> bool:
         """Returns True if provided sub_process is initialized
 
         Args:
             sub_process (str): sub_process
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/mixin.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 """
 Module to define TelemetryMixin class for adding methods to
 a class that allow easy Telemetry updates
 """
+
 from typing import Any, List, Union
 
 from errors import ReturnValueWithStatus
 
-from .helper import add_errors_from_return_value, \
-    add_telemetry_counters_from_return_value
+from .helper import (
+    add_errors_from_return_value,
+    add_telemetry_counters_from_return_value,
+)
 from .main import Telemetry
 from .settings.data_class import TelemetryCounter
 
 
-class TelemetryMixin():
-
+class TelemetryMixin:
     _telemetry: Telemetry
 
     def process_errors_from_return_value(
-            self, sub_process: str,
-            return_value: ReturnValueWithStatus) -> None:
+        self, sub_process: str, return_value: ReturnValueWithStatus
+    ) -> None:
         """
         Adds errors from return_value to _telemetry object for a specific
         sub_process.
 
         Args:
             sub_process (str):
                 One of the sub_processed defined in process type for this
                 telemetry object.
             return_value (ReturnValueWithStatus):
                 Return value object containing the errors
         """
         add_errors_from_return_value(
             object_with_telemetry=self,
             sub_process=sub_process,
-            return_value=return_value)
+            return_value=return_value,
+        )
 
     def process_telemetry_counters_from_return_value(
-            self, return_value: ReturnValueWithStatus) -> List[Any]:
+        self, return_value: ReturnValueWithStatus
+    ) -> List[Any]:
         """
         Adds TelemetryCounters from return_value to _telemetry object for a
         specific sub_process.
 
         Args:
             return_value (ReturnValueWithStatus):
                 Return value object containing the errors
@@ -48,19 +52,20 @@
         Returns:
             List:
                 List with all value from return_value.result that are not of
                 type TelemetryCounter. I.e. all the result entries that are not
                 processed by this method.
         """
         return add_telemetry_counters_from_return_value(
-            object_with_telemetry=self,
-            return_value=return_value)
+            object_with_telemetry=self, return_value=return_value
+        )
 
     def process_telemetry_counters_from_list(
-            self, result_list: List[Union[Any, TelemetryCounter]]) -> list[Any]:
+        self, result_list: List[Union[Any, TelemetryCounter]]
+    ) -> list[Any]:
         """
         Adds TelemetryCounters from result_list to _telemetry object.
 
         Args:
             result_list ([Any, TelemetryCounter]):
                 Result list containing data objects (not processed) and
                 Telemetry counters
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/settings/data_class.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/data_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""[summary]
-"""
+"""[summary]"""
+
 from dataclasses import dataclass, field
 from typing import Any, List, Optional
 
 from errors import ErrorCode
 
 from pipeline_telemetry.settings import exceptions
 
@@ -34,27 +34,30 @@
     process_types: Optional[List[ProcessType]] = None
     process_type: Optional[ProcessType] = None
     counter_name: Optional[str] = None
     increment: int = 1
     error: Optional[ErrorCode] = None
 
     def __hash__(self):
-        hash_list = [process_type.process_type for process_type
-                     in self.process_types or []]
+        hash_list = [
+            process_type.process_type for process_type in self.process_types or []
+        ]
         hash_list.append(self.sub_process)
         if self.process_type:
             hash_list.append(self.process_type.process_type)
         if self.counter_name:
             hash_list.append(self.counter_name)
         if self.error:
             hash_list.append(self.error.code)
         hash_list.append(str(self.increment))
         return hash(tuple(hash_list))
 
-    def add_to(self, object_with_telemetry: Any, increment: int = None) -> None:
+    def add_to(
+        self, object_with_telemetry: Any, increment: Optional[int] = None
+    ) -> None:
         """
         Method to add to add self (the TelemetryCounter) to an object telemetry
         instance
         """
         object_with_telemetry._telemetry.add_telemetry_counter(
             telemetry_counter=self, increment=increment
         )
@@ -77,18 +80,17 @@
         Returns:
             List[ProcessType]: list with process_types
         """
         all_process_types = [self.process_type]
         if self.process_types:
             all_process_types.extend(self.process_types)
 
-        return [
-            process_type for process_type in all_process_types if process_type]
+        return [process_type for process_type in all_process_types if process_type]
 
-    def set_increment(self, increment: int):
+    def set_increment(self, increment: int) -> "TelemetryCounter":
         """Returns same telemetry counter with a new increment."""
         return TelemetryCounter(
             sub_process=self.sub_process,
             process_types=self.process_types,
             process_type=self.process_type,
             counter_name=self.counter_name,
             increment=increment,
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/settings/date_ranges.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/date_ranges.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,114 +1,103 @@
-"""
-"""
+""" """
+
 from datetime import date, datetime, timedelta
 from typing import Iterator, NamedTuple
 
 
 class DateRange(NamedTuple):
     from_date: date
     to_date: date
 
 
 class DateTimeRange(NamedTuple):
     from_date: datetime
     to_date: datetime
 
 
-def date_range_to_date_time_range(
-        date_range: DateRange) -> DateTimeRange:
+def date_range_to_date_time_range(date_range: DateRange) -> DateTimeRange:
     start_date, end_date = date_range
     start_date_time = datetime(*start_date.timetuple()[:6])
     end_date_time = datetime(*end_date.timetuple()[:6])
     return DateTimeRange(start_date_time, end_date_time)
 
 
 def date_range_generator(
-        start_date_time: datetime,
-        end_date_time: datetime,
-        time_delta: timedelta) -> Iterator[DateTimeRange]:
+    start_date_time: datetime, end_date_time: datetime, time_delta: timedelta
+) -> Iterator[DateTimeRange]:
     """Iterator for a list of DateTimeRange object
 
     Args:
         start_date_time (datetime): start date
         end_date_time (datetime): end date
         time_delta (timedelta): lengt of date time range
 
     The resulting date
     Yields:
         Iterator[DateTimeRange]: _description_
     """
     start_date = start_date_time.date()
     end_date = start_date + time_delta
     while end_date <= end_date_time.date():
-        yield date_range_to_date_time_range(
-            DateRange(start_date, end_date))
+        yield date_range_to_date_time_range(DateRange(start_date, end_date))
         start_date, end_date = end_date, end_date + time_delta
 
 
-def get_daily_date_ranges(
-        start_date: date, end_date: date) -> Iterator[DateTimeRange]:
+def get_daily_date_ranges(start_date: date, end_date: date) -> Iterator[DateTimeRange]:
     """
     Iterator to return single day date ranges from start_date to end_date.
     """
     start_date_time = datetime(*start_date.timetuple()[:6])
     end_date_time = datetime(*end_date.timetuple()[:6])
     return date_range_generator(
         start_date_time=start_date_time,
         end_date_time=end_date_time,
-        time_delta=timedelta(days=1)
+        time_delta=timedelta(days=1),
     )
 
 
-def get_daily_date_range_till_yesterday(
-        start_date: date) -> Iterator[DateTimeRange]:
+def get_daily_date_range_till_yesterday(start_date: date) -> Iterator[DateTimeRange]:
     """
     Iterator to return single day date ranges from start_date till yesterday.
     """
     end_date = date.today()
-    return get_daily_date_ranges(
-        start_date=start_date, end_date=end_date
-    )
+    return get_daily_date_ranges(start_date=start_date, end_date=end_date)
 
 
 def get_daily_date_range_yesterday() -> Iterator[DateTimeRange]:
     """
     Iterator to return single day date ranges for yesterday.
     """
     end_date = date.today()
     start_date = date.today() - timedelta(days=1)
-    return get_daily_date_ranges(
-        start_date=start_date, end_date=end_date
-    )
+    return get_daily_date_ranges(start_date=start_date, end_date=end_date)
 
 
-def get_daily_date_range_for_single_date(
-        date: date) -> DateTimeRange:
+def get_daily_date_range_for_single_date(date: date) -> DateTimeRange:
     """
     Return single daily date range for a given date.
     """
-    return next(get_daily_date_ranges(
-        start_date=date, end_date=date + timedelta(days=1)
-    ))
+    return next(
+        get_daily_date_ranges(start_date=date, end_date=date + timedelta(days=1))
+    )
 
 
-def get_monthly_date_range_for_single_date(
-        date: date) -> DateTimeRange:
+def get_monthly_date_range_for_single_date(date: date) -> DateTimeRange:
     """
     Return single monthly date range for a given date.
     """
     first_day_of_month = date.replace(day=1)
-    first_day_next_month = (
-        date.replace(day=1) + timedelta(days=32)).replace(day=1)
+    first_day_next_month = (date.replace(day=1) + timedelta(days=32)).replace(day=1)
     return date_range_to_date_time_range(
-        DateRange(from_date=first_day_of_month, to_date=first_day_next_month))
+        DateRange(from_date=first_day_of_month, to_date=first_day_next_month)
+    )
 
 
-def get_weekly_date_range_for_single_date(
-        date: date) -> DateTimeRange:
+def get_weekly_date_range_for_single_date(date: date) -> DateTimeRange:
     """
     Return single weekly date range for a given date.
     """
     first_day_of_week = date - timedelta(days=date.weekday())
     first_day_next_week = first_day_of_week + timedelta(days=7)
     return date_range_to_date_time_range(
-        DateRange(from_date=first_day_of_week, to_date=first_day_next_week))
+        DateRange(from_date=first_day_of_week, to_date=first_day_next_week)
+    )
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/settings/exceptions.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 - BaseCountForSubProcessNotAdded
 - TelemetryObjectAlreadyClosed
 - StorageClassOfIncorrectType
 - ProcessTypeMustBeOfClassProcessType
 - ProcessTypeNotRegistered
 - RequestedDataTimeRangeMethodNotFound
 """
+
 from typing import List
 
 
 class UnknownTelemetryType(Exception):
     """custom exception for Telemetry Module"""
 
     def __init__(self, telemetry_type):
-        message = \
-            f"Unknown telemetry_type `{telemetry_type}` used in aggregator"
+        message = f"Unknown telemetry_type `{telemetry_type}` used in aggregator"
         super().__init__(message)
 
 
 class FieldNameMandatory(Exception):
     """custom exception for Telemetry Module"""
 
     def __init__(self, instruction):
@@ -84,16 +84,15 @@
         super().__init__(message)
 
 
 class SubProcessAlreadyInitialized(Exception):
     """custom exception for Telemetry Module"""
 
     def __init__(self, sub_process: str):
-        message = \
-            f"Sub Process `{sub_process}` already initialized."
+        message = f"Sub Process `{sub_process}` already initialized."
         super().__init__(message)
 
 
 class InvalidSubProcess(Exception):
     """custom exception for Telemetry Module"""
 
     def __init__(self, sub_process: str, process_type):
@@ -177,25 +176,31 @@
     def __init__(self):
         message = "Provided sub process is not defined in ProcessType."
         super().__init__(message)
 
 
 class InvalidTelemetryType(Exception):
     def __init__(self, available_types: List[str]):
-        message = \
-            f"Telemetry Type must be of type: {', '.join(available_types)}."
+        message = f"Telemetry Type must be of type: {', '.join(available_types)}."
         super().__init__(message)
 
 
 class ClassTelemetryParamsNotDefined(Exception):
     def __init__(self, object):
         class_name = object.__class__.__name__
-        message = \
-            f"Telemetry params not defined for class {class_name}"
+        message = f"Telemetry params not defined for class {class_name}"
+        super().__init__(message)
+
+
+class ClassTelemetryParamsNotOfTypeDict(Exception):
+    def __init__(self, object):
+        class_name = object.__class__.__name__
+        message = (
+            f"Telemetry params defined for class {class_name} must be a of type dict."
+        )
         super().__init__(message)
 
 
 class RequestedDataTimeRangeMethodNotFound(Exception):
     def __init__(self, telemetry_aggr_type: str):
-        message = \
-            f"No date_time_range method found for {telemetry_aggr_type}."
+        message = f"No date_time_range method found for {telemetry_aggr_type}."
         super().__init__(message)
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/settings/process_type.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/process_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 """Module to define ProcesTypes class."""
+
 from typing import List, Type
 
 from pipeline_telemetry.settings import exceptions
 from pipeline_telemetry.settings.data_class import ProcessType
 from pipeline_telemetry.settings.settings import BaseEnumerator
 
 
-class ProcessTypes():
+class ProcessTypes:
     """Singleton Class for registering process_types"""
 
     _process_types: List[ProcessType] = []
 
     def __new__(cls):
         return cls
 
     @classmethod
     def register_process_type(
-            cls, process_type_key: str, process_type: ProcessType) -> None:
+        cls, process_type_key: str, process_type: ProcessType
+    ) -> None:
         """Class method to register a single process type."""
         if not isinstance(process_type, ProcessType):
             raise exceptions.ProcessTypeMustBeOfClassProcessType
         setattr(cls, process_type_key, process_type)
         cls._process_types.append(process_type)
 
     @classmethod
-    def register_process_types(
-            cls, process_types: Type[BaseEnumerator]) -> None:
+    def register_process_types(cls, process_types: Type[BaseEnumerator]) -> None:
         """Class method to register new errors from enumerator."""
         try:
             if not issubclass(process_types, BaseEnumerator):
                 raise exceptions.ProcessTypesMustBeOfClassBaseEnumertor
         except TypeError:
             raise exceptions.ProcessTypesMustBeOfClassBaseEnumertor
 
         for process_type_key in process_types.keys():
             process_type = getattr(process_types, process_type_key).value
             cls.register_process_type(
-                process_type_key=process_type_key, process_type=process_type)
+                process_type_key=process_type_key, process_type=process_type
+            )
 
     @classmethod
     def is_registered(cls, process_type: ProcessType) -> bool:
         """Method checks of a process_type is registered.
 
         Args:
             process_type (ProcessType): ProcessType instance to be checked
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/settings/settings.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,47 @@
-"""[summary]
-"""
+"""[summary]"""
+
 from enum import Enum
 from typing import Callable, Dict, List
 
 import pipeline_telemetry.settings.date_ranges as dr
 from pipeline_telemetry.settings.data_class import ProcessType
 
-SINGLE_TELEMETRY_TYPE = 'SINGLE TELEMETRY'
-DAILY_AGGR_TELEMETRY_TYPE = 'DAILY AGGREGATION'
-WEEKLY_AGGR_TELEMETRY_TYPE = 'WEEKLY AGGREGATION'
-MONTHLY_AGGR_TELEMETRY_TYPE = 'MONTHLY AGGREGATION'
-QUARTERLY_AGGR_TELEMETRY_TYPE = 'QUARTERLY AGGREGATION'
-PARTIAL_AGGR_TELEMETRY_TYPE = 'PARTIAL AGGREGATION'
+SINGLE_TELEMETRY_TYPE = "SINGLE TELEMETRY"
+DAILY_AGGR_TELEMETRY_TYPE = "DAILY AGGREGATION"
+WEEKLY_AGGR_TELEMETRY_TYPE = "WEEKLY AGGREGATION"
+MONTHLY_AGGR_TELEMETRY_TYPE = "MONTHLY AGGREGATION"
+QUARTERLY_AGGR_TELEMETRY_TYPE = "QUARTERLY AGGREGATION"
+PARTIAL_AGGR_TELEMETRY_TYPE = "PARTIAL AGGREGATION"
 
 # Constant to define date_range method specific to a given
 # TELEMETRY aggregation type
 AGGR_DATE_TIME_RANGE_METHODS: dict[str, Callable] = {
     DAILY_AGGR_TELEMETRY_TYPE: dr.get_daily_date_range_for_single_date,
     WEEKLY_AGGR_TELEMETRY_TYPE: dr.get_weekly_date_range_for_single_date,
-    MONTHLY_AGGR_TELEMETRY_TYPE: dr.get_monthly_date_range_for_single_date}
+    MONTHLY_AGGR_TELEMETRY_TYPE: dr.get_monthly_date_range_for_single_date,
+}
 
 DEFAULT_TELEMETRY_TYPE = SINGLE_TELEMETRY_TYPE
 TELEMETRY_TYPES: List[str] = [
-    PARTIAL_AGGR_TELEMETRY_TYPE, DEFAULT_TELEMETRY_TYPE,
-    DAILY_AGGR_TELEMETRY_TYPE, WEEKLY_AGGR_TELEMETRY_TYPE,
-    MONTHLY_AGGR_TELEMETRY_TYPE, QUARTERLY_AGGR_TELEMETRY_TYPE]
-
-telemetry_types: Dict[str, str] = \
-    {type.upper().replace(' ', '_'): type.upper() for type in TELEMETRY_TYPES}
-
-TRAFIC_LIGHT_COLOR_GREEN = 'GREEN'
-TRAFIC_LIGHT_COLOR_ORANGE = 'ORANGE'
-TRAFIC_LIGHT_COLOR_RED = 'RED'
+    PARTIAL_AGGR_TELEMETRY_TYPE,
+    DEFAULT_TELEMETRY_TYPE,
+    DAILY_AGGR_TELEMETRY_TYPE,
+    WEEKLY_AGGR_TELEMETRY_TYPE,
+    MONTHLY_AGGR_TELEMETRY_TYPE,
+    QUARTERLY_AGGR_TELEMETRY_TYPE,
+]
+
+telemetry_types: Dict[str, str] = {
+    type.upper().replace(" ", "_"): type.upper() for type in TELEMETRY_TYPES
+}
+
+TRAFIC_LIGHT_COLOR_GREEN = "GREEN"
+TRAFIC_LIGHT_COLOR_ORANGE = "ORANGE"
+TRAFIC_LIGHT_COLOR_RED = "RED"
 DEFAULT_TRAFIC_LIGHT_COLOR: str = TRAFIC_LIGHT_COLOR_GREEN
 
 
 BASE_COUNT_KEY = "base_counter"
 ERRORS_KEY = "errors"
 COUNTERS_KEY = "counters"
 FAIL_COUNT_KEY = "fail_counter"
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/settings/telemetry_errors.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/telemetry_errors.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,47 @@
-"""Module to define errors
-"""
+"""Module to define errors"""
+
 from errors import ErrorCode
 from errors.base import FunctionalErrorsBaseClass
 
 
 class ValidationErrors(FunctionalErrorsBaseClass):
     """
     Class to define enumerator errors for Error module
     """
+
     KEY_NOT_FOUND = ErrorCode(
-        code='HAS_KEY_ERR_0001',
-        description='Key missing in provided dict')
+        code="HAS_KEY_ERR_0001", description="Key missing in provided dict"
+    )
 
     FIELD_NOT_FOUND = ErrorCode(
-        code='VALIDATE_ENTRIES_ERR_001',
-        description='Field that needs counting can not be found')
+        code="VALIDATE_ENTRIES_ERR_001",
+        description="Field that needs counting can not be found",
+    )
 
     WRONG_TYPE_IN_FIELD = ErrorCode(
-        code='VALIDATE_ENTRIES_ERR_002',
-        description='Field does not contain dict or list')
+        code="VALIDATE_ENTRIES_ERR_002",
+        description="Field does not contain dict or list",
+    )
 
     UNEXPECTED_NR_OF_ITEMS = ErrorCode(
-        code='VALIDATE_ENTRIES_ERR_003',
-        description='Field contains unexpected nr of items')
+        code="VALIDATE_ENTRIES_ERR_003",
+        description="Field contains unexpected nr of items",
+    )
 
     ENTRIES_FIELD_NOT_FOUND = ErrorCode(
-        code='ENTRIES_HAVE_KEY_ERR_001',
-        description='Entries field does not exist')
+        code="ENTRIES_HAVE_KEY_ERR_001", description="Entries field does not exist"
+    )
 
     ENTRIES_FIELD_OF_WRONG_TYPE = ErrorCode(
-        code='ENTRIES_HAVE_KEY_ERR_002',
-        description='Entries field does not contain a list')
+        code="ENTRIES_HAVE_KEY_ERR_002",
+        description="Entries field does not contain a list",
+    )
 
     KEY_NOT_FOUND_IN_ENTRY = ErrorCode(
-        code='ENTRIES_HAVE_KEY_ERR_003',
-        description='Key missing in entry')
+        code="ENTRIES_HAVE_KEY_ERR_003", description="Key missing in entry"
+    )
 
     ENTRY_IS_NOT_A_DICT = ErrorCode(
-        code='ENTRIES_HAVE_KEY_ERR_004',
-        description='Entry that needs to have a key is not a dict')
+        code="ENTRIES_HAVE_KEY_ERR_004",
+        description="Entry that needs to have a key is not a dict",
+    )
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/storage/generic.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/generic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,92 @@
-"""Module to define abstract storage class
-"""
+"""Module to define abstract storage class"""
+
 from abc import ABCMeta, abstractmethod
 from datetime import datetime
 from typing import Any, Dict, Iterator, TypedDict
 
 from ..data_classes import TelemetryData, TelemetryModel
-from ..settings import AGGR_DATE_TIME_RANGE_METHODS, CATEGORY_KEY, \
-    PROCESS_TYPE_KEY, SOURCE_NAME_KEY, START_TIME, SUB_CATEGORY_KEY, \
-    TELEMETRY_TYPE_KEY
+from ..settings import (
+    AGGR_DATE_TIME_RANGE_METHODS,
+    CATEGORY_KEY,
+    PROCESS_TYPE_KEY,
+    SOURCE_NAME_KEY,
+    START_TIME,
+    SUB_CATEGORY_KEY,
+    TELEMETRY_TYPE_KEY,
+)
 from ..settings.date_ranges import DateTimeRange
 from ..settings.exceptions import RequestedDataTimeRangeMethodNotFound
 
 
 class UniqueAggregatedTelemetryKeys(TypedDict):
     """
     Class to define what query params are needed to define a unique
     aggregated telemetry object. For a set of query params given only 0 or 1
     telemetry object is allowed to exist (i.e. a daily aggregation can only
     occur once for each day, a weekly aggregation only once for each weak etc.)
     """
+
     telemetry_type: str
     category: str
     sub_category: str
     source_name: str
     process_type: str
     from_date_time: datetime
     to_date_time: datetime
 
 
 class AbstractTelemetryStorage(metaclass=ABCMeta):
-    """ Abstract Telemetry Storage class
+    """Abstract Telemetry Storage class
 
     implements store_telemetry method that persists a given telemetry object
 
     Any class that stores the telemetry objects should be subclassed from
     this Abstract Class
     """
-    __TELEMETRY_KEY: str = 'telemetry'
+
+    __TELEMETRY_KEY: str = "telemetry"
 
     @abstractmethod
     def store_telemetry(self, telemetry: TelemetryModel) -> None:
-        """ public method to persist telemetry object"""
+        """public method to persist telemetry object"""
 
     @abstractmethod
     def select_records(
-            self, telemetry_type: str, category: str, sub_category: str,
-            source_name: str, process_type: str, from_date_time: datetime,
-            to_date_time: datetime) -> Iterator:
+        self,
+        telemetry_type: str,
+        category: str,
+        sub_category: str,
+        source_name: str,
+        process_type: str,
+        from_date_time: datetime,
+        to_date_time: datetime,
+    ) -> Iterator:
         """
         Select telemetry records unique to a single process and source for as specific time period.
         """
 
     @abstractmethod
-    def _remove_existing_aggregation_telemetry(
-            self, telemetry: TelemetryModel) -> None:
+    def _remove_existing_aggregation_telemetry(self, telemetry: TelemetryModel) -> None:
         """
         Removes any already existing aggregations for a specific telemetry
         aggregation.
         If you want to run and store a new aggregation object (for example a
         daily aggrgation) then the already daily aggregation for that day must
         be removed.
 
         Args:
             telemetry (TelemetryModel): The new telemetry aggregation object
         """
 
     def _telemetry_storage_to_object(
-            self, stored_telemetry_object: Dict) -> TelemetryModel:
-        """Method to convert a sql light object into """
-        telemetry_data = stored_telemetry_object.pop(
-            self.__TELEMETRY_KEY, "{}")
+        self, stored_telemetry_object: Dict
+    ) -> TelemetryModel:
+        """Method to convert a sql light object into"""
+        telemetry_data = stored_telemetry_object.pop(self.__TELEMETRY_KEY, "{}")
         telemetry_model = TelemetryModel(**stored_telemetry_object)
         for sub_process, sub_process_tel_data in telemetry_data.items():
             telemetry_model.telemetry.update(
                 {sub_process: TelemetryData(**sub_process_tel_data)}
             )
         return telemetry_model
 
@@ -81,15 +94,16 @@
     def _db_object_to_dict(db_object: Any) -> Dict:
         """Returns a db object as a dict object."""
         # If the persistance model does not return a proper Dict object then
         # override this method to ensure a Dict object is available.
         return db_object
 
     def _get_aggr_telem_query_params(
-            self, telemetry: TelemetryModel) -> UniqueAggregatedTelemetryKeys:
+        self, telemetry: TelemetryModel
+    ) -> UniqueAggregatedTelemetryKeys:
         """
         Returns a dict with the query params to retrieve a unique aggregated
         telemetry object.
 
         Args:
             telemetry (TelemetryModel): The new telemetry aggregation object
 
@@ -104,46 +118,54 @@
         return UniqueAggregatedTelemetryKeys(
             telemetry_type=getattr(telemetry, TELEMETRY_TYPE_KEY),
             source_name=getattr(telemetry, SOURCE_NAME_KEY),
             category=getattr(telemetry, CATEGORY_KEY),
             sub_category=getattr(telemetry, SUB_CATEGORY_KEY),
             process_type=getattr(telemetry, PROCESS_TYPE_KEY),
             from_date_time=date_time_range.from_date,
-            to_date_time=date_time_range.to_date
+            to_date_time=date_time_range.to_date,
         )
 
     @staticmethod
-    def _get_aggr_telem_date_time_range(
-            telemetry: TelemetryModel) -> DateTimeRange:
+    def _get_aggr_telem_date_time_range(telemetry: TelemetryModel) -> DateTimeRange:
         """
         Method to get the correct datatime range for a date depending on the
         aggregation telemetry_type.
         For example for a monthly aggregation the input date of 2022-10-10
         will be converted into a datetime range of (2022-10-01, 2022-11-01).
         For a daily aggegration this would result in (2022-10-10, 2022-10-11).
         etc.
         """
         start_date_time = getattr(telemetry, START_TIME)
         telemetry_type = getattr(telemetry, TELEMETRY_TYPE_KEY)
-        date_time_range_method = AGGR_DATE_TIME_RANGE_METHODS.get(
-            telemetry_type)
+        date_time_range_method = AGGR_DATE_TIME_RANGE_METHODS.get(telemetry_type)
         if not date_time_range_method:
             raise RequestedDataTimeRangeMethodNotFound(telemetry_type)
 
         return date_time_range_method(start_date_time.date())
 
     def telemetry_list(
-            self, telemetry_type: str, category: str, sub_category: str,
-            source_name: str, process_type: str, from_date_time: datetime,
-            to_date_time: datetime) -> Iterator[TelemetryModel]:
+        self,
+        telemetry_type: str,
+        category: str,
+        sub_category: str,
+        source_name: str,
+        process_type: str,
+        from_date_time: datetime,
+        to_date_time: datetime,
+    ) -> Iterator[TelemetryModel]:
         """
-        Method to return an iteraror TelemetryModel instances retrieved from a database query with the provided arguments.
+        Method to return an iteraror TelemetryModel instances retrieved
+        from a database query with the provided arguments.
         """
         selected_records = self.select_records(
-            telemetry_type=telemetry_type, category=category,
-            sub_category=sub_category, source_name=source_name,
-            process_type=process_type, from_date_time=from_date_time,
-            to_date_time=to_date_time
+            telemetry_type=telemetry_type,
+            category=category,
+            sub_category=sub_category,
+            source_name=source_name,
+            process_type=process_type,
+            from_date_time=from_date_time,
+            to_date_time=to_date_time,
         )
         for record in selected_records:
             record_dict = self._db_object_to_dict(record)
             yield self._telemetry_storage_to_object(record_dict)
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/storage/memory.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""[summary]
-"""
+"""[summary]"""
+
 import json
 import sqlite3
 from datetime import datetime
 from typing import Iterator, Optional
 
 from ..data_classes import TelemetryModel
 from ..settings import exceptions
@@ -15,23 +15,24 @@
     """Method to allow sql queries to be returned as a dict.
 
     The telemetry field is seperately converted to a dict because
     sqlite returns a nested dict as a string.
     """
     col_names = [col[0] for col in cursor.description]
     telemetry = {key: value for key, value in zip(col_names, row)}
-    telemetry_str = telemetry.pop('telemetry', "{}")
-    telemetry.update({'telemetry': json.loads(telemetry_str)})
+    telemetry_str = telemetry.pop("telemetry", "{}")
+    telemetry.update({"telemetry": json.loads(telemetry_str)})
     return telemetry
 
 
 class TelemetryInMemoryStorage(AbstractTelemetryStorage):
     """
     Class to provice telemetry in memory storage for use when unit testing
     """
+
     db_in_memory: Optional[sqlite3.Connection] = None
     db_cursor: Optional[sqlite3.Cursor] = None
 
     def __init__(self):
         if not self.db_in_memory:
             self.initialize_db()
 
@@ -78,86 +79,105 @@
             raise exceptions.StorageNotInitialized
 
         telemetry_type = getattr(telemetry, st.TELEMETRY_TYPE_KEY)
         category = getattr(telemetry, st.CATEGORY_KEY)
         sub_category = getattr(telemetry, st.SUB_CATEGORY_KEY)
         source_name = getattr(telemetry, st.SOURCE_NAME_KEY)
         process_type = getattr(telemetry, st.PROCESS_TYPE_KEY)
-        start_date_time = getattr(telemetry, st.START_TIME)
+        start_date_time = getattr(telemetry, st.START_TIME).isoformat()
         run_time_in_seconds = getattr(telemetry, st.RUN_TIME)
         traffic_light = getattr(telemetry, st.TRAFFIC_LIGHT_KEY)
         io_time_in_seconds = getattr(telemetry, st.IO_TIME_KEY)
         telemetry_dict = {
-            k: v.__dict__ for k, v in
-            getattr(telemetry, st.TELEMETRY_FIELD_KEY).items()
+            k: v.__dict__ for k, v in getattr(telemetry, st.TELEMETRY_FIELD_KEY).items()
         }
         telemetry_json = json.dumps(telemetry_dict)
 
         self.db_cursor.execute(
             "insert into telemetry values (?, ?, ?, ?, ?, ?, ?, ?, ?, ?)",
             [
-                telemetry_type, category, sub_category,
-                source_name, process_type, start_date_time,
-                str(run_time_in_seconds), telemetry_json,
-                traffic_light, str(io_time_in_seconds)
-            ])
+                telemetry_type,
+                category,
+                sub_category,
+                source_name,
+                process_type,
+                start_date_time,
+                str(run_time_in_seconds),
+                telemetry_json,
+                traffic_light,
+                str(io_time_in_seconds),
+            ],
+        )
 
     def select_records(
-            self, telemetry_type: str, category: str, sub_category: str,
-            source_name: str, process_type: str, from_date_time: datetime,
-            to_date_time: datetime) -> Iterator:
+        self,
+        telemetry_type: str,
+        category: str,
+        sub_category: str,
+        source_name: str,
+        process_type: str,
+        from_date_time: datetime,
+        to_date_time: datetime,
+    ) -> Iterator:
         """
         Select telemetry records unique to a single process, source category
         and sub category for as specific time period.
         """
         if not self.db_cursor:
             raise exceptions.StorageNotInitialized
 
-        select_statement = \
-            ("SELECT * FROM telemetry WHERE "
-             f"telemetry_type='{telemetry_type}' AND "
-             f"category='{category}' AND "
-             f"sub_category='{sub_category}' AND "
-             f"source_name='{source_name}' AND "
-             f"process_type='{process_type}' AND "
-             f"start_date_time >= '{from_date_time}' AND "
-             f"start_date_time < '{to_date_time}'")
+        select_statement = (
+            "SELECT * FROM telemetry WHERE "
+            f"telemetry_type='{telemetry_type}' AND "
+            f"category='{category}' AND "
+            f"sub_category='{sub_category}' AND "
+            f"source_name='{source_name}' AND "
+            f"process_type='{process_type}' AND "
+            f"start_date_time >= '{from_date_time}' AND "
+            f"start_date_time < '{to_date_time}'"
+        )
 
         return self.db_cursor.execute(select_statement)
 
-    def _remove_existing_aggregation_telemetry(
-            self, telemetry: TelemetryModel) -> None:
+    def _remove_existing_aggregation_telemetry(self, telemetry: TelemetryModel) -> None:
         """
         Removes any already existing aggregations for a specific telemetry
         aggregation.
         If you want to run and store a new aggregation object (for example a
         daily aggrgation) then the already daily aggregation for that day must
         be removed.
 
         Args:
             telemetry (TelemetryModel): The new telemetry aggregation object
         """
         query_params_exist_aggr = self._get_aggr_telem_query_params(telemetry)
         self.delete_records(**query_params_exist_aggr)
 
     def delete_records(
-            self, telemetry_type: str, category: str, sub_category: str,
-            source_name: str, process_type: str, from_date_time: datetime,
-            to_date_time: datetime) -> None:
+        self,
+        telemetry_type: str,
+        category: str,
+        sub_category: str,
+        source_name: str,
+        process_type: str,
+        from_date_time: datetime,
+        to_date_time: datetime,
+    ) -> None:
         """
         Delete telemetry records unique to a single process, source category
         and sub category for as specific time period.
         """
         if not self.db_cursor:
             raise exceptions.StorageNotInitialized
 
-        select_statement = \
-            ("DELETE * FROM telemetry WHERE "
-             f"telemetry_type='{telemetry_type}' AND "
-             f"category='{category}' AND "
-             f"sub_category='{sub_category}' AND "
-             f"source_name='{source_name}' AND "
-             f"process_type='{process_type}' AND "
-             f"start_date_time > '{from_date_time}' AND "
-             f"start_date_time < '{to_date_time}'")
+        select_statement = (
+            "DELETE * FROM telemetry WHERE "
+            f"telemetry_type='{telemetry_type}' AND "
+            f"category='{category}' AND "
+            f"sub_category='{sub_category}' AND "
+            f"source_name='{source_name}' AND "
+            f"process_type='{process_type}' AND "
+            f"start_date_time > '{from_date_time}' AND "
+            f"start_date_time < '{to_date_time}'"
+        )
 
         self.db_cursor.execute(select_statement)
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/storage/mongo.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/mongo.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,32 +8,40 @@
 MONGO_DB_USERNAME
 MONGO_DB_HOST
 MONGO_DB_PORT
 
 If no host and port are defined the connection will dedault to a localhost
 mongoDB instance.
 """
+
 from datetime import datetime
 from typing import Any, Dict, Iterator
 
-from mongoengine import DateTimeField, DictField, Document, FloatField, \
-    StringField, connect
+from mongoengine import (
+    DateTimeField,
+    DictField,
+    Document,
+    FloatField,
+    StringField,
+    connect,
+)
 
 from ..data_classes import TelemetryModel
 from ..settings import settings as st
 from .generic import AbstractTelemetryStorage
 from .mongo_connection import MONGO_ACCESS_PARAMS
 
 connect(alias="telemetry", **MONGO_ACCESS_PARAMS)
 
 
 class TelemetryMongoModel(Document):
     """
     Class to provice telemetry Mongo Model for persistance in MongoDB
     """
+
     category = StringField()
     sub_category = StringField()
     source_name = StringField()
     process_type = StringField()
     start_date_time = DateTimeField()
     run_time_in_seconds = StringField()
     traffic_light = StringField()
@@ -58,15 +66,15 @@
         """
         Method to convert TelemetryMongoModel instance to a dict that can be
         used to instatiate a TelemetryModel object.
         The mongo object '_id' field needs to be removed as it is not used by
         TelemetryModel.
         """
         telemetry_dict = self.to_mongo().to_dict()
-        telemetry_dict.pop('_id', None)
+        telemetry_dict.pop("_id", None)
         # run_time_on_seconds is stored as str in Mongo but needs to be a float
         # when processing telemetry data
         telemetry_dict[st.RUN_TIME] = float(telemetry_dict[st.RUN_TIME])
         return telemetry_dict
 
 
 class TelemetryMongoStorage(AbstractTelemetryStorage):
@@ -82,16 +90,15 @@
         self.store_telemetry(telemetry)
 
     def store_telemetry(self, telemetry: TelemetryModel) -> None:
         """public method to persist telemetry object"""
         telemetry_mongo_kwargs = self._telemetry_model_kwargs(telemetry)
         TelemetryMongoModel(**telemetry_mongo_kwargs).save()
 
-    def _remove_existing_aggregation_telemetry(
-            self, telemetry: TelemetryModel) -> None:
+    def _remove_existing_aggregation_telemetry(self, telemetry: TelemetryModel) -> None:
         """
         Removes any already existing aggregations for a specific telemetry
         aggregation.
         If you want to run and store a new aggregation object (for example a
         daily aggrgation) then the already daily aggregation for that day must
         be removed.
 
@@ -114,16 +121,15 @@
         source_name = getattr(telemetry, st.SOURCE_NAME_KEY)
         process_type = getattr(telemetry, st.PROCESS_TYPE_KEY)
         start_date_time = getattr(telemetry, st.START_TIME)
         run_time_in_seconds = getattr(telemetry, st.RUN_TIME)
         traffic_light = getattr(telemetry, st.TRAFFIC_LIGHT_KEY)
         io_time_in_seconds = getattr(telemetry, st.IO_TIME_KEY)
         telemetry_data = {
-            k: v.__dict__ for k, v in
-            getattr(telemetry, st.TELEMETRY_FIELD_KEY).items()
+            k: v.__dict__ for k, v in getattr(telemetry, st.TELEMETRY_FIELD_KEY).items()
         }
 
         return {
             st.TELEMETRY_TYPE_KEY: telemetry_type,
             st.CATEGORY_KEY: category,
             st.SUB_CATEGORY_KEY: sub_category,
             st.SOURCE_NAME_KEY: source_name,
@@ -132,31 +138,39 @@
             st.RUN_TIME: str(round(run_time_in_seconds, 2)),
             st.TRAFFIC_LIGHT_KEY: traffic_light,
             st.TELEMETRY_FIELD_KEY: telemetry_data,
             st.IO_TIME_KEY: io_time_in_seconds,
         }
 
     def select_records(
-            self, telemetry_type: str, category: str, sub_category: str,
-            source_name: str, process_type: str, from_date_time: datetime,
-            to_date_time: datetime) -> Iterator:
+        self,
+        telemetry_type: str,
+        category: str,
+        sub_category: str,
+        source_name: str,
+        process_type: str,
+        from_date_time: datetime,
+        to_date_time: datetime,
+    ) -> Iterator:
         """
         Select telemetry records unique to a single process, source category
         and sub category for as specific time period.
         """
         query_details = {
-            'telemetry_type': telemetry_type,
-            'category': category, 'sub_category': sub_category,
-            'source_name': source_name, 'process_type': process_type
+            "telemetry_type": telemetry_type,
+            "category": category,
+            "sub_category": sub_category,
+            "source_name": source_name,
+            "process_type": process_type,
         }
 
         return TelemetryMongoModel.objects(
             start_date_time__gte=from_date_time,
             start_date_time__lt=to_date_time,
-            **query_details
+            **query_details,
         )
 
     @staticmethod
     def _db_object_to_dict(db_object: Any) -> Dict:
         """Returns a db object as a dict object."""
         # Mongo onbject need to be converted to Dict object first
         return db_object.to_dict()
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/validators/abstract_validator_instruction.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/abstract_validator_instruction.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""Module to define abstract validator class
-"""
+"""Module to define abstract validator class"""
+
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 from typing import List, Type
 
 from errors import ErrorCode
 
 
 @dataclass(frozen=True)
 class BaseValidatorInstructionRuleData:
     field_name: str
 
     def __post_init__(self):
-        if type(self.field_name) is not str:
+        if not isinstance(self.field_name, str):
             raise TypeError("Field 'field_name' must be of type 'str'.")
 
 
 class AbstractValidatorInstruction(metaclass=ABCMeta):
-    """Abstract Validator Instruction class
-    """
-    RULE_DATA_CLASS: Type[BaseValidatorInstructionRuleData] = \
+    """Abstract Validator Instruction class"""
+
+    RULE_DATA_CLASS: Type[BaseValidatorInstructionRuleData] = (
         BaseValidatorInstructionRuleData
-    INSTRUCTION = 'instruction_name'
-    FIELDNAME = 'field_name'
+    )
+    INSTRUCTION = "instruction_name"
+    FIELDNAME = "field_name"
 
     def __new__(cls):
-        """ make this a singleton class """
+        """make this a singleton class"""
         return cls
 
     @classmethod
-    def validate(
-            cls, dict_to_validate: dict, rule_dict: dict) -> list[ErrorCode]:
+    def validate(cls, dict_to_validate: dict, rule_dict: dict) -> list[ErrorCode]:
         """
         Public method to run the validation
         prior to validation the rule will be validated.
 
         Args:
             dict_to_validate (dict): Input dict that needs validation
             rule_content (dict): actual rule
@@ -47,31 +47,29 @@
         """
         rule_data = cls.RULE_DATA_CLASS(**rule_dict)
         return cls._validate(dict_to_validate, rule_data)
 
     @classmethod
     @abstractmethod
     def _validate(
-            cls, dict_to_validate: dict,
-            rule_data: BaseValidatorInstructionRuleData) -> List[ErrorCode]:
+        cls, dict_to_validate: dict, rule_data: BaseValidatorInstructionRuleData
+    ) -> List[ErrorCode]:
         """
         method to do the actual validation
 
         returns:
             - list of errorcodes
         """
 
     @classmethod
-    def _get_field_name(
-            cls, rule_data: BaseValidatorInstructionRuleData) -> str:
+    def _get_field_name(cls, rule_data: BaseValidatorInstructionRuleData) -> str:
         """
         Retrieves the field name in scope from the rule content.
         """
         return getattr(rule_data, cls.FIELDNAME)
 
     @staticmethod
     @abstractmethod
-    def _validation_error(
-            error_code: ErrorCode, fieldname: str) -> list[ErrorCode]:
+    def _validation_error(error_code: ErrorCode, fieldname: str) -> list[ErrorCode]:
         """
         Customize the errors and their content for the specific validation rule.
         """
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/validators/dict_validator.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/dict_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 """
 Module to define the DictValidator class
 
 classes:
     - DictValidator
 """
+
 from typing import Dict, List, Type
 
 from errors import ErrorCode
 
-from ..settings.exceptions import InstructionRegisteredTwice, \
-    RuleCanHaveOnlyOneInstruction, UnknownInstruction
+from ..settings.exceptions import (
+    InstructionRegisteredTwice,
+    RuleCanHaveOnlyOneInstruction,
+    UnknownInstruction,
+)
 from .abstract_validator_instruction import AbstractValidatorInstruction
 
 
-class DictValidator():
+class DictValidator:
     """Class to allow a dict validation according to a set of rules.
 
     class methods:
         - register_instruction():
             method to add instruction sets to the dictvalidator
     public methods:
         - validate():
             method to run the validate of a dict
     """
 
     _instructions: Dict[str, Type[AbstractValidatorInstruction]] = {}
 
     @classmethod
-    def validate(cls,
-                 dict_to_validate: dict,
-                 validation_rules: dict) -> List[ErrorCode]:
+    def validate(
+        cls, dict_to_validate: dict, validation_rules: dict
+    ) -> List[ErrorCode]:
         """Public class method to run the validation.
 
         :param dict_to_validate: data dict to be validated
         :type dict_to_validate: dict
         :param validation_rules: validation rules for this data object
         :type validation_rules: dict
 
@@ -41,16 +45,15 @@
         """
         errors = []
         for rule in validation_rules.items():
             errors.extend(cls._apply_rule(dict_to_validate, rule))
         return errors
 
     @classmethod
-    def _apply_rule(
-            cls, dict_to_validate: dict, rule: tuple) -> List[ErrorCode]:
+    def _apply_rule(cls, dict_to_validate: dict, rule: tuple) -> List[ErrorCode]:
         """[summary]
 
         Args:
             dict_to_validate (dict): data dict to be validated
             rule (tuple): The rule with the instruction on position 0 and
                           details for the instruction on position 1
 
@@ -63,36 +66,35 @@
         instruction = cls._instruction_from_rule(rule)
         if instruction not in cls._instructions:
             raise UnknownInstruction(instruction)
         validation_rule = cls._instructions.get(instruction)
 
         if validation_rule:
             return validation_rule.validate(
-                dict_to_validate=dict_to_validate,
-                rule_dict=rule[1]
+                dict_to_validate=dict_to_validate, rule_dict=rule[1]
             )
 
         return []
 
     @classmethod
     def register_instruction(
-            cls, instruction_class: Type[AbstractValidatorInstruction]) -> None:
+        cls, instruction_class: Type[AbstractValidatorInstruction]
+    ) -> None:
         """Registration at class level of the instruction
 
         Args:
             instruction_class (type):
 
         Raises:
             InstructionRegisteredTwice: [description]
         """
         instruction = instruction_class.INSTRUCTION
         if instruction in cls._instructions:
             raise InstructionRegisteredTwice(instruction_class)
-        cls._instructions.update({
-            instruction_class.INSTRUCTION: instruction_class})
+        cls._instructions.update({instruction_class.INSTRUCTION: instruction_class})
 
     @staticmethod
     def _instruction_from_rule(rule: tuple) -> str:
         """Returns the instruction string from rule dict
 
         Args:
             rule (tuple): The rule with the instruction on position 0 and
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/validators/entries_have_key.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/entries_have_key.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-"""Module to define EntriesHaveKey class validator
-"""
+"""Module to define EntriesHaveKey class validator"""
+
 from dataclasses import dataclass
 
 import jmespath
 from errors import ErrorCode, ListErrors
 
-from .abstract_validator_instruction import AbstractValidatorInstruction, \
-    BaseValidatorInstructionRuleData
+from .abstract_validator_instruction import (
+    AbstractValidatorInstruction,
+    BaseValidatorInstructionRuleData,
+)
 
 
 @dataclass(frozen=True)
 class EntriesHaveKeyRuleData(BaseValidatorInstructionRuleData):
     must_have_key: str
 
 
@@ -25,115 +27,114 @@
                             validated
         - must_have_key (str): field that hold the key that is to be present
                                in all entries
 
     public method
         - validate
     """
+
     RULE_DATA_CLASS = EntriesHaveKeyRuleData
-    INSTRUCTION = 'entries_have_key'
-    must_have_key = 'must_have_key'
+    INSTRUCTION = "entries_have_key"
+    must_have_key = "must_have_key"
 
     @classmethod
     def _validate(
-            cls, dict_to_validate: dict,
-            rule_data: BaseValidatorInstructionRuleData) -> list[ErrorCode]:
+        cls, dict_to_validate: dict, rule_data: BaseValidatorInstructionRuleData
+    ) -> list[ErrorCode]:
         """
         method to do the actual validation
 
         returns:
             - list of errorcodes
         """
         # if entries does not exist stop validation
         if error := cls._validate_field_exists(dict_to_validate, rule_data):
             return error
 
         # if entries field is not a list stop validation
-        if error := cls._validate_type_entries_field(
-                dict_to_validate, rule_data):
+        if error := cls._validate_type_entries_field(dict_to_validate, rule_data):
             return error
 
         # return the errors per entry
         return cls._validate_entries_have_key(dict_to_validate, rule_data)
 
     @classmethod
     def _validate_entries_have_key(
-            cls, dict_to_validate: dict,
-            rule_data: BaseValidatorInstructionRuleData) -> list[ErrorCode]:
+        cls, dict_to_validate: dict, rule_data: BaseValidatorInstructionRuleData
+    ) -> list[ErrorCode]:
         """
         method to check if the values in the entry have a specific key
 
         returns:
             - list{ErrorCode]: Empty list in case all entries have the key
         """
         errors = []
         fieldname = cls._get_field_name(rule_data)
         must_have_key = cls._get_must_have_key(rule_data)
 
         # prepare error messages
         entry_is_not_a_dict_error = cls._validation_error(
-            ListErrors.ENTRY_IS_NOT_A_DICT, fieldname)
+            ListErrors.ENTRY_IS_NOT_A_DICT, fieldname
+        )
         missing_key_in_entry_error = cls._validation_error(
-            ListErrors.KEY_NOT_FOUND_IN_ENTRY, fieldname + "__" + must_have_key)
+            ListErrors.KEY_NOT_FOUND_IN_ENTRY, fieldname + "__" + must_have_key
+        )
 
         # for each entry do a has_key validation with the `must_have_key` field
         for entry in jmespath.search(fieldname, dict_to_validate):
             if not isinstance(entry, dict):
                 errors.extend(entry_is_not_a_dict_error)
                 continue
 
             if not jmespath.search(must_have_key, entry):
                 errors.extend(missing_key_in_entry_error)
 
         return errors
 
     @classmethod
     def _validate_field_exists(
-            cls, dict_to_validate: dict,
-            rule_data: BaseValidatorInstructionRuleData) -> list[ErrorCode]:
+        cls, dict_to_validate: dict, rule_data: BaseValidatorInstructionRuleData
+    ) -> list[ErrorCode]:
         """
         method to check if entries field exists in dict_to_validate
 
         returns:
             - list{ErrorCode]: Empty list in case the field does exist
         """
         fieldname = cls._get_field_name(rule_data)
 
         if not jmespath.search(fieldname, dict_to_validate):
-            return cls._validation_error(
-                ListErrors.ENTRIES_FIELD_NOT_FOUND, fieldname)
+            return cls._validation_error(ListErrors.ENTRIES_FIELD_NOT_FOUND, fieldname)
 
         return []
 
     @classmethod
     def _validate_type_entries_field(
-            cls, dict_to_validate: dict,
-            rule_data: BaseValidatorInstructionRuleData) -> list[ErrorCode]:
+        cls, dict_to_validate: dict, rule_data: BaseValidatorInstructionRuleData
+    ) -> list[ErrorCode]:
         """
         method to check if entries field in dict_to_validate is a list
 
         returns:
             - list[ErrorCode]: Empty list in case the field holds a list
         """
         fieldname = cls._get_field_name(rule_data)
         entries = jmespath.search(fieldname, dict_to_validate)
         if not isinstance(entries, (list)):
             return cls._validation_error(
-                ListErrors.ENTRIES_FIELD_OF_WRONG_TYPE, fieldname)
+                ListErrors.ENTRIES_FIELD_OF_WRONG_TYPE, fieldname
+            )
 
         return []
 
     @classmethod
-    def _get_must_have_key(
-            cls, rule_data: BaseValidatorInstructionRuleData) -> str:
+    def _get_must_have_key(cls, rule_data: BaseValidatorInstructionRuleData) -> str:
         """
         retrieves the must_have_key from the rule content
         """
         return getattr(rule_data, cls.must_have_key)
 
     @staticmethod
-    def _validation_error(
-            error_code: ErrorCode, fieldname: str) -> list[ErrorCode]:
-        """ returns error code object in list with fieldname as error data """
-        key_specific_error = error_code.code + '@KEY_<' + fieldname + '>'
-        return [ErrorCode(
-            code=key_specific_error, description=error_code.description)]
+    def _validation_error(error_code: ErrorCode, fieldname: str) -> list[ErrorCode]:
+        """returns error code object in list with fieldname as error data"""
+        key_specific_error = error_code.code + "@KEY_<" + fieldname + ">"
+        return [ErrorCode(code=key_specific_error, description=error_code.description)]
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/validators/has_key.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/has_key.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""Module to define HasKey class validator
-"""
+"""Module to define HasKey class validator"""
+
 import jmespath
 from errors import ErrorCode, ListErrors
 
-from .abstract_validator_instruction import AbstractValidatorInstruction, \
-    BaseValidatorInstructionRuleData
+from .abstract_validator_instruction import (
+    AbstractValidatorInstruction,
+    BaseValidatorInstructionRuleData,
+)
 
 
 class HasKey(AbstractValidatorInstruction):
     """
     class to define HasFieldName validation instruction.
     """
-    INSTRUCTION = 'has_key'
-    FIELDNAME = 'field_name'
+
+    INSTRUCTION = "has_key"
+    FIELDNAME = "field_name"
 
     @classmethod
     def _validate(
-            cls, dict_to_validate: dict,
-            rule_data: BaseValidatorInstructionRuleData) -> list[ErrorCode]:
+        cls, dict_to_validate: dict, rule_data: BaseValidatorInstructionRuleData
+    ) -> list[ErrorCode]:
         """
         method to do the actual validation
 
         returns:
             - error in case
         """
         fieldname = cls._get_field_name(rule_data)
         if not jmespath.search(fieldname, dict_to_validate):
-            return cls._validation_error(
-                ListErrors.KEY_NOT_FOUND, fieldname)
+            return cls._validation_error(ListErrors.KEY_NOT_FOUND, fieldname)
 
         return []
 
     @staticmethod
-    def _validation_error(
-            error_code: ErrorCode, fieldname: str) -> list[ErrorCode]:
-        """ returns error code object in list with fieldname as error data """
-        key_specific_error = error_code.code + '@KEY_<' + fieldname + '>'
-        return [ErrorCode(
-            code=key_specific_error, description=error_code.description)]
+    def _validation_error(error_code: ErrorCode, fieldname: str) -> list[ErrorCode]:
+        """returns error code object in list with fieldname as error data"""
+        key_specific_error = error_code.code + "@KEY_<" + fieldname + ">"
+        return [ErrorCode(code=key_specific_error, description=error_code.description)]
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry/validators/validate_entries.py` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/validate_entries.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-"""Module to define validate entries validator class
-"""
+"""Module to define validate entries validator class"""
+
 from dataclasses import dataclass
 from typing import Optional
 
 import jmespath
 from errors import ErrorCode, ListErrors, add_error_data
 
 from ..settings import exceptions
-from .abstract_validator_instruction import AbstractValidatorInstruction, \
-    BaseValidatorInstructionRuleData
+from .abstract_validator_instruction import (
+    AbstractValidatorInstruction,
+    BaseValidatorInstructionRuleData,
+)
 
 
 @dataclass(frozen=True)
 class ValidateEntriesRuleData(BaseValidatorInstructionRuleData):
     expected_count: int
 
     def __post_init__(self):
-        if type(self.expected_count) is not int:
+        if not isinstance(self.expected_count, int):
             raise TypeError("Field 'expected_count' must be of type 'int'.")
 
         if self.expected_count < 0:
             raise exceptions.ExpectedCountMustBePositiveInt
 
         super().__post_init__()
 
@@ -28,52 +30,50 @@
 class ValidateEntries(AbstractValidatorInstruction):
     """
     class to define validate entries instruction.
     This instruction counts the entries in a list or a dict and reports an
     error when the number of items in the list or dict is different from the
     expected nr of items
     """
+
     RULE_DATA_CLASS = ValidateEntriesRuleData
-    INSTRUCTION = 'validate_entries'
-    expected_count_field = 'expected_count'
+    INSTRUCTION = "validate_entries"
+    expected_count_field = "expected_count"
 
     @classmethod
     def _validate(
-            cls, dict_to_validate: dict,
-            rule_data: BaseValidatorInstructionRuleData) -> list[ErrorCode]:
+        cls, dict_to_validate: dict, rule_data: BaseValidatorInstructionRuleData
+    ) -> list[ErrorCode]:
         """
         method to do the actual validation
 
         returns:
             - error in case
         """
         fieldname = cls._get_field_name(rule_data)
 
         field_to_validate = jmespath.search(fieldname, dict_to_validate)
 
         if not field_to_validate:
-            return cls._validation_error(
-                ListErrors.FIELD_NOT_FOUND, fieldname)
+            return cls._validation_error(ListErrors.FIELD_NOT_FOUND, fieldname)
 
         if not isinstance(field_to_validate, (list, dict)):
-            return cls._validation_error(
-                ListErrors.WRONG_TYPE_IN_FIELD, fieldname)
+            return cls._validation_error(ListErrors.WRONG_TYPE_IN_FIELD, fieldname)
 
         if len(field_to_validate) != cls._get_expected_count(rule_data):
-            return cls._validation_error(
-                ListErrors.UNEXPECTED_NR_OF_ITEMS, fieldname)
+            return cls._validation_error(ListErrors.UNEXPECTED_NR_OF_ITEMS, fieldname)
 
         return []
 
     @classmethod
-    def _get_expected_count(cls, rule_data: BaseValidatorInstructionRuleData
-                            ) -> Optional[str]:
+    def _get_expected_count(
+        cls, rule_data: BaseValidatorInstructionRuleData
+    ) -> Optional[str]:
         """
         retrieves the expected_count in scope of the rule content
         """
         return getattr(rule_data, cls.expected_count_field)
 
     @staticmethod
-    def _validation_error(
-            error_code: ErrorCode, fieldname: str) -> list[ErrorCode]:
-        """ returns error code object in list with fieldname as error data """
+    def _validation_error(error_code: ErrorCode, fieldname: str) -> list[ErrorCode]:
+        """returns error code object in list with fieldname as error data"""
         return [add_error_data(error=error_code, error_data=fieldname)]
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry.egg-info/PKG-INFO` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,88 @@
 Metadata-Version: 2.1
 Name: pipeline-telemetry
-Version: 0.9.4
-Summary: Create and store data pipeline telemetry data
+Version: 1.0.0
+Summary: Measure your data pipelines with easy to use telemetry logic
 Home-page: https://github.com/MaartendeRuyter/pipeline-telemetry
 Author: Maarten de Ruyter
-Author-email: maarten@geodatagarden.com
-License: LGPL-3.0-or-later
-Project-URL: Documentation, https://pipeline-telemetry.readthedocs.io/
-Project-URL: Changelog, https://pipeline-telemetry.readthedocs.io/en/latest/changelog.html
-Project-URL: Issue Tracker, https://github.com/MaartendeRuyter/pipeline-telemetry/issues
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
+Author-email: "Maarten de Ruyter" <maarten@geodatagarden.com>
+License: GNU
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Utilities
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.rst
+Requires-Dist: error-manager
+Requires-Dist: mongoengine
+Requires-Dist: jmespath
 
 ========
 Overview
 ========
 
+.. start-badges
+
+.. list-table::
+    :stub-columns: 1
+
+    * - docs
+      - |docs|
+    * - tests
+      - | |travis| |requires|
+        | |codecov|
+    * - package
+      - | |version| |wheel|
+        | |supported-versions|
+        | |supported-implementations|
+        | |commits-since|
+.. |docs| image:: https://readthedocs.org/projects/pipeline-telemetry/badge/?style=flat
+    :target: https://pipeline-telemetry.readthedocs.io/
+    :alt: Documentation Status
+
+.. |travis| image:: https://api.travis-ci.com/MaartendeRuyter/pipeline-telemetry.svg?branch=master
+    :alt: Travis-CI Build Status
+    :target: https://travis-ci.com/github/MaartendeRuyter/pipeline-telemetry
+
+.. |requires| image:: https://requires.io/github/MaartendeRuyter/pipeline-telemetry/requirements.svg?branch=master
+    :alt: Requirements Status
+    :target: https://requires.io/github/MaartendeRuyter/pipeline-telemetry/requirements/?branch=master
+
+.. |codecov| image:: https://codecov.io/gh/MaartendeRuyter/pipeline-telemetry/branch/master/graphs/badge.svg?branch=master
+    :alt: Coverage Status
+    :target: https://codecov.io/github/MaartendeRuyter/pipeline-telemetry
+
+.. |version| image:: https://img.shields.io/pypi/v/pipeline-telemetry.svg
+    :alt: PyPI Package latest release
+    :target: https://pypi.org/project/pipeline-telemetry
+
+.. |wheel| image:: https://img.shields.io/pypi/wheel/pipeline-telemetry.svg
+    :alt: PyPI Wheel
+    :target: https://pypi.org/project/pipeline-telemetry
+
+.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/pipeline-telemetry.svg
+    :alt: Supported versions
+    :target: https://pypi.org/project/pipeline-telemetry
+
+.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pipeline-telemetry.svg
+    :alt: Supported implementations
+    :target: https://pypi.org/project/pipeline-telemetry
+
+.. |commits-since| image:: https://img.shields.io/github/commits-since/MaartendeRuyter/pipeline-telemetry/v0.0.1.svg
+    :alt: Commits since latest release
+    :target: https://github.com/MaartendeRuyter/pipeline-telemetry/compare/v0.0.1...master
 
 
+
+.. end-badges
+
 Create and store data pipeline telemetry data
 
 * Free software: GNU Lesser General Public License v3 or later (LGPLv3+)
 
 Installing pipeline-telemetry
 =============================
 
@@ -79,14 +125,17 @@
       - ::
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
+1.0.0 (2024-05-08)
+-------------------
+* Added python 3.12 support
 
 0.9.4 (2022-11-03)
 -------------------
 * Added ``PartialToSingleMongoAggregator`` and ``PartialToSingleAggregator``
   classes to allow automated aggregation of multiple partial telemetry objects to a single telemetry object.
 
 
@@ -277,9 +326,7 @@
 * Added MongoDb storage class
 * Started with documentation
 
 
 0.0.1 (2021-10-06)
 ------------------
 * First release on PyPI.
-
-
```

### Comparing `pipeline-telemetry-0.9.4/src/pipeline_telemetry.egg-info/SOURCES.txt` & `pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,16 @@
-.bumpversion.cfg
-.cookiecutterrc
-.coveragerc
-.editorconfig
-.isort.cfg
-.pre-commit-config.yaml
 .readthedocs.yml
-.travis.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
-setup.py
-tox.ini
-ci/bootstrap.py
-ci/requirements.txt
-ci/templates/.appveyor.yml
-ci/templates/.travis.yml
 docs/adding telemetry.rst
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/decorators.rst
 docs/index.rst
@@ -35,25 +23,21 @@
 docs/telemetry counters.rst
 docs/telemetry mixin.rst
 docs/telemetry object.rst
 docs/usage.rst
 docs/reference/index.rst
 docs/reference/pipeline_telemetry.rst
 src/pipeline_telemetry/__init__.py
-src/pipeline_telemetry/__main__.py
-src/pipeline_telemetry/cli.py
 src/pipeline_telemetry/decorator.py
 src/pipeline_telemetry/helper.py
 src/pipeline_telemetry/main.py
 src/pipeline_telemetry/mixin.py
 src/pipeline_telemetry.egg-info/PKG-INFO
 src/pipeline_telemetry.egg-info/SOURCES.txt
 src/pipeline_telemetry.egg-info/dependency_links.txt
-src/pipeline_telemetry.egg-info/entry_points.txt
-src/pipeline_telemetry.egg-info/not-zip-safe
 src/pipeline_telemetry.egg-info/requires.txt
 src/pipeline_telemetry.egg-info/top_level.txt
 src/pipeline_telemetry/aggregator/__init__.py
 src/pipeline_telemetry/aggregator/aggregator.py
 src/pipeline_telemetry/aggregator/helper.py
 src/pipeline_telemetry/aggregator/mongo_aggregator.py
 src/pipeline_telemetry/data_classes/__init__.py
@@ -77,15 +61,14 @@
 src/pipeline_telemetry/validators/has_key.py
 src/pipeline_telemetry/validators/validate_entries.py
 tests/test_add_telemetry.py
 tests/test_data.py
 tests/test_decorator.py
 tests/test_helpers.py
 tests/test_mixin.py
-tests/test_pipeline_telemetry.py
 tests/test_process_types.py
 tests/test_settings_module.py
 tests/test_telemetry_class_methods.py
 tests/test_telemetry_counter.py
 tests/test_aggregator/test_aggregator.py
 tests/test_aggregator/test_aggregator_data.py
 tests/test_aggregator/test_daily_aggregator.py
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_add_telemetry.py` & `pipeline_telemetry-1.0.0/tests/test_add_telemetry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,65 @@
 """Module to define tests for adding telemetry"""
+
 import pytest
 from errors.error import ListErrors
 from test_data import DEFAULT_TELEMETRY_PARAMS, TEST_TELEMETRY_RULES
 
 from pipeline_telemetry import Telemetry
 from pipeline_telemetry.settings import exceptions
 from pipeline_telemetry.settings import settings as st
 
 
 def test_add_method_adds_errors_to_sub_process():
     """Test that errors are added to telemetry sub_process."""
     telemetry = Telemetry(**DEFAULT_TELEMETRY_PARAMS)
-    telemetry.add('RETRIEVE_RAW_DATA', None, [ListErrors.KEY_NOT_FOUND])
-    sub_process_telemetry = telemetry.get('RETRIEVE_RAW_DATA')
-    assert getattr(sub_process_telemetry, st.ERRORS_KEY).get(
-        ListErrors.KEY_NOT_FOUND.code) == 1
+    telemetry.add("RETRIEVE_RAW_DATA", None, [ListErrors.KEY_NOT_FOUND])
+    sub_process_telemetry = telemetry.get("RETRIEVE_RAW_DATA")
+    assert (
+        getattr(sub_process_telemetry, st.ERRORS_KEY).get(ListErrors.KEY_NOT_FOUND.code)
+        == 1
+    )
 
 
 def test_add_method_raises_exception_when_telemetry_closed():
     """Test that errors are added to telemetry sub_process."""
     telemetry = Telemetry(**DEFAULT_TELEMETRY_PARAMS)
     telemetry.save_and_close()
     with pytest.raises(exceptions.TelemetryObjectAlreadyClosed):
-        telemetry.add('RETRIEVE_RAW_DATA', None, [ListErrors.KEY_NOT_FOUND])
+        telemetry.add("RETRIEVE_RAW_DATA", None, [ListErrors.KEY_NOT_FOUND])
 
 
 def test_add_errors_method_adds_errors_to_sub_process():
     """Test that errors are added to telemetry sub_process."""
     telemetry = Telemetry(**DEFAULT_TELEMETRY_PARAMS)
-    telemetry.increase_sub_process_base_count('RETRIEVE_RAW_DATA')
-    telemetry._add_errors('RETRIEVE_RAW_DATA', [ListErrors.KEY_NOT_FOUND])
-    sub_process_telemetry = telemetry.get('RETRIEVE_RAW_DATA')
-    assert getattr(sub_process_telemetry, st.ERRORS_KEY).get(
-        ListErrors.KEY_NOT_FOUND.code) == 1
+    telemetry.increase_sub_process_base_count("RETRIEVE_RAW_DATA")
+    telemetry._add_errors("RETRIEVE_RAW_DATA", [ListErrors.KEY_NOT_FOUND])
+    sub_process_telemetry = telemetry.get("RETRIEVE_RAW_DATA")
+    assert (
+        getattr(sub_process_telemetry, st.ERRORS_KEY).get(ListErrors.KEY_NOT_FOUND.code)
+        == 1
+    )
 
 
 def test_validate_data_method():
     """Test _validate_data_method returns list of errors."""
-    telemetry = Telemetry(telemetry_rules=TEST_TELEMETRY_RULES,
-                          **DEFAULT_TELEMETRY_PARAMS)
-    telemetry.increase_sub_process_base_count('RETRIEVE_RAW_DATA')
-    errors = telemetry._validate_data(sub_process='RETRIEVE_RAW_DATA',
-                                      data={})
+    telemetry = Telemetry(
+        telemetry_rules=TEST_TELEMETRY_RULES, **DEFAULT_TELEMETRY_PARAMS
+    )
+    telemetry.increase_sub_process_base_count("RETRIEVE_RAW_DATA")
+    errors = telemetry._validate_data(sub_process="RETRIEVE_RAW_DATA", data={})
     assert ListErrors.KEY_NOT_FOUND.code in str(errors[0])
-    assert '@KEY_<items>' in str(errors[0])
+    assert "@KEY_<items>" in str(errors[0])
 
 
 def test_validate_data_method_returns_empty_list():
     """
     Test _validate_data_method returns empty list when no errors are found.
     """
-    telemetry = Telemetry(telemetry_rules=TEST_TELEMETRY_RULES,
-                          **DEFAULT_TELEMETRY_PARAMS)
-    telemetry.increase_sub_process_base_count('RETRIEVE_RAW_DATA')
-    errors = telemetry._validate_data(sub_process='RETRIEVE_RAW_DATA',
-                                      data={'items': [1, 2, 3]})
+    telemetry = Telemetry(
+        telemetry_rules=TEST_TELEMETRY_RULES, **DEFAULT_TELEMETRY_PARAMS
+    )
+    telemetry.increase_sub_process_base_count("RETRIEVE_RAW_DATA")
+    errors = telemetry._validate_data(
+        sub_process="RETRIEVE_RAW_DATA", data={"items": [1, 2, 3]}
+    )
     assert errors == []
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_aggregator/test_aggregator.py` & `pipeline_telemetry-1.0.0/tests/test_aggregator/test_aggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""Module to test aggregator logic.
-"""
+"""Module to test aggregator logic."""
+
 from pipeline_telemetry import TelemetryAggregator
 
 
 def test_aggegator_class_exists():
     """Test the TelemetryAggregator class exists."""
     assert TelemetryAggregator
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_aggregator/test_aggregator_data.py` & `pipeline_telemetry-1.0.0/tests/test_aggregator/test_aggregator_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,34 +12,44 @@
 YESTERDAY = date.today() - timedelta(days=1)
 DAY_BEFORE_YESTERDAY = date.today() - timedelta(days=2)
 
 TELEMETRY_MODEL_1 = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
 
 telemetry_model_2 = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
 telemetry_data_2 = TelemetryData(base_counter=1)
-telemetry_model_2.telemetry.update({'DATA_STORAGE': telemetry_data_2})
+telemetry_model_2.telemetry.update({"DATA_STORAGE": telemetry_data_2})
 
 telemetry_model_3 = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
 telemetry_data_3 = TelemetryData(base_counter=2, fail_counter=1)
-telemetry_model_3.telemetry.update({'DATA_STORAGE': telemetry_data_3})
+telemetry_model_3.telemetry.update({"DATA_STORAGE": telemetry_data_3})
 
 
-class TelemetryTestList():
+class TelemetryTestList:
     __telemetry_models: List[TelemetryModel] = [
-        TELEMETRY_MODEL_1, telemetry_model_2, telemetry_model_3]
+        TELEMETRY_MODEL_1,
+        telemetry_model_2,
+        telemetry_model_3,
+    ]
     stored_telemetry: List[TelemetryModel]
 
     def telemetry_list(
-            self, telemetry_type: str, category: str, sub_category: str,
-            source_name: str, process_type: str, from_date_time: datetime,
-            to_date_time: datetime) -> Iterator[TelemetryModel]:
+        self,
+        telemetry_type: str,
+        category: str,
+        sub_category: str,
+        source_name: str,
+        process_type: str,
+        from_date_time: datetime,
+        to_date_time: datetime,
+    ) -> Iterator[TelemetryModel]:
         """
-        Method to return an iteraror TelemetryModel instances retrieved from a database query with the provided arguments.
+        Method to return an iteraror TelemetryModel instances retrieved from a database
+        query with the provided arguments.
         """
         for telemetry_model in self.__telemetry_models:
             yield telemetry_model
 
     def store_telemetry(self, telemetry: TelemetryModel) -> None:
-        """ public method to persist telemetry object"""
-        if not hasattr(self, 'stored_telemetry'):
+        """public method to persist telemetry object"""
+        if not hasattr(self, "stored_telemetry"):
             self.stored_telemetry = []
         self.stored_telemetry.append(telemetry)
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_aggregator/test_daily_aggregator.py` & `pipeline_telemetry-1.0.0/tests/test_aggregator/test_daily_aggregator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,31 @@
-"""Module to test the DailyAggregator class.
-"""
-from test_aggregator_data import DAY_BEFORE_YESTERDAY, TODAY, YESTERDAY, \
-    TelemetryTestList
+"""Module to test the DailyAggregator class."""
+
+from test_aggregator_data import (
+    DAY_BEFORE_YESTERDAY,
+    TODAY,
+    YESTERDAY,
+    TelemetryTestList,
+)
 
 from pipeline_telemetry import DailyAggregator, TelemetrySelector
 from pipeline_telemetry.aggregator.helper import TelemetryListArgs
 from pipeline_telemetry.data_classes import TelemetryModel
 from pipeline_telemetry.settings import settings as st
-from pipeline_telemetry.settings.date_ranges import \
-    get_daily_date_range_yesterday
+from pipeline_telemetry.settings.date_ranges import get_daily_date_range_yesterday
 
 keys_in_telemetry_list_params = [
-    'telemetry_type', 'category', 'sub_category', 'source_name',
-    'process_type', 'from_date_time', 'to_date_time']
+    "telemetry_type",
+    "category",
+    "sub_category",
+    "source_name",
+    "process_type",
+    "from_date_time",
+    "to_date_time",
+]
 
 
 def test_daily_aggregator_exists():
     """Test that the DailyAggregator class exists."""
     assert DailyAggregator
 
 
@@ -24,89 +33,100 @@
     """Test that the TelemetrySelector class exists."""
     assert TelemetrySelector
 
 
 def test_telemetry_selector_class_can_be_instantiated():
     """Test that the TelemetrySelector class exists."""
     assert TelemetrySelector(
-        category='test', sub_category='sub_test', source_name='source',
-        process_type='process_type'
+        category="test",
+        sub_category="sub_test",
+        source_name="source",
+        process_type="process_type",
     )
 
 
 def test_daily_aggregator_defines_target_telemetry_object():
     """Test that the DailyAggregator defines ."""
     telemetry_selector = TelemetrySelector(
-        category='test', sub_category='sub_test', source_name='source',
-        process_type='process_type')
+        category="test",
+        sub_category="sub_test",
+        source_name="source",
+        process_type="process_type",
+    )
 
     aggr = DailyAggregator(
-        telemetry_selector=telemetry_selector,
-        telemetry_storage=TelemetryTestList
+        telemetry_selector=telemetry_selector, telemetry_storage=TelemetryTestList
     )
-    assert aggr.target_telemetry.telemetry_type == \
-        st.DAILY_AGGR_TELEMETRY_TYPE
+    assert aggr.target_telemetry.telemetry_type == st.DAILY_AGGR_TELEMETRY_TYPE
 
 
 def test_telememtry_list_params():
     """Test if telemetry list params returns TelemetryListArgs."""
     telemetry_selector = TelemetrySelector(
-        category='test', sub_category='sub_test', source_name='source',
-        process_type='process_type')
+        category="test",
+        sub_category="sub_test",
+        source_name="source",
+        process_type="process_type",
+    )
 
     aggr = DailyAggregator(
-        telemetry_selector=telemetry_selector,
-        telemetry_storage=TelemetryTestList
+        telemetry_selector=telemetry_selector, telemetry_storage=TelemetryTestList
     )
     telemetry_list_params = aggr._telememtry_list_params(
-        date_time_range=next(get_daily_date_range_yesterday()))
+        date_time_range=next(get_daily_date_range_yesterday())
+    )
     assert isinstance(telemetry_list_params, TelemetryListArgs)
 
 
 def test_run_aggregation():
     """Method to test a single aggregation."""
     telemetry_selector = TelemetrySelector(
-        category='test', sub_category='sub_test', source_name='source',
-        process_type='process_type')
+        category="test",
+        sub_category="sub_test",
+        source_name="source",
+        process_type="process_type",
+    )
     aggr = DailyAggregator(
-        telemetry_selector=telemetry_selector,
-        telemetry_storage=TelemetryTestList()
+        telemetry_selector=telemetry_selector, telemetry_storage=TelemetryTestList()
     )
-    result_telemetry = aggr._run_aggregation(
-        next(get_daily_date_range_yesterday()))
+    result_telemetry = aggr._run_aggregation(next(get_daily_date_range_yesterday()))
     assert isinstance(result_telemetry, TelemetryModel)
-    assert result_telemetry.telemetry['DATA_STORAGE'].base_counter == 3
-    assert result_telemetry.telemetry['DATA_STORAGE'].fail_counter == 1
+    assert result_telemetry.telemetry["DATA_STORAGE"].base_counter == 3
+    assert result_telemetry.telemetry["DATA_STORAGE"].fail_counter == 1
 
 
 def test_run_aggregation_for_one_day():
     """Method to test that one aggregation was stored."""
     telemetry_selector = TelemetrySelector(
-        category='test', sub_category='sub_test', source_name='source',
-        process_type='process_type')
+        category="test",
+        sub_category="sub_test",
+        source_name="source",
+        process_type="process_type",
+    )
     storage = TelemetryTestList()
     aggr = DailyAggregator(
-        telemetry_selector=telemetry_selector,
-        telemetry_storage=storage
+        telemetry_selector=telemetry_selector, telemetry_storage=storage
     )
     aggr.aggregate(YESTERDAY, TODAY)
     assert len(storage.stored_telemetry) == 1
     result_telemetry = storage.stored_telemetry[0]
-    assert result_telemetry.telemetry['DATA_STORAGE'].base_counter == 3
+    assert result_telemetry.telemetry["DATA_STORAGE"].base_counter == 3
 
 
 def test_run_aggregation_for_two_days():
     """Method to test that two aggregations were stored."""
     telemetry_selector = TelemetrySelector(
-        category='test', sub_category='sub_test', source_name='source',
-        process_type='process_type')
+        category="test",
+        sub_category="sub_test",
+        source_name="source",
+        process_type="process_type",
+    )
     storage = TelemetryTestList()
     aggr = DailyAggregator(
-        telemetry_selector=telemetry_selector,
-        telemetry_storage=storage
+        telemetry_selector=telemetry_selector, telemetry_storage=storage
     )
     aggr.aggregate(DAY_BEFORE_YESTERDAY, TODAY)
     assert len(storage.stored_telemetry) == 2
     first_telemetry = storage.stored_telemetry[0]
     second_telemetry = storage.stored_telemetry[1]
     assert first_telemetry.start_date_time.date() == DAY_BEFORE_YESTERDAY
     assert second_telemetry.start_date_time.date() == YESTERDAY
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_aggregator/test_helper.py` & `pipeline_telemetry-1.0.0/tests/test_aggregator/test_helper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,152 +1,143 @@
-""" Module for testing aggregator helper functions
-"""
+"""Module for testing aggregator helper functions"""
+
 from datetime import date, datetime, timedelta
 
-from pipeline_telemetry.settings.date_ranges import DateTimeRange, \
-    date_range_generator, get_daily_date_range_for_single_date, \
-    get_daily_date_range_till_yesterday, get_daily_date_range_yesterday, \
-    get_daily_date_ranges, get_monthly_date_range_for_single_date, \
-    get_weekly_date_range_for_single_date
+from pipeline_telemetry.settings.date_ranges import (
+    DateTimeRange,
+    date_range_generator,
+    get_daily_date_range_for_single_date,
+    get_daily_date_range_till_yesterday,
+    get_daily_date_range_yesterday,
+    get_daily_date_ranges,
+    get_monthly_date_range_for_single_date,
+    get_weekly_date_range_for_single_date,
+)
 
 
 def str_to_date_time(date_str: str) -> datetime:
-    return datetime.strptime(date_str, '%Y-%m-%d')
+    return datetime.strptime(date_str, "%Y-%m-%d")
 
 
 def str_to_date(date_str: str) -> date:
     return str_to_date_time(date_str).date()
 
 
 def test_date_range_generator():
     """Test date_range_generator generates DateTimeRanges."""
-    start_date_time = datetime.strptime("2022-01-18", '%Y-%m-%d')
+    start_date_time = datetime.strptime("2022-01-18", "%Y-%m-%d")
     time_delta = timedelta(days=1)
     end_date_time = start_date_time + timedelta(days=3)
     daterange_generator = date_range_generator(
         start_date_time=start_date_time,
         end_date_time=end_date_time,
-        time_delta=time_delta
+        time_delta=time_delta,
     )
     result = [daterange for daterange in daterange_generator]
     assert result == [
-        DateTimeRange(
-            str_to_date_time('2022-01-18'), str_to_date_time('2022-01-19')),
-        DateTimeRange(
-            str_to_date_time('2022-01-19'), str_to_date_time('2022-01-20')),
-        DateTimeRange(
-            str_to_date_time('2022-01-20'), str_to_date_time('2022-01-21'))]
+        DateTimeRange(str_to_date_time("2022-01-18"), str_to_date_time("2022-01-19")),
+        DateTimeRange(str_to_date_time("2022-01-19"), str_to_date_time("2022-01-20")),
+        DateTimeRange(str_to_date_time("2022-01-20"), str_to_date_time("2022-01-21")),
+    ]
 
 
 def test_date_range_generator_with_during_day_time_stamps():
     """
     Test date_range_generator generates correct DateTimeRanges when atributes
     contain a time other the 00:00:00. The first daterange should start with
     the date part of the from_data."""
-    start_date_time = datetime.strptime(
-        "2022-01-18 13:55:26", '%Y-%m-%d %H:%M:%S')
+    start_date_time = datetime.strptime("2022-01-18 13:55:26", "%Y-%m-%d %H:%M:%S")
     time_delta = timedelta(days=1)
     end_date_time = start_date_time + timedelta(days=3)
     daterange_generator = date_range_generator(
         start_date_time=start_date_time,
         end_date_time=end_date_time,
-        time_delta=time_delta
+        time_delta=time_delta,
     )
     result = [daterange for daterange in daterange_generator]
     assert result == [
-        DateTimeRange(
-            str_to_date_time('2022-01-18'), str_to_date_time('2022-01-19')),
-        DateTimeRange(
-            str_to_date_time('2022-01-19'), str_to_date_time('2022-01-20')),
-        DateTimeRange(
-            str_to_date_time('2022-01-20'), str_to_date_time('2022-01-21'))]
+        DateTimeRange(str_to_date_time("2022-01-18"), str_to_date_time("2022-01-19")),
+        DateTimeRange(str_to_date_time("2022-01-19"), str_to_date_time("2022-01-20")),
+        DateTimeRange(str_to_date_time("2022-01-20"), str_to_date_time("2022-01-21")),
+    ]
 
 
 def test_get_daily_date_ranges():
     """Test daterange_generator returns DateTimeRange ranges."""
     start_date = date(year=2022, month=1, day=18)
     end_date = date(year=2022, month=1, day=21)
     daterange_generator = get_daily_date_ranges(
-        start_date=start_date,
-        end_date=end_date
+        start_date=start_date, end_date=end_date
     )
     result = [daterange for daterange in daterange_generator]
     assert result == [
-        DateTimeRange(
-            str_to_date_time('2022-01-18'), str_to_date_time('2022-01-19')),
-        DateTimeRange(
-            str_to_date_time('2022-01-19'), str_to_date_time('2022-01-20')),
-        DateTimeRange(
-            str_to_date_time('2022-01-20'), str_to_date_time('2022-01-21'))]
+        DateTimeRange(str_to_date_time("2022-01-18"), str_to_date_time("2022-01-19")),
+        DateTimeRange(str_to_date_time("2022-01-19"), str_to_date_time("2022-01-20")),
+        DateTimeRange(str_to_date_time("2022-01-20"), str_to_date_time("2022-01-21")),
+    ]
 
 
 def test_get_daily_date_range_till_yesterday():
     """
     Test get_daily_date_range_till_yesterday generates a DateTimeRange
     till yesterday.
     """
     start_date = date.today() - timedelta(days=3)
-    daterange_generator = get_daily_date_range_till_yesterday(
-        start_date=start_date)
+    daterange_generator = get_daily_date_range_till_yesterday(start_date=start_date)
     result = [daterange for daterange in daterange_generator]
     assert len(result) == 3
 
 
 def test_get_daily_date_ranges_yesterday():
     """
     Test get_daily_date_ranges_yesterday generates a DateTimeRange
     for only yesterday.
     """
-    today = datetime.strftime(datetime.now(), '%Y-%m-%d')
-    yesterday = datetime.strftime(
-        datetime.now() - timedelta(days=1), '%Y-%m-%d')
+    today = datetime.strftime(datetime.now(), "%Y-%m-%d")
+    yesterday = datetime.strftime(datetime.now() - timedelta(days=1), "%Y-%m-%d")
 
     daterange_generator = get_daily_date_range_yesterday()
     result = [daterange for daterange in daterange_generator]
     assert result[0].from_date == str_to_date_time(yesterday)
     assert result[0].to_date == str_to_date_time(today)
     assert len(result) == 1
 
 
 def test_get_daily_date_range_for_single_date():
     """
     Test get_daily_date_range_for_single_date returns a single DateTimeRange.
     """
     today = date.today()
     yesterday = date.today() - timedelta(days=1)
-    single_daily_date_range = get_daily_date_range_for_single_date(
-        date=yesterday
-    )
+    single_daily_date_range = get_daily_date_range_for_single_date(date=yesterday)
 
     assert isinstance(single_daily_date_range, DateTimeRange)
     assert single_daily_date_range.from_date.date() == yesterday
     assert single_daily_date_range.to_date.date() == today
 
 
 def test_get_monthly_date_range_for_single_date():
     """
     Test get_monthly_date_range_for_single_date returns a single DateTimeRange.
     """
-    first_day_of_month = datetime.strptime('2022-02-01', '%Y-%m-%d')
-    first_day_of_next_month = datetime.strptime('2022-03-01', '%Y-%m-%d')
-    input_date = datetime.strptime('2022-02-11', '%Y-%m-%d')
-    single_monthly_date_range = get_monthly_date_range_for_single_date(
-        date=input_date
-    )
+    first_day_of_month = datetime.strptime("2022-02-01", "%Y-%m-%d")
+    first_day_of_next_month = datetime.strptime("2022-03-01", "%Y-%m-%d")
+    input_date = datetime.strptime("2022-02-11", "%Y-%m-%d")
+    single_monthly_date_range = get_monthly_date_range_for_single_date(date=input_date)
     assert isinstance(single_monthly_date_range, DateTimeRange)
     assert single_monthly_date_range.from_date == first_day_of_month
     assert single_monthly_date_range.to_date == first_day_of_next_month
 
 
 def test_get_weekly_date_range_for_single_date():
     """
     Test get_monthly_date_range_for_single_date returns a single DateTimeRange.
     """
-    first_day_of_week = datetime.strptime('2022-10-03', '%Y-%m-%d')
-    first_day_of_next_week = datetime.strptime('2022-10-10', '%Y-%m-%d')
-    input_date = datetime.strptime('2022-10-07', '%Y-%m-%d')
+    first_day_of_week = datetime.strptime("2022-10-03", "%Y-%m-%d")
+    first_day_of_next_week = datetime.strptime("2022-10-10", "%Y-%m-%d")
+    input_date = datetime.strptime("2022-10-07", "%Y-%m-%d")
     single_weekly_date_range = get_weekly_date_range_for_single_date(
         date=input_date.date()
     )
     assert isinstance(single_weekly_date_range, DateTimeRange)
     assert single_weekly_date_range.from_date == first_day_of_week
     assert single_weekly_date_range.to_date == first_day_of_next_week
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_aggregator/test_mongo_aggregator.py` & `pipeline_telemetry-1.0.0/tests/test_aggregator/test_mongo_aggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""Module to test the momgo Aggregators.
-"""
+"""Module to test the momgo Aggregators."""
+
 from test_aggregator_data import TEST_TELEMETRY_SELECTOR
 
 from pipeline_telemetry import DailyAggregator, DailyMongoAggregator
 from pipeline_telemetry.storage import TelemetryMongoStorage
 
 
 def test_daily_mongo_aggregator_class_exists():
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_aggregator/test_partial_aggregator.py` & `pipeline_telemetry-1.0.0/tests/test_aggregator/test_partial_aggregator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,39 @@
-"""Module to test the DailyAggregator class.
-"""
+"""Module to test the DailyAggregator class."""
+
 from test_aggregator_data import TelemetryTestList
 
 from pipeline_telemetry import PartialToSingleAggregator, TelemetrySelector
 from pipeline_telemetry.data_classes import TelemetryModel
-from pipeline_telemetry.settings.date_ranges import \
-    get_daily_date_range_yesterday
+from pipeline_telemetry.settings.date_ranges import get_daily_date_range_yesterday
 
 keys_in_telemetry_list_params = [
-    'telemetry_type', 'category', 'sub_category', 'source_name',
-    'process_type', 'from_date_time', 'to_date_time']
+    "telemetry_type",
+    "category",
+    "sub_category",
+    "source_name",
+    "process_type",
+    "from_date_time",
+    "to_date_time",
+]
 
 
 def test_partial_to_daily_aggregator_exists():
     """Test that the PartialToDailyAggregator class exists."""
     assert PartialToSingleAggregator
 
 
 def test_run_aggregation():
     """Method to test a single aggregation."""
     telemetry_selector = TelemetrySelector(
-        category='test', sub_category='sub_test', source_name='source',
-        process_type='process_type')
+        category="test",
+        sub_category="sub_test",
+        source_name="source",
+        process_type="process_type",
+    )
     aggr = PartialToSingleAggregator(
-        telemetry_selector=telemetry_selector,
-        telemetry_storage=TelemetryTestList()
+        telemetry_selector=telemetry_selector, telemetry_storage=TelemetryTestList()
     )
-    result_telemetry = aggr._run_aggregation(
-        next(get_daily_date_range_yesterday()))
+    result_telemetry = aggr._run_aggregation(next(get_daily_date_range_yesterday()))
     assert isinstance(result_telemetry, TelemetryModel)
-    assert result_telemetry.telemetry['DATA_STORAGE'].base_counter == 3
-    assert result_telemetry.telemetry['DATA_STORAGE'].fail_counter == 1
+    assert result_telemetry.telemetry["DATA_STORAGE"].base_counter == 3
+    assert result_telemetry.telemetry["DATA_STORAGE"].fail_counter == 1
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_data.py` & `pipeline_telemetry-1.0.0/tests/test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 This module provides test data for the telemetry tests
 """
+
 from errors import ErrorCode, ListErrors, ReturnValueWithStatus
 
 from pipeline_telemetry import ProcessType, ProcessTypes, TelemetryCounter
-from pipeline_telemetry.settings.settings import \
-    DEFAULT_CREATE_DATA_SUB_PROCESS_TYPES
-from pipeline_telemetry.validators.abstract_validator_instruction import \
-    AbstractValidatorInstruction
+from pipeline_telemetry.settings.settings import DEFAULT_CREATE_DATA_SUB_PROCESS_TYPES
+from pipeline_telemetry.validators.abstract_validator_instruction import (
+    AbstractValidatorInstruction,
+)
 
 
 class InstructionTestClass(AbstractValidatorInstruction):
     """Instruction class for test purposes."""
 
     INSTRUCTION = "test_instruction"
 
@@ -21,15 +22,15 @@
     "category": "WEATHER",
     "sub_category": "DAILY_PREDICTIONS",
     "source_name": "load_weather_data",
     "process_type": ProcessTypes.CREATE_DATA_FROM_URL,
 }
 
 DEFAULT_TELEMETRY_MODEL_PARAMS = {
-    "telemetry_type": 'SINGLE TELEMETRY',
+    "telemetry_type": "SINGLE TELEMETRY",
     "category": "WEATHER",
     "sub_category": "DAILY_PREDICTIONS",
     "source_name": "load_weather_data",
     "process_type": ProcessTypes.CREATE_DATA_FROM_URL.name,
 }
 
 # custom process type for testing extending the default process types
@@ -117,11 +118,10 @@
 TEST_TC_MULT_PROCESS_TYPES_2 = TelemetryCounter(
     process_types=[TEST_PROCESS_TYPE],
     sub_process="RETRIEVE_RAW_DATA",
     counter_name="test_counter",
 )
 
 
-TEST_RESULT = [1, TEST_TELEMETRY_COUNTER, 2,
-               TEST_ERROR_TELEMETRY_COUNTER]
+TEST_RESULT = [1, TEST_TELEMETRY_COUNTER, 2, TEST_ERROR_TELEMETRY_COUNTER]
 
 TEST_RETURN_VALUE = ReturnValueWithStatus(result=TEST_RESULT)
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_decorator.py` & `pipeline_telemetry-1.0.0/tests/test_decorator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-"""Module to test decorator logic.
-"""
+"""Module to test decorator logic."""
+
 import pytest
 from test_data import DEFAULT_TELEMETRY_PARAMS
 
-from pipeline_telemetry.decorator import add_mongo_single_usage_telemetry, \
-    add_mongo_telemetry, add_single_usage_telemetry, add_telemetry
+from pipeline_telemetry.decorator import (
+    add_mongo_single_usage_telemetry,
+    add_mongo_telemetry,
+    add_single_usage_telemetry,
+    add_telemetry,
+)
 from pipeline_telemetry.settings import exceptions
 from pipeline_telemetry.settings import settings as st
 from pipeline_telemetry.storage.memory import TelemetryInMemoryStorage
 from pipeline_telemetry.storage.mongo import TelemetryMongoStorage
 
 
 def test_default_decorator():
@@ -29,16 +33,17 @@
 
 
 def test_mongo_telemetry_decorator(mocker):
     """
     Test that mongo decorator does not effect decorated method result
     but sets the telemetry property.
     """
-    mocker.patch("pipeline_telemetry.decorator.TelemetryMongoStorage",
-                 TelemetryInMemoryStorage)
+    mocker.patch(
+        "pipeline_telemetry.decorator.TelemetryMongoStorage", TelemetryInMemoryStorage
+    )
 
     class DecoratorTest:
         @add_mongo_telemetry(DEFAULT_TELEMETRY_PARAMS)
         def decorated_method(self):
             return "method result"
 
     class_instance = DecoratorTest()
@@ -48,16 +53,15 @@
 
 
 def test_mongo_telemetry_decorator_sets_mongo_storage_class(mocker):
     """
     Test that mongo decorator sets the mongo storage class
     """
     mongo_module_path = "pipeline_telemetry.storage.mongo."
-    mocker.patch(mongo_module_path + "TelemetryMongoModel.save",
-                 return_value=None)
+    mocker.patch(mongo_module_path + "TelemetryMongoModel.save", return_value=None)
 
     class DecoratorTest:
         @add_mongo_telemetry(DEFAULT_TELEMETRY_PARAMS)
         def decorated_method(self):
             return self._telemetry.storage_class
 
     assert issubclass(DecoratorTest().decorated_method(), TelemetryMongoStorage)
@@ -65,16 +69,15 @@
 
 def test_calling_mongo_decorated_method_from_within_decorated_method(mocker):
     """
     Test that when telemetry is active it is not changed by any other telemetry
     decorated method that is being called.
     """
     mongo_module_path = "pipeline_telemetry.storage.mongo."
-    mocker.patch(mongo_module_path + "TelemetryMongoModel.save",
-                 return_value=None)
+    mocker.patch(mongo_module_path + "TelemetryMongoModel.save", return_value=None)
 
     changed_telemetry_params = DEFAULT_TELEMETRY_PARAMS.copy() | {
         "category": "OTHER VALUE",
     }
 
     class DecoratorTestMongo:
         @add_mongo_telemetry(DEFAULT_TELEMETRY_PARAMS)
@@ -83,16 +86,15 @@
 
         @add_mongo_telemetry(changed_telemetry_params)
         def second_decorated_method(self):
             return self._telemetry.category
 
     class_instance = DecoratorTestMongo()
     assert not hasattr(class_instance, "_telemetry")
-    assert class_instance.decorated_method() == \
-        DEFAULT_TELEMETRY_PARAMS.get("category")
+    assert class_instance.decorated_method() == DEFAULT_TELEMETRY_PARAMS.get("category")
     assert hasattr(class_instance, "_telemetry")
 
 
 def test_calling_decorated_method_from_within_decorated_method():
     """
     Test that when a telemetry instance created with add_telemetry is
     active it is not changed by any other telemetry decorated method that is
@@ -109,32 +111,32 @@
 
         @add_telemetry(changed_telemetry_params)
         def second_decorated_method(self):
             return self._telemetry.category
 
     class_instance = DecoratorTest()
     assert not hasattr(class_instance, "_telemetry")
-    assert class_instance.decorated_method() == \
-        DEFAULT_TELEMETRY_PARAMS.get("category")
+    assert class_instance.decorated_method() == DEFAULT_TELEMETRY_PARAMS.get("category")
     assert hasattr(class_instance, "_telemetry")
 
 
 def test_single_usage_decorator_raises_params_not_def_exc():
     """
     Test that add_single_usage_telemetry decorator raises an exception when
     no telemetry params are defined in class of class instance.
     """
+
     class DecoratorTest:
         @add_single_usage_telemetry()
         def decorated_method(self):
             return "method result"
 
     with pytest.raises(exceptions.ClassTelemetryParamsNotDefined) as excep:
         DecoratorTest().decorated_method()
-    assert 'Telemetry params not defined' in str(excep)
+    assert "Telemetry params not defined" in str(excep)
 
 
 def test_single_usage_class_telemetry_settings():
     """
     Test that add_single_usage_telemetry decorator can use class defined
     telemetry settings.
     """
@@ -153,15 +155,15 @@
 
 
 def test_single_usage_telemetry_settings_with_sub_process():
     """
     Test that add_single_usage_telemetry decorator can use class defined
     telemetry settings.
     """
-    sub_process = DEFAULT_TELEMETRY_PARAMS['process_type'].sub_processes[0]
+    sub_process = DEFAULT_TELEMETRY_PARAMS["process_type"].sub_processes[0]
 
     class DecoratorTest:
         TELEMETRY_PARAMS = DEFAULT_TELEMETRY_PARAMS
 
         @add_single_usage_telemetry(sub_process=sub_process)
         def decorated_method(self):
             return self._telemetry
@@ -173,16 +175,15 @@
 
 
 def test_single_usage_telemetry_settings_with_mongho_storage(mocker):
     """
     Test that mongo decorator sets the mongo storage class
     """
     mongo_module_path = "pipeline_telemetry.storage.mongo."
-    mocker.patch(mongo_module_path + "TelemetryMongoModel.save",
-                 return_value=None)
+    mocker.patch(mongo_module_path + "TelemetryMongoModel.save", return_value=None)
 
     class DecoratorTest:
         TELEMETRY_PARAMS = DEFAULT_TELEMETRY_PARAMS
 
         @add_mongo_single_usage_telemetry()
         def decorated_method(self):
             return self._telemetry.storage_class
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_helpers.py` & `pipeline_telemetry-1.0.0/tests/test_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,28 @@
-"""Module to test pipeline telemetry helper methods.
-"""
+"""Module to test pipeline telemetry helper methods."""
+
 import test_data as td
 from errors import ReturnValueWithErrorStatus, ReturnValueWithStatus
 
 import pipeline_telemetry.helper as HP
-from pipeline_telemetry import Telemetry, add_errors_from_return_value, \
-    add_telemetry_counters_from_return_value, increase_base_count, \
-    increase_fail_count, is_telemetry_counter, process_return_value
-from pipeline_telemetry.settings.settings import BASE_COUNT_KEY, \
-    COUNTERS_KEY, ERRORS_KEY, FAIL_COUNT_KEY
+from pipeline_telemetry import (
+    Telemetry,
+    add_errors_from_return_value,
+    add_telemetry_counters_from_return_value,
+    increase_base_count,
+    increase_fail_count,
+    is_telemetry_counter,
+    process_return_value,
+)
+from pipeline_telemetry.settings.settings import (
+    BASE_COUNT_KEY,
+    COUNTERS_KEY,
+    ERRORS_KEY,
+    FAIL_COUNT_KEY,
+)
 
 
 class HelperTest:
     pass
 
 
 def test_add_result_value_with_status_without_errors():
@@ -22,190 +32,182 @@
     """
     test_obj = HelperTest()
     test_obj._telemetry = Telemetry(**td.DEFAULT_TELEMETRY_PARAMS)
     return_value_without_error = ReturnValueWithStatus(result=[])
     add_errors_from_return_value(
         object_with_telemetry=test_obj,
         sub_process="RETRIEVE_RAW_DATA",
-        return_value=return_value_without_error)
+        return_value=return_value_without_error,
+    )
     telemetry_data = test_obj._telemetry.get("RETRIEVE_RAW_DATA")
     assert not getattr(telemetry_data, ERRORS_KEY)
 
 
 def test_add_result_value_with_status_with_one_error():
     """
     Test adding the ResultValueWithStatus instance with an error in it to the
     telemetry adds the actual error to the telemetry object.
     """
     test_obj = HelperTest()
     test_obj._telemetry = Telemetry(**td.DEFAULT_TELEMETRY_PARAMS)
-    return_value_with_error = ReturnValueWithErrorStatus(
-        error=td.TEST_ERROR_CODE)
+    return_value_with_error = ReturnValueWithErrorStatus(error=td.TEST_ERROR_CODE)
     add_errors_from_return_value(
         object_with_telemetry=test_obj,
         sub_process="RETRIEVE_RAW_DATA",
-        return_value=return_value_with_error)
+        return_value=return_value_with_error,
+    )
     telemetry_data = test_obj._telemetry.get("RETRIEVE_RAW_DATA")
     assert td.TEST_ERROR_CODE.code in getattr(telemetry_data, ERRORS_KEY)
-    assert getattr(telemetry_data, ERRORS_KEY).get(
-        td.TEST_ERROR_CODE.code) == 1
+    assert getattr(telemetry_data, ERRORS_KEY).get(td.TEST_ERROR_CODE.code) == 1
 
 
 def test_add_result_value_with_status_with_errors():
     """
     Test adding the ResultValueWithStatus instance with 2 errors in it to the
     telemetry adds the actual errors to the telemetry object.
     """
     test_obj = HelperTest()
     test_obj._telemetry = Telemetry(**td.DEFAULT_TELEMETRY_PARAMS)
-    return_value_with_error = ReturnValueWithErrorStatus(
-        error=td.TEST_ERROR_CODE)
+    return_value_with_error = ReturnValueWithErrorStatus(error=td.TEST_ERROR_CODE)
     # add the second error code to return_value_with_error
     return_value_with_error.add_error(td.TEST_ERROR_CODE)
     add_errors_from_return_value(
         object_with_telemetry=test_obj,
         sub_process="RETRIEVE_RAW_DATA",
-        return_value=return_value_with_error)
+        return_value=return_value_with_error,
+    )
     telemetry_data = test_obj._telemetry.get("RETRIEVE_RAW_DATA")
-    assert getattr(telemetry_data, ERRORS_KEY).get(
-        td.TEST_ERROR_CODE.code) == 2
+    assert getattr(telemetry_data, ERRORS_KEY).get(td.TEST_ERROR_CODE.code) == 2
 
 
 def test_process_telemetry_counters_in_return_value():
     """
     Test that when a ResultValueWithStatus instance with 2 telemetry counters
-    (of which one with an error) in the result is processed by process_telemetry_counters_in_return_value both the error counter and
+    (of which one with an error) in the result is processed by
+    process_telemetry_counters_in_return_value both the error counter and
     counter are increased
-
     """
     test_obj = HelperTest()
     test_obj._telemetry = Telemetry(**td.DEFAULT_TELEMETRY_PARAMS)
     add_telemetry_counters_from_return_value(
-        object_with_telemetry=test_obj,
-        return_value=td.TEST_RETURN_VALUE)
+        object_with_telemetry=test_obj, return_value=td.TEST_RETURN_VALUE
+    )
     telemetry_data = test_obj._telemetry.get("RETRIEVE_RAW_DATA")
     assert getattr(telemetry_data, ERRORS_KEY) is not None
-    assert getattr(telemetry_data, COUNTERS_KEY).get('test_counter') == 1
+    assert getattr(telemetry_data, COUNTERS_KEY).get("test_counter") == 1
 
 
 def test_process_telemetry_counters_in_return_value_returns_list():
     """
     Test that when a ResultValueWithStatus instance with 2 telemetry counters
     in the result is processed by process_telemetry_counters_in_return_value
     the result list without TelemetryCounters is returned.
     """
     test_obj = HelperTest()
     test_obj._telemetry = Telemetry(**td.DEFAULT_TELEMETRY_PARAMS)
     res_without_telem_counters = add_telemetry_counters_from_return_value(
-        object_with_telemetry=test_obj,
-        return_value=td.TEST_RETURN_VALUE)
+        object_with_telemetry=test_obj, return_value=td.TEST_RETURN_VALUE
+    )
     assert res_without_telem_counters == [
-        res for res in td.TEST_RETURN_VALUE.result
-        if not is_telemetry_counter(res)]
+        res for res in td.TEST_RETURN_VALUE.result if not is_telemetry_counter(res)
+    ]
 
 
 def test_increase_base_count():
     """
     Test increase base count without increment increase base counter with 1 for
     a given sub process.
     """
     test_obj = HelperTest()
     test_obj._telemetry = Telemetry(**td.DEFAULT_TELEMETRY_PARAMS)
-    increase_base_count(
-        object_with_telemetry=test_obj,
-        sub_process="RETRIEVE_RAW_DATA")
+    increase_base_count(object_with_telemetry=test_obj, sub_process="RETRIEVE_RAW_DATA")
     telemetry_data = test_obj._telemetry.get("RETRIEVE_RAW_DATA")
     assert getattr(telemetry_data, BASE_COUNT_KEY) == 1
 
 
 def test_increase_base_count_with_increment():
     """
     Test increase base count with increment 2 increases base counter with 2 for
     a given sub process.
     """
     test_obj = HelperTest()
     test_obj._telemetry = Telemetry(**td.DEFAULT_TELEMETRY_PARAMS)
     increase_base_count(
-        object_with_telemetry=test_obj,
-        sub_process="RETRIEVE_RAW_DATA",
-        increment=2)
+        object_with_telemetry=test_obj, sub_process="RETRIEVE_RAW_DATA", increment=2
+    )
     telemetry_data = test_obj._telemetry.get("RETRIEVE_RAW_DATA")
     assert getattr(telemetry_data, BASE_COUNT_KEY) == 2
 
 
 def test_increase_fail_count():
     """
     Test increase fail count without increment increases teh fail counter with
     1 for a given sub process.
     """
     test_obj = HelperTest()
     test_obj._telemetry = Telemetry(**td.DEFAULT_TELEMETRY_PARAMS)
     test_obj._telemetry._initialize_sub_process("RETRIEVE_RAW_DATA")
-    increase_fail_count(
-        object_with_telemetry=test_obj,
-        sub_process="RETRIEVE_RAW_DATA")
+    increase_fail_count(object_with_telemetry=test_obj, sub_process="RETRIEVE_RAW_DATA")
     telemetry_data = test_obj._telemetry.get("RETRIEVE_RAW_DATA")
     assert getattr(telemetry_data, FAIL_COUNT_KEY) == 1
 
 
 def test_process_return_value(mocker):
     """
     Test that process_return_value returns helper method returns the list
     retrieved add_telemetry_counters_from_return_value helper method.
     """
     mocker.patch(
-        ("pipeline_telemetry.helper."
-         "add_telemetry_counters_from_return_value"),
-        return_value=['list with values'])
-    mocker.patch(
-        ("pipeline_telemetry.helper."
-         "add_errors_from_return_value"),
-        return_value=None)
+        ("pipeline_telemetry.helper." "add_telemetry_counters_from_return_value"),
+        return_value=["list with values"],
+    )
+    mocker.patch(
+        ("pipeline_telemetry.helper." "add_errors_from_return_value"), return_value=None
+    )
     assert process_return_value(
         object_with_telemetry=None,
         sub_process="na for this test",
-        return_value=td.TEST_RETURN_VALUE) == ['list with values']
+        return_value=td.TEST_RETURN_VALUE,
+    ) == ["list with values"]
 
 
 def test_process_return_value_processes_the_errors(mocker):
     """
     Test process_return_value calls the add_errors_from_return_value method.
     """
     mocker.patch(
-        ("pipeline_telemetry.helper."
-         "add_telemetry_counters_from_return_value"),
-        return_value=None)
-    mocker.patch(
-        ("pipeline_telemetry.helper."
-         "add_errors_from_return_value"),
-        return_value=None)
-    process_telemetry_spy = mocker.spy(
-        HP, "add_telemetry_counters_from_return_value")
+        ("pipeline_telemetry.helper." "add_telemetry_counters_from_return_value"),
+        return_value=None,
+    )
+    mocker.patch(
+        ("pipeline_telemetry.helper." "add_errors_from_return_value"), return_value=None
+    )
+    process_telemetry_spy = mocker.spy(HP, "add_telemetry_counters_from_return_value")
 
     process_return_value(
         object_with_telemetry=None,
         sub_process="na for this test",
-        return_value=td.TEST_RETURN_VALUE)
+        return_value=td.TEST_RETURN_VALUE,
+    )
     assert process_telemetry_spy.called
 
 
 def test_process_return_value_processes_the_telemetry_counters(mocker):
     """
     Test process_return_value calls the
     process_telemetry_counters_in_return_value method.
     """
     mocker.patch(
-        ("pipeline_telemetry.helper."
-         "add_telemetry_counters_from_return_value"),
-        return_value=None)
-    mocker.patch(
-        ("pipeline_telemetry.helper."
-         "add_errors_from_return_value"),
-        return_value=None)
-    process_telemetry_spy = mocker.spy(
-        HP, "add_telemetry_counters_from_return_value")
+        ("pipeline_telemetry.helper." "add_telemetry_counters_from_return_value"),
+        return_value=None,
+    )
+    mocker.patch(
+        ("pipeline_telemetry.helper." "add_errors_from_return_value"), return_value=None
+    )
+    process_telemetry_spy = mocker.spy(HP, "add_telemetry_counters_from_return_value")
 
     process_return_value(
         object_with_telemetry=None,
         sub_process="na for this test",
-        return_value=td.TEST_RETURN_VALUE)
+        return_value=td.TEST_RETURN_VALUE,
+    )
     assert process_telemetry_spy.called
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_integration/test_int_telemetry.py` & `pipeline_telemetry-1.0.0/tests/test_integration/test_int_telemetry.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,86 +1,76 @@
-"""Module to run integration test for telemetry module
-"""
+"""Module to run integration test for telemetry module"""
+
 from test_data import DEFAULT_TELEMETRY_PARAMS
-from test_integration_data import BASIC_RETRIEVE_DATA_TEST, \
-    ITEMS_FIELD_HAS_DICT_TEST, MISSING_KEY_RETRIEVE_DATA_TEST, \
-    MUST_HAVE_KEY_IN_ITEMS_TEST, NO_ITEMS_HAVE_MUST_HAVE_KEY_TEST
+from test_integration_data import (
+    BASIC_RETRIEVE_DATA_TEST,
+    ITEMS_FIELD_HAS_DICT_TEST,
+    MISSING_KEY_RETRIEVE_DATA_TEST,
+    MUST_HAVE_KEY_IN_ITEMS_TEST,
+    NO_ITEMS_HAVE_MUST_HAVE_KEY_TEST,
+)
 
 from pipeline_telemetry.main import Telemetry
 
 
 def test_basic_test_data():
     """Test data basic data test returns correct telemetry."""
     telemetry_rules = BASIC_RETRIEVE_DATA_TEST.validation_rules
-    telemetry_params = DEFAULT_TELEMETRY_PARAMS | \
-        {'telemetry_rules': telemetry_rules}
+    telemetry_params = DEFAULT_TELEMETRY_PARAMS | {"telemetry_rules": telemetry_rules}
     telemetry = Telemetry(**telemetry_params)
-    telemetry.increase_sub_process_base_count('RETRIEVE_RAW_DATA')
-    telemetry.add('RETRIEVE_RAW_DATA', BASIC_RETRIEVE_DATA_TEST.data, None)
+    telemetry.increase_sub_process_base_count("RETRIEVE_RAW_DATA")
+    telemetry.add("RETRIEVE_RAW_DATA", BASIC_RETRIEVE_DATA_TEST.data, None)
     telemetry.save_and_close()
-    assert BASIC_RETRIEVE_DATA_TEST.validate_telemetry_data(
-        telemetry)
+    assert BASIC_RETRIEVE_DATA_TEST.validate_telemetry_data(telemetry)
 
 
 def test_missing_key_integration_test():
     """Test telemetry returns correct telemetry object when key is missing."""
     telemetry_rules = MISSING_KEY_RETRIEVE_DATA_TEST.validation_rules
-    telemetry_params = DEFAULT_TELEMETRY_PARAMS | \
-        {'telemetry_rules': telemetry_rules}
+    telemetry_params = DEFAULT_TELEMETRY_PARAMS | {"telemetry_rules": telemetry_rules}
     telemetry = Telemetry(**telemetry_params)
-    telemetry.increase_sub_process_base_count('RETRIEVE_RAW_DATA')
-    telemetry.add('RETRIEVE_RAW_DATA',
-                  MISSING_KEY_RETRIEVE_DATA_TEST.data, None)
+    telemetry.increase_sub_process_base_count("RETRIEVE_RAW_DATA")
+    telemetry.add("RETRIEVE_RAW_DATA", MISSING_KEY_RETRIEVE_DATA_TEST.data, None)
     telemetry.save_and_close()
-    assert MISSING_KEY_RETRIEVE_DATA_TEST.validate_telemetry_data(
-        telemetry)
+    assert MISSING_KEY_RETRIEVE_DATA_TEST.validate_telemetry_data(telemetry)
 
 
 def test_must_have_key_in_items_integration_test():
     """
     Test telemetry returns correct telemetry object when key is missing in one
     of the items.
     """
     telemetry_rules = MUST_HAVE_KEY_IN_ITEMS_TEST.validation_rules
-    telemetry_params = DEFAULT_TELEMETRY_PARAMS | \
-        {'telemetry_rules': telemetry_rules}
+    telemetry_params = DEFAULT_TELEMETRY_PARAMS | {"telemetry_rules": telemetry_rules}
     telemetry = Telemetry(**telemetry_params)
-    telemetry.increase_sub_process_base_count('RETRIEVE_RAW_DATA')
-    telemetry.add('RETRIEVE_RAW_DATA',
-                  MUST_HAVE_KEY_IN_ITEMS_TEST.data, None)
+    telemetry.increase_sub_process_base_count("RETRIEVE_RAW_DATA")
+    telemetry.add("RETRIEVE_RAW_DATA", MUST_HAVE_KEY_IN_ITEMS_TEST.data, None)
     telemetry.save_and_close()
-    assert MUST_HAVE_KEY_IN_ITEMS_TEST.validate_telemetry_data(
-        telemetry)
+    assert MUST_HAVE_KEY_IN_ITEMS_TEST.validate_telemetry_data(telemetry)
 
 
 def test_no_items_have_must_have_key_in_items_integration_test():
     """
     Test telemetry returns correct telemetry object when no item has the
     correct key.
     """
     telemetry_rules = NO_ITEMS_HAVE_MUST_HAVE_KEY_TEST.validation_rules
-    telemetry_params = DEFAULT_TELEMETRY_PARAMS | \
-        {'telemetry_rules': telemetry_rules}
+    telemetry_params = DEFAULT_TELEMETRY_PARAMS | {"telemetry_rules": telemetry_rules}
     telemetry = Telemetry(**telemetry_params)
-    telemetry.increase_sub_process_base_count('RETRIEVE_RAW_DATA')
-    telemetry.add('RETRIEVE_RAW_DATA',
-                  NO_ITEMS_HAVE_MUST_HAVE_KEY_TEST.data, None)
+    telemetry.increase_sub_process_base_count("RETRIEVE_RAW_DATA")
+    telemetry.add("RETRIEVE_RAW_DATA", NO_ITEMS_HAVE_MUST_HAVE_KEY_TEST.data, None)
     telemetry.save_and_close()
-    assert NO_ITEMS_HAVE_MUST_HAVE_KEY_TEST.validate_telemetry_data(
-        telemetry)
+    assert NO_ITEMS_HAVE_MUST_HAVE_KEY_TEST.validate_telemetry_data(telemetry)
 
 
 def test_items_has_dict_field_test():
     """
     Test telemetry returns correct telemetry object when items field contains
     a dict field.
     """
     telemetry_rules = ITEMS_FIELD_HAS_DICT_TEST.validation_rules
-    telemetry_params = DEFAULT_TELEMETRY_PARAMS | \
-        {'telemetry_rules': telemetry_rules}
+    telemetry_params = DEFAULT_TELEMETRY_PARAMS | {"telemetry_rules": telemetry_rules}
     telemetry = Telemetry(**telemetry_params)
-    telemetry.increase_sub_process_base_count('RETRIEVE_RAW_DATA')
-    telemetry.add('RETRIEVE_RAW_DATA',
-                  ITEMS_FIELD_HAS_DICT_TEST.data, None)
+    telemetry.increase_sub_process_base_count("RETRIEVE_RAW_DATA")
+    telemetry.add("RETRIEVE_RAW_DATA", ITEMS_FIELD_HAS_DICT_TEST.data, None)
     telemetry.save_and_close()
-    assert ITEMS_FIELD_HAS_DICT_TEST.validate_telemetry_data(
-        telemetry)
+    assert ITEMS_FIELD_HAS_DICT_TEST.validate_telemetry_data(telemetry)
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_integration/test_integration_data.py` & `pipeline_telemetry-1.0.0/tests/test_integration/test_integration_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""Module to define test data for the integration tests
-"""
+"""Module to define test data for the integration tests"""
+
 from dataclasses import dataclass
 
 from pipeline_telemetry import Telemetry
 from pipeline_telemetry.data_classes import TelemetryData
 from pipeline_telemetry.settings import settings as st
 
 
@@ -41,71 +41,75 @@
     validation_rules={
         "RETRIEVE_RAW_DATA": {
             "has_key": {"field_name": "items"},
             "validate_entries": {"field_name": "items", "expected_count": 4},
         }
     },
     result_field="RETRIEVE_RAW_DATA",
-    expected_result=TelemetryData(**{
-        "base_counter": 1,
-        "fail_counter": 0
-    })
+    expected_result=TelemetryData(**{"base_counter": 1, "fail_counter": 0}),
 )
 
 MISSING_KEY_RETRIEVE_DATA_TEST = IntegrationTestData(
     data={"no items key": []},
-    validation_rules={
-        "RETRIEVE_RAW_DATA": {"has_key": {"field_name": "items"}}},
+    validation_rules={"RETRIEVE_RAW_DATA": {"has_key": {"field_name": "items"}}},
     result_field="RETRIEVE_RAW_DATA",
-    expected_result=TelemetryData(**{
-        "base_counter": 1,
-        "fail_counter": 0,
-        st.ERRORS_KEY: {"HAS_KEY_ERR_0001@KEY_<items>": 1}
-    }),
+    expected_result=TelemetryData(
+        **{
+            "base_counter": 1,
+            "fail_counter": 0,
+            st.ERRORS_KEY: {"HAS_KEY_ERR_0001@KEY_<items>": 1},
+        }
+    ),
 )
 
 
 MUST_HAVE_KEY_IN_ITEMS_TEST = IntegrationTestData(
     data={"items": [{"key": 1}, {"no_key": 2}]},
     validation_rules={
         "RETRIEVE_RAW_DATA": {
             "entries_have_key": {"field_name": "items", "must_have_key": "key"}
         }
     },
     result_field="RETRIEVE_RAW_DATA",
-    expected_result=TelemetryData(**{
-        "base_counter": 1,
-        "fail_counter": 0,
-        st.ERRORS_KEY: {"ENTRIES_HAVE_KEY_ERR_003@KEY_<items__key>": 1}
-    }),
+    expected_result=TelemetryData(
+        **{
+            "base_counter": 1,
+            "fail_counter": 0,
+            st.ERRORS_KEY: {"ENTRIES_HAVE_KEY_ERR_003@KEY_<items__key>": 1},
+        }
+    ),
 )
 
 NO_ITEMS_HAVE_MUST_HAVE_KEY_TEST = IntegrationTestData(
     data={"items": [{"no_key": 1}, {"no_key": 2}]},
     validation_rules={
         "RETRIEVE_RAW_DATA": {
             "entries_have_key": {"field_name": "items", "must_have_key": "key"}
         }
     },
     result_field="RETRIEVE_RAW_DATA",
-    expected_result=TelemetryData(**{
-        "base_counter": 1,
-        "fail_counter": 0,
-        st.ERRORS_KEY: {"ENTRIES_HAVE_KEY_ERR_003@KEY_<items__key>": 2}
-    }),
+    expected_result=TelemetryData(
+        **{
+            "base_counter": 1,
+            "fail_counter": 0,
+            st.ERRORS_KEY: {"ENTRIES_HAVE_KEY_ERR_003@KEY_<items__key>": 2},
+        }
+    ),
 )
 
 
 ITEMS_FIELD_HAS_DICT_TEST = IntegrationTestData(
     data={"items": {"key": 1, "no_key": 2}},
     validation_rules={
         "RETRIEVE_RAW_DATA": {
             "entries_have_key": {"field_name": "items", "must_have_key": "key"}
         }
     },
     result_field="RETRIEVE_RAW_DATA",
-    expected_result=TelemetryData(**{
-        "base_counter": 1,
-        "fail_counter": 0,
-        st.ERRORS_KEY: {"ENTRIES_HAVE_KEY_ERR_002@KEY_<items>": 1},
-    }),
+    expected_result=TelemetryData(
+        **{
+            "base_counter": 1,
+            "fail_counter": 0,
+            st.ERRORS_KEY: {"ENTRIES_HAVE_KEY_ERR_002@KEY_<items>": 1},
+        }
+    ),
 )
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_mixin.py` & `pipeline_telemetry-1.0.0/tests/test_mixin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module to test telemetry mixin class for pipeline telemetry module.
 """
+
 from test_data import DEFAULT_TELEMETRY_PARAMS
 
 import pipeline_telemetry.mixin as MX
 from pipeline_telemetry.main import Telemetry
 
 
 def test_telemetry_mixin_exists():
@@ -13,73 +14,79 @@
 
 
 def test_set_source_name():
     """
     test method set_telemetry_source_name changes the telemetry
     source name attribute
     """
+
     class TelTest(MX.TelemetryMixin):
         def __init__(self):
             self._telemetry = Telemetry(**DEFAULT_TELEMETRY_PARAMS)
 
         def get_source_name(self):
             return self._telemetry.telemetry.source_name
 
     tel_test = TelTest()
-    test_source_name = 'abcd'
+    test_source_name = "abcd"
     assert not tel_test.get_source_name() == test_source_name
     tel_test.set_telemetry_source_name(test_source_name)
     assert tel_test.get_source_name() == test_source_name
 
 
 def test_process_errors_from_return_value(mocker):
     """
     Test method process_errors_from_return_value calls helper method
     add_errors_from_return_value
     """
     mocker.patch(
-        ("pipeline_telemetry.mixin."
-         "add_errors_from_return_value"),
-        return_value=None)
-    add_errors_spy = mocker.spy(
-        MX, "add_errors_from_return_value")
+        ("pipeline_telemetry.mixin." "add_errors_from_return_value"), return_value=None
+    )
+    add_errors_spy = mocker.spy(MX, "add_errors_from_return_value")
 
     MX.TelemetryMixin().process_errors_from_return_value(
-        sub_process='TEST',
-        return_value='test')
+        sub_process="TEST", return_value="test"
+    )
     assert add_errors_spy.called
 
 
 def test_process_telemetry_counters_from_return_value(mocker):
     """
     Test method process_telemetry_counters_from_return_value calls helper
     method add_telemetry_counters_from_return_value
     """
     mocker.patch(
-        ("pipeline_telemetry.mixin."
-         "add_telemetry_counters_from_return_value"),
-        return_value='correct return object')
+        ("pipeline_telemetry.mixin." "add_telemetry_counters_from_return_value"),
+        return_value="correct return object",
+    )
     add_telemetry_counters_spy = mocker.spy(
-        MX, "add_telemetry_counters_from_return_value")
+        MX, "add_telemetry_counters_from_return_value"
+    )
 
     result = MX.TelemetryMixin().process_telemetry_counters_from_return_value(
-        return_value='test')
+        return_value="test"
+    )
     assert add_telemetry_counters_spy.called
-    assert result == 'correct return object'
+    assert result == "correct return object"
 
 
 def test_process_telemetry_counters_from_result_list(mocker):
     """
     Test method process_telemetry_counters_from_result_list calls mixin
     method process_telemetry_counters_from_return_value
     """
     mocker.patch(
-        ("pipeline_telemetry.mixin.TelemetryMixin."
-         "process_telemetry_counters_from_return_value"),
-        return_value='correct return object')
+        (
+            "pipeline_telemetry.mixin.TelemetryMixin."
+            "process_telemetry_counters_from_return_value"
+        ),
+        return_value="correct return object",
+    )
     process_telemetry_counters_spy = mocker.spy(
-        MX.TelemetryMixin, "process_telemetry_counters_from_return_value")
+        MX.TelemetryMixin, "process_telemetry_counters_from_return_value"
+    )
 
     result = MX.TelemetryMixin().process_telemetry_counters_from_list(
-        result_list=['test'])
+        result_list=["test"]
+    )
     assert process_telemetry_counters_spy.called
-    assert result == 'correct return object'
+    assert result == "correct return object"
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_process_types.py` & `pipeline_telemetry-1.0.0/tests/test_process_types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-"""Module to test processtype logic.
-"""
+"""Module to test processtype logic."""
+
 import pytest
 from test_data import TEST_PROCESS_TYPE
 
 from pipeline_telemetry.settings import exceptions
 from pipeline_telemetry.settings.process_type import ProcessTypes
-from pipeline_telemetry.settings.settings import \
-    DEFAULT_CREATE_DATA_SUB_PROCESS_TYPES
+from pipeline_telemetry.settings.settings import DEFAULT_CREATE_DATA_SUB_PROCESS_TYPES
 
 
 def test_process_type_class_exists():
     """Test that process types class exists."""
     assert ProcessTypes
 
 
@@ -25,51 +24,52 @@
 
 
 def test_calling_name_property_on_a_process_type_returns_a_str():
     """
     Test that calling name property on a process type returns the
     process_type name.
     """
-    assert ProcessTypes.CREATE_DATA_FROM_URL.name == \
-        'create_data_from_url'
+    assert ProcessTypes.CREATE_DATA_FROM_URL.name == "create_data_from_url"
 
 
 def test_calling_sub_processes_property_on_a_process_type_returns_a_list():
     """
     Test that calling sub_processes property on a process type returns the
     list of sub_processes.
     """
-    assert ProcessTypes.CREATE_DATA_FROM_URL.sub_processes == \
-        DEFAULT_CREATE_DATA_SUB_PROCESS_TYPES
+    assert (
+        ProcessTypes.CREATE_DATA_FROM_URL.sub_processes
+        == DEFAULT_CREATE_DATA_SUB_PROCESS_TYPES
+    )
 
 
 def test_registering_process_type_success():
     """
     Test that a processtype can be registered
     """
     assert not ProcessTypes.is_registered(TEST_PROCESS_TYPE)
-    ProcessTypes.register_process_type('TEST_PROCESS_TYPE', TEST_PROCESS_TYPE)
+    ProcessTypes.register_process_type("TEST_PROCESS_TYPE", TEST_PROCESS_TYPE)
     assert ProcessTypes.is_registered(TEST_PROCESS_TYPE)
 
 
 def test_registering_process_type_raises_exception():
     """
     Test that registering a processtype with a processtype of wrong class
     raises an exception.
     """
     with pytest.raises(exceptions.ProcessTypeMustBeOfClassProcessType):
-        ProcessTypes.register_process_type('TEST_PROCESS_TYPE', 'process_type')
+        ProcessTypes.register_process_type("TEST_PROCESS_TYPE", "process_type")
 
 
 def test_registering_process_types_with_class_instance_raises_exception():
     """
     Test that registering a process types enumerator with a class instance    raises an exception.
     """
     with pytest.raises(exceptions.ProcessTypesMustBeOfClassBaseEnumertor):
-        ProcessTypes.register_process_types('process_type')
+        ProcessTypes.register_process_types("process_type")
 
 
 def test_registering_process_types_with_wrong_class_raises_exception():
     """
     Test that registering a process types enumerator with a wrong class
     raises an exception.
     """
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_settings/test_date_time_ranges.py` & `pipeline_telemetry-1.0.0/tests/test_settings/test_date_time_ranges.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,152 +1,143 @@
-""" Module for testing date_ranges functions.
-"""
+"""Module for testing date_ranges functions."""
+
 from datetime import date, datetime, timedelta
 
-from pipeline_telemetry.settings.date_ranges import DateTimeRange, \
-    date_range_generator, get_daily_date_range_for_single_date, \
-    get_daily_date_range_till_yesterday, get_daily_date_range_yesterday, \
-    get_daily_date_ranges, get_monthly_date_range_for_single_date, \
-    get_weekly_date_range_for_single_date
+from pipeline_telemetry.settings.date_ranges import (
+    DateTimeRange,
+    date_range_generator,
+    get_daily_date_range_for_single_date,
+    get_daily_date_range_till_yesterday,
+    get_daily_date_range_yesterday,
+    get_daily_date_ranges,
+    get_monthly_date_range_for_single_date,
+    get_weekly_date_range_for_single_date,
+)
 
 
 def str_to_date_time(date_str: str) -> datetime:
-    return datetime.strptime(date_str, '%Y-%m-%d')
+    return datetime.strptime(date_str, "%Y-%m-%d")
 
 
 def str_to_date(date_str: str) -> date:
     return str_to_date_time(date_str).date()
 
 
 def test_date_range_generator():
     """Test date_range_generator generates DateTimeRanges."""
-    start_date_time = datetime.strptime("2022-01-18", '%Y-%m-%d')
+    start_date_time = datetime.strptime("2022-01-18", "%Y-%m-%d")
     time_delta = timedelta(days=1)
     end_date_time = start_date_time + timedelta(days=3)
     daterange_generator = date_range_generator(
         start_date_time=start_date_time,
         end_date_time=end_date_time,
-        time_delta=time_delta
+        time_delta=time_delta,
     )
     result = [daterange for daterange in daterange_generator]
     assert result == [
-        DateTimeRange(
-            str_to_date_time('2022-01-18'), str_to_date_time('2022-01-19')),
-        DateTimeRange(
-            str_to_date_time('2022-01-19'), str_to_date_time('2022-01-20')),
-        DateTimeRange(
-            str_to_date_time('2022-01-20'), str_to_date_time('2022-01-21'))]
+        DateTimeRange(str_to_date_time("2022-01-18"), str_to_date_time("2022-01-19")),
+        DateTimeRange(str_to_date_time("2022-01-19"), str_to_date_time("2022-01-20")),
+        DateTimeRange(str_to_date_time("2022-01-20"), str_to_date_time("2022-01-21")),
+    ]
 
 
 def test_date_range_generator_with_during_day_time_stamps():
     """
     Test date_range_generator generates correct DateTimeRanges when atributes
     contain a time other the 00:00:00. The first daterange should start with
     the date part of the from_data."""
-    start_date_time = datetime.strptime(
-        "2022-01-18 13:55:26", '%Y-%m-%d %H:%M:%S')
+    start_date_time = datetime.strptime("2022-01-18 13:55:26", "%Y-%m-%d %H:%M:%S")
     time_delta = timedelta(days=1)
     end_date_time = start_date_time + timedelta(days=3)
     daterange_generator = date_range_generator(
         start_date_time=start_date_time,
         end_date_time=end_date_time,
-        time_delta=time_delta
+        time_delta=time_delta,
     )
     result = [daterange for daterange in daterange_generator]
     assert result == [
-        DateTimeRange(
-            str_to_date_time('2022-01-18'), str_to_date_time('2022-01-19')),
-        DateTimeRange(
-            str_to_date_time('2022-01-19'), str_to_date_time('2022-01-20')),
-        DateTimeRange(
-            str_to_date_time('2022-01-20'), str_to_date_time('2022-01-21'))]
+        DateTimeRange(str_to_date_time("2022-01-18"), str_to_date_time("2022-01-19")),
+        DateTimeRange(str_to_date_time("2022-01-19"), str_to_date_time("2022-01-20")),
+        DateTimeRange(str_to_date_time("2022-01-20"), str_to_date_time("2022-01-21")),
+    ]
 
 
 def test_get_daily_date_ranges():
     """Test daterange_generator returns DateTimeRange ranges."""
     start_date = date(year=2022, month=1, day=18)
     end_date = date(year=2022, month=1, day=21)
     daterange_generator = get_daily_date_ranges(
-        start_date=start_date,
-        end_date=end_date
+        start_date=start_date, end_date=end_date
     )
     result = [daterange for daterange in daterange_generator]
     assert result == [
-        DateTimeRange(
-            str_to_date_time('2022-01-18'), str_to_date_time('2022-01-19')),
-        DateTimeRange(
-            str_to_date_time('2022-01-19'), str_to_date_time('2022-01-20')),
-        DateTimeRange(
-            str_to_date_time('2022-01-20'), str_to_date_time('2022-01-21'))]
+        DateTimeRange(str_to_date_time("2022-01-18"), str_to_date_time("2022-01-19")),
+        DateTimeRange(str_to_date_time("2022-01-19"), str_to_date_time("2022-01-20")),
+        DateTimeRange(str_to_date_time("2022-01-20"), str_to_date_time("2022-01-21")),
+    ]
 
 
 def test_get_daily_date_range_till_yesterday():
     """
     Test get_daily_date_range_till_yesterday generates a DateTimeRange
     till yesterday.
     """
     start_date = date.today() - timedelta(days=3)
-    daterange_generator = get_daily_date_range_till_yesterday(
-        start_date=start_date)
+    daterange_generator = get_daily_date_range_till_yesterday(start_date=start_date)
     result = [daterange for daterange in daterange_generator]
     assert len(result) == 3
 
 
 def test_get_daily_date_ranges_yesterday():
     """
     Test get_daily_date_ranges_yesterday generates a DateTimeRange
     for only yesterday.
     """
-    today = datetime.strftime(datetime.now(), '%Y-%m-%d')
-    yesterday = datetime.strftime(
-        datetime.now() - timedelta(days=1), '%Y-%m-%d')
+    today = datetime.strftime(datetime.now(), "%Y-%m-%d")
+    yesterday = datetime.strftime(datetime.now() - timedelta(days=1), "%Y-%m-%d")
 
     daterange_generator = get_daily_date_range_yesterday()
     result = [daterange for daterange in daterange_generator]
     assert result[0].from_date == str_to_date_time(yesterday)
     assert result[0].to_date == str_to_date_time(today)
     assert len(result) == 1
 
 
 def test_get_daily_date_range_for_single_date():
     """
     Test get_daily_date_range_for_single_date returns a single DateTimeRange.
     """
     today = date.today()
     yesterday = date.today() - timedelta(days=1)
-    single_daily_date_range = get_daily_date_range_for_single_date(
-        date=yesterday
-    )
+    single_daily_date_range = get_daily_date_range_for_single_date(date=yesterday)
 
     assert isinstance(single_daily_date_range, DateTimeRange)
     assert single_daily_date_range.from_date.date() == yesterday
     assert single_daily_date_range.to_date.date() == today
 
 
 def test_get_monthly_date_range_for_single_date():
     """
     Test get_monthly_date_range_for_single_date returns a single DateTimeRange.
     """
-    first_day_of_month = datetime.strptime('2022-02-01', '%Y-%m-%d')
-    first_day_of_next_month = datetime.strptime('2022-03-01', '%Y-%m-%d')
-    input_date = datetime.strptime('2022-02-11', '%Y-%m-%d')
-    single_monthly_date_range = get_monthly_date_range_for_single_date(
-        date=input_date
-    )
+    first_day_of_month = datetime.strptime("2022-02-01", "%Y-%m-%d")
+    first_day_of_next_month = datetime.strptime("2022-03-01", "%Y-%m-%d")
+    input_date = datetime.strptime("2022-02-11", "%Y-%m-%d")
+    single_monthly_date_range = get_monthly_date_range_for_single_date(date=input_date)
     assert isinstance(single_monthly_date_range, DateTimeRange)
     assert single_monthly_date_range.from_date == first_day_of_month
     assert single_monthly_date_range.to_date == first_day_of_next_month
 
 
 def test_get_weekly_date_range_for_single_date():
     """
     Test get_monthly_date_range_for_single_date returns a single DateTimeRange.
     """
-    first_day_of_week = datetime.strptime('2022-10-03', '%Y-%m-%d')
-    first_day_of_next_week = datetime.strptime('2022-10-10', '%Y-%m-%d')
-    input_date = datetime.strptime('2022-10-07', '%Y-%m-%d')
+    first_day_of_week = datetime.strptime("2022-10-03", "%Y-%m-%d")
+    first_day_of_next_week = datetime.strptime("2022-10-10", "%Y-%m-%d")
+    input_date = datetime.strptime("2022-10-07", "%Y-%m-%d")
     single_weekly_date_range = get_weekly_date_range_for_single_date(
         date=input_date.date()
     )
     assert isinstance(single_weekly_date_range, DateTimeRange)
     assert single_weekly_date_range.from_date == first_day_of_week
     assert single_weekly_date_range.to_date == first_day_of_next_week
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_settings/test_exceptions.py` & `pipeline_telemetry-1.0.0/tests/test_settings/test_exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,182 +1,170 @@
 """
 module to test custom exceptions in pipeline telemetry module
 """
+
 import pytest
 from test_data import TEST_PROCESS_TYPE
 
 from pipeline_telemetry.settings import exceptions
 
 
 def raise_exception(exception, value):
-    """ test helper method to raise exception """
+    """test helper method to raise exception"""
     if value:
         raise exception(value)
     raise exception
 
 
 def test_field_name_mandatory_exception():
-    """ test FieldNameMandatory exception """
+    """test FieldNameMandatory exception"""
     with pytest.raises(exceptions.FieldNameMandatory) as exception:
-        raise_exception(exceptions.FieldNameMandatory, 'test_field_name')
+        raise_exception(exceptions.FieldNameMandatory, "test_field_name")
 
-    assert 'For `test_field_name` instruction' in str(exception)
+    assert "For `test_field_name` instruction" in str(exception)
 
 
 def test_unknown_instruction_exception():
-    """ test UnknownInstruction exception """
+    """test UnknownInstruction exception"""
     with pytest.raises(exceptions.UnknownInstruction) as exception:
-        raise_exception(exceptions.UnknownInstruction, 'test_instruction')
+        raise_exception(exceptions.UnknownInstruction, "test_instruction")
 
-    assert 'test_instruction not registered' in str(exception)
+    assert "test_instruction not registered" in str(exception)
 
 
 def test_instruction_registered_twice_exception():
-    """ test InstructionRegisteredTwice exception """
-    class TestInstructrion():
-        """ test class """
-        INSTRUCTION = 'test_instruction'
+    """test InstructionRegisteredTwice exception"""
+
+    class TestInstructrion:
+        """test class"""
+
+        INSTRUCTION = "test_instruction"
 
     with pytest.raises(exceptions.InstructionRegisteredTwice) as exception:
-        raise_exception(
-            exceptions.InstructionRegisteredTwice, TestInstructrion)
+        raise_exception(exceptions.InstructionRegisteredTwice, TestInstructrion)
 
-    assert 'test_instruction from class TestInstructrion.' in str(exception)
+    assert "test_instruction from class TestInstructrion." in str(exception)
 
 
 def test_rule_can_only_have_one_instruction_exception():
-    """ test RuleCanHaveOnlyOneInstruction exception """
+    """test RuleCanHaveOnlyOneInstruction exception"""
     with pytest.raises(exceptions.RuleCanHaveOnlyOneInstruction) as exception:
         raise_exception(
-            exceptions.RuleCanHaveOnlyOneInstruction, {'key1': 1, 'key2': 2})
+            exceptions.RuleCanHaveOnlyOneInstruction, {"key1": 1, "key2": 2}
+        )
 
-    assert 'Rule contains multiple keys' in str(exception)
-    assert 'key1, key2' in str(exception)
+    assert "Rule contains multiple keys" in str(exception)
+    assert "key1, key2" in str(exception)
 
 
 def test_base_count_for_sub_process_not_added_exception():
-    """ test BaseCountForSubProcessNotAdded exception """
+    """test BaseCountForSubProcessNotAdded exception"""
     with pytest.raises(exceptions.BaseCountForSubProcessNotAdded) as exception:
-        raise_exception(
-            exceptions.BaseCountForSubProcessNotAdded, 'sub_process')
+        raise_exception(exceptions.BaseCountForSubProcessNotAdded, "sub_process")
 
-    assert 'Sub process sub_process has not yet been initialized' in \
-        str(exception)
+    assert "Sub process sub_process has not yet been initialized" in str(exception)
 
 
 def test_telemetry_object_already_closed_exception():
-    """ test TelemetryObjectAlreadyClosed exception """
+    """test TelemetryObjectAlreadyClosed exception"""
     with pytest.raises(exceptions.TelemetryObjectAlreadyClosed) as exception:
         raise_exception(exceptions.TelemetryObjectAlreadyClosed, None)
 
-    assert 'Telemetry object is already closed' in str(exception)
+    assert "Telemetry object is already closed" in str(exception)
 
 
 def test_storage_class_of_incorrect_type_exception():
-    """ test StorageClassOfIncorrectType exception """
+    """test StorageClassOfIncorrectType exception"""
     with pytest.raises(exceptions.StorageClassOfIncorrectType) as exception:
-        raise_exception(
-            exceptions.StorageClassOfIncorrectType, 'Incorrect_class')
+        raise_exception(exceptions.StorageClassOfIncorrectType, "Incorrect_class")
 
-    assert 'StorageClass `Incorrect_class` not a child class' in str(exception)
+    assert "StorageClass `Incorrect_class` not a child class" in str(exception)
 
 
 def test_expected_count_must_be_positive_int_exception():
-    """ test ExpectedCountMustBePositiveInt exception """
+    """test ExpectedCountMustBePositiveInt exception"""
     with pytest.raises(exceptions.ExpectedCountMustBePositiveInt) as exception:
         raise exceptions.ExpectedCountMustBePositiveInt
 
-    assert \
-        'Ruleset field `expected_count` can not be negative' in str(exception)
+    assert "Ruleset field `expected_count` can not be negative" in str(exception)
 
 
 def test_invalid_sub_process():
-    """ test InvalidSubProcess exception """
+    """test InvalidSubProcess exception"""
     with pytest.raises(exceptions.InvalidSubProcess) as exception:
-        raise exceptions.InvalidSubProcess('test_process', TEST_PROCESS_TYPE)
+        raise exceptions.InvalidSubProcess("test_process", TEST_PROCESS_TYPE)
 
-    assert 'Sub Process `test_process` does not exist' in str(exception)
+    assert "Sub Process `test_process` does not exist" in str(exception)
 
 
 def test_process_type_not_registered():
-    """ test ProcessTypeNotRegistered exception """
+    """test ProcessTypeNotRegistered exception"""
     with pytest.raises(exceptions.ProcessTypeNotRegistered) as exception:
         raise exceptions.ProcessTypeNotRegistered(TEST_PROCESS_TYPE)
 
-    assert 'provided process_type test_process_type not registered' in \
-        str(exception)
+    assert "provided process_type test_process_type not registered" in str(exception)
 
 
 def test_process_types_not_of_right_class():
-    """ test ProcessTypesMustBeOfClassBaseEnumertor exception """
-    with pytest.raises(
-            exceptions.ProcessTypesMustBeOfClassBaseEnumertor) as exception:
+    """test ProcessTypesMustBeOfClassBaseEnumertor exception"""
+    with pytest.raises(exceptions.ProcessTypesMustBeOfClassBaseEnumertor) as exception:
         raise exceptions.ProcessTypesMustBeOfClassBaseEnumertor
 
-    assert 'provided process_types enumerator not of class BaseEnumrator' in \
-        str(exception)
+    assert "provided process_types enumerator not of class BaseEnumrator" in str(
+        exception
+    )
 
 
 def test_sub_process_not_defined_in_process_type():
-    """ test InvalidSubProcessForProcessType exception """
-    with pytest.raises(
-            exceptions.InvalidSubProcessForProcessType) as exception:
+    """test InvalidSubProcessForProcessType exception"""
+    with pytest.raises(exceptions.InvalidSubProcessForProcessType) as exception:
         raise exceptions.InvalidSubProcessForProcessType
 
-    assert 'Provided sub process is not defined in ProcessType.' in \
-        str(exception)
+    assert "Provided sub process is not defined in ProcessType." in str(exception)
 
 
 def test_invalid_telemetry_type():
-    """ test InvalidTelemetryType exception """
-    with pytest.raises(
-            exceptions.InvalidTelemetryType) as exception:
-        raise exceptions.InvalidTelemetryType(['type1', 'type2'])
+    """test InvalidTelemetryType exception"""
+    with pytest.raises(exceptions.InvalidTelemetryType) as exception:
+        raise exceptions.InvalidTelemetryType(["type1", "type2"])
 
-    assert 'Telemetry Type must be of type: type1' in \
-        str(exception)
+    assert "Telemetry Type must be of type: type1" in str(exception)
 
 
 def test_class_telemetry_params_not_defined():
-    """ test ClassTelemetryParamsNotDefined exception """
-    obj = 'object'
-    with pytest.raises(
-            exceptions.ClassTelemetryParamsNotDefined) as exception:
+    """test ClassTelemetryParamsNotDefined exception"""
+    obj = "object"
+    with pytest.raises(exceptions.ClassTelemetryParamsNotDefined) as exception:
         raise exceptions.ClassTelemetryParamsNotDefined(obj)
 
-    assert \
-        f"Telemetry params not defined for class {obj.__class__.__name__}" in \
-        str(exception)
+    assert f"Telemetry params not defined for class {obj.__class__.__name__}" in str(
+        exception
+    )
 
 
 def test_unknown_telemety_type():
-    """ test UnknownTelemetryType exception """
-    telem_type = 'SINGLE'
-    with pytest.raises(
-            exceptions.UnknownTelemetryType) as exception:
+    """test UnknownTelemetryType exception"""
+    telem_type = "SINGLE"
+    with pytest.raises(exceptions.UnknownTelemetryType) as exception:
         raise exceptions.UnknownTelemetryType(telem_type)
 
-    assert \
-        f"Unknown telemetry_type `{telem_type}` used in aggregator" in \
-        str(exception)
+    assert f"Unknown telemetry_type `{telem_type}` used in aggregator" in str(exception)
 
 
 def test_must_have_key_mandatory():
-    """ test MustHaveKeyMandatory exception """
-    instruction = 'instruction'
-    with pytest.raises(
-            exceptions.MustHaveKeyMandatory) as exception:
+    """test MustHaveKeyMandatory exception"""
+    instruction = "instruction"
+    with pytest.raises(exceptions.MustHaveKeyMandatory) as exception:
         raise exceptions.MustHaveKeyMandatory(instruction)
 
     assert f"For `{instruction}` instruction" in str(exception)
 
 
 def test_requested_date_time_range_method_not_found():
-    """ test RequestedDataTimeRangeMethodNotFound exception """
-    telemetry_aggr_type = 'telemetry_aggr_type'
-    with pytest.raises(
-            exceptions.RequestedDataTimeRangeMethodNotFound) as exception:
-        raise exceptions.RequestedDataTimeRangeMethodNotFound(
-            telemetry_aggr_type)
-
-    assert f"No date_time_range method found for {telemetry_aggr_type}." \
-        in str(exception)
+    """test RequestedDataTimeRangeMethodNotFound exception"""
+    telemetry_aggr_type = "telemetry_aggr_type"
+    with pytest.raises(exceptions.RequestedDataTimeRangeMethodNotFound) as exception:
+        raise exceptions.RequestedDataTimeRangeMethodNotFound(telemetry_aggr_type)
+
+    assert f"No date_time_range method found for {telemetry_aggr_type}." in str(
+        exception
+    )
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_storage/test_mongo_storage.py` & `pipeline_telemetry-1.0.0/tests/test_storage/test_mongo_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-"""Module to test storage module.
-"""
+"""Module to test storage module."""
+
 from datetime import datetime, timedelta
 
 from test_data import DEFAULT_TELEMETRY_MODEL_PARAMS
 
 from pipeline_telemetry.data_classes import TelemetryModel
-from pipeline_telemetry.settings.settings import DEFAULT_TRAFIC_LIGHT_COLOR, \
-    RUN_TIME
-from pipeline_telemetry.storage.mongo import TelemetryMongoModel, \
-    TelemetryMongoStorage
+from pipeline_telemetry.settings.settings import DEFAULT_TRAFIC_LIGHT_COLOR, RUN_TIME
+from pipeline_telemetry.storage.mongo import TelemetryMongoModel, TelemetryMongoStorage
 from pipeline_telemetry.storage.mongo_connection import get_mongo_db_port
 
 
 def telemetry_query_params():
     """Returns a default set of query params"""
     return DEFAULT_TELEMETRY_MODEL_PARAMS | {
-        'from_date_time': datetime.now() - timedelta(days=1),
-        'to_date_time': datetime.now() + timedelta(days=1)
+        "from_date_time": datetime.now() - timedelta(days=1),
+        "to_date_time": datetime.now() + timedelta(days=1),
     }
 
 
 def test_telemetry_mongo_model_class_exists():
     """Test TelemetryMongoModel class exists."""
     assert TelemetryMongoModel
 
@@ -63,15 +61,16 @@
                 "source_name": "tst_source_name",
                 "process_type": "tst_process_type",
                 "start_date_time": "tst_start_date_time",
                 "run_time_in_seconds": 1.123,
                 "io_time_in_seconds": 1.1,
                 "traffic_light": DEFAULT_TRAFIC_LIGHT_COLOR,
             }
-        ))
+        )
+    )
 
     assert result == {
         "telemetry_type": "test telemetry type",
         "category": "test",
         "sub_category": "sub_test",
         "source_name": "tst_source_name",
         "process_type": "tst_process_type",
@@ -104,13 +103,13 @@
 
 
 def test_mongo_model_to_dict():
     """
     Test to_dict method returns a dict with run_time_in_seconds atrribute converted to float.
     """
     telemetry = TelemetryMongoModel()
-    telemetry._id = 'test _id'
-    telemetry.run_time_in_seconds = '1'
+    telemetry._id = "test _id"
+    telemetry.run_time_in_seconds = "1"
     telemetry_to_dict = telemetry.to_dict()
     assert isinstance(telemetry_to_dict, dict)
     assert isinstance(getattr(telemetry, RUN_TIME), str)
     assert isinstance(telemetry_to_dict[RUN_TIME], float)
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_storage/test_sqllite_storage.py` & `pipeline_telemetry-1.0.0/tests/test_storage/test_sqllite_storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-"""Module to test storage module.
-"""
+"""Module to test storage module."""
+
 import sqlite3
 from datetime import datetime, timedelta
 
 import pytest
 from freezegun import freeze_time
-from test_storage_data import DEFAULT_TELEMETRY_MODEL_PARAMS, \
-    DEFAULT_TELEMETRY_PARAMS
+from test_storage_data import DEFAULT_TELEMETRY_MODEL_PARAMS, DEFAULT_TELEMETRY_PARAMS
 
 from pipeline_telemetry import Telemetry
 from pipeline_telemetry.data_classes import TelemetryModel
 from pipeline_telemetry.settings import DateTimeRange, exceptions
 from pipeline_telemetry.settings import settings as st
 from pipeline_telemetry.storage.generic import AbstractTelemetryStorage
 from pipeline_telemetry.storage.memory import TelemetryInMemoryStorage
 
 
 def telemetry_query_params():
     """Returns a default set of query params"""
     return DEFAULT_TELEMETRY_MODEL_PARAMS | {
-        'from_date_time': datetime.now() - timedelta(days=1),
-        'to_date_time': datetime.now() + timedelta(days=1)
+        "from_date_time": datetime.now() - timedelta(days=1),
+        "to_date_time": datetime.now() + timedelta(days=1),
     }
 
 
 def test_in_abstract_strorage_class_exists():
     """Test that abstract storage class exists."""
     assert AbstractTelemetryStorage
 
@@ -36,38 +35,41 @@
 
 def test_db_object_to_dict_method():
     """
     Test _db_object_to_dict method exists and if no override is done returns an
     object unchanged.
     """
     in_memory_storage = TelemetryInMemoryStorage()
-    assert in_memory_storage._db_object_to_dict(
-        {'test': 'dict'}) == {'test': 'dict'}
+    assert in_memory_storage._db_object_to_dict({"test": "dict"}) == {"test": "dict"}
 
 
 def test_get_aggr_telem_query_params():
     """
     Test _get_aggr_telem_query_params converts TelemetryModel into
     dict with the correct keys.
     """
     telemetry_params = DEFAULT_TELEMETRY_MODEL_PARAMS.copy() | {
-        'telemetry_type': 'DAILY AGGREGATION'
+        "telemetry_type": "DAILY AGGREGATION"
     }
 
     telemetry = TelemetryModel(**telemetry_params)
     in_memory_storage = TelemetryInMemoryStorage()
-    aggr_telem_query_params = in_memory_storage._get_aggr_telem_query_params(
-        telemetry)
+    aggr_telem_query_params = in_memory_storage._get_aggr_telem_query_params(telemetry)
     assert isinstance(aggr_telem_query_params, dict)
-    keys = ['telemetry_type', 'source_name', 'category', 'sub_category',
-            'process_type', 'from_date_time', 'to_date_time']
+    keys = [
+        "telemetry_type",
+        "source_name",
+        "category",
+        "sub_category",
+        "process_type",
+        "from_date_time",
+        "to_date_time",
+    ]
     assert all([key in aggr_telem_query_params.keys() for key in keys])
-    assert not [
-        key for key in aggr_telem_query_params.keys()
-        if key not in keys]
+    assert not [key for key in aggr_telem_query_params.keys() if key not in keys]
 
 
 def test_in_memory_storage_creates_db_in_memory():
     """Test in memory storage instance has db_in_memory and db_cursor"""
     in_memory_storage = TelemetryInMemoryStorage()
     assert in_memory_storage.db_in_memory
     assert in_memory_storage.db_cursor
@@ -77,24 +79,24 @@
 
 def test_store_telemetry_raise_exception_when_db_is_closed():
     """Test in memory storage instance has db_in_memory and db_cursor"""
     in_memory_storage = TelemetryInMemoryStorage()
     in_memory_storage.close_db()
     with pytest.raises(exceptions.StorageNotInitialized):
         in_memory_storage.store_telemetry(
-            TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
+            TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
+        )
 
 
 def test_select_records_raise_exception_when_db_is_closed():
     """Test in memory storage instance has db_in_memory and db_cursor"""
     in_memory_storage = TelemetryInMemoryStorage()
     in_memory_storage.close_db()
     with pytest.raises(exceptions.StorageNotInitialized):
-        in_memory_storage.select_records(
-            **telemetry_query_params())
+        in_memory_storage.select_records(**telemetry_query_params())
 
 
 def test_close_db_in_memory():
     """Test in memory storage close method close the db."""
     in_memory_storage = TelemetryInMemoryStorage()
     db_in_memory = in_memory_storage.db_in_memory
     cursor = in_memory_storage.db_cursor
@@ -128,221 +130,223 @@
 
 
 def test_store_telemetry_stores_object():
     """Test in memory storage instance has db_in_memory and db_cursor"""
     # Table reset for each test is needed as the table is a class property
     TelemetryInMemoryStorage._define_db_table(TelemetryInMemoryStorage.db_cursor)
     in_memory_storage = TelemetryInMemoryStorage()
-    in_memory_storage.store_telemetry(
-        TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
+    in_memory_storage.store_telemetry(TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
     all_in_memory_objects = in_memory_storage.db_cursor.execute(
         "SELECT * FROM telemetry "
     )
     assert len(all_in_memory_objects.fetchall()) == 1
 
 
 def test_select_records_returns_sql_lite_cursor():
     """Test select_records method returns sqllite Cursor with one object."""
     # Table reset for each test is needed as the table is a class property
     TelemetryInMemoryStorage._define_db_table(TelemetryInMemoryStorage.db_cursor)
     in_memory_storage = TelemetryInMemoryStorage()
-    in_memory_storage.store_telemetry(
-        TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
-    selected_in_memory_objects = \
-        in_memory_storage.select_records(**telemetry_query_params())
+    in_memory_storage.store_telemetry(TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
+    selected_in_memory_objects = in_memory_storage.select_records(
+        **telemetry_query_params()
+    )
     assert len(selected_in_memory_objects.fetchall()) == 1
     assert isinstance(selected_in_memory_objects, sqlite3.Cursor)
 
 
 def test_records_with_outside_date_range_are_not_returned():
     """
     Test select_records method returns only those records within the given date
     range.
     """
     # Table reset for each test is needed as the table is a class property
     TelemetryInMemoryStorage._define_db_table(TelemetryInMemoryStorage.db_cursor)
     in_memory_storage = TelemetryInMemoryStorage()
+    in_memory_storage.store_telemetry(TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
     in_memory_storage.store_telemetry(
-        TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
-    in_memory_storage.store_telemetry(
-        TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS | {
-            'start_date_time': datetime.now() - timedelta(days=2)}))
-    selected_in_memory_objects = \
-        in_memory_storage.select_records(**telemetry_query_params())
+        TelemetryModel(
+            **DEFAULT_TELEMETRY_MODEL_PARAMS
+            | {"start_date_time": datetime.now() - timedelta(days=2)}
+        )
+    )
+    selected_in_memory_objects = in_memory_storage.select_records(
+        **telemetry_query_params()
+    )
     assert len(selected_in_memory_objects.fetchall()) == 1
     all_in_memory_objects = in_memory_storage.db_cursor.execute(
         "SELECT * FROM telemetry "
     )
     assert len(all_in_memory_objects.fetchall()) == 2
 
 
 def test_select_records_returns_only_selected_records():
     """
     Test select_records method returns only records accordding to giv.encode()attriubures.
     """
     # Table reset for each test is needed as the table is a class property
     TelemetryInMemoryStorage._define_db_table(TelemetryInMemoryStorage.db_cursor)
     in_memory_storage = TelemetryInMemoryStorage()
+    in_memory_storage.store_telemetry(TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
+    in_memory_storage.store_telemetry(TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
     in_memory_storage.store_telemetry(
-        TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
-    in_memory_storage.store_telemetry(
-        TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
-    in_memory_storage.store_telemetry(
-        TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS |
-                       {'category': 'different_category'}))
+        TelemetryModel(
+            **DEFAULT_TELEMETRY_MODEL_PARAMS | {"category": "different_category"}
+        )
+    )
     selected_in_memory_objects = in_memory_storage.select_records(
-        **telemetry_query_params())
+        **telemetry_query_params()
+    )
     assert len(selected_in_memory_objects.fetchall()) == 2
     all_in_memory_objects = in_memory_storage.db_cursor.execute(
-        "SELECT * FROM telemetry ")
+        "SELECT * FROM telemetry "
+    )
     assert len(all_in_memory_objects.fetchall()) == 3
 
 
 @freeze_time("2022-01-18 18:00:00.123456")
 def test_store_telemetry_stores_object_with_create_date(mocker):
     """Test in memory storage instance has db_in_memory and db_cursor"""
     frozen_time = {"start_date_time": datetime.now()}
     telemetry = DEFAULT_TELEMETRY_MODEL_PARAMS | frozen_time
     # Table reset for each test is needed as the table is a class property
     TelemetryInMemoryStorage._define_db_table(TelemetryInMemoryStorage.db_cursor)
     in_memory_storage = TelemetryInMemoryStorage()
-    in_memory_storage.store_telemetry(
-        TelemetryModel(**telemetry))
+    in_memory_storage.store_telemetry(TelemetryModel(**telemetry))
     in_memory_record = in_memory_storage.db_cursor.execute(
         "SELECT * FROM telemetry LIMIT 1"
     ).fetchone()
-    assert in_memory_record['start_date_time'] == "2022-01-18 18:00:00.123456"
+    assert in_memory_record["start_date_time"] == "2022-01-18T18:00:00.123456"
 
 
 def test_telemetry_storage_to_object_returns_telemetry_model():
     """
     Test _telemetry_storage_to_object method returns a TelemetryModel instance
     created from an in memory storage object.
     """
     # Table reset for each test is needed as the table is a class property
     TelemetryInMemoryStorage._define_db_table(TelemetryInMemoryStorage.db_cursor)
     in_memory_storage = TelemetryInMemoryStorage()
-    in_memory_storage.store_telemetry(
-        TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
+    in_memory_storage.store_telemetry(TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
     in_memory_record = in_memory_storage.db_cursor.execute(
-        "SELECT * FROM telemetry LIMIT 1").fetchone()
-    telemetry = in_memory_storage._telemetry_storage_to_object(
-        in_memory_record)
+        "SELECT * FROM telemetry LIMIT 1"
+    ).fetchone()
+    telemetry = in_memory_storage._telemetry_storage_to_object(in_memory_record)
     assert isinstance(telemetry, TelemetryModel)
 
 
 def test_telemetry_storage_to_object_returns_object_with_correct_values():
     """
     Test _telemetry_storage_to_object method returns a TelemetryModel instance
     with the correct values.
     """
     # Table reset for each test is needed as the table is a class property
     TelemetryInMemoryStorage._define_db_table(TelemetryInMemoryStorage.db_cursor)
     in_memory_storage = TelemetryInMemoryStorage()
-    in_memory_storage.store_telemetry(
-        TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
+    in_memory_storage.store_telemetry(TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
     in_memory_record = in_memory_storage.db_cursor.execute(
-        "SELECT * FROM telemetry LIMIT 1").fetchone()
-    telemetry = in_memory_storage._telemetry_storage_to_object(
-        in_memory_record)
+        "SELECT * FROM telemetry LIMIT 1"
+    ).fetchone()
+    telemetry = in_memory_storage._telemetry_storage_to_object(in_memory_record)
     for key, value in DEFAULT_TELEMETRY_MODEL_PARAMS.items():
         assert getattr(telemetry, key) == value
 
 
 def test_telemetry_storage_to_object_returns_object_with_telemetry_data():
     """
     Test _telemetry_storage_to_object method returns a TelemetryModel instance
     with the correct values.
     """
-    counter_key = 'TEST_COUNTER'
+    counter_key = "TEST_COUNTER"
     telemetry = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
-    sub_process = telemetry.get_sub_process_data('sub_process')
+    sub_process = telemetry.get_sub_process_data("sub_process")
     sub_process.increase_base_count(increment=1)
     sub_process.increase_custom_count(increment=2, counter=counter_key)
     # Table reset for each test is needed as the table is a class property
     TelemetryInMemoryStorage._define_db_table(TelemetryInMemoryStorage.db_cursor)
     in_memory_storage = TelemetryInMemoryStorage()
     in_memory_storage.store_telemetry(telemetry)
     in_memory_record = in_memory_storage.db_cursor.execute(
-        "SELECT * FROM telemetry LIMIT 1").fetchone()
-    telemetry_model = in_memory_storage._telemetry_storage_to_object(
-        in_memory_record)
-    telemetry_data = telemetry_model.get_sub_process_data(
-        'sub_process')
+        "SELECT * FROM telemetry LIMIT 1"
+    ).fetchone()
+    telemetry_model = in_memory_storage._telemetry_storage_to_object(in_memory_record)
+    telemetry_data = telemetry_model.get_sub_process_data("sub_process")
     assert telemetry_data
     assert getattr(telemetry_data, st.BASE_COUNT_KEY) == 1
     assert getattr(telemetry_data, st.COUNTERS_KEY)[counter_key] == 2
 
 
 @freeze_time("2022-01-18 18:00:00.123456")
 def test_get_aggr_telem_date_time_range():
     """
     Test _get_aggr_telem_date_time_range returns the proper date time range.
     """
     telemetry_params = DEFAULT_TELEMETRY_PARAMS.copy() | {
-        "telemetry_type": 'DAILY AGGREGATION'
+        "telemetry_type": "DAILY AGGREGATION"
     }
     telemetry = Telemetry(**telemetry_params)
     telemetry._telemetry.start_date_time = datetime.now()
     telemetry.start_date_time
-    aggr_telem_date_time_range = TelemetryInMemoryStorage(
-    )._get_aggr_telem_date_time_range(telemetry)
+    aggr_telem_date_time_range = (
+        TelemetryInMemoryStorage()._get_aggr_telem_date_time_range(telemetry)
+    )
 
     assert isinstance(aggr_telem_date_time_range, DateTimeRange)
     assert aggr_telem_date_time_range.from_date == datetime(2022, 1, 18)
     assert aggr_telem_date_time_range.to_date == datetime(2022, 1, 19)
 
 
 @freeze_time("2022-01-18 18:00:00.123456")
 def test_get_aggr_telem_date_time_range_monthly_aggr():
     """
     Test _get_aggr_telem_date_time_range returns the proper date time range
     with monthly telemetry aggregation type
     """
     telemetry_params = DEFAULT_TELEMETRY_PARAMS.copy() | {
-        "telemetry_type": 'MONTHLY AGGREGATION'
+        "telemetry_type": "MONTHLY AGGREGATION"
     }
     telemetry = Telemetry(**telemetry_params)
     telemetry._telemetry.start_date_time = datetime.now()
     telemetry.start_date_time
-    aggr_telem_date_time_range = TelemetryInMemoryStorage(
-    )._get_aggr_telem_date_time_range(telemetry)
+    aggr_telem_date_time_range = (
+        TelemetryInMemoryStorage()._get_aggr_telem_date_time_range(telemetry)
+    )
 
     assert aggr_telem_date_time_range.from_date == datetime(2022, 1, 1)
     assert aggr_telem_date_time_range.to_date == datetime(2022, 2, 1)
 
 
 @freeze_time("2022-01-18 18:00:00.123456")
 def test_get_aggr_telem_date_time_range_weekly_aggr():
     """
     Test _get_aggr_telem_date_time_range returns the proper date time range
     with weekly telemetry aggregation type
     """
     telemetry_params = DEFAULT_TELEMETRY_PARAMS.copy() | {
-        "telemetry_type": 'WEEKLY AGGREGATION'
+        "telemetry_type": "WEEKLY AGGREGATION"
     }
     telemetry = Telemetry(**telemetry_params)
     telemetry._telemetry.start_date_time = datetime.now()
     telemetry.start_date_time
-    aggr_telem_date_time_range = TelemetryInMemoryStorage(
-    )._get_aggr_telem_date_time_range(telemetry)
+    aggr_telem_date_time_range = (
+        TelemetryInMemoryStorage()._get_aggr_telem_date_time_range(telemetry)
+    )
 
     assert aggr_telem_date_time_range.from_date == datetime(2022, 1, 17)
     assert aggr_telem_date_time_range.to_date == datetime(2022, 1, 24)
 
 
 def test_delete_telemetry_deletes_telemetry_record():
     """
     Test _telemetry_storage_to_object method returns a TelemetryModel instance
     with the correct values.
     """
     # Table reset for each test is needed as the table is a class property
     TelemetryInMemoryStorage._define_db_table(TelemetryInMemoryStorage.db_cursor)
     in_memory_storage = TelemetryInMemoryStorage()
-    in_memory_storage.store_telemetry(
-        TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
+    in_memory_storage.store_telemetry(TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS))
     in_memory_record = in_memory_storage.db_cursor.execute(
-        "SELECT * FROM telemetry LIMIT 1").fetchone()
-    telemetry = in_memory_storage._telemetry_storage_to_object(
-        in_memory_record)
+        "SELECT * FROM telemetry LIMIT 1"
+    ).fetchone()
+    telemetry = in_memory_storage._telemetry_storage_to_object(in_memory_record)
     for key, value in DEFAULT_TELEMETRY_MODEL_PARAMS.items():
         assert getattr(telemetry, key) == value
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_telemetry_class_methods.py` & `pipeline_telemetry-1.0.0/tests/test_telemetry_class_methods.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 """
 module to test the class methods fro Telemetry class of telemetry module
 
 """
+
 import pytest
 
 from pipeline_telemetry.main import Telemetry
 from pipeline_telemetry.settings import exceptions
 from pipeline_telemetry.settings.data_class import ProcessType
 
 
 def test_telemetry_class_method_add_process_type():
     """
     check that Telemetry class method add_process_type adds a process type
     """
     process_type = ProcessType(
-        process_type='custom_process_type',
-        subtypes=['custom_sub_process_type'])
-    Telemetry.add_process_type('TEST_TYPE', process_type)
-    assert Telemetry('test', 'test', 'test', process_type)
+        process_type="custom_process_type", subtypes=["custom_sub_process_type"]
+    )
+    Telemetry.add_process_type("TEST_TYPE", process_type)
+    assert Telemetry("test", "test", "test", process_type)
 
 
 def test_sub_process_types_also_added():
     """
     check that Telemetry class method add_process_type adds a process type
     including all sub_processes.
     """
     process_type = ProcessType(
-        process_type='custom_process_type',
-        subtypes=['custom_sub_process_type'])
-    Telemetry.add_process_type('TEST_TYPE', process_type)
-    telemetry = Telemetry('category', 'sub_category', 'name', process_type)
-    assert telemetry._process_type.sub_processes == ['custom_sub_process_type']
+        process_type="custom_process_type", subtypes=["custom_sub_process_type"]
+    )
+    Telemetry.add_process_type("TEST_TYPE", process_type)
+    telemetry = Telemetry("category", "sub_category", "name", process_type)
+    assert telemetry._process_type.sub_processes == ["custom_sub_process_type"]
 
 
 def test_add_process_type_raises_exception():
     """
     test class method add_process_type raises an excpetion when an object
     other the a ProcessType is offered
     """
     with pytest.raises(exceptions.ProcessTypeMustBeOfClassProcessType):
-        Telemetry.add_process_type('TYPE_NAME', 'not a ProcessType')
+        Telemetry.add_process_type("TYPE_NAME", "not a ProcessType")
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_telemetry_counter.py` & `pipeline_telemetry-1.0.0/tests/test_telemetry_counter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module to test telemetry counter login for pipeline telemetry module.
 """
+
 import pytest
 import test_data as TD
 
 from pipeline_telemetry import ProcessTypes
 from pipeline_telemetry.helper import is_telemetry_counter
 from pipeline_telemetry.main import Telemetry
 from pipeline_telemetry.settings import exceptions
@@ -28,15 +29,15 @@
     """
     Test that add_method on a telemetry counter adds the telemetry counter
     to given object with a _telemetry attribute
     """
     sub_process = TD.TEST_TELEMETRY_COUNTER_INC_2.sub_process
     telemetry = Telemetry(**TD.DEFAULT_TELEMETRY_PARAMS)
 
-    class ClassToTestAddTo():
+    class ClassToTestAddTo:
         _telemetry = telemetry
 
     obj_with_telemetry = ClassToTestAddTo()
 
     # ensure sub process is initialized in object's telemetry
     telemetry._initialize_sub_process(sub_process)
 
@@ -91,16 +92,15 @@
 
 
 def test_add_telemetry_counter_with_increment_arg(telemetry_inst):
     """
     Check invoking add_telemetry_counter method using increment argument adds
     the value of increment to the counter
     """
-    telemetry_inst.add_telemetry_counter(
-        TD.TEST_TELEMETRY_COUNTER, increment=10)
+    telemetry_inst.add_telemetry_counter(TD.TEST_TELEMETRY_COUNTER, increment=10)
     telemetry_data = telemetry_inst.get("RETRIEVE_RAW_DATA")
     assert getattr(telemetry_data, st.COUNTERS_KEY)["test_counter"] == 10
 
 
 def test_add_telemetry_counter_raises_exception(telemetry_inst):
     """
     Check invoking add_telemetry_counter method using increment argument adds
@@ -225,45 +225,55 @@
 def test_telementry_counter_hash():
     """Test that a TelemetryCounter object can be hashed."""
     assert TD.TEST_TELEMETRY_COUNTER.__hash__()
 
 
 def test_tc_hash_does_include_the_increment():
     """Test that increment value changes the hash."""
-    assert not TD.TEST_TELEMETRY_COUNTER.__hash__() == \
-        TD.TEST_TELEMETRY_COUNTER_INC_2.__hash__()
+    assert (
+        not TD.TEST_TELEMETRY_COUNTER.__hash__()
+        == TD.TEST_TELEMETRY_COUNTER_INC_2.__hash__()
+    )
 
 
 def test_tc_hash_works_with_errors():
     """
     Test that a telementry counters with different errors return a different
     hash.
     """
-    assert not TD.TEST_ERROR_TELEMETRY_COUNTER.__hash__() == \
-        TD.TEST_ERROR_TELEMETRY_COUNTER_2.__hash__()
+    assert (
+        not TD.TEST_ERROR_TELEMETRY_COUNTER.__hash__()
+        == TD.TEST_ERROR_TELEMETRY_COUNTER_2.__hash__()
+    )
 
 
 def test_tc_hash_works_with_counters():
     """
     Test that a telementry counters with different counters return a different
     hash.
     """
-    assert not TD.TEST_TELEMETRY_COUNTER.__hash__() == \
-        TD.TEST_TELEMETRY_COUNTER_2.__hash__()
+    assert (
+        not TD.TEST_TELEMETRY_COUNTER.__hash__()
+        == TD.TEST_TELEMETRY_COUNTER_2.__hash__()
+    )
 
 
 def test_tc_hash_does_include_process_types_field():
     """
     Test that a telementry counters with a different list of process types
     return a different hash.
     """
-    assert not TD.TEST_TC_MULT_PROCESS_TYPES.__hash__() == \
-        TD.TEST_TC_MULT_PROCESS_TYPES_2.__hash__()
+    assert (
+        not TD.TEST_TC_MULT_PROCESS_TYPES.__hash__()
+        == TD.TEST_TC_MULT_PROCESS_TYPES_2.__hash__()
+    )
 
 
 def test_tc_hash_does_include_sub_process_field():
     """
     Test that a telementry counters with a different sub_process
     return a different hash.
     """
-    assert not TD.TEST_TELEMETRY_COUNTER.__hash__() == \
-        TD.TEST_TELEMETRY_COUNTER_3.__hash__()
+    assert (
+        not TD.TEST_TELEMETRY_COUNTER.__hash__()
+        == TD.TEST_TELEMETRY_COUNTER_3.__hash__()
+    )
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_telemetry_models/test_telemetry_class.py` & `pipeline_telemetry-1.0.0/tests/test_telemetry_models/test_telemetry_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module to test telemetry main class for pipeline telemetry module.
 """
+
 from datetime import datetime
 
 import pytest
 from test_data import DEFAULT_TELEMETRY_PARAMS, TEST_PROCESS_TYPE_3
 
 from pipeline_telemetry import Telemetry
 from pipeline_telemetry.data_classes import TelemetryData, TelemetryModel
@@ -25,64 +26,65 @@
 def test_telemetry_instance_creation():
     """check that Telemetry instance can be created using default_params"""
     assert Telemetry(**DEFAULT_TELEMETRY_PARAMS)
 
 
 def test_telemetry_instance_has_telemetry_type_property():
     """check that Telemetry instance has a telemetry_type property"""
-    assert Telemetry(**DEFAULT_TELEMETRY_PARAMS).telemetry_type == \
-        st.DEFAULT_TELEMETRY_TYPE
+    assert (
+        Telemetry(**DEFAULT_TELEMETRY_PARAMS).telemetry_type
+        == st.DEFAULT_TELEMETRY_TYPE
+    )
 
 
 def test_telemetry_instance_has_source_name_property():
     """check that Telemetry instance has a source_name property"""
-    assert Telemetry(**DEFAULT_TELEMETRY_PARAMS).source_name == \
-        "load_weather_data"
+    assert Telemetry(**DEFAULT_TELEMETRY_PARAMS).source_name == "load_weather_data"
 
 
 def test_telemetry_instance_has_category_property():
     """check that Telemetry instance has a source_name property"""
-    assert Telemetry(**DEFAULT_TELEMETRY_PARAMS).category == \
-        "WEATHER"
+    assert Telemetry(**DEFAULT_TELEMETRY_PARAMS).category == "WEATHER"
 
 
 def test_telemetry_instance_has_sub_category_property():
     """check that Telemetry instance has a sub_category property"""
-    assert Telemetry(**DEFAULT_TELEMETRY_PARAMS).sub_category == \
-        "DAILY_PREDICTIONS"
+    assert Telemetry(**DEFAULT_TELEMETRY_PARAMS).sub_category == "DAILY_PREDICTIONS"
 
 
 def test_telemetry_instance_has_traffic_light_property():
     """
     Test that Telemetry instance has a traffic_light property that is
     set to the default value."""
-    assert Telemetry(**DEFAULT_TELEMETRY_PARAMS).traffic_light == \
-        st.DEFAULT_TRAFIC_LIGHT_COLOR
+    assert (
+        Telemetry(**DEFAULT_TELEMETRY_PARAMS).traffic_light
+        == st.DEFAULT_TRAFIC_LIGHT_COLOR
+    )
 
 
 def test_telemetry_instance_has_sub_process_types_property():
     """check that Telemetry instance has a sub_processes_types property"""
-    assert Telemetry(**DEFAULT_TELEMETRY_PARAMS).sub_process_types == \
-        DEFAULT_TELEMETRY_PARAMS['process_type'].sub_processes
+    assert (
+        Telemetry(**DEFAULT_TELEMETRY_PARAMS).sub_process_types
+        == DEFAULT_TELEMETRY_PARAMS["process_type"].sub_processes
+    )
 
 
 def test_telemetry_instance_has_telemetry_property():
     """
     Test that a Telemetry instance has a telemetry property that is an
     instance of class TelemetryModel"""
-    assert isinstance(Telemetry(**DEFAULT_TELEMETRY_PARAMS).telemetry,
-                      TelemetryModel)
+    assert isinstance(Telemetry(**DEFAULT_TELEMETRY_PARAMS).telemetry, TelemetryModel)
 
 
 def test_telemetry_instance_has_a_start_date_time_property():
     """
     Test that a Telemetry instance has a start_date_time property that is an
     instance of class TelemetryModel"""
-    assert isinstance(Telemetry(**DEFAULT_TELEMETRY_PARAMS).start_date_time,
-                      datetime)
+    assert isinstance(Telemetry(**DEFAULT_TELEMETRY_PARAMS).start_date_time, datetime)
 
 
 def test_telemetry_instance_has_io_time_in_seconds_property():
     """check that Telemetry instance has a io_time_in_seconds property"""
     assert hasattr(Telemetry(**DEFAULT_TELEMETRY_PARAMS), st.IO_TIME_KEY)
 
 
@@ -169,26 +171,24 @@
 
 def test_increase_sub_process_base_count():
     """
     Check that a sub process base count can be increased.
     """
     telemetry_inst = Telemetry(**DEFAULT_TELEMETRY_PARAMS)
     telemetry_inst.increase_sub_process_base_count("RETRIEVE_RAW_DATA")
-    assert getattr(
-        telemetry_inst.get("RETRIEVE_RAW_DATA"), st.BASE_COUNT_KEY) == 1
+    assert getattr(telemetry_inst.get("RETRIEVE_RAW_DATA"), st.BASE_COUNT_KEY) == 1
 
 
 def test_increase_sub_process_fail_count():
     """
     Check that a sub process base count can be increased.
     """
     telemetry_inst = Telemetry(**DEFAULT_TELEMETRY_PARAMS)
     telemetry_inst.increase_sub_process_fail_count("RETRIEVE_RAW_DATA")
-    assert getattr(
-        telemetry_inst.get("RETRIEVE_RAW_DATA"), st.FAIL_COUNT_KEY) == 1
+    assert getattr(telemetry_inst.get("RETRIEVE_RAW_DATA"), st.FAIL_COUNT_KEY) == 1
 
 
 def test_increase_non_exsiting_sub_process_raises_exception():
     """
     Check that a add a based count for a non existing sub process raises
     an excpetion
     """
@@ -201,16 +201,15 @@
     """
     Check that an existing sub process base count can be inreased multiple
     times and with different values
     """
     telemetry = Telemetry(**DEFAULT_TELEMETRY_PARAMS)
     telemetry.increase_sub_process_base_count("RETRIEVE_RAW_DATA")
     telemetry.increase_sub_process_base_count("RETRIEVE_RAW_DATA", increment=2)
-    assert getattr(
-        telemetry.get("RETRIEVE_RAW_DATA"), st.BASE_COUNT_KEY) == 3
+    assert getattr(telemetry.get("RETRIEVE_RAW_DATA"), st.BASE_COUNT_KEY) == 3
 
 
 def test_increase_sub_process_count_not_allowed_with_closed_telemetry():
     """
     check that a sub process base count can be added to th eTelemetry instance
     """
     telemetry_inst = Telemetry(**DEFAULT_TELEMETRY_PARAMS)
@@ -322,44 +321,44 @@
     mocker.patch(
         (
             "pipeline_telemetry.storage.memory."
             "TelemetryInMemoryStorage.store_telemetry"
         ),
         return_value=None,
     )
-    _store_telemetry_spy = mocker.spy(
-        TelemetryInMemoryStorage, "store_telemetry")
+    _store_telemetry_spy = mocker.spy(TelemetryInMemoryStorage, "store_telemetry")
     Telemetry(**DEFAULT_TELEMETRY_PARAMS).save_and_close()
     assert _store_telemetry_spy.called
 
 
 def test_get_storage_class_returns_in_memory_storage_by_default():
     """
     check that _get_storage_class method returns TelemetryInMemoryStorage
     instance if no storage class is provided
     """
     telemetry_inst = Telemetry(**DEFAULT_TELEMETRY_PARAMS)
-    assert issubclass(
-        telemetry_inst._storage_class, TelemetryInMemoryStorage)
+    assert issubclass(telemetry_inst._storage_class, TelemetryInMemoryStorage)
 
 
 def test_storage_class_returns_the_correct_storage_class():
     """
     check that storage_class attribute returns the correct
     Storage class.
     """
+
     # pylint: disable=too-few-public-methods
     class TestStorage(AbstractTelemetryStorage):
         """test class"""
 
         def store_telemetry(self, telemetry):
             """test method"""
             return None
+
     telemetry_params = DEFAULT_TELEMETRY_PARAMS.copy()
-    telemetry_params['storage_class'] = TestStorage
+    telemetry_params["storage_class"] = TestStorage
     telemetry_inst = Telemetry(**telemetry_params)
     assert telemetry_inst.storage_class is TestStorage
 
 
 def test_storage_class_close_method_closes_db():
     """
     check that _get_storage_class method returns an instance of
@@ -370,16 +369,18 @@
     storage_instance.close_db()
     assert storage_instance.db_in_memory is None
     assert storage_instance.db_cursor is None
 
 
 def test_new_telemetry_has_default_traffic_light_color():
     """New telemetry instance should have default trafic light color."""
-    assert Telemetry(**DEFAULT_TELEMETRY_PARAMS).telemetry.traffic_light == \
-        st.DEFAULT_TRAFIC_LIGHT_COLOR
+    assert (
+        Telemetry(**DEFAULT_TELEMETRY_PARAMS).telemetry.traffic_light
+        == st.DEFAULT_TRAFIC_LIGHT_COLOR
+    )
 
 
 def test_set_telemetry_traffic_light_to_orange():
     """New telemetry instance traffic light property can be set to orange."""
     tele_inst = Telemetry(**DEFAULT_TELEMETRY_PARAMS)
     tele_inst.set_orange_traffic_light()
     assert tele_inst.telemetry.traffic_light == st.TRAFIC_LIGHT_COLOR_ORANGE
@@ -432,15 +433,15 @@
 
 def test_instanciating_telemetry_with_invalid_telemetry_type():
     """
     Test that instanciating a telemetry object with invalid telemetry type
     raises an exception.
     """
     telemetry_params = DEFAULT_TELEMETRY_PARAMS.copy()
-    telemetry_params['telemetry_type'] = 'invalid_type'
+    telemetry_params["telemetry_type"] = "invalid_type"
     with pytest.raises(exceptions.InvalidTelemetryType):
         Telemetry(**telemetry_params)
 
 
 def test_validate_process_type_returns_none_with_valid_process_type():
     """
     Test that _valid_process_type validates a valid process_type by returning
@@ -452,21 +453,21 @@
 
 def test_validate_process_raises_exception_process_type_of_invalid_type():
     """
     Test that _valid_process_type raises exception when process_type is not
     of type ProcessType.
     """
     telemetry_params = DEFAULT_TELEMETRY_PARAMS.copy()
-    telemetry_params['process_type'] = "process_type_of_invalid_type"
+    telemetry_params["process_type"] = "process_type_of_invalid_type"
     with pytest.raises(exceptions.ProcessTypeMustBeOfClassProcessType):
         Telemetry(**telemetry_params)
 
 
 def test_validate_process_raises_exception_if_process_type_not_registered():
     """
     Test that _valid_process_type raises exception when process_type is not
     registered.
     """
     telemetry_params = DEFAULT_TELEMETRY_PARAMS.copy()
-    telemetry_params['process_type'] = TEST_PROCESS_TYPE_3
+    telemetry_params["process_type"] = TEST_PROCESS_TYPE_3
     with pytest.raises(exceptions.ProcessTypeNotRegistered):
         Telemetry(**telemetry_params)
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_telemetry_models/test_telemetry_data.py` & `pipeline_telemetry-1.0.0/tests/test_telemetry_models/test_telemetry_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module to test telemetry main class for pipeline telemetry module.
 """
+
 from test_data import TEST_ERROR_CODE, TEST_ERROR_CODE_2
 
 from pipeline_telemetry.data_classes import TelemetryData
 from pipeline_telemetry.settings import settings as st
 
 
 def test_telemetry_data_exists():
@@ -30,29 +31,29 @@
     tel_data = TelemetryData()
     tel_data.increase_error_count(increment=1, error_code=TEST_ERROR_CODE)
     assert getattr(tel_data, st.ERRORS_KEY)[TEST_ERROR_CODE.code] == 1
 
 
 def test_telemetry_data_inc_custom_count():
     tel_data = TelemetryData()
-    tel_data.increase_custom_count(increment=1, counter='counter')
-    assert getattr(tel_data, st.COUNTERS_KEY)['counter'] == 1
+    tel_data.increase_custom_count(increment=1, counter="counter")
+    assert getattr(tel_data, st.COUNTERS_KEY)["counter"] == 1
 
 
 def test_add_telemetry_custom_count_data():
     tel_data_1 = TelemetryData()
     tel_data_2 = TelemetryData()
-    tel_data_1.increase_custom_count(increment=1, counter='counter')
-    tel_data_2.increase_custom_count(increment=2, counter='counter')
-    tel_data_1.increase_custom_count(increment=3, counter='counter_1')
-    tel_data_2.increase_custom_count(increment=4, counter='counter_2')
+    tel_data_1.increase_custom_count(increment=1, counter="counter")
+    tel_data_2.increase_custom_count(increment=2, counter="counter")
+    tel_data_1.increase_custom_count(increment=3, counter="counter_1")
+    tel_data_2.increase_custom_count(increment=4, counter="counter_2")
     tel_data_1 += tel_data_2
-    assert getattr(tel_data_1, st.COUNTERS_KEY)['counter'] == 3
-    assert getattr(tel_data_1, st.COUNTERS_KEY)['counter_1'] == 3
-    assert getattr(tel_data_1, st.COUNTERS_KEY)['counter_2'] == 4
+    assert getattr(tel_data_1, st.COUNTERS_KEY)["counter"] == 3
+    assert getattr(tel_data_1, st.COUNTERS_KEY)["counter_1"] == 3
+    assert getattr(tel_data_1, st.COUNTERS_KEY)["counter_2"] == 4
 
 
 def test_add_telemetry_base_and_fail_count_data():
     tel_data_1 = TelemetryData()
     tel_data_2 = TelemetryData()
     tel_data_1.increase_base_count(increment=1)
     tel_data_2.increase_base_count(increment=2)
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_telemetry_models/test_telemetry_model.py` & `pipeline_telemetry-1.0.0/tests/test_telemetry_models/test_telemetry_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module to test telemetry model class for pipeline telemetry module.
 """
+
 import pytest
 from test_data import DEFAULT_TELEMETRY_MODEL_PARAMS
 
 from pipeline_telemetry.data_classes import TelemetryModel
 from pipeline_telemetry.settings import exceptions
 from pipeline_telemetry.settings import settings as st
 
@@ -14,15 +15,15 @@
 def test_telemetry_model_exists():
     """check that TelemetryModel class exists"""
     assert TelemetryModel
 
 
 def test_check_telemetry_type_raises_exception_with_inv_type():
     telemetry_params = DEFAULT_TELEMETRY_MODEL_PARAMS.copy()
-    telemetry_params[st.TELEMETRY_TYPE_KEY] = 'invalid'
+    telemetry_params[st.TELEMETRY_TYPE_KEY] = "invalid"
     with pytest.raises(exceptions.InvalidTelemetryType):
         TelemetryModel(**telemetry_params)._check_telemetry_type()
 
 
 def test_telemetry_model_can_be_added():
     tel_model_1 = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
     tel_model_2 = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
@@ -46,116 +47,128 @@
     Test that adding up to telemetry model instances returns a TelemetryModel
     instance with aggregated Traffic Ligth counters in aggregation telemetry
     subprocess.
     """
     tel_model_1 = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
     tel_model_2 = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
     tel_model_3 = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
-    tel_model_2.get_sub_process_data('sub_process').increase_custom_count(
-        increment=1, counter='counter_1')
-    tel_model_2.get_sub_process_data('sub_process').increase_custom_count(
-        increment=2, counter='counter_2')
-    tel_model_3.get_sub_process_data('sub_process').increase_custom_count(
-        increment=2, counter='counter_1')
-    tel_model_3.get_sub_process_data('sub_process').increase_custom_count(
-        increment=4, counter='counter_3')
+    tel_model_2.get_sub_process_data("sub_process").increase_custom_count(
+        increment=1, counter="counter_1"
+    )
+    tel_model_2.get_sub_process_data("sub_process").increase_custom_count(
+        increment=2, counter="counter_2"
+    )
+    tel_model_3.get_sub_process_data("sub_process").increase_custom_count(
+        increment=2, counter="counter_1"
+    )
+    tel_model_3.get_sub_process_data("sub_process").increase_custom_count(
+        increment=4, counter="counter_3"
+    )
     tel_model_added = tel_model_1 + tel_model_2
     tel_model_added += tel_model_3
     aggregation_data = tel_model_added.telemetry[st.AGGREGATION_KEY]
-    telemetry_data = tel_model_added.telemetry['sub_process']
-    assert getattr(aggregation_data, st.COUNTERS_KEY)[
-        st.TRAFIC_LIGHT_COLOR_GREEN] == 2
+    telemetry_data = tel_model_added.telemetry["sub_process"]
+    assert getattr(aggregation_data, st.COUNTERS_KEY)[st.TRAFIC_LIGHT_COLOR_GREEN] == 2
     assert getattr(telemetry_data, st.COUNTERS_KEY) == {
-        'counter_1': 3,
-        'counter_2': 2,
-        'counter_3': 4}
+        "counter_1": 3,
+        "counter_2": 2,
+        "counter_3": 4,
+    }
 
 
 def test_telemetry_model_addition_aggregates_errors():
     """
     Test that adding up to telemetry model instances returns a TelemetryModel
     instance with aggregated errors.
     """
     tel_model_1 = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
     tel_model_2 = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
     tel_model_3 = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
-    tel_model_2.get_sub_process_data('sub_process')._increase_error_count(
-        increment=1, error_code_key='error_1')
-    tel_model_2.get_sub_process_data('sub_process')._increase_error_count(
-        increment=2, error_code_key='error_2')
-    tel_model_3.get_sub_process_data('sub_process')._increase_error_count(
-        increment=2, error_code_key='error_1')
-    tel_model_3.get_sub_process_data('sub_process')._increase_error_count(
-        increment=4, error_code_key='error_3')
+    tel_model_2.get_sub_process_data("sub_process")._increase_error_count(
+        increment=1, error_code_key="error_1"
+    )
+    tel_model_2.get_sub_process_data("sub_process")._increase_error_count(
+        increment=2, error_code_key="error_2"
+    )
+    tel_model_3.get_sub_process_data("sub_process")._increase_error_count(
+        increment=2, error_code_key="error_1"
+    )
+    tel_model_3.get_sub_process_data("sub_process")._increase_error_count(
+        increment=4, error_code_key="error_3"
+    )
     tel_model_added = tel_model_1 + tel_model_2
     tel_model_added += tel_model_3
-    telemetry_data = tel_model_added.telemetry['sub_process']
+    telemetry_data = tel_model_added.telemetry["sub_process"]
     assert getattr(telemetry_data, st.ERRORS_KEY) == {
-        'error_1': 3,
-        'error_2': 2,
-        'error_3': 4}
+        "error_1": 3,
+        "error_2": 2,
+        "error_3": 4,
+    }
 
 
 def test_telemetry_model_addition_aggregates_traffic_lights():
     """
     Test that adding up to telemetry model instances returns a TelemetryModel
     instance with aggregated Traffic Ligth counters in aggregation telemetry
     subprocess.
     """
     tel_model_1 = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
     tel_model_2 = TelemetryModel(
-        **(DEFAULT_TELEMETRY_MODEL_PARAMS |
-           {'traffic_light': st.TRAFIC_LIGHT_COLOR_ORANGE}))
+        **(
+            DEFAULT_TELEMETRY_MODEL_PARAMS
+            | {"traffic_light": st.TRAFIC_LIGHT_COLOR_ORANGE}
+        )
+    )
     tel_model_3 = TelemetryModel(
-        **(DEFAULT_TELEMETRY_MODEL_PARAMS |
-           {'traffic_light': st.TRAFIC_LIGHT_COLOR_RED}))
+        **(
+            DEFAULT_TELEMETRY_MODEL_PARAMS
+            | {"traffic_light": st.TRAFIC_LIGHT_COLOR_RED}
+        )
+    )
     tel_model_added = tel_model_1 + tel_model_2
     tel_model_added += tel_model_3
     aggregation_data = tel_model_added.telemetry[st.AGGREGATION_KEY]
-    aggregation_data_counters = getattr(
-        aggregation_data, st.COUNTERS_KEY)
+    aggregation_data_counters = getattr(aggregation_data, st.COUNTERS_KEY)
     assert st.TRAFIC_LIGHT_COLOR_ORANGE in aggregation_data_counters
     assert st.TRAFIC_LIGHT_COLOR_RED in aggregation_data_counters
     assert aggregation_data_counters[st.TRAFIC_LIGHT_COLOR_RED] == 1
     assert aggregation_data_counters[st.TRAFIC_LIGHT_COLOR_ORANGE] == 1
 
 
 def test_telemetry_model_addition_aggregates_io_time():
     """
     Test that adding up to telemetry model instances returns a TelemetryModel
     instance with aggregated io time rounded in seconds
     """
     tel_model_1 = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
     tel_model_2 = TelemetryModel(
-        **(DEFAULT_TELEMETRY_MODEL_PARAMS |
-           {'io_time_in_seconds': 1.2}))
+        **(DEFAULT_TELEMETRY_MODEL_PARAMS | {"io_time_in_seconds": 1.2})
+    )
     tel_model_3 = TelemetryModel(
-        **(DEFAULT_TELEMETRY_MODEL_PARAMS |
-           {'io_time_in_seconds': 1.7}))
+        **(DEFAULT_TELEMETRY_MODEL_PARAMS | {"io_time_in_seconds": 1.7})
+    )
     tel_model_added = tel_model_1 + tel_model_2
     tel_model_added += tel_model_3
     aggregation_data = tel_model_added.telemetry[st.AGGREGATION_KEY]
-    aggregation_data_counters = getattr(
-        aggregation_data, st.COUNTERS_KEY)
-    assert 'io_time_in_seconds' in aggregation_data_counters
-    assert aggregation_data_counters['io_time_in_seconds'] == 3
+    aggregation_data_counters = getattr(aggregation_data, st.COUNTERS_KEY)
+    assert "io_time_in_seconds" in aggregation_data_counters
+    assert aggregation_data_counters["io_time_in_seconds"] == 3
 
 
 def test_telemetry_model_addition_aggregates_run_time():
     """
     Test that adding up to telemetry model instances returns a TelemetryModel
     instance with aggregated run time rounded in seconds
     """
     tel_model_1 = TelemetryModel(**DEFAULT_TELEMETRY_MODEL_PARAMS)
     tel_model_2 = TelemetryModel(
-        **(DEFAULT_TELEMETRY_MODEL_PARAMS |
-           {'run_time_in_seconds': 1.2}))
+        **(DEFAULT_TELEMETRY_MODEL_PARAMS | {"run_time_in_seconds": 1.2})
+    )
     tel_model_3 = TelemetryModel(
-        **(DEFAULT_TELEMETRY_MODEL_PARAMS |
-           {'run_time_in_seconds': 1.7}))
+        **(DEFAULT_TELEMETRY_MODEL_PARAMS | {"run_time_in_seconds": 1.7})
+    )
     tel_model_added = tel_model_1 + tel_model_2
     tel_model_added += tel_model_3
     aggregation_data = tel_model_added.telemetry[st.AGGREGATION_KEY]
-    aggregation_data_counters = getattr(
-        aggregation_data, st.COUNTERS_KEY)
-    assert 'run_time_in_seconds' in aggregation_data_counters
-    assert aggregation_data_counters['run_time_in_seconds'] == 3
+    aggregation_data_counters = getattr(aggregation_data, st.COUNTERS_KEY)
+    assert "run_time_in_seconds" in aggregation_data_counters
+    assert aggregation_data_counters["run_time_in_seconds"] == 3
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_validators/test_dict_validator.py` & `pipeline_telemetry-1.0.0/tests/test_validators/test_dict_validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """
 module to test validate module of data-validator
 """
+
 import pytest
 from test_data import InstructionTestClass
 
 from pipeline_telemetry.settings import exceptions
 from pipeline_telemetry.validators.dict_validator import DictValidator
 from pipeline_telemetry.validators.has_key import HasKey
 
 # pylint: disable=protected-access
 
 
 def test_dict_validator_class_exists():
-    """ check that DictValidator class exists """
+    """check that DictValidator class exists"""
     assert DictValidator
 
 
 def test_dict_validator_has_instructions():
-    """ check that DictValidator class has instructions attribute"""
+    """check that DictValidator class has instructions attribute"""
     assert DictValidator._instructions
 
 
 def test_dict_validator_register_instruction():
     """
     check that register_instruction method registers an instruction
     """
     # ensure that test is not corrupted by previous registrations
     DictValidator._instructions = {}
     DictValidator.register_instruction(InstructionTestClass)
-    assert InstructionTestClass.INSTRUCTION in \
-        list(DictValidator._instructions.keys())
+    assert InstructionTestClass.INSTRUCTION in list(DictValidator._instructions.keys())
 
 
 def test_dict_validator_register_instruction_twice():
     """
     check that register_instruction method raises exception if you try to
     register an instruction twice
     """
@@ -46,41 +46,42 @@
 
 def test_apply_rule_raises_exception_with_unregistered_instruction():
     """
     test that _apply_rule method returns an exception when a rule with an
     unregistered instruction is provided
     """
     with pytest.raises(exceptions.UnknownInstruction):
-        DictValidator()._apply_rule(
-            {}, ('unkwown_rule', {'rule details': 'details'}))
+        DictValidator()._apply_rule({}, ("unkwown_rule", {"rule details": "details"}))
 
 
 def test_apply_rule_calls_do_validate_method(mocker):
     """
     test that _apply_rule method calls the `validate` method on the instruction
     class and returns the value receive from the validate method
     """
     # as previous tests might have cleaned the instruction set it needs to be
     # reregistered
     DictValidator.register_instruction(HasKey)
-    rule = ('has_key', {'has_key_details': 'rule'})
-    mocker.patch('pipeline_telemetry.validators.has_key.HasKey.validate',
-                 return_value='return_value')
-    _do_validate_spy = mocker.spy(
-        HasKey, 'validate')
+    rule = ("has_key", {"has_key_details": "rule"})
+    mocker.patch(
+        "pipeline_telemetry.validators.has_key.HasKey.validate",
+        return_value="return_value",
+    )
+    _do_validate_spy = mocker.spy(HasKey, "validate")
     return_value = DictValidator()._apply_rule({}, rule)
-    assert return_value == 'return_value'
+    assert return_value == "return_value"
     assert _do_validate_spy.called
 
 
 def test_instruction_from_rule_succes():
-    """ test instruction returns instruction when given a valid rule """
-    valid_rule = ('instruction_in_valid_rule',  {'rule_details': 'test'})
-    assert DictValidator._instruction_from_rule(valid_rule) == \
-        'instruction_in_valid_rule'
+    """test instruction returns instruction when given a valid rule"""
+    valid_rule = ("instruction_in_valid_rule", {"rule_details": "test"})
+    assert (
+        DictValidator._instruction_from_rule(valid_rule) == "instruction_in_valid_rule"
+    )
 
 
 def test_instruction_from_rule_with_more_the_one_rule():
-    """ test instruction returns instruction when given a valid rule """
-    to_many_rules = {'rule_1': 'test1', 'rule_2': 'test2'}
+    """test instruction returns instruction when given a valid rule"""
+    to_many_rules = {"rule_1": "test1", "rule_2": "test2"}
     with pytest.raises(exceptions.RuleCanHaveOnlyOneInstruction):
         DictValidator._instruction_from_rule(to_many_rules)
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_validators/test_entries_have_key.py` & `pipeline_telemetry-1.0.0/tests/test_validators/test_entries_have_key.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,202 +1,214 @@
 """
 module to test entries_have_key instruction class
 """
-from pipeline_telemetry.validators.entries_have_key import EntriesHaveKey, \
-    EntriesHaveKeyRuleData
+
+from pipeline_telemetry.validators.entries_have_key import (
+    EntriesHaveKey,
+    EntriesHaveKeyRuleData,
+)
 
 # pylint: disable=protected-access
 
 
 def test_has_key_class_exists():
-    """ check that HasKey class exists """
+    """check that HasKey class exists"""
     assert EntriesHaveKey
 
 
 def test_has_key_class_is_singelton():
-    """ check that HasKey is a singleton class """
+    """check that HasKey is a singleton class"""
     instance_one = EntriesHaveKey()
     instance_two = EntriesHaveKey()
     assert instance_one is instance_two
 
 
 def test_get_field_name_method():
     """
     check that _get_field_name method returns value of
     field_name that is in scope of validation
     """
     rule_content = EntriesHaveKeyRuleData(
-        **{'field_name': 'test', 'must_have_key': 'test'})
-    assert EntriesHaveKey._get_field_name(rule_content) == 'test'
+        **{"field_name": "test", "must_have_key": "test"}
+    )
+    assert EntriesHaveKey._get_field_name(rule_content) == "test"
 
 
 def test_get_must_have_key_method():
     """
     check that _get_must_have_key method returns value of
     must_have_key that is in scope of validation
     """
     rule_content = EntriesHaveKeyRuleData(
-        **{'field_name': 'fieldname', 'must_have_key': 'test'})
-    assert EntriesHaveKey._get_must_have_key(rule_content) == 'test'
+        **{"field_name": "fieldname", "must_have_key": "test"}
+    )
+    assert EntriesHaveKey._get_must_have_key(rule_content) == "test"
 
 
 def test_validate_field_exists():
     """
     test that _validate_field_exists method returns empty list when
     entries field exists
     """
-    dict_to_validate = {'items': [{'key': 1}, {'key': 2}]}
+    dict_to_validate = {"items": [{"key": 1}, {"key": 2}]}
     rule_data = EntriesHaveKeyRuleData(
-        **{'field_name': 'items', 'must_have_key': 'key'})
+        **{"field_name": "items", "must_have_key": "key"}
+    )
 
-    assert EntriesHaveKey._validate_field_exists(
-        dict_to_validate, rule_data) == []
+    assert EntriesHaveKey._validate_field_exists(dict_to_validate, rule_data) == []
 
 
 def test_validate_field_exists_returns_error():
     """
     test that _validate_field_exists method returns empty list when
     entries field exists
     """
-    dict_to_validate = {'not_items': [{'key': 1}, {'key': 2}]}
+    dict_to_validate = {"not_items": [{"key": 1}, {"key": 2}]}
     rule_content = EntriesHaveKeyRuleData(
-        **{'field_name': 'items', 'must_have_key': 'key'})
-    errors = EntriesHaveKey._validate_field_exists(
-        dict_to_validate, rule_content)
+        **{"field_name": "items", "must_have_key": "key"}
+    )
+    errors = EntriesHaveKey._validate_field_exists(dict_to_validate, rule_content)
 
     assert len(errors) == 1
-    assert 'Entries field does not exist' in errors[0].description
+    assert "Entries field does not exist" in errors[0].description
 
 
 def test_validate_entries_have_key():
     """
     test that _validate_entries_have_key method returns empty list when all
     entries have the right key
     """
-    dict_to_validate = {'items': [{'key': 1}, {'key': 2}]}
+    dict_to_validate = {"items": [{"key": 1}, {"key": 2}]}
     rule_content = EntriesHaveKeyRuleData(
-        **{'field_name': 'items', 'must_have_key': 'key'})
+        **{"field_name": "items", "must_have_key": "key"}
+    )
 
-    assert EntriesHaveKey._validate_entries_have_key(
-        dict_to_validate, rule_content) == []
+    assert (
+        EntriesHaveKey._validate_entries_have_key(dict_to_validate, rule_content) == []
+    )
 
 
 def test_validate_entries_have_nested_key():
     """
     test that _validate_entries_have_key method returns empty list when all
     entries have the right key
     """
-    dict_to_validate = {'items': [{'key': {'nested_key': 2}}]}
+    dict_to_validate = {"items": [{"key": {"nested_key": 2}}]}
     rule_content = EntriesHaveKeyRuleData(
-        **{'field_name': 'items', 'must_have_key': 'key.nested_key'})
+        **{"field_name": "items", "must_have_key": "key.nested_key"}
+    )
 
-    assert EntriesHaveKey._validate_entries_have_key(
-        dict_to_validate, rule_content) == []
+    assert (
+        EntriesHaveKey._validate_entries_have_key(dict_to_validate, rule_content) == []
+    )
 
 
 def test_validate_entries_have_key_with_missing_key():
     """
     test that _validate_entries_have_key method returns list with has_key
     error when a key is missing
     """
-    dict_to_validate = {'items': [{'not_key': 1}, {'key': 2}]}
+    dict_to_validate = {"items": [{"not_key": 1}, {"key": 2}]}
     rule_content = EntriesHaveKeyRuleData(
-        **{'field_name': 'items', 'must_have_key': 'key'})
+        **{"field_name": "items", "must_have_key": "key"}
+    )
 
-    errors = EntriesHaveKey._validate_entries_have_key(
-        dict_to_validate, rule_content)
+    errors = EntriesHaveKey._validate_entries_have_key(dict_to_validate, rule_content)
 
     assert len(errors) == 1
-    assert 'Key missing in entry' in errors[0].description
+    assert "Key missing in entry" in errors[0].description
 
 
 def test_validate_entries_have_key_with_non_dict_items():
     """
     test that _validate_entries_have_key method returns list with
     entry_is_not_a_dict error when entry is not a dicy
     """
-    dict_to_validate = {'items': ['not_a_dict', {'key': 2}]}
+    dict_to_validate = {"items": ["not_a_dict", {"key": 2}]}
     rule_content = EntriesHaveKeyRuleData(
-        **{'field_name': 'items', 'must_have_key': 'key'})
+        **{"field_name": "items", "must_have_key": "key"}
+    )
 
-    errors = EntriesHaveKey._validate_entries_have_key(
-        dict_to_validate, rule_content)
+    errors = EntriesHaveKey._validate_entries_have_key(dict_to_validate, rule_content)
 
     assert len(errors) == 1
-    assert 'Entry that needs to have a key is not a dict' in \
-        errors[0].description
+    assert "Entry that needs to have a key is not a dict" in errors[0].description
 
 
 def test_validate_entries_have_keys_with_missing_key():
     """
     test that _validate_entries_have_key method returns list with has_key
     errors when a all keys are missing
     """
-    dict_to_validate = {'items': [{'not_key': 1}, {'also_not_key': 2}]}
+    dict_to_validate = {"items": [{"not_key": 1}, {"also_not_key": 2}]}
     rule_content = EntriesHaveKeyRuleData(
-        **{'field_name': 'items', 'must_have_key': 'key'})
+        **{"field_name": "items", "must_have_key": "key"}
+    )
 
-    errors = EntriesHaveKey._validate_entries_have_key(
-        dict_to_validate, rule_content)
+    errors = EntriesHaveKey._validate_entries_have_key(dict_to_validate, rule_content)
 
     assert len(errors) == 2
 
 
 def test_validate_calls_validate_field_exists(mocker):
     """
     test that _validate method calls the _validate_field_exists method
     """
-    dict_to_validate = {'not_items': [{'not_key': 1}, {'also_not_key': 2}]}
+    dict_to_validate = {"not_items": [{"not_key": 1}, {"also_not_key": 2}]}
     rule_content = EntriesHaveKeyRuleData(
-        **{'field_name': 'items', 'must_have_key': 'key'})
+        **{"field_name": "items", "must_have_key": "key"}
+    )
 
-    _validate_field_exists_spy = mocker.spy(
-        EntriesHaveKey, '_validate_field_exists')
+    _validate_field_exists_spy = mocker.spy(EntriesHaveKey, "_validate_field_exists")
 
     EntriesHaveKey._validate(dict_to_validate, rule_content)
 
     assert _validate_field_exists_spy.called
 
 
 def test_validate_calls_validate_type_entries_field(mocker):
     """
     test that _validate method calls the _validate_type_entries_field method
     """
-    dict_to_validate = {'items': 'not a list or a dict'}
+    dict_to_validate = {"items": "not a list or a dict"}
     rule_content = EntriesHaveKeyRuleData(
-        **{'field_name': 'items', 'must_have_key': 'key'})
+        **{"field_name": "items", "must_have_key": "key"}
+    )
 
     _validate_type_entries_field_spy = mocker.spy(
-        EntriesHaveKey, '_validate_type_entries_field')
+        EntriesHaveKey, "_validate_type_entries_field"
+    )
 
     EntriesHaveKey._validate(dict_to_validate, rule_content)
 
     assert _validate_type_entries_field_spy.called
 
 
 def test_validate_calls_validate_entries_have_key(mocker):
     """
     test that _validate method calls the _validate_type_entries_field method
     """
-    dict_to_validate = {'items': [{'a': 1}]}
+    dict_to_validate = {"items": [{"a": 1}]}
     rule_content = EntriesHaveKeyRuleData(
-        **{'field_name': 'items', 'must_have_key': 'key'})
+        **{"field_name": "items", "must_have_key": "key"}
+    )
 
     _validate_entries_have_key_spy = mocker.spy(
-        EntriesHaveKey, '_validate_type_entries_field')
+        EntriesHaveKey, "_validate_type_entries_field"
+    )
 
     EntriesHaveKey._validate(dict_to_validate, rule_content)
 
     assert _validate_entries_have_key_spy.called
 
 
 def test_validate_calls_validate(mocker):
     """
     test that public validate method calls the _validate method
     """
-    dict_to_validate = {'items': [{'a': 1}]}
-    rule_content = {'field_name': 'items', 'must_have_key': 'key'}
+    dict_to_validate = {"items": [{"a": 1}]}
+    rule_content = {"field_name": "items", "must_have_key": "key"}
 
-    _validate_spy = mocker.spy(EntriesHaveKey, '_validate')
+    _validate_spy = mocker.spy(EntriesHaveKey, "_validate")
     EntriesHaveKey.validate(dict_to_validate, rule_content)
 
     assert _validate_spy.called
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_validators/test_has_key_instruction.py` & `pipeline_telemetry-1.0.0/tests/test_validators/test_has_key_instruction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,98 +1,97 @@
 """
 module to test has_key instruction class
 """
+
 from test_data import TEST_ERROR_CODE
 
 from pipeline_telemetry.settings.telemetry_errors import ErrorCode
-from pipeline_telemetry.validators.abstract_validator_instruction import \
-    BaseValidatorInstructionRuleData
+from pipeline_telemetry.validators.abstract_validator_instruction import (
+    BaseValidatorInstructionRuleData,
+)
 from pipeline_telemetry.validators.has_key import HasKey
 
 # pylint: disable=protected-access
 
 
 def test_has_key_class_exists():
-    """ check that HasKey class exists """
+    """check that HasKey class exists"""
     assert HasKey
 
 
 def test_has_key_class_is_singelton():
-    """ check that HasKey is a singleton class """
+    """check that HasKey is a singleton class"""
     instance_one = HasKey()
     instance_two = HasKey()
     assert instance_one is instance_two
 
 
 def test_get_field_name_method():
     """
     check that _get_field_name method returns value of
     field_name that is in scope of validation
     """
-    rule_data = BaseValidatorInstructionRuleData(**{'field_name': 'test'})
-    assert HasKey._get_field_name(rule_data) == 'test'
+    rule_data = BaseValidatorInstructionRuleData(**{"field_name": "test"})
+    assert HasKey._get_field_name(rule_data) == "test"
 
 
 def test_validation_error_method():
     """
     Check that _validation_error method returns a list with
     ErrorCode instance.
     """
-    validation_error_list = HasKey._validation_error(
-        TEST_ERROR_CODE, 'test_error_data')
+    validation_error_list = HasKey._validation_error(TEST_ERROR_CODE, "test_error_data")
     validation_error = validation_error_list[0]
     assert isinstance(validation_error_list, list)
     assert isinstance(validation_error, ErrorCode)
 
 
 def test_validate_valid_dict():
-    """Test that a dict with right key returns empty error list
-    """
-    valid_dict = {'correct_key': 'value'}
-    rule_dict = {'field_name': 'correct_key'}
+    """Test that a dict with right key returns empty error list"""
+    valid_dict = {"correct_key": "value"}
+    rule_dict = {"field_name": "correct_key"}
     validation_result = HasKey.validate(
         dict_to_validate=valid_dict, rule_dict=rule_dict
     )
     assert validation_result == []
 
 
 def test_validate_valid_dict_with_nested_key():
     """
     Test that a dict with right key returns empty error list when the nested
     key in input dict is found
     """
-    valid_dict = {'correct_key': {'nested_key': 'value'}}
-    rule_dict = {'field_name': 'correct_key.nested_key'}
+    valid_dict = {"correct_key": {"nested_key": "value"}}
+    rule_dict = {"field_name": "correct_key.nested_key"}
     validation_result = HasKey.validate(
         dict_to_validate=valid_dict, rule_dict=rule_dict
     )
     assert validation_result == []
 
 
 def test_validate_invalid_dict():
     """
     Test that a dict without right key returns a list with error_code
     KEY_NOT_FOUND_001 and the field_name in the error_data
 
     """
-    invalid_dict = {'incorrect_key': 'value'}
-    rule_dict = {'field_name': 'correct_key'}
+    invalid_dict = {"incorrect_key": "value"}
+    rule_dict = {"field_name": "correct_key"}
     validation_result = HasKey.validate(
         dict_to_validate=invalid_dict, rule_dict=rule_dict
     )
     assert len(validation_result) == 1
-    assert validation_result[0].code == 'HAS_KEY_ERR_0001@KEY_<correct_key>'
+    assert validation_result[0].code == "HAS_KEY_ERR_0001@KEY_<correct_key>"
 
 
 def test_validate_invalid_nested_dict():
     """
     Test that a nested dict without right nested key returns a list with
     error_code KEY_NOT_FOUND_001 and the nested field_name in the error_data.
     """
-    invalid_dict = {'incorrect_key': {'nested_key': 'value'}}
-    rule_dict = {'field_name': 'correct_key.nested_key'}
+    invalid_dict = {"incorrect_key": {"nested_key": "value"}}
+    rule_dict = {"field_name": "correct_key.nested_key"}
     validation_result = HasKey.validate(
         dict_to_validate=invalid_dict, rule_dict=rule_dict
     )
     assert len(validation_result) == 1
-    assert validation_result[0].code == \
-        'HAS_KEY_ERR_0001@KEY_<correct_key.nested_key>'
+    assert validation_result[0].code == "HAS_KEY_ERR_0001@KEY_<correct_key.nested_key>"
```

### Comparing `pipeline-telemetry-0.9.4/tests/test_validators/test_validate_entries.py` & `pipeline_telemetry-1.0.0/tests/test_validators/test_validate_entries.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,140 +1,140 @@
 """
 module to test has_key instruction class
 """
+
 # pylint: disable=protected-access
 import pytest
 from test_data import TEST_ERROR_CODE
 
-from pipeline_telemetry.settings.exceptions import \
-    ExpectedCountMustBePositiveInt
+from pipeline_telemetry.settings.exceptions import ExpectedCountMustBePositiveInt
 from pipeline_telemetry.settings.telemetry_errors import ErrorCode
-from pipeline_telemetry.validators.validate_entries import ValidateEntries, \
-    ValidateEntriesRuleData
+from pipeline_telemetry.validators.validate_entries import (
+    ValidateEntries,
+    ValidateEntriesRuleData,
+)
 
 
 def test_validate_entries_class_exists():
-    """ check that ValidateEntries class exists """
+    """check that ValidateEntries class exists"""
     assert ValidateEntries
 
 
 def test_validate_entries_class_is_singleton_clss():
     """Check that ValidateEntries class is a singleton class."""
     assert ValidateEntries() is ValidateEntries()
 
 
 def test_validate_rule_method_with_neg_expected_count_raises_exception():
     """
     check that _validate_rule method raises exception when expected_count
     is a negative integer
     """
     with pytest.raises(ExpectedCountMustBePositiveInt):
-        ValidateEntriesRuleData(
-            **{'field_name': 'test', 'expected_count': -1})
+        ValidateEntriesRuleData(**{"field_name": "test", "expected_count": -1})
 
 
 def test_get_field_name_method():
     """
     check that _get_field_name method returns value of
     field_name that is in scope of validation
     """
-    rule_data = ValidateEntriesRuleData(
-        **{'field_name': 'test', 'expected_count': 1})
-    assert ValidateEntries._get_field_name(rule_data) == 'test'
+    rule_data = ValidateEntriesRuleData(**{"field_name": "test", "expected_count": 1})
+    assert ValidateEntries._get_field_name(rule_data) == "test"
 
 
 def test_get_expected_count():
     """
     check that _get_expected_count method returns value of
     expected_count
     """
-    rule_data = ValidateEntriesRuleData(
-        **{'field_name': 'test', 'expected_count': 1})
+    rule_data = ValidateEntriesRuleData(**{"field_name": "test", "expected_count": 1})
 
     assert ValidateEntries._get_expected_count(rule_data) == 1
 
 
 def test_validation_error_method():
     """
     check that _validation_error method returns instance
     of ErrorCode with fieldname in error_data
     """
     validation_error_list = ValidateEntries._validation_error(
-        TEST_ERROR_CODE, 'test_error_data')
+        TEST_ERROR_CODE, "test_error_data"
+    )
     validation_error = validation_error_list[0]
     assert isinstance(validation_error_list, list)
     assert isinstance(validation_error, ErrorCode)
-    assert validation_error.error_data == 'test_error_data'
+    assert validation_error.error_data == "test_error_data"
 
 
 def test_validate_valid_dict():
     """
     Test that a dict with a field with a list with the expected count (length)
     returns empty error list
     """
-    valid_dict = {'correct_key': [1, 2, 3, 4]}
-    rule_dict = {'field_name': 'correct_key', 'expected_count': 4}
+    valid_dict = {"correct_key": [1, 2, 3, 4]}
+    rule_dict = {"field_name": "correct_key", "expected_count": 4}
     validation_result = ValidateEntries.validate(
         dict_to_validate=valid_dict, rule_dict=rule_dict
     )
     assert validation_result == []
 
 
 def test_validate_valid_dict_with_nested_key():
     """
     Test that a dict of the right length in nested key returns an empty error
     lits
     """
-    valid_dict = {'key': {'nested_key': {'a': 1, 'b': 2}}}
-    rule_dict = {'field_name': 'key.nested_key', 'expected_count': 2}
+    valid_dict = {"key": {"nested_key": {"a": 1, "b": 2}}}
+    rule_dict = {"field_name": "key.nested_key", "expected_count": 2}
     validation_result = ValidateEntries.validate(
         dict_to_validate=valid_dict, rule_dict=rule_dict
     )
     assert validation_result == []
 
 
 def test_validate_invalid_dict():
     """
     Test that a dict without right key returns a list with error_code
     VALIDATE_ENTRIES_ERR_001 and the field_name in the error_data
 
     """
-    invalid_dict = {'incorrect_key': 'value'}
-    rule_dict = {'field_name': 'correct_key', 'expected_count': 2}
+    invalid_dict = {"incorrect_key": "value"}
+    rule_dict = {"field_name": "correct_key", "expected_count": 2}
     validation_result = ValidateEntries.validate(
         dict_to_validate=invalid_dict, rule_dict=rule_dict
     )
     assert len(validation_result) == 1
-    assert validation_result[0].code == 'VALIDATE_ENTRIES_ERR_001'
-    assert validation_result[0].error_data == 'correct_key'
+    assert validation_result[0].code == "VALIDATE_ENTRIES_ERR_001"
+    assert validation_result[0].error_data == "correct_key"
 
 
 def test_validate_dict_with_wrong_type_in_field():
     """
     Test that a dict without right key returns a list with error_code
     VALIDATE_ENTRIES_ERR_002 and the field_name in the error_data
 
     """
-    invalid_dict = {'correct_key': 'value'}
-    rule_dict = {'field_name': 'correct_key', 'expected_count': 2}
+    invalid_dict = {"correct_key": "value"}
+    rule_dict = {"field_name": "correct_key", "expected_count": 2}
     validation_result = ValidateEntries.validate(
         dict_to_validate=invalid_dict, rule_dict=rule_dict
     )
     assert len(validation_result) == 1
-    assert validation_result[0].code == 'VALIDATE_ENTRIES_ERR_002'
-    assert validation_result[0].error_data == 'correct_key'
+    assert validation_result[0].code == "VALIDATE_ENTRIES_ERR_002"
+    assert validation_result[0].error_data == "correct_key"
 
 
 def test_validate_dict_with_wrong_number_of_entries():
     """
     Test that a dict without right key returns a list with error_code
     VALIDATE_ENTRIES_ERR_003 and the field_name in the error_data
 
     """
-    invalid_dict = {'correct_key': [1, 2, 3]}
-    rule_dict = {'field_name': 'correct_key', 'expected_count': 2}
+    invalid_dict = {"correct_key": [1, 2, 3]}
+    rule_dict = {"field_name": "correct_key", "expected_count": 2}
     validation_result = ValidateEntries.validate(
         dict_to_validate=invalid_dict, rule_dict=rule_dict
     )
     assert len(validation_result) == 1
-    assert validation_result[0].code == 'VALIDATE_ENTRIES_ERR_003'
-    assert validation_result[0].error_data == 'correct_key'
+    assert validation_result[0].code == "VALIDATE_ENTRIES_ERR_003"
+    assert validation_result[0].error_data == "correct_key"
```

