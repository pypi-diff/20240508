# Comparing `tmp/aiozk-0.8.0.tar.gz` & `tmp/aiozk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiozk-0.8.0.tar", last modified: Mon Jun 18 08:41:26 2018, max compression
+gzip compressed data, was "dist/aiozk-0.9.0.tar", last modified: Tue Jun 19 22:28:58 2018, max compression
```

## Comparing `aiozk-0.8.0.tar` & `aiozk-0.9.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 kpi       (1000) kpi       (1000)        0 2018-06-18 08:41:26.000000 aiozk-0.8.0/
-drwxr-xr-x   0 kpi       (1000) kpi       (1000)        0 2018-06-18 08:41:26.000000 aiozk-0.8.0/aiozk.egg-info/
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1060 2018-06-18 08:41:26.000000 aiozk-0.8.0/aiozk.egg-info/PKG-INFO
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1535 2018-06-18 08:41:26.000000 aiozk-0.8.0/aiozk.egg-info/SOURCES.txt
--rw-r--r--   0 kpi       (1000) kpi       (1000)        1 2018-06-18 08:41:26.000000 aiozk-0.8.0/aiozk.egg-info/dependency_links.txt
--rw-r--r--   0 kpi       (1000) kpi       (1000)        6 2018-06-18 08:41:26.000000 aiozk-0.8.0/aiozk.egg-info/top_level.txt
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1498 2018-06-16 10:02:31.000000 aiozk-0.8.0/setup.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1060 2018-06-18 08:41:26.000000 aiozk-0.8.0/PKG-INFO
--rw-r--r--   0 kpi       (1000) kpi       (1000)     4618 2018-06-16 09:58:07.000000 aiozk-0.8.0/README.md
-drwxr-xr-x   0 kpi       (1000) kpi       (1000)        0 2018-06-18 08:41:26.000000 aiozk-0.8.0/aiozk/
-drwxr-xr-x   0 kpi       (1000) kpi       (1000)        0 2018-06-18 08:41:26.000000 aiozk-0.8.0/aiozk/protocol/
--rw-r--r--   0 kpi       (1000) kpi       (1000)     2805 2016-08-30 14:12:21.000000 aiozk-0.8.0/aiozk/protocol/transaction.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      391 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/auth.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      339 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/delete.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      367 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/exists.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      269 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/close.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      819 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/stat.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      313 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/sasl.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      312 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/sync.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      705 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/children.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      980 2016-08-29 22:26:46.000000 aiozk-0.8.0/aiozk/protocol/response.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      997 2016-08-30 14:32:19.000000 aiozk-0.8.0/aiozk/protocol/request.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      553 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/connect.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      706 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/data.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1099 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/create.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     6579 2016-08-30 09:13:33.000000 aiozk-0.8.0/aiozk/protocol/primitives.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      468 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/reconfig.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     2073 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/acl.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      329 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/check.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1300 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/watches.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     3111 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/part.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1682 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/__init__.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      261 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/protocol/ping.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     2982 2017-04-18 19:25:57.000000 aiozk-0.8.0/aiozk/exc.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     2793 2016-08-30 08:25:47.000000 aiozk-0.8.0/aiozk/transaction.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)    10242 2018-06-16 10:02:31.000000 aiozk-0.8.0/aiozk/session.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      604 2017-04-18 19:25:57.000000 aiozk-0.8.0/aiozk/iterables.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     6493 2018-06-16 09:58:07.000000 aiozk-0.8.0/aiozk/client.py
-drwxr-xr-x   0 kpi       (1000) kpi       (1000)        0 2018-06-18 08:41:26.000000 aiozk-0.8.0/aiozk/test/
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1106 2018-06-16 09:58:07.000000 aiozk-0.8.0/aiozk/test/test_barrier.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     2084 2018-06-16 09:58:07.000000 aiozk-0.8.0/aiozk/test/test_treecache.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1707 2018-06-16 09:58:07.000000 aiozk-0.8.0/aiozk/test/conftest.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     4002 2018-06-16 09:58:07.000000 aiozk-0.8.0/aiozk/test/test_watchers.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)        0 2016-09-02 14:59:45.000000 aiozk-0.8.0/aiozk/test/__init__.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      918 2018-06-18 08:40:57.000000 aiozk-0.8.0/aiozk/test/test_shared_lock.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      823 2018-06-16 09:58:07.000000 aiozk-0.8.0/aiozk/test/test_client.py
-drwxr-xr-x   0 kpi       (1000) kpi       (1000)        0 2018-06-18 08:41:26.000000 aiozk-0.8.0/aiozk/recipes/
--rw-r--r--   0 kpi       (1000) kpi       (1000)     2289 2017-05-29 12:43:20.000000 aiozk-0.8.0/aiozk/recipes/counter.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      309 2018-06-16 09:58:07.000000 aiozk-0.8.0/aiozk/recipes/children_watcher.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     3818 2018-06-16 09:58:07.000000 aiozk-0.8.0/aiozk/recipes/tree_cache.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     3730 2017-05-29 12:43:20.000000 aiozk-0.8.0/aiozk/recipes/allocator.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1409 2018-06-18 08:40:55.000000 aiozk-0.8.0/aiozk/recipes/election.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1862 2016-10-21 19:15:38.000000 aiozk-0.8.0/aiozk/recipes/proxy.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1721 2018-06-16 09:58:07.000000 aiozk-0.8.0/aiozk/recipes/base_watcher.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     2256 2018-06-18 08:40:57.000000 aiozk-0.8.0/aiozk/recipes/base_lock.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1299 2017-05-29 12:43:20.000000 aiozk-0.8.0/aiozk/recipes/party.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      289 2018-06-16 09:58:07.000000 aiozk-0.8.0/aiozk/recipes/data_watcher.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1194 2016-08-29 22:29:21.000000 aiozk-0.8.0/aiozk/recipes/recipe.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1074 2018-06-18 08:40:55.000000 aiozk-0.8.0/aiozk/recipes/barrier.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)       74 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/recipes/__init__.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      673 2016-08-31 19:46:30.000000 aiozk-0.8.0/aiozk/recipes/shared_lock.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      993 2018-06-18 08:40:55.000000 aiozk-0.8.0/aiozk/recipes/lease.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      337 2017-04-18 19:25:57.000000 aiozk-0.8.0/aiozk/recipes/lock.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     2299 2018-06-18 08:40:55.000000 aiozk-0.8.0/aiozk/recipes/double_barrier.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     2422 2018-06-18 08:40:55.000000 aiozk-0.8.0/aiozk/recipes/sequential.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     2124 2017-05-29 12:43:20.000000 aiozk-0.8.0/aiozk/retry.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     9825 2018-06-16 10:02:31.000000 aiozk-0.8.0/aiozk/connection.py
--rw-------   0 kpi       (1000) kpi       (1000)      216 2018-06-18 08:41:03.000000 aiozk-0.8.0/aiozk/__init__.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1878 2017-05-29 12:43:20.000000 aiozk-0.8.0/aiozk/states.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)      324 2016-08-29 21:50:38.000000 aiozk-0.8.0/aiozk/features.py
--rw-r--r--   0 kpi       (1000) kpi       (1000)       38 2018-06-18 08:41:26.000000 aiozk-0.8.0/setup.cfg
--rw-r--r--   0 kpi       (1000) kpi       (1000)     1057 2016-08-30 10:07:53.000000 aiozk-0.8.0/LICENSE
+drwxr-xr-x   0 kpi       (1000) kpi       (1000)        0 2018-06-19 22:28:58.000000 aiozk-0.9.0/
+drwxr-xr-x   0 kpi       (1000) kpi       (1000)        0 2018-06-19 22:28:58.000000 aiozk-0.9.0/aiozk.egg-info/
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1060 2018-06-19 22:28:58.000000 aiozk-0.9.0/aiozk.egg-info/PKG-INFO
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1535 2018-06-19 22:28:58.000000 aiozk-0.9.0/aiozk.egg-info/SOURCES.txt
+-rw-r--r--   0 kpi       (1000) kpi       (1000)        1 2018-06-19 22:28:58.000000 aiozk-0.9.0/aiozk.egg-info/dependency_links.txt
+-rw-r--r--   0 kpi       (1000) kpi       (1000)        6 2018-06-19 22:28:58.000000 aiozk-0.9.0/aiozk.egg-info/top_level.txt
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1498 2018-06-16 10:02:31.000000 aiozk-0.9.0/setup.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1060 2018-06-19 22:28:58.000000 aiozk-0.9.0/PKG-INFO
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     4618 2018-06-16 09:58:07.000000 aiozk-0.9.0/README.md
+drwxr-xr-x   0 kpi       (1000) kpi       (1000)        0 2018-06-19 22:28:58.000000 aiozk-0.9.0/aiozk/
+drwxr-xr-x   0 kpi       (1000) kpi       (1000)        0 2018-06-19 22:28:58.000000 aiozk-0.9.0/aiozk/protocol/
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     2805 2016-08-30 14:12:21.000000 aiozk-0.9.0/aiozk/protocol/transaction.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      391 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/auth.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      339 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/delete.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      367 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/exists.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      269 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/close.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      819 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/stat.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      313 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/sasl.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      312 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/sync.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      705 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/children.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      980 2016-08-29 22:26:46.000000 aiozk-0.9.0/aiozk/protocol/response.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      997 2016-08-30 14:32:19.000000 aiozk-0.9.0/aiozk/protocol/request.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      553 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/connect.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      706 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/data.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1099 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/create.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     6579 2016-08-30 09:13:33.000000 aiozk-0.9.0/aiozk/protocol/primitives.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      468 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/reconfig.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     2073 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/acl.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      329 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/check.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1300 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/watches.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     3111 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/part.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1682 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/__init__.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      261 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/protocol/ping.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     2982 2017-04-18 19:25:57.000000 aiozk-0.9.0/aiozk/exc.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     2793 2016-08-30 08:25:47.000000 aiozk-0.9.0/aiozk/transaction.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)    10411 2018-06-19 22:28:48.000000 aiozk-0.9.0/aiozk/session.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      604 2017-04-18 19:25:57.000000 aiozk-0.9.0/aiozk/iterables.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     6493 2018-06-16 09:58:07.000000 aiozk-0.9.0/aiozk/client.py
+drwxr-xr-x   0 kpi       (1000) kpi       (1000)        0 2018-06-19 22:28:58.000000 aiozk-0.9.0/aiozk/test/
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1106 2018-06-16 09:58:07.000000 aiozk-0.9.0/aiozk/test/test_barrier.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     2084 2018-06-16 09:58:07.000000 aiozk-0.9.0/aiozk/test/test_treecache.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1707 2018-06-16 09:58:07.000000 aiozk-0.9.0/aiozk/test/conftest.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     4002 2018-06-16 09:58:07.000000 aiozk-0.9.0/aiozk/test/test_watchers.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)        0 2016-09-02 14:59:45.000000 aiozk-0.9.0/aiozk/test/__init__.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      918 2018-06-18 08:40:57.000000 aiozk-0.9.0/aiozk/test/test_shared_lock.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      982 2018-06-19 22:28:48.000000 aiozk-0.9.0/aiozk/test/test_client.py
+drwxr-xr-x   0 kpi       (1000) kpi       (1000)        0 2018-06-19 22:28:58.000000 aiozk-0.9.0/aiozk/recipes/
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     2289 2017-05-29 12:43:20.000000 aiozk-0.9.0/aiozk/recipes/counter.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      309 2018-06-16 09:58:07.000000 aiozk-0.9.0/aiozk/recipes/children_watcher.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     3818 2018-06-16 09:58:07.000000 aiozk-0.9.0/aiozk/recipes/tree_cache.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     3730 2017-05-29 12:43:20.000000 aiozk-0.9.0/aiozk/recipes/allocator.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1409 2018-06-18 08:40:55.000000 aiozk-0.9.0/aiozk/recipes/election.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1862 2016-10-21 19:15:38.000000 aiozk-0.9.0/aiozk/recipes/proxy.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1721 2018-06-16 09:58:07.000000 aiozk-0.9.0/aiozk/recipes/base_watcher.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     2256 2018-06-18 08:40:57.000000 aiozk-0.9.0/aiozk/recipes/base_lock.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1299 2017-05-29 12:43:20.000000 aiozk-0.9.0/aiozk/recipes/party.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      289 2018-06-16 09:58:07.000000 aiozk-0.9.0/aiozk/recipes/data_watcher.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1194 2016-08-29 22:29:21.000000 aiozk-0.9.0/aiozk/recipes/recipe.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1074 2018-06-18 08:40:55.000000 aiozk-0.9.0/aiozk/recipes/barrier.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)       74 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/recipes/__init__.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      673 2016-08-31 19:46:30.000000 aiozk-0.9.0/aiozk/recipes/shared_lock.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      993 2018-06-18 08:40:55.000000 aiozk-0.9.0/aiozk/recipes/lease.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      337 2017-04-18 19:25:57.000000 aiozk-0.9.0/aiozk/recipes/lock.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     2299 2018-06-18 08:40:55.000000 aiozk-0.9.0/aiozk/recipes/double_barrier.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     2422 2018-06-18 08:40:55.000000 aiozk-0.9.0/aiozk/recipes/sequential.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     2124 2017-05-29 12:43:20.000000 aiozk-0.9.0/aiozk/retry.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     9825 2018-06-16 10:02:31.000000 aiozk-0.9.0/aiozk/connection.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      216 2018-06-19 22:28:48.000000 aiozk-0.9.0/aiozk/__init__.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1878 2017-05-29 12:43:20.000000 aiozk-0.9.0/aiozk/states.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)      324 2016-08-29 21:50:38.000000 aiozk-0.9.0/aiozk/features.py
+-rw-r--r--   0 kpi       (1000) kpi       (1000)       38 2018-06-19 22:28:58.000000 aiozk-0.9.0/setup.cfg
+-rw-r--r--   0 kpi       (1000) kpi       (1000)     1057 2016-08-30 10:07:53.000000 aiozk-0.9.0/LICENSE
```

### Comparing `aiozk-0.8.0/aiozk.egg-info/PKG-INFO` & `aiozk-0.9.0/aiozk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aiozk
-Version: 0.8.0
+Version: 0.9.0
 Summary: Asyncio client for Zookeeper.
 Home-page: http://github.com/tipsi/aiozk
 Author: Kirill Pinchuk
 Author-email: cybergrind@gmail.com
 Maintainer: Kirill Pinchuk
 Maintainer-email: cybergrind@gmail.com
 License: MIT
