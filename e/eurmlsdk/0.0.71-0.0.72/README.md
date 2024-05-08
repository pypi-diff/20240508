# Comparing `tmp/eurmlsdk-0.0.71.tar.gz` & `tmp/eurmlsdk-0.0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.71.tar", last modified: Tue May  7 11:51:30 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.72.tar", last modified: Wed May  8 07:38:45 2024, max compression
```

## Comparing `eurmlsdk-0.0.71.tar` & `eurmlsdk-0.0.72.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 11:51:30.284356 eurmlsdk-0.0.71/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       16 2024-04-29 05:37:24.000000 eurmlsdk-0.0.71/LICENSE.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-04-29 05:37:24.000000 eurmlsdk-0.0.71/MANIFEST.in
--rw-r--r--   0 surajram  (1000) surajram  (1000)      461 2024-05-07 11:51:30.284356 eurmlsdk-0.0.71/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)       10 2024-05-07 07:43:41.000000 eurmlsdk-0.0.71/README.md
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 11:51:30.274356 eurmlsdk-0.0.71/eurmlsdk/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       31 2024-05-07 10:58:56.000000 eurmlsdk-0.0.71/eurmlsdk/__init__.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)     3155 2024-05-07 11:03:15.000000 eurmlsdk-0.0.71/eurmlsdk/__main__.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)    10466 2024-05-07 09:25:59.000000 eurmlsdk-0.0.71/eurmlsdk/base_class.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)     3332 2024-05-07 11:51:04.000000 eurmlsdk-0.0.71/eurmlsdk/eur_sdk.py
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 11:51:30.274356 eurmlsdk-0.0.71/eurmlsdk.egg-info/
--rw-r--r--   0 surajram  (1000) surajram  (1000)      461 2024-05-07 11:51:29.000000 eurmlsdk-0.0.71/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)      321 2024-05-07 11:51:29.000000 eurmlsdk-0.0.71/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-05-07 11:51:29.000000 eurmlsdk-0.0.71/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       52 2024-05-07 11:51:29.000000 eurmlsdk-0.0.71/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       41 2024-05-07 11:51:29.000000 eurmlsdk-0.0.71/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        9 2024-05-07 11:51:29.000000 eurmlsdk-0.0.71/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-05-07 11:51:30.284356 eurmlsdk-0.0.71/setup.cfg
--rw-r--r--   0 surajram  (1000) surajram  (1000)      719 2024-05-07 11:51:25.000000 eurmlsdk-0.0.71/setup.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 07:38:45.479799 eurmlsdk-0.0.72/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-07 14:45:59.000000 eurmlsdk-0.0.72/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-07 14:45:59.000000 eurmlsdk-0.0.72/MANIFEST.in
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 07:38:45.479799 eurmlsdk-0.0.72/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-07 14:45:59.000000 eurmlsdk-0.0.72/README.md
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 07:38:45.479799 eurmlsdk-0.0.72/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-07 14:45:59.000000 eurmlsdk-0.0.72/eurmlsdk/__init__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3198 2024-05-08 07:27:05.000000 eurmlsdk-0.0.72/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-07 14:45:59.000000 eurmlsdk-0.0.72/eurmlsdk/base_class.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3944 2024-05-08 07:34:00.000000 eurmlsdk-0.0.72/eurmlsdk/eur_sdk.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 07:38:45.479799 eurmlsdk-0.0.72/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 07:38:45.000000 eurmlsdk-0.0.72/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-08 07:38:45.000000 eurmlsdk-0.0.72/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-08 07:38:45.000000 eurmlsdk-0.0.72/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-08 07:38:45.000000 eurmlsdk-0.0.72/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       41 2024-05-08 07:38:45.000000 eurmlsdk-0.0.72/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-08 07:38:45.000000 eurmlsdk-0.0.72/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-08 07:38:45.479799 eurmlsdk-0.0.72/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      719 2024-05-08 07:35:49.000000 eurmlsdk-0.0.72/setup.py
```

### Comparing `eurmlsdk-0.0.71/eurmlsdk/__main__.py` & `eurmlsdk-0.0.72/eurmlsdk/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,65 +6,63 @@
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'  # Suppress TensorFlow info and warning logs
 logging.getLogger('tensorflow').setLevel(logging.ERROR)  # Suppress TensorFlow warning logs
 logging.getLogger('tensorflow.compiler.tf2tensorrt').setLevel(logging.ERROR)  # Suppress TensorFlow-TRT warning logs
 
 def list_commands():
     print("Available commands in mlsdk package are:")
     print("  help | --h                : Lists all commands available in mlsdk package")
