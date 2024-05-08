# Comparing `tmp/label-message-local-0.0.4.tar.gz` & `tmp/label_message_local-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "label-message-local-0.0.4.tar", last modified: Wed Jan 31 19:50:02 2024, max compression
+gzip compressed data, was "label_message_local-0.0.5.tar", last modified: Wed May  8 14:41:02 2024, max compression
```

## Comparing `label-message-local-0.0.4.tar` & `label_message_local-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:50:02.090424 label-message-local-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-01-31 19:50:02.090424 label-message-local-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 19:49:40.000000 label-message-local-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:50:02.090424 label-message-local-0.0.4/label_message_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:50:02.090424 label-message-local-0.0.4/label_message_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-31 19:49:40.000000 label-message-local-0.0.4/label_message_local/src/LabelConstants.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-01-31 19:49:40.000000 label-message-local-0.0.4/label_message_local/src/LabelMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 19:49:40.000000 label-message-local-0.0.4/label_message_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:50:02.090424 label-message-local-0.0.4/label_message_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-01-31 19:50:02.000000 label-message-local-0.0.4/label_message_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-01-31 19:50:02.000000 label-message-local-0.0.4/label_message_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 19:50:02.000000 label-message-local-0.0.4/label_message_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-31 19:50:02.000000 label-message-local-0.0.4/label_message_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-31 19:50:02.000000 label-message-local-0.0.4/label_message_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-31 19:49:40.000000 label-message-local-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 19:50:02.090424 label-message-local-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-31 19:49:40.000000 label-message-local-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:41:02.727966 label_message_local-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-08 14:41:02.723966 label_message_local-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:40:40.000000 label_message_local-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:41:02.723966 label_message_local-0.0.5/label_message_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:41:02.723966 label_message_local-0.0.5/label_message_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-08 14:40:40.000000 label_message_local-0.0.5/label_message_local/src/LabelConstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-08 14:40:40.000000 label_message_local-0.0.5/label_message_local/src/LabelMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:40:40.000000 label_message_local-0.0.5/label_message_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:41:02.723966 label_message_local-0.0.5/label_message_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-08 14:41:02.000000 label_message_local-0.0.5/label_message_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-08 14:41:02.000000 label_message_local-0.0.5/label_message_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:41:02.000000 label_message_local-0.0.5/label_message_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 14:41:02.000000 label_message_local-0.0.5/label_message_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-08 14:41:02.000000 label_message_local-0.0.5/label_message_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-08 14:40:40.000000 label_message_local-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:41:02.727966 label_message_local-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-08 14:40:40.000000 label_message_local-0.0.5/setup.py
```

### Comparing `label-message-local-0.0.4/PKG-INFO` & `label_message_local-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: label-message-local
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles label-message-local Python
 Home-page: https://github.com/circles-zone/label-message-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: logger-local
-Requires-Dist: database-mysql-local
+Requires-Dist: logger-local>=0.0.135
+Requires-Dist: database-mysql-local>=0.0.290
 
 PyPI Package for Circles label-message-local Python
```

### Comparing `label-message-local-0.0.4/label_message_local/src/LabelConstants.py` & `label_message_local-0.0.5/label_message_local/src/LabelConstants.py`

 * *Files identical despite different names*

### Comparing `label-message-local-0.0.4/label_message_local.egg-info/PKG-INFO` & `label_message_local-0.0.5/label_message_local.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: label-message-local
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles label-message-local Python
 Home-page: https://github.com/circles-zone/label-message-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: logger-local
-Requires-Dist: database-mysql-local
+Requires-Dist: logger-local>=0.0.135
+Requires-Dist: database-mysql-local>=0.0.290
 
 PyPI Package for Circles label-message-local Python
```

### Comparing `label-message-local-0.0.4/pyproject.toml` & `label_message_local-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `label-message-local-0.0.4/setup.py` & `label_message_local-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "label-message-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
-    name=PACKAGE_NAME,
-    version='0.0.4',
+    name=PACKAGE_NAME,  # https://pypi.org/project/label-message-local/
+    version='0.0.5',
     author="Circles",
     author_email="info@circlez.ai",
     description=f"PyPI Package for Circles {PACKAGE_NAME} Python",
     long_description=f"PyPI Package for Circles {PACKAGE_NAME} Python",
     long_description_content_type='text/markdown',
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     # packages=setuptools.find_packages(),
@@ -18,11 +18,11 @@
     package_data={package_dir: ['*.py']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        "logger-local",
-        "database-mysql-local"
+        "logger-local>=0.0.135",
+        "database-mysql-local>=0.0.290",
     ],
 )
```