```

### Comparing `aiozk-0.8.0/aiozk.egg-info/SOURCES.txt` & `aiozk-0.9.0/aiozk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/setup.py` & `aiozk-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/PKG-INFO` & `aiozk-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aiozk
-Version: 0.8.0
+Version: 0.9.0
 Summary: Asyncio client for Zookeeper.
 Home-page: http://github.com/tipsi/aiozk
 Author: Kirill Pinchuk
 Author-email: cybergrind@gmail.com
 Maintainer: Kirill Pinchuk
 Maintainer-email: cybergrind@gmail.com
 License: MIT
```

### Comparing `aiozk-0.8.0/README.md` & `aiozk-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/protocol/transaction.py` & `aiozk-0.9.0/aiozk/protocol/transaction.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/protocol/stat.py` & `aiozk-0.9.0/aiozk/protocol/stat.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/protocol/children.py` & `aiozk-0.9.0/aiozk/protocol/children.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/protocol/response.py` & `aiozk-0.9.0/aiozk/protocol/response.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/protocol/request.py` & `aiozk-0.9.0/aiozk/protocol/request.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/protocol/connect.py` & `aiozk-0.9.0/aiozk/protocol/connect.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/protocol/data.py` & `aiozk-0.9.0/aiozk/protocol/data.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/protocol/create.py` & `aiozk-0.9.0/aiozk/protocol/create.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/protocol/primitives.py` & `aiozk-0.9.0/aiozk/protocol/primitives.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/protocol/acl.py` & `aiozk-0.9.0/aiozk/protocol/acl.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/protocol/watches.py` & `aiozk-0.9.0/aiozk/protocol/watches.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/protocol/part.py` & `aiozk-0.9.0/aiozk/protocol/part.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/protocol/__init__.py` & `aiozk-0.9.0/aiozk/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/exc.py` & `aiozk-0.9.0/aiozk/exc.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/transaction.py` & `aiozk-0.9.0/aiozk/transaction.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/session.py` & `aiozk-0.9.0/aiozk/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,10 +283,13 @@
 
     async def close(self):
         if self.closing:
             return
         self.closing = True
         if self.repair_loop_task:
             self.repair_loop_task.cancel()
