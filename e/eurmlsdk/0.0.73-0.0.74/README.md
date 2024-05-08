# Comparing `tmp/eurmlsdk-0.0.73.tar.gz` & `tmp/eurmlsdk-0.0.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.73.tar", last modified: Wed May  8 07:46:48 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.74.tar", last modified: Wed May  8 08:08:11 2024, max compression
```

## Comparing `eurmlsdk-0.0.73.tar` & `eurmlsdk-0.0.74.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 07:46:48.589799 eurmlsdk-0.0.73/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-07 14:45:59.000000 eurmlsdk-0.0.73/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-07 14:45:59.000000 eurmlsdk-0.0.73/MANIFEST.in
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 07:46:48.589799 eurmlsdk-0.0.73/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-07 14:45:59.000000 eurmlsdk-0.0.73/README.md
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 07:46:48.579799 eurmlsdk-0.0.73/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-07 14:45:59.000000 eurmlsdk-0.0.73/eurmlsdk/__init__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3198 2024-05-08 07:27:05.000000 eurmlsdk-0.0.73/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-07 14:45:59.000000 eurmlsdk-0.0.73/eurmlsdk/base_class.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3945 2024-05-08 07:45:52.000000 eurmlsdk-0.0.73/eurmlsdk/eur_sdk.py
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 07:46:48.589799 eurmlsdk-0.0.73/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 07:46:48.000000 eurmlsdk-0.0.73/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-08 07:46:48.000000 eurmlsdk-0.0.73/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-08 07:46:48.000000 eurmlsdk-0.0.73/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-08 07:46:48.000000 eurmlsdk-0.0.73/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       41 2024-05-08 07:46:48.000000 eurmlsdk-0.0.73/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-08 07:46:48.000000 eurmlsdk-0.0.73/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-08 07:46:48.589799 eurmlsdk-0.0.73/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      719 2024-05-08 07:46:32.000000 eurmlsdk-0.0.73/setup.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 08:08:11.039799 eurmlsdk-0.0.74/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-07 14:45:59.000000 eurmlsdk-0.0.74/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-07 14:45:59.000000 eurmlsdk-0.0.74/MANIFEST.in
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 08:08:11.039799 eurmlsdk-0.0.74/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-07 14:45:59.000000 eurmlsdk-0.0.74/README.md
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 08:08:11.039799 eurmlsdk-0.0.74/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-07 14:45:59.000000 eurmlsdk-0.0.74/eurmlsdk/__init__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3199 2024-05-08 08:08:02.000000 eurmlsdk-0.0.74/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-07 14:45:59.000000 eurmlsdk-0.0.74/eurmlsdk/base_class.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4022 2024-05-08 08:03:23.000000 eurmlsdk-0.0.74/eurmlsdk/eur_sdk.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 08:08:11.039799 eurmlsdk-0.0.74/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 08:08:10.000000 eurmlsdk-0.0.74/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-08 08:08:10.000000 eurmlsdk-0.0.74/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-08 08:08:10.000000 eurmlsdk-0.0.74/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-08 08:08:10.000000 eurmlsdk-0.0.74/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       67 2024-05-08 08:08:10.000000 eurmlsdk-0.0.74/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-08 08:08:10.000000 eurmlsdk-0.0.74/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-08 08:08:11.039799 eurmlsdk-0.0.74/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      767 2024-05-08 08:07:08.000000 eurmlsdk-0.0.74/setup.py
```

### Comparing `eurmlsdk-0.0.73/eurmlsdk/__main__.py` & `eurmlsdk-0.0.74/eurmlsdk/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     print("     <username>   : username to connect to Raspberry pi")
     print("     <password>   : password to connect to Raspberry pi")
 
 def main(): 
     if len(argv) == 1:
         print("Model Zoo SDK")
         print("Package name: eurmlsdk")
-        print("Version: 0.0.1")
+        print("Version: 0.0.74")
         print("Run 'eurmlsdk help' or eurmlsdk --h to find the list of commands.")
         exit(1)
 
     command = argv[1]
     if command == "help" or command == "--h":
         list_commands()
         exit(1)
```

### Comparing `eurmlsdk-0.0.73/eurmlsdk/base_class.py` & `eurmlsdk-0.0.74/eurmlsdk/base_class.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.73/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.74/eurmlsdk/eur_sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,13 +93,15 @@
             print("Error :", err)
     
     def predictModel(self, pathArg, dataSet):
         data = []
         data.append(dataSet)
         try:
             model = self.loadModel(pathArg)
-            results = model(data, save=True)
-            for result in results:
-                result.save(filename="./result.jpg")
-                print("resuts saved in result.jpg")
+            model(data, save=True)
+            # for result in results:
+            #     result.save(filename="./result.jpg")
+            #     print("resuts saved in result.jpg")
         except ModelNotFound as err:
-            print("Error :", err)
+            print("Error :", err)
+        except Exception as err:
+            print("Error in Prediction :", err)
```

### Comparing `eurmlsdk-0.0.73/setup.py` & `eurmlsdk-0.0.74/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.73',
+    version='0.0.74',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'python-dotenv',
         'paramiko',
+        'tensorflow',
+        'tflite_runtime',
         'ultralytics'
     ],
     author='eUR',
     author_email='aiml@embedur.com',
     license='MIT',
     entry_points={
         "console_scripts": [
```

