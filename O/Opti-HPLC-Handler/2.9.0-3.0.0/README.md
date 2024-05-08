# Comparing `tmp/opti_hplc_handler-2.9.0.tar.gz` & `tmp/opti_hplc_handler-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opti_hplc_handler-2.9.0.tar", last modified: Tue May  7 12:51:01 2024, max compression
+gzip compressed data, was "opti_hplc_handler-3.0.0.tar", last modified: Wed May  8 13:27:51 2024, max compression
```

## Comparing `opti_hplc_handler-2.9.0.tar` & `opti_hplc_handler-3.0.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:51:01.834134 opti_hplc_handler-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-05-07 12:51:01.834134 opti_hplc_handler-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-07 12:50:44.000000 opti_hplc_handler-2.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 12:51:01.834134 opti_hplc_handler-2.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:51:01.826134 opti_hplc_handler-2.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:51:01.826134 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 12:50:44.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:51:01.826134 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:51:01.826134 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/empower_implementation/
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/empower_implementation/empower_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/generate_basic_robustness_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:51:01.826134 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/method_generators/
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/method_generators/add_isocratic_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/method_generators/alter_strong_eluent_pct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/method_generators/alter_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/method_generators/condense_gradient_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/method_generators/ramp_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/revert_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/empower_api_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    17114 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/empower_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/empower_instrument_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    15927 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/empower_module_method.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:51:01.830134 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/utils/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/utils/validate_gradient_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/src/OptiHPLCHandler/utils/validate_method_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:51:01.830134 opti_hplc_handler-2.9.0/src/Opti_HPLC_Handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-05-07 12:51:01.000000 opti_hplc_handler-2.9.0/src/Opti_HPLC_Handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-07 12:51:01.000000 opti_hplc_handler-2.9.0/src/Opti_HPLC_Handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 12:51:01.000000 opti_hplc_handler-2.9.0/src/Opti_HPLC_Handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-07 12:51:01.000000 opti_hplc_handler-2.9.0/src/Opti_HPLC_Handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 12:51:01.000000 opti_hplc_handler-2.9.0/src/Opti_HPLC_Handler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:51:01.830134 opti_hplc_handler-2.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14613 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/tests/test_core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14293 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/tests/test_instrument_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    50054 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/tests/test_module_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    23590 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/tests/test_proxy_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-07 12:50:29.000000 opti_hplc_handler-2.9.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:27:51.523965 opti_hplc_handler-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-05-08 13:27:51.523965 opti_hplc_handler-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-08 13:27:37.000000 opti_hplc_handler-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:27:51.523965 opti_hplc_handler-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:27:51.515965 opti_hplc_handler-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:27:51.515965 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-08 13:27:37.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:27:51.515965 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:27:51.515965 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/empower_implementation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/empower_implementation/empower_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/generate_basic_robustness_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:27:51.519965 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/method_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/method_generators/add_isocratic_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/method_generators/alter_strong_eluent_pct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/method_generators/alter_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/method_generators/condense_gradient_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/method_generators/ramp_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/revert_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/empower_api_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17114 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/empower_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/empower_instrument_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15854 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/empower_module_method.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:27:51.519965 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/utils/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/utils/validate_gradient_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/src/OptiHPLCHandler/utils/validate_method_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:27:51.519965 opti_hplc_handler-3.0.0/src/Opti_HPLC_Handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-05-08 13:27:51.000000 opti_hplc_handler-3.0.0/src/Opti_HPLC_Handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-08 13:27:51.000000 opti_hplc_handler-3.0.0/src/Opti_HPLC_Handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:27:51.000000 opti_hplc_handler-3.0.0/src/Opti_HPLC_Handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-08 13:27:51.000000 opti_hplc_handler-3.0.0/src/Opti_HPLC_Handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 13:27:51.000000 opti_hplc_handler-3.0.0/src/Opti_HPLC_Handler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:27:51.519965 opti_hplc_handler-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14613 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/tests/test_core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/tests/test_instrument_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49127 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/tests/test_module_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23590 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/tests/test_proxy_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-08 13:27:28.000000 opti_hplc_handler-3.0.0/tests/test_utils.py
```

### Comparing `opti_hplc_handler-2.9.0/LICENSE` & `opti_hplc_handler-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/PKG-INFO` & `opti_hplc_handler-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Opti_HPLC_Handler
-Version: 2.9.0
+Version: 3.0.0
 Summary: Simplified proxy API for interacting with the Waters Empower Web API.
 Author-email: Søren Furbo <srfu@novonordisk.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, novonordisk-research
         
         Redistribution and use in source and binary forms, with or without
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Opti_HPLC_Handler Version: 2.9.0 Summary:
+Metadata-Version: 2.1 Name: Opti_HPLC_Handler Version: 3.0.0 Summary:
 Simplified proxy API for interacting with the Waters Empower Web API. Author-
 email: SÃ¸ren Furbo
 novonordisk.com> License: BSD 3-Clause License Copyright (c) 2023, novonordisk-
 research Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