-        await self.send(protocol.CloseRequest())
-        self.state.transition_to(States.LOST)
-        await self.conn.close(self.timeout)
+            await asyncio.wait_for(self.send(protocol.CloseRequest()), self.timeout,
+                                   loop=self.loop)
+        if self.state.current_state != States.LOST:
+            self.state.transition_to(States.LOST)
+        if self.conn:
+            await self.conn.close(self.timeout)
```

### Comparing `aiozk-0.8.0/aiozk/iterables.py` & `aiozk-0.9.0/aiozk/iterables.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/client.py` & `aiozk-0.9.0/aiozk/client.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/test/test_barrier.py` & `aiozk-0.9.0/aiozk/test/test_barrier.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/test/test_treecache.py` & `aiozk-0.9.0/aiozk/test/test_treecache.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/test/conftest.py` & `aiozk-0.9.0/aiozk/test/conftest.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/test/test_watchers.py` & `aiozk-0.9.0/aiozk/test/test_watchers.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/test/test_shared_lock.py` & `aiozk-0.9.0/aiozk/test/test_shared_lock.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/test/test_client.py` & `aiozk-0.9.0/aiozk/test/test_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import logging
 import uuid
 import pytest
 
 from aiozk import WatchEvent
+from .conftest import get_client
 
 
 logging.getLogger('asyncio').setLevel(logging.DEBUG)
 
 
 @pytest.fixture
 async def full_zk(zk, path):
