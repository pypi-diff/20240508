# Comparing `tmp/eurmlsdk-0.0.72.tar.gz` & `tmp/eurmlsdk-0.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.72.tar", last modified: Wed May  8 07:38:45 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.73.tar", last modified: Wed May  8 07:46:48 2024, max compression
```

## Comparing `eurmlsdk-0.0.72.tar` & `eurmlsdk-0.0.73.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 07:38:45.479799 eurmlsdk-0.0.72/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-07 14:45:59.000000 eurmlsdk-0.0.72/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-07 14:45:59.000000 eurmlsdk-0.0.72/MANIFEST.in
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 07:38:45.479799 eurmlsdk-0.0.72/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-07 14:45:59.000000 eurmlsdk-0.0.72/README.md
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 07:38:45.479799 eurmlsdk-0.0.72/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-07 14:45:59.000000 eurmlsdk-0.0.72/eurmlsdk/__init__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3198 2024-05-08 07:27:05.000000 eurmlsdk-0.0.72/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-07 14:45:59.000000 eurmlsdk-0.0.72/eurmlsdk/base_class.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3944 2024-05-08 07:34:00.000000 eurmlsdk-0.0.72/eurmlsdk/eur_sdk.py
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 07:38:45.479799 eurmlsdk-0.0.72/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 07:38:45.000000 eurmlsdk-0.0.72/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-08 07:38:45.000000 eurmlsdk-0.0.72/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-08 07:38:45.000000 eurmlsdk-0.0.72/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-08 07:38:45.000000 eurmlsdk-0.0.72/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       41 2024-05-08 07:38:45.000000 eurmlsdk-0.0.72/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-08 07:38:45.000000 eurmlsdk-0.0.72/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-08 07:38:45.479799 eurmlsdk-0.0.72/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      719 2024-05-08 07:35:49.000000 eurmlsdk-0.0.72/setup.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 07:46:48.589799 eurmlsdk-0.0.73/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-07 14:45:59.000000 eurmlsdk-0.0.73/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-07 14:45:59.000000 eurmlsdk-0.0.73/MANIFEST.in
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 07:46:48.589799 eurmlsdk-0.0.73/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-07 14:45:59.000000 eurmlsdk-0.0.73/README.md
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 07:46:48.579799 eurmlsdk-0.0.73/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-07 14:45:59.000000 eurmlsdk-0.0.73/eurmlsdk/__init__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3198 2024-05-08 07:27:05.000000 eurmlsdk-0.0.73/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-07 14:45:59.000000 eurmlsdk-0.0.73/eurmlsdk/base_class.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3945 2024-05-08 07:45:52.000000 eurmlsdk-0.0.73/eurmlsdk/eur_sdk.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-08 07:46:48.589799 eurmlsdk-0.0.73/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-08 07:46:48.000000 eurmlsdk-0.0.73/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-08 07:46:48.000000 eurmlsdk-0.0.73/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-08 07:46:48.000000 eurmlsdk-0.0.73/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-08 07:46:48.000000 eurmlsdk-0.0.73/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       41 2024-05-08 07:46:48.000000 eurmlsdk-0.0.73/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-08 07:46:48.000000 eurmlsdk-0.0.73/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-08 07:46:48.589799 eurmlsdk-0.0.73/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      719 2024-05-08 07:46:32.000000 eurmlsdk-0.0.73/setup.py
```

### Comparing `eurmlsdk-0.0.72/eurmlsdk/__main__.py` & `eurmlsdk-0.0.73/eurmlsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.72/eurmlsdk/base_class.py` & `eurmlsdk-0.0.73/eurmlsdk/base_class.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.72/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.73/eurmlsdk/eur_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
      def __init__(self, error= "Cannot Load Model"):
           self.error = error
           super().___init__(self.error)
 
 class EurBaseSDK():  
     def getModel(self, filepath) ->str:
         extension = filepath.split(".")
-        if extension[1] != "pt" or extension[1] != "tflite":
+        if extension[1] != "pt" and extension[1] != "tflite":
             print("Not supported file path")
             return ""
         
         if os.path.exists(filepath):
             print("Model file exist and ready to load")
             return filepath        
         else:
```

### Comparing `eurmlsdk-0.0.72/setup.py` & `eurmlsdk-0.0.73/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.72',
+    version='0.0.73',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'python-dotenv',
         'paramiko',
```

