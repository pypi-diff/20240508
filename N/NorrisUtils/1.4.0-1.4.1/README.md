# Comparing `tmp/NorrisUtils-1.4.0.tar.gz` & `tmp/NorrisUtils-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NorrisUtils-1.4.0.tar", last modified: Wed May  8 02:32:53 2024, max compression
+gzip compressed data, was "NorrisUtils-1.4.1.tar", last modified: Wed May  8 03:18:35 2024, max compression
```

## Comparing `NorrisUtils-1.4.0.tar` & `NorrisUtils-1.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 02:32:53.172912 NorrisUtils-1.4.0/
-drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 02:32:53.170669 NorrisUtils-1.4.0/NorrisUtils/
--rw-r--r--   0 htd        (502) staff       (20)       42 2022-12-21 09:04:02.000000 NorrisUtils-1.4.0/NorrisUtils/BuildConfig.py
--rw-r--r--   0 htd        (502) staff       (20)    12573 2024-05-07 09:49:57.000000 NorrisUtils-1.4.0/NorrisUtils/DingTalkGenius.py
--rw-r--r--   0 htd        (502) staff       (20)     5581 2023-10-17 09:11:02.000000 NorrisUtils-1.4.0/NorrisUtils/FileUtil.py
--rw-r--r--   0 htd        (502) staff       (20)     1392 2022-12-21 09:04:02.000000 NorrisUtils-1.4.0/NorrisUtils/GarbageGenius.py
--rw-r--r--   0 htd        (502) staff       (20)     2939 2024-04-30 02:40:51.000000 NorrisUtils-1.4.0/NorrisUtils/ImageUploadUtils.py
--rw-r--r--   0 htd        (502) staff       (20)    10121 2022-12-21 09:04:02.000000 NorrisUtils-1.4.0/NorrisUtils/RawUtil.py
--rw-r--r--   0 htd        (502) staff       (20)     2755 2022-12-21 09:04:02.000000 NorrisUtils-1.4.0/NorrisUtils/RawUtils.py
--rw-r--r--   0 htd        (502) staff       (20)     8470 2022-12-21 09:04:02.000000 NorrisUtils-1.4.0/NorrisUtils/RequestUtils.py
--rw-r--r--   0 htd        (502) staff       (20)       20 2022-12-21 09:04:02.000000 NorrisUtils-1.4.0/NorrisUtils/__init__.py
-drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 02:32:53.172309 NorrisUtils-1.4.0/NorrisUtils.egg-info/
--rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 02:32:53.000000 NorrisUtils-1.4.0/NorrisUtils.egg-info/PKG-INFO
--rw-r--r--   0 htd        (502) staff       (20)      433 2024-05-08 02:32:53.000000 NorrisUtils-1.4.0/NorrisUtils.egg-info/SOURCES.txt
--rw-r--r--   0 htd        (502) staff       (20)        1 2024-05-08 02:32:53.000000 NorrisUtils-1.4.0/NorrisUtils.egg-info/dependency_links.txt
--rw-r--r--   0 htd        (502) staff       (20)       17 2024-05-08 02:32:53.000000 NorrisUtils-1.4.0/NorrisUtils.egg-info/requires.txt
--rw-r--r--   0 htd        (502) staff       (20)       12 2024-05-08 02:32:53.000000 NorrisUtils-1.4.0/NorrisUtils.egg-info/top_level.txt
--rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 02:32:53.172628 NorrisUtils-1.4.0/PKG-INFO
--rw-r--r--   0 htd        (502) staff       (20)       60 2022-12-21 09:04:02.000000 NorrisUtils-1.4.0/README.md
--rw-r--r--   0 htd        (502) staff       (20)       38 2024-05-08 02:32:53.172989 NorrisUtils-1.4.0/setup.cfg
--rw-r--r--   0 htd        (502) staff       (20)     1256 2024-05-08 02:32:47.000000 NorrisUtils-1.4.0/setup.py
+drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 03:18:34.997584 NorrisUtils-1.4.1/
+drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 03:18:34.994783 NorrisUtils-1.4.1/NorrisUtils/
+-rw-r--r--   0 htd        (502) staff       (20)       42 2022-12-21 09:04:02.000000 NorrisUtils-1.4.1/NorrisUtils/BuildConfig.py
+-rw-r--r--   0 htd        (502) staff       (20)    12573 2024-05-08 03:18:05.000000 NorrisUtils-1.4.1/NorrisUtils/DingTalkGenius.py
+-rw-r--r--   0 htd        (502) staff       (20)     5581 2023-10-17 09:11:02.000000 NorrisUtils-1.4.1/NorrisUtils/FileUtil.py
+-rw-r--r--   0 htd        (502) staff       (20)     1392 2022-12-21 09:04:02.000000 NorrisUtils-1.4.1/NorrisUtils/GarbageGenius.py
+-rw-r--r--   0 htd        (502) staff       (20)     3351 2024-05-08 03:17:50.000000 NorrisUtils-1.4.1/NorrisUtils/ImageUploadUtils.py
+-rw-r--r--   0 htd        (502) staff       (20)    10121 2022-12-21 09:04:02.000000 NorrisUtils-1.4.1/NorrisUtils/RawUtil.py
+-rw-r--r--   0 htd        (502) staff       (20)     2755 2022-12-21 09:04:02.000000 NorrisUtils-1.4.1/NorrisUtils/RawUtils.py
+-rw-r--r--   0 htd        (502) staff       (20)     8470 2022-12-21 09:04:02.000000 NorrisUtils-1.4.1/NorrisUtils/RequestUtils.py
+-rw-r--r--   0 htd        (502) staff       (20)       20 2022-12-21 09:04:02.000000 NorrisUtils-1.4.1/NorrisUtils/__init__.py
+drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 03:18:34.996832 NorrisUtils-1.4.1/NorrisUtils.egg-info/
+-rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 03:18:34.000000 NorrisUtils-1.4.1/NorrisUtils.egg-info/PKG-INFO
+-rw-r--r--   0 htd        (502) staff       (20)      433 2024-05-08 03:18:34.000000 NorrisUtils-1.4.1/NorrisUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 htd        (502) staff       (20)        1 2024-05-08 03:18:34.000000 NorrisUtils-1.4.1/NorrisUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 htd        (502) staff       (20)       17 2024-05-08 03:18:34.000000 NorrisUtils-1.4.1/NorrisUtils.egg-info/requires.txt
+-rw-r--r--   0 htd        (502) staff       (20)       12 2024-05-08 03:18:34.000000 NorrisUtils-1.4.1/NorrisUtils.egg-info/top_level.txt
+-rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 03:18:34.997206 NorrisUtils-1.4.1/PKG-INFO
+-rw-r--r--   0 htd        (502) staff       (20)       60 2022-12-21 09:04:02.000000 NorrisUtils-1.4.1/README.md
+-rw-r--r--   0 htd        (502) staff       (20)       38 2024-05-08 03:18:34.997678 NorrisUtils-1.4.1/setup.cfg
+-rw-r--r--   0 htd        (502) staff       (20)     1256 2024-05-08 03:18:24.000000 NorrisUtils-1.4.1/setup.py
```

### Comparing `NorrisUtils-1.4.0/NorrisUtils/DingTalkGenius.py` & `NorrisUtils-1.4.1/NorrisUtils/DingTalkGenius.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.0/NorrisUtils/FileUtil.py` & `NorrisUtils-1.4.1/NorrisUtils/FileUtil.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.0/NorrisUtils/GarbageGenius.py` & `NorrisUtils-1.4.1/NorrisUtils/GarbageGenius.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.0/NorrisUtils/ImageUploadUtils.py` & `NorrisUtils-1.4.1/NorrisUtils/ImageUploadUtils.py`

 * *Files 20% similar despite different names*

```diff
@@ -39,36 +39,42 @@
             print(f"请求失败，状态码：{response.status_code}")
     except requests.RequestException as e:
         print(f"请求过程中发生错误：{e}")
 
     return None
 
 
