# Comparing `tmp/eurmlsdk-0.0.75.tar.gz` & `tmp/eurmlsdk-0.0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.75.tar", last modified: Wed May  8 08:27:33 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.76.tar", last modified: Wed May  8 08:36:21 2024, max compression
```

## Comparing `eurmlsdk-0.0.75.tar` & `eurmlsdk-0.0.76.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 08:27:33.109799 eurmlsdk-0.0.75/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-07 14:45:59.000000 eurmlsdk-0.0.75/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-07 14:45:59.000000 eurmlsdk-0.0.75/MANIFEST.in
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 08:27:33.109799 eurmlsdk-0.0.75/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-07 14:45:59.000000 eurmlsdk-0.0.75/README.md
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 08:27:33.109799 eurmlsdk-0.0.75/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-07 14:45:59.000000 eurmlsdk-0.0.75/eurmlsdk/__init__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3255 2024-05-08 08:12:52.000000 eurmlsdk-0.0.75/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-07 14:45:59.000000 eurmlsdk-0.0.75/eurmlsdk/base_class.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4022 2024-05-08 08:03:23.000000 eurmlsdk-0.0.75/eurmlsdk/eur_sdk.py
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 08:27:33.109799 eurmlsdk-0.0.75/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 08:27:33.000000 eurmlsdk-0.0.75/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-08 08:27:33.000000 eurmlsdk-0.0.75/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-08 08:27:33.000000 eurmlsdk-0.0.75/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-08 08:27:33.000000 eurmlsdk-0.0.75/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       67 2024-05-08 08:27:33.000000 eurmlsdk-0.0.75/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-08 08:27:33.000000 eurmlsdk-0.0.75/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-08 08:27:33.109799 eurmlsdk-0.0.75/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      767 2024-05-08 08:26:45.000000 eurmlsdk-0.0.75/setup.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 08:36:21.639799 eurmlsdk-0.0.76/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-07 14:45:59.000000 eurmlsdk-0.0.76/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-07 14:45:59.000000 eurmlsdk-0.0.76/MANIFEST.in
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 08:36:21.639799 eurmlsdk-0.0.76/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-07 14:45:59.000000 eurmlsdk-0.0.76/README.md
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 08:36:21.639799 eurmlsdk-0.0.76/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-07 14:45:59.000000 eurmlsdk-0.0.76/eurmlsdk/__init__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3255 2024-05-08 08:35:54.000000 eurmlsdk-0.0.76/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-07 14:45:59.000000 eurmlsdk-0.0.76/eurmlsdk/base_class.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4022 2024-05-08 08:03:23.000000 eurmlsdk-0.0.76/eurmlsdk/eur_sdk.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 08:36:21.639799 eurmlsdk-0.0.76/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 08:36:21.000000 eurmlsdk-0.0.76/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-08 08:36:21.000000 eurmlsdk-0.0.76/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-08 08:36:21.000000 eurmlsdk-0.0.76/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-08 08:36:21.000000 eurmlsdk-0.0.76/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       41 2024-05-08 08:36:21.000000 eurmlsdk-0.0.76/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-08 08:36:21.000000 eurmlsdk-0.0.76/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-08 08:36:21.639799 eurmlsdk-0.0.76/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      719 2024-05-08 08:35:16.000000 eurmlsdk-0.0.76/setup.py
```

### Comparing `eurmlsdk-0.0.75/eurmlsdk/__main__.py` & `eurmlsdk-0.0.76/eurmlsdk/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     print("     <username>   : username to connect to Raspberry pi")
     print("     <password>   : password to connect to Raspberry pi")
 
 def main(): 
     if len(argv) == 1:
         print("Model Zoo SDK")
         print("Package name: eurmlsdk")
-        print("Version: 0.0.74")
+        print("Version: 0.0.76")
         print("Run 'eurmlsdk help' or eurmlsdk --h to find the list of commands.")
         exit(1)
 
     command = argv[1]
     if command == "help" or command == "--h":
         list_commands()
         exit(1)
```

### Comparing `eurmlsdk-0.0.75/eurmlsdk/base_class.py` & `eurmlsdk-0.0.76/eurmlsdk/base_class.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.75/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.76/eurmlsdk/eur_sdk.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.75/setup.py` & `eurmlsdk-0.0.76/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.75',
+    version='0.0.76',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'python-dotenv',
         'paramiko',
-        'tensorflow',
-        'tflite_runtime',
         'ultralytics'
     ],
     author='eUR',
     author_email='aiml@embedur.com',
     license='MIT',
     entry_points={
         "console_scripts": [
```

