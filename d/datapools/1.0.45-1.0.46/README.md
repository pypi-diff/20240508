# Comparing `tmp/datapools-1.0.45.tar.gz` & `tmp/datapools-1.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.45.tar", last modified: Thu Apr 25 14:37:49 2024, max compression
+gzip compressed data, was "datapools-1.0.46.tar", last modified: Wed May  8 15:41:37 2024, max compression
```

## Comparing `datapools-1.0.45.tar` & `datapools-1.0.46.tar`

### file list

```diff
@@ -1,88 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.354473 datapools-1.0.45/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-25 14:37:36.000000 datapools-1.0.45/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    16729 2024-04-25 14:37:36.000000 datapools-1.0.45/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-25 14:37:36.000000 datapools-1.0.45/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-25 14:37:36.000000 datapools-1.0.45/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-25 14:37:49.350473 datapools-1.0.45/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-25 14:37:36.000000 datapools-1.0.45/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.338473 datapools-1.0.45/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.342473 datapools-1.0.45/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.342473 datapools-1.0.45/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.342473 datapools-1.0.45/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.342473 datapools-1.0.45/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12221 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.350473 datapools-1.0.45/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.350473 datapools-1.0.45/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.350473 datapools-1.0.45/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16774 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.350473 datapools-1.0.45/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-25 14:37:49.000000 datapools-1.0.45/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-25 14:37:49.000000 datapools-1.0.45/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:37:49.000000 datapools-1.0.45/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 14:37:49.000000 datapools-1.0.45/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-25 14:37:49.000000 datapools-1.0.45/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 14:37:49.000000 datapools-1.0.45/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 14:37:49.354473 datapools-1.0.45/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-25 14:37:36.000000 datapools-1.0.45/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.350473 datapools-1.0.45/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:36.000000 datapools-1.0.45/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-25 14:37:36.000000 datapools-1.0.45/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-25 14:37:36.000000 datapools-1.0.45/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.172133 datapools-1.0.46/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 15:41:28.000000 datapools-1.0.46/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    16945 2024-05-08 15:41:28.000000 datapools-1.0.46/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-08 15:41:28.000000 datapools-1.0.46/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-08 15:41:28.000000 datapools-1.0.46/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-08 15:41:37.172133 datapools-1.0.46/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-08 15:41:28.000000 datapools-1.0.46/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.152133 datapools-1.0.46/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.156133 datapools-1.0.46/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/freesound_org/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/freesound_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/freesound_org/freesound_org.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-08 15:41:28.000000 datapools-1.0.46/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-08 15:41:37.000000 datapools-1.0.46/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-08 15:41:37.000000 datapools-1.0.46/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:41:37.000000 datapools-1.0.46/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 15:41:37.000000 datapools-1.0.46/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-08 15:41:37.000000 datapools-1.0.46/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 15:41:37.000000 datapools-1.0.46/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:41:37.172133 datapools-1.0.46/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-08 15:41:28.000000 datapools-1.0.46/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:37.168133 datapools-1.0.46/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:41:28.000000 datapools-1.0.46/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-08 15:41:28.000000 datapools-1.0.46/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-08 15:41:28.000000 datapools-1.0.46/tests/test_base.py
```

### Comparing `datapools-1.0.45/HISTORY.md` & `datapools-1.0.46/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Merge pull request #64 from torrentsai/sergpsu-fixes. [S]
+
+  Freesound.org
+- Env keys. [sergpsu]
+- Freesound.org plugin. [sergpsu]
+
+
+1.0.45 (2024-04-25)
+-------------------
+- Release: version 1.0.45 🚀 [sergpsu]
 - Merge pull request #63 from torrentsai/sergpsu-fixes. [S]
 
   Keepout tags implemented
 - Types requests. [sergpsu]
 - Mypy --install-types. [sergpsu]
 - Keepout tags and tests. [sergpsu]
 - Backend exception processing. [sergpsu]
