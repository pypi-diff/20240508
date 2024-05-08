# Comparing `tmp/uac-cli-0.2.3.tar.gz` & `tmp/uac-cli-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uac-cli-0.2.3.tar", last modified: Wed May  8 04:09:40 2024, max compression
+gzip compressed data, was "uac-cli-0.2.4.tar", last modified: Wed May  8 04:53:38 2024, max compression
```

## Comparing `uac-cli-0.2.3.tar` & `uac-cli-0.2.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 04:09:40.910192 uac-cli-0.2.3/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9672 2024-05-08 04:09:40.909914 uac-cli-0.2.3/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9041 2024-05-07 21:43:44.000000 uac-cli-0.2.3/README.md
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      405 2024-05-07 21:45:43.000000 uac-cli-0.2.3/pyproject.toml
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-08 04:09:40.910247 uac-cli-0.2.3/setup.cfg
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1185 2024-05-08 02:51:37.000000 uac-cli-0.2.3/setup.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 04:09:40.896879 uac-cli-0.2.3/uac_cli/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      145 2024-05-08 04:09:35.000000 uac-cli-0.2.3/uac_cli/__init__.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 04:09:40.908329 uac-cli-0.2.3/uac_cli/commands/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:55:51.000000 uac-cli-0.2.3/uac_cli/commands/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5545 2024-05-07 20:59:24.000000 uac-cli-0.2.3/uac_cli/commands/agent.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6346 2024-05-07 21:00:04.000000 uac-cli-0.2.3/uac_cli/commands/agent_cluster.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      918 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/audit.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9331 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/bundle.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2994 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/business_service.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5357 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/calendar.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1188 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/cluster_node.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2183 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/config.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    11836 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/connection.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3875 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/credential.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3434 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/custom_day.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2929 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/email_template.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1491 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/ldap.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      756 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/metric.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2954 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/oauth_client.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3023 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/oms_server.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1616 2024-05-08 03:23:56.000000 uac-cli-0.2.3/uac_cli/commands/property.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      958 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/report.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2527 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/script.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3134 2024-05-08 03:49:16.000000 uac-cli-0.2.3/uac_cli/commands/server_operation.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2993 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/simulation.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      726 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/system.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9664 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/task.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18242 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/task_instance.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6392 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/trigger.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1499 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/universal_event.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3084 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/universal_event_template.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6360 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/universal_template.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4716 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/user.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2678 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/user_group.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3495 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/variable.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3691 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/virtual_resource.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4208 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/webhook.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5184 2024-05-07 15:20:53.000000 uac-cli-0.2.3/uac_cli/commands/workflow.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4504 2024-05-07 19:37:27.000000 uac-cli-0.2.3/uac_cli/main.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 04:09:40.909478 uac-cli-0.2.3/uac_cli/utils/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:56:14.000000 uac-cli-0.2.3/uac_cli/utils/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2922 2024-05-05 22:04:40.000000 uac-cli-0.2.3/uac_cli/utils/config.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      479 2024-05-08 04:03:24.000000 uac-cli-0.2.3/uac_cli/utils/options.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2092 2024-05-08 04:06:30.000000 uac-cli-0.2.3/uac_cli/utils/process.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 04:09:40.898423 uac-cli-0.2.3/uac_cli.egg-info/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9672 2024-05-08 04:09:40.000000 uac-cli-0.2.3/uac_cli.egg-info/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1433 2024-05-08 04:09:40.000000 uac-cli-0.2.3/uac_cli.egg-info/SOURCES.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-08 04:09:40.000000 uac-cli-0.2.3/uac_cli.egg-info/dependency_links.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       41 2024-05-08 04:09:40.000000 uac-cli-0.2.3/uac_cli.egg-info/entry_points.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       66 2024-05-08 04:09:40.000000 uac-cli-0.2.3/uac_cli.egg-info/requires.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-08 04:09:40.000000 uac-cli-0.2.3/uac_cli.egg-info/top_level.txt
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 04:53:38.811894 uac-cli-0.2.4/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9672 2024-05-08 04:53:38.811570 uac-cli-0.2.4/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9041 2024-05-07 21:43:44.000000 uac-cli-0.2.4/README.md
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      405 2024-05-07 21:45:43.000000 uac-cli-0.2.4/pyproject.toml
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-08 04:53:38.811940 uac-cli-0.2.4/setup.cfg
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1185 2024-05-08 02:51:37.000000 uac-cli-0.2.4/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 04:53:38.789819 uac-cli-0.2.4/uac_cli/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      145 2024-05-08 04:29:08.000000 uac-cli-0.2.4/uac_cli/__init__.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 04:53:38.809147 uac-cli-0.2.4/uac_cli/commands/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:55:51.000000 uac-cli-0.2.4/uac_cli/commands/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5545 2024-05-07 20:59:24.000000 uac-cli-0.2.4/uac_cli/commands/agent.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6346 2024-05-07 21:00:04.000000 uac-cli-0.2.4/uac_cli/commands/agent_cluster.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      918 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/audit.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9331 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/bundle.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2994 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/business_service.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5357 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/calendar.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1188 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/cluster_node.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2183 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/config.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    11836 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/connection.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3875 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/credential.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3434 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/custom_day.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2929 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/email_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1491 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/ldap.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      756 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/metric.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2954 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/oauth_client.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3023 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/oms_server.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1616 2024-05-08 03:23:56.000000 uac-cli-0.2.4/uac_cli/commands/property.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      958 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/report.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2527 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/script.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3134 2024-05-08 03:49:16.000000 uac-cli-0.2.4/uac_cli/commands/server_operation.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2993 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/simulation.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      726 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/system.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9664 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/task.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    19049 2024-05-08 04:47:43.000000 uac-cli-0.2.4/uac_cli/commands/task_instance.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6392 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/trigger.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1499 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/universal_event.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3084 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/universal_event_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6360 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/universal_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4716 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/user.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2678 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/user_group.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3495 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/variable.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3691 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/virtual_resource.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4208 2024-05-07 15:20:53.000000 uac-cli-0.2.4/uac_cli/commands/webhook.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5716 2024-05-08 04:31:39.000000 uac-cli-0.2.4/uac_cli/commands/workflow.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4504 2024-05-07 19:37:27.000000 uac-cli-0.2.4/uac_cli/main.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 04:53:38.811083 uac-cli-0.2.4/uac_cli/utils/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:56:14.000000 uac-cli-0.2.4/uac_cli/utils/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2922 2024-05-05 22:04:40.000000 uac-cli-0.2.4/uac_cli/utils/config.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      479 2024-05-08 04:03:24.000000 uac-cli-0.2.4/uac_cli/utils/options.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2092 2024-05-08 04:06:30.000000 uac-cli-0.2.4/uac_cli/utils/process.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 04:53:38.792141 uac-cli-0.2.4/uac_cli.egg-info/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9672 2024-05-08 04:53:38.000000 uac-cli-0.2.4/uac_cli.egg-info/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1433 2024-05-08 04:53:38.000000 uac-cli-0.2.4/uac_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-08 04:53:38.000000 uac-cli-0.2.4/uac_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       41 2024-05-08 04:53:38.000000 uac-cli-0.2.4/uac_cli.egg-info/entry_points.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       66 2024-05-08 04:53:38.000000 uac-cli-0.2.4/uac_cli.egg-info/requires.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-08 04:53:38.000000 uac-cli-0.2.4/uac_cli.egg-info/top_level.txt
```

### Comparing `uac-cli-0.2.3/PKG-INFO` & `uac-cli-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uac-cli
-Version: 0.2.3
+Version: 0.2.4
 Summary: A CLI tool for executing commands against the Stonebranch UAC API
 Author: Stonebranch
 Author-email: "Huseyin G." <huseyim@gmail.com>
 License: CC BY-NC 4.0
 Project-URL: Homepage, https://github.com/gomleksiz/uac-cli
 Project-URL: Issues, https://github.com/gomleksiz/uac-cli/issues
 Project-URL: Documentation, https://uac-cli.readthedocs.io/en/latest/index.html
