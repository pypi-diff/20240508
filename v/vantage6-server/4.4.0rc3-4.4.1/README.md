# Comparing `tmp/vantage6-server-4.4.0rc3.tar.gz` & `tmp/vantage6-server-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-server-4.4.0rc3.tar", last modified: Mon Apr 15 13:15:20 2024, max compression
+gzip compressed data, was "vantage6-server-4.4.1.tar", last modified: Wed May  8 12:54:35 2024, max compression
```

## Comparing `vantage6-server-4.4.0rc3.tar` & `vantage6-server-4.4.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.303516 vantage6-server-4.4.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-04-15 13:15:20.303516 vantage6-server-4.4.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:15:20.303516 vantage6-server-4.4.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.287515 vantage6-server-4.4.0rc3/tests_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/tests_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/tests_server/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)   174647 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/tests_server/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.287515 vantage6-server-4.4.0rc3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.291516 vantage6-server-4.4.0rc3/vantage6/server/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/__build__
--rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.291516 vantage6-server-4.4.0rc3/vantage6/server/_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.291516 vantage6-server-4.4.0rc3/vantage6/server/_data/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_data/dev/fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_data/dev/node_a.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_data/dev/node_b.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_data/dev/server.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_data/example_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_data/unittest_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_data/unittest_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/algo_store_communication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.291516 vantage6-server-4.4.0rc3/vantage6/server/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.295516 vantage6-server-4.4.0rc3/vantage6/server/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/controller/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/mail_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.295516 vantage6-server-4.4.0rc3/vantage6/server/model/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/algorithm_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/algorithm_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/authenticatable.py
--rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.295516 vantage6-server-4.4.0rc3/vantage6/server/model/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/member.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/node_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/role.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/role_rule_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/study.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/task_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    18080 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.299516 vantage6-server-4.4.0rc3/vantage6/server/resource/
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22084 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/algorithm_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    31301 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.299516 vantage6-server-4.4.0rc3/vantage6/server/resource/common/
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/common/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19918 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/common/input_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/common/output_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/common/swagger_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    21884 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/node.py
--rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/port.py
--rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/recover.py
--rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    23751 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28647 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/study.py
--rw-r--r--   0 runner    (1001) docker     (127)    40748 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.303516 vantage6-server-4.4.0rc3/vantage6/server/resource/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/ui/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/vpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/websocket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15348 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.303516 vantage6-server-4.4.0rc3/vantage6_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-04-15 13:15:20.000000 vantage6-server-4.4.0rc3/vantage6_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-15 13:15:20.000000 vantage6-server-4.4.0rc3/vantage6_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:15:20.000000 vantage6-server-4.4.0rc3/vantage6_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 13:15:20.000000 vantage6-server-4.4.0rc3/vantage6_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-15 13:15:20.000000 vantage6-server-4.4.0rc3/vantage6_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 13:15:20.000000 vantage6-server-4.4.0rc3/vantage6_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.460864 vantage6-server-4.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-08 12:54:35.460864 vantage6-server-4.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:54:35.460864 vantage6-server-4.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.444864 vantage6-server-4.4.1/tests_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/tests_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/tests_server/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)   174647 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/tests_server/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.444864 vantage6-server-4.4.1/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.448864 vantage6-server-4.4.1/vantage6/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.448864 vantage6-server-4.4.1/vantage6/server/_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.448864 vantage6-server-4.4.1/vantage6/server/_data/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_data/dev/fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_data/dev/node_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_data/dev/node_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_data/dev/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_data/example_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_data/unittest_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_data/unittest_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/algo_store_communication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.448864 vantage6-server-4.4.1/vantage6/server/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.448864 vantage6-server-4.4.1/vantage6/server/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/controller/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/mail_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.452864 vantage6-server-4.4.1/vantage6/server/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/algorithm_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/algorithm_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/authenticatable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.452864 vantage6-server-4.4.1/vantage6/server/model/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/node_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/role_rule_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/study.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/task_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18080 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.456864 vantage6-server-4.4.1/vantage6/server/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22084 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/algorithm_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31301 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.456864 vantage6-server-4.4.1/vantage6/server/resource/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/common/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19918 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/common/input_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/common/output_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/common/swagger_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21884 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/recover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23751 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28647 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/study.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40748 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.456864 vantage6-server-4.4.1/vantage6/server/resource/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/ui/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/websocket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15348 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.456864 vantage6-server-4.4.1/vantage6_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-08 12:54:35.000000 vantage6-server-4.4.1/vantage6_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-08 12:54:35.000000 vantage6-server-4.4.1/vantage6_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:54:35.000000 vantage6-server-4.4.1/vantage6_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 12:54:35.000000 vantage6-server-4.4.1/vantage6_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-08 12:54:35.000000 vantage6-server-4.4.1/vantage6_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 12:54:35.000000 vantage6-server-4.4.1/vantage6_server.egg-info/top_level.txt
```

### Comparing `vantage6-server-4.4.0rc3/PKG-INFO` & `vantage6-server-4.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 4.4.0rc3
+Version: 4.4.1
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 4.4.0rc3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 4.4.1 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-server-4.4.0rc3/setup.py` & `vantage6-server-4.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         "marshmallow==3.19.0",
         "PyJWT==2.6.0",
         "pyotp==2.8.0",
         "requests==2.31.0",
         "requests-oauthlib==1.3.1",
         "schema==0.7.5",
         "SQLAlchemy==1.4.46",