-    print("  validate <local path>")
-    print("  predict <local path> <dataset>")
-    print("  deploy <local path> <hostname> <username> <password> : Uploads the model file in the Raspberry pi")
-    print("     <local path> : path to the model file")
+    print("  validate <model path>     : Validates the model and returns the metrics using default dataset")
+    print("  predict <model path> <dataset> : Predicts the labels and saves the predicted image")
+    print("  deploy <model path> <hostname> <username> <password> : Uploads the model file in the Raspberry pi")
+    print("     <model path> : path to the model file")
     print("     <dataset>    : sample dataset image")
     print("     <hostname>   : hostname to connect to Raspberry pi")
     print("     <username>   : username to connect to Raspberry pi")
     print("     <password>   : password to connect to Raspberry pi")
 
-
-
 def main(): 
     if len(argv) == 1:
         print("Model Zoo SDK")
         print("Package name: eurmlsdk")
         print("Version: 0.0.1")
         print("Run 'eurmlsdk help' or eurmlsdk --h to find the list of commands.")
         exit(1)
 
     command = argv[1]
     if command == "help" or command == "--h":
         list_commands()
         exit(1)
         
     elif command == "validate":
-            if len(argv) <3:
-                print("Give the model file name or file path")
-            else:
-                modelPath = argv[2]
-                yoloSDK = ModelYolo()
-                yoloSDK.vaidateModel(modelPath)
-            exit(1)
+        if len(argv) <3:
+            print("Give the model file name or file path")
+        else:
+            modelPath = argv[2]
+            yoloSDK = ModelYolo()
+            yoloSDK.validateModel(modelPath)
+        exit(1)
         
     elif command == "predict":
-            if len(argv) <3:
-                print("Give the model file name or file file path")
-                exit(1)
-            elif len(argv) <4:
-                print("Please provide atlest one data set of images")
-                exit(1)                                                                                                                               
-            else:
-                 modelPath = argv[2]
-                 predictData = argv[3]
-                 yoloSDK = ModelYolo()
-                 yoloSDK.predictModel(modelPath, predictData)
-            exit(1)    
+        if len(argv) <3:
+            print("Give the model file name or file file path")
+            exit(1)
+        elif len(argv) <4:
+            print("Please provide atlest one data set of images")
+            exit(1)                                                                                                                               
+        else:
+            modelPath = argv[2]
+            predictData = argv[3]
+            yoloSDK = ModelYolo()
+            yoloSDK.predictModel(modelPath, predictData)
+        exit(1)    
     
     elif command == "deploy":
         if len(argv) < 6:
             print("Missing required arguments")
-            print("Usage: eurmlsdk deploy <local path> <hostname> <username> <password>")
+            print("Usage: eurmlsdk deploy <model path> <hostname> <username> <password>")
         else:
             localPath = argv[2]
             remotePath = "/home/embeduradmin/" + localPath.split("/")[-1]
             hostname = argv[3]
             username = argv[4]
             password = argv[5]
             yoloSDK = ModelYolo()
```

### Comparing `eurmlsdk-0.0.71/eurmlsdk/base_class.py` & `eurmlsdk-0.0.72/eurmlsdk/base_class.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.71/setup.py` & `eurmlsdk-0.0.72/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.71',
+    version='0.0.72',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'python-dotenv',
         'paramiko',
```

