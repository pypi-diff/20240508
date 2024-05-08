# Comparing `tmp/vantage6-4.4.0rc3.tar.gz` & `tmp/vantage6-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-4.4.0rc3.tar", last modified: Mon Apr 15 13:15:19 2024, max compression
+gzip compressed data, was "vantage6-4.4.1.tar", last modified: Wed May  8 12:54:34 2024, max compression
```

## Comparing `vantage6-4.4.0rc3.tar` & `vantage6-4.4.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.051506 vantage6-4.4.0rc3/tests_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/tests_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/tests_cli/test_example.py
--rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/tests_cli/test_node_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/tests_cli/test_server_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/tests_cli/test_wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.047506 vantage6-4.4.0rc3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.051506 vantage6-4.4.0rc3/vantage6/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/__build__
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.051506 vantage6-4.4.0rc3/vantage6/cli/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algorithm/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algorithm/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.055506 vantage6-4.4.0rc3/vantage6/cli/algostore/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algostore/attach.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algostore/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algostore/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algostore/new.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algostore/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algostore/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.055506 vantage6-4.4.0rc3/vantage6/cli/common/
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/common/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/common/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    17949 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/configuration_wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.055506 vantage6-4.4.0rc3/vantage6/cli/context/
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/context/algorithm_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/context/base_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/context/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/context/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.055506 vantage6-4.4.0rc3/vantage6/cli/dev/
--rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/dev/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/dev/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/dev/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/dev/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.055506 vantage6-4.4.0rc3/vantage6/cli/node/
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/attach.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.055506 vantage6-4.4.0rc3/vantage6/cli/node/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/create_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/new.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/set_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11893 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/vantage6/cli/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/rabbitmq/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/rabbitmq/queue_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/rabbitmq/rabbitmq.config
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/vantage6/cli/server/
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/attach.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/vantage6/cli/server/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/import_.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/new.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/vantage6/cli/template/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/template/node_config.j2
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/template/server_config.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/template/server_import_config.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/vantage6/cli/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/vantage6/cli/test/common/
--rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/test/common/diagnostic_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/test/feature_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/test/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.051506 vantage6-4.4.0rc3/vantage6.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-04-15 13:15:19.000000 vantage6-4.4.0rc3/vantage6.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-15 13:15:19.000000 vantage6-4.4.0rc3/vantage6.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:15:19.000000 vantage6-4.4.0rc3/vantage6.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-15 13:15:19.000000 vantage6-4.4.0rc3/vantage6.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-15 13:15:19.000000 vantage6-4.4.0rc3/vantage6.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 13:15:19.000000 vantage6-4.4.0rc3/vantage6.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.256867 vantage6-4.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-05-08 12:54:34.256867 vantage6-4.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:54:34.256867 vantage6-4.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-08 12:54:22.000000 vantage6-4.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.244867 vantage6-4.4.1/tests_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:22.000000 vantage6-4.4.1/tests_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-08 12:54:22.000000 vantage6-4.4.1/tests_cli/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-05-08 12:54:22.000000 vantage6-4.4.1/tests_cli/test_node_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-08 12:54:22.000000 vantage6-4.4.1/tests_cli/test_server_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-08 12:54:22.000000 vantage6-4.4.1/tests_cli/test_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.244867 vantage6-4.4.1/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.248867 vantage6-4.4.1/vantage6/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.248867 vantage6-4.4.1/vantage6/cli/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/algorithm/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/algorithm/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.248867 vantage6-4.4.1/vantage6/cli/algostore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/algostore/attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/algostore/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/algostore/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/algostore/new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/algostore/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/algostore/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.248867 vantage6-4.4.1/vantage6/cli/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/common/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/common/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17949 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/configuration_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.248867 vantage6-4.4.1/vantage6/cli/context/
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/context/algorithm_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/context/base_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/context/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/context/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.252867 vantage6-4.4.1/vantage6/cli/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/dev/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/dev/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/dev/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/dev/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.252867 vantage6-4.4.1/vantage6/cli/node/
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/node/attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/node/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.252867 vantage6-4.4.1/vantage6/cli/node/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/node/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/node/create_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/node/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/node/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/node/new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/node/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/node/set_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11893 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/node/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/node/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/node/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.252867 vantage6-4.4.1/vantage6/cli/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/rabbitmq/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/rabbitmq/queue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/rabbitmq/rabbitmq.config
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.252867 vantage6-4.4.1/vantage6/cli/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/server/attach.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.252867 vantage6-4.4.1/vantage6/cli/server/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/server/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/server/import_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/server/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/server/new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/server/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/server/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/server/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/server/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.256867 vantage6-4.4.1/vantage6/cli/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/template/node_config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/template/server_config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/template/server_import_config.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.256867 vantage6-4.4.1/vantage6/cli/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.256867 vantage6-4.4.1/vantage6/cli/test/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/test/common/diagnostic_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/test/feature_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/test/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-08 12:54:22.000000 vantage6-4.4.1/vantage6/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:34.244867 vantage6-4.4.1/vantage6.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-05-08 12:54:34.000000 vantage6-4.4.1/vantage6.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-08 12:54:34.000000 vantage6-4.4.1/vantage6.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:54:34.000000 vantage6-4.4.1/vantage6.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-08 12:54:34.000000 vantage6-4.4.1/vantage6.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-08 12:54:34.000000 vantage6-4.4.1/vantage6.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 12:54:34.000000 vantage6-4.4.1/vantage6.egg-info/top_level.txt
```

### Comparing `vantage6-4.4.0rc3/PKG-INFO` & `vantage6-4.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 4.4.0rc3
+Version: 4.4.1
 Summary: vantage6 command line interface
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 4.4.0rc3 Summary: vantage6
-command line interface Home-page: https://github.com/vantage6/vantage6
-Requires-Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra:
-dev
+Metadata-Version: 2.1 Name: vantage6 Version: 4.4.1 Summary: vantage6 command
+line interface Home-page: https://github.com/vantage6/vantage6 Requires-Python:
+>=3.10 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll)) [[!![[PPyyPPII vvaannttaaggee66]]((hhttttppss::////bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66..ssvvgg))]]((hhttttppss::////
 bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66)) [[!![[UUnniitttteessttss]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//
```

### Comparing `vantage6-4.4.0rc3/setup.py` & `vantage6-4.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     python_requires=">=3.10",
     install_requires=[
         "click==8.1.3",
         "colorama==0.4.6",
         "copier==9.2.0",
         "docker==6.1.2",
         "ipython==8.10.0",
-        "jinja2==3.1.3",
+        "jinja2==3.1.4",
         "questionary==1.10.0",
         "rich==13.5.2",
         "schema==0.7.5",
         "SQLAlchemy==1.4.46",
         f'vantage6-common == {version_ns["__version__"]}',
         f'vantage6-client == {version_ns["__version__"]}',
     ],
```

### Comparing `vantage6-4.4.0rc3/tests_cli/test_node_cli.py` & `vantage6-4.4.1/tests_cli/test_node_cli.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/tests_cli/test_server_cli.py` & `vantage6-4.4.1/tests_cli/test_server_cli.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/tests_cli/test_wizard.py` & `vantage6-4.4.1/tests_cli/test_wizard.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/_version.py` & `vantage6-4.4.1/vantage6/cli/_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "__build__")) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (4, 4, 0, "candidate", __build__, 0)
+version_info = (4, 4, 1, "final", __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {"alpha": "a", "beta": "b", "candidate": "rc", "final": ""}
 version = f"{version_info[0]}.{version_info[1]}.{version_info[2]}"
 pre_release = (
     ""
     if version_info[3] == "final"
```

### Comparing `vantage6-4.4.0rc3/vantage6/cli/algorithm/create.py` & `vantage6-4.4.1/vantage6/cli/algorithm/create.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/algorithm/update.py` & `vantage6-4.4.1/vantage6/cli/algorithm/update.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/algostore/attach.py` & `vantage6-4.4.1/vantage6/cli/algostore/attach.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/algostore/files.py` & `vantage6-4.4.1/vantage6/cli/algostore/files.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/algostore/new.py` & `vantage6-4.4.1/vantage6/cli/algostore/new.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/algostore/start.py` & `vantage6-4.4.1/vantage6/cli/algostore/start.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/algostore/stop.py` & `vantage6-4.4.1/vantage6/cli/algostore/stop.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/cli.py` & `vantage6-4.4.1/vantage6/cli/cli.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/common/decorator.py` & `vantage6-4.4.1/vantage6/cli/common/decorator.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/common/start.py` & `vantage6-4.4.1/vantage6/cli/common/start.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/common/utils.py` & `vantage6-4.4.1/vantage6/cli/common/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/configuration_manager.py` & `vantage6-4.4.1/vantage6/cli/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/configuration_wizard.py` & `vantage6-4.4.1/vantage6/cli/configuration_wizard.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/context/__init__.py` & `vantage6-4.4.1/vantage6/cli/context/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/context/algorithm_store.py` & `vantage6-4.4.1/vantage6/cli/context/algorithm_store.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/context/base_server.py` & `vantage6-4.4.1/vantage6/cli/context/base_server.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/context/node.py` & `vantage6-4.4.1/vantage6/cli/context/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/context/server.py` & `vantage6-4.4.1/vantage6/cli/context/server.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/dev/create.py` & `vantage6-4.4.1/vantage6/cli/dev/create.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/dev/remove.py` & `vantage6-4.4.1/vantage6/cli/dev/remove.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/dev/start.py` & `vantage6-4.4.1/vantage6/cli/dev/start.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/dev/stop.py` & `vantage6-4.4.1/vantage6/cli/dev/stop.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/globals.py` & `vantage6-4.4.1/vantage6/cli/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/node/attach.py` & `vantage6-4.4.1/vantage6/cli/node/attach.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/node/clean.py` & `vantage6-4.4.1/vantage6/cli/node/clean.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/node/common/__init__.py` & `vantage6-4.4.1/vantage6/cli/node/common/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/node/create_private_key.py` & `vantage6-4.4.1/vantage6/cli/node/create_private_key.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/node/files.py` & `vantage6-4.4.1/vantage6/cli/node/files.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/node/list.py` & `vantage6-4.4.1/vantage6/cli/node/list.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/node/new.py` & `vantage6-4.4.1/vantage6/cli/node/new.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/node/remove.py` & `vantage6-4.4.1/vantage6/cli/node/remove.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/node/set_api_key.py` & `vantage6-4.4.1/vantage6/cli/node/set_api_key.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/node/start.py` & `vantage6-4.4.1/vantage6/cli/node/start.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/node/stop.py` & `vantage6-4.4.1/vantage6/cli/node/stop.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/node/version.py` & `vantage6-4.4.1/vantage6/cli/node/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/rabbitmq/__init__.py` & `vantage6-4.4.1/vantage6/cli/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/rabbitmq/definitions.py` & `vantage6-4.4.1/vantage6/cli/rabbitmq/definitions.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/rabbitmq/queue_manager.py` & `vantage6-4.4.1/vantage6/cli/rabbitmq/queue_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/server/attach.py` & `vantage6-4.4.1/vantage6/cli/server/attach.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/server/common/__init__.py` & `vantage6-4.4.1/vantage6/cli/server/common/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/server/import_.py` & `vantage6-4.4.1/vantage6/cli/server/import_.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/server/new.py` & `vantage6-4.4.1/vantage6/cli/server/new.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/server/remove.py` & `vantage6-4.4.1/vantage6/cli/server/remove.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/server/shell.py` & `vantage6-4.4.1/vantage6/cli/server/shell.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/server/start.py` & `vantage6-4.4.1/vantage6/cli/server/start.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/server/stop.py` & `vantage6-4.4.1/vantage6/cli/server/stop.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/server/version.py` & `vantage6-4.4.1/vantage6/cli/server/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/template/node_config.j2` & `vantage6-4.4.1/vantage6/cli/template/node_config.j2`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/template/server_import_config.j2` & `vantage6-4.4.1/vantage6/cli/template/server_import_config.j2`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/test/common/diagnostic_runner.py` & `vantage6-4.4.1/vantage6/cli/test/common/diagnostic_runner.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/test/feature_tester.py` & `vantage6-4.4.1/vantage6/cli/test/feature_tester.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/test/integration_test.py` & `vantage6-4.4.1/vantage6/cli/test/integration_test.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6/cli/utils.py` & `vantage6-4.4.1/vantage6/cli/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.4.0rc3/vantage6.egg-info/PKG-INFO` & `vantage6-4.4.1/vantage6.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 4.4.0rc3
+Version: 4.4.1
 Summary: vantage6 command line interface
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 4.4.0rc3 Summary: vantage6
-command line interface Home-page: https://github.com/vantage6/vantage6
-Requires-Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra:
-dev
+Metadata-Version: 2.1 Name: vantage6 Version: 4.4.1 Summary: vantage6 command
+line interface Home-page: https://github.com/vantage6/vantage6 Requires-Python:
+>=3.10 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll)) [[!![[PPyyPPII vvaannttaaggee66]]((hhttttppss::////bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66..ssvvgg))]]((hhttttppss::////
 bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66)) [[!![[UUnniitttteessttss]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//
```

### Comparing `vantage6-4.4.0rc3/vantage6.egg-info/SOURCES.txt` & `vantage6-4.4.1/vantage6.egg-info/SOURCES.txt`

 * *Files identical despite different names*

