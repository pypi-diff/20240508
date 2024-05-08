# Comparing `tmp/opencv_cam_idx-1.0.0.tar.gz` & `tmp/opencv_cam_idx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencv_cam_idx-1.0.0.tar", last modified: Tue May  7 14:46:03 2024, max compression
+gzip compressed data, was "opencv_cam_idx-1.0.1.tar", last modified: Wed May  8 13:43:47 2024, max compression
```

## Comparing `opencv_cam_idx-1.0.0.tar` & `opencv_cam_idx-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:46:03.833317 opencv_cam_idx-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 14:45:58.000000 opencv_cam_idx-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 14:45:58.000000 opencv_cam_idx-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-07 14:46:03.833317 opencv_cam_idx-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-07 14:45:58.000000 opencv_cam_idx-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:46:03.833317 opencv_cam_idx-1.0.0/opencv_cam_idx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:45:58.000000 opencv_cam_idx-1.0.0/opencv_cam_idx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-07 14:45:58.000000 opencv_cam_idx-1.0.0/opencv_cam_idx/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-07 14:45:58.000000 opencv_cam_idx-1.0.0/opencv_cam_idx/moniker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:45:58.000000 opencv_cam_idx-1.0.0/opencv_cam_idx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:46:03.833317 opencv_cam_idx-1.0.0/opencv_cam_idx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-07 14:46:03.000000 opencv_cam_idx-1.0.0/opencv_cam_idx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-07 14:46:03.000000 opencv_cam_idx-1.0.0/opencv_cam_idx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:46:03.000000 opencv_cam_idx-1.0.0/opencv_cam_idx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 14:46:03.000000 opencv_cam_idx-1.0.0/opencv_cam_idx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 14:46:03.000000 opencv_cam_idx-1.0.0/opencv_cam_idx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-07 14:45:58.000000 opencv_cam_idx-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:46:03.833317 opencv_cam_idx-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:43:47.261236 opencv_cam_idx-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-08 13:43:42.000000 opencv_cam_idx-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 13:43:42.000000 opencv_cam_idx-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-08 13:43:47.261236 opencv_cam_idx-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-08 13:43:42.000000 opencv_cam_idx-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:43:47.261236 opencv_cam_idx-1.0.1/opencv_cam_idx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:43:42.000000 opencv_cam_idx-1.0.1/opencv_cam_idx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-08 13:43:42.000000 opencv_cam_idx-1.0.1/opencv_cam_idx/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-08 13:43:42.000000 opencv_cam_idx-1.0.1/opencv_cam_idx/moniker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:43:42.000000 opencv_cam_idx-1.0.1/opencv_cam_idx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:43:47.261236 opencv_cam_idx-1.0.1/opencv_cam_idx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-08 13:43:47.000000 opencv_cam_idx-1.0.1/opencv_cam_idx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-08 13:43:47.000000 opencv_cam_idx-1.0.1/opencv_cam_idx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:43:47.000000 opencv_cam_idx-1.0.1/opencv_cam_idx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 13:43:47.000000 opencv_cam_idx-1.0.1/opencv_cam_idx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 13:43:47.000000 opencv_cam_idx-1.0.1/opencv_cam_idx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-08 13:43:42.000000 opencv_cam_idx-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:43:47.261236 opencv_cam_idx-1.0.1/setup.cfg
```

### Comparing `opencv_cam_idx-1.0.0/LICENSE` & `opencv_cam_idx-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opencv_cam_idx-1.0.0/PKG-INFO` & `opencv_cam_idx-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencv-cam-idx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Find opencv camera index in windows using win32 api
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `opencv_cam_idx-1.0.0/README.md` & `opencv_cam_idx-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `opencv_cam_idx-1.0.0/opencv_cam_idx/finder.py` & `opencv_cam_idx-1.0.1/opencv_cam_idx/finder.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from ctypes import POINTER
 from ctypes import c_int
 from dataclasses import dataclass
 from typing import Any
 
 from comtypes import COMMETHOD  # type: ignore
 from comtypes import GUID
+from comtypes import CoInitialize
 from comtypes import COMError
 from comtypes import IUnknown
 from comtypes import client
 from comtypes.persist import IPropertyBag
 
 from opencv_cam_idx.moniker import IEnumMoniker
 
@@ -58,14 +59,15 @@
     description: str
 
 
 def find_cameras():
     # Reference
     # https://learn.microsoft.com/en-us/windows/win32/directshow/selecting-a-capture-device
 
+    CoInitialize()  # fixes CoInitialize has not been called
     system_device_enum: Any = client.CreateObject(
         clsids.CLSID_SystemDeviceEnum, interface=ICreateDevEnum
     )
     filter_enumerator = system_device_enum.CreateClassEnumerator(
         GUID(DeviceCategories.VideoInputDevice), dwFlags=0
     )
     cameras: list[Camera] = []
```

### Comparing `opencv_cam_idx-1.0.0/opencv_cam_idx/moniker.py` & `opencv_cam_idx-1.0.1/opencv_cam_idx/moniker.py`

 * *Files identical despite different names*

### Comparing `opencv_cam_idx-1.0.0/opencv_cam_idx.egg-info/PKG-INFO` & `opencv_cam_idx-1.0.1/opencv_cam_idx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencv-cam-idx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Find opencv camera index in windows using win32 api
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `opencv_cam_idx-1.0.0/pyproject.toml` & `opencv_cam_idx-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "opencv-cam-idx"
-version = "1.0.0"
+version = "1.0.1"
 dependencies = ["comtypes"]
 requires-python = ">=3"
 authors = [{ name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" }]
 description = "Find opencv camera index in windows using win32 api"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = []
```

