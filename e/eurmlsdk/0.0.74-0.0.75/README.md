# Comparing `tmp/eurmlsdk-0.0.74.tar.gz` & `tmp/eurmlsdk-0.0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.74.tar", last modified: Wed May  8 08:08:11 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.75.tar", last modified: Wed May  8 08:27:33 2024, max compression
```

## Comparing `eurmlsdk-0.0.74.tar` & `eurmlsdk-0.0.75.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 08:08:11.039799 eurmlsdk-0.0.74/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-07 14:45:59.000000 eurmlsdk-0.0.74/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-07 14:45:59.000000 eurmlsdk-0.0.74/MANIFEST.in
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 08:08:11.039799 eurmlsdk-0.0.74/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-07 14:45:59.000000 eurmlsdk-0.0.74/README.md
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 08:08:11.039799 eurmlsdk-0.0.74/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-07 14:45:59.000000 eurmlsdk-0.0.74/eurmlsdk/__init__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3199 2024-05-08 08:08:02.000000 eurmlsdk-0.0.74/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-07 14:45:59.000000 eurmlsdk-0.0.74/eurmlsdk/base_class.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4022 2024-05-08 08:03:23.000000 eurmlsdk-0.0.74/eurmlsdk/eur_sdk.py
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 08:08:11.039799 eurmlsdk-0.0.74/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 08:08:10.000000 eurmlsdk-0.0.74/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-08 08:08:10.000000 eurmlsdk-0.0.74/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-08 08:08:10.000000 eurmlsdk-0.0.74/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-08 08:08:10.000000 eurmlsdk-0.0.74/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       67 2024-05-08 08:08:10.000000 eurmlsdk-0.0.74/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-08 08:08:10.000000 eurmlsdk-0.0.74/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-08 08:08:11.039799 eurmlsdk-0.0.74/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      767 2024-05-08 08:07:08.000000 eurmlsdk-0.0.74/setup.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 08:27:33.109799 eurmlsdk-0.0.75/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-07 14:45:59.000000 eurmlsdk-0.0.75/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-07 14:45:59.000000 eurmlsdk-0.0.75/MANIFEST.in
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 08:27:33.109799 eurmlsdk-0.0.75/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-07 14:45:59.000000 eurmlsdk-0.0.75/README.md
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 08:27:33.109799 eurmlsdk-0.0.75/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-07 14:45:59.000000 eurmlsdk-0.0.75/eurmlsdk/__init__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3255 2024-05-08 08:12:52.000000 eurmlsdk-0.0.75/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-07 14:45:59.000000 eurmlsdk-0.0.75/eurmlsdk/base_class.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4022 2024-05-08 08:03:23.000000 eurmlsdk-0.0.75/eurmlsdk/eur_sdk.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 08:27:33.109799 eurmlsdk-0.0.75/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 08:27:33.000000 eurmlsdk-0.0.75/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-08 08:27:33.000000 eurmlsdk-0.0.75/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-08 08:27:33.000000 eurmlsdk-0.0.75/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-08 08:27:33.000000 eurmlsdk-0.0.75/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       67 2024-05-08 08:27:33.000000 eurmlsdk-0.0.75/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-08 08:27:33.000000 eurmlsdk-0.0.75/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-08 08:27:33.109799 eurmlsdk-0.0.75/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      767 2024-05-08 08:26:45.000000 eurmlsdk-0.0.75/setup.py
```

### Comparing `eurmlsdk-0.0.74/eurmlsdk/__main__.py` & `eurmlsdk-0.0.75/eurmlsdk/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 logging.getLogger('tensorflow.compiler.tf2tensorrt').setLevel(logging.ERROR)  # Suppress TensorFlow-TRT warning logs
 
 def list_commands():
     print("Available commands in mlsdk package are:")
     print("  help | --h                : Lists all commands available in mlsdk package")
     print("  validate <model path>     : Validates the model and returns the metrics using default dataset")
     print("  predict <model path> <dataset> : Predicts the labels and saves the predicted image")
-    print("  deploy <model path> <hostname> <username> <password> : Uploads the model file in the Raspberry pi")
     print("     <model path> : path to the model file")
     print("     <dataset>    : sample dataset image")
+    print("  deploy <model path> <hostname> <username> <password> : Uploads the model file in the Raspberry pi")
+    print("     <model path> : path to the model file")
     print("     <hostname>   : hostname to connect to Raspberry pi")
     print("     <username>   : username to connect to Raspberry pi")
     print("     <password>   : password to connect to Raspberry pi")
 
 def main(): 
     if len(argv) == 1:
         print("Model Zoo SDK")
```

### Comparing `eurmlsdk-0.0.74/eurmlsdk/base_class.py` & `eurmlsdk-0.0.75/eurmlsdk/base_class.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.74/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.75/eurmlsdk/eur_sdk.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.74/setup.py` & `eurmlsdk-0.0.75/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.74',
+    version='0.0.75',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'python-dotenv',
         'paramiko',
```