-def upload_image_to_smms(image_path, token):
+def upload_image_to_smms(image_path, **kwargs):
     """
     使用PostImage API上传本地图片并返回图片的公网URL。
 
     :param image_path: 本地图片的路径
+    :param kwargs: 可选参数字典，可用于提供额外的选项，比如：
+                   - token: 图床token，可选。
+                   - logfunc: 日志记录函数，默认为print，用于记录发送过程中的信息，可选。
     :return: 图片的公网URL，如果失败则返回None
     """
+    kwargs.setdefault("token", "Sx3b2Rbbb0gbr5hffo6144Fxp0T0s5BG")
+    kwargs.setdefault("logfunc", print)
+    logfunc = kwargs["logfunc"]
     api_url = "https://sm.ms/api/v2/upload"
 
     # 检查图片文件是否存在
     if not os.path.exists(image_path):
-        print("图片文件不存在")
+        logfunc("图片文件不存在")
         return None
 
     compress_image(os.path.abspath(image_path), kb=5 * 1024)
     try:
         # 准备上传的文件
         with open(image_path, 'rb') as file:
             files = {'smfile': file}
 
             headers = {
-                "Authorization": "Basic " + token
+                "Authorization": "Basic " + kwargs["token"]
             }
             print(api_url)
             # 发送POST请求
             response = requests.post(api_url, files=files, headers=headers)
             print(response)
             print(response.text)
 