```

### Comparing `datapools-1.0.45/LICENSE` & `datapools-1.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/PKG-INFO` & `datapools-1.0.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.45
+Version: 1.0.46
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.45/README.md` & `datapools-1.0.46/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/api.py` & `datapools-1.0.46/datapools/api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/cli.py` & `datapools-1.0.46/datapools/cli.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/common/backend_api.py` & `datapools-1.0.46/datapools/common/backend_api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/common/queues/__init__.py` & `datapools-1.0.46/datapools/common/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/common/queues/rabbitmq.py` & `datapools-1.0.46/datapools/common/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/common/queues/types.py` & `datapools-1.0.46/datapools/common/queues/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/common/session_manager.py` & `datapools-1.0.46/datapools/common/session_manager.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/common/stoppable.py` & `datapools-1.0.46/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/common/storage/base_storage.py` & `datapools-1.0.46/datapools/common/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/common/storage/file_storage.py` & `datapools-1.0.46/datapools/common/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.46/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.46/datapools/common/tasks_db/tasks_db.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/common/types.py` & `datapools-1.0.46/datapools/common/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from .storage import FileStorage
 
 DEFAULT_QUEUE_WORKER_TASKS = "worker_tasks"
 DEFAULT_QUEUE_REPORTS = "worker_reports"
 DEFAULT_QUEUE_EVAL_TASKS = "eval_tasks"
 DEFAULT_QUEUE_TOPICS = "topics"
 
-DEFAULT_RABBITMQ_HOST = "rabbitmq.crawler"
+DEFAULT_RABBITMQ_HOST = "rabbitmq.openlicense"
 DEFAULT_RABBITMQ_PORT: int = 5672
-DEFAULT_REDIS_HOST = "redis.crawler"
+DEFAULT_REDIS_HOST = "redis.openlicense"
 DEFAULT_REDIS_PORT: int = 6379
 
 DEFAULT_CONNECTION_URL: str = "amqp://guest:guest@{host}:{port}/".format(
     host=DEFAULT_RABBITMQ_HOST, port=DEFAULT_RABBITMQ_PORT
 )
 
 DEFAULT_BACKEND_API_URL: str = "https://openlicense.ai/internal/"
@@ -251,14 +251,15 @@
     copyright_tag_id: Optional[str] = None
     copyright_tag_keepout: Optional[bool] = False
     platform_tag_id: Optional[str] = None
     platform_tag_keepout: Optional[bool] = False
     type: DatapoolContentType
     storage_id: Any
     url: Union[str, AnyUrl]
+    priority_timestamp: Optional[int] = None
 
     def to_dict(self):
         res = self.__dict__
         res["type"] = res["type"].value
         return res
```

### Comparing `datapools-1.0.45/datapools/producer/base_producer.py` & `datapools-1.0.46/datapools/producer/base_producer.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/scheduler/scheduler.py` & `datapools-1.0.46/datapools/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.46/datapools/worker/plugins/base_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,27 +134,28 @@
             async with httpx.AsyncClient(max_redirects=max_redirects) as client:
                 r = await client.get(url, follow_redirects=follow_redirects, headers=headers)
                 return r.content
 
         except Exception as e:
             logger.error(f"failed get content of {url}: {e}")
 
-    async def download_content(self, url, type: DatapoolContentType):
+    async def download_content(self, url, content_type: DatapoolContentType):
         storage_id = BaseStorage.gen_id(url)
 
-        content = await self.download(url)
-        if content:
-            logger.info(f"putting to {storage_id=}")
-            await self.ctx.storage.put(storage_id, content)
-
-            return CrawlerContent(
-                type=type,
-                storage_id=storage_id,
-                url=url,
-            )
+        if not await self.is_content_processed(url):
+            content = await self.download(url)
+            if content:
+                logger.info(f"putting to {storage_id=}")
+                await self.ctx.storage.put(storage_id, content)
+
+                return CrawlerContent(
+                    type=content_type,
+                    storage_id=storage_id,
+                    url=url,
+                )
         return CrawlerNop()
 
     @staticmethod
     def parse_url(url):
         return urlparse(url)
 
     @staticmethod
