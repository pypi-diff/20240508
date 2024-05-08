# Comparing `tmp/minvectordb-0.3.2.tar.gz` & `tmp/minvectordb-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minvectordb-0.3.2.tar", last modified: Fri Apr 26 10:55:19 2024, max compression
+gzip compressed data, was "minvectordb-0.3.3.tar", last modified: Wed May  8 09:42:04 2024, max compression
```

## Comparing `minvectordb-0.3.2.tar` & `minvectordb-0.3.3.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.385584 minvectordb-0.3.2/
--rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 minvectordb-0.3.2/LICENSE
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.384998 minvectordb-0.3.2/MinVectorDB.egg-info/
--rw-r--r--   0 guobingming   (501) staff       (20)    12327 2024-04-26 10:55:19.000000 minvectordb-0.3.2/MinVectorDB.egg-info/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)     1470 2024-04-26 10:55:19.000000 minvectordb-0.3.2/MinVectorDB.egg-info/SOURCES.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-04-26 10:55:19.000000 minvectordb-0.3.2/MinVectorDB.egg-info/dependency_links.txt
--rw-r--r--   0 guobingming   (501) staff       (20)       54 2024-04-26 10:55:19.000000 minvectordb-0.3.2/MinVectorDB.egg-info/entry_points.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 minvectordb-0.3.2/MinVectorDB.egg-info/not-zip-safe
--rw-r--r--   0 guobingming   (501) staff       (20)      240 2024-04-26 10:55:19.000000 minvectordb-0.3.2/MinVectorDB.egg-info/requires.txt
--rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-04-26 10:55:19.000000 minvectordb-0.3.2/MinVectorDB.egg-info/top_level.txt
--rw-r--r--   0 guobingming   (501) staff       (20)    12327 2024-04-26 10:55:19.385294 minvectordb-0.3.2/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)    10961 2024-04-26 10:54:39.000000 minvectordb-0.3.2/README.md
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.376425 minvectordb-0.3.2/min_vec/
--rw-r--r--   0 guobingming   (501) staff       (20)     1100 2024-04-26 10:04:57.000000 minvectordb-0.3.2/min_vec/__init__.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.377261 minvectordb-0.3.2/min_vec/api/
--rw-r--r--   0 guobingming   (501) staff       (20)      273 2024-04-23 05:39:11.000000 minvectordb-0.3.2/min_vec/api/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    24476 2024-04-26 09:16:06.000000 minvectordb-0.3.2/min_vec/api/client_api.py
--rw-r--r--   0 guobingming   (501) staff       (20)    11043 2024-04-26 09:49:47.000000 minvectordb-0.3.2/min_vec/api/high_level.py
--rw-r--r--   0 guobingming   (501) staff       (20)    35323 2024-04-26 10:25:25.000000 minvectordb-0.3.2/min_vec/api/http_api.py
--rw-r--r--   0 guobingming   (501) staff       (20)    15062 2024-04-26 07:41:58.000000 minvectordb-0.3.2/min_vec/api/low_level.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.377553 minvectordb-0.3.2/min_vec/computational_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:06:12.000000 minvectordb-0.3.2/min_vec/computational_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)      890 2024-04-17 08:04:09.000000 minvectordb-0.3.2/min_vec/computational_layer/engines.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.378231 minvectordb-0.3.2/min_vec/configs/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:24.000000 minvectordb-0.3.2/min_vec/configs/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2553 2024-04-23 13:22:47.000000 minvectordb-0.3.2/min_vec/configs/config.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3624 2024-04-25 06:47:17.000000 minvectordb-0.3.2/min_vec/configs/parameters_validator.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.379612 minvectordb-0.3.2/min_vec/execution_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:09:45.000000 minvectordb-0.3.2/min_vec/execution_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2710 2024-04-26 08:20:20.000000 minvectordb-0.3.2/min_vec/execution_layer/cluster_worker.py
--rw-r--r--   0 guobingming   (501) staff       (20)    19573 2024-04-26 08:44:04.000000 minvectordb-0.3.2/min_vec/execution_layer/matrix_serializer.py
--rw-r--r--   0 guobingming   (501) staff       (20)     8031 2024-04-26 08:19:12.000000 minvectordb-0.3.2/min_vec/execution_layer/query.py
--rw-r--r--   0 guobingming   (501) staff       (20)      409 2024-04-26 02:40:02.000000 minvectordb-0.3.2/min_vec/execution_layer/session.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.380030 minvectordb-0.3.2/min_vec/storage_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:04:15.000000 minvectordb-0.3.2/min_vec/storage_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    15749 2024-04-26 07:59:35.000000 minvectordb-0.3.2/min_vec/storage_layer/storage.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.382139 minvectordb-0.3.2/min_vec/structures/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:07:22.000000 minvectordb-0.3.2/min_vec/structures/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)      677 2024-04-26 06:44:38.000000 minvectordb-0.3.2/min_vec/structures/counter.py
--rw-r--r--   0 guobingming   (501) staff       (20)     6280 2024-04-26 05:45:48.000000 minvectordb-0.3.2/min_vec/structures/fields_filter.py
--rw-r--r--   0 guobingming   (501) staff       (20)     5448 2024-04-24 23:46:29.000000 minvectordb-0.3.2/min_vec/structures/filter.py
--rw-r--r--   0 guobingming   (501) staff       (20)      866 2024-04-26 05:45:48.000000 minvectordb-0.3.2/min_vec/structures/id_checker.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1642 2024-04-26 08:20:02.000000 minvectordb-0.3.2/min_vec/structures/kmeans.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1449 2024-04-18 02:30:25.000000 minvectordb-0.3.2/min_vec/structures/limited_dict.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3258 2024-04-26 07:02:33.000000 minvectordb-0.3.2/min_vec/structures/limited_sort.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3864 2024-04-25 06:47:17.000000 minvectordb-0.3.2/min_vec/structures/scaler.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.382554 minvectordb-0.3.2/min_vec/utils/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:09.000000 minvectordb-0.3.2/min_vec/utils/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     4021 2024-04-25 06:40:13.000000 minvectordb-0.3.2/min_vec/utils/utils.py
--rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-04-26 10:55:19.385627 minvectordb-0.3.2/setup.cfg
--rw-r--r--   0 guobingming   (501) staff       (20)     1485 2024-04-26 10:28:05.000000 minvectordb-0.3.2/setup.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.382895 minvectordb-0.3.2/test/
--rw-r--r--   0 guobingming   (501) staff       (20)      310 2024-04-25 11:00:27.000000 minvectordb-0.3.2/test/__init__.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.383106 minvectordb-0.3.2/test/docker_tests/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-04-26 03:04:25.000000 minvectordb-0.3.2/test/docker_tests/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3057 2024-04-26 04:00:27.000000 minvectordb-0.3.2/test/docker_tests/test_docker_api.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-26 10:55:19.384440 minvectordb-0.3.2/test/standard_tests/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-04-26 03:03:57.000000 minvectordb-0.3.2/test/standard_tests/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1601 2024-04-24 13:16:55.000000 minvectordb-0.3.2/test/standard_tests/test_hmvdb_initial.py
--rw-r--r--   0 guobingming   (501) staff       (20)     6019 2024-04-26 03:51:59.000000 minvectordb-0.3.2/test/standard_tests/test_http_api.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1591 2024-04-23 10:40:50.000000 minvectordb-0.3.2/test/standard_tests/test_smvdb_initial.py
--rw-r--r--   0 guobingming   (501) staff       (20)    14141 2024-04-26 08:24:07.000000 minvectordb-0.3.2/test/standard_tests/test_smvdb_save_and_query.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-08 09:42:04.259140 minvectordb-0.3.3/
+-rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 minvectordb-0.3.3/LICENSE
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-08 09:42:04.258381 minvectordb-0.3.3/MinVectorDB.egg-info/
+-rw-r--r--   0 guobingming   (501) staff       (20)    12501 2024-05-08 09:42:04.000000 minvectordb-0.3.3/MinVectorDB.egg-info/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)     1632 2024-05-08 09:42:04.000000 minvectordb-0.3.3/MinVectorDB.egg-info/SOURCES.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-05-08 09:42:04.000000 minvectordb-0.3.3/MinVectorDB.egg-info/dependency_links.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)       54 2024-05-08 09:42:04.000000 minvectordb-0.3.3/MinVectorDB.egg-info/entry_points.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 minvectordb-0.3.3/MinVectorDB.egg-info/not-zip-safe
+-rw-r--r--   0 guobingming   (501) staff       (20)      257 2024-05-08 09:42:04.000000 minvectordb-0.3.3/MinVectorDB.egg-info/requires.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-05-08 09:42:04.000000 minvectordb-0.3.3/MinVectorDB.egg-info/top_level.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)    12501 2024-05-08 09:42:04.258776 minvectordb-0.3.3/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)    11103 2024-05-08 09:13:09.000000 minvectordb-0.3.3/README.md
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-08 09:42:04.237994 minvectordb-0.3.3/min_vec/
+-rw-r--r--   0 guobingming   (501) staff       (20)     1100 2024-04-29 06:35:19.000000 minvectordb-0.3.3/min_vec/__init__.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-08 09:42:04.240590 minvectordb-0.3.3/min_vec/api/
+-rw-r--r--   0 guobingming   (501) staff       (20)      273 2024-04-23 05:39:11.000000 minvectordb-0.3.3/min_vec/api/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    29402 2024-05-04 07:05:03.000000 minvectordb-0.3.3/min_vec/api/client_api.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    10758 2024-05-04 13:08:15.000000 minvectordb-0.3.3/min_vec/api/high_level.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    22498 2024-05-06 10:35:49.000000 minvectordb-0.3.3/min_vec/api/http_api.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    14874 2024-05-08 06:54:12.000000 minvectordb-0.3.3/min_vec/api/low_level.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-08 09:42:04.241058 minvectordb-0.3.3/min_vec/computational_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:06:12.000000 minvectordb-0.3.3/min_vec/computational_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      890 2024-04-17 08:04:09.000000 minvectordb-0.3.3/min_vec/computational_layer/engines.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-08 09:42:04.241958 minvectordb-0.3.3/min_vec/configs/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:24.000000 minvectordb-0.3.3/min_vec/configs/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2670 2024-05-04 07:03:32.000000 minvectordb-0.3.3/min_vec/configs/config.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3548 2024-05-04 10:58:46.000000 minvectordb-0.3.3/min_vec/configs/parameters_validator.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-08 09:42:04.245264 minvectordb-0.3.3/min_vec/core_components/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:07:22.000000 minvectordb-0.3.3/min_vec/core_components/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      707 2024-05-04 11:43:20.000000 minvectordb-0.3.3/min_vec/core_components/counter.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      501 2024-05-04 11:46:53.000000 minvectordb-0.3.3/min_vec/core_components/cross_lock.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     8893 2024-05-08 06:48:31.000000 minvectordb-0.3.3/min_vec/core_components/filter.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1236 2024-05-04 10:58:46.000000 minvectordb-0.3.3/min_vec/core_components/id_checker.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1570 2024-05-04 10:58:46.000000 minvectordb-0.3.3/min_vec/core_components/kmeans.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1548 2024-05-04 11:43:20.000000 minvectordb-0.3.3/min_vec/core_components/limited_dict.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3294 2024-05-04 11:43:20.000000 minvectordb-0.3.3/min_vec/core_components/limited_sort.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    10511 2024-05-08 08:43:01.000000 minvectordb-0.3.3/min_vec/core_components/metadata_kv.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3785 2024-05-04 10:58:46.000000 minvectordb-0.3.3/min_vec/core_components/scaler.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1390 2024-05-04 11:43:20.000000 minvectordb-0.3.3/min_vec/core_components/thread_safe_list.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-08 09:42:04.247130 minvectordb-0.3.3/min_vec/execution_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:09:45.000000 minvectordb-0.3.3/min_vec/execution_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2679 2024-05-03 07:00:59.000000 minvectordb-0.3.3/min_vec/execution_layer/cluster_worker.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    20844 2024-05-08 09:01:11.000000 minvectordb-0.3.3/min_vec/execution_layer/matrix_serializer.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     6743 2024-05-08 06:53:32.000000 minvectordb-0.3.3/min_vec/execution_layer/query.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      409 2024-04-26 02:40:02.000000 minvectordb-0.3.3/min_vec/execution_layer/session.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-08 09:42:04.247604 minvectordb-0.3.3/min_vec/storage_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:04:15.000000 minvectordb-0.3.3/min_vec/storage_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    18716 2024-05-04 11:43:20.000000 minvectordb-0.3.3/min_vec/storage_layer/storage.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-08 09:42:04.248301 minvectordb-0.3.3/min_vec/utils/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:09.000000 minvectordb-0.3.3/min_vec/utils/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     4022 2024-05-03 07:43:27.000000 minvectordb-0.3.3/min_vec/utils/utils.py
+-rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-05-08 09:42:04.259209 minvectordb-0.3.3/setup.cfg
+-rw-r--r--   0 guobingming   (501) staff       (20)     1485 2024-04-29 06:35:19.000000 minvectordb-0.3.3/setup.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-08 09:42:04.248553 minvectordb-0.3.3/test/
+-rw-r--r--   0 guobingming   (501) staff       (20)      315 2024-05-03 07:00:59.000000 minvectordb-0.3.3/test/__init__.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-08 09:42:04.249301 minvectordb-0.3.3/test/docker_tests/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-04-26 03:04:25.000000 minvectordb-0.3.3/test/docker_tests/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3038 2024-05-03 13:31:22.000000 minvectordb-0.3.3/test/docker_tests/test_client_api.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3029 2024-05-08 06:55:47.000000 minvectordb-0.3.3/test/docker_tests/test_docker_api.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-05-08 09:42:04.257782 minvectordb-0.3.3/test/standard_tests/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-04-26 03:03:57.000000 minvectordb-0.3.3/test/standard_tests/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1601 2024-04-24 13:16:55.000000 minvectordb-0.3.3/test/standard_tests/test_hmvdb_initial.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     7588 2024-05-08 06:48:31.000000 minvectordb-0.3.3/test/standard_tests/test_http_api.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1591 2024-04-23 10:40:50.000000 minvectordb-0.3.3/test/standard_tests/test_smvdb_initial.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    18258 2024-05-08 06:52:06.000000 minvectordb-0.3.3/test/standard_tests/test_smvdb_save_and_query.py
```

### Comparing `minvectordb-0.3.2/LICENSE` & `minvectordb-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.2/MinVectorDB.egg-info/PKG-INFO` & `minvectordb-0.3.3/MinVectorDB.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MinVectorDB
-Version: 0.3.2
+Version: 0.3.3
 Summary: A pure Python-implemented, lightweight, server-optional, multi-end compatible, vector database deployable locally or remotely.
 Home-page: https://github.com/BirchKwok/MinVectorDB
 Author: Birch Kwok
 Author-email: birchkwok@gmail.com
 Keywords: vector database
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -23,57 +23,61 @@
 Requires-Dist: spinesUtils>=0.3.13
 Requires-Dist: msgpack>=1.0.2
 Requires-Dist: scikit-learn>=1.0.0
 Requires-Dist: cloudpickle>=2.0.0
 Requires-Dist: numexpr>=2.7.3
 Requires-Dist: pyroaring>=0.4.5
 Requires-Dist: jax>=0.4.25
-Requires-Dist: numba>=0.54.0
 Requires-Dist: jaxlib>=0.4.25
 Requires-Dist: flask>=2.0.1
 Requires-Dist: PyYAML>=5.4.1
-Requires-Dist: portalocker>=2.3.0
-Requires-Dist: requests>=2.26.0
 Requires-Dist: waitress>=2.0.0
+Requires-Dist: pytest>=7.4.4
+Requires-Dist: tqdm>=4.62.3
+Requires-Dist: setuptools>=68.0.0
+Requires-Dist: httpx[http2]>=0.19.0
 
 <div align="center">
   <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB" style="max-width: 20%; height: auto;"></a>
   <h3>A pure Python-implemented, lightweight, server-optional, multi-end compatible, vector database deployable locally or remotely.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/l/MinVectorDB" alt="PyPI - License"></a>
-    <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml/badge.svg" alt="Python package"></a>
+    <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-tests.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-tests.yml/badge.svg" alt="Python testing"></a>
+    <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/docker-tests.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/docker-tests.yml/badge.svg" alt="Docker build"></a>
   </p>
 </div>
 
-⚡ **Serverless, simple parameters, simple API.**
+⚡ **Server-optional, simple parameters, simple API.**
 
 ⚡ **Fast, memory-efficient, easily scales to millions of vectors.**
 
 ⚡ **Supports cosine similarity and L2 distance, uses FLAT for exhaustive search or IVF-FLAT for inverted indexing.**
 
 ⚡ **Friendly caching technology stores recently queried vectors for accelerated access.**
 
 ⚡ **Based on a generic Python software stack, platform-independent, highly versatile.**
 
 > **WARNING**: MinVectorDB is actively being updated, and API backward compatibility is not guaranteed. You should use version numbers as a strong constraint during deployment to avoid unnecessary feature conflicts and errors.
 > **Although our goal is to enable brute force search or inverted indexing on billion-scale vectors, we currently still recommend using it on a scale of millions of vectors or less for the best experience.**
 
-*MinVectorDB* is a vector database implemented purely in Python, designed to be lightweight, serverless, and easy to deploy locally. It offers straightforward and clear Python APIs, aiming to lower the entry barrier for using vector databases. In response to user needs and to enhance its practicality, we are planning to introduce new features, including but not limited to:
+*MinVectorDB* is a vector database implemented purely in Python, designed to be lightweight, server-optional, and easy to deploy locally or remotely. It offers straightforward and clear Python APIs, aiming to lower the entry barrier for using vector databases. In response to user needs and to enhance its practicality, we are planning to introduce new features, including but not limited to:
 
 - **Optimizing Global Search Performance**: We are focusing on algorithm and data structure enhancements to speed up searches across the database, enabling faster retrieval of vector data.
 - **Enhancing Cluster Search with Inverted Indexes**: Utilizing inverted index technology, we aim to refine the cluster search process for better search efficiency and precision.
 - **Refining Clustering Algorithms**: By improving our clustering algorithms, we intend to offer more precise and efficient data clustering to support complex queries.
 - **Facilitating Vector Modifications and Deletions**: We will introduce features to modify and delete vectors, allowing for more flexible data management.
-- **Implementing Rollback Strategies**: To increase database robustness and data security, rollback strategies will be added, helping users recover from incorrect operations or system failures easily.
 
 MinVectorDB focuses on achieving 100% recall, prioritizing recall accuracy over high-speed search performance. This approach ensures that users can reliably retrieve all relevant vector data, making MinVectorDB particularly suitable for applications that require responses within hundreds of milliseconds.
 
-While the project has not yet been benchmarked against other systems, we believe these planned features will significantly enhance MinVectorDB's capabilities in managing and retrieving vector data, addressing a wide range of user needs.
+- [x] **Now supports HTTP API and Python local code API.**
+- [X] **Now supports Docker deployment.**
+- [X] **Now supports vector id and field filtering.**
+- [X] **Now supports transaction management; if a commit fails, it will automatically roll back.**
 
 ## Install Client API package (Mandatory)
 
 ```shell
 pip install MinVectorDB
 ```
 
@@ -87,58 +91,54 @@
 
 
 ```python
 import min_vec
 print("MinVectorDB version is: ", min_vec.__version__)
 ```
 
-    MinVectorDB version is:  0.3.2
+    MinVectorDB version is:  0.3.3
 
 
 ## Initialize Database
 
 MinVectorDB now supports HTTP API and Python local code API. 
 
 
 The HTTP API mode requires starting an HTTP server beforehand. You have two options: 
 - start directly.
   
   For direct startup, the default port is 7637. You can run the following command in the terminal to start the service:
 ```shell
-min_vec run --host 127.0.0.1 --port 7637
+min_vec run --host localhost --port 7637
 ```
 
 - within Docker
   
-  In Docker, the default port is 5403. You can run the following command in the terminal to start the service:
+  In Docker, You can run the following command in the terminal to start the service:
 ```shell
-docker run -p 5403:7637 birchkwok/minvectordb:latest
+docker run -p 7637:7637 birchkwok/minvectordb:latest
 ```
 
 ```python
 from min_vec import MinVectorDB
 
 # This method is for the Python local code API, recommended only for CI/CD testing or single-user local use.
 # Specify database root directory
 my_db = MinVectorDB('my_vec_db')  # Judgment condition, root_path does not start with http or https
 # or
 # Use the HTTP API mode, it is suitable for use in production environments.
-# For direct startup
-my_db = MinVectorDB("http://127.0.0.1:7637")
-
-# within Docker
-my_db = MinVectorDB("http://127.0.0.1:5403")
+my_db = MinVectorDB("http://localhost:7637")
 ```
 
 
 ```python
 from min_vec import MinVectorDB
 
 # For direct startup
-my_db = MinVectorDB("http://localhost:5403")
+my_db = MinVectorDB("http://localhost:7637")
 ```
 
 ### create a collection
 
 
 ```python
 collection = my_db.require_collection("test_collection", 4, drop_if_exists=True, scaler_bits=8)
@@ -203,15 +203,15 @@
 ```python
 print(collection.query_report_)
 ```
 
     
     * - MOST RECENT QUERY REPORT -
     | - Collection Shape: (10, 4)
-    | - Query Time: 0.20518 s
+    | - Query Time: 0.15716 s
     | - Query Distance: cosine
     | - Query K: 10
     | - Top 10 Results ID: [ 2  9  1  4  6  5 10  7  8  3]
     | - Top 10 Results Similarity: [1.         0.92355633 0.86097705 0.85727406 0.81551266 0.813797
      0.78595245 0.7741583  0.6871773  0.34695023]
     * - END OF REPORT -
     
@@ -219,72 +219,76 @@
 
 ### Use Filter
 
 
 ```python
 import operator
 
-from min_vec.structures.filter import Filter, FieldCondition, MatchField, IDCondition, MatchID
+from min_vec.core_components.filter import Filter, FieldCondition, MatchField, IDCondition, MatchID
 
 
 collection.query(
     vector=[0.36, 0.43, 0.56, 0.12], 
     k=10, 
     query_filter=Filter(
         must=[
             FieldCondition(key='field', matcher=MatchField('test_1')),  # Support for filtering fields
         ], 
         any=[
-
             FieldCondition(key='order', matcher=MatchField(8, comparator=operator.ge)),
             IDCondition(MatchID([1, 2, 3, 4, 5])),  # Support for filtering IDs
+        ],
+        must_not=[
+            IDCondition(MatchID([8])), 
+            FieldCondition(key='order', matcher=MatchField(8, comparator=operator.ge)),
         ]
     )
 )
 
 print(collection.query_report_)
 ```
 
     
     * - MOST RECENT QUERY REPORT -
     | - Collection Shape: (10, 4)
-    | - Query Time: 0.11985 s
+    | - Query Time: 0.09065 s
     | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 Results ID: [ 2  1  4  5 10  3]
-    | - Top 10 Results Similarity: [1.         0.86097705 0.85727406 0.813797   0.78595245 0.34695023]
+    | - Top 10 Results ID: [2 1]
+    | - Top 10 Results Similarity: [1.         0.86097705]
     * - END OF REPORT -
     
 
 
 ### Drop a collection
 
 
 ```python
 print("Collection list before dropping:", my_db.show_collections())
-my_db.drop_collection("test_collection")
+status = my_db.drop_collection("test_collection")
 print("Collection list after dropped:", my_db.show_collections())
 ```
 
     Collection list before dropping: ['test_collection']
+    {'status': 'success', 'params': {'collection_name': 'test_collection', 'exists': False}}
     Collection list after dropped: []
 
 
 ## Drop the database
 
 
 ```python
 my_db.drop_database()
 my_db
 ```
 
 
 
 
-    MinVectorDB remote server at http://localhost:5403 does not exist.
+    MinVectorDB remote server at http://localhost:7637 does not exist.
 
 
 
 
 ```python
 my_db.database_exists()
 ```
```

