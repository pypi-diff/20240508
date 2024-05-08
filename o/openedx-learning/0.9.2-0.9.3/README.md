# Comparing `tmp/openedx_learning-0.9.2.tar.gz` & `tmp/openedx_learning-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx_learning-0.9.2.tar", last modified: Thu Apr 18 17:58:39 2024, max compression
+gzip compressed data, was "openedx_learning-0.9.3.tar", last modified: Wed May  8 19:16:13 2024, max compression
```

## Comparing `openedx_learning-0.9.2.tar` & `openedx_learning-0.9.3.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.866148 openedx_learning-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-04-18 17:58:39.866148 openedx_learning-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.846148 openedx_learning-0.9.2/openedx_learning/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.850148 openedx_learning-0.9.2/openedx_learning/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.850148 openedx_learning-0.9.2/openedx_learning/contrib/media_server/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/contrib/media_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/contrib/media_server/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/contrib/media_server/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/contrib/media_server/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.850148 openedx_learning-0.9.2/openedx_learning/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.850148 openedx_learning-0.9.2/openedx_learning/core/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/components/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/components/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/components/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.850148 openedx_learning-0.9.2/openedx_learning/core/components/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/components/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/components/migrations/0002_alter_componentversioncontent_key.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/components/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/components/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.850148 openedx_learning-0.9.2/openedx_learning/core/contents/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/contents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/contents/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/contents/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/contents/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.850148 openedx_learning-0.9.2/openedx_learning/core/contents/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/contents/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/contents/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15143 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/contents/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.854148 openedx_learning-0.9.2/openedx_learning/core/publishing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/publishing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/publishing/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    14254 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/publishing/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/publishing/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.854148 openedx_learning-0.9.2/openedx_learning/core/publishing/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/publishing/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/publishing/migrations/0002_alter_learningpackage_key_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/publishing/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13412 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/publishing/model_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    20321 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/core/publishing/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.854148 openedx_learning-0.9.2/openedx_learning/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/lib/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/lib/collations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/lib/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/lib/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/lib/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/lib/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.854148 openedx_learning-0.9.2/openedx_learning/rest_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/rest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/rest_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/rest_api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.854148 openedx_learning-0.9.2/openedx_learning/rest_api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/rest_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/rest_api/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_learning/rest_api/v1/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.866148 openedx_learning-0.9.2/openedx_learning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-04-18 17:58:39.000000 openedx_learning-0.9.2/openedx_learning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-18 17:58:39.000000 openedx_learning-0.9.2/openedx_learning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:58:39.000000 openedx_learning-0.9.2/openedx_learning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:58:39.000000 openedx_learning-0.9.2/openedx_learning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-18 17:58:39.000000 openedx_learning-0.9.2/openedx_learning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 17:58:39.000000 openedx_learning-0.9.2/openedx_learning.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.854148 openedx_learning-0.9.2/openedx_tagging/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.854148 openedx_learning-0.9.2/openedx_tagging/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.858148 openedx_learning-0.9.2/openedx_tagging/core/tagging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.858148 openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/import_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/template.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.862148 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0001_squashed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0002_auto_20230718_2026.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0003_auto_20230721_1238.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0004_auto_20230723_2001.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0005_language_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0006_alter_objecttag_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0006_auto_20230802_1631.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0007_tag_import_task_log_null_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0008_taxonomy_description_not_null.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0009_alter_objecttag_object_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0010_cleanups.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0011_remove_required.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0012_language_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0013_tag_parent_blank.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0014_minor_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0015_taxonomy_export_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0016_object_tag_export_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0017_alter_tagimporttask_status.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.862148 openedx_learning-0.9.2/openedx_tagging/core/tagging/models/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39335 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/models/import_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     9062 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/models/system_defined.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.862148 openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/paginators.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.866148 openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/v1/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    35581 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/v1/views_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/core/tagging/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/openedx_tagging/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:58:39.866148 openedx_learning-0.9.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-18 17:58:39.866148 openedx_learning-0.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2930 2024-04-18 17:58:36.000000 openedx_learning-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.936154 openedx_learning-0.9.3/openedx_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.936154 openedx_learning-0.9.3/openedx_learning/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.936154 openedx_learning-0.9.3/openedx_learning/contrib/media_server/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/contrib/media_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/contrib/media_server/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/contrib/media_server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/contrib/media_server/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.936154 openedx_learning-0.9.3/openedx_learning/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.940154 openedx_learning-0.9.3/openedx_learning/core/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.940154 openedx_learning-0.9.3/openedx_learning/core/components/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/migrations/0002_alter_componentversioncontent_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/components/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.940154 openedx_learning-0.9.3/openedx_learning/core/contents/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/contents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/contents/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/contents/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/contents/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.940154 openedx_learning-0.9.3/openedx_learning/core/contents/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/contents/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/contents/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15143 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/contents/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.940154 openedx_learning-0.9.3/openedx_learning/core/publishing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14254 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.940154 openedx_learning-0.9.3/openedx_learning/core/publishing/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/migrations/0002_alter_learningpackage_key_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13412 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/model_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20321 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/core/publishing/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.944154 openedx_learning-0.9.3/openedx_learning/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/collations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/lib/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.944154 openedx_learning-0.9.3/openedx_learning/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/rest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/rest_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/rest_api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.944154 openedx_learning-0.9.3/openedx_learning/rest_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/rest_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/rest_api/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_learning/rest_api/v1/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/openedx_learning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-08 19:16:13.000000 openedx_learning-0.9.3/openedx_learning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-08 19:16:13.000000 openedx_learning-0.9.3/openedx_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:16:13.000000 openedx_learning-0.9.3/openedx_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:16:13.000000 openedx_learning-0.9.3/openedx_learning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 19:16:13.000000 openedx_learning-0.9.3/openedx_learning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 19:16:13.000000 openedx_learning-0.9.3/openedx_learning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.944154 openedx_learning-0.9.3/openedx_tagging/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.944154 openedx_learning-0.9.3/openedx_tagging/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.944154 openedx_learning-0.9.3/openedx_tagging/core/tagging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.948154 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/import_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/template.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0001_squashed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0002_auto_20230718_2026.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0003_auto_20230721_1238.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0004_auto_20230723_2001.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0005_language_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0006_alter_objecttag_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0006_auto_20230802_1631.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0007_tag_import_task_log_null_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0008_taxonomy_description_not_null.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0009_alter_objecttag_object_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0010_cleanups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0011_remove_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0012_language_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0013_tag_parent_blank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0014_minor_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0015_taxonomy_export_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0016_object_tag_export_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0017_alter_tagimporttask_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/openedx_tagging/core/tagging/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39335 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/models/import_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9062 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/models/system_defined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/paginators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13749 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35581 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/views_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/core/tagging/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/openedx_tagging/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-08 19:16:13.952154 openedx_learning-0.9.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2930 2024-05-08 19:16:10.000000 openedx_learning-0.9.3/setup.py
```

### Comparing `openedx_learning-0.9.2/CHANGELOG.rst` & `openedx_learning-0.9.3/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/LICENSE.txt` & `openedx_learning-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/PKG-INFO` & `openedx_learning-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-learning
-Version: 0.9.2
+Version: 0.9.3
 Summary: An experiment.
 Home-page: https://github.com/openedx/openedx-learning
 Author: David Ormsbee
 Author-email: dave@tcril.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -15,20 +15,20 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE.txt