@@ -170,15 +171,14 @@
         s2 = dom2.split(".")
         return s1[-len(s2) : :] == s2
 
     @staticmethod
     def get_local_url(href, page_url):
         pc = urlparse(page_url)
         p = urlparse(href)
-        # print(p)
         if p.netloc == "" or BasePlugin.is_same_or_subdomain(p.netloc, pc.netloc):
             return urljoin(page_url, href)
         return False
 
     @staticmethod
     def merge_head_tail(head, tail):
         # returns intersection length
```

### Comparing `datapools-1.0.45/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.46/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/worker/plugins/default/default.py` & `datapools-1.0.46/datapools/worker/plugins/default/default.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.46/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.46/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,43 @@
-# import os
+import os
+
 # import asyncio
 # import io
 import traceback
+from typing import Optional
 
 from google.auth.api_key import Credentials
 
 # from google.auth.transport.requests import Request
 # from google.oauth2.credentials import Credentials
 # from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 
 from ....common.logger import logger
 from ....common.storage import BaseStorage
 from ....common.types import CrawlerContent, DatapoolContentType
-from ..base_plugin import BasePlugin, BasePluginException, WorkerTask
+from ..base_plugin import BasePlugin, BasePluginException, WorkerTask, BaseTag
 
 # from googleapiclient.http import MediaIoBaseDownload
 
 
 # from googleapiclient.errors import HttpError
 
 
 # If modifying these scopes, delete the file token.json.
 # SCOPES = ['https://www.googleapis.com/auth/drive.metadata.readonly']
 
 
 class GoogleDrivePlugin(BasePlugin):
-    def __init__(self, ctx, api_key):
+    tag_id: Optional[BaseTag] = None
+
+    def __init__(self, ctx, api_key=None):
         super().__init__(ctx)
+        if not api_key:
+            api_key = os.environ.get("GOOGLE_DRIVE_API_KEY")
         self.creds = Credentials(api_key)
 
     # https://drive.google.com/drive/folders/1CPDmula2V83KWOocJR9jVvsTk6tVSpKd?usp=sharing
 
     @staticmethod
     def is_supported(url):
         u = BasePlugin.parse_url(url)
```

### Comparing `datapools-1.0.45/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.46/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,26 +28,14 @@
         u = BasePlugin.parse_url(url)
         # logger.info( f'imageshack {u=}')
         return u.netloc == DOMAIN
 
     async def process(self, task: WorkerTask):
         logger.info(f"imageshack::process({task.url})")
 
-        if task.content_type == DatapoolContentType.Image:
-            logger.info("Got content_type => direct download")
-            yield await self.download_content(task.url, task.content_type)
-            return
-
-        logger.info(f"loading url {task.url}")
-        r = await self.download(task.url)
-        if r is None:
-            return
-        # logger.info( f'text: {r}')
-        logger.info(f"got url content length={len(r)}")
-
         async with async_playwright() as playwright:
             webkit = playwright.chromium
             browser = await webkit.launch()
             viewport_height = 1024
             context = await browser.new_context(viewport={"width": 1920, "height": viewport_height})
 
             page = await context.new_page()
@@ -79,17 +67,15 @@
 
                         full_local_url = BasePlugin.get_local_url(href, session_meta["url"])
                         if full_local_url:
                             # strict constraint on urls, else may get endless recursions etc
                             full_local_url = canonicalize_url(full_local_url)
                             logger.info(f"adding task: {full_local_url}")
 
-                            # logger.info( f'---------yielding {video_url=}')
                             yield CrawlerBackTask(url=full_local_url)
-                            # logger.info( f'---------yielded {video_url=}')
                         else:
                             logger.info(f'non local: {href=} {session_meta["url"]=}')
 
                     except PlaywriteTimeoutError as e:
                         # element may be not ready yet, no problems, will get it on the next iteration
                         # logger.info( 'get_attribute timeout' )
                         expect_changes = True