#### html2text {}

```diff
@@ -1,142 +1,142 @@
-Metadata-Version: 2.1 Name: MinVectorDB Version: 0.3.2 Summary: A pure Python-
+Metadata-Version: 2.1 Name: MinVectorDB Version: 0.3.3 Summary: A pure Python-
 implemented, lightweight, server-optional, multi-end compatible, vector
 database deployable locally or remotely. Home-page: https://github.com/
 BirchKwok/MinVectorDB Author: Birch Kwok Author-email: birchkwok@gmail.com
 Keywords: vector database Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development Classifier: Topic :: Scientific/Engineering Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: numpy>=1.17.0 Requires-Dist: spinesUtils>=0.3.13 Requires-Dist:
 msgpack>=1.0.2 Requires-Dist: scikit-learn>=1.0.0 Requires-Dist:
 cloudpickle>=2.0.0 Requires-Dist: numexpr>=2.7.3 Requires-Dist:
-pyroaring>=0.4.5 Requires-Dist: jax>=0.4.25 Requires-Dist: numba>=0.54.0
-Requires-Dist: jaxlib>=0.4.25 Requires-Dist: flask>=2.0.1 Requires-Dist:
-PyYAML>=5.4.1 Requires-Dist: portalocker>=2.3.0 Requires-Dist: requests>=2.26.0
-Requires-Dist: waitress>=2.0.0
+pyroaring>=0.4.5 Requires-Dist: jax>=0.4.25 Requires-Dist: jaxlib>=0.4.25
+Requires-Dist: flask>=2.0.1 Requires-Dist: PyYAML>=5.4.1 Requires-Dist:
+waitress>=2.0.0 Requires-Dist: pytest>=7.4.4 Requires-Dist: tqdm>=4.62.3
+Requires-Dist: setuptools>=68.0.0 Requires-Dist: httpx[http2]>=0.19.0
                                  _[_M_i_n_V_e_c_t_o_r_D_B_]
     ******** AA ppuurree PPyytthhoonn--iimmpplleemmeenntteedd,, lliigghhttwweeiigghhtt,, sseerrvveerr--ooppttiioonnaall,, mmuullttii--eenndd
        ccoommppaattiibbllee,, vveeccttoorr ddaattaabbaassee ddeeppllooyyaabbllee llooccaallllyy oorr rreemmootteellyy.. ********
-     _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _p_a_c_k_a_g_e_]
-â¡ **Serverless, simple parameters, simple API.** â¡ **Fast, memory-
+ _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _t_e_s_t_i_n_g_]_[_D_o_c_k_e_r
+                                    _b_u_i_l_d_]
+â¡ **Server-optional, simple parameters, simple API.** â¡ **Fast, memory-
 efficient, easily scales to millions of vectors.** â¡ **Supports cosine
 similarity and L2 distance, uses FLAT for exhaustive search or IVF-FLAT for
 inverted indexing.** â¡ **Friendly caching technology stores recently queried
 vectors for accelerated access.** â¡ **Based on a generic Python software
 stack, platform-independent, highly versatile.** > **WARNING**: MinVectorDB is
 actively being updated, and API backward compatibility is not guaranteed. You
 should use version numbers as a strong constraint during deployment to avoid
 unnecessary feature conflicts and errors. > **Although our goal is to enable
 brute force search or inverted indexing on billion-scale vectors, we currently
 still recommend using it on a scale of millions of vectors or less for the best
 experience.** *MinVectorDB* is a vector database implemented purely in Python,
-designed to be lightweight, serverless, and easy to deploy locally. It offers
-straightforward and clear Python APIs, aiming to lower the entry barrier for
-using vector databases. In response to user needs and to enhance its
-practicality, we are planning to introduce new features, including but not
-limited to: - **Optimizing Global Search Performance**: We are focusing on
-algorithm and data structure enhancements to speed up searches across the
+designed to be lightweight, server-optional, and easy to deploy locally or
+remotely. It offers straightforward and clear Python APIs, aiming to lower the
+entry barrier for using vector databases. In response to user needs and to
+enhance its practicality, we are planning to introduce new features, including
+but not limited to: - **Optimizing Global Search Performance**: We are focusing
+on algorithm and data structure enhancements to speed up searches across the
 database, enabling faster retrieval of vector data. - **Enhancing Cluster
 Search with Inverted Indexes**: Utilizing inverted index technology, we aim to
 refine the cluster search process for better search efficiency and precision. -
 **Refining Clustering Algorithms**: By improving our clustering algorithms, we
 intend to offer more precise and efficient data clustering to support complex
 queries. - **Facilitating Vector Modifications and Deletions**: We will
 introduce features to modify and delete vectors, allowing for more flexible
-data management. - **Implementing Rollback Strategies**: To increase database
-robustness and data security, rollback strategies will be added, helping users
-recover from incorrect operations or system failures easily. MinVectorDB
-focuses on achieving 100% recall, prioritizing recall accuracy over high-speed
-search performance. This approach ensures that users can reliably retrieve all
-relevant vector data, making MinVectorDB particularly suitable for applications
-that require responses within hundreds of milliseconds. While the project has
-not yet been benchmarked against other systems, we believe these planned
-features will significantly enhance MinVectorDB's capabilities in managing and
-retrieving vector data, addressing a wide range of user needs. ## Install
-Client API package (Mandatory) ```shell pip install MinVectorDB ``` ## If you
-wish to use Docker (Optional) ```shell docker pull birchkwok/minvectordb:latest
-``` ## Qucik Start ```python import min_vec print("MinVectorDB version is: ",
-min_vec.__version__) ``` MinVectorDB version is: 0.3.2 ## Initialize Database
-MinVectorDB now supports HTTP API and Python local code API. The HTTP API mode
-requires starting an HTTP server beforehand. You have two options: - start
-directly. For direct startup, the default port is 7637. You can run the
-following command in the terminal to start the service: ```shell min_vec run --
-host 127.0.0.1 --port 7637 ``` - within Docker In Docker, the default port is
-5403. You can run the following command in the terminal to start the service:
-```shell docker run -p 5403:7637 birchkwok/minvectordb:latest ``` ```python
-from min_vec import MinVectorDB # This method is for the Python local code API,
-recommended only for CI/CD testing or single-user local use. # Specify database
-root directory my_db = MinVectorDB('my_vec_db') # Judgment condition, root_path
-does not start with http or https # or # Use the HTTP API mode, it is suitable
-for use in production environments. # For direct startup my_db = MinVectorDB
-("http://127.0.0.1:7637") # within Docker my_db = MinVectorDB("http://
-127.0.0.1:5403") ``` ```python from min_vec import MinVectorDB # For direct
-startup my_db = MinVectorDB("http://localhost:5403") ``` ### create a
-collection ```python collection = my_db.require_collection("test_collection",
-4, drop_if_exists=True, scaler_bits=8) ``` ### Add vectors When inserting
-vectors, collection requires manually running the `commit` function or
-inserting within the `insert_session` function context manager, which will run
-the `commit` function in the background. ```python with
-collection.insert_session(): id = collection.add_item(vector=[0.01, 0.34, 0.74,
-0.31], id=1, field={'field': 'test_1', 'order': 0}) # id = 0 id =
-collection.add_item(vector=[0.36, 0.43, 0.56, 0.12], id=2, field={'field':
-'test_1', 'order': 1}) # id = 1 id = collection.add_item(vector=[0.03, 0.04,
-0.10, 0.51], id=3, field={'field': 'test_2', 'order': 2}) # id = 2 id =
-collection.add_item(vector=[0.11, 0.44, 0.23, 0.24], id=4, field={'field':
-'test_2', 'order': 3}) # id = 3 id = collection.add_item(vector=[0.91, 0.43,
-0.44, 0.67], id=5, field={'field': 'test_2', 'order': 4}) # id = 4 id =
-collection.add_item(vector=[0.92, 0.12, 0.56, 0.19], id=6, field={'field':
-'test_3', 'order': 5}) # id = 5 id = collection.add_item(vector=[0.18, 0.34,
-0.56, 0.71], id=7, field={'field': 'test_1', 'order': 6}) # id = 6 id =
-collection.add_item(vector=[0.01, 0.33, 0.14, 0.31], id=8, field={'field':
-'test_2', 'order': 7}) # id = 7 id = collection.add_item(vector=[0.71, 0.75,
-0.91, 0.82], id=9, field={'field': 'test_3', 'order': 8}) # id = 8 id =
-collection.add_item(vector=[0.75, 0.44, 0.38, 0.75], id=10, field={'field':
-'test_1', 'order': 9}) # id = 9 # If you do not use the insert_session
-function, you need to manually call the commit function to submit the data #
-collection.commit() ``` ```python # or use the bulk_add_items function # with
-collection.insert_session(): # ids = collection.bulk_add_items([([0.01, 0.34,
-0.74, 0.31], 0, {'field': 'test_1', 'order': 0}), # ([0.36, 0.43, 0.56, 0.12],
-1, {'field': 'test_1', 'order': 1}), # ([0.03, 0.04, 0.10, 0.51], 2, {'field':
-'test_2', 'order': 2}), # ([0.11, 0.44, 0.23, 0.24], 3, {'field': 'test_2',
-'order': 3}), # ([0.91, 0.43, 0.44, 0.67], 4, {'field': 'test_2', 'order': 4}),
-# ([0.92, 0.12, 0.56, 0.19], 5, {'field': 'test_3', 'order': 5}), # ([0.18,
-0.34, 0.56, 0.71], 6, {'field': 'test_1', 'order': 6}), # ([0.01, 0.33, 0.14,
-0.31], 7, {'field': 'test_2', 'order': 7}), # ([0.71, 0.75, 0.91, 0.82], 8,
-{'field': 'test_3', 'order': 8}), # ([0.75, 0.44, 0.38, 0.75], 9, {'field':
-'test_1', 'order': 9})]) # print(ids) # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9] ``` ###
-Query ```python collection.query(vector=[0.36, 0.43, 0.56, 0.12], k=10) ```
-(array([ 2, 9, 1, 4, 6, 5, 10, 7, 8, 3]), array([1. , 0.92355633, 0.86097705,
-0.85727406, 0.81551266, 0.813797 , 0.78595245, 0.7741583 , 0.6871773 ,
-0.34695023])) ```python print(collection.query_report_) ``` * - MOST RECENT
-QUERY REPORT - | - Collection Shape: (10, 4) | - Query Time: 0.20518 s | -
-Query Distance: cosine | - Query K: 10 | - Top 10 Results ID: [ 2 9 1 4 6 5 10
-7 8 3] | - Top 10 Results Similarity: [1. 0.92355633 0.86097705 0.85727406
-0.81551266 0.813797 0.78595245 0.7741583 0.6871773 0.34695023] * - END OF
-REPORT - ### Use Filter ```python import operator from
-min_vec.structures.filter import Filter, FieldCondition, MatchField,
-IDCondition, MatchID collection.query( vector=[0.36, 0.43, 0.56, 0.12], k=10,
-query_filter=Filter( must=[ FieldCondition(key='field', matcher=MatchField
-('test_1')), # Support for filtering fields ], any=[ FieldCondition
-(key='order', matcher=MatchField(8, comparator=operator.ge)), IDCondition
-(MatchID([1, 2, 3, 4, 5])), # Support for filtering IDs ] ) ) print
+data management. MinVectorDB focuses on achieving 100% recall, prioritizing
+recall accuracy over high-speed search performance. This approach ensures that
+users can reliably retrieve all relevant vector data, making MinVectorDB
+particularly suitable for applications that require responses within hundreds
+of milliseconds. - [x] **Now supports HTTP API and Python local code API.** -
+[X] **Now supports Docker deployment.** - [X] **Now supports vector id and
+field filtering.** - [X] **Now supports transaction management; if a commit
+fails, it will automatically roll back.** ## Install Client API package
+(Mandatory) ```shell pip install MinVectorDB ``` ## If you wish to use Docker
+(Optional) ```shell docker pull birchkwok/minvectordb:latest ``` ## Qucik Start
+```python import min_vec print("MinVectorDB version is: ", min_vec.__version__)
+``` MinVectorDB version is: 0.3.3 ## Initialize Database MinVectorDB now
+supports HTTP API and Python local code API. The HTTP API mode requires
+starting an HTTP server beforehand. You have two options: - start directly. For
+direct startup, the default port is 7637. You can run the following command in
+the terminal to start the service: ```shell min_vec run --host localhost --port
+7637 ``` - within Docker In Docker, You can run the following command in the
+terminal to start the service: ```shell docker run -p 7637:7637 birchkwok/
+minvectordb:latest ``` ```python from min_vec import MinVectorDB # This method
+is for the Python local code API, recommended only for CI/CD testing or single-
+user local use. # Specify database root directory my_db = MinVectorDB
+('my_vec_db') # Judgment condition, root_path does not start with http or https
+# or # Use the HTTP API mode, it is suitable for use in production
+environments. my_db = MinVectorDB("http://localhost:7637") ``` ```python from
+min_vec import MinVectorDB # For direct startup my_db = MinVectorDB("http://
+localhost:7637") ``` ### create a collection ```python collection =
+my_db.require_collection("test_collection", 4, drop_if_exists=True,
+scaler_bits=8) ``` ### Add vectors When inserting vectors, collection requires
+manually running the `commit` function or inserting within the `insert_session`
+function context manager, which will run the `commit` function in the
+background. ```python with collection.insert_session(): id =
+collection.add_item(vector=[0.01, 0.34, 0.74, 0.31], id=1, field={'field':
+'test_1', 'order': 0}) # id = 0 id = collection.add_item(vector=[0.36, 0.43,
+0.56, 0.12], id=2, field={'field': 'test_1', 'order': 1}) # id = 1 id =
+collection.add_item(vector=[0.03, 0.04, 0.10, 0.51], id=3, field={'field':
+'test_2', 'order': 2}) # id = 2 id = collection.add_item(vector=[0.11, 0.44,
+0.23, 0.24], id=4, field={'field': 'test_2', 'order': 3}) # id = 3 id =
+collection.add_item(vector=[0.91, 0.43, 0.44, 0.67], id=5, field={'field':
+'test_2', 'order': 4}) # id = 4 id = collection.add_item(vector=[0.92, 0.12,
+0.56, 0.19], id=6, field={'field': 'test_3', 'order': 5}) # id = 5 id =
+collection.add_item(vector=[0.18, 0.34, 0.56, 0.71], id=7, field={'field':
+'test_1', 'order': 6}) # id = 6 id = collection.add_item(vector=[0.01, 0.33,
+0.14, 0.31], id=8, field={'field': 'test_2', 'order': 7}) # id = 7 id =
+collection.add_item(vector=[0.71, 0.75, 0.91, 0.82], id=9, field={'field':
+'test_3', 'order': 8}) # id = 8 id = collection.add_item(vector=[0.75, 0.44,
+0.38, 0.75], id=10, field={'field': 'test_1', 'order': 9}) # id = 9 # If you do
+not use the insert_session function, you need to manually call the commit
+function to submit the data # collection.commit() ``` ```python # or use the
+bulk_add_items function # with collection.insert_session(): # ids =
+collection.bulk_add_items([([0.01, 0.34, 0.74, 0.31], 0, {'field': 'test_1',
+'order': 0}), # ([0.36, 0.43, 0.56, 0.12], 1, {'field': 'test_1', 'order': 1}),
+# ([0.03, 0.04, 0.10, 0.51], 2, {'field': 'test_2', 'order': 2}), # ([0.11,
+0.44, 0.23, 0.24], 3, {'field': 'test_2', 'order': 3}), # ([0.91, 0.43, 0.44,
+0.67], 4, {'field': 'test_2', 'order': 4}), # ([0.92, 0.12, 0.56, 0.19], 5,
+{'field': 'test_3', 'order': 5}), # ([0.18, 0.34, 0.56, 0.71], 6, {'field':
+'test_1', 'order': 6}), # ([0.01, 0.33, 0.14, 0.31], 7, {'field': 'test_2',
+'order': 7}), # ([0.71, 0.75, 0.91, 0.82], 8, {'field': 'test_3', 'order': 8}),
+# ([0.75, 0.44, 0.38, 0.75], 9, {'field': 'test_1', 'order': 9})]) # print(ids)
+# [0, 1, 2, 3, 4, 5, 6, 7, 8, 9] ``` ### Query ```python collection.query
+(vector=[0.36, 0.43, 0.56, 0.12], k=10) ``` (array([ 2, 9, 1, 4, 6, 5, 10, 7,
+8, 3]), array([1. , 0.92355633, 0.86097705, 0.85727406, 0.81551266, 0.813797 ,
+0.78595245, 0.7741583 , 0.6871773 , 0.34695023])) ```python print
 (collection.query_report_) ``` * - MOST RECENT QUERY REPORT - | - Collection
-Shape: (10, 4) | - Query Time: 0.11985 s | - Query Distance: cosine | - Query
-K: 10 | - Top 10 Results ID: [ 2 1 4 5 10 3] | - Top 10 Results Similarity: [1.
-0.86097705 0.85727406 0.813797 0.78595245 0.34695023] * - END OF REPORT - ###
-Drop a collection ```python print("Collection list before dropping:",
-my_db.show_collections()) my_db.drop_collection("test_collection") print
-("Collection list after dropped:", my_db.show_collections()) ``` Collection
-list before dropping: ['test_collection'] Collection list after dropped: [] ##
-Drop the database ```python my_db.drop_database() my_db ``` MinVectorDB remote
-server at http://localhost:5403 does not exist. ```python my_db.database_exists
+Shape: (10, 4) | - Query Time: 0.15716 s | - Query Distance: cosine | - Query
+K: 10 | - Top 10 Results ID: [ 2 9 1 4 6 5 10 7 8 3] | - Top 10 Results
+Similarity: [1. 0.92355633 0.86097705 0.85727406 0.81551266 0.813797 0.78595245
+0.7741583 0.6871773 0.34695023] * - END OF REPORT - ### Use Filter ```python
+import operator from min_vec.core_components.filter import Filter,
+FieldCondition, MatchField, IDCondition, MatchID collection.query( vector=
+[0.36, 0.43, 0.56, 0.12], k=10, query_filter=Filter( must=[ FieldCondition
+(key='field', matcher=MatchField('test_1')), # Support for filtering fields ],
+any=[ FieldCondition(key='order', matcher=MatchField(8,
+comparator=operator.ge)), IDCondition(MatchID([1, 2, 3, 4, 5])), # Support for
+filtering IDs ], must_not=[ IDCondition(MatchID([8])), FieldCondition
+(key='order', matcher=MatchField(8, comparator=operator.ge)), ] ) ) print
+(collection.query_report_) ``` * - MOST RECENT QUERY REPORT - | - Collection
+Shape: (10, 4) | - Query Time: 0.09065 s | - Query Distance: cosine | - Query
+K: 10 | - Top 10 Results ID: [2 1] | - Top 10 Results Similarity: [1.
+0.86097705] * - END OF REPORT - ### Drop a collection ```python print
+("Collection list before dropping:", my_db.show_collections()) status =
+my_db.drop_collection("test_collection") print("Collection list after dropped:
+", my_db.show_collections()) ``` Collection list before dropping:
+['test_collection'] {'status': 'success', 'params': {'collection_name':
+'test_collection', 'exists': False}} Collection list after dropped: [] ## Drop
+the database ```python my_db.drop_database() my_db ``` MinVectorDB remote
+server at http://localhost:7637 does not exist. ```python my_db.database_exists
 () ``` {'status': 'success', 'params': {'exists': False}} ## What's Next -
 [Collection's operations](https://github.com/BirchKwok/MinVectorDB/blob/main/
 tutorials/collections.ipynb) - [Add vectors to collection](https://github.com/
 BirchKwok/MinVectorDB/blob/main/tutorials/add_vectors.ipynb) - [Using different
 indexing methods](https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/
 index_mode.ipynb) - [Using different distance metric functions](https://
 github.com/BirchKwok/MinVectorDB/blob/main/tutorials/distance.ipynb) -
```

### Comparing `minvectordb-0.3.2/MinVectorDB.egg-info/SOURCES.txt` & `minvectordb-0.3.3/MinVectorDB.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,33 +15,36 @@
 min_vec/api/http_api.py
 min_vec/api/low_level.py
 min_vec/computational_layer/__init__.py
 min_vec/computational_layer/engines.py
 min_vec/configs/__init__.py
 min_vec/configs/config.py
 min_vec/configs/parameters_validator.py
+min_vec/core_components/__init__.py
+min_vec/core_components/counter.py
+min_vec/core_components/cross_lock.py
+min_vec/core_components/filter.py
+min_vec/core_components/id_checker.py
+min_vec/core_components/kmeans.py
+min_vec/core_components/limited_dict.py
+min_vec/core_components/limited_sort.py
+min_vec/core_components/metadata_kv.py
+min_vec/core_components/scaler.py
+min_vec/core_components/thread_safe_list.py
 min_vec/execution_layer/__init__.py
 min_vec/execution_layer/cluster_worker.py
 min_vec/execution_layer/matrix_serializer.py
 min_vec/execution_layer/query.py
 min_vec/execution_layer/session.py
 min_vec/storage_layer/__init__.py
 min_vec/storage_layer/storage.py
-min_vec/structures/__init__.py
-min_vec/structures/counter.py
-min_vec/structures/fields_filter.py
-min_vec/structures/filter.py
-min_vec/structures/id_checker.py
-min_vec/structures/kmeans.py
-min_vec/structures/limited_dict.py
-min_vec/structures/limited_sort.py
-min_vec/structures/scaler.py
 min_vec/utils/__init__.py
 min_vec/utils/utils.py
 test/__init__.py
 test/docker_tests/__init__.py
+test/docker_tests/test_client_api.py
 test/docker_tests/test_docker_api.py
 test/standard_tests/__init__.py
 test/standard_tests/test_hmvdb_initial.py
 test/standard_tests/test_http_api.py
 test/standard_tests/test_smvdb_initial.py
 test/standard_tests/test_smvdb_save_and_query.py
```

### Comparing `minvectordb-0.3.2/PKG-INFO` & `minvectordb-0.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MinVectorDB
-Version: 0.3.2
+Version: 0.3.3
 Summary: A pure Python-implemented, lightweight, server-optional, multi-end compatible, vector database deployable locally or remotely.
 Home-page: https://github.com/BirchKwok/MinVectorDB
 Author: Birch Kwok
 Author-email: birchkwok@gmail.com
 Keywords: vector database
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -23,57 +23,61 @@
 Requires-Dist: spinesUtils>=0.3.13
 Requires-Dist: msgpack>=1.0.2
 Requires-Dist: scikit-learn>=1.0.0
 Requires-Dist: cloudpickle>=2.0.0
 Requires-Dist: numexpr>=2.7.3
 Requires-Dist: pyroaring>=0.4.5
 Requires-Dist: jax>=0.4.25
-Requires-Dist: numba>=0.54.0
 Requires-Dist: jaxlib>=0.4.25
 Requires-Dist: flask>=2.0.1
 Requires-Dist: PyYAML>=5.4.1
-Requires-Dist: portalocker>=2.3.0
-Requires-Dist: requests>=2.26.0
 Requires-Dist: waitress>=2.0.0
+Requires-Dist: pytest>=7.4.4
+Requires-Dist: tqdm>=4.62.3
+Requires-Dist: setuptools>=68.0.0
+Requires-Dist: httpx[http2]>=0.19.0
 
 <div align="center">
   <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB" style="max-width: 20%; height: auto;"></a>
   <h3>A pure Python-implemented, lightweight, server-optional, multi-end compatible, vector database deployable locally or remotely.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/l/MinVectorDB" alt="PyPI - License"></a>
-    <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml/badge.svg" alt="Python package"></a>
+    <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-tests.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-tests.yml/badge.svg" alt="Python testing"></a>
+    <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/docker-tests.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/docker-tests.yml/badge.svg" alt="Docker build"></a>
   </p>
 </div>
 
-⚡ **Serverless, simple parameters, simple API.**
+⚡ **Server-optional, simple parameters, simple API.**
 
 ⚡ **Fast, memory-efficient, easily scales to millions of vectors.**
 
 ⚡ **Supports cosine similarity and L2 distance, uses FLAT for exhaustive search or IVF-FLAT for inverted indexing.**
 
 ⚡ **Friendly caching technology stores recently queried vectors for accelerated access.**
 
 ⚡ **Based on a generic Python software stack, platform-independent, highly versatile.**
 
 > **WARNING**: MinVectorDB is actively being updated, and API backward compatibility is not guaranteed. You should use version numbers as a strong constraint during deployment to avoid unnecessary feature conflicts and errors.
 > **Although our goal is to enable brute force search or inverted indexing on billion-scale vectors, we currently still recommend using it on a scale of millions of vectors or less for the best experience.**
 
-*MinVectorDB* is a vector database implemented purely in Python, designed to be lightweight, serverless, and easy to deploy locally. It offers straightforward and clear Python APIs, aiming to lower the entry barrier for using vector databases. In response to user needs and to enhance its practicality, we are planning to introduce new features, including but not limited to:
+*MinVectorDB* is a vector database implemented purely in Python, designed to be lightweight, server-optional, and easy to deploy locally or remotely. It offers straightforward and clear Python APIs, aiming to lower the entry barrier for using vector databases. In response to user needs and to enhance its practicality, we are planning to introduce new features, including but not limited to:
 
 - **Optimizing Global Search Performance**: We are focusing on algorithm and data structure enhancements to speed up searches across the database, enabling faster retrieval of vector data.
 - **Enhancing Cluster Search with Inverted Indexes**: Utilizing inverted index technology, we aim to refine the cluster search process for better search efficiency and precision.
 - **Refining Clustering Algorithms**: By improving our clustering algorithms, we intend to offer more precise and efficient data clustering to support complex queries.
 - **Facilitating Vector Modifications and Deletions**: We will introduce features to modify and delete vectors, allowing for more flexible data management.
-- **Implementing Rollback Strategies**: To increase database robustness and data security, rollback strategies will be added, helping users recover from incorrect operations or system failures easily.
 
 MinVectorDB focuses on achieving 100% recall, prioritizing recall accuracy over high-speed search performance. This approach ensures that users can reliably retrieve all relevant vector data, making MinVectorDB particularly suitable for applications that require responses within hundreds of milliseconds.
 
-While the project has not yet been benchmarked against other systems, we believe these planned features will significantly enhance MinVectorDB's capabilities in managing and retrieving vector data, addressing a wide range of user needs.
+- [x] **Now supports HTTP API and Python local code API.**
+- [X] **Now supports Docker deployment.**
+- [X] **Now supports vector id and field filtering.**
+- [X] **Now supports transaction management; if a commit fails, it will automatically roll back.**
 
 ## Install Client API package (Mandatory)
 
 ```shell
 pip install MinVectorDB
 ```
 
@@ -87,58 +91,54 @@
 
 
 ```python
 import min_vec
 print("MinVectorDB version is: ", min_vec.__version__)
 ```
 
-    MinVectorDB version is:  0.3.2
+    MinVectorDB version is:  0.3.3
 
 
 ## Initialize Database
 
 MinVectorDB now supports HTTP API and Python local code API. 
 
 
 The HTTP API mode requires starting an HTTP server beforehand. You have two options: 
 - start directly.
   
   For direct startup, the default port is 7637. You can run the following command in the terminal to start the service:
 ```shell
-min_vec run --host 127.0.0.1 --port 7637
+min_vec run --host localhost --port 7637
 ```
 
 - within Docker
   
-  In Docker, the default port is 5403. You can run the following command in the terminal to start the service:
+  In Docker, You can run the following command in the terminal to start the service:
 ```shell
-docker run -p 5403:7637 birchkwok/minvectordb:latest
+docker run -p 7637:7637 birchkwok/minvectordb:latest
 ```
 
 ```python
 from min_vec import MinVectorDB
 
 # This method is for the Python local code API, recommended only for CI/CD testing or single-user local use.
 # Specify database root directory
 my_db = MinVectorDB('my_vec_db')  # Judgment condition, root_path does not start with http or https
 # or
 # Use the HTTP API mode, it is suitable for use in production environments.
-# For direct startup
-my_db = MinVectorDB("http://127.0.0.1:7637")
-
-# within Docker
-my_db = MinVectorDB("http://127.0.0.1:5403")
+my_db = MinVectorDB("http://localhost:7637")
 ```
 
 
 ```python
 from min_vec import MinVectorDB
 
 # For direct startup
-my_db = MinVectorDB("http://localhost:5403")
+my_db = MinVectorDB("http://localhost:7637")
 ```
 
 ### create a collection
 
 
 ```python
 collection = my_db.require_collection("test_collection", 4, drop_if_exists=True, scaler_bits=8)
@@ -203,15 +203,15 @@
 ```python
 print(collection.query_report_)
 ```
 
     
     * - MOST RECENT QUERY REPORT -
     | - Collection Shape: (10, 4)
-    | - Query Time: 0.20518 s
+    | - Query Time: 0.15716 s
     | - Query Distance: cosine
     | - Query K: 10
     | - Top 10 Results ID: [ 2  9  1  4  6  5 10  7  8  3]
     | - Top 10 Results Similarity: [1.         0.92355633 0.86097705 0.85727406 0.81551266 0.813797
      0.78595245 0.7741583  0.6871773  0.34695023]
     * - END OF REPORT -
     
@@ -219,72 +219,76 @@
 
 ### Use Filter
 
 
 ```python
 import operator
 
-from min_vec.structures.filter import Filter, FieldCondition, MatchField, IDCondition, MatchID
+from min_vec.core_components.filter import Filter, FieldCondition, MatchField, IDCondition, MatchID
 
 
 collection.query(
     vector=[0.36, 0.43, 0.56, 0.12], 
     k=10, 
     query_filter=Filter(
         must=[
             FieldCondition(key='field', matcher=MatchField('test_1')),  # Support for filtering fields
         ], 
         any=[
-
             FieldCondition(key='order', matcher=MatchField(8, comparator=operator.ge)),
             IDCondition(MatchID([1, 2, 3, 4, 5])),  # Support for filtering IDs
+        ],
+        must_not=[
+            IDCondition(MatchID([8])), 
+            FieldCondition(key='order', matcher=MatchField(8, comparator=operator.ge)),
         ]
     )
 )
 
 print(collection.query_report_)
 ```
 
     
     * - MOST RECENT QUERY REPORT -
     | - Collection Shape: (10, 4)
-    | - Query Time: 0.11985 s
+    | - Query Time: 0.09065 s
     | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 Results ID: [ 2  1  4  5 10  3]
-    | - Top 10 Results Similarity: [1.         0.86097705 0.85727406 0.813797   0.78595245 0.34695023]
+    | - Top 10 Results ID: [2 1]
+    | - Top 10 Results Similarity: [1.         0.86097705]
     * - END OF REPORT -
     
 
 
 ### Drop a collection
 
 
 ```python
 print("Collection list before dropping:", my_db.show_collections())
-my_db.drop_collection("test_collection")
+status = my_db.drop_collection("test_collection")
 print("Collection list after dropped:", my_db.show_collections())
 ```
 
     Collection list before dropping: ['test_collection']
+    {'status': 'success', 'params': {'collection_name': 'test_collection', 'exists': False}}
     Collection list after dropped: []
 
 
 ## Drop the database
 
 
 ```python
 my_db.drop_database()
 my_db
 ```
 
 
 
 
-    MinVectorDB remote server at http://localhost:5403 does not exist.
+    MinVectorDB remote server at http://localhost:7637 does not exist.
 
 
 
 
 ```python
 my_db.database_exists()
 ```
```

#### html2text {}

```diff
@@ -1,142 +1,142 @@
-Metadata-Version: 2.1 Name: MinVectorDB Version: 0.3.2 Summary: A pure Python-
+Metadata-Version: 2.1 Name: MinVectorDB Version: 0.3.3 Summary: A pure Python-
 implemented, lightweight, server-optional, multi-end compatible, vector
 database deployable locally or remotely. Home-page: https://github.com/
 BirchKwok/MinVectorDB Author: Birch Kwok Author-email: birchkwok@gmail.com
 Keywords: vector database Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development Classifier: Topic :: Scientific/Engineering Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: numpy>=1.17.0 Requires-Dist: spinesUtils>=0.3.13 Requires-Dist:
 msgpack>=1.0.2 Requires-Dist: scikit-learn>=1.0.0 Requires-Dist:
 cloudpickle>=2.0.0 Requires-Dist: numexpr>=2.7.3 Requires-Dist:
-pyroaring>=0.4.5 Requires-Dist: jax>=0.4.25 Requires-Dist: numba>=0.54.0
-Requires-Dist: jaxlib>=0.4.25 Requires-Dist: flask>=2.0.1 Requires-Dist:
-PyYAML>=5.4.1 Requires-Dist: portalocker>=2.3.0 Requires-Dist: requests>=2.26.0
-Requires-Dist: waitress>=2.0.0
+pyroaring>=0.4.5 Requires-Dist: jax>=0.4.25 Requires-Dist: jaxlib>=0.4.25
+Requires-Dist: flask>=2.0.1 Requires-Dist: PyYAML>=5.4.1 Requires-Dist:
+waitress>=2.0.0 Requires-Dist: pytest>=7.4.4 Requires-Dist: tqdm>=4.62.3
+Requires-Dist: setuptools>=68.0.0 Requires-Dist: httpx[http2]>=0.19.0
                                  _[_M_i_n_V_e_c_t_o_r_D_B_]
     ******** AA ppuurree PPyytthhoonn--iimmpplleemmeenntteedd,, lliigghhttwweeiigghhtt,, sseerrvveerr--ooppttiioonnaall,, mmuullttii--eenndd
        ccoommppaattiibbllee,, vveeccttoorr ddaattaabbaassee ddeeppllooyyaabbllee llooccaallllyy oorr rreemmootteellyy.. ********
-     _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _p_a_c_k_a_g_e_]
-â¡ **Serverless, simple parameters, simple API.** â¡ **Fast, memory-
+ _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _t_e_s_t_i_n_g_]_[_D_o_c_k_e_r
+                                    _b_u_i_l_d_]
+â¡ **Server-optional, simple parameters, simple API.** â¡ **Fast, memory-
 efficient, easily scales to millions of vectors.** â¡ **Supports cosine
 similarity and L2 distance, uses FLAT for exhaustive search or IVF-FLAT for
 inverted indexing.** â¡ **Friendly caching technology stores recently queried
 vectors for accelerated access.** â¡ **Based on a generic Python software
 stack, platform-independent, highly versatile.** > **WARNING**: MinVectorDB is
 actively being updated, and API backward compatibility is not guaranteed. You
 should use version numbers as a strong constraint during deployment to avoid
 unnecessary feature conflicts and errors. > **Although our goal is to enable
 brute force search or inverted indexing on billion-scale vectors, we currently
 still recommend using it on a scale of millions of vectors or less for the best
 experience.** *MinVectorDB* is a vector database implemented purely in Python,
-designed to be lightweight, serverless, and easy to deploy locally. It offers
-straightforward and clear Python APIs, aiming to lower the entry barrier for
-using vector databases. In response to user needs and to enhance its
-practicality, we are planning to introduce new features, including but not
-limited to: - **Optimizing Global Search Performance**: We are focusing on
-algorithm and data structure enhancements to speed up searches across the
+designed to be lightweight, server-optional, and easy to deploy locally or
+remotely. It offers straightforward and clear Python APIs, aiming to lower the
+entry barrier for using vector databases. In response to user needs and to
+enhance its practicality, we are planning to introduce new features, including
+but not limited to: - **Optimizing Global Search Performance**: We are focusing
+on algorithm and data structure enhancements to speed up searches across the
 database, enabling faster retrieval of vector data. - **Enhancing Cluster
 Search with Inverted Indexes**: Utilizing inverted index technology, we aim to
 refine the cluster search process for better search efficiency and precision. -
 **Refining Clustering Algorithms**: By improving our clustering algorithms, we
 intend to offer more precise and efficient data clustering to support complex
 queries. - **Facilitating Vector Modifications and Deletions**: We will
 introduce features to modify and delete vectors, allowing for more flexible
-data management. - **Implementing Rollback Strategies**: To increase database
-robustness and data security, rollback strategies will be added, helping users
-recover from incorrect operations or system failures easily. MinVectorDB
-focuses on achieving 100% recall, prioritizing recall accuracy over high-speed
-search performance. This approach ensures that users can reliably retrieve all
-relevant vector data, making MinVectorDB particularly suitable for applications
-that require responses within hundreds of milliseconds. While the project has
-not yet been benchmarked against other systems, we believe these planned
-features will significantly enhance MinVectorDB's capabilities in managing and
-retrieving vector data, addressing a wide range of user needs. ## Install
-Client API package (Mandatory) ```shell pip install MinVectorDB ``` ## If you
-wish to use Docker (Optional) ```shell docker pull birchkwok/minvectordb:latest
-``` ## Qucik Start ```python import min_vec print("MinVectorDB version is: ",
-min_vec.__version__) ``` MinVectorDB version is: 0.3.2 ## Initialize Database
-MinVectorDB now supports HTTP API and Python local code API. The HTTP API mode
-requires starting an HTTP server beforehand. You have two options: - start
-directly. For direct startup, the default port is 7637. You can run the
-following command in the terminal to start the service: ```shell min_vec run --
-host 127.0.0.1 --port 7637 ``` - within Docker In Docker, the default port is
-5403. You can run the following command in the terminal to start the service:
-```shell docker run -p 5403:7637 birchkwok/minvectordb:latest ``` ```python
-from min_vec import MinVectorDB # This method is for the Python local code API,
-recommended only for CI/CD testing or single-user local use. # Specify database
-root directory my_db = MinVectorDB('my_vec_db') # Judgment condition, root_path
-does not start with http or https # or # Use the HTTP API mode, it is suitable
-for use in production environments. # For direct startup my_db = MinVectorDB
-("http://127.0.0.1:7637") # within Docker my_db = MinVectorDB("http://
-127.0.0.1:5403") ``` ```python from min_vec import MinVectorDB # For direct
-startup my_db = MinVectorDB("http://localhost:5403") ``` ### create a
-collection ```python collection = my_db.require_collection("test_collection",
-4, drop_if_exists=True, scaler_bits=8) ``` ### Add vectors When inserting
-vectors, collection requires manually running the `commit` function or
-inserting within the `insert_session` function context manager, which will run
-the `commit` function in the background. ```python with
-collection.insert_session(): id = collection.add_item(vector=[0.01, 0.34, 0.74,
-0.31], id=1, field={'field': 'test_1', 'order': 0}) # id = 0 id =
-collection.add_item(vector=[0.36, 0.43, 0.56, 0.12], id=2, field={'field':
-'test_1', 'order': 1}) # id = 1 id = collection.add_item(vector=[0.03, 0.04,
-0.10, 0.51], id=3, field={'field': 'test_2', 'order': 2}) # id = 2 id =
-collection.add_item(vector=[0.11, 0.44, 0.23, 0.24], id=4, field={'field':
-'test_2', 'order': 3}) # id = 3 id = collection.add_item(vector=[0.91, 0.43,
-0.44, 0.67], id=5, field={'field': 'test_2', 'order': 4}) # id = 4 id =
-collection.add_item(vector=[0.92, 0.12, 0.56, 0.19], id=6, field={'field':
-'test_3', 'order': 5}) # id = 5 id = collection.add_item(vector=[0.18, 0.34,
-0.56, 0.71], id=7, field={'field': 'test_1', 'order': 6}) # id = 6 id =
-collection.add_item(vector=[0.01, 0.33, 0.14, 0.31], id=8, field={'field':
-'test_2', 'order': 7}) # id = 7 id = collection.add_item(vector=[0.71, 0.75,
-0.91, 0.82], id=9, field={'field': 'test_3', 'order': 8}) # id = 8 id =
-collection.add_item(vector=[0.75, 0.44, 0.38, 0.75], id=10, field={'field':
-'test_1', 'order': 9}) # id = 9 # If you do not use the insert_session
-function, you need to manually call the commit function to submit the data #
-collection.commit() ``` ```python # or use the bulk_add_items function # with
-collection.insert_session(): # ids = collection.bulk_add_items([([0.01, 0.34,
-0.74, 0.31], 0, {'field': 'test_1', 'order': 0}), # ([0.36, 0.43, 0.56, 0.12],
-1, {'field': 'test_1', 'order': 1}), # ([0.03, 0.04, 0.10, 0.51], 2, {'field':
-'test_2', 'order': 2}), # ([0.11, 0.44, 0.23, 0.24], 3, {'field': 'test_2',
-'order': 3}), # ([0.91, 0.43, 0.44, 0.67], 4, {'field': 'test_2', 'order': 4}),
-# ([0.92, 0.12, 0.56, 0.19], 5, {'field': 'test_3', 'order': 5}), # ([0.18,
-0.34, 0.56, 0.71], 6, {'field': 'test_1', 'order': 6}), # ([0.01, 0.33, 0.14,
-0.31], 7, {'field': 'test_2', 'order': 7}), # ([0.71, 0.75, 0.91, 0.82], 8,
-{'field': 'test_3', 'order': 8}), # ([0.75, 0.44, 0.38, 0.75], 9, {'field':
-'test_1', 'order': 9})]) # print(ids) # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9] ``` ###
-Query ```python collection.query(vector=[0.36, 0.43, 0.56, 0.12], k=10) ```
-(array([ 2, 9, 1, 4, 6, 5, 10, 7, 8, 3]), array([1. , 0.92355633, 0.86097705,
-0.85727406, 0.81551266, 0.813797 , 0.78595245, 0.7741583 , 0.6871773 ,
-0.34695023])) ```python print(collection.query_report_) ``` * - MOST RECENT
-QUERY REPORT - | - Collection Shape: (10, 4) | - Query Time: 0.20518 s | -
-Query Distance: cosine | - Query K: 10 | - Top 10 Results ID: [ 2 9 1 4 6 5 10
-7 8 3] | - Top 10 Results Similarity: [1. 0.92355633 0.86097705 0.85727406
-0.81551266 0.813797 0.78595245 0.7741583 0.6871773 0.34695023] * - END OF
-REPORT - ### Use Filter ```python import operator from
-min_vec.structures.filter import Filter, FieldCondition, MatchField,
-IDCondition, MatchID collection.query( vector=[0.36, 0.43, 0.56, 0.12], k=10,
-query_filter=Filter( must=[ FieldCondition(key='field', matcher=MatchField
-('test_1')), # Support for filtering fields ], any=[ FieldCondition
-(key='order', matcher=MatchField(8, comparator=operator.ge)), IDCondition
-(MatchID([1, 2, 3, 4, 5])), # Support for filtering IDs ] ) ) print
+data management. MinVectorDB focuses on achieving 100% recall, prioritizing
+recall accuracy over high-speed search performance. This approach ensures that
+users can reliably retrieve all relevant vector data, making MinVectorDB
+particularly suitable for applications that require responses within hundreds
+of milliseconds. - [x] **Now supports HTTP API and Python local code API.** -
+[X] **Now supports Docker deployment.** - [X] **Now supports vector id and
+field filtering.** - [X] **Now supports transaction management; if a commit
+fails, it will automatically roll back.** ## Install Client API package
+(Mandatory) ```shell pip install MinVectorDB ``` ## If you wish to use Docker
+(Optional) ```shell docker pull birchkwok/minvectordb:latest ``` ## Qucik Start
+```python import min_vec print("MinVectorDB version is: ", min_vec.__version__)
+``` MinVectorDB version is: 0.3.3 ## Initialize Database MinVectorDB now
+supports HTTP API and Python local code API. The HTTP API mode requires
+starting an HTTP server beforehand. You have two options: - start directly. For
+direct startup, the default port is 7637. You can run the following command in
+the terminal to start the service: ```shell min_vec run --host localhost --port
+7637 ``` - within Docker In Docker, You can run the following command in the
+terminal to start the service: ```shell docker run -p 7637:7637 birchkwok/
+minvectordb:latest ``` ```python from min_vec import MinVectorDB # This method
+is for the Python local code API, recommended only for CI/CD testing or single-
+user local use. # Specify database root directory my_db = MinVectorDB
+('my_vec_db') # Judgment condition, root_path does not start with http or https
+# or # Use the HTTP API mode, it is suitable for use in production
+environments. my_db = MinVectorDB("http://localhost:7637") ``` ```python from
+min_vec import MinVectorDB # For direct startup my_db = MinVectorDB("http://
+localhost:7637") ``` ### create a collection ```python collection =
+my_db.require_collection("test_collection", 4, drop_if_exists=True,
+scaler_bits=8) ``` ### Add vectors When inserting vectors, collection requires
+manually running the `commit` function or inserting within the `insert_session`
+function context manager, which will run the `commit` function in the
+background. ```python with collection.insert_session(): id =
+collection.add_item(vector=[0.01, 0.34, 0.74, 0.31], id=1, field={'field':
+'test_1', 'order': 0}) # id = 0 id = collection.add_item(vector=[0.36, 0.43,
+0.56, 0.12], id=2, field={'field': 'test_1', 'order': 1}) # id = 1 id =
+collection.add_item(vector=[0.03, 0.04, 0.10, 0.51], id=3, field={'field':
+'test_2', 'order': 2}) # id = 2 id = collection.add_item(vector=[0.11, 0.44,
+0.23, 0.24], id=4, field={'field': 'test_2', 'order': 3}) # id = 3 id =
+collection.add_item(vector=[0.91, 0.43, 0.44, 0.67], id=5, field={'field':
+'test_2', 'order': 4}) # id = 4 id = collection.add_item(vector=[0.92, 0.12,
+0.56, 0.19], id=6, field={'field': 'test_3', 'order': 5}) # id = 5 id =
+collection.add_item(vector=[0.18, 0.34, 0.56, 0.71], id=7, field={'field':
+'test_1', 'order': 6}) # id = 6 id = collection.add_item(vector=[0.01, 0.33,
+0.14, 0.31], id=8, field={'field': 'test_2', 'order': 7}) # id = 7 id =
+collection.add_item(vector=[0.71, 0.75, 0.91, 0.82], id=9, field={'field':
+'test_3', 'order': 8}) # id = 8 id = collection.add_item(vector=[0.75, 0.44,
+0.38, 0.75], id=10, field={'field': 'test_1', 'order': 9}) # id = 9 # If you do
+not use the insert_session function, you need to manually call the commit
+function to submit the data # collection.commit() ``` ```python # or use the
+bulk_add_items function # with collection.insert_session(): # ids =
+collection.bulk_add_items([([0.01, 0.34, 0.74, 0.31], 0, {'field': 'test_1',
+'order': 0}), # ([0.36, 0.43, 0.56, 0.12], 1, {'field': 'test_1', 'order': 1}),
+# ([0.03, 0.04, 0.10, 0.51], 2, {'field': 'test_2', 'order': 2}), # ([0.11,
+0.44, 0.23, 0.24], 3, {'field': 'test_2', 'order': 3}), # ([0.91, 0.43, 0.44,
+0.67], 4, {'field': 'test_2', 'order': 4}), # ([0.92, 0.12, 0.56, 0.19], 5,
+{'field': 'test_3', 'order': 5}), # ([0.18, 0.34, 0.56, 0.71], 6, {'field':
+'test_1', 'order': 6}), # ([0.01, 0.33, 0.14, 0.31], 7, {'field': 'test_2',
+'order': 7}), # ([0.71, 0.75, 0.91, 0.82], 8, {'field': 'test_3', 'order': 8}),
+# ([0.75, 0.44, 0.38, 0.75], 9, {'field': 'test_1', 'order': 9})]) # print(ids)
+# [0, 1, 2, 3, 4, 5, 6, 7, 8, 9] ``` ### Query ```python collection.query
+(vector=[0.36, 0.43, 0.56, 0.12], k=10) ``` (array([ 2, 9, 1, 4, 6, 5, 10, 7,
+8, 3]), array([1. , 0.92355633, 0.86097705, 0.85727406, 0.81551266, 0.813797 ,
+0.78595245, 0.7741583 , 0.6871773 , 0.34695023])) ```python print
 (collection.query_report_) ``` * - MOST RECENT QUERY REPORT - | - Collection
-Shape: (10, 4) | - Query Time: 0.11985 s | - Query Distance: cosine | - Query
-K: 10 | - Top 10 Results ID: [ 2 1 4 5 10 3] | - Top 10 Results Similarity: [1.
-0.86097705 0.85727406 0.813797 0.78595245 0.34695023] * - END OF REPORT - ###
-Drop a collection ```python print("Collection list before dropping:",
-my_db.show_collections()) my_db.drop_collection("test_collection") print
-("Collection list after dropped:", my_db.show_collections()) ``` Collection
-list before dropping: ['test_collection'] Collection list after dropped: [] ##
-Drop the database ```python my_db.drop_database() my_db ``` MinVectorDB remote
-server at http://localhost:5403 does not exist. ```python my_db.database_exists
+Shape: (10, 4) | - Query Time: 0.15716 s | - Query Distance: cosine | - Query
+K: 10 | - Top 10 Results ID: [ 2 9 1 4 6 5 10 7 8 3] | - Top 10 Results
+Similarity: [1. 0.92355633 0.86097705 0.85727406 0.81551266 0.813797 0.78595245
+0.7741583 0.6871773 0.34695023] * - END OF REPORT - ### Use Filter ```python
+import operator from min_vec.core_components.filter import Filter,
+FieldCondition, MatchField, IDCondition, MatchID collection.query( vector=
+[0.36, 0.43, 0.56, 0.12], k=10, query_filter=Filter( must=[ FieldCondition
+(key='field', matcher=MatchField('test_1')), # Support for filtering fields ],
+any=[ FieldCondition(key='order', matcher=MatchField(8,
+comparator=operator.ge)), IDCondition(MatchID([1, 2, 3, 4, 5])), # Support for
+filtering IDs ], must_not=[ IDCondition(MatchID([8])), FieldCondition
+(key='order', matcher=MatchField(8, comparator=operator.ge)), ] ) ) print
+(collection.query_report_) ``` * - MOST RECENT QUERY REPORT - | - Collection
+Shape: (10, 4) | - Query Time: 0.09065 s | - Query Distance: cosine | - Query
+K: 10 | - Top 10 Results ID: [2 1] | - Top 10 Results Similarity: [1.
+0.86097705] * - END OF REPORT - ### Drop a collection ```python print
+("Collection list before dropping:", my_db.show_collections()) status =
+my_db.drop_collection("test_collection") print("Collection list after dropped:
+", my_db.show_collections()) ``` Collection list before dropping:
+['test_collection'] {'status': 'success', 'params': {'collection_name':
+'test_collection', 'exists': False}} Collection list after dropped: [] ## Drop
+the database ```python my_db.drop_database() my_db ``` MinVectorDB remote
+server at http://localhost:7637 does not exist. ```python my_db.database_exists
 () ``` {'status': 'success', 'params': {'exists': False}} ## What's Next -
 [Collection's operations](https://github.com/BirchKwok/MinVectorDB/blob/main/
 tutorials/collections.ipynb) - [Add vectors to collection](https://github.com/
 BirchKwok/MinVectorDB/blob/main/tutorials/add_vectors.ipynb) - [Using different
 indexing methods](https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/
 index_mode.ipynb) - [Using different distance metric functions](https://
 github.com/BirchKwok/MinVectorDB/blob/main/tutorials/distance.ipynb) -
```

### Comparing `minvectordb-0.3.2/README.md` & `minvectordb-0.3.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 <div align="center">
   <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB" style="max-width: 20%; height: auto;"></a>
   <h3>A pure Python-implemented, lightweight, server-optional, multi-end compatible, vector database deployable locally or remotely.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/l/MinVectorDB" alt="PyPI - License"></a>
-    <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml/badge.svg" alt="Python package"></a>
+    <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-tests.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-tests.yml/badge.svg" alt="Python testing"></a>
+    <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/docker-tests.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/docker-tests.yml/badge.svg" alt="Docker build"></a>
   </p>
 </div>
 
-⚡ **Serverless, simple parameters, simple API.**
+⚡ **Server-optional, simple parameters, simple API.**
 
 ⚡ **Fast, memory-efficient, easily scales to millions of vectors.**
 
 ⚡ **Supports cosine similarity and L2 distance, uses FLAT for exhaustive search or IVF-FLAT for inverted indexing.**
 
 ⚡ **Friendly caching technology stores recently queried vectors for accelerated access.**
 
 ⚡ **Based on a generic Python software stack, platform-independent, highly versatile.**
 
 > **WARNING**: MinVectorDB is actively being updated, and API backward compatibility is not guaranteed. You should use version numbers as a strong constraint during deployment to avoid unnecessary feature conflicts and errors.
 > **Although our goal is to enable brute force search or inverted indexing on billion-scale vectors, we currently still recommend using it on a scale of millions of vectors or less for the best experience.**
 
-*MinVectorDB* is a vector database implemented purely in Python, designed to be lightweight, serverless, and easy to deploy locally. It offers straightforward and clear Python APIs, aiming to lower the entry barrier for using vector databases. In response to user needs and to enhance its practicality, we are planning to introduce new features, including but not limited to:
+*MinVectorDB* is a vector database implemented purely in Python, designed to be lightweight, server-optional, and easy to deploy locally or remotely. It offers straightforward and clear Python APIs, aiming to lower the entry barrier for using vector databases. In response to user needs and to enhance its practicality, we are planning to introduce new features, including but not limited to:
 
 - **Optimizing Global Search Performance**: We are focusing on algorithm and data structure enhancements to speed up searches across the database, enabling faster retrieval of vector data.
 - **Enhancing Cluster Search with Inverted Indexes**: Utilizing inverted index technology, we aim to refine the cluster search process for better search efficiency and precision.
 - **Refining Clustering Algorithms**: By improving our clustering algorithms, we intend to offer more precise and efficient data clustering to support complex queries.
 - **Facilitating Vector Modifications and Deletions**: We will introduce features to modify and delete vectors, allowing for more flexible data management.
-- **Implementing Rollback Strategies**: To increase database robustness and data security, rollback strategies will be added, helping users recover from incorrect operations or system failures easily.
 
 MinVectorDB focuses on achieving 100% recall, prioritizing recall accuracy over high-speed search performance. This approach ensures that users can reliably retrieve all relevant vector data, making MinVectorDB particularly suitable for applications that require responses within hundreds of milliseconds.
 
-While the project has not yet been benchmarked against other systems, we believe these planned features will significantly enhance MinVectorDB's capabilities in managing and retrieving vector data, addressing a wide range of user needs.
+- [x] **Now supports HTTP API and Python local code API.**
+- [X] **Now supports Docker deployment.**
+- [X] **Now supports vector id and field filtering.**
+- [X] **Now supports transaction management; if a commit fails, it will automatically roll back.**
 
 ## Install Client API package (Mandatory)
 
 ```shell
 pip install MinVectorDB
 ```
 
@@ -50,58 +53,54 @@
 
 
 ```python
 import min_vec
 print("MinVectorDB version is: ", min_vec.__version__)
 ```
 
-    MinVectorDB version is:  0.3.2
+    MinVectorDB version is:  0.3.3
 
 
 ## Initialize Database
 
 MinVectorDB now supports HTTP API and Python local code API. 
 
 
 The HTTP API mode requires starting an HTTP server beforehand. You have two options: 
 - start directly.
   
   For direct startup, the default port is 7637. You can run the following command in the terminal to start the service:
 ```shell
-min_vec run --host 127.0.0.1 --port 7637
+min_vec run --host localhost --port 7637
 ```
 
 - within Docker
   
-  In Docker, the default port is 5403. You can run the following command in the terminal to start the service:
+  In Docker, You can run the following command in the terminal to start the service:
 ```shell
-docker run -p 5403:7637 birchkwok/minvectordb:latest
+docker run -p 7637:7637 birchkwok/minvectordb:latest
 ```
 
 ```python
 from min_vec import MinVectorDB
 
 # This method is for the Python local code API, recommended only for CI/CD testing or single-user local use.
 # Specify database root directory
 my_db = MinVectorDB('my_vec_db')  # Judgment condition, root_path does not start with http or https
 # or
 # Use the HTTP API mode, it is suitable for use in production environments.
-# For direct startup
-my_db = MinVectorDB("http://127.0.0.1:7637")
-
-# within Docker
-my_db = MinVectorDB("http://127.0.0.1:5403")
+my_db = MinVectorDB("http://localhost:7637")
 ```
 
 
 ```python
 from min_vec import MinVectorDB
 
 # For direct startup
-my_db = MinVectorDB("http://localhost:5403")
+my_db = MinVectorDB("http://localhost:7637")
 ```
 
 ### create a collection
 
 
 ```python
 collection = my_db.require_collection("test_collection", 4, drop_if_exists=True, scaler_bits=8)
@@ -166,15 +165,15 @@
 ```python
 print(collection.query_report_)
 ```
 
     
     * - MOST RECENT QUERY REPORT -
     | - Collection Shape: (10, 4)
-    | - Query Time: 0.20518 s
+    | - Query Time: 0.15716 s
     | - Query Distance: cosine
     | - Query K: 10
     | - Top 10 Results ID: [ 2  9  1  4  6  5 10  7  8  3]
     | - Top 10 Results Similarity: [1.         0.92355633 0.86097705 0.85727406 0.81551266 0.813797
      0.78595245 0.7741583  0.6871773  0.34695023]
     * - END OF REPORT -
     
@@ -182,72 +181,76 @@
 
 ### Use Filter
 
 
 ```python
 import operator
 
-from min_vec.structures.filter import Filter, FieldCondition, MatchField, IDCondition, MatchID
+from min_vec.core_components.filter import Filter, FieldCondition, MatchField, IDCondition, MatchID
 
 
 collection.query(
     vector=[0.36, 0.43, 0.56, 0.12], 
     k=10, 
     query_filter=Filter(
         must=[
             FieldCondition(key='field', matcher=MatchField('test_1')),  # Support for filtering fields
         ], 
         any=[
-
             FieldCondition(key='order', matcher=MatchField(8, comparator=operator.ge)),
             IDCondition(MatchID([1, 2, 3, 4, 5])),  # Support for filtering IDs
+        ],
+        must_not=[
+            IDCondition(MatchID([8])), 
+            FieldCondition(key='order', matcher=MatchField(8, comparator=operator.ge)),
         ]
     )
 )
 
 print(collection.query_report_)
 ```
 
     
     * - MOST RECENT QUERY REPORT -
     | - Collection Shape: (10, 4)
-    | - Query Time: 0.11985 s
+    | - Query Time: 0.09065 s
     | - Query Distance: cosine
     | - Query K: 10
-    | - Top 10 Results ID: [ 2  1  4  5 10  3]
-    | - Top 10 Results Similarity: [1.         0.86097705 0.85727406 0.813797   0.78595245 0.34695023]
+    | - Top 10 Results ID: [2 1]
+    | - Top 10 Results Similarity: [1.         0.86097705]
     * - END OF REPORT -
     
 
 
 ### Drop a collection
 
 
 ```python
 print("Collection list before dropping:", my_db.show_collections())
-my_db.drop_collection("test_collection")
+status = my_db.drop_collection("test_collection")
 print("Collection list after dropped:", my_db.show_collections())
 ```
 
     Collection list before dropping: ['test_collection']
+    {'status': 'success', 'params': {'collection_name': 'test_collection', 'exists': False}}
     Collection list after dropped: []
 
 
 ## Drop the database
 
 
 ```python
 my_db.drop_database()
 my_db
 ```
 
 
 
 
-    MinVectorDB remote server at http://localhost:5403 does not exist.
+    MinVectorDB remote server at http://localhost:7637 does not exist.
 
 
 
 
 ```python
 my_db.database_exists()
 ```
```

#### html2text {}

```diff
@@ -1,123 +1,123 @@
                                  _[_M_i_n_V_e_c_t_o_r_D_B_]
     ******** AA ppuurree PPyytthhoonn--iimmpplleemmeenntteedd,, lliigghhttwweeiigghhtt,, sseerrvveerr--ooppttiioonnaall,, mmuullttii--eenndd
        ccoommppaattiibbllee,, vveeccttoorr ddaattaabbaassee ddeeppllooyyaabbllee llooccaallllyy oorr rreemmootteellyy.. ********
-     _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _p_a_c_k_a_g_e_]
-â¡ **Serverless, simple parameters, simple API.** â¡ **Fast, memory-
+ _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _t_e_s_t_i_n_g_]_[_D_o_c_k_e_r
+                                    _b_u_i_l_d_]
+â¡ **Server-optional, simple parameters, simple API.** â¡ **Fast, memory-
 efficient, easily scales to millions of vectors.** â¡ **Supports cosine
 similarity and L2 distance, uses FLAT for exhaustive search or IVF-FLAT for
 inverted indexing.** â¡ **Friendly caching technology stores recently queried
 vectors for accelerated access.** â¡ **Based on a generic Python software
 stack, platform-independent, highly versatile.** > **WARNING**: MinVectorDB is
 actively being updated, and API backward compatibility is not guaranteed. You
 should use version numbers as a strong constraint during deployment to avoid
 unnecessary feature conflicts and errors. > **Although our goal is to enable
 brute force search or inverted indexing on billion-scale vectors, we currently
 still recommend using it on a scale of millions of vectors or less for the best
 experience.** *MinVectorDB* is a vector database implemented purely in Python,
-designed to be lightweight, serverless, and easy to deploy locally. It offers
-straightforward and clear Python APIs, aiming to lower the entry barrier for
-using vector databases. In response to user needs and to enhance its
-practicality, we are planning to introduce new features, including but not
-limited to: - **Optimizing Global Search Performance**: We are focusing on
-algorithm and data structure enhancements to speed up searches across the
+designed to be lightweight, server-optional, and easy to deploy locally or
+remotely. It offers straightforward and clear Python APIs, aiming to lower the
+entry barrier for using vector databases. In response to user needs and to
+enhance its practicality, we are planning to introduce new features, including
+but not limited to: - **Optimizing Global Search Performance**: We are focusing
+on algorithm and data structure enhancements to speed up searches across the
 database, enabling faster retrieval of vector data. - **Enhancing Cluster
 Search with Inverted Indexes**: Utilizing inverted index technology, we aim to
 refine the cluster search process for better search efficiency and precision. -
 **Refining Clustering Algorithms**: By improving our clustering algorithms, we
 intend to offer more precise and efficient data clustering to support complex
 queries. - **Facilitating Vector Modifications and Deletions**: We will
 introduce features to modify and delete vectors, allowing for more flexible
-data management. - **Implementing Rollback Strategies**: To increase database
-robustness and data security, rollback strategies will be added, helping users
-recover from incorrect operations or system failures easily. MinVectorDB
-focuses on achieving 100% recall, prioritizing recall accuracy over high-speed
-search performance. This approach ensures that users can reliably retrieve all
-relevant vector data, making MinVectorDB particularly suitable for applications
-that require responses within hundreds of milliseconds. While the project has
-not yet been benchmarked against other systems, we believe these planned
-features will significantly enhance MinVectorDB's capabilities in managing and
-retrieving vector data, addressing a wide range of user needs. ## Install
-Client API package (Mandatory) ```shell pip install MinVectorDB ``` ## If you
-wish to use Docker (Optional) ```shell docker pull birchkwok/minvectordb:latest
-``` ## Qucik Start ```python import min_vec print("MinVectorDB version is: ",
-min_vec.__version__) ``` MinVectorDB version is: 0.3.2 ## Initialize Database
-MinVectorDB now supports HTTP API and Python local code API. The HTTP API mode
-requires starting an HTTP server beforehand. You have two options: - start
-directly. For direct startup, the default port is 7637. You can run the
-following command in the terminal to start the service: ```shell min_vec run --
-host 127.0.0.1 --port 7637 ``` - within Docker In Docker, the default port is
-5403. You can run the following command in the terminal to start the service:
-```shell docker run -p 5403:7637 birchkwok/minvectordb:latest ``` ```python
-from min_vec import MinVectorDB # This method is for the Python local code API,
-recommended only for CI/CD testing or single-user local use. # Specify database
-root directory my_db = MinVectorDB('my_vec_db') # Judgment condition, root_path
-does not start with http or https # or # Use the HTTP API mode, it is suitable
-for use in production environments. # For direct startup my_db = MinVectorDB
-("http://127.0.0.1:7637") # within Docker my_db = MinVectorDB("http://
-127.0.0.1:5403") ``` ```python from min_vec import MinVectorDB # For direct
-startup my_db = MinVectorDB("http://localhost:5403") ``` ### create a
-collection ```python collection = my_db.require_collection("test_collection",
-4, drop_if_exists=True, scaler_bits=8) ``` ### Add vectors When inserting
-vectors, collection requires manually running the `commit` function or
-inserting within the `insert_session` function context manager, which will run
-the `commit` function in the background. ```python with
-collection.insert_session(): id = collection.add_item(vector=[0.01, 0.34, 0.74,
-0.31], id=1, field={'field': 'test_1', 'order': 0}) # id = 0 id =
-collection.add_item(vector=[0.36, 0.43, 0.56, 0.12], id=2, field={'field':
-'test_1', 'order': 1}) # id = 1 id = collection.add_item(vector=[0.03, 0.04,
-0.10, 0.51], id=3, field={'field': 'test_2', 'order': 2}) # id = 2 id =
-collection.add_item(vector=[0.11, 0.44, 0.23, 0.24], id=4, field={'field':
-'test_2', 'order': 3}) # id = 3 id = collection.add_item(vector=[0.91, 0.43,
-0.44, 0.67], id=5, field={'field': 'test_2', 'order': 4}) # id = 4 id =
-collection.add_item(vector=[0.92, 0.12, 0.56, 0.19], id=6, field={'field':
-'test_3', 'order': 5}) # id = 5 id = collection.add_item(vector=[0.18, 0.34,
-0.56, 0.71], id=7, field={'field': 'test_1', 'order': 6}) # id = 6 id =
-collection.add_item(vector=[0.01, 0.33, 0.14, 0.31], id=8, field={'field':
-'test_2', 'order': 7}) # id = 7 id = collection.add_item(vector=[0.71, 0.75,
-0.91, 0.82], id=9, field={'field': 'test_3', 'order': 8}) # id = 8 id =
-collection.add_item(vector=[0.75, 0.44, 0.38, 0.75], id=10, field={'field':
-'test_1', 'order': 9}) # id = 9 # If you do not use the insert_session
-function, you need to manually call the commit function to submit the data #
-collection.commit() ``` ```python # or use the bulk_add_items function # with
-collection.insert_session(): # ids = collection.bulk_add_items([([0.01, 0.34,
-0.74, 0.31], 0, {'field': 'test_1', 'order': 0}), # ([0.36, 0.43, 0.56, 0.12],
-1, {'field': 'test_1', 'order': 1}), # ([0.03, 0.04, 0.10, 0.51], 2, {'field':
-'test_2', 'order': 2}), # ([0.11, 0.44, 0.23, 0.24], 3, {'field': 'test_2',
-'order': 3}), # ([0.91, 0.43, 0.44, 0.67], 4, {'field': 'test_2', 'order': 4}),
-# ([0.92, 0.12, 0.56, 0.19], 5, {'field': 'test_3', 'order': 5}), # ([0.18,
-0.34, 0.56, 0.71], 6, {'field': 'test_1', 'order': 6}), # ([0.01, 0.33, 0.14,
-0.31], 7, {'field': 'test_2', 'order': 7}), # ([0.71, 0.75, 0.91, 0.82], 8,
-{'field': 'test_3', 'order': 8}), # ([0.75, 0.44, 0.38, 0.75], 9, {'field':
-'test_1', 'order': 9})]) # print(ids) # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9] ``` ###
-Query ```python collection.query(vector=[0.36, 0.43, 0.56, 0.12], k=10) ```
-(array([ 2, 9, 1, 4, 6, 5, 10, 7, 8, 3]), array([1. , 0.92355633, 0.86097705,
-0.85727406, 0.81551266, 0.813797 , 0.78595245, 0.7741583 , 0.6871773 ,
-0.34695023])) ```python print(collection.query_report_) ``` * - MOST RECENT
-QUERY REPORT - | - Collection Shape: (10, 4) | - Query Time: 0.20518 s | -
-Query Distance: cosine | - Query K: 10 | - Top 10 Results ID: [ 2 9 1 4 6 5 10
-7 8 3] | - Top 10 Results Similarity: [1. 0.92355633 0.86097705 0.85727406
-0.81551266 0.813797 0.78595245 0.7741583 0.6871773 0.34695023] * - END OF
-REPORT - ### Use Filter ```python import operator from
-min_vec.structures.filter import Filter, FieldCondition, MatchField,
-IDCondition, MatchID collection.query( vector=[0.36, 0.43, 0.56, 0.12], k=10,
-query_filter=Filter( must=[ FieldCondition(key='field', matcher=MatchField
-('test_1')), # Support for filtering fields ], any=[ FieldCondition
-(key='order', matcher=MatchField(8, comparator=operator.ge)), IDCondition
-(MatchID([1, 2, 3, 4, 5])), # Support for filtering IDs ] ) ) print
+data management. MinVectorDB focuses on achieving 100% recall, prioritizing
+recall accuracy over high-speed search performance. This approach ensures that
+users can reliably retrieve all relevant vector data, making MinVectorDB
+particularly suitable for applications that require responses within hundreds
+of milliseconds. - [x] **Now supports HTTP API and Python local code API.** -
+[X] **Now supports Docker deployment.** - [X] **Now supports vector id and
+field filtering.** - [X] **Now supports transaction management; if a commit
+fails, it will automatically roll back.** ## Install Client API package
+(Mandatory) ```shell pip install MinVectorDB ``` ## If you wish to use Docker
+(Optional) ```shell docker pull birchkwok/minvectordb:latest ``` ## Qucik Start
+```python import min_vec print("MinVectorDB version is: ", min_vec.__version__)
+``` MinVectorDB version is: 0.3.3 ## Initialize Database MinVectorDB now
+supports HTTP API and Python local code API. The HTTP API mode requires
+starting an HTTP server beforehand. You have two options: - start directly. For
+direct startup, the default port is 7637. You can run the following command in
+the terminal to start the service: ```shell min_vec run --host localhost --port
+7637 ``` - within Docker In Docker, You can run the following command in the
+terminal to start the service: ```shell docker run -p 7637:7637 birchkwok/
+minvectordb:latest ``` ```python from min_vec import MinVectorDB # This method
+is for the Python local code API, recommended only for CI/CD testing or single-
+user local use. # Specify database root directory my_db = MinVectorDB
+('my_vec_db') # Judgment condition, root_path does not start with http or https
+# or # Use the HTTP API mode, it is suitable for use in production
+environments. my_db = MinVectorDB("http://localhost:7637") ``` ```python from
+min_vec import MinVectorDB # For direct startup my_db = MinVectorDB("http://
+localhost:7637") ``` ### create a collection ```python collection =
+my_db.require_collection("test_collection", 4, drop_if_exists=True,
+scaler_bits=8) ``` ### Add vectors When inserting vectors, collection requires
+manually running the `commit` function or inserting within the `insert_session`
+function context manager, which will run the `commit` function in the
+background. ```python with collection.insert_session(): id =
+collection.add_item(vector=[0.01, 0.34, 0.74, 0.31], id=1, field={'field':
+'test_1', 'order': 0}) # id = 0 id = collection.add_item(vector=[0.36, 0.43,
+0.56, 0.12], id=2, field={'field': 'test_1', 'order': 1}) # id = 1 id =
+collection.add_item(vector=[0.03, 0.04, 0.10, 0.51], id=3, field={'field':
+'test_2', 'order': 2}) # id = 2 id = collection.add_item(vector=[0.11, 0.44,
+0.23, 0.24], id=4, field={'field': 'test_2', 'order': 3}) # id = 3 id =
+collection.add_item(vector=[0.91, 0.43, 0.44, 0.67], id=5, field={'field':
+'test_2', 'order': 4}) # id = 4 id = collection.add_item(vector=[0.92, 0.12,
+0.56, 0.19], id=6, field={'field': 'test_3', 'order': 5}) # id = 5 id =
+collection.add_item(vector=[0.18, 0.34, 0.56, 0.71], id=7, field={'field':
+'test_1', 'order': 6}) # id = 6 id = collection.add_item(vector=[0.01, 0.33,
+0.14, 0.31], id=8, field={'field': 'test_2', 'order': 7}) # id = 7 id =
+collection.add_item(vector=[0.71, 0.75, 0.91, 0.82], id=9, field={'field':
+'test_3', 'order': 8}) # id = 8 id = collection.add_item(vector=[0.75, 0.44,
+0.38, 0.75], id=10, field={'field': 'test_1', 'order': 9}) # id = 9 # If you do
+not use the insert_session function, you need to manually call the commit
+function to submit the data # collection.commit() ``` ```python # or use the
+bulk_add_items function # with collection.insert_session(): # ids =
+collection.bulk_add_items([([0.01, 0.34, 0.74, 0.31], 0, {'field': 'test_1',
+'order': 0}), # ([0.36, 0.43, 0.56, 0.12], 1, {'field': 'test_1', 'order': 1}),
+# ([0.03, 0.04, 0.10, 0.51], 2, {'field': 'test_2', 'order': 2}), # ([0.11,
+0.44, 0.23, 0.24], 3, {'field': 'test_2', 'order': 3}), # ([0.91, 0.43, 0.44,
+0.67], 4, {'field': 'test_2', 'order': 4}), # ([0.92, 0.12, 0.56, 0.19], 5,
+{'field': 'test_3', 'order': 5}), # ([0.18, 0.34, 0.56, 0.71], 6, {'field':
+'test_1', 'order': 6}), # ([0.01, 0.33, 0.14, 0.31], 7, {'field': 'test_2',
+'order': 7}), # ([0.71, 0.75, 0.91, 0.82], 8, {'field': 'test_3', 'order': 8}),
+# ([0.75, 0.44, 0.38, 0.75], 9, {'field': 'test_1', 'order': 9})]) # print(ids)
+# [0, 1, 2, 3, 4, 5, 6, 7, 8, 9] ``` ### Query ```python collection.query
+(vector=[0.36, 0.43, 0.56, 0.12], k=10) ``` (array([ 2, 9, 1, 4, 6, 5, 10, 7,
+8, 3]), array([1. , 0.92355633, 0.86097705, 0.85727406, 0.81551266, 0.813797 ,
+0.78595245, 0.7741583 , 0.6871773 , 0.34695023])) ```python print
 (collection.query_report_) ``` * - MOST RECENT QUERY REPORT - | - Collection
-Shape: (10, 4) | - Query Time: 0.11985 s | - Query Distance: cosine | - Query
-K: 10 | - Top 10 Results ID: [ 2 1 4 5 10 3] | - Top 10 Results Similarity: [1.
-0.86097705 0.85727406 0.813797 0.78595245 0.34695023] * - END OF REPORT - ###
-Drop a collection ```python print("Collection list before dropping:",
-my_db.show_collections()) my_db.drop_collection("test_collection") print
-("Collection list after dropped:", my_db.show_collections()) ``` Collection
-list before dropping: ['test_collection'] Collection list after dropped: [] ##
-Drop the database ```python my_db.drop_database() my_db ``` MinVectorDB remote
-server at http://localhost:5403 does not exist. ```python my_db.database_exists
+Shape: (10, 4) | - Query Time: 0.15716 s | - Query Distance: cosine | - Query
+K: 10 | - Top 10 Results ID: [ 2 9 1 4 6 5 10 7 8 3] | - Top 10 Results
+Similarity: [1. 0.92355633 0.86097705 0.85727406 0.81551266 0.813797 0.78595245
+0.7741583 0.6871773 0.34695023] * - END OF REPORT - ### Use Filter ```python
+import operator from min_vec.core_components.filter import Filter,
+FieldCondition, MatchField, IDCondition, MatchID collection.query( vector=
+[0.36, 0.43, 0.56, 0.12], k=10, query_filter=Filter( must=[ FieldCondition
+(key='field', matcher=MatchField('test_1')), # Support for filtering fields ],
+any=[ FieldCondition(key='order', matcher=MatchField(8,
+comparator=operator.ge)), IDCondition(MatchID([1, 2, 3, 4, 5])), # Support for
+filtering IDs ], must_not=[ IDCondition(MatchID([8])), FieldCondition
+(key='order', matcher=MatchField(8, comparator=operator.ge)), ] ) ) print
+(collection.query_report_) ``` * - MOST RECENT QUERY REPORT - | - Collection
+Shape: (10, 4) | - Query Time: 0.09065 s | - Query Distance: cosine | - Query
+K: 10 | - Top 10 Results ID: [2 1] | - Top 10 Results Similarity: [1.
+0.86097705] * - END OF REPORT - ### Drop a collection ```python print
+("Collection list before dropping:", my_db.show_collections()) status =
+my_db.drop_collection("test_collection") print("Collection list after dropped:
+", my_db.show_collections()) ``` Collection list before dropping:
+['test_collection'] {'status': 'success', 'params': {'collection_name':
+'test_collection', 'exists': False}} Collection list after dropped: [] ## Drop
+the database ```python my_db.drop_database() my_db ``` MinVectorDB remote
+server at http://localhost:7637 does not exist. ```python my_db.database_exists
 () ``` {'status': 'success', 'params': {'exists': False}} ## What's Next -
 [Collection's operations](https://github.com/BirchKwok/MinVectorDB/blob/main/
 tutorials/collections.ipynb) - [Add vectors to collection](https://github.com/
 BirchKwok/MinVectorDB/blob/main/tutorials/add_vectors.ipynb) - [Using different
 indexing methods](https://github.com/BirchKwok/MinVectorDB/blob/main/tutorials/
 index_mode.ipynb) - [Using different distance metric functions](https://
 github.com/BirchKwok/MinVectorDB/blob/main/tutorials/distance.ipynb) -
```

### Comparing `minvectordb-0.3.2/min_vec/__init__.py` & `minvectordb-0.3.3/min_vec/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__ = '0.3.2'
+__version__ = '0.3.3'
 
 
 class MinVectorDB:
     """
     Create a MinVectorDB instance.
 
     Parameters:
```

### Comparing `minvectordb-0.3.2/min_vec/api/client_api.py` & `minvectordb-0.3.3/min_vec/api/client_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,86 @@
 import time
 from datetime import datetime
 from typing import Union, List, Tuple
 
+import msgpack
 import numpy as np
-import requests
+import httpx
 from spinesUtils.asserts import raise_if
+from tqdm import trange
 
-from min_vec.structures.filter import Filter
+from min_vec.core_components.filter import Filter
 from min_vec.api import config
-from min_vec.utils.utils import QueryVectorCache
+from min_vec.core_components.thread_safe_list import SafeList
+from min_vec.utils.utils import QueryResultsCache
 
 
 class ExecutionError(Exception):
     pass
 
 
+def raise_error_response(response):
+    """
+    Raise an error response.
+
+    Parameters:
+        response: The response from the server.
+
+    Raises:
+        ExecutionError: If the server returns an error.
+    """
+    try:
+        rj = response.json()
+        raise ExecutionError(rj)
+    except Exception as e:
+        print(e)
+        raise ExecutionError(response.text)
+
+
+def pack_data(data):
+    """
+    Pack the data.
+
+    Parameters:
+        data: The data to pack.
+
+    Returns:
+        bytes: The packed data.
+    """
+    packed_data = msgpack.packb(data, use_bin_type=True)
+    return packed_data
+
+
+def quantize_vector(vector):
+    """
+    Quantize the vector to 8 bits.
+
+    Parameters:
+        vector: The vector to quantize.
+
+    Returns:
+        (np.ndarray, min_vals, range_vals): The quantized vector, minimum values, and range values.
+    """
+    if isinstance(vector, list):
+        vector = np.array(vector)
+
+    epsilon = 1e-9
+    n_levels_minus_1 = 2 ** 8 - 1
+    max_val = np.max(vector, axis=0)
+    min_val = np.min(vector, axis=0)
+    range_val = max_val - min_val
+
+    quantized = ((vector - min_val) / (range_val + epsilon)) * n_levels_minus_1
+    quantized = np.clip(quantized, 0, n_levels_minus_1).astype(np.uint8)
+
+    return (quantized.tolist(),
+            min_val.tolist() if isinstance(min_val, np.ndarray) else min_val,
+            range_val.tolist() if isinstance(range_val, np.ndarray) else range_val)
+
+
 class Collection:
     def __init__(self, url, collection_name, **params):
         """
         Initialize the collection.
             .. versionadded:: 0.3.2
 
         Parameters:
@@ -36,35 +98,39 @@
                 - n_threads (int): The number of threads.
                 - warm_up (bool): Whether to warm up.
                 - drop_if_exists (bool): Whether to drop the collection if it exists.
         """
         self.IS_DELETED = False
         self._url = url
         self._collection_name = collection_name
+        self._session = httpx.Client(http2=True, timeout=120)
         self._init_params = params
 
         self.most_recent_query_report = {}
         self.query_report = {}
 
         self.COMMIT_FLAG = False
 
+        self._mesosphere_list = SafeList()
+
     def _get_commit_msg(self):
         """
         Get the commit message.
 
         Returns:
             str: The last commit time.
 
         Raises:
             ExecutionError: If the server returns an error.
         """
         url = f'{self._url}/get_commit_msg'
         data = {"collection_name": self._collection_name}
 
-        response = requests.post(url, json=data)
+        response = self._session.post(url, json=data)
+
         rj = response.json()
         if response.status_code == 200:
             if rj['params']['commit_msg'] is None:
                 return None
             return rj['params']['commit_msg']['last_commit_time']
         else:
             raise ExecutionError(rj)
@@ -84,231 +150,284 @@
         """
         url = f'{self._url}/update_commit_msg'
         data = {
             "collection_name": self._collection_name,
             "last_commit_time": last_commit_time,
         }
 
-        response = requests.post(url, json=data)
+        response = self._session.post(url, json=data)
 
         if response.status_code == 200:
             return response.json()
         else:
-            raise ExecutionError(response.json())
+            try:
+                rj = response.json()
+                raise ExecutionError(rj)
+            except Exception as e:
+                print(e)
+                raise ExecutionError(response.text)
 
     def _if_exists(self):
         """
         Check if the collection exists.
 
         Returns:
             bool: Whether the collection exists.
 
         Raises:
             ExecutionError: If the server returns an error.
         """
         url = f'{self._url}/is_collection_exists'
         data = {"collection_name": self._collection_name}
 
-        response = requests.post(url, json=data)
+        response = self._session.post(url, json=data)
 
         if response.status_code == 200:
             return response.json()['params']['exists']
         else:
-            raise ExecutionError(response.json())
+            raise_error_response(response)
 
-    def add_item(self, vector: Union[list[float], np.ndarray], id: int, field: dict):
+    def add_item(self, vector: Union[list[float], np.ndarray], id: int, field: Union[dict, None] = None):
         """
         Add an item to the collection.
             .. versionadded:: 0.3.2
 
         Parameters:
             vector (list[float], np.ndarray): The vector of the item.
             id (int): The ID of the item.
-            field (dict): The fields of the item.
+            field (dict, optional): The fields of the item.
 
         Returns:
-            int: The ID of the item.
+            int: The ID of the item. If delay_num is greater than 0, and the number of items added is less than delay_num,
+                the function will return None. Otherwise, the function will return the IDs of the items added.
 
         Raises:
             ValueError: If the collection has been deleted or does not exist.
             ExecutionError: If the server returns an error.
         """
-        raise_if(ValueError, self.IS_DELETED or not self._if_exists(),
-                 'The collection has been deleted or does not exist.')
+        delay_num = config.MVDB_DELAY_NUM
 
-        url = f'{self._url}/add_item'
-        data = {
-            "collection_name": self._collection_name,
-            "item": {
-                "vector": vector if isinstance(vector, list) else vector.tolist(),
-                "id": id,
-                "field": field
+        if delay_num == 0:
+            url = f'{self._url}/add_item'
+
+            headers = {'Content-Type': 'application/msgpack'}
+
+            data = {
+                "collection_name": self._collection_name,
+                "item": {
+                    "vector": vector if isinstance(vector, list) else vector.tolist(),
+                    "id": id if id is not None else None,
+                    "field": field if field is not None else {},
+                }
             }
-        }
-        response = requests.post(url, json=data)
 
-        if response.status_code == 200:
-            self.COMMIT_FLAG = False
-            return response.json()['params']['item']['id']
+            response = self._session.post(url, content=pack_data(data), headers=headers)
+
+            if response.status_code == 200:
+                self.COMMIT_FLAG = False
+                return response.json()['params']['item']['id']
+            else:
+                raise_error_response(response)
         else:
-            raise ExecutionError(response.json())
+            self._mesosphere_list.append({
+                "vector": vector if isinstance(vector, list) else vector.tolist(),
+                "id": id if id is not None else None,
+                "field": field if field is not None else {},
+            })
+
+            if len(self._mesosphere_list) == delay_num:
+                url = f'{self._url}/bulk_add_items'
+
+                headers = {'Content-Type': 'application/msgpack'}
+
+                data = {
+                    "collection_name": self._collection_name,
+                    "items": self._mesosphere_list
+                }
+
+                response = self._session.post(url, content=pack_data(data), headers=headers)
+
+                if response.status_code == 200:
+                    self.COMMIT_FLAG = False
+                    self._mesosphere_list = self._mesosphere_list[delay_num:]
+                else:
+                    raise_error_response(response)
+
+            return id
+
+    @staticmethod
+    def _check_bulk_add_items(vectors):
+        items = []
+        for vector in vectors:
+            raise_if(TypeError, not isinstance(vector, tuple), 'Each item must be a tuple of vector, '
+                                                               'ID, and fields(optional).')
+            vec_len = len(vector)
+
+            if vec_len == 3:
+                v1, v2, v3 = vector
+                items.append({
+                    "vector": v1.tolist() if isinstance(v1, np.ndarray) else v1,
+                    "id": v2,
+                    "field": v3,
+                })
+            elif vec_len == 2:
+                v1, v2 = vector
+                items.append({
+                    "vector": v1.tolist() if isinstance(v1, np.ndarray) else v1,
+                    "id": v2,
+                    "field": {},
+                })
+            else:
+                raise TypeError('Each item must be a tuple of vector, ID, and fields(optional).')
+
+        return items
 
     def bulk_add_items(
             self,
             vectors: List[Union[
                 Tuple[Union[List, Tuple, np.ndarray], int, dict],
-                Tuple[Union[List, Tuple, np.ndarray], int],
-                Tuple[Union[List, Tuple, np.ndarray]]
-            ]]
+                Tuple[Union[List, Tuple, np.ndarray], int]
+            ]],
+            batch_size: int = 1000,
+            enable_progress_bar: bool = True
     ):
         """
         Add multiple items to the collection.
             .. versionadded:: 0.3.2
 
         Parameters:
             vectors (List[Tuple[Union[List, Tuple, np.ndarray], int, dict]],
-            List[Tuple[Union[List, Tuple, np.ndarray], int]] , List[Tuple[Union[List, Tuple, np.ndarray]]]):
+            List[Tuple[Union[List, Tuple, np.ndarray], int]]):
                 The list of items to add. Each item is a tuple containing the vector, ID, and fields.
+            batch_size (int): The batch size. Default is 1000.
+            enable_progress_bar (bool): Whether to enable the progress bar. Default is True.
 
         Returns:
             dict: The response from the server.
 
         Raises:
             ValueError: If the collection has been deleted or does not exist.
             TypeError: If the vectors are not in the correct format.
             ExecutionError: If the server returns an error.
         """
-        raise_if(ValueError, self.IS_DELETED or not self._if_exists(),
-                 'The collection has been deleted or does not exist.')
-
-        items = []
-        for vector in vectors:
-            raise_if(TypeError, not isinstance(vector, tuple), 'Each item must be a tuple of vector, '
-                                                               'ID(optional), and fields(optional).')
-
-            if len(vector) == 3:
-                items.append({
-                    "vector": vector[0].tolist() if isinstance(vector[0], np.ndarray) else vector[0],
-                    "id": vector[1],
-                    "field": vector[2]
-                })
-            elif len(vector) == 2:
-                items.append({
-                    "vector": vector[0].tolist() if isinstance(vector[0], np.ndarray) else vector[0],
-                    "id": vector[1],
-                    "field": {}
-                })
-            else:
-                items.append({
-                    "vector": vector[0].tolist() if isinstance(vector[0], np.ndarray) else vector[0],
-                    "id": None,
-                    "field": {}
-                })
 
         url = f'{self._url}/bulk_add_items'
-        data = {
-            "collection_name": self._collection_name,
-            "items": items
-        }
+        total_batches = (len(vectors) + batch_size - 1) // batch_size
 
-        response = requests.post(url, json=data)
+        ids = []
 
-        if response.status_code == 200:
-            self.COMMIT_FLAG = False
-            return response.json()['params']['ids']
+        if enable_progress_bar:
+            iter_obj = trange(total_batches, desc='Adding items', unit='batch')
         else:
-            raise ExecutionError(response.json())
+            iter_obj = range(total_batches)
+
+        headers = {'Content-Type': 'application/msgpack'}
+
+        for i in iter_obj:
+            start = i * batch_size
+            end = (i + 1) * batch_size
+            items = vectors[start:end]
+
+            items_after_checking = self._check_bulk_add_items(items)
+
+            data = {
+                "collection_name": self._collection_name,
+                "items": items_after_checking
+            }
+            # Send request using session to keep the connection alive
+            response = self._session.post(url, content=pack_data(data), headers=headers)
+
+            if response.status_code == 200:
+                self.COMMIT_FLAG = False
+                ids.extend(response.json()['params']['ids'])
+            else:
+                raise_error_response(response)
+
+        return ids
+
+    def _rollback(self):
+        self._mesosphere_list = SafeList()
 
     def commit(self):
         """
         Commit the changes in the collection.
             .. versionadded:: 0.3.2
 
         Returns:
             dict: The response from the server.
 
         Raises:
             ExecutionError: If the server returns an error.
         """
         url = f'{self._url}/commit'
         data = {"collection_name": self._collection_name}
-        response = requests.post(url, json=data)
+
+        if self._mesosphere_list:
+            data["items"] = self._mesosphere_list
+
+        response = self._session.post(url, content=pack_data(data), headers={'Content-Type': 'application/msgpack'})
+
+        if self._mesosphere_list:
+            self._mesosphere_list = SafeList()
 
         if response.status_code == 200:
             self._update_commit_msg(datetime.now().strftime('%Y-%m-%d %H:%M:%S'))
             return response.json()
         else:
-            raise ExecutionError(response.json())
+            raise_error_response(response)
 
     def insert_session(self):
         """
         Start an insert session.
             .. versionadded:: 0.3.2
         """
         from min_vec.execution_layer.session import DatabaseSession
 
         return DatabaseSession(self)
 
-    @QueryVectorCache(config.MVDB_QUERY_CACHE_SIZE)
+    @QueryResultsCache(config.MVDB_QUERY_CACHE_SIZE)
     def _query(self, vector: Union[list[float], np.ndarray], k: int = 10, distance: str = 'cosine',
-               query_filter: Union[Filter, None] = None, return_similarity: bool = True, **kwargs):
+               query_filter: Union[Filter, None] = None, **kwargs):
         """
         Query the collection.
             .. versionadded:: 0.3.2
 
         Parameters:
             vector (list[float] or np.ndarray): The query vector.
             k (int): The number of results to return. Default is 10.
             distance (str): The distance metric. Default is 'cosine', it can be 'cosine' or 'L2'.
             query_filter (Filter, optional): The field filter to apply to the query, must be a Filter object.
-            return_similarity (bool): Whether to return the similarity. Default is True.
 
         Returns:
             Tuple: The indices and similarity scores of the top k nearest vectors.
 
         Raises:
             ValueError: If the collection has been deleted or does not exist.
             ExecutionError: If the server returns an error.
         """
