# Comparing `tmp/itk_dev_shared_components-2.1.1.tar.gz` & `tmp/itk_dev_shared_components-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itk_dev_shared_components-2.1.1.tar", last modified: Mon Apr 15 09:33:16 2024, max compression
+gzip compressed data, was "itk_dev_shared_components-2.2.0.tar", last modified: Wed May  8 08:45:47 2024, max compression
```

## Comparing `itk_dev_shared_components-2.1.1.tar` & `itk_dev_shared_components-2.2.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.445789 itk_dev_shared_components-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-15 09:33:16.445789 itk_dev_shared_components-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.441789 itk_dev_shared_components-2.1.1/itk_dev_shared_components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.441789 itk_dev_shared_components-2.1.1/itk_dev_shared_components/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/graph/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/graph/mail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.441789 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/cpr.py
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.441789 itk_dev_shared_components-2.1.1/itk_dev_shared_components/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/misc/cpr_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.445789 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/fmcacov.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/gridview_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/multi_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/opret_kundekontakt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/sap_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/sap_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/tree_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.445789 itk_dev_shared_components-2.1.1/itk_dev_shared_components/smtp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/smtp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components/smtp/smtp_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:33:16.445789 itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-15 09:33:16.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-15 09:33:16.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:33:16.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 09:33:16.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 09:33:16.000000 itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-15 09:33:11.000000 itk_dev_shared_components-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:33:16.445789 itk_dev_shared_components-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:45:47.534627 itk_dev_shared_components-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-08 08:45:47.534627 itk_dev_shared_components-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:45:47.526627 itk_dev_shared_components-2.2.0/itk_dev_shared_components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:45:47.530627 itk_dev_shared_components-2.2.0/itk_dev_shared_components/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/graph/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/graph/mail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:45:47.530627 itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/cpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/nova_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/nova_documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/nova_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/nova_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/nova_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:45:47.530627 itk_dev_shared_components-2.2.0/itk_dev_shared_components/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/misc/cpr_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:45:47.530627 itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/fmcacov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/gridview_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/multi_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/opret_kundekontakt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/sap_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/sap_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/tree_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:45:47.534627 itk_dev_shared_components-2.2.0/itk_dev_shared_components/smtp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/smtp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components/smtp/smtp_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:45:47.534627 itk_dev_shared_components-2.2.0/itk_dev_shared_components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-08 08:45:47.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-08 08:45:47.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:45:47.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 08:45:47.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 08:45:47.000000 itk_dev_shared_components-2.2.0/itk_dev_shared_components.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-08 08:45:43.000000 itk_dev_shared_components-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:45:47.534627 itk_dev_shared_components-2.2.0/setup.cfg
```

### Comparing `itk_dev_shared_components-2.1.1/LICENSE` & `itk_dev_shared_components-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/PKG-INFO` & `itk_dev_shared_components-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itk_dev_shared_components
-Version: 2.1.1
+Version: 2.2.0
 Summary: Shared components to use in RPA projects
 Author-email: ITK Development <itk-rpa@mkb.aarhus.dk>
 Project-URL: Homepage, https://github.com/itk-dev-rpa/itk-dev-shared-components
 Project-URL: Bug Tracker, https://github.com/itk-dev-rpa/itk-dev-shared-components/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `itk_dev_shared_components-2.1.1/README.md` & `itk_dev_shared_components-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/graph/authentication.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/graph/authentication.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/graph/mail.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/graph/mail.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/authentication.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/authentication.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/cpr.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/cpr.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_cases.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/nova_cases.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_documents.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/nova_documents.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_objects.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/nova_objects.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/nova_tasks.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/nova_tasks.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/kmd_nova/util.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/kmd_nova/util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/misc/cpr_util.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/misc/cpr_util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/fmcacov.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/fmcacov.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/gridview_util.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/gridview_util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/multi_session.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/multi_session.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/opret_kundekontakt.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/opret_kundekontakt.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/sap_login.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/sap_login.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/sap_util.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/sap_util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/sap/tree_util.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/sap/tree_util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components/smtp/smtp_util.py` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components/smtp/smtp_util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/PKG-INFO` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itk_dev_shared_components
-Version: 2.1.1
+Version: 2.2.0
 Summary: Shared components to use in RPA projects
 Author-email: ITK Development <itk-rpa@mkb.aarhus.dk>
 Project-URL: Homepage, https://github.com/itk-dev-rpa/itk-dev-shared-components
 Project-URL: Bug Tracker, https://github.com/itk-dev-rpa/itk-dev-shared-components/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `itk_dev_shared_components-2.1.1/itk_dev_shared_components.egg-info/SOURCES.txt` & `itk_dev_shared_components-2.2.0/itk_dev_shared_components.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 itk_dev_shared_components/graph/authentication.py
 itk_dev_shared_components/graph/mail.py
 itk_dev_shared_components/kmd_nova/__init__.py
 itk_dev_shared_components/kmd_nova/authentication.py
 itk_dev_shared_components/kmd_nova/cpr.py
 itk_dev_shared_components/kmd_nova/nova_cases.py
 itk_dev_shared_components/kmd_nova/nova_documents.py
+itk_dev_shared_components/kmd_nova/nova_notes.py
 itk_dev_shared_components/kmd_nova/nova_objects.py
 itk_dev_shared_components/kmd_nova/nova_tasks.py
 itk_dev_shared_components/kmd_nova/util.py
 itk_dev_shared_components/misc/__init__.py
 itk_dev_shared_components/misc/cpr_util.py
 itk_dev_shared_components/sap/__init__.py
 itk_dev_shared_components/sap/fmcacov.py
```

### Comparing `itk_dev_shared_components-2.1.1/pyproject.toml` & `itk_dev_shared_components-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "itk_dev_shared_components"
-version = "2.1.1"
+version = "2.2.0"
 authors = [
   { name="ITK Development", email="itk-rpa@mkb.aarhus.dk" },
 ]
 description = "Shared components to use in RPA projects"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