```

### Comparing `uac-cli-0.2.3/README.md` & `uac-cli-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/setup.py` & `uac-cli-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/agent.py` & `uac-cli-0.2.4/uac_cli/commands/agent.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/agent_cluster.py` & `uac-cli-0.2.4/uac_cli/commands/agent_cluster.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/audit.py` & `uac-cli-0.2.4/uac_cli/commands/audit.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/bundle.py` & `uac-cli-0.2.4/uac_cli/commands/bundle.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/business_service.py` & `uac-cli-0.2.4/uac_cli/commands/business_service.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/calendar.py` & `uac-cli-0.2.4/uac_cli/commands/calendar.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/cluster_node.py` & `uac-cli-0.2.4/uac_cli/commands/cluster_node.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/config.py` & `uac-cli-0.2.4/uac_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/connection.py` & `uac-cli-0.2.4/uac_cli/commands/connection.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/credential.py` & `uac-cli-0.2.4/uac_cli/commands/credential.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/custom_day.py` & `uac-cli-0.2.4/uac_cli/commands/custom_day.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/email_template.py` & `uac-cli-0.2.4/uac_cli/commands/email_template.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/ldap.py` & `uac-cli-0.2.4/uac_cli/commands/ldap.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/metric.py` & `uac-cli-0.2.4/uac_cli/commands/metric.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/oauth_client.py` & `uac-cli-0.2.4/uac_cli/commands/oauth_client.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/oms_server.py` & `uac-cli-0.2.4/uac_cli/commands/oms_server.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/property.py` & `uac-cli-0.2.4/uac_cli/commands/property.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/report.py` & `uac-cli-0.2.4/uac_cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/script.py` & `uac-cli-0.2.4/uac_cli/commands/script.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/server_operation.py` & `uac-cli-0.2.4/uac_cli/commands/server_operation.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/simulation.py` & `uac-cli-0.2.4/uac_cli/commands/simulation.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/system.py` & `uac-cli-0.2.4/uac_cli/commands/system.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/task.py` & `uac-cli-0.2.4/uac_cli/commands/task.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/task_instance.py` & `uac-cli-0.2.4/uac_cli/commands/task_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -221,19 +221,37 @@
 
 
 @task_instance.command('rerun', short_help='None')
 @click.argument('args', nargs=-1, metavar='name=value id=value criteria=value workflow_instance_name=value resource_name=value recursive=value predecessor_name=value wait_type=value wait_time=value wait_duration=value wait_seconds=value wait_day_constraint=value delay_type=value delay_duration=value delay_seconds=value halt=value priority_type=value task_status=value operational_memo=value hold_reason=value')
 @click.pass_obj
 @output_option
 @select_option
