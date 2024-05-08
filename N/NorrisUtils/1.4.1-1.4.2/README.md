# Comparing `tmp/NorrisUtils-1.4.1.tar.gz` & `tmp/NorrisUtils-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NorrisUtils-1.4.1.tar", last modified: Wed May  8 03:18:35 2024, max compression
+gzip compressed data, was "NorrisUtils-1.4.2.tar", last modified: Wed May  8 03:28:08 2024, max compression
```

## Comparing `NorrisUtils-1.4.1.tar` & `NorrisUtils-1.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 03:18:34.997584 NorrisUtils-1.4.1/
-drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 03:18:34.994783 NorrisUtils-1.4.1/NorrisUtils/
--rw-r--r--   0 htd        (502) staff       (20)       42 2022-12-21 09:04:02.000000 NorrisUtils-1.4.1/NorrisUtils/BuildConfig.py
--rw-r--r--   0 htd        (502) staff       (20)    12573 2024-05-08 03:18:05.000000 NorrisUtils-1.4.1/NorrisUtils/DingTalkGenius.py
--rw-r--r--   0 htd        (502) staff       (20)     5581 2023-10-17 09:11:02.000000 NorrisUtils-1.4.1/NorrisUtils/FileUtil.py
--rw-r--r--   0 htd        (502) staff       (20)     1392 2022-12-21 09:04:02.000000 NorrisUtils-1.4.1/NorrisUtils/GarbageGenius.py
--rw-r--r--   0 htd        (502) staff       (20)     3351 2024-05-08 03:17:50.000000 NorrisUtils-1.4.1/NorrisUtils/ImageUploadUtils.py
--rw-r--r--   0 htd        (502) staff       (20)    10121 2022-12-21 09:04:02.000000 NorrisUtils-1.4.1/NorrisUtils/RawUtil.py
--rw-r--r--   0 htd        (502) staff       (20)     2755 2022-12-21 09:04:02.000000 NorrisUtils-1.4.1/NorrisUtils/RawUtils.py
--rw-r--r--   0 htd        (502) staff       (20)     8470 2022-12-21 09:04:02.000000 NorrisUtils-1.4.1/NorrisUtils/RequestUtils.py
--rw-r--r--   0 htd        (502) staff       (20)       20 2022-12-21 09:04:02.000000 NorrisUtils-1.4.1/NorrisUtils/__init__.py
-drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 03:18:34.996832 NorrisUtils-1.4.1/NorrisUtils.egg-info/
--rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 03:18:34.000000 NorrisUtils-1.4.1/NorrisUtils.egg-info/PKG-INFO
--rw-r--r--   0 htd        (502) staff       (20)      433 2024-05-08 03:18:34.000000 NorrisUtils-1.4.1/NorrisUtils.egg-info/SOURCES.txt
--rw-r--r--   0 htd        (502) staff       (20)        1 2024-05-08 03:18:34.000000 NorrisUtils-1.4.1/NorrisUtils.egg-info/dependency_links.txt
--rw-r--r--   0 htd        (502) staff       (20)       17 2024-05-08 03:18:34.000000 NorrisUtils-1.4.1/NorrisUtils.egg-info/requires.txt
--rw-r--r--   0 htd        (502) staff       (20)       12 2024-05-08 03:18:34.000000 NorrisUtils-1.4.1/NorrisUtils.egg-info/top_level.txt
--rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 03:18:34.997206 NorrisUtils-1.4.1/PKG-INFO
--rw-r--r--   0 htd        (502) staff       (20)       60 2022-12-21 09:04:02.000000 NorrisUtils-1.4.1/README.md
--rw-r--r--   0 htd        (502) staff       (20)       38 2024-05-08 03:18:34.997678 NorrisUtils-1.4.1/setup.cfg
--rw-r--r--   0 htd        (502) staff       (20)     1256 2024-05-08 03:18:24.000000 NorrisUtils-1.4.1/setup.py
+drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 03:28:08.920722 NorrisUtils-1.4.2/
+drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 03:28:08.917478 NorrisUtils-1.4.2/NorrisUtils/
+-rw-r--r--   0 htd        (502) staff       (20)       42 2022-12-21 09:04:02.000000 NorrisUtils-1.4.2/NorrisUtils/BuildConfig.py
+-rw-r--r--   0 htd        (502) staff       (20)    12597 2024-05-08 03:28:03.000000 NorrisUtils-1.4.2/NorrisUtils/DingTalkGenius.py
+-rw-r--r--   0 htd        (502) staff       (20)     5581 2023-10-17 09:11:02.000000 NorrisUtils-1.4.2/NorrisUtils/FileUtil.py
+-rw-r--r--   0 htd        (502) staff       (20)     1392 2022-12-21 09:04:02.000000 NorrisUtils-1.4.2/NorrisUtils/GarbageGenius.py
+-rw-r--r--   0 htd        (502) staff       (20)     3351 2024-05-08 03:17:50.000000 NorrisUtils-1.4.2/NorrisUtils/ImageUploadUtils.py
+-rw-r--r--   0 htd        (502) staff       (20)    10121 2022-12-21 09:04:02.000000 NorrisUtils-1.4.2/NorrisUtils/RawUtil.py
+-rw-r--r--   0 htd        (502) staff       (20)     2755 2022-12-21 09:04:02.000000 NorrisUtils-1.4.2/NorrisUtils/RawUtils.py
+-rw-r--r--   0 htd        (502) staff       (20)     8470 2022-12-21 09:04:02.000000 NorrisUtils-1.4.2/NorrisUtils/RequestUtils.py
+-rw-r--r--   0 htd        (502) staff       (20)       20 2022-12-21 09:04:02.000000 NorrisUtils-1.4.2/NorrisUtils/__init__.py
+drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 03:28:08.919866 NorrisUtils-1.4.2/NorrisUtils.egg-info/
+-rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 03:28:08.000000 NorrisUtils-1.4.2/NorrisUtils.egg-info/PKG-INFO
+-rw-r--r--   0 htd        (502) staff       (20)      433 2024-05-08 03:28:08.000000 NorrisUtils-1.4.2/NorrisUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 htd        (502) staff       (20)        1 2024-05-08 03:28:08.000000 NorrisUtils-1.4.2/NorrisUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 htd        (502) staff       (20)       17 2024-05-08 03:28:08.000000 NorrisUtils-1.4.2/NorrisUtils.egg-info/requires.txt
+-rw-r--r--   0 htd        (502) staff       (20)       12 2024-05-08 03:28:08.000000 NorrisUtils-1.4.2/NorrisUtils.egg-info/top_level.txt
+-rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 03:28:08.920287 NorrisUtils-1.4.2/PKG-INFO
+-rw-r--r--   0 htd        (502) staff       (20)       60 2022-12-21 09:04:02.000000 NorrisUtils-1.4.2/README.md
+-rw-r--r--   0 htd        (502) staff       (20)       38 2024-05-08 03:28:08.920868 NorrisUtils-1.4.2/setup.cfg
+-rw-r--r--   0 htd        (502) staff       (20)     1256 2024-05-08 03:28:03.000000 NorrisUtils-1.4.2/setup.py
```

### Comparing `NorrisUtils-1.4.1/NorrisUtils/DingTalkGenius.py` & `NorrisUtils-1.4.2/NorrisUtils/DingTalkGenius.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import base64
 import hashlib
 import hmac
 import json
 import time
 import urllib.parse
 
