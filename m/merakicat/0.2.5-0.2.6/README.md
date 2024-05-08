# Comparing `tmp/merakicat-0.2.5.tar.gz` & `tmp/merakicat-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merakicat-0.2.5.tar", last modified: Thu Apr 25 13:24:34 2024, max compression
+gzip compressed data, was "merakicat-0.2.6.tar", last modified: Wed May  8 00:16:38 2024, max compression
```

## Comparing `merakicat-0.2.5.tar` & `merakicat-0.2.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.895661 merakicat-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.883662 merakicat-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.887662 merakicat-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-25 13:24:28.000000 merakicat-0.2.5/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-25 13:24:28.000000 merakicat-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 13:24:28.000000 merakicat-0.2.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-25 13:24:28.000000 merakicat-0.2.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-25 13:24:28.000000 merakicat-0.2.5/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-25 13:24:28.000000 merakicat-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 13:24:28.000000 merakicat-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-25 13:24:28.000000 merakicat-0.2.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-04-25 13:24:34.895661 merakicat-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-04-25 13:24:28.000000 merakicat-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.887662 merakicat-0.2.5/files/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 13:24:28.000000 merakicat-0.2.5/files/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.891662 merakicat-0.2.5/images/
--rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-04-25 13:24:28.000000 merakicat-0.2.5/images/botcongrats.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-04-25 13:24:28.000000 merakicat-0.2.5/images/cisco_meraki.png
--rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-04-25 13:24:28.000000 merakicat-0.2.5/images/createbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-04-25 13:24:28.000000 merakicat-0.2.5/images/mc_quick.gif
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-25 13:24:28.000000 merakicat-0.2.5/images/merakicat.png
--rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-25 13:24:28.000000 merakicat-0.2.5/images/newapp.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-04-25 13:24:28.000000 merakicat-0.2.5/images/newbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-25 13:24:28.000000 merakicat-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-25 13:24:28.000000 merakicat-0.2.5/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 13:24:34.895661 merakicat-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-25 13:24:28.000000 merakicat-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.883662 merakicat-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.895661 merakicat-0.2.5/src/merakicat/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.895661 merakicat-0.2.5/src/merakicat/batch_helper/
--rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/batch_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/batch_helper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/batch_helper/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/bulk_check.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/bulk_migrate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     6487 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_cfg_check.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4690 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_cloud_mon.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1275 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_file_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_get_nms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    54918 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_pedia.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_ping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8881 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_register.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_splitcheck_serials.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    35813 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_user_info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    91540 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/merakicat.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.895661 merakicat-0.2.5/src/merakicat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-04-25 13:24:34.000000 merakicat-0.2.5/src/merakicat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-25 13:24:34.000000 merakicat-0.2.5/src/merakicat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:24:34.000000 merakicat-0.2.5/src/merakicat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:24:34.000000 merakicat-0.2.5/src/merakicat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-25 13:24:34.000000 merakicat-0.2.5/src/merakicat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 13:24:34.000000 merakicat-0.2.5/src/merakicat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-25 13:24:28.000000 merakicat-0.2.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:16:38.980372 merakicat-0.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:16:38.968371 merakicat-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:16:38.972371 merakicat-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-08 00:16:32.000000 merakicat-0.2.6/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-08 00:16:32.000000 merakicat-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-08 00:16:32.000000 merakicat-0.2.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-08 00:16:32.000000 merakicat-0.2.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-08 00:16:32.000000 merakicat-0.2.6/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-08 00:16:32.000000 merakicat-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 00:16:32.000000 merakicat-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-08 00:16:32.000000 merakicat-0.2.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-05-08 00:16:38.980372 merakicat-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7800 2024-05-08 00:16:32.000000 merakicat-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:16:38.972371 merakicat-0.2.6/files/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 00:16:32.000000 merakicat-0.2.6/files/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:16:38.976372 merakicat-0.2.6/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-05-08 00:16:32.000000 merakicat-0.2.6/images/botcongrats.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-05-08 00:16:32.000000 merakicat-0.2.6/images/cisco_meraki.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-05-08 00:16:32.000000 merakicat-0.2.6/images/createbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-05-08 00:16:32.000000 merakicat-0.2.6/images/mc_quick.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-05-08 00:16:32.000000 merakicat-0.2.6/images/merakicat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-05-08 00:16:32.000000 merakicat-0.2.6/images/newapp.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-05-08 00:16:32.000000 merakicat-0.2.6/images/newbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-08 00:16:32.000000 merakicat-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 00:16:32.000000 merakicat-0.2.6/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:16:38.980372 merakicat-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-08 00:16:32.000000 merakicat-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:16:38.968371 merakicat-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:16:38.976372 merakicat-0.2.6/src/merakicat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:16:38.980372 merakicat-0.2.6/src/merakicat/batch_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/batch_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/batch_helper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/batch_helper/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/bulk_check.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/bulk_migrate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6487 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/mc_cfg_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4939 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/mc_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/mc_cloud_mon.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1275 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/mc_file_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/mc_get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/mc_get_nms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54918 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/mc_pedia.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/mc_ping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8881 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/mc_register.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/mc_splitcheck_serials.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35813 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/mc_translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/mc_user_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    91540 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/merakicat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 00:16:32.000000 merakicat-0.2.6/src/merakicat/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:16:38.980372 merakicat-0.2.6/src/merakicat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-05-08 00:16:38.000000 merakicat-0.2.6/src/merakicat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-08 00:16:38.000000 merakicat-0.2.6/src/merakicat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:16:38.000000 merakicat-0.2.6/src/merakicat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:16:38.000000 merakicat-0.2.6/src/merakicat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 00:16:38.000000 merakicat-0.2.6/src/merakicat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 00:16:38.000000 merakicat-0.2.6/src/merakicat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-08 00:16:32.000000 merakicat-0.2.6/tox.ini
```

### Comparing `merakicat-0.2.5/.gitignore` & `merakicat-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/CONTRIBUTING.rst` & `merakicat-0.2.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/HISTORY.md` & `merakicat-0.2.6/HISTORY.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # History
 