-        raise_if(ValueError, self.IS_DELETED or not self._if_exists(),
-                 'The collection has been deleted or does not exist.')
-
         url = f'{self._url}/query'
 
         if query_filter is not None:
             raise_if(TypeError, not isinstance(query_filter, Filter), 'The query filter must be a Filter object.')
             query_filter = query_filter.to_dict()
 
         data = {
             "collection_name": self._collection_name,
             "vector": vector if isinstance(vector, list) else vector.tolist(),
             "k": k,
             'distance': distance,
             "query_filter": query_filter,
-            "return_similarity": return_similarity
+            "return_similarity": True
         }
-        response = requests.post(url, json=data)
+        response = self._session.post(url, json=data)
 
         if response.status_code == 200:
-            rjson = response.json()
-            self.most_recent_query_report['Collection Shape'] = self.shape
-            self.most_recent_query_report['Query Time'] = rjson['params']['items']['query time']
-            self.most_recent_query_report['Query Distance'] = rjson['params']['items']['distance']
-            self.most_recent_query_report['Query K'] = k
-
-            ids, scores = np.array(rjson['params']['items']['ids']), np.array(rjson['params']['items']['scores'])
-
-            if ids is not None:
-                self.most_recent_query_report[f'Top {k} Results ID'] = ids
-                if return_similarity:
-                    self.most_recent_query_report[f'Top {k} Results Similarity'] = scores
-
-            return ids, scores
+            return response.json()
         else:
