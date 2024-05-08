# Comparing `tmp/uac-cli-0.2.2.tar.gz` & `tmp/uac-cli-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uac-cli-0.2.2.tar", last modified: Wed May  8 02:51:50 2024, max compression
+gzip compressed data, was "uac-cli-0.2.3.tar", last modified: Wed May  8 04:09:40 2024, max compression
```

## Comparing `uac-cli-0.2.2.tar` & `uac-cli-0.2.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 02:51:50.854400 uac-cli-0.2.2/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9672 2024-05-08 02:51:50.854106 uac-cli-0.2.2/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9041 2024-05-07 21:43:44.000000 uac-cli-0.2.2/README.md
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      405 2024-05-07 21:45:43.000000 uac-cli-0.2.2/pyproject.toml
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-08 02:51:50.854447 uac-cli-0.2.2/setup.cfg
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1185 2024-05-08 02:51:37.000000 uac-cli-0.2.2/setup.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 02:51:50.839837 uac-cli-0.2.2/uac_cli/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      145 2024-05-08 02:51:45.000000 uac-cli-0.2.2/uac_cli/__init__.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 02:51:50.852860 uac-cli-0.2.2/uac_cli/commands/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:55:51.000000 uac-cli-0.2.2/uac_cli/commands/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5545 2024-05-07 20:59:24.000000 uac-cli-0.2.2/uac_cli/commands/agent.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6346 2024-05-07 21:00:04.000000 uac-cli-0.2.2/uac_cli/commands/agent_cluster.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      918 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/audit.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9331 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/bundle.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2994 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/business_service.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5357 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/calendar.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1188 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/cluster_node.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2183 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/config.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    11836 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/connection.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3875 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/credential.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3434 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/custom_day.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2929 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/email_template.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1491 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/ldap.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      756 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/metric.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2954 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/oauth_client.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3023 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/oms_server.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1587 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/property.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      958 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/report.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2527 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/script.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1157 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/server_operation.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2993 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/simulation.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      726 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/system.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9664 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/task.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18242 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/task_instance.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6392 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/trigger.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1499 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/universal_event.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3084 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/universal_event_template.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6360 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/universal_template.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4716 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/user.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2678 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/user_group.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3495 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/variable.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3691 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/virtual_resource.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4208 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/webhook.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5184 2024-05-07 15:20:53.000000 uac-cli-0.2.2/uac_cli/commands/workflow.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4504 2024-05-07 19:37:27.000000 uac-cli-0.2.2/uac_cli/main.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 02:51:50.853842 uac-cli-0.2.2/uac_cli/utils/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:56:14.000000 uac-cli-0.2.2/uac_cli/utils/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2922 2024-05-05 22:04:40.000000 uac-cli-0.2.2/uac_cli/utils/config.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      460 2024-05-05 18:06:43.000000 uac-cli-0.2.2/uac_cli/utils/options.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2079 2024-05-06 20:06:47.000000 uac-cli-0.2.2/uac_cli/utils/process.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 02:51:50.841919 uac-cli-0.2.2/uac_cli.egg-info/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9672 2024-05-08 02:51:50.000000 uac-cli-0.2.2/uac_cli.egg-info/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1433 2024-05-08 02:51:50.000000 uac-cli-0.2.2/uac_cli.egg-info/SOURCES.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-08 02:51:50.000000 uac-cli-0.2.2/uac_cli.egg-info/dependency_links.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       41 2024-05-08 02:51:50.000000 uac-cli-0.2.2/uac_cli.egg-info/entry_points.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       66 2024-05-08 02:51:50.000000 uac-cli-0.2.2/uac_cli.egg-info/requires.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-08 02:51:50.000000 uac-cli-0.2.2/uac_cli.egg-info/top_level.txt
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 04:09:40.910192 uac-cli-0.2.3/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9672 2024-05-08 04:09:40.909914 uac-cli-0.2.3/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9041 2024-05-07 21:43:44.000000 uac-cli-0.2.3/README.md
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      405 2024-05-07 21:45:43.000000 uac-cli-0.2.3/pyproject.toml
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-08 04:09:40.910247 uac-cli-0.2.3/setup.cfg
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1185 2024-05-08 02:51:37.000000 uac-cli-0.2.3/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 04:09:40.896879 uac-cli-0.2.3/uac_cli/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      145 2024-05-08 04:09:35.000000 uac-cli-0.2.3/uac_cli/__init__.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 04:09:40.908329 uac-cli-0.2.3/uac_cli/commands/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:55:51.000000 uac-cli-0.2.3/uac_cli/commands/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5545 2024-05-07 20:59:24.000000 uac-cli-0.2.3/uac_cli/commands/agent.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6346 2024-05-07 21:00:04.000000 uac-cli-0.2.3/uac_cli/commands/agent_cluster.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      918 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/audit.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9331 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/bundle.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2994 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/business_service.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5357 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/calendar.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1188 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/cluster_node.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2183 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/config.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    11836 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/connection.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3875 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/credential.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3434 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/custom_day.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2929 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/email_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1491 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/ldap.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      756 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/metric.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2954 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/oauth_client.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3023 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/oms_server.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1616 2024-05-08 03:23:56.000000 uac-cli-0.2.3/uac_cli/commands/property.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      958 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/report.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2527 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/script.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3134 2024-05-08 03:49:16.000000 uac-cli-0.2.3/uac_cli/commands/server_operation.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2993 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/simulation.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      726 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/system.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9664 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/task.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18242 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/task_instance.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6392 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/trigger.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1499 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/universal_event.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3084 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/universal_event_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6360 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/universal_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4716 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/user.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2678 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/user_group.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3495 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/variable.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3691 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/virtual_resource.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4208 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/webhook.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5184 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/workflow.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4504 2024-05-07 19:37:27.000000 uac-cli-0.2.3/uac_cli/main.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 04:09:40.909478 uac-cli-0.2.3/uac_cli/utils/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:56:14.000000 uac-cli-0.2.3/uac_cli/utils/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2922 2024-05-05 22:04:40.000000 uac-cli-0.2.3/uac_cli/utils/config.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      479 2024-05-08 04:03:24.000000 uac-cli-0.2.3/uac_cli/utils/options.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2092 2024-05-08 04:06:30.000000 uac-cli-0.2.3/uac_cli/utils/process.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 04:09:40.898423 uac-cli-0.2.3/uac_cli.egg-info/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9672 2024-05-08 04:09:40.000000 uac-cli-0.2.3/uac_cli.egg-info/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1433 2024-05-08 04:09:40.000000 uac-cli-0.2.3/uac_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-08 04:09:40.000000 uac-cli-0.2.3/uac_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       41 2024-05-08 04:09:40.000000 uac-cli-0.2.3/uac_cli.egg-info/entry_points.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       66 2024-05-08 04:09:40.000000 uac-cli-0.2.3/uac_cli.egg-info/requires.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-08 04:09:40.000000 uac-cli-0.2.3/uac_cli.egg-info/top_level.txt
```

### Comparing `uac-cli-0.2.2/PKG-INFO` & `uac-cli-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uac-cli
-Version: 0.2.2
+Version: 0.2.3
 Summary: A CLI tool for executing commands against the Stonebranch UAC API
 Author: Stonebranch
 Author-email: "Huseyin G." <huseyim@gmail.com>
 License: CC BY-NC 4.0
 Project-URL: Homepage, https://github.com/gomleksiz/uac-cli
 Project-URL: Issues, https://github.com/gomleksiz/uac-cli/issues
 Project-URL: Documentation, https://uac-cli.readthedocs.io/en/latest/index.html