+## 0.2.6 (05-07-2024)
+
+  - Resolved Issue #6.
+  - Fixed issue with unclaiming switches before removing switch stack.
+  - Updated requirements.
+
 ## 0.2.5 (04-25-2024)
 
   - Reverted back to Finbarr Brady's webex-bot after a pull merge.
 
 ## 0.2.4 (04-12-2024)
 
   - Added Private VLAN -> Port Isolation to encyclopedia.
```

### Comparing `merakicat-0.2.5/LICENSE` & `merakicat-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/Makefile` & `merakicat-0.2.6/Makefile`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/PKG-INFO` & `merakicat-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.2.5
+Version: 0.2.6
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -18,17 +18,17 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: webex-bot==0.4.7
 Requires-Dist: webexteamssdk==1.6.1
 Requires-Dist: Flask>=0.12.1
 Requires-Dist: netmiko==4.3.0
 Requires-Dist: tabulate==0.9.0
-Requires-Dist: ciscoconfparse2==0.5
-Requires-Dist: meraki==1.42.0
-Requires-Dist: python-docx==1.1.0
+Requires-Dist: ciscoconfparse2==0.7.50
+Requires-Dist: meraki==1.46.0
+Requires-Dist: python-docx==1.1.2
 Requires-Dist: docx2pdf==0.1.8
 Requires-Dist: requests==2.31.0
 
 [![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/ecoen66/merakicat)
 # ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/merakicat.png) merakicat
 
 This package makes migrating [Cisco](https://www.cisco.com) Catalyst switches to [Meraki](https:www.meraki.com) Dashboard much easier. #merakicat
@@ -242,19 +242,25 @@
 # Credits
 **This project is _heavily_ based on the work of others:**
 
 `Catalyst_to_Meraki_Migration_Tool` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
 `Catalyst_2_Meraki_Config_Checker` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
-The bot functionality is based on the `webex_bot` project by [Finbarr Brady](https://github.com/fbradyirl).
+The bot functionality is using `webex_bot` by [Finbarr Brady](https://github.com/fbradyirl).
 
 
 # History
 
+## 0.2.6 (05-07-2024)
+
+  - Resolved Issue #6.
+  - Fixed issue with unclaiming switches before removing switch stack.
+  - Updated requirements.
+
 ## 0.2.5 (04-25-2024)
 
   - Reverted back to Finbarr Brady's webex-bot after a pull merge.
 
 ## 0.2.4 (04-12-2024)
 
   - Added Private VLAN -> Port Isolation to encyclopedia.
```