-Requires-Dist: celery
-Requires-Dist: rules<4.0
-Requires-Dist: attrs
 Requires-Dist: djangorestframework<4.0
-Requires-Dist: edx-drf-extensions
 Requires-Dist: Django<5.0
+Requires-Dist: edx-drf-extensions
+Requires-Dist: attrs
+Requires-Dist: celery
+Requires-Dist: rules<4.0
 
 openedx-learning
 =============================
 
 |pypi-badge| |ci-badge| |codecov-badge| |doc-badge| |pyversions-badge|
 |license-badge|
```

### Comparing `openedx_learning-0.9.2/README.rst` & `openedx_learning-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/contrib/media_server/apps.py` & `openedx_learning-0.9.3/openedx_learning/contrib/media_server/apps.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/contrib/media_server/views.py` & `openedx_learning-0.9.3/openedx_learning/contrib/media_server/views.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/components/admin.py` & `openedx_learning-0.9.3/openedx_learning/core/components/admin.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/components/api.py` & `openedx_learning-0.9.3/openedx_learning/core/components/api.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/components/apps.py` & `openedx_learning-0.9.3/openedx_learning/core/components/apps.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/components/migrations/0001_initial.py` & `openedx_learning-0.9.3/openedx_learning/core/components/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/components/migrations/0002_alter_componentversioncontent_key.py` & `openedx_learning-0.9.3/openedx_learning/core/components/migrations/0002_alter_componentversioncontent_key.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/components/models.py` & `openedx_learning-0.9.3/openedx_learning/core/components/models.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/contents/admin.py` & `openedx_learning-0.9.3/openedx_learning/core/contents/admin.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/contents/api.py` & `openedx_learning-0.9.3/openedx_learning/core/contents/api.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/contents/migrations/0001_initial.py` & `openedx_learning-0.9.3/openedx_learning/core/contents/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/contents/models.py` & `openedx_learning-0.9.3/openedx_learning/core/contents/models.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/publishing/admin.py` & `openedx_learning-0.9.3/openedx_learning/core/publishing/admin.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/publishing/api.py` & `openedx_learning-0.9.3/openedx_learning/core/publishing/api.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/publishing/migrations/0001_initial.py` & `openedx_learning-0.9.3/openedx_learning/core/publishing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/publishing/migrations/0002_alter_learningpackage_key_and_more.py` & `openedx_learning-0.9.3/openedx_learning/core/publishing/migrations/0002_alter_learningpackage_key_and_more.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/publishing/model_mixins.py` & `openedx_learning-0.9.3/openedx_learning/core/publishing/model_mixins.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/core/publishing/models.py` & `openedx_learning-0.9.3/openedx_learning/core/publishing/models.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/lib/admin_utils.py` & `openedx_learning-0.9.3/openedx_learning/lib/admin_utils.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/lib/cache.py` & `openedx_learning-0.9.3/openedx_learning/lib/cache.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/lib/collations.py` & `openedx_learning-0.9.3/openedx_learning/lib/collations.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/lib/fields.py` & `openedx_learning-0.9.3/openedx_learning/lib/fields.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/lib/managers.py` & `openedx_learning-0.9.3/openedx_learning/lib/managers.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/lib/test_utils.py` & `openedx_learning-0.9.3/openedx_learning/lib/test_utils.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning/rest_api/v1/components.py` & `openedx_learning-0.9.3/openedx_learning/rest_api/v1/components.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_learning.egg-info/PKG-INFO` & `openedx_learning-0.9.3/openedx_learning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-learning
-Version: 0.9.2
+Version: 0.9.3
 Summary: An experiment.
 Home-page: https://github.com/openedx/openedx-learning
 Author: David Ormsbee
 Author-email: dave@tcril.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -15,20 +15,20 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE.txt