-            raise ExecutionError(response.json())
+            raise_error_response(response)
 
     def query(
             self, vector: Union[list[float], np.ndarray], k: int = 10, distance: str = 'cosine',
             query_filter: Union[Filter, None] = None, return_similarity: bool = True
     ):
         """
         Query the collection.
@@ -324,25 +443,47 @@
         Returns:
             Tuple: The indices and similarity scores of the top k nearest vectors.
 
         Raises:
             ValueError: If the collection has been deleted or does not exist.
             ExecutionError: If the server returns an error.
         """
+        self.most_recent_query_report = {}
+
         tik = time.time()
         if self._init_params['use_cache']:
-            res = self._query(vector, k, distance, query_filter, return_similarity)
+            rjson = self._query(vector=vector, k=k, distance=distance,
+                                query_filter=query_filter, return_similarity=return_similarity)
         else:
-            res = self._query(vector, k, distance, query_filter, return_similarity=return_similarity, now=time.time())
+            rjson = self._query(vector=vector, k=k, distance=distance, query_filter=query_filter,
+                                return_similarity=return_similarity, now=time.time())
 
         tok = time.time()
 
+        self.most_recent_query_report['Collection Shape'] = self.shape
+        self.most_recent_query_report['Query Time'] = rjson['params']['items']['query time']
+        self.most_recent_query_report['Query Distance'] = rjson['params']['items']['distance']
+        self.most_recent_query_report['Query K'] = k
+
+        ids, scores = np.array(rjson['params']['items']['ids']), np.array(rjson['params']['items']['scores'])
+
+        if ids is not None:
+            self.most_recent_query_report[f'Top {k} Results ID'] = ids
+            if return_similarity:
+                self.most_recent_query_report[f'Top {k} Results Similarity'] = scores
+            else:
+                if f'Top {k} Results Similarity' in self.most_recent_query_report:
+                    del self.most_recent_query_report[f'Top {k} Results Similarity']
+
         self.most_recent_query_report['Query Time'] = f"{tok - tik :>.5f} s"
 