-        "werkzeug==3.0.1",
+        "werkzeug==3.0.3",
         f'vantage6 == {version_ns["__version__"]}',
         f'vantage6-common == {version_ns["__version__"]}',
     ],
     extras_require={
         "dev": [
             "coverage==6.4.4",
             "black",
```

### Comparing `vantage6-server-4.4.0rc3/tests_server/test_models.py` & `vantage6-server-4.4.1/tests_server/test_models.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/tests_server/test_resources.py` & `vantage6-server-4.4.1/tests_server/test_resources.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/__init__.py` & `vantage6-server-4.4.1/vantage6/server/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -136,23 +136,23 @@
         self.permissions = PermissionManager()
 
         # Api - REST JSON-rpc
         self.api = Api(self.app)
         self.configure_api()
         self.load_resources()
 
-        # couple any algoritm stores to the server if defined in config. This should be
-        # done after the resources are loaded to ensure that rules are set up
-        self.couple_algorithm_stores()
-
         # set environment variable for dev environment
         host_uri = self.ctx.config.get("dev", {}).get("host_uri")
         if host_uri:
             os.environ[HOST_URI_ENV] = host_uri
 
+        # couple any algoritm stores to the server if defined in config. This should be
+        # done after the resources are loaded to ensure that rules are set up
+        self.couple_algorithm_stores()
+
         # set the server version
         self.__version__ = __version__
 
         # set up socket ping/pong
         log.debug("Starting thread to set node status")
         t = Thread(target=self.__node_status_worker, daemon=True)
         t.start()
```

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/_data/dev/fixtures.yaml` & `vantage6-server-4.4.1/vantage6/server/_data/dev/fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/_data/dev/node_a.yaml` & `vantage6-server-4.4.1/vantage6/server/_data/dev/node_a.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/_data/dev/node_b.yaml` & `vantage6-server-4.4.1/vantage6/server/_data/dev/node_b.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/_data/dev/server.yaml` & `vantage6-server-4.4.1/vantage6/server/_data/dev/server.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/_data/example_fixtures.yaml` & `vantage6-server-4.4.1/vantage6/server/_data/example_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/_data/unittest_config.yaml` & `vantage6-server-4.4.1/vantage6/server/_data/unittest_config.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/_data/unittest_fixtures.yaml` & `vantage6-server-4.4.1/vantage6/server/_data/unittest_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/_version.py` & `vantage6-server-4.4.1/vantage6/server/_version.py`

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

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/algo_store_communication.py` & `vantage6-server-4.4.1/vantage6/server/algo_store_communication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import logging
 import requests
 from flask import Response
 from http import HTTPStatus
 
+from vantage6.backend.common.globals import HOST_URI_ENV
 from vantage6.server import db
 
 
 module_name = __name__.split(".")[-1]
 log = logging.getLogger(module_name)
 
 
@@ -145,15 +146,15 @@
         if not is_localhost_algo_store:
             log.warning("Request to algorithm store failed")
             log.exception(exc)
         response = None
 
     if not response and is_localhost_algo_store:
         # try again with the docker host ip
-        host_uri = os.environ.get("HOST_URI_ENV_VAR", None)
+        host_uri = os.environ.get(HOST_URI_ENV, None)
         if not host_uri:
             msg = (
                 "You are trying to connect to a localhost algorithm store, but this "
                 "refers to the container itself. Please set the configuration option "
                 "'host_uri' in the 'dev' section  of the config file to the host's IP "
                 "address."
             )
```

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/cli/server.py` & `vantage6-server-4.4.1/vantage6/server/cli/server.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/context.py` & `vantage6-server-4.4.1/vantage6/server/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/controller/fixture.py` & `vantage6-server-4.4.1/vantage6/server/controller/fixture.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/db.py` & `vantage6-server-4.4.1/vantage6/server/db.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/default_roles.py` & `vantage6-server-4.4.1/vantage6/server/default_roles.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/globals.py` & `vantage6-server-4.4.1/vantage6/server/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/mail_service.py` & `vantage6-server-4.4.1/vantage6/server/mail_service.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/__init__.py` & `vantage6-server-4.4.1/vantage6/server/model/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/algorithm_port.py` & `vantage6-server-4.4.1/vantage6/server/model/algorithm_port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/algorithm_store.py` & `vantage6-server-4.4.1/vantage6/server/model/algorithm_store.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/authenticatable.py` & `vantage6-server-4.4.1/vantage6/server/model/authenticatable.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/base.py` & `vantage6-server-4.4.1/vantage6/server/model/base.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/collaboration.py` & `vantage6-server-4.4.1/vantage6/server/model/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/common/utils.py` & `vantage6-server-4.4.1/vantage6/server/model/common/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/member.py` & `vantage6-server-4.4.1/vantage6/server/model/member.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/node.py` & `vantage6-server-4.4.1/vantage6/server/model/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/node_config.py` & `vantage6-server-4.4.1/vantage6/server/model/node_config.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/organization.py` & `vantage6-server-4.4.1/vantage6/server/model/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/permission.py` & `vantage6-server-4.4.1/vantage6/server/model/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/role.py` & `vantage6-server-4.4.1/vantage6/server/model/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/rule.py` & `vantage6-server-4.4.1/vantage6/server/model/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/run.py` & `vantage6-server-4.4.1/vantage6/server/model/run.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/study.py` & `vantage6-server-4.4.1/vantage6/server/model/study.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/task.py` & `vantage6-server-4.4.1/vantage6/server/model/task.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/task_database.py` & `vantage6-server-4.4.1/vantage6/server/model/task_database.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/model/user.py` & `vantage6-server-4.4.1/vantage6/server/model/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/permission.py` & `vantage6-server-4.4.1/vantage6/server/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/__init__.py` & `vantage6-server-4.4.1/vantage6/server/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/algorithm_store.py` & `vantage6-server-4.4.1/vantage6/server/resource/algorithm_store.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/collaboration.py` & `vantage6-server-4.4.1/vantage6/server/resource/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/common/auth_helper.py` & `vantage6-server-4.4.1/vantage6/server/resource/common/auth_helper.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/common/input_schema.py` & `vantage6-server-4.4.1/vantage6/server/resource/common/input_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/common/output_schema.py` & `vantage6-server-4.4.1/vantage6/server/resource/common/output_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/common/swagger_templates.py` & `vantage6-server-4.4.1/vantage6/server/resource/common/swagger_templates.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/event.py` & `vantage6-server-4.4.1/vantage6/server/resource/event.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/health.py` & `vantage6-server-4.4.1/vantage6/server/resource/health.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/node.py` & `vantage6-server-4.4.1/vantage6/server/resource/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/organization.py` & `vantage6-server-4.4.1/vantage6/server/resource/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/port.py` & `vantage6-server-4.4.1/vantage6/server/resource/port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/recover.py` & `vantage6-server-4.4.1/vantage6/server/resource/recover.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/role.py` & `vantage6-server-4.4.1/vantage6/server/resource/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/rule.py` & `vantage6-server-4.4.1/vantage6/server/resource/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/run.py` & `vantage6-server-4.4.1/vantage6/server/resource/run.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/stats.py` & `vantage6-server-4.4.1/vantage6/server/resource/stats.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/study.py` & `vantage6-server-4.4.1/vantage6/server/resource/study.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/task.py` & `vantage6-server-4.4.1/vantage6/server/resource/task.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/token.py` & `vantage6-server-4.4.1/vantage6/server/resource/token.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/ui/column.py` & `vantage6-server-4.4.1/vantage6/server/resource/ui/column.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/user.py` & `vantage6-server-4.4.1/vantage6/server/resource/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/version.py` & `vantage6-server-4.4.1/vantage6/server/resource/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/vpn.py` & `vantage6-server-4.4.1/vantage6/server/resource/vpn.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/resource/websocket_test.py` & `vantage6-server-4.4.1/vantage6/server/resource/websocket_test.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/utils.py` & `vantage6-server-4.4.1/vantage6/server/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6/server/websockets.py` & `vantage6-server-4.4.1/vantage6/server/websockets.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.0rc3/vantage6_server.egg-info/PKG-INFO` & `vantage6-server-4.4.1/vantage6_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 4.4.0rc3
+Version: 4.4.1
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 4.4.0rc3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 4.4.1 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-server-4.4.0rc3/vantage6_server.egg-info/SOURCES.txt` & `vantage6-server-4.4.1/vantage6_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

