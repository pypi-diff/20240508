# Comparing `tmp/owega-5.6.2.tar.gz` & `tmp/owega-5.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owega-5.6.2.tar", last modified: Tue Apr 23 20:55:18 2024, max compression
+gzip compressed data, was "owega-5.6.3.tar", last modified: Wed May  8 02:37:45 2024, max compression
```

## Comparing `owega-5.6.2.tar` & `owega-5.6.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.699515 owega-5.6.2/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      496 2024-04-17 02:21:38.000000 owega-5.6.2/LICENSE
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15764 2024-04-23 20:55:18.699515 owega-5.6.2/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5023 2024-04-17 02:21:38.000000 owega-5.6.2/README.md
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.697515 owega-5.6.2/owega/
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.698515 owega-5.6.2/owega/OweHandlers/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      874 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_add_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1430 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_commands.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1076 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_context.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1515 2024-04-18 20:54:01.000000 owega-5.6.2/owega/OweHandlers/handle_del_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1695 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_dinput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3372 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_edit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1175 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_estimation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4778 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_finput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1692 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_frequency.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      418 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_genconf.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      422 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_history.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3056 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_image.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      993 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_load.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1568 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_model.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1670 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_presence.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      552 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_quit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      967 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_save.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      846 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_system.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1617 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_temperature.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1277 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_tokens.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1446 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_top_p.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1105 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_tts.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handlers.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.698515 owega-5.6.2/owega/OwegaFun/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OwegaFun/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OwegaFun/functions.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4341 2024-04-18 20:54:01.000000 owega-5.6.2/owega/OwegaFun/longTermSouvenirs.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5813 2024-04-18 20:54:01.000000 owega-5.6.2/owega/OwegaFun/utility.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.699515 owega-5.6.2/owega/OwegaSession/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OwegaSession/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2762 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OwegaSession/main_bottom_toolbar.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5590 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OwegaSession/promptsession.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       62 2024-04-17 02:21:38.000000 owega-5.6.2/owega/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.6.2/owega/__main__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     9249 2024-04-18 20:54:01.000000 owega-5.6.2/owega/ask.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.699515 owega-5.6.2/owega/changelog/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-17 02:21:38.000000 owega-5.6.2/owega/changelog/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    23651 2024-04-23 20:40:46.000000 owega-5.6.2/owega/changelog/changelog.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1533 2024-04-17 02:21:38.000000 owega-5.6.2/owega/changelog/changelogEntry.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.6.2/owega/changelog/version.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.699515 owega-5.6.2/owega/config/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.6.2/owega/config/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1808 2024-04-17 02:21:38.000000 owega-5.6.2/owega/config/baseConf.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.699515 owega-5.6.2/owega/conversation/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.6.2/owega/conversation/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10102 2024-04-18 20:54:01.000000 owega-5.6.2/owega/conversation/conversation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1417 2024-04-18 20:54:01.000000 owega-5.6.2/owega/getLogger.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.6.2/owega/handlerBase.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      549 2024-04-17 02:21:38.000000 owega-5.6.2/owega/license.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    12104 2024-04-23 20:51:39.000000 owega-5.6.2/owega/owega.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6107 2024-04-23 20:31:42.000000 owega-5.6.2/owega/utils.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.699515 owega-5.6.2/owega.egg-info/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15764 2024-04-23 20:55:18.000000 owega-5.6.2/owega.egg-info/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1656 2024-04-23 20:55:18.000000 owega-5.6.2/owega.egg-info/SOURCES.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-04-23 20:55:18.000000 owega-5.6.2/owega.egg-info/dependency_links.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-04-23 20:55:18.000000 owega-5.6.2/owega.egg-info/entry_points.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-23 20:55:18.000000 owega-5.6.2/owega.egg-info/requires.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-04-23 20:55:18.000000 owega-5.6.2/owega.egg-info/top_level.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.6.2/pyproject.toml
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-04-23 20:55:18.699515 owega-5.6.2/setup.cfg
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2082 2024-04-17 02:21:38.000000 owega-5.6.2/setup.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.573945 owega-5.6.3/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      496 2024-04-17 02:21:38.000000 owega-5.6.3/LICENSE
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15847 2024-05-08 02:37:45.572944 owega-5.6.3/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5023 2024-04-17 02:21:38.000000 owega-5.6.3/README.md
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.570945 owega-5.6.3/owega/
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.571945 owega-5.6.3/owega/OweHandlers/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-27 12:05:16.000000 owega-5.6.3/owega/OweHandlers/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      980 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_add_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1590 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_commands.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1185 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_context.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1601 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_del_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_dinput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3457 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_edit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1339 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_estimation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5059 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_finput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_frequency.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      521 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_genconf.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      523 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_history.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3310 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_image.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1118 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_load.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1698 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_model.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1791 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_presence.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      637 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_quit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1090 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_save.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      945 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_system.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1739 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_temperature.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1404 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_tokens.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1556 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_top_p.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1245 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_tts.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-04-27 12:05:16.000000 owega-5.6.3/owega/OweHandlers/handlers.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.571945 owega-5.6.3/owega/OwegaFun/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-27 12:05:16.000000 owega-5.6.3/owega/OwegaFun/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.6.3/owega/OwegaFun/functions.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4342 2024-04-27 12:05:16.000000 owega-5.6.3/owega/OwegaFun/longTermSouvenirs.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5816 2024-04-27 12:05:16.000000 owega-5.6.3/owega/OwegaFun/utility.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.572944 owega-5.6.3/owega/OwegaSession/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.6.3/owega/OwegaSession/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2763 2024-04-27 12:05:16.000000 owega-5.6.3/owega/OwegaSession/main_bottom_toolbar.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5592 2024-04-27 12:05:16.000000 owega-5.6.3/owega/OwegaSession/promptsession.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      175 2024-05-08 01:58:10.000000 owega-5.6.3/owega/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.6.3/owega/__main__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     9227 2024-05-08 02:31:24.000000 owega-5.6.3/owega/ask.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.572944 owega-5.6.3/owega/changelog/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-27 12:05:16.000000 owega-5.6.3/owega/changelog/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    23840 2024-05-08 02:33:11.000000 owega-5.6.3/owega/changelog/changelog.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1534 2024-04-27 12:05:16.000000 owega-5.6.3/owega/changelog/changelogEntry.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.6.3/owega/changelog/version.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.572944 owega-5.6.3/owega/config/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.6.3/owega/config/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1810 2024-04-27 12:05:16.000000 owega-5.6.3/owega/config/baseConf.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.572944 owega-5.6.3/owega/conversation/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.6.3/owega/conversation/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10105 2024-04-27 12:05:16.000000 owega-5.6.3/owega/conversation/conversation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1417 2024-04-18 20:54:01.000000 owega-5.6.3/owega/getLogger.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.6.3/owega/handlerBase.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      549 2024-04-17 02:21:38.000000 owega-5.6.3/owega/license.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    12103 2024-04-27 12:05:16.000000 owega-5.6.3/owega/owega.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6111 2024-04-27 12:05:16.000000 owega-5.6.3/owega/utils.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.572944 owega-5.6.3/owega.egg-info/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15847 2024-05-08 02:37:45.000000 owega-5.6.3/owega.egg-info/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1656 2024-05-08 02:37:45.000000 owega-5.6.3/owega.egg-info/SOURCES.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-08 02:37:45.000000 owega-5.6.3/owega.egg-info/dependency_links.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-08 02:37:45.000000 owega-5.6.3/owega.egg-info/entry_points.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-05-08 02:37:45.000000 owega-5.6.3/owega.egg-info/requires.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-08 02:37:45.000000 owega-5.6.3/owega.egg-info/top_level.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.6.3/pyproject.toml
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-08 02:37:45.573945 owega-5.6.3/setup.cfg
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2082 2024-04-27 12:05:16.000000 owega-5.6.3/setup.py
```

### Comparing `owega-5.6.2/PKG-INFO` & `owega-5.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.6.2
+Version: 5.6.3
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: WTFPL
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -135,15 +135,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.6.2 CHANGELOG:
+OWEGA v5.6.3 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -352,13 +352,15 @@
 5.5.2: Added debug info on mistral's part of ask()
        Added matching for mixtral
 5.5.3: Removed debug lines that shouldn't have been left there.
 5.5.4: Fixed a debug_print never showing.
 5.5.5: Now using openai module to ask mistral API.
        (the code is waaaay cleaner)
 