-Requires-Dist: celery
-Requires-Dist: rules<4.0
-Requires-Dist: attrs
 Requires-Dist: djangorestframework<4.0
-Requires-Dist: edx-drf-extensions
 Requires-Dist: Django<5.0
+Requires-Dist: edx-drf-extensions
+Requires-Dist: attrs
+Requires-Dist: celery
+Requires-Dist: rules<4.0
 
 openedx-learning
 =============================
 
 |pypi-badge| |ci-badge| |codecov-badge| |doc-badge| |pyversions-badge|
 |license-badge|
```

### Comparing `openedx_learning-0.9.2/openedx_learning.egg-info/SOURCES.txt` & `openedx_learning-0.9.3/openedx_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/admin.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/admin.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/api.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/api.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/data.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/data.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/actions.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/actions.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/api.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/api.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/exceptions.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/import_plan.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/import_plan.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/parsers.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/parsers.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/tasks.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/tasks.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/template.csv` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/template.csv`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/import_export/template.json` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/import_export/template.json`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0001_initial.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0001_squashed.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0001_squashed.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0002_auto_20230718_2026.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0002_auto_20230718_2026.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0003_auto_20230721_1238.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0003_auto_20230721_1238.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0004_auto_20230723_2001.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0004_auto_20230723_2001.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0005_language_taxonomy.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0005_language_taxonomy.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0006_auto_20230802_1631.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0006_auto_20230802_1631.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0008_taxonomy_description_not_null.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0008_taxonomy_description_not_null.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0009_alter_objecttag_object_id.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0009_alter_objecttag_object_id.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0010_cleanups.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0010_cleanups.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0011_remove_required.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0011_remove_required.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0012_language_taxonomy.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0012_language_taxonomy.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0013_tag_parent_blank.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0013_tag_parent_blank.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0014_minor_fixes.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0014_minor_fixes.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0015_taxonomy_export_id.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0015_taxonomy_export_id.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0016_object_tag_export_id.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0016_object_tag_export_id.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/migrations/0017_alter_tagimporttask_status.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/migrations/0017_alter_tagimporttask_status.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/models/base.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/models/base.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/models/import_export.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/models/import_export.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/models/system_defined.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/models/system_defined.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/models/utils.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/models/utils.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/paginators.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/paginators.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/utils.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/utils.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/v1/permissions.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/permissions.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/v1/serializers.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,22 @@
     """
 
     class Meta:
         model = ObjectTag
         fields = ["value", "lineage", "can_delete_objecttag"]
 
     lineage = serializers.ListField(child=serializers.CharField(), source="get_lineage", read_only=True)
-    can_delete_objecttag = serializers.SerializerMethodField(method_name='get_can_delete')
+    can_delete_objecttag = serializers.SerializerMethodField()
+
+    def get_can_delete_objecttag(self, instance) -> bool | None:
+        """
+        Returns True if the current request user may delete object tags on this taxonomy
+        """
+        perm_name = f'{self.app_label}.remove_objecttag_objectid'
+        return self._can(perm_name, instance.object_id)
 
 
 class ObjectTagSerializer(ObjectTagMinimalSerializer):
     """
     Serializer for the ObjectTag model.
     """
     class Meta:
```

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/v1/urls.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/v1/views.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/views.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/rest_api/v1/views_import.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/rest_api/v1/views_import.py`

 * *Files identical despite different names*

### Comparing `openedx_learning-0.9.2/openedx_tagging/core/tagging/rules.py` & `openedx_learning-0.9.3/openedx_tagging/core/tagging/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,24 @@
 
     This rule should be defined in other apps for proper permission checking.
     """
     return False
 
 
 @rules.predicate
