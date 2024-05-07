# Comparing `tmp/ls_api_clients-0.14.0.tar.gz` & `tmp/ls_api_clients-0.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ls_api_clients-0.14.0.tar", last modified: Tue Apr 30 12:55:46 2024, max compression
+gzip compressed data, was "ls_api_clients-0.14.1.tar", last modified: Tue May  7 23:58:24 2024, max compression
```

## Comparing `ls_api_clients-0.14.0.tar` & `ls_api_clients-0.14.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 12:55:46.340902 ls_api_clients-0.14.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1077 2024-04-30 12:42:41.000000 ls_api_clients-0.14.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      720 2024-04-30 12:55:46.340902 ls_api_clients-0.14.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      111 2024-04-30 12:42:41.000000 ls_api_clients-0.14.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 12:55:46.340902 ls_api_clients-0.14.0/ls_api_clients/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       53 2024-04-30 12:42:41.000000 ls_api_clients-0.14.0/ls_api_clients/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10433 2024-04-30 12:42:41.000000 ls_api_clients-0.14.0/ls_api_clients/ls_api_client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 12:55:46.340902 ls_api_clients-0.14.0/ls_api_clients.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      720 2024-04-30 12:55:46.000000 ls_api_clients-0.14.0/ls_api_clients.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      280 2024-04-30 12:55:46.000000 ls_api_clients-0.14.0/ls_api_clients.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-30 12:55:46.000000 ls_api_clients-0.14.0/ls_api_clients.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      100 2024-04-30 12:55:46.000000 ls_api_clients-0.14.0/ls_api_clients.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2024-04-30 12:55:46.000000 ls_api_clients-0.14.0/ls_api_clients.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      695 2024-04-30 12:55:43.000000 ls_api_clients-0.14.0/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-30 12:55:46.340902 ls_api_clients-0.14.0/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:58:24.170688 ls_api_clients-0.14.1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-07 23:56:23.000000 ls_api_clients-0.14.1/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      732 2024-05-07 23:58:24.170688 ls_api_clients-0.14.1/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      111 2024-05-07 23:56:23.000000 ls_api_clients-0.14.1/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:58:24.166688 ls_api_clients-0.14.1/ls_api_clients/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       53 2024-05-07 23:56:23.000000 ls_api_clients-0.14.1/ls_api_clients/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10433 2024-05-07 23:56:23.000000 ls_api_clients-0.14.1/ls_api_clients/ls_api_client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:58:24.170688 ls_api_clients-0.14.1/ls_api_clients.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      732 2024-05-07 23:58:24.000000 ls_api_clients-0.14.1/ls_api_clients.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      280 2024-05-07 23:58:24.000000 ls_api_clients-0.14.1/ls_api_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-07 23:58:24.000000 ls_api_clients-0.14.1/ls_api_clients.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      100 2024-05-07 23:58:24.000000 ls_api_clients-0.14.1/ls_api_clients.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2024-05-07 23:58:24.000000 ls_api_clients-0.14.1/ls_api_clients.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      707 2024-05-07 23:58:21.000000 ls_api_clients-0.14.1/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-07 23:58:24.170688 ls_api_clients-0.14.1/setup.cfg
```

### Comparing `ls_api_clients-0.14.0/PKG-INFO` & `ls_api_clients-0.14.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ls-api-clients
-Version: 0.14.0
+Version: 0.14.1
 Summary: A package for laser-mind clients
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3==1.26.13
 Requires-Dist: requests>=2.23
 Requires-Dist: msgpack>=1.0.0
```

### Comparing `ls_api_clients-0.14.0/ls_api_clients/ls_api_client.py` & `ls_api_clients-0.14.1/ls_api_clients/ls_api_client.py`

 * *Files identical despite different names*

### Comparing `ls_api_clients-0.14.0/ls_api_clients.egg-info/PKG-INFO` & `ls_api_clients-0.14.1/ls_api_clients.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ls-api-clients
-Version: 0.14.0
+Version: 0.14.1
 Summary: A package for laser-mind clients
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3==1.26.13
 Requires-Dist: requests>=2.23
 Requires-Dist: msgpack>=1.0.0
```

### Comparing `ls_api_clients-0.14.0/pyproject.toml` & `ls_api_clients-0.14.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ls-api-clients"
-version = "0.14.0"
+version = "0.14.1"
 description = "A package for laser-mind clients"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [ "urllib3==1.26.13", "requests>=2.23", "msgpack>=1.0.0", "ls-cred-storage>=0.1.9", "laser-mind-client-meta>=0.0.9",]
-classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
+classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "Assaf Kalinski"
 email = "assaf@lightsolver.com"
 
 [project.urls]
 Homepage = "https://lightsolver.com"
```