-        return res
+        if return_similarity:
+            return ids, scores
+
+        return ids, None
 
     @property
     def shape(self):
         """
         Get the shape of the collection.
             .. versionadded:: 0.3.2
 
@@ -350,24 +491,24 @@
             Tuple: The shape of the collection.
 
         Raises:
             ExecutionError: If the server returns an error.
         """
         url = f'{self._url}/collection_shape'
         data = {"collection_name": self._collection_name}
-        response = requests.post(url, json=data)
+        response = self._session.post(url, json=data)
 
         if response.status_code == 200:
             return tuple(response.json()['params']['shape'])
         else:
             rj = response.json()
             if 'error' in rj and rj['error'] == f"Collection '{self._collection_name}' does not exist.":
                 return 0, self._init_params['dim']
             else:
-                raise ExecutionError(response.json())
+                raise_error_response(response)
 
     @property
     def query_report_(self):
         """
         Get the query report of the collection.
             .. versionadded:: 0.3.2
 
@@ -411,18 +552,18 @@
         Raises:
             ExecutionError: If the server returns an error.
         """
         name = "Collection"
 
         url = f'{self._url}/is_collection_exists'
         data = {"collection_name": self._collection_name}
-        response = requests.post(url, json=data)
+        response = self._session.post(url, json=data)
 
         if response.status_code != 200:
