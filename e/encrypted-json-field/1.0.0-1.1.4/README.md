# Comparing `tmp/encrypted-json-field-1.0.0.tar.gz` & `tmp/encrypted_json_field-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encrypted-json-field-1.0.0.tar", last modified: Sun Aug  6 15:56:19 2023, max compression
+gzip compressed data, was "encrypted_json_field-1.1.4.tar", last modified: Wed May  8 18:39:14 2024, max compression
```

## Comparing `encrypted-json-field-1.0.0.tar` & `encrypted_json_field-1.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 el        (1000) el        (1000)        0 2023-08-06 15:56:19.975442 encrypted-json-field-1.0.0/
--rw-r--r--   0 el        (1000) el        (1000)     1778 2023-08-06 15:56:19.975442 encrypted-json-field-1.0.0/PKG-INFO
--rw-r--r--   0 el        (1000) el        (1000)      856 2023-08-06 15:35:49.000000 encrypted-json-field-1.0.0/README.md
-drwxr-xr-x   0 el        (1000) el        (1000)        0 2023-08-06 15:56:19.975442 encrypted-json-field-1.0.0/encrypted_json_field/
--rw-r--r--   0 el        (1000) el        (1000)     2632 2023-08-06 15:32:27.000000 encrypted-json-field-1.0.0/encrypted_json_field/__init__.py
--rw-r--r--   0 el        (1000) el        (1000)     1354 2023-08-06 15:35:59.000000 encrypted-json-field-1.0.0/encrypted_json_field/mixins.py
-drwxr-xr-x   0 el        (1000) el        (1000)        0 2023-08-06 15:56:19.975442 encrypted-json-field-1.0.0/encrypted_json_field.egg-info/
--rw-r--r--   0 el        (1000) el        (1000)     1778 2023-08-06 15:56:19.000000 encrypted-json-field-1.0.0/encrypted_json_field.egg-info/PKG-INFO
--rw-r--r--   0 el        (1000) el        (1000)      307 2023-08-06 15:56:19.000000 encrypted-json-field-1.0.0/encrypted_json_field.egg-info/SOURCES.txt
--rw-r--r--   0 el        (1000) el        (1000)        1 2023-08-06 15:56:19.000000 encrypted-json-field-1.0.0/encrypted_json_field.egg-info/dependency_links.txt
--rw-r--r--   0 el        (1000) el        (1000)       33 2023-08-06 15:56:19.000000 encrypted-json-field-1.0.0/encrypted_json_field.egg-info/requires.txt
--rw-r--r--   0 el        (1000) el        (1000)       21 2023-08-06 15:56:19.000000 encrypted-json-field-1.0.0/encrypted_json_field.egg-info/top_level.txt
--rw-r--r--   0 el        (1000) el        (1000)     1047 2023-08-06 15:53:52.000000 encrypted-json-field-1.0.0/pyproject.toml
--rw-r--r--   0 el        (1000) el        (1000)       38 2023-08-06 15:56:19.975442 encrypted-json-field-1.0.0/setup.cfg
+drwxr-xr-x   0 el        (1000) el        (1000)        0 2024-05-08 18:39:14.954923 encrypted_json_field-1.1.4/
+-rw-r--r--   0 el        (1000) el        (1000)     1841 2024-05-08 18:39:14.954923 encrypted_json_field-1.1.4/PKG-INFO
+-rw-r--r--   0 el        (1000) el        (1000)      856 2023-08-06 15:35:49.000000 encrypted_json_field-1.1.4/README.md
+drwxr-xr-x   0 el        (1000) el        (1000)        0 2024-05-08 18:39:14.951590 encrypted_json_field-1.1.4/encrypted_json_field/
+-rw-r--r--   0 el        (1000) el        (1000)     2632 2023-08-06 15:32:27.000000 encrypted_json_field-1.1.4/encrypted_json_field/__init__.py
+-rw-r--r--   0 el        (1000) el        (1000)     1354 2024-05-08 17:56:37.000000 encrypted_json_field-1.1.4/encrypted_json_field/mixins.py
+drwxr-xr-x   0 el        (1000) el        (1000)        0 2024-05-08 18:39:14.954923 encrypted_json_field-1.1.4/encrypted_json_field.egg-info/
+-rw-r--r--   0 el        (1000) el        (1000)     1841 2024-05-08 18:39:14.000000 encrypted_json_field-1.1.4/encrypted_json_field.egg-info/PKG-INFO
+-rw-r--r--   0 el        (1000) el        (1000)      307 2024-05-08 18:39:14.000000 encrypted_json_field-1.1.4/encrypted_json_field.egg-info/SOURCES.txt
+-rw-r--r--   0 el        (1000) el        (1000)        1 2024-05-08 18:39:14.000000 encrypted_json_field-1.1.4/encrypted_json_field.egg-info/dependency_links.txt
+-rw-r--r--   0 el        (1000) el        (1000)       33 2024-05-08 18:39:14.000000 encrypted_json_field-1.1.4/encrypted_json_field.egg-info/requires.txt
+-rw-r--r--   0 el        (1000) el        (1000)       21 2024-05-08 18:39:14.000000 encrypted_json_field-1.1.4/encrypted_json_field.egg-info/top_level.txt
+-rw-r--r--   0 el        (1000) el        (1000)     1047 2024-05-08 18:37:55.000000 encrypted_json_field-1.1.4/pyproject.toml
+-rw-r--r--   0 el        (1000) el        (1000)       38 2024-05-08 18:39:14.954923 encrypted_json_field-1.1.4/setup.cfg
```

### Comparing `encrypted-json-field-1.0.0/PKG-INFO` & `encrypted_json_field-1.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encrypted-json-field
-Version: 1.0.0
+Version: 1.1.4
 Summary: Encrypted JSON field supports automatic encryption/ decryption of JSON fields with padding to conceal start and end of value.
 Author-email: El Majidi <elm.majidi@gmail.com>
 Project-URL: Homepage, https://github.com/MurphyAdam/encrypted-json-field
 Project-URL: Bug Tracker, https://github.com/MurphyAdam/encrypted-json-field/issues
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
@@ -13,14 +13,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: pycryptodome==3.20.0
+Requires-Dist: Django>=4.2
 
 # Encrypted JSON Field
 
 Encrypted JSON field supports automatic encryption/ decryption of JSON fields with padding to conceal start and end of value.
 
 ## Setup