```

### Comparing `uac-cli-0.2.2/README.md` & `uac-cli-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/setup.py` & `uac-cli-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/agent.py` & `uac-cli-0.2.3/uac_cli/commands/agent.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/agent_cluster.py` & `uac-cli-0.2.3/uac_cli/commands/agent_cluster.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/audit.py` & `uac-cli-0.2.3/uac_cli/commands/audit.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/bundle.py` & `uac-cli-0.2.3/uac_cli/commands/bundle.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/business_service.py` & `uac-cli-0.2.3/uac_cli/commands/business_service.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/calendar.py` & `uac-cli-0.2.3/uac_cli/commands/calendar.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/cluster_node.py` & `uac-cli-0.2.3/uac_cli/commands/cluster_node.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/config.py` & `uac-cli-0.2.3/uac_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/connection.py` & `uac-cli-0.2.3/uac_cli/commands/connection.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/credential.py` & `uac-cli-0.2.3/uac_cli/commands/credential.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/custom_day.py` & `uac-cli-0.2.3/uac_cli/commands/custom_day.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/email_template.py` & `uac-cli-0.2.3/uac_cli/commands/email_template.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/ldap.py` & `uac-cli-0.2.3/uac_cli/commands/ldap.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/metric.py` & `uac-cli-0.2.3/uac_cli/commands/metric.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/oauth_client.py` & `uac-cli-0.2.3/uac_cli/commands/oauth_client.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/oms_server.py` & `uac-cli-0.2.3/uac_cli/commands/oms_server.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/property.py` & `uac-cli-0.2.3/uac_cli/commands/property.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def get_property(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.properties.get_property(**vars_dict)
     process_output(output, select, response)
 
 
 @property.command('update', short_help='Modifies the specified property.')
-@click.argument('args', nargs=-1, metavar='')
+@click.argument('args', nargs=-1, metavar='propertyname=name value=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 def update_property(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.properties.update_property(**vars_dict)
```

### Comparing `uac-cli-0.2.2/uac_cli/commands/report.py` & `uac-cli-0.2.3/uac_cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/script.py` & `uac-cli-0.2.3/uac_cli/commands/script.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/server_operation.py` & `uac-cli-0.2.3/uac_cli/commands/universal_event.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 import click
 from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
-@click.group(help='Commands for server operations, such as log rolling and temporary property changes.')
-def server_operation():
+@click.group(help='Commands related to universal events, including publishing and managing universal events.')
+def universal_event():
     pass
 
-@server_operation.command('roll_log', short_help='None')
-@click.argument('args', nargs=-1, metavar='')
+@universal_event.command('publish', short_help='None')
+@click.argument('args', nargs=-1, metavar='name=value business_services=value ttl=value attributes=value')
+@click.pass_obj
+@output_option
+@select_option
+def publish(uac: UniversalController, args, output=None, select=None):
+    vars_dict = process_input(args)
+    response = uac.universal_events.publish(**vars_dict)
+    process_output(output, select, response)
+
+
+@universal_event.command('pushg', short_help='None')
+@click.argument('args', nargs=-1, metavar='payload=value')
 @click.pass_obj
 @output_option
 @select_option
-def roll_log(uac: UniversalController, args, output=None, select=None):
+def pushg(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.serveroperations.roll_log(**vars_dict)
+    response = uac.universal_events.pushg(**vars_dict)
     process_output(output, select, response)
 
 
-@server_operation.command('temporary_property_change', short_help='None')
-@click.argument('args', nargs=-1, metavar='name=value value=value')
+@universal_event.command('push', short_help='None')
+@click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def temporary_property_change(uac: UniversalController, args, output=None, select=None):
+def push(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.serveroperations.temporary_property_change(**vars_dict)
+    response = uac.universal_events.push(**vars_dict)
     process_output(output, select, response)
+
```

### Comparing `uac-cli-0.2.2/uac_cli/commands/simulation.py` & `uac-cli-0.2.3/uac_cli/commands/simulation.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/system.py` & `uac-cli-0.2.3/uac_cli/commands/system.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/task.py` & `uac-cli-0.2.3/uac_cli/commands/task.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/task_instance.py` & `uac-cli-0.2.3/uac_cli/commands/task_instance.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/trigger.py` & `uac-cli-0.2.3/uac_cli/commands/trigger.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/universal_event.py` & `uac-cli-0.2.3/uac_cli/commands/universal_event_template.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,66 @@
 import click
 from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
-@click.group(help='Commands related to universal events, including publishing and managing universal events.')
-def universal_event():
+
+@click.group(help='Commands for managing universal event templates, including creating, updating, and deleting templates.')
+def universal_event_template():
     pass
 
-@universal_event.command('publish', short_help='None')
-@click.argument('args', nargs=-1, metavar='name=value business_services=value ttl=value attributes=value')
+@universal_event_template.command('get', short_help='None')
+@click.argument('args', nargs=-1, metavar='templateid=value templatename=value')
 @click.pass_obj
 @output_option
 @select_option
-def publish(uac: UniversalController, args, output=None, select=None):
+def get_universal_event_template(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.universal_events.publish(**vars_dict)
+    response = uac.universal_event_templates.get_universal_event_template(**vars_dict)
     process_output(output, select, response)
 
 
-@universal_event.command('pushg', short_help='None')
-@click.argument('args', nargs=-1, metavar='payload=value')
+@universal_event_template.command('update', short_help='None')
+@click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value label=value description=value ttl=value attributes_policy=value attributes=value metric_type=value metric_name=value metric_value_attribute=value metric_unit=value metric_label_attributes=value metric_optional_labels=value retain_sys_ids=value attributes_from_string=value')
 @click.pass_obj
 @output_option
+@input_option
 @select_option
-def pushg(uac: UniversalController, args, output=None, select=None):
-    vars_dict = process_input(args)
-    response = uac.universal_events.pushg(**vars_dict)
+def update_universal_event_template(uac: UniversalController, args, output=None, input=None, select=None):
+    vars_dict = process_input(args, input)
+    response = uac.universal_event_templates.update_universal_event_template(**vars_dict)
+    process_output(output, select, response)
+
+
+@universal_event_template.command('create', short_help='None')
+@click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
+@click.pass_obj
+@output_option
+@input_option
+@select_option
+@ignore_ids
+def create_universal_event_template(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
+    vars_dict = process_input(args, input, ignore_ids)
+    response = uac.universal_event_templates.create_universal_event_template(**vars_dict)
     process_output(output, select, response)
 
 
-@universal_event.command('push', short_help='None')
-@click.argument('args', nargs=-1, metavar='')
+@universal_event_template.command('delete', short_help='None')
+@click.argument('args', nargs=-1, metavar='templateid=value templatename=value')
 @click.pass_obj
 @output_option
 @select_option
-def push(uac: UniversalController, args, output=None, select=None):
+def delete_universal_event_template(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.universal_events.push(**vars_dict)
+    response = uac.universal_event_templates.delete_universal_event_template(**vars_dict)
     process_output(output, select, response)
 
+
+@universal_event_template.command('list', short_help='None')
+@click.argument('args', nargs=-1, metavar='templatename=value')
+@click.pass_obj
+@output_option
+@select_option
+def list_universal_event_templates(uac: UniversalController, args, output=None, select=None):
+    vars_dict = process_input(args)
+    response = uac.universal_event_templates.list_universal_event_templates(**vars_dict)
+    process_output(output, select, response)
```

### Comparing `uac-cli-0.2.2/uac_cli/commands/universal_event_template.py` & `uac-cli-0.2.3/uac_cli/commands/user_group.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 import click
 from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 
-@click.group(help='Commands for managing universal event templates, including creating, updating, and deleting templates.')
-def universal_event_template():
+@click.group(help='User group management commands, including listing, creating, updating, and deleting user groups.')
+def user_group():
     pass
 
-@universal_event_template.command('get', short_help='None')
-@click.argument('args', nargs=-1, metavar='templateid=value templatename=value')
+
+
+@user_group.command('get', short_help='None')
+@click.argument('args', nargs=-1, metavar='groupid=value groupname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_universal_event_template(uac: UniversalController, args, output=None, select=None):
+def get_user_group(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.universal_event_templates.get_universal_event_template(**vars_dict)
+    response = uac.user_groups.get_user_group(**vars_dict)
     process_output(output, select, response)
 
 
-@universal_event_template.command('update', short_help='None')
-@click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value label=value description=value ttl=value attributes_policy=value attributes=value metric_type=value metric_name=value metric_value_attribute=value metric_unit=value metric_label_attributes=value metric_optional_labels=value retain_sys_ids=value attributes_from_string=value')
+@user_group.command('update', short_help='None')
+@click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value retain_sys_ids=value name=value email=value manager=value description=value parent=value ctrl_navigation_visibility=value navigation_visibility=value permissions=value group_roles=value group_members=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_universal_event_template(uac: UniversalController, args, output=None, input=None, select=None):
+def update_user_group(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
-    response = uac.universal_event_templates.update_universal_event_template(**vars_dict)
+    response = uac.user_groups.update_user_group(**vars_dict)
     process_output(output, select, response)
 
 
-@universal_event_template.command('create', short_help='None')
+@user_group.command('create', short_help='None')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_universal_event_template(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
+def create_user_group(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
-    response = uac.universal_event_templates.create_universal_event_template(**vars_dict)
+    response = uac.user_groups.create_user_group(**vars_dict)
     process_output(output, select, response)
 
 
-@universal_event_template.command('delete', short_help='None')
-@click.argument('args', nargs=-1, metavar='templateid=value templatename=value')
+@user_group.command('delete', short_help='None')
+@click.argument('args', nargs=-1, metavar='groupid=value groupname=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_universal_event_template(uac: UniversalController, args, output=None, select=None):
+def delete_user_group(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.universal_event_templates.delete_universal_event_template(**vars_dict)
+    response = uac.user_groups.delete_user_group(**vars_dict)
     process_output(output, select, response)
 
 
-@universal_event_template.command('list', short_help='None')
-@click.argument('args', nargs=-1, metavar='templatename=value')
+@user_group.command('list', short_help='None')
+@click.argument('args', nargs=-1, metavar='')
 @click.pass_obj
 @output_option
 @select_option
-def list_universal_event_templates(uac: UniversalController, args, output=None, select=None):
+def list_user_groups(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.universal_event_templates.list_universal_event_templates(**vars_dict)
+    response = uac.user_groups.list_user_groups(**vars_dict)
     process_output(output, select, response)
```

### Comparing `uac-cli-0.2.2/uac_cli/commands/universal_template.py` & `uac-cli-0.2.3/uac_cli/commands/universal_template.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/user.py` & `uac-cli-0.2.3/uac_cli/commands/user.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/user_group.py` & `uac-cli-0.2.3/uac_cli/commands/variable.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,91 @@
 import click
 from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
 
-@click.group(help='User group management commands, including listing, creating, updating, and deleting user groups.')
-def user_group():
+@click.group(help='Commands for managing variables, including setting, updating, and listing variables.')
+def variable():
     pass
 
 
-
-@user_group.command('get', short_help='None')
-@click.argument('args', nargs=-1, metavar='groupid=value groupname=value')
+@variable.command('get', short_help='None')
+@click.argument('args', nargs=-1, metavar='variableid=value variablename=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_user_group(uac: UniversalController, args, output=None, select=None):
+def get_variable(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.user_groups.get_user_group(**vars_dict)
+    response = uac.variables.get_variable(**vars_dict)
     process_output(output, select, response)
 
 
-@user_group.command('update', short_help='None')
-@click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value retain_sys_ids=value name=value email=value manager=value description=value parent=value ctrl_navigation_visibility=value navigation_visibility=value permissions=value group_roles=value group_members=value')
+@variable.command('update', short_help='None')
+@click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value value=value description=value opswise_groups=value retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_user_group(uac: UniversalController, args, output=None, input=None, select=None):
+def update_variable(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
-    response = uac.user_groups.update_user_group(**vars_dict)
+    response = uac.variables.update_variable(**vars_dict)
     process_output(output, select, response)
 
 
-@user_group.command('create', short_help='None')
+@variable.command('create', short_help='None')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_user_group(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
+def create_variable(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
-    response = uac.user_groups.create_user_group(**vars_dict)
+    response = uac.variables.create_variable(**vars_dict)
     process_output(output, select, response)
 
 
-@user_group.command('delete', short_help='None')
-@click.argument('args', nargs=-1, metavar='groupid=value groupname=value')
+@variable.command('delete', short_help='None')
+@click.argument('args', nargs=-1, metavar='variableid=value variablename=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_user_group(uac: UniversalController, args, output=None, select=None):
+def delete_variable(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.user_groups.delete_user_group(**vars_dict)
+    response = uac.variables.delete_variable(**vars_dict)
     process_output(output, select, response)
 
 
-@user_group.command('list', short_help='None')
-@click.argument('args', nargs=-1, metavar='')
+@variable.command('list', short_help='None')
+@click.argument('args', nargs=-1, metavar='variable_name=value scope=value task_name=value trigger_name=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_user_groups(uac: UniversalController, args, output=None, select=None):
+def list_variables(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.user_groups.list_user_groups(**vars_dict)
+    response = uac.variables.list_variables(**vars_dict)
     process_output(output, select, response)
+
+
+@variable.command('list_advanced', short_help='None')
+@click.argument('args', nargs=-1, metavar='scope=value variablename=value taskname=value triggername=value business_services=value')
+@click.pass_obj
+@output_option
+@select_option
+def list_variables_advanced(uac: UniversalController, args, output=None, select=None):
+    vars_dict = process_input(args)
+    response = uac.variables.list_variables_advanced(**vars_dict)
+    process_output(output, select, response)
+
+
+@variable.command('set', short_help='None')
+@click.argument('args', nargs=-1, metavar='scope=value create=value trigger=value task=value variable=value')
+@click.pass_obj
+@output_option
+@input_option
+@select_option
+def variable_set(uac: UniversalController, args, output=None, input=None, select=None):
+    vars_dict = process_input(args, input)
+    response = uac.variables.variable_set(**vars_dict)
+    process_output(output, select, response)
+
```

### Comparing `uac-cli-0.2.2/uac_cli/commands/variable.py` & `uac-cli-0.2.3/uac_cli/commands/webhook.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,91 +1,99 @@
 import click
 from uac_api import UniversalController
 from uac_cli.utils.process import process_output, process_input, create_payload
 from uac_cli.utils.options import output_option, input_option, select_option, ignore_ids
 
-
-@click.group(help='Commands for managing variables, including setting, updating, and listing variables.')
-def variable():
+@click.group(help='Webhook management commands, including creating, updating, enabling, and disabling webhooks.')
+def webhook():
     pass
 
 
-@variable.command('get', short_help='None')
-@click.argument('args', nargs=-1, metavar='variableid=value variablename=value')
+@webhook.command('unassign_execution_user_1', short_help='None')
+@click.argument('args', nargs=-1, metavar='webhookid=value webhookname=value')
+@click.pass_obj
+@output_option
+@select_option
+def unassign_execution_user_1(uac: UniversalController, args, output=None, select=None):
+    vars_dict = process_input(args)
+    response = uac.webhooks.unassign_execution_user_1(**vars_dict)
+    process_output(output, select, response)
+
+
+@webhook.command('get', short_help='None')
+@click.argument('args', nargs=-1, metavar='webhookid=value webhookname=value')
 @click.pass_obj
 @output_option
 @select_option
-def get_variable(uac: UniversalController, args, output=None, select=None):
+def get_webhook(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.variables.get_variable(**vars_dict)
+    response = uac.webhooks.get_webhook(**vars_dict)
     process_output(output, select, response)
 
 
-@variable.command('update', short_help='None')
-@click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value value=value description=value opswise_groups=value retain_sys_ids=value')
+@webhook.command('update', short_help='None')
+@click.argument('args', nargs=-1, metavar='version=value sys_id=value exclude_related=value export_release_level=value export_table=value name=value description=value retain_sys_ids=value opswise_groups=value event=value action=value task=value url=value filter=value enabled_by=value enabled_time=value disabled_by=value disabled_time=value execution_user=value status=value status_description=value url_parameters=value http_headers=value http_auth=value credentials=value url_parameters_from_string=value http_headers_from_string=value event_business_service_criteria=value event_business_services=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
-def update_variable(uac: UniversalController, args, output=None, input=None, select=None):
+def update_webhook(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
-    response = uac.variables.update_variable(**vars_dict)
+    response = uac.webhooks.update_webhook(**vars_dict)
     process_output(output, select, response)
 
 
-@variable.command('create', short_help='None')
+@webhook.command('create', short_help='None')
 @click.argument('args', nargs=-1, metavar='retain_sys_ids=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 @ignore_ids
-def create_variable(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
+def create_webhook(uac: UniversalController, args, output=None, input=None, select=None, ignore_ids=False):
     vars_dict = process_input(args, input, ignore_ids)
-    response = uac.variables.create_variable(**vars_dict)
+    response = uac.webhooks.create_webhook(**vars_dict)
     process_output(output, select, response)
 
 
-@variable.command('delete', short_help='None')
-@click.argument('args', nargs=-1, metavar='variableid=value variablename=value')
+@webhook.command('delete', short_help='None')
+@click.argument('args', nargs=-1, metavar='webhookid=value webhookname=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_variable(uac: UniversalController, args, output=None, select=None):
+def delete_webhook(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.variables.delete_variable(**vars_dict)
+    response = uac.webhooks.delete_webhook(**vars_dict)
     process_output(output, select, response)
 
 
-@variable.command('list', short_help='None')
-@click.argument('args', nargs=-1, metavar='variable_name=value scope=value task_name=value trigger_name=value')
+@webhook.command('disable', short_help='None')
+@click.argument('args', nargs=-1, metavar='webhookid=value webhookname=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_variables(uac: UniversalController, args, output=None, select=None):
+def disable_webhook(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.variables.list_variables(**vars_dict)
+    response = uac.webhooks.disable_webhook(**vars_dict)
     process_output(output, select, response)
 
 
-@variable.command('list_advanced', short_help='None')
-@click.argument('args', nargs=-1, metavar='scope=value variablename=value taskname=value triggername=value business_services=value')
+@webhook.command('enable', short_help='None')
+@click.argument('args', nargs=-1, metavar='webhookid=value webhookname=value')
 @click.pass_obj
 @output_option
 @select_option
-def list_variables_advanced(uac: UniversalController, args, output=None, select=None):
+def enable_webhook(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
-    response = uac.variables.list_variables_advanced(**vars_dict)
+    response = uac.webhooks.enable_webhook(**vars_dict)
     process_output(output, select, response)
 
 
-@variable.command('set', short_help='None')
-@click.argument('args', nargs=-1, metavar='scope=value create=value trigger=value task=value variable=value')
+@webhook.command('list', short_help='None')
+@click.argument('args', nargs=-1, metavar='webhookname=value action=value business_services=value description=value event=value task=value taskname=value url=value')
 @click.pass_obj
 @output_option
-@input_option
 @select_option
-def variable_set(uac: UniversalController, args, output=None, input=None, select=None):
-    vars_dict = process_input(args, input)
-    response = uac.variables.variable_set(**vars_dict)
+def list_webhooks(uac: UniversalController, args, output=None, select=None):
+    vars_dict = process_input(args)
+    response = uac.webhooks.list_webhooks(**vars_dict)
     process_output(output, select, response)
-
```

### Comparing `uac-cli-0.2.2/uac_cli/commands/virtual_resource.py` & `uac-cli-0.2.3/uac_cli/commands/virtual_resource.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/commands/workflow.py` & `uac-cli-0.2.3/uac_cli/commands/workflow.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/main.py` & `uac-cli-0.2.3/uac_cli/main.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/utils/config.py` & `uac-cli-0.2.3/uac_cli/utils/config.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.2/uac_cli/utils/process.py` & `uac-cli-0.2.3/uac_cli/utils/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,21 +27,22 @@
     
     if select:
         jsonpath_expr = parse(select)
         result = [str(match.value) for match in jsonpath_expr.find(response)]
         click.echo("\n".join(result))
     else:
         if output is None:
-            if not text:
-                click.echo(json.dumps(response, indent=4))
+            if binary:
+                click.echo(response)
             else:
-                if binary:
-                    click.echo(response)
-                else:
+                if text:
                     click.echo(response.get("response", "").replace("\\n", "\n"))
+                else:
+                    click.echo(json.dumps(response, indent=4))
+                
 
 def process_input(args, input=None, ignore_ids=None):
     vars_dict = dict(var.split('=', 1) for var in args)
     if ignore_ids is not None:
         vars_dict["retain_sys_ids"] = not ignore_ids
     if input:
         payload = input.read()
```

### Comparing `uac-cli-0.2.2/uac_cli.egg-info/PKG-INFO` & `uac-cli-0.2.3/uac_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uac-cli
-Version: 0.2.2
+Version: 0.2.3
 Summary: A CLI tool for executing commands against the Stonebranch UAC API
 Author: Stonebranch
 Author-email: "Huseyin G." <huseyim@gmail.com>
 License: CC BY-NC 4.0
 Project-URL: Homepage, https://github.com/gomleksiz/uac-cli
 Project-URL: Issues, https://github.com/gomleksiz/uac-cli/issues
 Project-URL: Documentation, https://uac-cli.readthedocs.io/en/latest/index.html
```

### Comparing `uac-cli-0.2.2/uac_cli.egg-info/SOURCES.txt` & `uac-cli-0.2.3/uac_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