@@ -32,7 +33,13 @@
 async def test_cancel_crash(zk, path):
     async def wait_loop():
         while 1:
             await zk.wait_for_events([WatchEvent.DATA_CHANGED], path)
 
     f = asyncio.ensure_future(wait_loop())
     f.cancel()
+
+
+@pytest.mark.asyncio
+async def test_closed_close():
+    zk = get_client()
+    await asyncio.wait_for(zk.session.close(), 2)
```

### Comparing `aiozk-0.8.0/aiozk/recipes/counter.py` & `aiozk-0.9.0/aiozk/recipes/counter.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/recipes/tree_cache.py` & `aiozk-0.9.0/aiozk/recipes/tree_cache.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/recipes/allocator.py` & `aiozk-0.9.0/aiozk/recipes/allocator.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/recipes/election.py` & `aiozk-0.9.0/aiozk/recipes/election.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/recipes/proxy.py` & `aiozk-0.9.0/aiozk/recipes/proxy.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/recipes/base_watcher.py` & `aiozk-0.9.0/aiozk/recipes/base_watcher.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/recipes/base_lock.py` & `aiozk-0.9.0/aiozk/recipes/base_lock.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/recipes/party.py` & `aiozk-0.9.0/aiozk/recipes/party.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/recipes/recipe.py` & `aiozk-0.9.0/aiozk/recipes/recipe.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/recipes/barrier.py` & `aiozk-0.9.0/aiozk/recipes/barrier.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/recipes/shared_lock.py` & `aiozk-0.9.0/aiozk/recipes/shared_lock.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/recipes/lease.py` & `aiozk-0.9.0/aiozk/recipes/lease.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/recipes/double_barrier.py` & `aiozk-0.9.0/aiozk/recipes/double_barrier.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/recipes/sequential.py` & `aiozk-0.9.0/aiozk/recipes/sequential.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/retry.py` & `aiozk-0.9.0/aiozk/retry.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/connection.py` & `aiozk-0.9.0/aiozk/connection.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/aiozk/states.py` & `aiozk-0.9.0/aiozk/states.py`

 * *Files identical despite different names*

### Comparing `aiozk-0.8.0/LICENSE` & `aiozk-0.9.0/LICENSE`

 * *Files identical despite different names*

