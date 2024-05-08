# Comparing `tmp/olx-api-wrapper-0.3.0.tar.gz` & `tmp/olx-api-wrapper-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olx-api-wrapper-0.3.0.tar", last modified: Wed May  8 15:55:14 2024, max compression
+gzip compressed data, was "olx-api-wrapper-0.3.1.tar", last modified: Wed May  8 16:24:43 2024, max compression
```

## Comparing `olx-api-wrapper-0.3.0.tar` & `olx-api-wrapper-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:14.036358 olx-api-wrapper-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 15:55:06.000000 olx-api-wrapper-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-08 15:55:14.036358 olx-api-wrapper-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-05-08 15:55:06.000000 olx-api-wrapper-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:14.036358 olx-api-wrapper-0.3.0/olx/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-08 15:55:06.000000 olx-api-wrapper-0.3.0/olx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:14.036358 olx-api-wrapper-0.3.0/olx_api_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-08 15:55:13.000000 olx-api-wrapper-0.3.0/olx_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-08 15:55:14.000000 olx-api-wrapper-0.3.0/olx_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:55:13.000000 olx-api-wrapper-0.3.0/olx_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 15:55:13.000000 olx-api-wrapper-0.3.0/olx_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 15:55:13.000000 olx-api-wrapper-0.3.0/olx_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:55:14.036358 olx-api-wrapper-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-08 15:55:06.000000 olx-api-wrapper-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:24:43.906155 olx-api-wrapper-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 16:24:31.000000 olx-api-wrapper-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-08 16:24:43.906155 olx-api-wrapper-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-05-08 16:24:31.000000 olx-api-wrapper-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:24:43.906155 olx-api-wrapper-0.3.1/olx/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-08 16:24:31.000000 olx-api-wrapper-0.3.1/olx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:24:43.906155 olx-api-wrapper-0.3.1/olx_api_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-08 16:24:43.000000 olx-api-wrapper-0.3.1/olx_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-08 16:24:43.000000 olx-api-wrapper-0.3.1/olx_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:24:43.000000 olx-api-wrapper-0.3.1/olx_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 16:24:43.000000 olx-api-wrapper-0.3.1/olx_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 16:24:43.000000 olx-api-wrapper-0.3.1/olx_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:24:43.906155 olx-api-wrapper-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-08 16:24:31.000000 olx-api-wrapper-0.3.1/setup.py
```

### Comparing `olx-api-wrapper-0.3.0/LICENSE` & `olx-api-wrapper-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.0/PKG-INFO` & `olx-api-wrapper-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olx-api-wrapper
-Version: 0.3.0
+Version: 0.3.1
 Summary: Unofficial Wrapper for OLX API
 Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: Paweł Stawikowski
 Author-email: pawikoski@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.0 Summary: Unofficial
+Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.1 Summary: Unofficial
 Wrapper for OLX API Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: PaweÅ Stawikowski Author-email: pawikoski@gmail.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
```

### Comparing `olx-api-wrapper-0.3.0/README.md` & `olx-api-wrapper-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.0/olx_api_wrapper.egg-info/PKG-INFO` & `olx-api-wrapper-0.3.1/olx_api_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olx-api-wrapper
-Version: 0.3.0
+Version: 0.3.1
 Summary: Unofficial Wrapper for OLX API
 Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: Paweł Stawikowski
 Author-email: pawikoski@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.0 Summary: Unofficial
+Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.1 Summary: Unofficial
 Wrapper for OLX API Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: PaweÅ Stawikowski Author-email: pawikoski@gmail.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
```

### Comparing `olx-api-wrapper-0.3.0/setup.py` & `olx-api-wrapper-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="olx-api-wrapper",
-    version="0.3.0",
+    version="0.3.1",
     description="Unofficial Wrapper for OLX API",
     author="Paweł Stawikowski",
     author_email="pawikoski@gmail.com",
     packages=["olx"],
     url="https://github.com/Pawikoski/olx-api-wrapper",
     install_requires=["requests", "dacite"],
     long_description=long_description,
```