-import ImageUploadUtils
+import NorrisUtils.ImageUploadUtils
 
 
 def sign(secret: str, timestamp):
     """
     生成钉钉消息签名。
 
     参数:
@@ -247,15 +247,15 @@
     kwargs.setdefault("atMobiles", [])
     callback = kwargs["callback"]
     logfunc = kwargs["logfunc"]
     magic = kwargs["magic"]
     if magic is not None:
         image_url = magic(image_path)
     else:
-        image_url = ImageUploadUtils.upload_image_to_smms(
+        image_url = NorrisUtils.ImageUploadUtils.upload_image_to_smms(
             image_path,
             kwargs["token"]
         )
     if image_url is None or image_url == "":
         logfunc("未能成功上传图片，请检查！")
         if callback:
             callback()
```

### Comparing `NorrisUtils-1.4.1/NorrisUtils/FileUtil.py` & `NorrisUtils-1.4.2/NorrisUtils/FileUtil.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.1/NorrisUtils/GarbageGenius.py` & `NorrisUtils-1.4.2/NorrisUtils/GarbageGenius.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.1/NorrisUtils/ImageUploadUtils.py` & `NorrisUtils-1.4.2/NorrisUtils/ImageUploadUtils.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.1/NorrisUtils/RawUtil.py` & `NorrisUtils-1.4.2/NorrisUtils/RawUtil.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.1/NorrisUtils/RawUtils.py` & `NorrisUtils-1.4.2/NorrisUtils/RawUtils.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.1/NorrisUtils/RequestUtils.py` & `NorrisUtils-1.4.2/NorrisUtils/RequestUtils.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.1/NorrisUtils.egg-info/PKG-INFO` & `NorrisUtils-1.4.2/NorrisUtils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NorrisUtils
-Version: 1.4.1
+Version: 1.4.2
 Summary: 图床工具包，支持上传到sm.ms图床，支持发送钉钉消息
 Home-page: https://www.baidu.com
 Author: AlaricNorris
 Author-email: norris.sly@gmail.com
 Maintainer: AlaricNorris
 Maintainer-email: norris.sly@gmail.com
 License: BSD License
```

### Comparing `NorrisUtils-1.4.1/PKG-INFO` & `NorrisUtils-1.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NorrisUtils
-Version: 1.4.1
+Version: 1.4.2
 Summary: 图床工具包，支持上传到sm.ms图床，支持发送钉钉消息
 Home-page: https://www.baidu.com
 Author: AlaricNorris
 Author-email: norris.sly@gmail.com
 Maintainer: AlaricNorris
 Maintainer-email: norris.sly@gmail.com
 License: BSD License
```

### Comparing `NorrisUtils-1.4.1/setup.py` & `NorrisUtils-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='NorrisUtils',
-    version='1.4.1',
+    version='1.4.2',
     description=(
         '图床工具包，支持上传到sm.ms图床，支持发送钉钉消息'
     ),
     long_description=open('README.md').read(),
     author='AlaricNorris',
     author_email='norris.sly@gmail.com',
     maintainer='AlaricNorris',
```