@@ -76,15 +82,15 @@
             if response.status_code == 200:
                 json_response = response.json()
                 if json_response.get('code') == "success":
                     return json_response['data']['url']
                 if json_response.get('code') == "image_repeated":
                     return json_response['images']
                 else:
-                    print(f"上传失败，错误信息：{json_response.get('message')}")
+                    logfunc(f"上传失败，错误信息：{json_response.get('message')}")
                     return None
             else:
-                print(f"上传请求失败，状态码：{response.status_code}")
+                logfunc(f"上传请求失败，状态码：{response.status_code}")
                 return None
     except Exception as e:
-        print(f"上传过程中发生错误：{e}")
+        logfunc(f"上传过程中发生错误：{e}")
         return None
```

### Comparing `NorrisUtils-1.4.0/NorrisUtils/RawUtil.py` & `NorrisUtils-1.4.1/NorrisUtils/RawUtil.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.0/NorrisUtils/RawUtils.py` & `NorrisUtils-1.4.1/NorrisUtils/RawUtils.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.0/NorrisUtils/RequestUtils.py` & `NorrisUtils-1.4.1/NorrisUtils/RequestUtils.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.0/NorrisUtils.egg-info/PKG-INFO` & `NorrisUtils-1.4.1/NorrisUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NorrisUtils
-Version: 1.4.0
+Version: 1.4.1
 Summary: 图床工具包，支持上传到sm.ms图床，支持发送钉钉消息
 Home-page: https://www.baidu.com
 Author: AlaricNorris
 Author-email: norris.sly@gmail.com
 Maintainer: AlaricNorris
 Maintainer-email: norris.sly@gmail.com
 License: BSD License
```

### Comparing `NorrisUtils-1.4.0/PKG-INFO` & `NorrisUtils-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NorrisUtils
-Version: 1.4.0
+Version: 1.4.1
 Summary: 图床工具包，支持上传到sm.ms图床，支持发送钉钉消息
 Home-page: https://www.baidu.com
 Author: AlaricNorris
 Author-email: norris.sly@gmail.com
 Maintainer: AlaricNorris
 Maintainer-email: norris.sly@gmail.com
 License: BSD License
```

### Comparing `NorrisUtils-1.4.0/setup.py` & `NorrisUtils-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='NorrisUtils',
-    version='1.4.0',
+    version='1.4.1',
     description=(
         '图床工具包，支持上传到sm.ms图床，支持发送钉钉消息'
     ),
     long_description=open('README.md').read(),
     author='AlaricNorris',
     author_email='norris.sly@gmail.com',
     maintainer='AlaricNorris',
```