```

### Comparing `datapools-1.0.45/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.46/datapools/worker/plugins/s3/s3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# import asyncio
+import os
 import tempfile
 import traceback
 
 import boto3
 import filetype
 from botocore import UNSIGNED
 from botocore.client import Config
@@ -20,14 +20,20 @@
     pass
 
 
 class S3Plugin(BasePlugin):
     def __init__(self, ctx, aws_access_key_id=None, aws_secret_access_key=None):
         super().__init__(ctx)
 
+        if aws_access_key_id is None:
+            logger.info("getting aws_access_key_id from env")
+            aws_access_key_id = os.environ.get("AWS_ACCESS_KEY_ID")
+        if aws_secret_access_key is None:
+            logger.info("getting aws_secret_access_key from env")
+            aws_secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY")
         logger.info(f"{aws_access_key_id=}")
         logger.info(f"{aws_secret_access_key=}")
 
         # empty key means bucket is public
         if aws_access_key_id == "":
             self.is_public_bucket = True
             self.s3_client = boto3.client("s3", config=Config(signature_version=UNSIGNED))
```

### Comparing `datapools-1.0.45/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.46/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.46/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.46/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.46/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/datapools/worker/worker.py` & `datapools-1.0.46/datapools/worker/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
 
                         if deleted_or_stopped(qm.session_id):
                             break
 
                         if t is CrawlerContent:
                             session.inc_crawled_content()
 
-                            # notifying datapool pipeline about new crawled data
+                            # notifying producer about new crawled data
                             await self.producer_queue.push(
                                 QueueMessage(
                                     qm.session_id,
                                     QueueMessageType.Task,
                                     {
                                         "parent_url": task.url,
                                         "url": content_or_task.url,
@@ -269,14 +269,15 @@
                                         "tag_id": content_or_task.tag_id,
                                         "tag_keepout": content_or_task.tag_keepout,
                                         "copyright_tag_id": content_or_task.copyright_tag_id,
                                         "copyright_tag_keepout": content_or_task.copyright_tag_keepout,
                                         "platform_tag_id": content_or_task.platform_tag_id,
                                         "platform_tag_keepout": content_or_task.platform_tag_keepout,
                                         "type": DatapoolContentType(content_or_task.type).value,
+                                        "priority_timestamp": content_or_task.priority_timestamp,
                                         "worker_id": self.id,
                                     },
                                 )
                             )
 
                         elif t is CrawlerBackTask:
                             await self._add_back_task(qm.session_id, content_or_task)
```

### Comparing `datapools-1.0.45/datapools.egg-info/PKG-INFO` & `datapools-1.0.46/datapools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.45
+Version: 1.0.46
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.45/datapools.egg-info/SOURCES.txt` & `datapools-1.0.46/datapools.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 datapools/worker/plugins/base_plugin.py
 datapools/worker/plugins/dataphoenix_info/__init__.py
 datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
 datapools/worker/plugins/default/__init__.py
 datapools/worker/plugins/default/default.py
 datapools/worker/plugins/deutsche_welle/__init__.py
 datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+datapools/worker/plugins/freesound_org/__init__.py
+datapools/worker/plugins/freesound_org/freesound_org.py
 datapools/worker/plugins/google_drive/__init__.py
 datapools/worker/plugins/google_drive/google_drive.py
 datapools/worker/plugins/imageshack/__init__.py
 datapools/worker/plugins/imageshack/imageshack.py
 datapools/worker/plugins/s3/__init__.py
 datapools/worker/plugins/s3/s3.py
 datapools/worker/plugins/theguardian/__init__.py
```

### Comparing `datapools-1.0.45/setup.py` & `datapools-1.0.46/setup.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.45/tests/test_base.py` & `datapools-1.0.46/tests/test_base.py`

 * *Files identical despite different names*