-def task_instance_rerun(uac: UniversalController, args, output=None, select=None):
+@click.option('--wait', '-w', is_flag=True)
+@click.option('--timeout', '-t', type=int, default=300)
+@click.option('--interval', '-i', type=int, default=10)
+@click.option('--return_rc', '-r', is_flag=True)
+def task_instance_rerun(uac: UniversalController, args, output=None, select=None, wait=False, timeout=300, interval=10, return_rc=False):
     vars_dict = process_input(args)
     response = uac.task_instances.rerun(**vars_dict)
-    process_output(output, select, response)
+    if wait:
+        if "id" in vars_dict:
+            response = uac.task_instances.wait_for_status(id=vars_dict["id"], timeout=timeout, interval=interval)
+        else:
+            click.echo(click.style(f"Wait option only works with id", fg='red'))
+            exit(1)
 
+    process_output(output, select, response)
+    if wait and return_rc:
+        if "exitCode" in response:
+            exit(int(response["exitCode"]))
+        else:
+            if response.get("status", "UNKNOWN") in uac.task_instances.SUCCESS_STATUSES:
+                exit(0)
+            else:
+                exit(1)
 
 @task_instance.command('retrieve_output', short_help='None')
 @click.argument('args', nargs=-1, metavar='taskinstancename=value taskinstanceid=value workflowinstancename=value criteria=value outputtype=value startline=value numlines=value scantext=value operational_memo=value')
 @click.pass_obj
 @output_option
 @select_option
 def task_instance_retrieve_output(uac: UniversalController, args, output=None, select=None):
```

### Comparing `uac-cli-0.2.3/uac_cli/commands/trigger.py` & `uac-cli-0.2.4/uac_cli/commands/trigger.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/universal_event.py` & `uac-cli-0.2.4/uac_cli/commands/universal_event.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/universal_event_template.py` & `uac-cli-0.2.4/uac_cli/commands/universal_event_template.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/universal_template.py` & `uac-cli-0.2.4/uac_cli/commands/universal_template.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/user.py` & `uac-cli-0.2.4/uac_cli/commands/user.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/user_group.py` & `uac-cli-0.2.4/uac_cli/commands/user_group.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/variable.py` & `uac-cli-0.2.4/uac_cli/commands/variable.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/virtual_resource.py` & `uac-cli-0.2.4/uac_cli/commands/virtual_resource.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/webhook.py` & `uac-cli-0.2.4/uac_cli/commands/webhook.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/commands/workflow.py` & `uac-cli-0.2.4/uac_cli/commands/workflow.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,71 +6,71 @@
 
 @click.group(help='Workflow management commands, including operations for managing workflow vertices and edges, as well as running workflow forecasts.')
 def workflow():
     pass
 
 
 