-5.6.0: Added basic support for Chub's API 
+5.6.0: Added basic support for Chub's API
        (chub mars, mercury, mixtral)
        Also, Mi(s/x)tral support is no more in beta :D
 5.6.1: Added extensive logging for errors.
 5.6.2: Added terminal title status :3
+5.6.3: Fixes config's api_key not being used.
+       Better docstrings on handlers.
 ```
```

### Comparing `owega-5.6.2/README.md` & `owega-5.6.3/README.md`

 * *Files identical despite different names*

### Comparing `owega-5.6.2/owega/OweHandlers/handle_add_sysmem.py` & `owega-5.6.3/owega/OweHandlers/handle_add_sysmem.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 """Handle /add_sysmem."""
 import prompt_toolkit as pt
-from ..utils import (
-    info_print,
-    clrtxt,
-)
+
 from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt, info_print
 
 
 # adds a system message
 def handle_add_sysmem(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /add_sysmem."""
+    """Handle /add_sysmem.
+
+    Command description:
+        Adds a system souvenir (permanent).
+
+    Usage:
+        /add_sysmem [souvenir]
+    """
     given = given.strip()
     if not given:
         try:
             given = ps['main'].prompt(pt.ANSI(
                 '\n' + clrtxt("magenta", " System souvenir ") + ": ")).strip()
         except (KeyboardInterrupt, EOFError):
             return messages
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_commands.py` & `owega-5.6.3/owega/OweHandlers/handle_commands.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 """Handle /commands."""
-from ..OwegaFun import existingFunctions
 from ..config import baseConf
-from ..utils import info_print
+from ..OwegaFun import existingFunctions
 from ..OwegaSession import OwegaSession as ps
+from ..utils import info_print
 
 
 # enables/disables command execution
 def handle_commands(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /add_commands."""
+    """Handle /commands.
+
+    Command description:
+        Toggles command execution / file creation.
+
+    Usage:
+        /commands [on/true/enable/enabled/off/false/disable/disabled]
+    """
     given = given.strip()
     if given.lower() in ["on", "true", "enable", "enabled"]:
         baseConf["commands"] = True
         existingFunctions.enableGroup("utility.system")
         if not silent:
             info_print("Command execution enabled.")
         return messages
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_context.py` & `owega-5.6.3/owega/OweHandlers/handle_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """Handle /context."""
 import prompt_toolkit as pt
-from ..utils import (info_print, clrtxt)
+
 from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt, info_print
 
 
 # change owega's system prompt
 def handle_context(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /context."""
+    """Handle /context.
+
+    Command description:
+        Changes the AI's behaviour.
+
+    Usage:
+        /context [new context]
+    """
     given = given.strip()
     if given:
         messages.set_context(given)
         if not silent:
             info_print(f"New context: {messages.get_context()}")
         return messages
     if not silent:
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_del_sysmem.py` & `owega-5.6.3/owega/OweHandlers/handle_del_sysmem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 """Handle /del_sysmem."""
 import prompt_toolkit as pt
-from ..utils import (
-    info_print,
-    clrtxt,
-)
+
 from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt, info_print
 
 
 # adds a system message
 def handle_del_sysmem(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /del_sysmem."""
+    """Handle /del_sysmem.
+
+    Command description:
+        Deletes a system souvenir.
+
+    Usage:
+        /del_sysmem
+    """
     given = given.strip()
     for index, sysmem in enumerate(messages.systemsouv):
         if not silent:
             print("[\033[0;95mSystem souvenir\033[0m] "
                   + f"[\033[0;92m{index}\033[0m]:")
             print('\033[0;37m', end='')
             print(sysmem)
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_dinput.py` & `owega-5.6.3/owega/OweHandlers/handle_dinput.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Handle /dir_input."""
 import os
+
 import prompt_toolkit as pt
-from ..utils import (
-    clrtxt,
-    info_print,
-)
+
 from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt, info_print
 from .handle_finput import guess_language
 
 
 def is_readable(filename: str) -> bool:
     try:
         open(filename, 'r').read()
     except UnicodeDecodeError:
@@ -31,15 +30,22 @@
 def handle_dinput(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /dir_input."""
+    """Handle /dir_input.
+
+    Command description:
+        Sends text-readable files from a given directory.
+
+    Usage:
+        /dir_input [directory]
+    """
     given = given.strip()
     if given:
         dir_path = given
     else:
         dir_path = ps['dirload'].prompt(pt.ANSI(
             clrtxt("yellow", " DIR LOCATION ") + ": ")).strip()
     for file_path in file_list(dir_path):
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_edit.py` & `owega-5.6.3/owega/OweHandlers/handle_edit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 """Handle /edit."""
 import editor
 import prompt_toolkit as pt
-from ..utils import (
-    info_print,
-    clrtxt,
-)
+
 from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt, info_print
 
 
 def handle_edit(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /edit."""
+    """Handle /edit.
+
+    Command description:
+        Edits the history.
+
+    Usage:
+        /edit [message id]
+    """
     given = given.strip()
     ids = []
     for msg_id, msg in enumerate(messages.messages):
         if isinstance(msg.get('content', ''), str):
             ids.append(msg_id)
             role = msg.get('role', 'unknown')
             if role == 'user':
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_estimation.py` & `owega-5.6.3/owega/OweHandlers/handle_tts.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,50 @@
-"""Handle /estimation."""
+"""Handle /tts."""
 from ..config import baseConf
-from ..utils import info_print
 from ..OwegaSession import OwegaSession as ps
+from ..utils import info_print
 
 
-# enables/disables command execution
-def handle_estimation(
+# enables/disables the TTS
+def handle_tts(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /estimation."""
+    """Handle /tts.
+
+    Command description:
+        Toggles the TTS output.
+
+    Usage:
+        /tts [on/true/enable/enabled/off/false/disable/disabled]
+    """
     given = given.strip()
     if given.lower() in ["on", "true", "enable", "enabled"]:
-        baseConf["estimation"] = True
+        baseConf["tts_enabled"] = True
         if not silent:
-            info_print("Token estimation enabled.")
+            info_print("Text-to-speech enabled.")
         return messages
 
     if given.lower() in ["off", "false", "disable", "disabled"]:
-        baseConf["estimation"] = False
+        baseConf["tts_enabled"] = False
         if not silent:
-            info_print("Token estimation disabled.")
+            info_print("Text-to-speech disabled.")
         return messages
 
-    baseConf["estimation"] = (not baseConf.get("estimation", False))
-    if baseConf.get("estimation", False):
+    baseConf["tts_enabled"] = (not baseConf.get("tts_enabled", False))
+    if baseConf.get("tts_enabled", False):
         if not silent:
-            info_print("Token estimation enabled.")
+            info_print("Text-to-speech enabled.")
     else:
         if not silent:
-            info_print("Token estimation disabled.")
+            info_print("Text-to-speech disabled.")
     return messages
 
 
-item_estimation = {
-    "fun": handle_estimation,
-    "help": "toggles displaying the token estimation",
-    "commands": ["estimation"],
+item_tts = {
+    "fun": handle_tts,
+    "help": "enables/disables the TTS",
+    "commands": ["tts"],
 }
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_finput.py` & `owega-5.6.3/owega/OweHandlers/handle_finput.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 """Handle /file_input."""
 import os
+
 import prompt_toolkit as pt
-from ..utils import (
-    clrtxt,
-    info_print,
-)
+
 from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt, info_print
 
 
 def guess_language(file_path: str) -> str:
-    """Try to guess the file's [programming] language."""
+    """
+    Try to guess the file's [programming] language.
+
+    Args:
+        file_path: The path to the file to guess.
+
+    Returns:
+        A string corresponding to the guessed programming language.
+    """
     filename = file_path.split('/')[-1].lower()
     if 'iptables' in filename:
         return 'iptables'
     if 'makefile' in filename:
         return 'makefile'
 
     ext = filename.split('.')[-1]
@@ -100,15 +107,22 @@
 def handle_finput(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /file_input."""
+    """Handle /file_input.
+
+    Command description:
+        Sends a prompt and a file from the system.
+
+    Usage:
+        /file_input [file] [pre-file prompt]
+    """
     given = given.strip()
     if given.split(' ')[0]:
         file_path = given.split(' ')[0]
         given = ' '.join(given.split(' ')[1:])
     else:
         file_path = ps['load'].prompt(pt.ANSI(
             clrtxt("yellow", " FILE LOCATION ") + ": ")).strip()
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_frequency.py` & `owega-5.6.3/owega/OweHandlers/handle_frequency.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """Handle /frequency."""
 import prompt_toolkit as pt
+
 from ..config import baseConf
-from ..utils import (
-    info_print,
-    clrtxt,
-)
 from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt, info_print
 
 
 # change frequency penalty
 def handle_frequency(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /frequency."""
+    """Handle /frequency.
+
+    Command description:
+        Sets the frequency penalty (0.0 - 2.0, defaults 0.0).
+
+    Usage:
+        /frequency [frequency]
+    """
     given = given.strip()
     try:
         new_frequency_penalty = float(given)
     except ValueError:
         if not silent:
             info_print('Current frequency penalty: '
                 + f'{baseConf.get("frequency_penalty", 1.0)}')
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_image.py` & `owega-5.6.3/owega/OweHandlers/handle_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """Handle /image."""
-import openai
-import tempfile
-import prompt_toolkit as pt
 import base64
 import mimetypes
-from ..utils import (
-    info_print,
-    estimated_tokens,
-    clrtxt,
-    play_tts,
-)
-from ..OwegaSession import OwegaSession as ps
-from ..config import baseConf
-from ..OwegaFun import existingFunctions, functionlist_to_toollist
+import tempfile
 import time
+
+import openai
+import prompt_toolkit as pt
+
 from ..ask import ask
+from ..config import baseConf
+from ..OwegaFun import existingFunctions, functionlist_to_toollist
+from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt, estimated_tokens, info_print, play_tts
 
 
-def encode_image(filename):
-    """Return the local image as a base64 url."""
+def encode_image(filename: str) -> str:
+    """
+    Return the local image as a base64 url.
+
+    Args:
+        filename: The path to the image file to encode.
+
+    Returns:
+        The base64url-encoded image.
+    """
     if "http" in filename:
         return filename
     out_str = filename
     try:
         with open(filename, "rb") as image_data:
             mt = mimetypes.guess_type(filename)[0]
             if not isinstance(mt, str):
@@ -33,15 +38,22 @@
         pass
     return out_str
 
 
 def handle_image(
     temp_file, messages, given="", temp_is_temp=False, silent=False
 ):
-    """Handle /image."""
+    """Handle /image.
+
+    Command description:
+        Sends a prompt and an image from an url.
+
+    Usage:
+        /image [image path/url] [prompt]
+    """
     given = given.strip()
     user_prompt = ''
     if given.split(' ')[0]:
         image_url = given.split(' ')[0]
         user_prompt = ' '.join(given.split(' ')[1:])
     else:
         image_url = ps['main'].prompt(pt.ANSI(
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_load.py` & `owega-5.6.3/owega/OweHandlers/handle_load.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """Handle /load."""
 import prompt_toolkit as pt
-from ..utils import clrtxt
+
 from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt
 
 
 # loads the messages and prompt from a json file
 def handle_load(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /load."""
+    """Handle /load.
+
+    Command description:
+        Loads the conversation history from a file.
+
+    Usage:
+        /load [history file]
+    """
     given = given.strip()
     file_path = ''
     try:
         if given:
             file_path = given
         else:
             file_path = ps['load'].prompt(pt.ANSI(
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_model.py` & `owega-5.6.3/owega/OweHandlers/handle_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 """Handle /model."""
 import prompt_toolkit as pt
+
 from ..config import baseConf, list_models
-from ..utils import (info_print, clrtxt)
 from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt, info_print
 
 
 # changes the selected model
 def handle_model(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /model."""
+    """Handle /model.
+
+    Command description:
+        List the available models and prompt for change.
+
+    Usage:
+        /model [model name/ID]
+    """
     given = given.strip()
     if not silent:
         info_print(f"Current model: {baseConf.get('model', '')}")
         list_models()
         print()
     if given:
         new_model = given
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_presence.py` & `owega-5.6.3/owega/OweHandlers/handle_presence.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """Handle /presence."""
 import prompt_toolkit as pt
+
 from ..config import baseConf
-from ..utils import (
-    info_print,
-    clrtxt,
-)
 from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt, info_print
 
 
 # change presence penalty
 def handle_presence(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /presence."""
+    """Handle /presence.
+
+    Command description:
+        Sets the presence penalty (0.0 - 2.0, defaults 0.0).
+
+    Usage:
+        /presence [presence]
+    """
     given = given.strip()
     try:
         new_presence_penalty = float(given)
     except ValueError:
         if not silent:
             info_print('Current presence penalty: '
                 + f'{baseConf.get("presence_penalty", 1.0)}')
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_quit.py` & `owega-5.6.3/owega/OweHandlers/handle_quit.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 """Handle /quit."""
-from ..utils import (
-    do_quit,
-    success_msg,
-)
 from ..OwegaSession import OwegaSession as ps
+from ..utils import do_quit, success_msg
 
 
 # quits the program, deleting temp_file
 def handle_quit(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /quit."""
+    """Handle /quit.
+
+    Command description:
+        Exits the program.
+
+    Usage:
+        /quit
+        /exit
+    """
     do_quit(
         success_msg(),
         temp_file=temp_file,
         is_temp=temp_is_temp,
         should_del=temp_is_temp
     )
     return messages
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_save.py` & `owega-5.6.3/owega/OweHandlers/handle_save.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """Handle /save."""
 import prompt_toolkit as pt
-from ..utils import clrtxt
+
 from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt
 
 
 # saves the messages and prompt to a json file
 def handle_save(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /save."""
+    """Handle /save.
+
+    Command description:
+        Saves the conversation history to a file.
+
+    Usage:
+        /save [history file]
+    """
     given = given.strip()
     try:
         if given:
             file_path = given
         else:
             file_path = ps['save'].prompt(pt.ANSI(
                 '\n' + clrtxt("magenta", " file output ") + ': ')).strip()
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_system.py` & `owega-5.6.3/owega/OweHandlers/handle_system.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 """Handle /system."""
 import prompt_toolkit as pt
-from ..utils import (
-    info_print,
-    clrtxt,
-)
+
 from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt, info_print
 
 
 # adds a system message
 def handle_system(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /system."""
+    """Handle /system.
+
+    Command description:
+        Adds a system prompt in the chat.
+
+    Usage:
+        /system [message]
+    """
     given = given.strip()
     if not given:
         try:
             given = ps['main'].prompt(pt.ANSI(
                 '\n' + clrtxt("magenta", " System message ") + ": ")).strip()
         except (KeyboardInterrupt, EOFError):
             return messages
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_temperature.py` & `owega-5.6.3/owega/OweHandlers/handle_temperature.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """Handle /temperature."""
 import prompt_toolkit as pt
+
 from ..config import baseConf
-from ..utils import (
-    info_print,
-    clrtxt,
-)
 from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt, info_print
 
 
 # change temperature
 def handle_temperature(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /temperature."""
+    """Handle /temperature.
+
+    Command description:
+        Sets the temperature (0.0 - 1.0, defaults 0.8).
+
+    Usage:
+        /temperature [temperature]
+    """
     given = given.strip()
     try:
         new_temperature = float(given)
     except ValueError:
         if not silent:
             info_print('Current temperature: '
                 + f'{baseConf.get("temperature", 1.0)}')
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_tokens.py` & `owega-5.6.3/owega/OweHandlers/handle_tokens.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 """Handle /tokens."""
 import prompt_toolkit as pt
+
 from ..config import baseConf
-from ..utils import (info_print, clrtxt)
 from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt, info_print
 
 
 # change requested tokens amount
 def handle_tokens(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /tokens."""
+    """Handle /tokens.
+
+    Command description:
+        Changes the max amount of requested tokens.
+
+    Usage:
+        /tokens [max tokens]
+    """
     given = given.strip()
     if given.isdigit():
         baseConf["max_tokens"] = int(given)
         if not silent:
             info_print(f'Set requested tokens to {baseConf.get("max_tokens", 3000)}')
         return messages
     if not silent:
@@ -34,10 +42,10 @@
         if not silent:
             info_print('Invalid input, keeping current requested tokens amount')
     return messages
 
 
 item_tokens = {
     "fun": handle_tokens,
-    "help": "changes the amount of requested tokens",
+    "help": "changes the max amount of requested tokens",
     "commands": ["tokens"],
 }
```

### Comparing `owega-5.6.2/owega/OweHandlers/handle_top_p.py` & `owega-5.6.3/owega/OweHandlers/handle_top_p.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """Handle /top_p."""
 import prompt_toolkit as pt
+
 from ..config import baseConf
-from ..utils import (
-    info_print,
-    clrtxt,
-)
 from ..OwegaSession import OwegaSession as ps
+from ..utils import clrtxt, info_print
 
 
 # change top_p value
 def handle_top_p(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
-    """Handle /top_p."""
+    """Handle /top_p.
+
+    Command description:
+        Sets the top_p value (0.0 - 1.0, defaults 1.0).
+
+    Usage:
+        /top_p [top_p]
+    """
     given = given.strip()
     try:
         new_top_p = float(given)
     except ValueError:
         if not silent:
             info_print(f'Current top_p: {baseConf.get("top_p", 1.0)}')
             info_print('New top_p value (0.0 - 1.0, defaults 1.0)')
```

### Comparing `owega-5.6.2/owega/OweHandlers/handlers.py` & `owega-5.6.3/owega/OweHandlers/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """Gather all the handlers."""
+from ..handlerBase import handler_helps, handlers, items
+from ..OwegaSession import OwegaSession as ps
 from ..utils import print_help
-from .handle_quit import item_quit
-from .handle_genconf import item_genconf
-from .handle_history import item_history
+from .handle_add_sysmem import item_add_sysmem
 from .handle_commands import item_commands
-from .handle_estimation import item_estimation
-from .handle_tokens import item_tokens
 from .handle_context import item_context
-from .handle_save import item_save
-from .handle_load import item_load
-from .handle_model import item_model
-from .handle_finput import item_finput
+from .handle_del_sysmem import item_del_sysmem
 from .handle_dinput import item_dinput
-from .handle_temperature import item_temperature
-from .handle_top_p import item_top_p
+from .handle_edit import item_edit
+from .handle_estimation import item_estimation
+from .handle_finput import item_finput
 from .handle_frequency import item_frequency
+from .handle_genconf import item_genconf
+from .handle_history import item_history
+from .handle_image import item_image
+from .handle_load import item_load
+from .handle_model import item_model
 from .handle_presence import item_presence
-from .handle_edit import item_edit
+from .handle_quit import item_quit
+from .handle_save import item_save
 from .handle_system import item_system
-from .handle_add_sysmem import item_add_sysmem
-from .handle_del_sysmem import item_del_sysmem
+from .handle_temperature import item_temperature
+from .handle_tokens import item_tokens
+from .handle_top_p import item_top_p
 from .handle_tts import item_tts
-from .handle_image import item_image
-from ..OwegaSession import OwegaSession as ps
-from ..handlerBase import items, handlers, handler_helps
 
 
 # prints help
 def handle_help(temp_file, messages, given="", temp_is_temp=False):
     """Handle /help."""
     print_help(handler_helps)
     return messages
```

### Comparing `owega-5.6.2/owega/OwegaFun/__init__.py` & `owega-5.6.3/owega/OwegaFun/__init__.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Owega Functions init."""
-from .utility import Utility
 from . import longTermSouvenirs as lts
 # from .longTermSouvenirs import LTS, setAdd, setDel, setEdit
 from .functions import Functions
+from .utility import Utility
 
 existingFunctions = Functions().append(
     Utility, 'utility').append(lts.LTS, 'lts')
 existingFunctions.disableGroup('lts')
 
 
 def connectLTS(addfun, delfun, editfun):
```

### Comparing `owega-5.6.2/owega/OwegaFun/functions.py` & `owega-5.6.3/owega/OwegaFun/functions.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.2/owega/OwegaFun/longTermSouvenirs.py` & `owega-5.6.3/owega/OwegaFun/longTermSouvenirs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Long Term Souvenirs related functions."""
-from .functions import Functions, disabledFunction
 import json
 
+from .functions import Functions, disabledFunction
+
 LTS = Functions()
 
 
 fcts = {}
 fcts["addfun"] = disabledFunction
 fcts["delfun"] = disabledFunction
 fcts["editfun"] = disabledFunction
```

### Comparing `owega-5.6.2/owega/OwegaFun/utility.py` & `owega-5.6.3/owega/OwegaFun/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """Utility functions."""
-from owega.utils import command_text
-from .functions import Functions
+import json
 import subprocess
+
+import bs4
 import prompt_toolkit as pt
-import json
 import requests
-import bs4
 from markdownify import MarkdownConverter as MC
 
+from owega.utils import command_text
+
+from .functions import Functions
+
 Utility = Functions()
 
 
 # executes a given string, if bypass is true, do not ask for confirmation
 # def __execute(command: str, bypass: bool = False):
 def __execute(*args, **kwargs):
     command = ""
```

### Comparing `owega-5.6.2/owega/OwegaSession/main_bottom_toolbar.py` & `owega-5.6.3/owega/OwegaSession/main_bottom_toolbar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Main bottom toolbar for TUI."""
 import prompt_toolkit as pt
-from ..config import baseConf
+
 from ..changelog import OwegaChangelog
+from ..config import baseConf
 
 
 # bottom toolbar and style for prompt_toolkit
 def main_bottom_toolbar(what: str = "toolbar"):
     """Return the bottom style or toolbar."""
     if what == "style":
         msd = {
```

### Comparing `owega-5.6.2/owega/OwegaSession/promptsession.py` & `owega-5.6.3/owega/OwegaSession/promptsession.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Prompt sessions."""
-import re
 import os
+import re
+
 import prompt_toolkit as pt
+
 from ..config import baseConf
+from ..handlerBase import handlers
 from ..utils import get_home_dir
 from .main_bottom_toolbar import main_bottom_toolbar
-from ..handlerBase import handlers
 
 
 def set_ps(ps):
     """Set the prompt sessions."""
     # generate completion from command list (handlers)
     command_list = ['/' + command for command in handlers.keys()]
```

### Comparing `owega-5.6.2/owega/ask.py` & `owega-5.6.3/owega/ask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Ask a question to GPT."""
-from .config import baseConf
-from .conversation import Conversation
-from .OwegaFun import existingFunctions, connectLTS, functionlist_to_toollist
-import time
-import openai
-import json5 as json
 import json as jsonbase
 import re
+import time
+
+import json5 as json
+import openai
 import requests
-from .utils import debug_print
+
 from . import getLogger
+from .config import baseConf
+from .conversation import Conversation
+from .OwegaFun import connectLTS, existingFunctions, functionlist_to_toollist
+from .utils import debug_print
 
 
 def convert_invalid_json(invalid_json):
     """
     Try converting invalid json to valid json.
 
     Sometimes, GPT will give back invalid json.
@@ -53,35 +55,33 @@
     bc["api_key"] = "REDACTED"
     bc["mistral_api"] = "REDACTED"
     bc["chub_api"] = "REDACTED"
     logger.debug(f"{bc}")
 
     connectLTS(
         messages.add_memory, messages.remove_memory, messages.edit_memory)
-    old_api_key = openai.api_key
-    old_organization = openai.organization
     if (prompt):
         messages.add_question(prompt)
     else:
         prompt = messages.last_question()
 
     # Determine if we're using Mistral based on the model name
     is_mistral = False
     is_chub = False
     if model.startswith('chub-'):
         model = model[5:]
         is_chub = True
     elif ("mistral" in model) or ("mixtral" in model):
         is_mistral = True
 
-    headers = {}
-    data_payload = {}
-
     client = openai.OpenAI()
 
+    if (baseConf.get('api_key', '')):
+        client.api_key = baseConf.get('api_key', '')
+
     if is_chub:
         logger.info(f"Using Chub's API for model: {model}")
         if model in ["mars", "asha"]:
             model = "asha"
             client.base_url = 'https://mars.chub.ai/chub/asha/v1'
         elif model in ["mercury", "mythomax"]:
             model = "mythomax"
```

### Comparing `owega-5.6.2/owega/changelog/changelog.py` & `owega-5.6.3/owega/changelog/changelog.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,29 @@
         self.version = Version(0, 0, 0)
         self.initLogs()
         self.genLog()
 
     def initLogs(self):
         """Fill the changelog."""
         self.logs.append(
+            ChangelogEntry(5, 6, 3)
+            .addLine("Fixes config's api_key not being used.")
+            .addLine("Better docstrings on handlers.")
+        )
+        self.logs.append(
             ChangelogEntry(5, 6, 2)
             .addLine("Added terminal title status :3")
         )
         self.logs.append(
             ChangelogEntry(5, 6, 1)
             .addLine("Added extensive logging for errors.")
         )
         self.logs.append(
             ChangelogEntry(5, 6, 0)
-            .addLine("Added basic support for Chub's API ")
+            .addLine("Added basic support for Chub's API")
             .addLine("(chub mars, mercury, mixtral)")
             .addLine("Also, Mi(s/x)tral support is no more in beta :D")
         )
 
         self.logs.append(
             ChangelogEntry(5, 5, 5)
             .addLine("Now using openai module to ask mistral API.")
```

### Comparing `owega-5.6.2/owega/changelog/changelogEntry.py` & `owega-5.6.3/owega/changelog/changelogEntry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Handles a changelog entry."""
 import functools
+
 from .version import Version
 
 
 @functools.total_ordering
 class ChangelogEntry:
     """Handles a changelog entry."""
```

### Comparing `owega-5.6.2/owega/changelog/version.py` & `owega-5.6.3/owega/changelog/version.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.2/owega/config/baseConf.py` & `owega-5.6.3/owega/config/baseConf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Owega base configuration module."""
 
-from owega.utils import get_home_dir, info_print
-from owega.utils import debug_print as dp_internal
 import os
-import openai
+
 import json5 as json
+import openai
+
+from owega.utils import debug_print as dp_internal
+from owega.utils import get_home_dir, info_print
 
 baseModels = [
     "gpt-3.5-turbo-1106",
     "gpt-4-turbo-preview",
     "gpt-4-vision-preview",
     "open-mistral-7b",
     "open-mixtral-8x7b",
```

### Comparing `owega-5.6.2/owega/conversation/conversation.py` & `owega-5.6.3/owega/conversation/conversation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """Handles a GPT conversation history."""
-import json5 as json
 import sys
+
+import json5 as json
+
 from owega.changelog import OwegaChangelog, Version
+
 from .. import getLogger
 
 
 # messages class, contains helper functions to manage context and messages
 class Conversation:
     """Contains an history and everything that should be stored."""
```

### Comparing `owega-5.6.2/owega/getLogger.py` & `owega-5.6.3/owega/getLogger.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.2/owega/license.py` & `owega-5.6.3/owega/license.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.2/owega/owega.py` & `owega-5.6.3/owega/owega.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 #!/usr/bin/env python3
 """Owega's main function. Handle the CLI/TUI."""
 # Import the necessary modules
-import openai
-import os
-import json5 as json
+import argparse
 import getpass
+import os
+import re
 import sys
+import tempfile
 import time
-import re
-import argparse
+
+import json5 as json
+import openai
 import prompt_toolkit as pt
-import tempfile
+
+from .ask import ask
 from .changelog import OwegaChangelog
-from .license import OwegaLicense
 from .config import baseConf, get_conf, list_models
-from .OwegaFun import existingFunctions, connectLTS, functionlist_to_toollist
-from .OweHandlers import handlers, handle_help, handler_helps
-from .utils import (
-    get_home_dir,
-    get_temp_file,
-    info_print,
-    do_quit,
-    success_msg,
-    clrtxt,
-    print_help,
-    estimated_tokens,
-    play_tts,
-    set_term_title,
-)
 from .conversation import Conversation, Conversation_from
-from .ask import ask
+from .license import OwegaLicense
+from .OwegaFun import connectLTS, existingFunctions, functionlist_to_toollist
 from .OwegaSession import OwegaSession as ps
+from .OweHandlers import handle_help, handler_helps, handlers
+from .utils import (clrtxt, do_quit, estimated_tokens, get_home_dir,
+                    get_temp_file, info_print, play_tts, print_help,
+                    set_term_title, success_msg)
 
 
 def get_oc_conf():
     """Get a copy of owega's config."""
     return baseConf.copy()
```

### Comparing `owega-5.6.2/owega/utils.py` & `owega-5.6.3/owega/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """Utilities that don't fit anywhere else."""
 import os
-import tempfile
 import sys
+import tempfile
+import warnings
+
 import json5 as json
-import tiktoken
 import openai
-import warnings
-from .conversation import Conversation
+import tiktoken
+
 from .config import baseConf
+from .conversation import Conversation
+
 os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'
 warnings.filterwarnings("ignore", category=RuntimeWarning, message=".*pygame.*")
 import pygame  # noqa
+
 from . import getLogger
 
 
 def set_term_title(new_title: str):
     print(f"\033]0;{new_title}\a", end='')
```

### Comparing `owega-5.6.2/owega.egg-info/PKG-INFO` & `owega-5.6.3/owega.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.6.2
+Version: 5.6.3
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: WTFPL
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -135,15 +135,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.6.2 CHANGELOG:
+OWEGA v5.6.3 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -352,13 +352,15 @@
 5.5.2: Added debug info on mistral's part of ask()
        Added matching for mixtral
 5.5.3: Removed debug lines that shouldn't have been left there.
 5.5.4: Fixed a debug_print never showing.
 5.5.5: Now using openai module to ask mistral API.
        (the code is waaaay cleaner)
 
-5.6.0: Added basic support for Chub's API 
+5.6.0: Added basic support for Chub's API
        (chub mars, mercury, mixtral)
        Also, Mi(s/x)tral support is no more in beta :D
 5.6.1: Added extensive logging for errors.
 5.6.2: Added terminal title status :3
+5.6.3: Fixes config's api_key not being used.
+       Better docstrings on handlers.
 ```
```

### Comparing `owega-5.6.2/owega.egg-info/SOURCES.txt` & `owega-5.6.3/owega.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owega-5.6.2/setup.py` & `owega-5.6.3/setup.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """Setup config for installing the package."""
 
 from setuptools import setup
-from owega.changelog import OwegaChangelog as oc
 
+from owega.changelog import OwegaChangelog as oc
 
 desc = open('README.md').read()
 desc += '\n\n'
 desc += "## CHANGELOG: "
 desc += '\n```\n'
 desc += oc.log
 desc += '\n```\n'
```