```

### Comparing `opti_hplc_handler-2.9.0/README.md` & `opti_hplc_handler-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/pyproject.toml` & `opti_hplc_handler-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Opti_HPLC_Handler"
-version = "2.9.0"
+version = "3.0.0"
 description = "Simplified proxy API for interacting with the Waters Empower Web API."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
   { name="Søren Furbo", email="srfu@novonordisk.com" },
 ]
@@ -93,15 +93,15 @@
 
 [tool.pytest.ini_options]
 pythonpath = [
   "src"
 ]
 
 [tool.bumpver]
-current_version = "2.9.0"
+current_version = "3.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/__init__.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/empower_implementation/empower_tools.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/empower_implementation/empower_tools.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/generate_basic_robustness_methods.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/generate_basic_robustness_methods.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/method_generators/add_isocratic_segment.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/method_generators/add_isocratic_segment.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/method_generators/alter_strong_eluent_pct.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/method_generators/alter_strong_eluent_pct.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/method_generators/alter_temperature.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/method_generators/alter_temperature.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/method_generators/condense_gradient_table.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/method_generators/condense_gradient_table.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/method_generators/ramp_method.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/method_generators/ramp_method.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/applications/revert_method.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/applications/revert_method.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/empower_api_core.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/empower_api_core.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/empower_handler.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/empower_handler.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/empower_instrument_method.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/empower_instrument_method.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/empower_module_method.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/empower_module_method.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,26 +136,27 @@
                     "Replaced %s instances of %s with %s", num_replaced, original, new
                 )
         method["nativeXml"] = xml
         return method
 
     @staticmethod
     def _round(value: Union[str, float], decimal_digits: int = 3) -> str:
-        if isinstance(value, float):
-            rounded_value = f"{value:.{decimal_digits}f}"
-            if float(rounded_value) != value:
-                logger.warning(
-                    "Rounding %s to %s, as Empower only accepts %s decimal(s).",
-                    value,
-                    rounded_value,
-                    decimal_digits,
-                )  # No user warning, since it should only be accessed through the
-                # property methods, and it is described in the docstring.
-                return rounded_value
-        return str(value)
+        if value == "Initial":
+            return value
+        try:
+            value = float(value)
+        except ValueError:
+            raise ValueError(f"Could not convert {value} to a float.")
+        rounded_value = round(value, decimal_digits)
+        if rounded_value != float(value):
+            warnings.warn(
+                f"Rounding {value} to {rounded_value}, as Empower only "
+                f"accepts {decimal_digits} decimal(s)."
+            )
+        return str(rounded_value)
 
 
 class ColumnOvenMethod(EmpowerModuleMethod):
     """
     Class for module methods that have a column temperature.
 
     Attributes in addition to the ones from EmpowerModuleMethod:
```

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/utils/data_types.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/utils/data_types.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/utils/validate_gradient_table.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/utils/validate_gradient_table.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/src/OptiHPLCHandler/utils/validate_method_name.py` & `opti_hplc_handler-3.0.0/src/OptiHPLCHandler/utils/validate_method_name.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/src/Opti_HPLC_Handler.egg-info/PKG-INFO` & `opti_hplc_handler-3.0.0/src/Opti_HPLC_Handler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Opti_HPLC_Handler
-Version: 2.9.0
+Version: 3.0.0
 Summary: Simplified proxy API for interacting with the Waters Empower Web API.
 Author-email: Søren Furbo <srfu@novonordisk.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, novonordisk-research
         
         Redistribution and use in source and binary forms, with or without
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Opti_HPLC_Handler Version: 2.9.0 Summary:
+Metadata-Version: 2.1 Name: Opti_HPLC_Handler Version: 3.0.0 Summary:
 Simplified proxy API for interacting with the Waters Empower Web API. Author-
 email: SÃ¸ren Furbo
 novonordisk.com> License: BSD 3-Clause License Copyright (c) 2023, novonordisk-
 research Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
```

### Comparing `opti_hplc_handler-2.9.0/src/Opti_HPLC_Handler.egg-info/SOURCES.txt` & `opti_hplc_handler-3.0.0/src/Opti_HPLC_Handler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/tests/test_core_api.py` & `opti_hplc_handler-3.0.0/tests/test_core_api.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/tests/test_instrument_method.py` & `opti_hplc_handler-3.0.0/tests/test_instrument_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,18 +97,18 @@
         method = EmpowerInstrumentMethod(method_definition)
         original_column_temperature = method.column_oven_method_list[
             0
         ].column_temperature
         method.column_oven_method_list[0].column_temperature = "50.03"
         assert isinstance(method.current_method, dict)
         assert method.current_method != method_definition["results"][0]
-        assert method.current_method["modules"][-1]["nativeXml"].count("50.03") == 1
+        assert method.current_method["modules"][-1]["nativeXml"].count("50.0") == 1
         assert (
             method.current_method["modules"][-1]["nativeXml"].replace(
-                "50.03", original_column_temperature
+                "50.0", original_column_temperature
             )
             == method_definition["results"][0]["modules"][-1]["nativeXml"]
         )
         assert method.original_method == method_definition["results"][0]
 
 
 class TestColumnTemperature(unittest.TestCase):
@@ -140,26 +140,26 @@
         method.column_oven_method_list[0].column_temperature = "50.03"
         with self.assertRaises(ValueError):
             method.column_temperature
 
     def test_set(self):
         method_definition = self.column_manager_example
         method = EmpowerInstrumentMethod(method_definition)
-        new_temperature = "50.03"
+        new_temperature = "50.0"
         method.column_temperature = new_temperature
         assert method.column_temperature == new_temperature
         assert method.column_oven_method_list[0].column_temperature == new_temperature
 
     def test_set_multiple(self):
         method_definition = self.column_manager_example["results"][0]
         method_definition["modules"].append(method_definition["modules"][-1])
         method = EmpowerInstrumentMethod(method_definition)
         method.column_oven_method_list[0].column_temperature = "5"
-        method.column_temperature = "50.03"
-        assert method.column_temperature == "50.03"
+        method.column_temperature = "50.0"
+        assert method.column_temperature == "50.0"
 
     def test_set_none(self):
         method_definition = self.column_manager_example["results"][0]
         method_definition["modules"] = method_definition["modules"][0:-1]
         method = EmpowerInstrumentMethod(method_definition)
         with self.assertRaises(ValueError):
             method.column_temperature = "50.03"
@@ -177,17 +177,17 @@
                     "nativeXml": "<SetColumnTemperature>45.0</SetColumnTemperature>",
                 },
             ],
         }
         method = EmpowerInstrumentMethod(minimal_definition)
         assert method.column_temperature == "45.0"
         method.column_temperature = "50.03"
-        assert method.column_temperature == "50.03"
+        assert method.column_temperature == "50.0"
         assert method.module_method_list[0].column_temperature == "43.0"
-        assert method.module_method_list[1].column_temperature == "50.03"
+        assert method.module_method_list[1].column_temperature == "50.0"
 
     def test_setting_multiple(self):
         minimal_definition = {
             "methodName": "test_method",
             "modules": [
                 {
                     "name": "rAcquityFTN",
@@ -201,17 +201,17 @@
         }
         method = EmpowerInstrumentMethod(
             minimal_definition, use_sample_manager_oven=True
         )
         with self.assertRaises(ValueError):
             method.column_temperature
         method.column_temperature = "50.03"
-        assert method.column_temperature == "50.03"
-        assert method.module_method_list[0].column_temperature == "50.03"
-        assert method.module_method_list[1].column_temperature == "50.03"
+        assert method.column_temperature == "50.0"
+        assert method.module_method_list[0].column_temperature == "50.0"
+        assert method.module_method_list[1].column_temperature == "50.0"
 
 
 class TestSolventManager(unittest.TestCase):
     def setUp(self) -> None:
         self.example = get_example_file_dict()
         self.bsm_example = self.example["response-BSM-PDA-Acq.json"]
         self.method = EmpowerInstrumentMethod(self.bsm_example)
```

### Comparing `opti_hplc_handler-2.9.0/tests/test_module_method.py` & `opti_hplc_handler-3.0.0/tests/test_module_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,22 +484,22 @@
                 "CompositionC": "0.0",
                 "CompositionD": "10.0",
                 "Curve": "10",
             },
         ]
         assert len(module_method.gradient_table) == 2
         assert module_method.gradient_table[0]["Time"] == "Initial"
-        assert module_method.gradient_table[0]["Flow"] == "0.500"
+        assert module_method.gradient_table[0]["Flow"] == "0.5"
         assert module_method.gradient_table[0]["CompositionA"] == "70.0"
         assert module_method.gradient_table[0]["CompositionB"] == "10.0"
         assert module_method.gradient_table[0]["CompositionC"] == "10.0"
         assert module_method.gradient_table[0]["CompositionD"] == "10.0"
         assert str(module_method.gradient_table[0]["Curve"]) == "Initial"
-        assert module_method.gradient_table[1]["Time"] == "10.00"
-        assert module_method.gradient_table[1]["Flow"] == "0.600"
+        assert module_method.gradient_table[1]["Time"] == "10.0"
+        assert module_method.gradient_table[1]["Flow"] == "0.6"
         assert module_method.gradient_table[1]["CompositionA"] == "10.0"
         assert module_method.gradient_table[1]["CompositionB"] == "80.0"
         assert module_method.gradient_table[1]["CompositionC"] == "0.0"
         assert module_method.gradient_table[1]["CompositionD"] == "10.0"
         assert str(module_method.gradient_table[1]["Curve"]) == "10"
 
     def test_gradient_xml_setter(self):
@@ -523,49 +523,14 @@
                 "CompositionD": "10.0",
                 "Curve": "10",
             },
         ]
         new_method = QSMMethod(module_method.current_method)
         assert new_method.gradient_table == module_method.gradient_table
 
-    def test_floats_and_strings(self):
-        module_method = QSMMethod(self.minimal_definition)
-        module_method.gradient_table = [
-            {
-                "Time": "Initial",
-                "Flow": 1,
-                "CompositionA": 40,
-                "CompositionB": 40,
-                "CompositionC": 10,
-                "CompositionD": 10,
-                "Curve": "Initial",
-            },
-        ]
-        assert float(module_method.gradient_table[0]["Flow"]) == 1.0
-        assert float(module_method.gradient_table[0]["CompositionA"]) == 40.0
-        assert float(module_method.gradient_table[0]["CompositionB"]) == 40.0
-        assert float(module_method.gradient_table[0]["CompositionC"]) == 10.0
-        assert float(module_method.gradient_table[0]["CompositionD"]) == 10.0
-        module_method.gradient_table = [
-            {
-                "Time": "Initial",
-                "Flow": "0.5",
-                "CompositionA": "30.0",
-                "CompositionB": "30.0",
-                "CompositionC": "30.0",
-                "CompositionD": "10.0",
-                "Curve": "Initial",
-            },
-        ]
-        assert module_method.gradient_table[0]["Flow"] == "0.5"
-        assert module_method.gradient_table[0]["CompositionA"] == "30.0"
-        assert module_method.gradient_table[0]["CompositionB"] == "30.0"
-        assert module_method.gradient_table[0]["CompositionC"] == "30.0"
-        assert module_method.gradient_table[0]["CompositionD"] == "10.0"
-
     def test_rounding_floats(self):
         # Empower gives the wrong numbers if more than 10 decimals are given for
         # parameters in the gradient table. This test checks that the numbers are
         # rounded to 3 decimals before being sent to Empower.
         # Consider adding test for 3*1/3 = 1
         module_method = QSMMethod(self.minimal_definition)
         module_method.gradient_table = [
@@ -586,70 +551,94 @@
                 "CompositionC": 0,
                 "CompositionD": 2 / 3,
                 "Curve": 6,
             },
         ]
         assert module_method.gradient_table[0]["Flow"] == "0.333"
         assert module_method.gradient_table[0]["CompositionA"] == "0.667"
-        assert module_method.gradient_table[0]["CompositionB"] == "0"
+        assert module_method.gradient_table[0]["CompositionB"] == "0.0"
         assert module_method.gradient_table[0]["CompositionC"] == "0.333"
-        assert module_method.gradient_table[0]["CompositionD"] == "0"
+        assert module_method.gradient_table[0]["CompositionD"] == "0.0"
         assert module_method.gradient_table[1]["Time"] == "0.333"
         assert module_method.gradient_table[1]["Flow"] == "0.333"
         assert module_method.gradient_table[1]["CompositionA"] == "0.333"
-        assert module_method.gradient_table[1]["CompositionB"] == "0"
-        assert module_method.gradient_table[1]["CompositionC"] == "0"
+        assert module_method.gradient_table[1]["CompositionB"] == "0.0"
+        assert module_method.gradient_table[1]["CompositionC"] == "0.0"
         assert module_method.gradient_table[1]["CompositionD"] == "0.667"
-        assert (
-            "0.3333" not in module_method.current_method
-        )  # If values are given as strings, EmpowerHandler should not round them
+        assert "0.3333" not in module_method.current_method
+
+    def test_rounding_strings(self):
+        # If values are given as strings, EmpowerHandler should also round them
+        module_method = QSMMethod(self.minimal_definition)
+        module_method.gradient_table = [
+            {
+                "Time": "Initial",
+                "Flow": "0.33333",
+                "CompositionA": "0.66667",
+                "CompositionB": "0",
+                "CompositionC": "0",
+                "CompositionD": "0.33333",
+                "Curve": "Initial",
+            },
+            {
+                "Time": "0.33333333",  # 8 decimals should give a warning
+                "Flow": "0.33333",
+                "CompositionA": "0.33333",
+                "CompositionB": "0.0",
+                "CompositionC": "0.66667",
+                "CompositionD": "0",
+                "Curve": "6",
+            },
+        ]
+        assert module_method.gradient_table[0]["Flow"] == "0.333"
+        assert module_method.gradient_table[0]["CompositionA"] == "0.667"
+        assert module_method.gradient_table[0]["CompositionB"] == "0.0"
+        assert module_method.gradient_table[0]["CompositionC"] == "0.0"
+        assert module_method.gradient_table[0]["CompositionD"] == "0.333"
+        assert module_method.gradient_table[1]["Time"] == "0.333"
+        assert module_method.gradient_table[1]["Flow"] == "0.333"
+        assert module_method.gradient_table[1]["CompositionA"] == "0.333"
+        assert module_method.gradient_table[1]["CompositionB"] == "0.0"
+        assert module_method.gradient_table[1]["CompositionC"] == "0.667"
+        assert module_method.gradient_table[1]["CompositionD"] == "0.0"
+        assert "0.3333" not in module_method.current_method["nativeXml"]
+
+    def test_round_warning(self):
         module_method = QSMMethod(self.minimal_definition)
         with self.assertWarns(UserWarning):
             module_method.gradient_table = [
                 {
                     "Time": "Initial",
-                    "Flow": "0.33333",  # No rounding, since this is a string
-                    "CompositionA": 0.66667,  # Rounding, since this is a float
+                    "Flow": "0.33333",
+                    "CompositionA": "0.66667",
                     "CompositionB": "0",
                     "CompositionC": "0",
                     "CompositionD": "0.33333",
                     "Curve": "Initial",
                 },
                 {
                     "Time": "0.33333333",  # 8 decimals should give a warning
                     "Flow": "0.33333",
                     "CompositionA": "0.33333",
-                    "CompositionB": "0",
+                    "CompositionB": "0.0",
                     "CompositionC": "0.66667",
                     "CompositionD": "0",
-                    "Curve": 6,
+                    "Curve": "6",
                 },
             ]
-        assert module_method.gradient_table[0]["Flow"] == "0.33333"
-        assert module_method.gradient_table[0]["CompositionA"] == "0.667"
-        assert module_method.gradient_table[0]["CompositionB"] == "0"
-        assert module_method.gradient_table[0]["CompositionC"] == "0"
-        assert module_method.gradient_table[0]["CompositionD"] == "0.33333"
-        assert module_method.gradient_table[1]["Time"] == "0.33333333"
-        assert module_method.gradient_table[1]["Flow"] == "0.33333"
-        assert module_method.gradient_table[1]["CompositionA"] == "0.33333"
-        assert module_method.gradient_table[1]["CompositionB"] == "0"
-        assert module_method.gradient_table[1]["CompositionC"] == "0.66667"
-        assert module_method.gradient_table[1]["CompositionD"] == "0"
-        assert "0.3333" in module_method.current_method["nativeXml"]
 
     def test_manually_than_gradient_table_changed(self):
         # Checks that manual changes in the gradient table does not proclude the use
         # of the gradient_table setter.
         module_method = QSMMethod(self.minimal_definition)
         module_method.replace("<Flow>0.600</Flow>", "<Flow>0.010</Flow>")
         new_gradient_table = [
             {
                 "Time": "Initial",
-                "Flow": "0.500",
+                "Flow": "0.5",
                 "CompositionA": "50.0",
                 "CompositionB": "0.0",
                 "CompositionC": "50.0",
                 "CompositionD": "0.0",
                 "Curve": "Initial",
             },
         ]
@@ -666,15 +655,17 @@
                 "CompositionB": "0.0",
                 "CompositionC": "50.0",
                 "CompositionD": "0.0",
                 "Curve": "Initial",
             },
         ]
         module_method.gradient_table = new_gradient_table
-        module_method.replace("<Flow>0.500</Flow>", "<Flow>0.010</Flow>")
+        # code converts to a float to round and then back to a string thus
+        # 0.500 becomes 0.5
+        module_method.replace("<Flow>0.5</Flow>", "<Flow>0.010</Flow>")
         assert module_method.gradient_table[0]["Flow"] == "0.010"
 
     def test_gradient_table_float(self):
         module_method = QSMMethod(self.minimal_definition)
         new_gradient_table = [
             {
                 "Time": "Initial",
@@ -898,15 +889,15 @@
                 "CompositionA": "50.0",
                 "CompositionB": "50.0",
                 "Curve": "Initial",
             }
         ]
         assert len(module_method.gradient_table) == 1
         assert module_method.gradient_table[0]["Time"] == "Initial"
-        assert module_method.gradient_table[0]["Flow"] == "0.500"
+        assert module_method.gradient_table[0]["Flow"] == "0.5"
         assert module_method.gradient_table[0]["CompositionA"] == "50.0"
         assert module_method.gradient_table[0]["CompositionB"] == "50.0"
         assert str(module_method.gradient_table[0]["Curve"]) == "Initial"
 
     def test_gradient_table_setter_default(self):
         module_method = BSMMethod(self.minimal_definition)
         module_method.gradient_table = [
@@ -942,20 +933,20 @@
                 "CompositionA": "20.0",
                 "CompositionB": "80.0",
                 "Curve": "10",
             },
         ]
         assert len(module_method.gradient_table) == 2
         assert module_method.gradient_table[0]["Time"] == "Initial"
-        assert module_method.gradient_table[0]["Flow"] == "0.500"
+        assert module_method.gradient_table[0]["Flow"] == "0.5"
         assert module_method.gradient_table[0]["CompositionA"] == "70.0"
         assert module_method.gradient_table[0]["CompositionB"] == "30.0"
         assert str(module_method.gradient_table[0]["Curve"]) == "Initial"
-        assert module_method.gradient_table[1]["Time"] == "10.00"
-        assert module_method.gradient_table[1]["Flow"] == "0.600"
+        assert module_method.gradient_table[1]["Time"] == "10.0"
+        assert module_method.gradient_table[1]["Flow"] == "0.6"
         assert module_method.gradient_table[1]["CompositionA"] == "20.0"
         assert module_method.gradient_table[1]["CompositionB"] == "80.0"
         assert str(module_method.gradient_table[1]["Curve"]) == "10"
 
     def test_gradient_xml_setter(self):
         module_method = BSMMethod(self.minimal_definition)
         module_method.gradient_table = [
@@ -1028,74 +1019,71 @@
         assert module_method.gradient_table[0]["Flow"] == "0.333"
         assert module_method.gradient_table[0]["CompositionA"] == "0.667"
         assert module_method.gradient_table[0]["CompositionB"] == "0.333"
         assert module_method.gradient_table[1]["Time"] == "0.333"
         assert module_method.gradient_table[1]["Flow"] == "0.333"
         assert module_method.gradient_table[1]["CompositionA"] == "0.333"
         assert module_method.gradient_table[1]["CompositionB"] == "0.667"
-        assert (
-            "0.3333" not in module_method.current_method
-        )  # If values are given as strings, EmpowerHandler should not round them
+        assert "0.3333" not in module_method.current_method
         module_method = BSMMethod(self.minimal_definition)
-        with self.assertWarns(UserWarning):
-            module_method.gradient_table = [
-                {
-                    "Time": "Initial",
-                    "Flow": "0.33333",  # No rounding, since this is a string
-                    "CompositionA": 0.66667,  # Rounding, since this is a float
-                    "CompositionB": "0.33333",
-                    "Curve": "Initial",
-                },
-                {
-                    "Time": "0.33333333",  # 8 decimals should give a warning
-                    "Flow": "0.33333",
-                    "CompositionA": "0.33333",
-                    "CompositionB": "0.66667",
-                    "Curve": 6,
-                },
-            ]
-        assert module_method.gradient_table[0]["Flow"] == "0.33333"
+        module_method.gradient_table = [
+            {
+                "Time": "Initial",
+                "Flow": "0.333",  # No rounding, since this is a string
+                "CompositionA": 0.667,  # Rounding, since this is a float
+                "CompositionB": "0.333",
+                "Curve": "Initial",
+            },
+            {
+                "Time": "0.333",  # 8 decimals should give a warning
+                "Flow": "0.333",
+                "CompositionA": "0.333",
+                "CompositionB": "0.667",
+                "Curve": 6,
+            },
+        ]
+        assert module_method.gradient_table[0]["Flow"] == "0.333"
         assert module_method.gradient_table[0]["CompositionA"] == "0.667"
-        assert module_method.gradient_table[0]["CompositionB"] == "0.33333"
-        assert module_method.gradient_table[1]["Time"] == "0.33333333"
-        assert module_method.gradient_table[1]["Flow"] == "0.33333"
-        assert module_method.gradient_table[1]["CompositionA"] == "0.33333"
-        assert module_method.gradient_table[1]["CompositionB"] == "0.66667"
-        assert "0.3333" in module_method.current_method["nativeXml"]
+        assert module_method.gradient_table[0]["CompositionB"] == "0.333"
+        assert module_method.gradient_table[1]["Time"] == "0.333"
+        assert module_method.gradient_table[1]["Flow"] == "0.333"
+        assert module_method.gradient_table[1]["CompositionA"] == "0.333"
+        assert module_method.gradient_table[1]["CompositionB"] == "0.667"
+        assert "0.333" in module_method.current_method["nativeXml"]
 
     def test_manually_than_gradient_table_changed(self):
         # Checks that manual changes in the gradient table does not proclude the use
         # of the gradient_table setter.
         module_method = BSMMethod(self.minimal_definition)
         module_method.replace("<Flow>0.600</Flow>", "<Flow>0.010</Flow>")
         new_gradient_table = [
             {
                 "Time": "Initial",
-                "Flow": "0.500",
+                "Flow": "0.5",
                 "CompositionA": "50.0",
                 "CompositionB": "50.0",
                 "Curve": "Initial",
             },
         ]
         module_method.gradient_table = new_gradient_table
         assert module_method.gradient_table == new_gradient_table
 
     def test_gradient_table_then_manual(self):
         module_method = BSMMethod(self.minimal_definition)
         new_gradient_table = [
             {
                 "Time": "Initial",
-                "Flow": "0.500",
+                "Flow": "0.5",
                 "CompositionA": "50.0",
                 "CompositionB": "50.0",
                 "Curve": "Initial",
             },
         ]
         module_method.gradient_table = new_gradient_table
-        module_method.replace("<Flow>0.500</Flow>", "<Flow>0.010</Flow>")
+        module_method.replace("<Flow>0.5</Flow>", "<Flow>0.010</Flow>")
         assert module_method.gradient_table[0]["Flow"] == "0.010"
 
     def test_gradient_table_float(self):
         module_method = BSMMethod(self.minimal_definition)
         new_gradient_table = [
             {
                 "Time": "Initial",
```

### Comparing `opti_hplc_handler-2.9.0/tests/test_proxy_api.py` & `opti_hplc_handler-3.0.0/tests/test_proxy_api.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.9.0/tests/test_utils.py` & `opti_hplc_handler-3.0.0/tests/test_utils.py`

 * *Files identical despite different names*

