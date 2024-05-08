# Comparing `tmp/casaconfig-0.0.91.tar.gz` & `tmp/casaconfig-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casaconfig-0.0.91.tar", last modified: Thu Apr 18 19:17:58 2024, max compression
+gzip compressed data, was "casaconfig-1.0.0.tar", last modified: Wed May  8 15:27:47 2024, max compression
```

## Comparing `casaconfig-0.0.91.tar` & `casaconfig-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:17:58.200832 casaconfig-0.0.91/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-18 19:17:53.000000 casaconfig-0.0.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:17:53.000000 casaconfig-0.0.91/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-18 19:17:58.200832 casaconfig-0.0.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-18 19:17:53.000000 casaconfig-0.0.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:17:58.192832 casaconfig-0.0.91/casaconfig/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:17:58.200832 casaconfig-0.0.91/casaconfig/private/
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/CasaconfigErrors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/casasiteconfig_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/config_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/config_defaults_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/data_available.py
--rw-r--r--   0 runner    (1001) docker     (127)    20623 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/data_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/do_auto_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/do_pull_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/get_argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/get_data_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/get_data_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/io_redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/measures_available.py
--rw-r--r--   0 runner    (1001) docker     (127)    20738 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/measures_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/print_log_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/pull_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/read_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/set_casacore_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-18 19:17:53.000000 casaconfig-0.0.91/casaconfig/private/update_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:17:58.196832 casaconfig-0.0.91/casaconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-18 19:17:57.000000 casaconfig-0.0.91/casaconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-18 19:17:58.000000 casaconfig-0.0.91/casaconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:17:57.000000 casaconfig-0.0.91/casaconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 19:17:57.000000 casaconfig-0.0.91/casaconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 19:17:57.000000 casaconfig-0.0.91/casaconfig.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:17:58.200832 casaconfig-0.0.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-18 19:17:55.000000 casaconfig-0.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:47.337514 casaconfig-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-08 15:27:40.000000 casaconfig-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:40.000000 casaconfig-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-08 15:27:47.337514 casaconfig-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-08 15:27:40.000000 casaconfig-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:47.333514 casaconfig-1.0.0/casaconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:47.337514 casaconfig-1.0.0/casaconfig/private/
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/CasaconfigErrors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/casasiteconfig_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/config_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/config_defaults_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/data_available.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20623 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/data_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/do_auto_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/do_pull_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/get_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/get_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/get_data_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/io_redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/measures_available.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20738 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/measures_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/print_log_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/pull_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/read_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/set_casacore_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-08 15:27:40.000000 casaconfig-1.0.0/casaconfig/private/update_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:47.333514 casaconfig-1.0.0/casaconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-08 15:27:47.000000 casaconfig-1.0.0/casaconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-08 15:27:47.000000 casaconfig-1.0.0/casaconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:27:47.000000 casaconfig-1.0.0/casaconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 15:27:47.000000 casaconfig-1.0.0/casaconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 15:27:47.000000 casaconfig-1.0.0/casaconfig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:27:47.337514 casaconfig-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-08 15:27:42.000000 casaconfig-1.0.0/setup.py
```

### Comparing `casaconfig-0.0.91/LICENSE` & `casaconfig-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/PKG-INFO` & `casaconfig-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casaconfig
-Version: 0.0.91
+Version: 1.0.0
 Summary: CASA Operational Configuration Package
 Home-page: https://github.com/casangi/casaconfig
 Author: National Radio Astronomy Observatory
 Author-email: casa-feedback@nrao.edu
 License: Apache-2.0
 Description: # casaconfig
         Runtime data necessary for CASA operation.
```

### Comparing `casaconfig-0.0.91/README.md` & `casaconfig-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/__init__.py` & `casaconfig-1.0.0/casaconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/__main__.py` & `casaconfig-1.0.0/casaconfig/__main__.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/config.py` & `casaconfig-1.0.0/casaconfig/config.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/CasaconfigErrors.py` & `casaconfig-1.0.0/casaconfig/private/CasaconfigErrors.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/casasiteconfig_example.py` & `casaconfig-1.0.0/casaconfig/private/casasiteconfig_example.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/config_defaults.py` & `casaconfig-1.0.0/casaconfig/private/config_defaults.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/config_defaults_static.py` & `casaconfig-1.0.0/casaconfig/private/config_defaults_static.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/data_available.py` & `casaconfig-1.0.0/casaconfig/private/data_available.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/data_update.py` & `casaconfig-1.0.0/casaconfig/private/data_update.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/do_auto_updates.py` & `casaconfig-1.0.0/casaconfig/private/do_auto_updates.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/do_pull_data.py` & `casaconfig-1.0.0/casaconfig/private/do_pull_data.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/get_argparser.py` & `casaconfig-1.0.0/casaconfig/private/get_argparser.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/get_config.py` & `casaconfig-1.0.0/casaconfig/private/get_config.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/get_data_info.py` & `casaconfig-1.0.0/casaconfig/private/get_data_info.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/get_data_lock.py` & `casaconfig-1.0.0/casaconfig/private/get_data_lock.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/io_redirect.py` & `casaconfig-1.0.0/casaconfig/private/io_redirect.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/measures_available.py` & `casaconfig-1.0.0/casaconfig/private/measures_available.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/measures_update.py` & `casaconfig-1.0.0/casaconfig/private/measures_update.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/print_log_messages.py` & `casaconfig-1.0.0/casaconfig/private/print_log_messages.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/pull_data.py` & `casaconfig-1.0.0/casaconfig/private/pull_data.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/read_readme.py` & `casaconfig-1.0.0/casaconfig/private/read_readme.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/set_casacore_path.py` & `casaconfig-1.0.0/casaconfig/private/set_casacore_path.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/summary.py` & `casaconfig-1.0.0/casaconfig/private/summary.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig/private/update_all.py` & `casaconfig-1.0.0/casaconfig/private/update_all.py`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/casaconfig.egg-info/PKG-INFO` & `casaconfig-1.0.0/casaconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casaconfig
-Version: 0.0.91
+Version: 1.0.0
 Summary: CASA Operational Configuration Package
 Home-page: https://github.com/casangi/casaconfig
 Author: National Radio Astronomy Observatory
 Author-email: casa-feedback@nrao.edu
 License: Apache-2.0
 Description: # casaconfig
         Runtime data necessary for CASA operation.
```

### Comparing `casaconfig-0.0.91/casaconfig.egg-info/SOURCES.txt` & `casaconfig-1.0.0/casaconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `casaconfig-0.0.91/setup.py` & `casaconfig-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from glob import glob
 
 with open('README.md', "r") as fid:   #encoding='utf-8'
     long_description = fid.read()
 
 setup(
     name='casaconfig',
-    version='0.0.91',
+    version='1.0.0',
     description='CASA Operational Configuration Package',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='National Radio Astronomy Observatory',
     author_email='casa-feedback@nrao.edu',
     url='https://github.com/casangi/casaconfig',
     license='Apache-2.0',
```