-            raise ExecutionError(response.json())
+            raise_error_response(response)
 
         is_exists = response.json()['params']['exists']
 
         last_commit_time = self._get_commit_msg()
         db_report = {f'{name.upper()} STATUS REPORT': {
             f'{name} shape': (0, self._init_params['dim']) if self.IS_DELETED else self.shape,
             f'{name} last_commit_time': last_commit_time,
@@ -450,24 +591,35 @@
             ConnectionError: If the server cannot be connected to.
         """
 
         raise_if(TypeError, not isinstance(url, str), 'The URL must be a string.')
         raise_if(ValueError, not url.startswith('http://') or url.startswith('https://'),
                  'The URL must start with "http://" or "https://".')
 
+        self._session = httpx.Client()
+
         if url.endswith('/'):
             self.url = url[:-1]
         else:
             self.url = url
 
         try:
-            if requests.get(url).json() != {'status': 'success', 'message': 'MinVectorDB HTTP API'}:
+            response = self._session.get(url)
+            if response.status_code != 200:
                 raise ConnectionError(f'Failed to connect to the server at {url}.')
 
-        except requests.exceptions.ConnectionError:
+            try:
+                rj = response.json()
+                if rj != {'status': 'success', 'message': 'MinVectorDB HTTP API'}:
+                    raise ConnectionError(f'Failed to connect to the server at {url}.')
+            except Exception as e:
+                print(e)
+                raise ConnectionError(f'Failed to connect to the server at {url}.')
+
+        except httpx.RequestError:
             raise ConnectionError(f'Failed to connect to the server at {url}.')
 
     def require_collection(
             self,
             collection: str,
             dim: int = None,
             n_clusters: int = 16,
@@ -521,18 +673,23 @@
             "scaler_bits": scaler_bits,
             "n_threads": n_threads,
             "warm_up": warm_up,
             "drop_if_exists": drop_if_exists
         }
 
         try:
-            requests.post(url, json=data)
-            del data['collection_name']
-            return Collection(self.url, collection, **data)
-        except requests.exceptions.ConnectionError:
+            response = self._session.post(url, json=data)
+            if response.status_code == 200:
+                del data['collection_name']
+                collection = Collection(self.url, collection, **data)
+                collection._query.clear_cache()
+                return collection
+            else:
+                raise_error_response(response)
+        except httpx.RequestError:
             raise ConnectionError(f'Failed to connect to the server at {url}.')
 
     def drop_collection(self, collection: str):
         """
         Drop a collection.
             .. versionadded:: 0.3.2
 
@@ -543,20 +700,24 @@
             dict: The response from the server.
 
         Raises:
             ExecutionError: If the server returns an error.
         """
         url = f'{self.url}/drop_collection'
         data = {"collection_name": collection}
-        response = requests.post(url, json=data)
+        response = self._session.post(url, json=data)
 
-        if response.status_code == 200:
-            return response.json()
-        else:
-            raise ExecutionError(response.json())
+        try:
+            collection = self.get_collection(collection)
+
+            if response.status_code == 200:
+                collection._query.clear_cache()
+                return response.json()
+        except ExecutionError:
+            pass
 
     def drop_database(self):
         """
         Drop the database.
             .. versionadded:: 0.3.2
 
         Returns:
@@ -565,58 +726,58 @@
         Raises:
             ExecutionError: If the server returns an error.
         """
         if not self.database_exists()['params']['exists']:
             return {'status': 'success', 'message': 'The database does not exist.'}
 
         url = f'{self.url}/drop_database'
-        response = requests.get(url)
+        response = self._session.get(url)
 
         if response.status_code == 200:
             return response.json()
         else:
-            raise ExecutionError(response.text)
+            raise_error_response(response)
 
     def database_exists(self):
         """
         Check if the database exists.
             .. versionadded:: 0.3.2
 
         Returns:
             dict: The response from the server.
 
         Raises:
             ExecutionError: If the server returns an error.
         """
         url = f'{self.url}/database_exists'
-        response = requests.get(url)
+        response = self._session.get(url)
 
         if response.status_code == 200:
             return response.json()
         else:
-            raise ExecutionError(response.json())
+            raise_error_response(response)
 
     def show_collections(self):
         """
         Show all collections in the database.
             .. versionadded:: 0.3.2
 
         Returns:
             List: The list of collections.
 
         Raises:
             ExecutionError: If the server returns an error.
         """
         url = f'{self.url}/show_collections'
-        response = requests.get(url)
+        response = self._session.get(url)
 
         if response.status_code == 200:
             return response.json()['params']['collections']
         else:
-            raise ExecutionError(response.json())
+            raise_error_response(response)
 
     def set_environment(self, env: dict):
         """
         Set the environment variables.
             .. versionadded:: 0.3.2
 
         Parameters:
@@ -643,39 +804,39 @@
 
         data = {}
         for key in env:
             if key in env_list:
                 raise_if(TypeError, not isinstance(env[key], str), f'The value of {key} must be a string.')
                 data[key] = env[key]
 
-        response = requests.post(url, json=data)
+        response = self._session.post(url, json=data)
 
         if response.status_code == 200:
             return response.json()
         else:
-            raise ExecutionError(response.json())
+            raise_error_response(response)
 
     def get_environment(self):
         """
         Get the environment variables.
             .. versionadded:: 0.3.2
 
         Returns:
             dict: The response from the server.
 
         Raises:
             ExecutionError: If the server returns an error.
         """
         url = f'{self.url}/get_environment'
-        response = requests.get(url)
+        response = self._session.get(url)
 
         if response.status_code == 200:
             return response.json()
         else:
-            raise ExecutionError(response.json())
+            raise_error_response(response)
 
     def get_collection(self, collection: str):
         """
         Get a collection.
             .. versionadded:: 0.3.2
 
         Parameters:
@@ -685,24 +846,24 @@
             Collection: The collection object.
 
         Raises:
             ExecutionError: If the server returns an error.
         """
         url = f'{self.url}/is_collection_exists'
         data = {"collection_name": collection}
-        response = requests.post(url, json=data)
+        response = self._session.post(url, json=data)
 
         if response.status_code == 200 and response.json()['params']['exists']:
             url = f'{self.url}/get_collection_config'
             data = {"collection_name": collection}
-            response = requests.post(url, json=data)
+            response = self._session.post(url, json=data)
 
             return Collection(self.url, collection, **response.json()['params']['config'])
         else:
-            raise ExecutionError(response.json())
+            raise_error_response(response)
 
     def __repr__(self):
         if self.database_exists()['params']['exists']:
             return f'MinVectorDB HTTP Client connected to {self.url}.'
         else:
             return f'MinVectorDB remote server at {self.url} does not exist.'
```

### Comparing `minvectordb-0.3.2/min_vec/api/high_level.py` & `minvectordb-0.3.3/min_vec/api/high_level.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-"""high_level.py - The MinVectorDB API."""
 import json
 from pathlib import Path
 from typing import Union
 
 from spinesUtils.asserts import ParameterTypeAssert
-import portalocker
 
 from min_vec.api.low_level import StandaloneMinVectorDB
 from min_vec.api import logger
 from min_vec.utils.utils import unavailable_if_deleted
 
 
 class _Register:
@@ -24,24 +22,22 @@
         Save the collection name to the local database path.
 
         Parameters:
             collection (str): The name of the collection.
         """
         if not (self.root_path / 'collections.json').exists():
             with open(self.root_path / 'collections.json', 'w') as f:
-                portalocker.lock(f, portalocker.LOCK_EX)  # add lock
                 json.dump({collection: kwargs}, f)
         else:
             collections = self.get_collections_details()
 
             if collection not in collections:
                 collections[collection] = kwargs
 
                 with open(self.root_path / 'collections.json', 'w') as f:
-                    portalocker.lock(f, portalocker.LOCK_EX)  # add lock
                     json.dump(collections, f)
 
     def deregister_collection(self, collection: str):
         """
         Delete the collection name from the local database path.
 
         Parameters:
@@ -52,15 +48,14 @@
 
         collections = self.get_collections_details()
 
         if collection in collections:
             del collections[collection]
 
             with open(self.root_path / 'collections.json', 'w') as f:
-                portalocker.lock(f, portalocker.LOCK_EX)  # add lock
                 json.dump(collections, f)
 
     def get_collections_details(self) -> dict:
         """
         Show the collections in the database.
 
         Returns:
@@ -68,20 +63,18 @@
         """
         if not (self.root_path / 'collections.json').exists():
             return {}
 
         with open(self.root_path / 'collections.json', 'r') as f:
             collections = json.load(f)
 
-        # 遍历collections，如果有不存在的collection，删除
         for collection in list(collections.keys()):
             if not (self.root_path / collection).exists():
                 del collections[collection]
                 with open(self.root_path / 'collections.json', 'w') as f:
-                    portalocker.lock(f, portalocker.LOCK_EX)  # add lock
                     json.dump(collections, f)
 
         return collections
 
     def show_collections(self) -> list:
         """
         Show the collections in the database.
@@ -110,14 +103,16 @@
             cls._instance = None
             cls._last_root_path = root_path
 
         if cls._instance is None:
             cls._instance = super(MinVectorDBLocalClient, cls).__new__(cls)
             cls._instance._init(root_path)
 
+            cls._last_root_path = root_path
+
         return cls._instance
 
     @ParameterTypeAssert({
         'root_path': str
     }, func_name='MinVectorDB')
     def _init(self, root_path: Union[Path, str]):
         """
@@ -197,15 +192,16 @@
             dim=dim, database_path=collection_path.as_posix(), chunk_size=chunk_size, dtypes=dtypes,
             n_clusters=n_clusters, distance=distance, index_mode=index_mode, use_cache=use_cache,
             scaler_bits=scaler_bits, n_threads=n_threads, warm_up=warm_up, initialize_as_collection=True
         )
         self._register.register_collection(
             collection, dim=dim, database_path=collection_path.as_posix(), chunk_size=chunk_size, dtypes=dtypes,
             n_clusters=n_clusters, distance=distance, index_mode=index_mode, use_cache=use_cache,
-            scaler_bits=scaler_bits, n_threads=n_threads, warm_up=warm_up, initialize_as_collection=True)
+            scaler_bits=scaler_bits, n_threads=n_threads, warm_up=warm_up, initialize_as_collection=True
+        )
 
         return self._collections[collection]
 
     @unavailable_if_deleted
     def get_collection(self, collection: str):
         """
         Get a collection from the database.
@@ -242,21 +238,25 @@
         """
         Delete a collection from the database.
             .. versionadded:: 0.3.0
 
         Parameters:
             collection (str): The name of the collection to delete.
         """
+
         if collection in self._collections:
             self._collections[collection].delete()
             del self._collections[collection]
             self._register.deregister_collection(collection)
         else:
-            _temp_collection = self.get_collection(collection)
-            self.drop_collection(collection)
+            try:
+                _temp_collection = self.get_collection(collection)
+                self.drop_collection(collection)
+            except ValueError:
+                pass
 
     def drop_database(self):
         """
         Delete the database.
             .. versionadded:: 0.3.0
         """
         if self.STATUS == 'DELETED':
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `minvectordb-0.3.2/min_vec/api/low_level.py` & `minvectordb-0.3.3/min_vec/api/low_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 from typing import Union, List, Tuple
 
 import numpy as np
 from spinesUtils.asserts import raise_if, ParameterTypeAssert
 from spinesUtils.timer import Timer
 
 from min_vec.configs.parameters_validator import ParametersValidator
+from min_vec.core_components.cross_lock import ThreadLock
 from min_vec.execution_layer.query import Query
 from min_vec.execution_layer.matrix_serializer import MatrixSerializer
 from min_vec.utils.utils import unavailable_if_deleted
 from min_vec.api import logger
-from min_vec.structures.filter import Filter
+from min_vec.core_components.filter import Filter
 
 
 class StandaloneMinVectorDB:
     """
     A class for managing a vector database stored in .mvdb files and computing vectors similarity.
     """
 
@@ -130,53 +131,47 @@
 
         if warm_up and self._matrix_serializer.shape[0] > 0:
             # Pre query once to cache the jax function
             self.query(np.ones(dim), k=1)
 
             self.most_recent_query_report = {}
 
-    def get_max_id(self):
-        """
-        Get the maximum ID in the database.
-
-        Returns:
-            int: The maximum ID in the database.
-        """
-        if self._matrix_serializer.IS_DELETED or self._matrix_serializer.id_filter is None:
-            return
-        return self._matrix_serializer.id_filter.find_max_value()
+        self.lock = ThreadLock()
 
     @unavailable_if_deleted
-    def add_item(self, vector: Union[np.ndarray, list], *, id: int = None, field: dict = None) -> int:
+    def add_item(self, vector: Union[np.ndarray, list], id: int, *, field: dict = None) -> int:
         """
         Add a single vector to the database.
 
         Parameters:
             vector (np.ndarray or list): The vector to be added.
-            id (int, optional, keyword-only): The ID of the vector. If None, a new ID will be generated.
+            id (int): The ID of the vector.
             field (dict, optional, keyword-only): The field of the vector. Default is None. If None, the field will be
                 set to an empty string.
 
         Returns:
             int: The ID of the added vector.
 
         Raises:
             ValueError: If the vector dimensions don't match or the ID already exists.
         """
         return self._matrix_serializer.add_item(vector, index=id, field=field)
 
     @unavailable_if_deleted
     def bulk_add_items(
-            self, vectors: Union[List[Tuple[np.ndarray, int, dict]], List[Tuple[np.ndarray, int]], List[Tuple[np.ndarray]]]
+            self, vectors: Union[List[Tuple[np.ndarray, int, dict]], List[Tuple[np.ndarray, int]]],
+            **kwargs
     ):
         """
         Bulk add vectors to the database in batches.
 