-@workflow.command('get_edges', short_help='None')
+@workflow.command('get_edges', short_help='Gets an edge')
 @click.argument('args', nargs=-1, metavar='workflowid=value workflowname=value sourceid=value targetid=value')
 @click.pass_obj
 @output_option
 @select_option
 def get_edges(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.workflows.get_edges(**vars_dict)
     process_output(output, select, response)
 
 
-@workflow.command('update_edge', short_help='None')
+@workflow.command('update_edge', short_help='Updates an edge')
 @click.argument('args', nargs=-1, metavar='sys_id=value workflow_id=value condition=value straight_edge=value points=value source_id=value target_id=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 def update_edge(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
     response = uac.workflows.update_edge(**vars_dict)
     process_output(output, select, response)
 
 
-@workflow.command('add_edge', short_help='None')
+@workflow.command('add_edge', short_help='Adds an edge')
 @click.argument('args', nargs=-1, metavar='workflowid=value workflowname=value condition=value straight_edge=value points=value source_id=value target_id=value')
 @click.pass_obj
 @output_option
 @select_option
 def add_edge(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.workflows.add_edge(**vars_dict)
     process_output(output, select, response)
 
 
-@workflow.command('delete_edge', short_help='None')
+@workflow.command('delete_edge', short_help='Deletes an edge')
 @click.argument('args', nargs=-1, metavar='workflowid=value workflowname=value sourceid=value targetid=value')
 @click.pass_obj
 @output_option
 @select_option
 def delete_edge(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.workflows.delete_edge(**vars_dict)
     process_output(output, select, response)
 
 
-@workflow.command('get_vertices', short_help='None')
+@workflow.command('get_vertices', short_help='Gets a vertex')
 @click.argument('args', nargs=-1, metavar='workflowid=value workflowname=value taskid=value taskname=value taskalias=value vertexid=value')
 @click.pass_obj
 @output_option
 @select_option
 def get_vertices(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.workflows.get_vertices(**vars_dict)
     process_output(output, select, response)
 
 
-@workflow.command('update_vertex', short_help='None')
+@workflow.command('update_vertex', short_help='Updates a vertex')
 @click.argument('args', nargs=-1, metavar='sys_id=value workflow_id=value task=value alias=value vertex_id=value vertex_x=value vertex_y=value')
 @click.pass_obj
 @output_option
 @input_option
 @select_option
 def update_vertex(uac: UniversalController, args, output=None, input=None, select=None):
     vars_dict = process_input(args, input)
@@ -95,27 +95,37 @@
 @select_option
 def add_child_vertex(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.workflows.add_child_vertex(**vars_dict)
     process_output(output, select, response)
 
 
-@workflow.command('delete_vertices', short_help='None')
+@workflow.command('delete_vertice', short_help='Deletes a vertice')
 @click.argument('args', nargs=-1, metavar='workflowid=value workflowname=value taskid=value taskname=value taskalias=value vertexid=value')
 @click.pass_obj
 @output_option
 @select_option
-def delete_vertices(uac: UniversalController, args, output=None, select=None):
+def delete_vertice(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.workflows.delete_vertices(**vars_dict)
     process_output(output, select, response)
 
 
-@workflow.command('get_forecast', short_help='None')
+@workflow.command('get_forecast', short_help='Gets the forecast for a workflow')
 @click.argument('args', nargs=-1, metavar='workflowid=value workflowname=value calendarid=value calendarname=value triggerid=value triggername=value date=value time=value timezone=value forecast_timezone=value exclude=value variable=value')
 @click.pass_obj
 @output_option
 @select_option
 def get_forecast(uac: UniversalController, args, output=None, select=None):
     vars_dict = process_input(args)
     response = uac.workflows.get_forecast(**vars_dict)
-    process_output(output, select, response)
+    process_output(output, select, response)
+
+@workflow.command('auto_arrange_vertices', short_help='Auto arrange the vertex locations')
+@click.argument('args', nargs=-1, metavar='workflow_name=value')
+@click.pass_obj
+@output_option
+@select_option
+def auto_arrange_vertices(uac: UniversalController, args, output=None, select=None):
+    vars_dict = process_input(args)
+    response = uac.workflows.auto_arrange_vertices(**vars_dict)
+    process_output(output, select, response)
```

### Comparing `uac-cli-0.2.3/uac_cli/main.py` & `uac-cli-0.2.4/uac_cli/main.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/utils/config.py` & `uac-cli-0.2.4/uac_cli/utils/config.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli/utils/process.py` & `uac-cli-0.2.4/uac_cli/utils/process.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.3/uac_cli.egg-info/PKG-INFO` & `uac-cli-0.2.4/uac_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uac-cli
-Version: 0.2.3
+Version: 0.2.4
 Summary: A CLI tool for executing commands against the Stonebranch UAC API
 Author: Stonebranch
 Author-email: "Huseyin G." <huseyim@gmail.com>
 License: CC BY-NC 4.0
 Project-URL: Homepage, https://github.com/gomleksiz/uac-cli
 Project-URL: Issues, https://github.com/gomleksiz/uac-cli/issues
 Project-URL: Documentation, https://uac-cli.readthedocs.io/en/latest/index.html
```

### Comparing `uac-cli-0.2.3/uac_cli.egg-info/SOURCES.txt` & `uac-cli-0.2.4/uac_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