### Comparing `merakicat-0.2.5/README.md` & `merakicat-0.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -212,8 +212,8 @@
 # Credits
 **This project is _heavily_ based on the work of others:**
 
 `Catalyst_to_Meraki_Migration_Tool` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
 `Catalyst_2_Meraki_Config_Checker` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
-The bot functionality is based on the `webex_bot` project by [Finbarr Brady](https://github.com/fbradyirl).
+The bot functionality is using `webex_bot` by [Finbarr Brady](https://github.com/fbradyirl).
```

### Comparing `merakicat-0.2.5/images/botcongrats.jpg` & `merakicat-0.2.6/images/botcongrats.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/images/cisco_meraki.png` & `merakicat-0.2.6/images/cisco_meraki.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/images/createbot.jpg` & `merakicat-0.2.6/images/createbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/images/mc_quick.gif` & `merakicat-0.2.6/images/mc_quick.gif`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/images/merakicat.png` & `merakicat-0.2.6/images/merakicat.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/images/newapp.jpg` & `merakicat-0.2.6/images/newapp.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/images/newbot.jpg` & `merakicat-0.2.6/images/newbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/setup.py` & `merakicat-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 
 requirements = [
     "webex-bot==0.4.7",
     "webexteamssdk==1.6.1",
     "Flask>=0.12.1",
     "netmiko==4.3.0",
     "tabulate==0.9.0",
-    "ciscoconfparse2==0.5",
-    "meraki==1.42.0",
-    "python-docx==1.1.0",
+    "ciscoconfparse2==0.7.50",
+    "meraki==1.46.0",
+    "python-docx==1.1.2",
     "docx2pdf==0.1.8",
     "requests==2.31.0"
     ]
 
 setup_requirements = [ ]
 
 setup(
```

### Comparing `merakicat-0.2.5/src/merakicat/batch_helper/__init__.py` & `merakicat-0.2.6/src/merakicat/batch_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/src/merakicat/batch_helper/config.py` & `merakicat-0.2.6/src/merakicat/batch_helper/config.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/src/merakicat/batch_helper/exceptions.py` & `merakicat-0.2.6/src/merakicat/batch_helper/exceptions.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/src/merakicat/mc_cfg_check.py` & `merakicat-0.2.6/src/merakicat/mc_cfg_check.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/src/merakicat/mc_claim.py` & `merakicat-0.2.6/src/merakicat/mc_claim.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,84 +20,94 @@
     debug = DEBUG or DEBUG_CLAIM
 
     issues = ""
     claimed_switches = serials
     ac_switches = list()
     bad_switches = list()
 
-    for serial in serials:
-        try:
-            r = (dashboard.networks.removeNetworkDevices(
-                 networkId=dest_net, serial=serial))
-        except meraki.APIError:
-            pass
     try:
-        r = (dashboard.networks.claimNetworkDevices(
-             networkId=dest_net, serials=serials))
+        r = dashboard.switch.getNetworkSwitchStacks(networkId=dest_net)
         if debug:
-            print(f"issues from Dashboard for claiming switches was:\n{r}")
-    # Oops, we got a Dashboard ERROR while claiming switches to the network
+            print(f"I grabbed the list of switch stacks in network {dest_net}, it was {r}")
+        for stack in r:
+            for serial in serials:
+                if serial in stack['serials'][0]:
+                    try:
+                        response = dashboard.switch.deleteNetworkSwitchStack(dest_net,stack['id'])
+                        if debug:
+                            print(f"I deleted switch stack {stack['id']}, with switch {serial}")
+                        break
+                    except meraki.APIError as e:
+                        if debug:
+                            print(f"In an attempt to delete switch stack {stack['id']}, we encountered the following error:")
+                            print(f'Meraki API error: {e}')
+                            print(f'status code = {e.status}')
+                            print(f'reason = {e.reason}')
+                            print(f'error = {e.message}')
+                        continue
     except meraki.APIError as e:
         if debug:
+            print(f"In an attempt to get the list of switch stacks for network {dest_net}, we encountered the following error:")
             print(f'Meraki API error: {e}')
             print(f'status code = {e.status}')
             print(f'reason = {e.reason}')
             print(f'error = {e.message}')
-        # Let's parse through the list of errors returned and divide them
-        # into Already Claimed and Not Found
-        x = 0
-        while x <= len(e.message['errors'])-1:
+
+    for serial in serials:
+        try:
+            r = (dashboard.networks.removeNetworkDevices(
+                 networkId=dest_net, serial=serial))
+            if debug:
+                print(f"I deleted serial number {serial}.")
+        except meraki.APIError as e:
+            if debug:
+                print(f"In an attempt to delete serial number {serial}, we encountered the following error:")
+                print(f'Meraki API error: {e}')
+                print(f'status code = {e.status}')
+                print(f'reason = {e.reason}')
+                print(f'error = {e.message}')
+            continue
+
+    x = 0
+    while x <= len(serials)-1:
+        try:
+            r = (dashboard.networks.claimNetworkDevices(
+                 networkId=dest_net, serials=[serials[x]]))
+            if debug:
+                print(f"issues from Dashboard for claiming switch {serials[x]} was:\n{r}")
+        # Oops, we got a Dashboard ERROR while claiming switches to the network
+        except meraki.APIError as e:
+            if debug:
+                print(f'Meraki API error: {e}')
+                print(f'status code = {e.status}')
+                print(f'reason = {e.reason}')
+                print(f'error = {e.message}')
+            # Let's parse through the list of errors returned and divide them
+            # into Already Claimed and Not Found
             # If it is already claimed...
-            if re.search('already claimed', e.message['errors'][x]):
-                if debug:
-                    print(e.message['errors'][x].split(
-                          "Device with serial")[1].split()[0])
-                ac_switch = e.message['errors'][x].split(
-                    "Device with serial")[1].split()[0]
-                if debug:
-                    print(e.message['errors'][x].split(
-                          "already claimed and in ")[1].split('(')[0])
-                ac_net_name = e.message['errors'][x].split(
-                    "already claimed and in ")[1].split("(")[0]
-                if debug:
-                    print(e.message['errors'][x].split(
-                          "already claimed and in ")[1].split(
-                          "network ID: ")[1].split(')')[0])
-                # If it is already claimed but in a different network
-                # remove it from the claimed_switches list
-                # append it to the bad_switches list
-                # append a ERROR to the issues string
-                if not (e.message['errors'][x].split(
-                    "already claimed and in ")[1].split(
-                        "network ID: ")[1].split(')')[0]) == dest_net:
-                    issues += "ERROR: Switch "+ac_switch+" has already "
-                    issues += "been claimed and is in the "+ac_net_name
-                    issues += " network.\n"
-                    claimed_switches.remove(ac_switch)
-                    bad_switches.append(ac_switch)
+            if re.search('Devices already claimed', e.message['errors'][0]):
+                ac_switch = serials[x]
+
                 # If it is already claimed in the desired network
                 # remove it from the claimed_switches list and append it to
                 # ac_switches list and append a WARNING to the issues string
-                else:
-                    issues += "Warning: Switch "+ac_switch+" has already "
-                    issues += "been claimed in that network.\n"
-                    ac_switches.append(ac_switch)
+                issues += "Warning: Switch "+ac_switch+" has already "
+                issues += "been claimed in that network.\n"
+                ac_switches.append(ac_switch)
+
             # If it is not found, append it to the bad_switches list
             # remove it from the claimed_switches list and
             # append a ERROR to the issues string
-            elif re.search('not found', e.message['errors'][x]):
-                if debug:
-                    print(e.message['errors'][x].split(
-                        "Device with serial")[1].split()[0])
-                bad_switch = e.message['errors'][x].split(
-                    "Device with serial")[1].split()[0]
-                bad_switches.append(bad_switch)
+            elif re.search('not found', e.message['errors'][0]):
+                bad_switch = serials[x]
+                bad_switches.append(serial)
                 claimed_switches.remove(bad_switch)
                 issues += "Error: Switch "+bad_switch+" was not found.\n"
-            x += 1
-        if debug:
-            print(f"claimed_switches = {claimed_switches}")
-            print(f"ac_switches = {ac_switches}")
-            print(f"bad_switches = {bad_switches}")
-        # Even though we got an error, keep on going...
-        pass
+            # Even though we got an error, keep on going...
+        finally:
+            if debug:
+                print(f"claimed_switches = {claimed_switches}")
+                print(f"ac_switches = {ac_switches}")
+                print(f"bad_switches = {bad_switches}")
+        x += 1
+
     return (issues, bad_switches, ac_switches, claimed_switches)
```

### Comparing `merakicat-0.2.5/src/merakicat/mc_cloud_mon.py` & `merakicat-0.2.6/src/merakicat/mc_cloud_mon.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/src/merakicat/mc_file_exists.py` & `merakicat-0.2.6/src/merakicat/mc_file_exists.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/src/merakicat/mc_get_config.py` & `merakicat-0.2.6/src/merakicat/mc_get_config.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/src/merakicat/mc_get_nms.py` & `merakicat-0.2.6/src/merakicat/mc_get_nms.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/src/merakicat/mc_pedia.py` & `merakicat-0.2.6/src/merakicat/mc_pedia.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/src/merakicat/mc_ping.py` & `merakicat-0.2.6/src/merakicat/mc_ping.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/src/merakicat/mc_register.py` & `merakicat-0.2.6/src/merakicat/mc_register.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/src/merakicat/mc_splitcheck_serials.py` & `merakicat-0.2.6/src/merakicat/mc_splitcheck_serials.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/src/merakicat/mc_translate.py` & `merakicat-0.2.6/src/merakicat/mc_translate.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/src/merakicat/mc_user_info.py` & `merakicat-0.2.6/src/merakicat/mc_user_info.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/src/merakicat/merakicat.py` & `merakicat-0.2.6/src/merakicat/merakicat.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/src/merakicat.egg-info/PKG-INFO` & `merakicat-0.2.6/src/merakicat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.2.5
+Version: 0.2.6
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -18,17 +18,17 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: webex-bot==0.4.7
 Requires-Dist: webexteamssdk==1.6.1
 Requires-Dist: Flask>=0.12.1
 Requires-Dist: netmiko==4.3.0
 Requires-Dist: tabulate==0.9.0
-Requires-Dist: ciscoconfparse2==0.5
-Requires-Dist: meraki==1.42.0
-Requires-Dist: python-docx==1.1.0
+Requires-Dist: ciscoconfparse2==0.7.50
+Requires-Dist: meraki==1.46.0
+Requires-Dist: python-docx==1.1.2
 Requires-Dist: docx2pdf==0.1.8
 Requires-Dist: requests==2.31.0
 
 [![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/ecoen66/merakicat)
 # ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/merakicat.png) merakicat
 
 This package makes migrating [Cisco](https://www.cisco.com) Catalyst switches to [Meraki](https:www.meraki.com) Dashboard much easier. #merakicat
@@ -242,19 +242,25 @@
 # Credits
 **This project is _heavily_ based on the work of others:**
 
 `Catalyst_to_Meraki_Migration_Tool` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
 `Catalyst_2_Meraki_Config_Checker` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
-The bot functionality is based on the `webex_bot` project by [Finbarr Brady](https://github.com/fbradyirl).
+The bot functionality is using `webex_bot` by [Finbarr Brady](https://github.com/fbradyirl).
 
 
 # History
 
+## 0.2.6 (05-07-2024)
+
+  - Resolved Issue #6.
+  - Fixed issue with unclaiming switches before removing switch stack.
+  - Updated requirements.
+
 ## 0.2.5 (04-25-2024)
 
   - Reverted back to Finbarr Brady's webex-bot after a pull merge.
 
 ## 0.2.4 (04-12-2024)
 
   - Added Private VLAN -> Port Isolation to encyclopedia.
```

### Comparing `merakicat-0.2.5/src/merakicat.egg-info/SOURCES.txt` & `merakicat-0.2.6/src/merakicat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.5/tox.ini` & `merakicat-0.2.6/tox.ini`

 * *Files identical despite different names*