+def can_remove_object_tag_objectid(_user: UserType, _object_id: str) -> bool:
+    """
+    Nobody can remove object tags without checking the permission for the tagged object.
+
+    This rule could be defined in other apps for proper permission checking.
+    """
+    return can_change_object_tag_objectid(_user, _object_id)
+
+
+@rules.predicate
 def can_change_object_tag(
     user: UserType, perm_obj: ObjectTagPermissionItem | None = None
 ) -> bool:
     """
     Checks if the user has permissions to create or modify tags on the given taxonomy and object_id.
     """
 
@@ -190,7 +200,8 @@
 rules.add_perm("oel_tagging.can_tag_object", can_change_object_tag)
 
 # Users can tag objects using tags from any taxonomy that they have permission to view
 rules.add_perm("oel_tagging.view_objecttag_objectid", can_view_object_tag_objectid)
 rules.add_perm("oel_tagging.view_objecttag_taxonomy", can_view_object_tag_taxonomy)
 rules.add_perm("oel_tagging.change_objecttag_taxonomy", can_view_object_tag_taxonomy)
 rules.add_perm("oel_tagging.change_objecttag_objectid", can_change_object_tag_objectid)
+rules.add_perm("oel_tagging.remove_objecttag_objectid", can_remove_object_tag_objectid)
```

### Comparing `openedx_learning-0.9.2/setup.py` & `openedx_learning-0.9.3/setup.py`

 * *Files identical despite different names*