-        Parameters: vectors (list or tuple): A list or tuple of vectors to be saved. Each vector can be a tuple of (
+        Parameters:
+            vectors (list or tuple): A list or tuple of vectors to be saved. Each vector can be a tuple of (
             vector, id, field).
+            kwargs: Additional keyword arguments. Of no practical significance, only to maintain programming norms.
 
         Returns:
             list: A list of indices where the vectors are stored.
         """
         return self._matrix_serializer.bulk_add_items(vectors)
 
     @unavailable_if_deleted
@@ -255,15 +250,15 @@
 
         time_cost = self._timer.last_timestamp_diff()
         self.most_recent_query_report['Collection Shape'] = self.shape
         self.most_recent_query_report['Query Time'] = f"{time_cost :>.5f} s"
         self.most_recent_query_report['Query Distance'] = self._distance if distance is None else distance
         self.most_recent_query_report['Query K'] = k
 
-        if res[0] is not None:
+        if len(res[0]) > 0:
             self.most_recent_query_report[f'Top {k} Results ID'] = res[0]
             if return_similarity:
                 self.most_recent_query_report[f'Top {k} Results Similarity'] = np.array([round(i, 6) for i in res[1]])
 
         return res
 
     @property
```

### Comparing `minvectordb-0.3.2/min_vec/computational_layer/engines.py` & `minvectordb-0.3.3/min_vec/computational_layer/engines.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.2/min_vec/configs/config.py` & `minvectordb-0.3.3/min_vec/configs/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,28 +44,32 @@
 
     @property
     def MVDB_TRUNCATE_LOG(self):
         return self.get_env_variable('MVDB_TRUNCATE_LOG', True, bool, [bool])
 
     @property
     def MVDB_LOG_WITH_TIME(self):
-        return self.get_env_variable('MVDB_LOG_WITH_TIME', False, bool, [bool])
+        return self.get_env_variable('MVDB_LOG_WITH_TIME', True, bool, [bool])
 
     @property
     def MVDB_KMEANS_EPOCHS(self):
         return self.get_env_variable('MVDB_KMEANS_EPOCHS', 100, int, [int])
 
     @property
     def MVDB_QUERY_CACHE_SIZE(self):
         return self.get_env_variable('MVDB_QUERY_CACHE_SIZE', 10000, int, [int])
 
     @property
     def MVDB_DATALOADER_BUFFER_SIZE(self):
         return self.get_env_variable('MVDB_DATALOADER_BUFFER_SIZE', 20, int, [int, None])
 
+    @property
+    def MVDB_DELAY_NUM(self):
+        return self.get_env_variable('MVDB_DELAY_NUM', 1000, int, [int])
+
     def get_all_configs(self):
         return {
             'MVDB_LOG_LEVEL': self.MVDB_LOG_LEVEL,
             'MVDB_LOG_PATH': self.MVDB_LOG_PATH,
             'MVDB_TRUNCATE_LOG': self.MVDB_TRUNCATE_LOG,
             'MVDB_LOG_WITH_TIME': self.MVDB_LOG_WITH_TIME,
             'MVDB_KMEANS_EPOCHS': self.MVDB_KMEANS_EPOCHS,
```

### Comparing `minvectordb-0.3.2/min_vec/configs/parameters_validator.py` & `minvectordb-0.3.3/min_vec/configs/parameters_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 from functools import wraps
 from pathlib import Path
 
-import portalocker
 from spinesUtils.asserts import raise_if, generate_function_kwargs
 from spinesUtils.logging import Logger
 
 
 class ParametersValidator:
     """Database configuration, define once and can not be changed.
 
@@ -46,15 +45,14 @@
             self.logger.error(f"Failed to load the MinVectorDB configurations.")
             raise e
 
     def save_configs(self, configs_json: Path, configs: dict):
         """Save the configurations."""
         try:
             with open(configs_json, 'w') as f:
-                portalocker.lock(f, portalocker.LOCK_EX)
                 json.dump(configs, f)
 
             return configs
         except (PermissionError, OSError) as e:
             self.logger.error(f"Failed to save the MinVectorDB configurations.")
             raise e
```

### Comparing `minvectordb-0.3.2/min_vec/execution_layer/cluster_worker.py` & `minvectordb-0.3.3/min_vec/execution_layer/cluster_worker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from typing import Callable
 
 from spinesUtils.asserts import raise_if
 from spinesUtils.logging import Logger
 
-from min_vec.storage_layer.storage import StorageWorker
-from min_vec.structures.kmeans import BatchKMeans
+from min_vec.storage_layer.storage import PersistentFileStorage
+from min_vec.core_components.kmeans import BatchKMeans
 
 
 class ClusterWorker:
     def __init__(
             self,
             logger: Logger,
             iterable_dataloader: Callable,
             ann_model: BatchKMeans,
-            storage_worker: StorageWorker,
-            save_data: Callable,
+            storage_worker: PersistentFileStorage,
             n_clusters: int
     ):
         self.logger = logger
         self.iterable_dataloader = iterable_dataloader
         self.ann_model = ann_model
         self.storage_worker = storage_worker
-        self.save_data = save_data
         self.n_clusters = n_clusters
 
     def _kmeans_clustering(self, data, refit=False):
         """kmeans clustering"""
         if refit:
             self.ann_model = self.ann_model.partial_fit(data)
             labels = self.ann_model.labels_
@@ -59,19 +57,19 @@
                 temp_clusters[label][1].append(idx)
                 max_len += 1
 
             if max_len >= 10000:
                 # 遍历每个聚类，保存数据
                 for cluster_id, (d, idx) in temp_clusters.items():
                     if d:  # 检查是否有数据，避免保存空聚类
-                        self.save_data(d, idx, None, write_chunk=False, cluster_id=cluster_id)
+                        self.storage_worker.write(d, idx, write_type='cluster', cluster_id=cluster_id)
 
                 # 初始化每个聚类的存储列表
                 temp_clusters = {i: ([], []) for i in range(self.n_clusters)}
                 max_len = 0
 
         if max_len > 0:
             for cluster_id, (d, idx) in temp_clusters.items():
                 if d:
-                    self.save_data(d, idx, None, write_chunk=False, cluster_id=cluster_id)
+                    self.storage_worker.write(d, idx, write_type='cluster', cluster_id=cluster_id)
 
         self.storage_worker.delete_chunk()
```

### Comparing `minvectordb-0.3.2/min_vec/execution_layer/matrix_serializer.py` & `minvectordb-0.3.3/min_vec/execution_layer/matrix_serializer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from datetime import datetime
 from pathlib import Path
 import shutil
 from typing import Union
 
 import numpy as np
-import portalocker
 from spinesUtils.asserts import raise_if
 from spinesUtils.logging import Logger
 
-from min_vec.structures.id_checker import IDChecker
+from min_vec.core_components.cross_lock import ThreadLock
+from min_vec.core_components.id_checker import IDChecker
 from min_vec.utils.utils import io_checker
 from min_vec.configs.config import config
-from min_vec.structures.kmeans import BatchKMeans
-from min_vec.structures.scaler import ScalarQuantization
-from min_vec.structures.fields_filter import FieldIndex
-from min_vec.storage_layer.storage import StorageWorker
+from min_vec.core_components.kmeans import BatchKMeans
+from min_vec.core_components.scaler import ScalarQuantization
+from min_vec.core_components.metadata_kv import MetaDataKVCache
+from min_vec.storage_layer.storage import PersistentFileStorage, TemporaryFileStorage
 from min_vec.execution_layer.cluster_worker import ClusterWorker
-from min_vec.structures.counter import ThreadSafeCounter
+from min_vec.core_components.counter import SafeCounter
+from min_vec.core_components.thread_safe_list import SafeList
 
 
 class MatrixSerializer:
     """
     The MatrixSerializer class is used to serialize and deserialize the matrix data.
     """
+
     def __init__(
             self,
             dim: int,
             collection_path: Union[str, Path],
             logger: Logger,
             n_clusters: int = 16,
             chunk_size: int = 1_000_000,
@@ -78,53 +80,56 @@
         self.dim = dim
         # set chunk size
         self.chunk_size = chunk_size
         # set filter path
         self._filter_path = self.collections_path_parent / 'id_filter.mvdb'
 
         # set collection path
-        self.collections_path = self.collections_path_parent  # / Path(collection_path).name
+        self.collections_path = self.collections_path_parent
 
         # set scalar quantization bits
         self.scaler_bits = scaler_bits if scaler_bits is not None else None
         self.scaler = None
         if self.scaler_bits is not None:
             self._initialize_scalar_quantization()
 
         # initialize the storage worker
-        self.storage_worker = StorageWorker(self.collections_path_parent, self.dim,
-                                            self.chunk_size,
-                                            warm_up=warm_up)
-        self.counter = ThreadSafeCounter()
+        self.storage_worker = PersistentFileStorage(self.collections_path_parent, self.dim,
+                                                    self.chunk_size,
+                                                    warm_up=warm_up)
+        self.tempfile_storage_worker = TemporaryFileStorage(self.chunk_size)
+
+        self.counter = SafeCounter()
 
         # ============== Loading or create one empty collection ==============
         # first of all, initialize a collection
-        self.database = []
-        self.indices = []
-        self.fields = []
+        self.database = SafeList()
+        self.indices = SafeList()
+        self.fields = SafeList()
 
         self._initialize_fields_index()
         self._initialize_ann_model()
         self._initialize_id_checker()
 
         self.cluster_worker = ClusterWorker(
             logger=self.logger,
             iterable_dataloader=self.dataloader,
             ann_model=self.ann_model,
             storage_worker=self.storage_worker,
-            save_data=self.save_data,
             n_clusters=self.n_clusters
         )
 
         if self._get_cluster_dataset_num() > 0 and self.index_mode == 'FLAT':
             # cause the index mode is FLAT, but the cluster dataset is not empty,
             # so the clustered datasets will also be traversed during querying.
             self.logger.warning('The index mode is FLAT, but the cluster dataset is not empty, '
                                 'so the clustered datasets will also be traversed during querying.')
 
+        self.lock = ThreadLock()
+
     def _initialize_parent_path(self, collections_path):
         """make directory if not exist"""
         self.collections_path_parent = (Path(collections_path).parent.absolute() /
                                         Path(collections_path).absolute().name)
 
         self.collections_path_parent.mkdir(parents=True, exist_ok=True)
 
@@ -150,17 +155,19 @@
                                                  batch_size=10240, epochs=MVDB_KMEANS_EPOCHS)
         else:
             self.ann_model = None
 
     def _initialize_fields_index(self):
         """initialize fields index"""
         if Path(self.collections_path_parent / 'fields_index.mvdb').exists():
-            self.fields_index = FieldIndex().load(self.collections_path_parent / 'fields_index.mvdb')
+            self.kv_index = MetaDataKVCache().load(self.collections_path_parent / 'fields_index.mvdb')
         else:
-            self.fields_index = FieldIndex()
+            self.kv_index = MetaDataKVCache()
+
+        self.temp_kv_index = MetaDataKVCache()
 
     def _initialize_id_checker(self):
         """initialize id checker and shape"""
         self.id_filter = IDChecker()
 
         if self._filter_path.exists():
             self.id_filter.from_file(self._filter_path)
@@ -169,23 +176,21 @@
                 filenames = self.storage_worker.get_all_files(read_type='all')
                 for filename in filenames:
                     database, indices = self.storage_worker.read(filename=filename)
                     self.id_filter.add(indices)
 
         self.last_id = self.id_filter.find_max_value()
 
-    def check_commit(self):
-        if not self.COMMIT_FLAG:
-            raise ValueError("Did you forget to run `commit()` function ? Try to run `commit()` first.")
+        self.temp_id_filter = IDChecker()
 
     def reset_collection(self):
         """Reset the database to its initial state with zeros."""
-        self.database = []
-        self.indices = []
-        self.fields = []
+        self.database = SafeList()
+        self.indices = SafeList()
+        self.fields = SafeList()
 
     @io_checker
     def dataloader(self, filename):
         """
         Generator for loading the database and index.
 
         Parameters:
@@ -218,145 +223,178 @@
         Raises:
             ValueError: If the lengths of the database, indices, and fields are not the same.
         """
         if not self._is_collection_reset() and not self.COMMIT_FLAG:
             if not (len(self.database) == len(self.indices) == len(self.fields)):
                 raise ValueError('The database, index length and field length in collection are not the same.')
 
-    def save_data(self, data, indices, fields, write_chunk=True, cluster_id=None, normalize=False):
+    def save_data(self, data, indices, fields):
         """Optimized method to save data to chunk or cluster group with reusable logic."""
-        if fields is not None and cluster_id is None:
-            for id, field in zip(indices, fields):
-                self.fields_index.store(field, id)
-
-        self.storage_worker.write(data, indices,
-                                  write_type='chunk' if write_chunk else 'cluster',
-                                  cluster_id=str(cluster_id) if cluster_id is not None else cluster_id,
-                                  normalize=normalize)
+
+        for _id, _field in zip(indices, fields):
+            self.temp_kv_index.store(_field if _field is not None else {}, _id)
+
+        self.tempfile_storage_worker.write_temp_data(data, indices)
 
     @io_checker
-    def save_chunk_immediately(self, normalize=True):
+    def save_chunk_immediately(self):
         """
         Save the current state of the collection to a .mvdb file.
 
         Returns:
             Path: The path of the saved collection file.
         """
         self._length_checker()
 
         if self._is_collection_reset():
-            return []
+            return
 
         self.save_data(
             self.database,
             self.indices,
-            self.fields,
-            write_chunk=True,
-            cluster_id=None,
-            normalize=normalize
+            self.fields
         )
 
         self.reset_collection()  # reset collection, indices and fields
 
-    def auto_save_chunk(self, normalize=True):
+    def auto_save_chunk(self):
         self._length_checker()
         if len(self.database) >= self.chunk_size:
-            self.save_chunk_immediately(normalize=normalize)
+            self.save_chunk_immediately()
 
         return
 
     def _get_cluster_dataset_num(self):
         if not self.collections_path.exists():
             return 0
 
         return self.storage_worker.get_cluster_dataset_num()
 
-    def commit(self):
+    def rollback(self):
         """
-        Save the collection, ensuring that all data is written to disk.
-        This method is required to be called after saving vectors to query them.
+        Rollback the collection to the last commit.
         """
         if not self.COMMIT_FLAG:
-            self.logger.debug('Saving chunk immediately...')
-            self.save_chunk_immediately(normalize=True)
-
-            self.logger.debug('Saving id filter...')
-            # save filter
-            self.id_filter.to_file(self._filter_path)
-
-            # save fields index
-            self.logger.debug('Saving fields index...')
-            self.fields_index.save(self.collections_path_parent / 'fields_index.mvdb')
-
-            chunk_partition_size = self.storage_worker.get_shape(read_type='chunk')[0]
-            cluster_partition_size = self.storage_worker.get_shape(read_type='cluster')[0]
-
-            all_partition_size = self.storage_worker.get_shape(read_type='all')[0]
-
-            if all_partition_size >= 100000 and not (self.collections_path_parent / 'scaled_status.json').exists():
-                # only run once
-                self.storage_worker.update_quantizer(self.scaler)
-                filenames = self.storage_worker.get_all_files(read_type='chunk')
-                if filenames:
-                    for filename in filenames:
-                        self.storage_worker.write(filename=filename)
-
-                with open(self.collections_path_parent / 'scaled_status.json', 'w') as f:
-                    portalocker.lock(f, portalocker.LOCK_EX)
-                    import json
-                    json.dump({'status': True}, f)
-
-            if (
-                    cluster_partition_size == 0 and (chunk_partition_size >= 100000 and self.index_mode != 'FLAT')
-            ) or (
-                    cluster_partition_size > 0 and self.index_mode != 'FLAT'
-            ):
-                self.logger.info('Building index...')
-
-                if cluster_partition_size == 0 and (chunk_partition_size >= 100000 and self.index_mode != 'FLAT'):
-                    self.logger.info('Start to fit the index for cluster...')
-                    self.cluster_worker.build_index(refit=True)
-                else:
-                    self.counter.add(chunk_partition_size)
-                    if self.counter.get_value() >= 100000:
-                        self.logger.info('Refitting the index for cluster...')
-                        self.cluster_worker.build_index(refit=True)
-                        self.counter.reset()
-                    else:
-                        self.logger.info('Incrementally building the index for cluster...')
-                        self.cluster_worker.build_index(refit=False)
-
-                # save ivf index and k-means model
-                self.logger.debug('Saving ann model...')
-                self.ann_model.save(self.collections_path_parent / 'ann_model.mvdb')
-
             self.reset_collection()
-
-            if self.scaler_bits is not None:
-                if self.scaler.fitted:
-                    self.scaler.save(self.collections_path_parent / 'sq_model.mvdb')
+            self.tempfile_storage_worker.reincarnate()
+            self.temp_id_filter = IDChecker()
+            self.temp_kv_index = MetaDataKVCache()
 
             self.COMMIT_FLAG = True
 
-            self.last_commit_time = datetime.now()
-
-    def _generate_new_id(self):
+    def commit(self):
         """
-        Generate a new ID for the vector.
+        Save the collection, ensuring that all data is written to disk.
+        This method is required to be called after saving vectors to query them.
         """
-        while True:
-            self.last_id += 1
-            if self.last_id not in self.id_filter:
-                break
+        with self.lock:
+            if not self.COMMIT_FLAG:
+                try:
+                    self.logger.debug('Saving chunk immediately...')
+                    self.save_chunk_immediately()
+
+                    try:
+                        self.logger.debug('Concatenating id filter...')
+                        # concat filter
+                        self.id_filter.concat(self.temp_id_filter)
+                    except Exception as e:
+                        self.logger.error(f'Error occurred while concatenating the filter: {e}, rollback...')
+                        self.rollback()
+                        raise e
+
+                    self.logger.debug('Writing chunk to storage...')
+                    for data, indices in self.tempfile_storage_worker.get_file_iterator():
+                        self.storage_worker.write(data, indices, write_type='chunk', normalize=True)
+
+                    self.tempfile_storage_worker.reincarnate()
+
+                except Exception as e:
+                    self.logger.error(f'Error occurred while saving the collection: {e}, rollback...')
+                    self.rollback()
+                    raise e
+
+                try:
+                    self.logger.debug('Concatenating fields index...')
+                    self.kv_index.concat(self.temp_kv_index)
+                except Exception as e:
+                    self.logger.error(f'Error occurred while concatenating the fields index: {e}, rollback...')
+                    self.rollback()
+                    raise e
+
+                try:
+                    self.logger.debug('Saving id filter...')
+                    self.id_filter.to_file(self._filter_path)
+                except Exception as e:
+                    self.logger.error(f'Error occurred while saving the filter: {e}, rollback...')
+                    self.rollback()
+                    raise e
+
+                try:
+                    # save fields index
+                    self.logger.debug('Saving fields index...')
+                    self.kv_index.save(self.collections_path_parent / 'fields_index.mvdb')
+                except Exception as e:
+                    self.logger.error(f'Error occurred while saving the collection: {e}, rollback...')
+                    self.rollback()
+                    raise e
+
+                chunk_partition_size = self.storage_worker.get_shape(read_type='chunk')[0]
+                cluster_partition_size = self.storage_worker.get_shape(read_type='cluster')[0]
+
+                all_partition_size = self.storage_worker.get_shape(read_type='all')[0]
+
+                if all_partition_size >= 100000 and not (self.collections_path_parent / 'scaled_status.json').exists():
+                    # only run once
+                    self.storage_worker.update_quantizer(self.scaler)
+                    filenames = self.storage_worker.get_all_files(read_type='chunk')
+                    if filenames:
+                        for filename in filenames:
+                            self.storage_worker.write(filename=filename)
+
+                    with open(self.collections_path_parent / 'scaled_status.json', 'w') as f:
+                        import json
+                        json.dump({'status': True}, f)
+
+                if (
+                        cluster_partition_size == 0 and (chunk_partition_size >= 100000 and self.index_mode != 'FLAT')
+                ) or (
+                        cluster_partition_size > 0 and self.index_mode != 'FLAT'
+                ):
+                    self.logger.info('Building index...')
+
+                    if cluster_partition_size == 0 and (chunk_partition_size >= 100000 and self.index_mode != 'FLAT'):
+                        self.logger.info('Start to fit the index for cluster...')
+                        self.cluster_worker.build_index(refit=True)
+                    else:
+                        self.counter.add(chunk_partition_size)
+                        if self.counter.get_value() >= 100000:
+                            self.logger.info('Refitting the index for cluster...')
+                            self.cluster_worker.build_index(refit=True)
+                            self.counter.reset()
+                        else:
+                            self.logger.info('Incrementally building the index for cluster...')
+                            self.cluster_worker.build_index(refit=False)
+
+                    # save ivf index and k-means model
+                    self.logger.debug('Saving ann model...')
+                    self.ann_model.save(self.collections_path_parent / 'ann_model.mvdb')
+
+                self.reset_collection()
+
+                if self.scaler_bits is not None:
+                    if self.scaler.fitted:
+                        self.scaler.save(self.collections_path_parent / 'sq_model.mvdb')
 
-        return self.last_id
+                self.COMMIT_FLAG = True
+
+                self.last_commit_time = datetime.now()
 
     def _process_vector_item(self, vector, index, field):
-        if index in self.id_filter:
-            raise ValueError(f'id {index} already exists')
+        if index in self.id_filter or index in self.temp_id_filter:
+            raise ValueError(f'id {index} already exists.')
 
         if len(vector) != self.dim:
             raise ValueError(f'vector dim error, expect {self.dim}, got {len(vector)}')
 
         if vector.dtype != self.dtypes:
             vector = vector.astype(self.dtypes)
 
@@ -373,129 +411,121 @@
             vector, id, field).
 
         Returns:
             list: A list of indices where the vectors are stored.
         """
         raise_if(ValueError, not isinstance(vectors, (tuple, list)),
                  f'vectors must be tuple or list, got {type(vectors)}')
-        raise_if(ValueError, not all(isinstance(i, tuple) for i in vectors),
-                 f'vectors must be tuple of (vector, id[optional], field[optional]).')
 
-        new_ids = []
+        with self.lock:
+            new_ids = []
+
+            for i in range(0, len(vectors), self.chunk_size):
+                batch = vectors[i:i + self.chunk_size]
 
-        for i in range(0, len(vectors), self.chunk_size):
-            batch = vectors[i:i + self.chunk_size]
+                for sample in batch:
+                    sample_len = len(sample)
 
-            for sample in batch:
-                if len(sample) == 1:
-                    vector = sample[0]
-                    index = None
-                    field = {}
-                elif len(sample) == 2:
-                    vector, index = sample
-                    field = {}
-                else:
-                    raise_if(ValueError, len(sample) != 3,
-                             f'vectors must be tuple of (vector, id[optional], field[optional]).')
-                    vector, index, field = sample
+                    if sample_len == 3:
+                        vector, index, field = sample
+                    elif sample_len == 2:
+                        vector, index = sample
+                        field = {}
+                    else:
+                        raise ValueError('Each sample must be a tuple of (vector, id, field[optional]).')
 
                     raise_if(TypeError, not (isinstance(field, dict) or field is None),
                              f'field must be dict or None, got {type(field)}')
 
-                if isinstance(vector, list):
-                    vector = np.array(vector)
-
-                index = self._generate_new_id() if index is None else index
+                    if isinstance(vector, list):
+                        vector = np.array(vector)
 
-                raise_if(ValueError, index < 0, f'id must be greater than 0, got {index}')
+                    raise_if(ValueError, (not isinstance(index, int)) or index < 0,
+                             f'id must be integer and greater than 0, got {index}')
 
-                field = {} if field is None else field
-                vector, index, field = self._process_vector_item(vector, index, field)
+                    field = {} if field is None else field
+                    vector, index, field = self._process_vector_item(vector, index, field)
 
-                self.database.append(vector)
-                internal_id = index if index is not None else self._generate_new_id()
-                self.indices.append(internal_id)
-                new_ids.append(internal_id)
-                self.fields.append(field)
-                self.id_filter.add(index)
+                    self.database.append(vector)
+                    self.indices.append(index)
+                    new_ids.append(index)
+                    self.fields.append(field)
+                    self.temp_id_filter.add(index)
 
-            self.auto_save_chunk(normalize=True)
+                self.auto_save_chunk()
 
-        if self.COMMIT_FLAG:
-            self.COMMIT_FLAG = False
+            if self.COMMIT_FLAG:
+                self.COMMIT_FLAG = False
 
-        return new_ids
+            return new_ids
 
-    def add_item(self, vector, *, index: int = None, field: dict = None) -> int:
+    def add_item(self, vector, index: int, *, field: dict = None) -> int:
         """
         Add a single vector to the collection.
 
         Parameters:
             vector (np.ndarray): The vector to be added.