```

### Comparing `encrypted-json-field-1.0.0/README.md` & `encrypted_json_field-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `encrypted-json-field-1.0.0/encrypted_json_field/__init__.py` & `encrypted_json_field-1.1.4/encrypted_json_field/__init__.py`

 * *Files identical despite different names*

### Comparing `encrypted-json-field-1.0.0/encrypted_json_field/mixins.py` & `encrypted_json_field-1.1.4/encrypted_json_field/mixins.py`

 * *Files identical despite different names*

### Comparing `encrypted-json-field-1.0.0/encrypted_json_field.egg-info/PKG-INFO` & `encrypted_json_field-1.1.4/encrypted_json_field.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encrypted-json-field
-Version: 1.0.0
+Version: 1.1.4
 Summary: Encrypted JSON field supports automatic encryption/ decryption of JSON fields with padding to conceal start and end of value.
 Author-email: El Majidi <elm.majidi@gmail.com>
 Project-URL: Homepage, https://github.com/MurphyAdam/encrypted-json-field
 Project-URL: Bug Tracker, https://github.com/MurphyAdam/encrypted-json-field/issues
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
@@ -13,14 +13,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: pycryptodome==3.20.0
+Requires-Dist: Django>=4.2
 
 # Encrypted JSON Field
 
 Encrypted JSON field supports automatic encryption/ decryption of JSON fields with padding to conceal start and end of value.
 
 ## Setup
```

### Comparing `encrypted-json-field-1.0.0/pyproject.toml` & `encrypted_json_field-1.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "encrypted-json-field"
-version = "1.0.0"
+version = "1.1.4"
 authors = [
   { name="El Majidi", email="elm.majidi@gmail.com" },
 ]
 description = "Encrypted JSON field supports automatic encryption/ decryption of JSON fields with padding to conceal start and end of value."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
-    "pycryptodome==3.16.0",
+    "pycryptodome==3.20.0",
     "Django>=4.2",
 ]
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 4.2",
     "License :: OSI Approved :: MIT License",
```

