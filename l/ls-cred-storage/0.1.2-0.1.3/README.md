# Comparing `tmp/ls_cred_storage-0.1.2.tar.gz` & `tmp/ls_cred_storage-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ls_cred_storage-0.1.2.tar", last modified: Thu May  2 09:44:58 2024, max compression
+gzip compressed data, was "ls_cred_storage-0.1.3.tar", last modified: Tue May  7 23:58:54 2024, max compression
```

## Comparing `ls_cred_storage-0.1.2.tar` & `ls_cred_storage-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 09:44:58.360745 ls_cred_storage-0.1.2/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2024-05-02 09:44:35.000000 ls_cred_storage-0.1.2/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-05-02 09:44:58.360745 ls_cred_storage-0.1.2/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2024-05-02 09:33:45.000000 ls_cred_storage-0.1.2/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 09:44:58.360745 ls_cred_storage-0.1.2/ls_cred_storage/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-02 09:33:45.000000 ls_cred_storage-0.1.2/ls_cred_storage/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1983 2024-05-02 09:33:45.000000 ls_cred_storage-0.1.2/ls_cred_storage/ls_cred_storage.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 09:44:58.360745 ls_cred_storage-0.1.2/ls_cred_storage.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-05-02 09:44:58.000000 ls_cred_storage-0.1.2/ls_cred_storage.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      289 2024-05-02 09:44:58.000000 ls_cred_storage-0.1.2/ls_cred_storage.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-02 09:44:58.000000 ls_cred_storage-0.1.2/ls_cred_storage.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-02 09:44:58.000000 ls_cred_storage-0.1.2/ls_cred_storage.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-02 09:44:58.000000 ls_cred_storage-0.1.2/ls_cred_storage.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      628 2024-05-02 09:44:55.000000 ls_cred_storage-0.1.2/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-02 09:44:58.360745 ls_cred_storage-0.1.2/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:58:54.642895 ls_cred_storage-0.1.3/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-07 23:56:36.000000 ls_cred_storage-0.1.3/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-05-07 23:58:54.642895 ls_cred_storage-0.1.3/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2024-05-07 23:56:36.000000 ls_cred_storage-0.1.3/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:58:54.642895 ls_cred_storage-0.1.3/ls_cred_storage/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-07 23:56:36.000000 ls_cred_storage-0.1.3/ls_cred_storage/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1983 2024-05-07 23:56:36.000000 ls_cred_storage-0.1.3/ls_cred_storage/ls_cred_storage.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:58:54.642895 ls_cred_storage-0.1.3/ls_cred_storage.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-05-07 23:58:54.000000 ls_cred_storage-0.1.3/ls_cred_storage.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      289 2024-05-07 23:58:54.000000 ls_cred_storage-0.1.3/ls_cred_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-07 23:58:54.000000 ls_cred_storage-0.1.3/ls_cred_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-07 23:58:54.000000 ls_cred_storage-0.1.3/ls_cred_storage.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-07 23:58:54.000000 ls_cred_storage-0.1.3/ls_cred_storage.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      628 2024-05-07 23:58:51.000000 ls_cred_storage-0.1.3/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-07 23:58:54.642895 ls_cred_storage-0.1.3/setup.cfg
```

### Comparing `ls_cred_storage-0.1.2/LICENSE` & `ls_cred_storage-0.1.3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2024 LightSolver Internal
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ls_cred_storage-0.1.2/PKG-INFO` & `ls_cred_storage-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ls-cred-storage
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package containing storage user credential
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://dev.lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ls_cred_storage-0.1.2/ls_cred_storage/ls_cred_storage.py` & `ls_cred_storage-0.1.3/ls_cred_storage/ls_cred_storage.py`

 * *Files identical despite different names*

### Comparing `ls_cred_storage-0.1.2/ls_cred_storage.egg-info/PKG-INFO` & `ls_cred_storage-0.1.3/ls_cred_storage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ls-cred-storage
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package containing storage user credential
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://dev.lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ls_cred_storage-0.1.2/pyproject.toml` & `ls_cred_storage-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ls-cred-storage"
-version = "0.1.2"
+version = "0.1.3"
 description = "A package containing storage user credential"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [ "keyring>=23.2.1",]
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "Assaf Kalinski"
```