-            index (int, optional, keyword-only): The ID of the vector. If None, a new ID will be generated.
+            index (int): The ID of the vector.
             field (dict, optional, keyword-only): The field of the vector. Default is None. If None, the field will be
                 set to an empty string.
         Returns:
             int: The ID of the added vector.
 
         Raises:
             ValueError: If the vector dimensions don't match or the ID already exists.
         """
-        raise_if(ValueError, len(vector) != self.dim,
-                 f'vector dim error, expect {self.dim}, got {len(vector)}')
         if isinstance(vector, list):
             vector = np.array(vector)
 
         raise_if(ValueError, vector.ndim != 1, f'vector dim error, expect 1, got {vector.ndim}')
         raise_if(ValueError, field is not None and not isinstance(field, dict),
                  f'field must be dict, got {type(field)}')
-        raise_if(ValueError, index is not None and not isinstance(index, int), f'id must be int, got {type(index)}')
-        raise_if(ValueError, index is not None and index < 0, f'id must be greater than 0, got {index}')
 
-        index = self._generate_new_id() if index is None else index
+        raise_if(ValueError, (not isinstance(index, int)) or index < 0,
+                 f'id must be integer and greater than 0, got {index}')
 
-        raise_if(ValueError, index in self.id_filter, f'id {index} already exists')
+        with self.lock:
+            vector, index, field = self._process_vector_item(vector, index, field)
 
-        vector, index, field = self._process_vector_item(vector, index, field)
+            # Add the id to then filter.
+            self.temp_id_filter.add(index)
 
-        # Add the id to then filter.
-        self.id_filter.add(index)
+            self.database.append(vector)
+            self.indices.append(index)
+            self.fields.append(field)
 
-        self.database.append(vector)
-        self.indices.append(index)
-        self.fields.append(field)
+            self.auto_save_chunk()
 
-        self.auto_save_chunk(normalize=True)
+            if self.COMMIT_FLAG:
+                self.COMMIT_FLAG = False
 
-        if self.COMMIT_FLAG:
-            self.COMMIT_FLAG = False
-
-        return index
+            return index
 
     def delete(self):
         """Delete collection."""
-        if not self.collections_path_parent.exists():
-            return None
-
-        try:
-            shutil.rmtree(self.collections_path_parent)
-        except FileNotFoundError:
-            pass
+        with self.lock:
+            if not self.collections_path_parent.exists():
+                return None
+
+            try:
+                shutil.rmtree(self.collections_path_parent)
+            except FileNotFoundError:
+                pass
 
-        self.IS_DELETED = True
-        self.reset_collection()
+            self.IS_DELETED = True
+            self.reset_collection()
 
-        # reinitialize
-        if self.scaler_bits is not None:
-            self._initialize_scalar_quantization()
+            # reinitialize
+            if self.scaler_bits is not None:
+                self._initialize_scalar_quantization()
 
-        self._initialize_fields_index()
-        self._initialize_ann_model()
-        self._initialize_id_checker()
+            self._initialize_fields_index()
+            self._initialize_ann_model()
+            self._initialize_id_checker()
 
-        # clear cache
-        self.storage_worker.clear_cache()
+            # clear cache
+            self.storage_worker.clear_cache()
 
     @property
     def shape(self):
-        self.check_commit()
-        return tuple(self.storage_worker.get_shape(read_type='all'))
+        with self.lock:
+            return tuple(self.storage_worker.get_shape(read_type='all'))
```

### Comparing `minvectordb-0.3.2/min_vec/storage_layer/storage.py` & `minvectordb-0.3.3/min_vec/storage_layer/storage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,94 @@
+import os
+import shutil
+import tempfile
 from pathlib import Path
 import json
 
 import numpy as np
-import portalocker
 from spinesUtils.asserts import raise_if
 
 from min_vec.computational_layer.engines import to_normalize
 from min_vec.configs.config import config
-from min_vec.structures.limited_dict import LimitedDict
+from min_vec.core_components.cross_lock import ThreadLock
+from min_vec.core_components.limited_dict import LimitedDict
 
 
-class StorageWorker:
+class TemporaryFileStorage:
+    """Class for handling temporary storage of data and indices with specified chunk sizes,
+    ensuring paired data and indices with a sequential file ID."""
+
+    def __init__(self, chunk_size):
+        self.temp_dir = tempfile.TemporaryDirectory()
+        self.chunk_size = chunk_size
+        self.file_id = 0  # File ID to maintain the naming order
+        self.lock = ThreadLock()
+
+    def write_temp_data(self, data, indices, prefix='temp'):
+        with self.lock:
+            if not isinstance(data, np.ndarray):
+                data = np.vstack(data)
+
+            if not isinstance(indices, np.ndarray):
+                indices = np.array(indices)
+
+            num_rows = data.shape[0]
+            start = 0
+            file_paths = []
+
+            while start < num_rows:
+                end = min(start + self.chunk_size, num_rows)
+                chunk_data = data[start:end]
+                chunk_indices = indices[start:end]
+                file_id = self.file_id
+                self.file_id += 1  # Increment file ID for each new chunk
+
+                data_file_path = Path(self.temp_dir.name) / f"{prefix}_data_{file_id}.npy"
+                indices_file_path = Path(self.temp_dir.name) / f"{prefix}_indices_{file_id}.npy"
+
+                with open(data_file_path, 'wb') as df, open(indices_file_path, 'wb') as inf:
+                    np.save(df, chunk_data)
+                    np.save(inf, chunk_indices)
+
+                file_paths.append((data_file_path, indices_file_path))
+                start += self.chunk_size
+
+            return file_paths
+
+    @staticmethod
+    def read_temp_data(data_filepath, indices_filepath):
+        with open(data_filepath, 'rb') as df, open(indices_filepath, 'rb') as inf:
+            data = np.load(df)
+            indices = np.load(inf)
+        return data, indices
+
+    def get_file_iterator(self):
+        """Generate an iterator to read data and indices files sequentially."""
+        with self.lock:
+            file_ids = [int(i.stem.split('_')[-1]) for i in Path(self.temp_dir.name).glob('temp_data_*.npy')]
+            for file_id in file_ids:
+                data_path = Path(self.temp_dir.name) / f"temp_data_{file_id}.npy"
+                indices_path = Path(self.temp_dir.name) / f"temp_indices_{file_id}.npy"
+                yield self.read_temp_data(data_path, indices_path)
+
+    def cleanup(self):
+        if os.path.exists(self.temp_dir.name):
+            shutil.rmtree(self.temp_dir.name)
+
+    def reincarnate(self):
+        with self.lock:
+            self.cleanup()
+            self.temp_dir = tempfile.TemporaryDirectory()
+            self.file_id = 0
+
+    def __del__(self):
+        self.cleanup()
+
+
+class PersistentFileStorage:
     """The worker class for reading and writing data to the files."""
 
     def __init__(self, collection_path, dimension, chunk_size, warm_up=False):
         self.collection_path = Path(collection_path)
         self.collection_chunk_path = self.collection_path / 'chunk_data'
         self.collection_chunk_indices_path = self.collection_path / 'chunk_indices_data'
 
@@ -24,27 +98,33 @@
         for path in [self.collection_chunk_path, self.collection_chunk_indices_path,
                      self.collection_cluster_path, self.collection_cluster_indices_path]:
             path.mkdir(parents=True, exist_ok=True)
 
         self.dimension = dimension
         self.chunk_size = chunk_size
 
+        self.tempfile_storage = TemporaryFileStorage(chunk_size)
+
         self.cluster_last_file_shape = {}
 
         self.cache = LimitedDict(max_size=config.MVDB_DATALOADER_BUFFER_SIZE)
 
         self.quantizer = None
 
+        self.lock = ThreadLock()
+
         if warm_up:
             self.warm_up()
 
     def update_quantizer(self, quantizer):
-        self.quantizer = quantizer
+        with self.lock:
+            self.quantizer = quantizer
 
     def file_exists(self):
+        """Check if the file exists."""
         return ((self.collection_chunk_path / 'chunk_0').exists()
                 or (self.collection_cluster_path / 'cluster_0_0').exists())
 
     def warm_up(self):
         """Load the data from the file to the memory."""
         if not self.file_exists():
             return
@@ -122,19 +202,17 @@
             return max(ids)
 
         return -1
 
     @staticmethod
     def _write_to_disk(data, indices, data_path, indices_path, filename):
         with open(data_path / filename, 'wb') as f:
-            portalocker.lock(f, portalocker.LOCK_EX)
             np.save(f, data)
 
         with open(indices_path / filename, 'wb') as f:
-            portalocker.lock(f, portalocker.LOCK_EX)
             np.save(f, indices)
 
     def _incremental_write(self, data, indices, write_type='chunk', cluster_id=None, normalize=False):
         if normalize:
             data = to_normalize(np.vstack(data))
 
         if write_type == 'chunk':
@@ -151,15 +229,14 @@
         # read info file to get the shape of the data
         # file shape
         if write_type == 'chunk':
             # save the total shape of the data
             if not (self.collection_path / 'info.json').exists():
                 total_shape = [0, self.dimension]
                 with open(self.collection_path / 'info.json', 'w') as f:
-                    portalocker.lock(f, portalocker.LOCK_EX)
                     json.dump({"total_shape": total_shape}, f)
             else:
                 with open(self.collection_path / 'info.json', 'r') as f:
                     total_shape = json.load(f)['total_shape']
 
             # in this class, we only use the quantizer in chunk_write, after quantization,
             # the disk data and memory data will be changed to quantized data
@@ -234,15 +311,14 @@
                     self._write_to_disk(temp_data, temp_indices, collection_subfile_path,
                                         collection_indices_path, filename)
 
                     self._write_to_memory(filename, temp_data, temp_indices)
 
         if write_type == 'chunk':
             with open(self.collection_path / 'info.json', 'w') as f:
-                portalocker.lock(f, portalocker.LOCK_EX)
                 total_shape[0] += data_shape
                 json.dump({"total_shape": total_shape}, f)
         else:
             self.cluster_last_file_shape[cluster_id] = [data_shape + total_shape[0], self.dimension]
 
     def _overwrite(self, filename, normalize=False):
         """only use in chunk write"""
@@ -259,65 +335,70 @@
 
     def read(self, filename):
         """Read the data from the file."""
         return self._read(filename=filename)
 
     def write(self, data=None, indices=None, write_type='chunk', cluster_id=None, normalize=False, filename=None):
         """Write the data to the file."""
-        if write_type in ['chunk', 'cluster']:
-            if filename:
-                self._overwrite(filename, normalize=normalize)
+        with self.lock:
+            if write_type in ['chunk', 'cluster']:
+                if filename:
+                    self._overwrite(filename, normalize=normalize)
+                else:
+                    self._incremental_write(data, indices, write_type=write_type, cluster_id=cluster_id,
+                                            normalize=normalize)
             else:
-                self._incremental_write(data, indices, write_type=write_type, cluster_id=cluster_id,
-                                        normalize=normalize)
-        else:
-            raise ValueError('write_type must be "chunk" or "cluster"')
+                raise ValueError('write_type must be "chunk" or "cluster"')
 
     def get_shape(self, read_type='all'):
         """Get the shape of the data.
         parameters:
             read_type (str): The type of data to read. Must be 'chunk' or 'cluster' or 'all'.
         """
-        if read_type == 'chunk':
-            shape = [0, self.dimension]
-            filenames = self.get_all_files(read_type='chunk')
-            if filenames:
-                for filename in filenames:
-                    data, _ = self.read(filename)
-                    shape[0] += len(data)
-
-            return shape
-
-        elif read_type == 'cluster':
-            shape = [0, self.dimension]
+        with self.lock:
+            if read_type == 'chunk':
+                shape = [0, self.dimension]
+                filenames = self.get_all_files(read_type='chunk')
+                if filenames:
+                    for filename in filenames:
+                        data, _ = self.read(filename)
+                        shape[0] += len(data)
+
+                return shape
+
+            elif read_type == 'cluster':
+                shape = [0, self.dimension]
+
+                filenames = self.get_all_files(read_type='cluster')
+                if filenames:
+                    for filename in filenames:
+                        data, _ = self.read(filename)
+                        shape[0] += len(data)
+
+                return shape
+
+            elif read_type == 'all':
+                if not (self.collection_path / 'info.json').exists():
+                    return [self.get_shape('chunk')[0] + self.get_shape('cluster')[0], self.dimension]
 
-            filenames = self.get_all_files(read_type='cluster')
-            if filenames:
-                for filename in filenames:
-                    data, _ = self.read(filename)
-                    shape[0] += len(data)
-
-            return shape
-
-        elif read_type == 'all':
-            if not (self.collection_path / 'info.json').exists():
-                return [self.get_shape('chunk')[0] + self.get_shape('cluster')[0], self.dimension]
-
-            with open(self.collection_path / 'info.json', 'r') as f:
-                return json.load(f)['total_shape']
+                with open(self.collection_path / 'info.json', 'r') as f:
+                    return json.load(f)['total_shape']
 
     def delete_chunk(self):
         """Delete the chunk files."""
-        for file in self.collection_chunk_path.glob('*'):
-            file.unlink()
-        for file in self.collection_chunk_indices_path.glob('*'):
-            file.unlink()
+        with self.lock:
+            for file in self.collection_chunk_path.glob('*'):
+                file.unlink()
+            for file in self.collection_chunk_indices_path.glob('*'):
+                file.unlink()
 
     def get_cluster_dataset_num(self):
-        return len(list(self.collection_cluster_path.glob('cluster_*')))
+        """Get the number of cluster datasets."""
+        with self.lock:
+            return len(list(self.collection_cluster_path.glob('cluster_*')))
 
     def get_dataset_by_cluster_id(self, cluster_id):
         results = []
 
         filenames = self.get_all_files(read_type='cluster', cluster_id=cluster_id)
 
         for filename in filenames:
@@ -358,15 +439,14 @@
                 continue
 
             index = np.where(indices == by_indices)[0][0]
             _data[index] = data
 
             with open(self.collection_chunk_path / path if read_type == 'chunk'
                       else self.collection_cluster_path / path, 'wb') as f:
-                portalocker.lock(f, portalocker.LOCK_EX)
                 np.save(f, _data)
 
             # delete cache
             self.cache.pop(path, None)
 
             break
```

### Comparing `minvectordb-0.3.2/min_vec/structures/kmeans.py` & `minvectordb-0.3.3/min_vec/core_components/kmeans.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import portalocker
 from sklearn.cluster import MiniBatchKMeans
 
 
 class BatchKMeans:
     def __init__(self, n_clusters, random_state=42, epochs=100, batch_size=1024):
         self.model = MiniBatchKMeans(n_clusters=n_clusters, random_state=random_state, max_iter=epochs,
                                      batch_size=batch_size, n_init='auto', reassignment_ratio=0)
@@ -31,15 +30,14 @@
 
         return self.model.predict(X)
 
     def save(self, filename):
         import cloudpickle
 
         with open(filename, 'wb') as f:
-            portalocker.lock(f, portalocker.LOCK_EX)
             cloudpickle.dump(self.model, f)
 
     def load(self, filename):
         import cloudpickle
 
         self.model = cloudpickle.load(open(filename, 'rb'))
```

### Comparing `minvectordb-0.3.2/min_vec/structures/limited_dict.py` & `minvectordb-0.3.3/min_vec/core_components/limited_dict.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from collections import OrderedDict
-import threading
+
+from min_vec.core_components.cross_lock import ThreadLock
 
 
 class LimitedDict:
     def __init__(self, max_size):
         self.max_size = max_size
         self.cache = OrderedDict()
-        self.lock = threading.RLock()
+        self.lock = ThreadLock()
 
     def __setitem__(self, key, value):
         with self.lock:
             if key in self.cache:
                 del self.cache[key]
             self.cache[key] = value
             if len(self.cache) > self.max_size:
@@ -21,19 +22,22 @@
             try:
                 value = self.cache.pop(key)
                 self.cache[key] = value
                 return value
             except KeyError:
                 raise KeyError('Key not found')
 
+    @property
+    def is_reached_max_size(self):
+        return len(self.cache) == self.max_size
+
     def get(self, key, default=None):
-        with self.lock:
-            if key not in self.cache:
-                return default
-            return self.__getitem__(key)
+        if key not in self.cache:
+            return default
+        return self.__getitem__(key)
 
     def clear(self):
         with self.lock:
             self.cache.clear()
 
     def keys(self):
         with self.lock:
```

### Comparing `minvectordb-0.3.2/min_vec/structures/limited_sort.py` & `minvectordb-0.3.3/min_vec/core_components/limited_sort.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import threading
 import numpy as np
 
 from min_vec.computational_layer.engines import cosine_distance, argsort_topk, euclidean_distance
+from min_vec.core_components.cross_lock import ThreadLock
 
 
 class LimitedSorted:
     def __init__(self, dim, dtype, scaler, chunk_size):
         """A class to store the top n most similar vectors to a given vector.
 
         .. versionadded:: 0.2.5
@@ -13,15 +13,15 @@
         Parameters:
             dim (int): The dimension of the vectors.
             dtype (type): The data type of the vectors.
             scaler (Scaler, optional): The scaler to decode the vectors.
             chunk_size (int): The maximum number of vectors to store.
                 .. versionadded:: 0.2.7
         """
-        self.lock = threading.RLock()
+        self.lock = ThreadLock()
         self.dim = dim
         self.n = None
         self.scaler = scaler
         self.max_length = chunk_size
         self.current_length = 0
         self.similarities = np.empty(self.max_length, dtype=dtype)
         self.indices = np.empty(self.max_length, dtype=int)
```

### Comparing `minvectordb-0.3.2/min_vec/structures/scaler.py` & `minvectordb-0.3.3/min_vec/core_components/scaler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """scaler.py - Scalar Quantization module"""
 import numpy as np
 import numexpr as ne
 import cloudpickle
-import portalocker
 
 from spinesUtils.asserts import raise_if
 
 
 class ScalarQuantization:
     bits_map = {8: np.uint8, 16: np.uint16, 32: np.uint32}
 
@@ -87,15 +86,14 @@
 
         return decoded
 
     def save(self, filepath):
         raise_if(ValueError, not self.fitted, 'The model must be fitted before saving.')
         try:
             with open(filepath, 'wb') as file:
-                portalocker.lock(file, portalocker.LOCK_EX)
                 cloudpickle.dump(self, file)
         except IOError as e:
             print(f"Error saving model: {e}")
 
     @staticmethod
     def load(filepath):
         try:
```

### Comparing `minvectordb-0.3.2/min_vec/utils/utils.py` & `minvectordb-0.3.3/min_vec/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         except Exception:
             raise_if(UnKnownError, True, f"Encounter Unknown Error "
                                          f"when read or write the file.")
 
     return wrapper
 
 
-class QueryVectorCache:
+class QueryResultsCache:
     """A decorator that caches the results of a function call with the same arguments.
         Only use for DatabaseQuery.query function.
     """
 
     def __init__(self, max_size=1000):
         from collections import OrderedDict
```

### Comparing `minvectordb-0.3.2/setup.py` & `minvectordb-0.3.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 reqs = read_requirements(Path('.').parent.joinpath("requirements.txt"))
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='MinVectorDB',
-    version="0.3.2",
+    version="0.3.3",
     description='A pure Python-implemented, lightweight, server-optional, '
                 'multi-end compatible, vector database deployable locally or remotely.',
     keywords='vector database',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `minvectordb-0.3.2/test/docker_tests/test_docker_api.py` & `minvectordb-0.3.3/test/docker_tests/test_docker_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # The address of the docker container running the service is http://localhost:5403
 import numpy as np
 
 from test import MinVectorDB
 from test import MinVectorDBHTTPClient, Collection
 
-root_url = 'http://localhost:5403'
+root_url = 'http://localhost:7637'
 
 
 def test_initialization():
     db = MinVectorDB(root_url)
 
     assert isinstance(db, MinVectorDBHTTPClient)
 
@@ -51,33 +51,31 @@
                                          ([0.75, 0.44, 0.38, 0.75], 10, {'field': 'test_1', 'order': 9})])
     assert ids == [2, 3, 4, 5, 6, 7, 8, 9, 10]
 
 
 def test_query():
     import operator
 
-    from min_vec.structures.filter import Filter, FieldCondition, MatchField, IDCondition, MatchID
+    from min_vec.core_components.filter import Filter, FieldCondition, MatchField, IDCondition, MatchID
 
     db = MinVectorDB(root_url)
     collection = db.get_collection('test_collection')
     ids, scores = collection.query(
         vector=[0.36, 0.43, 0.56, 0.12],
         k=10,
         query_filter=Filter(
             must=[
                 FieldCondition(key='field', matcher=MatchField('test_1')),  # Support for filtering fields
             ],
             any=[
-
                 FieldCondition(key='order', matcher=MatchField(8, comparator=operator.ge)),
                 IDCondition(MatchID([1, 2, 3, 4, 5])),  # Support for filtering IDs
             ]
         )
     )
-    print(ids, scores)
-    assert np.array_equal(ids, np.array([2, 1, 4, 5, 10, 3]))
+    assert np.array_equal(ids, np.array([2, 1, 10]))
 
 
 def test_drop_collection():
     db = MinVectorDB(root_url)
     db.drop_collection('test_collection')
     assert 'test_collection' not in db.show_collections()
```

### Comparing `minvectordb-0.3.2/test/standard_tests/test_hmvdb_initial.py` & `minvectordb-0.3.3/test/standard_tests/test_hmvdb_initial.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.2/test/standard_tests/test_smvdb_initial.py` & `minvectordb-0.3.3/test/standard_tests/test_smvdb_initial.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.3.2/test/standard_tests/test_smvdb_save_and_query.py` & `minvectordb-0.3.3/test/standard_tests/test_smvdb_save_and_query.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import shutil
 from pathlib import Path
 
+import pytest
+
 from test import StandaloneMinVectorDB, Filter, FieldCondition, MatchField, IDCondition, MatchID
 import numpy as np
 
 
 def get_database(dim=100, database_path='test_min_vec', chunk_size=1000, dtypes='float32'):
     if Path(database_path).exists():
         shutil.rmtree(database_path)
@@ -24,15 +26,15 @@
         database.bulk_add_items(items)
 
     return database
 
 
 def test_add_single_item_without_id_and_field():
     database = get_database()
-    id = database.add_item(np.ones(100))
+    id = database.add_item(np.ones(100), id=1)
 
     database.commit()
 
     assert database._matrix_serializer.database == []
     assert database._matrix_serializer.fields == []
     assert database._matrix_serializer.indices == []
 
@@ -56,15 +58,15 @@
     database.delete()
 
 
 def test_bulk_add_item_without_id_and_field():
     database = get_database()
     items = []
     for i in range(101):
-        items.append((np.ones(100),))
+        items.append((np.ones(100),i))
 
     database.bulk_add_items(items)
 
     database.commit()
     assert database._matrix_serializer.database == []
     assert database._matrix_serializer.fields == []
     assert database._matrix_serializer.indices == []
@@ -296,20 +298,21 @@
     vec = np.random.random(100)
     n, d = database.query(
         vec, k=12, query_filter=Filter(
             must=[
                 IDCondition(MatchID(list(range(10, 20)) + list(range(70, 80))))
             ],
             any=[
-                FieldCondition(key="测试", matcher=MatchField('测试_1')),
-                FieldCondition(key="测试", matcher=MatchField('测试_7')),
+                FieldCondition(key="test", matcher=MatchField('测试_1')),
+                FieldCondition(key="test", matcher=MatchField('测试_7')),
             ]
         )
     )
 
+    print(n)
     assert len(n) == len(d) == 12
     assert list(d) == sorted(d, key=lambda s: -s)
     assert all(i in database._id_filter for i in n)
     assert all((10 <= i < 20) or (70 <= i < 80) for i in n)
 
     database.delete()
 
@@ -343,46 +346,54 @@
 
 
 # Test whether calling bulk_add_items multiple times can insert data normally
 def test_multiple_bulk_add_items():
     database = get_database()
     items = []
     for i in range(101):
-        items.append((np.ones(100),))
+        items.append((np.ones(100), i))
 
     database.bulk_add_items(items)
     assert len(database._matrix_serializer.fields) == 101
     assert database._matrix_serializer.indices == list(range(101))
 
     database.commit()
     assert database.shape == (101, 100)
 
+    items = []
+    for i in range(101):
+        items.append((np.ones(100), i + 101))
+
     database.bulk_add_items(items)
     database.commit()
     assert database._matrix_serializer.fields == []
     assert database._matrix_serializer.indices == []
 
     assert database.shape == (202, 100)
 
     database.delete()
 
 
 def test_multiple_bulk_add_items_with_insert_session():
     database = get_database()
     items = []
     for i in range(101):
-        items.append((np.ones(100),))
+        items.append((np.ones(100), i))
 
     with database.insert_session():
         database.bulk_add_items(items)
         assert len(database._matrix_serializer.fields) == 101
         assert database._matrix_serializer.indices == list(range(101))
 
     assert database.shape == (101, 100)
 
+    items = []
+    for i in range(101, 202):
+        items.append((np.ones(100), i))
+
     with database.insert_session():
         database.bulk_add_items(items)
 
     assert database._matrix_serializer.fields == []
     assert database._matrix_serializer.indices == []
 
     assert database.shape == (202, 100)
@@ -405,15 +416,15 @@
     assert database.shape == (101, 100)
     del database
 
     database = StandaloneMinVectorDB(dim=dim, database_path=database_path, chunk_size=chunk_size, dtypes=dtypes)
 
     items = []
     for i in range(101):
-        items.append((np.ones(100), None, {"test": "test_" + str(i // 10)}))
+        items.append((np.ones(100), i + 101, {"test": "test_" + str(i // 10)}))
     # insert
     with database.insert_session():
         database.bulk_add_items(items)
 
     assert database._matrix_serializer.fields == []
     assert database._matrix_serializer.indices == []
 
@@ -476,7 +487,137 @@
             db.add_item(np.random.rand(1024), id=i)
 
     out, err = capsys.readouterr()
     assert 'Refitting the index for cluster' in err
     assert db._matrix_serializer.ann_model.fitted
 
     db.delete()
+
+
+def test_transactions():
+    db = StandaloneMinVectorDB(dim=1024, database_path='test_min_vec', chunk_size=10000, index_mode='IVF-FLAT')
+
+    def get_test_vectors(shape):
+        for i in range(shape[0]):
+            yield np.random.random(shape[1])
+
+    with db.insert_session():
+        id = 0
+        vectors = []
+        for t in get_test_vectors((100000, 1024)):
+            vectors.append((t, id))
+            id += 1
+
+        db.bulk_add_items(vectors, batch_size=1000)
+
+    assert db.shape == (100000, 1024)
+
+    with pytest.raises(ValueError):
+        with db.insert_session():
+            id = 0
+            vectors = []
+            for t in get_test_vectors((100000, 1024)):
+                vectors.append((t, id))
+                id += 1
+            db.bulk_add_items(vectors, batch_size=1000)
+
+    assert db.shape == (100000, 1024)
+
+    with pytest.raises(ValueError):
+        db.bulk_add_items(vectors, batch_size=1000)
+
+    assert db.shape == (100000, 1024)
+
+
+def test_filter():
+    database = get_database_for_query(with_field=True)
+
+    vec = np.random.random(100)
+    n, d = database.query(
+        vec, k=6, query_filter=Filter(
+            must=[FieldCondition(key="test", matcher=MatchField('test_1'))]
+        )
+    )
+
+    assert len(n) == len(d) == 6
+    assert list(d) == sorted(d, key=lambda s: -s)
+    assert all(i in database._id_filter for i in n)
+    assert all(10 <= i < 20 for i in n)
+
+    n, d = database.query(
+        vec, k=6, query_filter=Filter(
+            must=[FieldCondition(key="test", matcher=MatchField('test_1'))],
+            any=[FieldCondition(key="test", matcher=MatchField('test_7'))]
+        )
+    )
+
+    assert len(n) == len(d) == 0
+
+    n, d = database.query(
+        vec, k=6, query_filter=Filter(
+            must=[FieldCondition(key="test", matcher=MatchField('test_1'))],
+            any=[FieldCondition(key="test", matcher=MatchField('test_0'))],
+            must_not=[FieldCondition(key="test", matcher=MatchField('test_0'))]
+        )
+    )
+
+    assert len(n) == len(d) == 0
+
+    n, d = database.query(
+        vec, k=6, query_filter=Filter(
+            must=[IDCondition(MatchID([1, 2, 3]))],
+            any=[FieldCondition(key="test", matcher=MatchField('test_0'))],
+        )
+    )
+
+    assert len(n) == len(d) == 3
+    assert list(d) == sorted(d, key=lambda s: -s)
+    assert all(i in database._id_filter for i in n)
+    assert all(1 <= i < 4 for i in n)
+
+    n, d = database.query(
+        vec, k=6, query_filter=Filter(
+            must=[IDCondition(MatchID([1, 2, 3]))],
+            any=[FieldCondition(key="test", matcher=MatchField('test_0'))],
+            must_not=[FieldCondition(key="test", matcher=MatchField('test_0'))]
+        )
+    )
+
+    assert len(n) == len(d) == 0
+
+    n, d = database.query(
+        vec, k=6, query_filter=Filter(
+            must=[IDCondition(MatchID([1, 2, 3]))],
+            any=[FieldCondition(key="test", matcher=MatchField('test_0'))],
+            must_not=[IDCondition(MatchID([1, 2, 3]))]
+        )
+    )
+
+    assert len(n) == len(d) == 0
+
+    n, d = database.query(
+        vec, k=6, query_filter=Filter(
+            must=[IDCondition(MatchID([1, 2, 3]))],
+            any=[FieldCondition(key="test", matcher=MatchField('test_0'))],
+            must_not=[IDCondition(MatchID([4, 5, 6]))]
+        )
+    )
+
+    assert len(n) == len(d) == 3
+    assert list(d) == sorted(d, key=lambda s: -s)
+    assert all(i in database._id_filter for i in n)
+    assert all(1 <= i < 4 for i in n)
+
+    n, d = database.query(
+        vec, k=6, query_filter=Filter(
+        must=[
+            FieldCondition(key='test', matcher=MatchField('test_0')),
+        ],
+        any=[
+            IDCondition(MatchID([1, 2, 3, 4, 5])),
+        ]
+    ))
+
+    assert len(n) == len(d) == 5
+    assert list(d) == sorted(d, key=lambda s: -s)
+    assert all(i in database._id_filter for i in n)
+    assert all(0 <= i < 6 for i in n)
```

