# Comparing `tmp/NorrisUtils-1.4.5.tar.gz` & `tmp/NorrisUtils-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NorrisUtils-1.4.5.tar", last modified: Wed May  8 05:50:29 2024, max compression
+gzip compressed data, was "NorrisUtils-1.4.6.tar", last modified: Wed May  8 06:26:04 2024, max compression
```

## Comparing `NorrisUtils-1.4.5.tar` & `NorrisUtils-1.4.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 05:50:29.267731 NorrisUtils-1.4.5/
-drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 05:50:29.265034 NorrisUtils-1.4.5/NorrisUtils/
--rw-r--r--   0 htd        (502) staff       (20)       42 2022-12-21 09:04:02.000000 NorrisUtils-1.4.5/NorrisUtils/BuildConfig.py
--rw-r--r--   0 htd        (502) staff       (20)    12595 2024-05-08 05:49:26.000000 NorrisUtils-1.4.5/NorrisUtils/DingTalkGenius.py
--rw-r--r--   0 htd        (502) staff       (20)     5581 2023-10-17 09:11:02.000000 NorrisUtils-1.4.5/NorrisUtils/FileUtil.py
--rw-r--r--   0 htd        (502) staff       (20)     1392 2022-12-21 09:04:02.000000 NorrisUtils-1.4.5/NorrisUtils/GarbageGenius.py
--rw-r--r--   0 htd        (502) staff       (20)     3351 2024-05-08 03:17:50.000000 NorrisUtils-1.4.5/NorrisUtils/ImageUploadUtils.py
--rw-r--r--   0 htd        (502) staff       (20)    10121 2022-12-21 09:04:02.000000 NorrisUtils-1.4.5/NorrisUtils/RawUtil.py
--rw-r--r--   0 htd        (502) staff       (20)     2755 2022-12-21 09:04:02.000000 NorrisUtils-1.4.5/NorrisUtils/RawUtils.py
--rw-r--r--   0 htd        (502) staff       (20)     8470 2022-12-21 09:04:02.000000 NorrisUtils-1.4.5/NorrisUtils/RequestUtils.py
--rw-r--r--   0 htd        (502) staff       (20)       20 2022-12-21 09:04:02.000000 NorrisUtils-1.4.5/NorrisUtils/__init__.py
-drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 05:50:29.267031 NorrisUtils-1.4.5/NorrisUtils.egg-info/
--rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 05:50:29.000000 NorrisUtils-1.4.5/NorrisUtils.egg-info/PKG-INFO
--rw-r--r--   0 htd        (502) staff       (20)      433 2024-05-08 05:50:29.000000 NorrisUtils-1.4.5/NorrisUtils.egg-info/SOURCES.txt
--rw-r--r--   0 htd        (502) staff       (20)        1 2024-05-08 05:50:29.000000 NorrisUtils-1.4.5/NorrisUtils.egg-info/dependency_links.txt
--rw-r--r--   0 htd        (502) staff       (20)       17 2024-05-08 05:50:29.000000 NorrisUtils-1.4.5/NorrisUtils.egg-info/requires.txt
--rw-r--r--   0 htd        (502) staff       (20)       12 2024-05-08 05:50:29.000000 NorrisUtils-1.4.5/NorrisUtils.egg-info/top_level.txt
--rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 05:50:29.267394 NorrisUtils-1.4.5/PKG-INFO
--rw-r--r--   0 htd        (502) staff       (20)       60 2022-12-21 09:04:02.000000 NorrisUtils-1.4.5/README.md
--rw-r--r--   0 htd        (502) staff       (20)       38 2024-05-08 05:50:29.267817 NorrisUtils-1.4.5/setup.cfg
--rw-r--r--   0 htd        (502) staff       (20)     1256 2024-05-08 05:50:24.000000 NorrisUtils-1.4.5/setup.py
+drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 06:26:04.602480 NorrisUtils-1.4.6/
+drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 06:26:04.599652 NorrisUtils-1.4.6/NorrisUtils/
+-rw-r--r--   0 htd        (502) staff       (20)       42 2022-12-21 09:04:02.000000 NorrisUtils-1.4.6/NorrisUtils/BuildConfig.py
+-rw-r--r--   0 htd        (502) staff       (20)    12658 2024-05-08 06:25:19.000000 NorrisUtils-1.4.6/NorrisUtils/DingTalkGenius.py
+-rw-r--r--   0 htd        (502) staff       (20)     5581 2023-10-17 09:11:02.000000 NorrisUtils-1.4.6/NorrisUtils/FileUtil.py
+-rw-r--r--   0 htd        (502) staff       (20)     1392 2022-12-21 09:04:02.000000 NorrisUtils-1.4.6/NorrisUtils/GarbageGenius.py
+-rw-r--r--   0 htd        (502) staff       (20)     3351 2024-05-08 03:17:50.000000 NorrisUtils-1.4.6/NorrisUtils/ImageUploadUtils.py
+-rw-r--r--   0 htd        (502) staff       (20)    10121 2022-12-21 09:04:02.000000 NorrisUtils-1.4.6/NorrisUtils/RawUtil.py
+-rw-r--r--   0 htd        (502) staff       (20)     2755 2022-12-21 09:04:02.000000 NorrisUtils-1.4.6/NorrisUtils/RawUtils.py
+-rw-r--r--   0 htd        (502) staff       (20)     8470 2022-12-21 09:04:02.000000 NorrisUtils-1.4.6/NorrisUtils/RequestUtils.py
+-rw-r--r--   0 htd        (502) staff       (20)       20 2022-12-21 09:04:02.000000 NorrisUtils-1.4.6/NorrisUtils/__init__.py
+drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 06:26:04.601548 NorrisUtils-1.4.6/NorrisUtils.egg-info/
+-rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 06:26:04.000000 NorrisUtils-1.4.6/NorrisUtils.egg-info/PKG-INFO
+-rw-r--r--   0 htd        (502) staff       (20)      433 2024-05-08 06:26:04.000000 NorrisUtils-1.4.6/NorrisUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 htd        (502) staff       (20)        1 2024-05-08 06:26:04.000000 NorrisUtils-1.4.6/NorrisUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 htd        (502) staff       (20)       17 2024-05-08 06:26:04.000000 NorrisUtils-1.4.6/NorrisUtils.egg-info/requires.txt
+-rw-r--r--   0 htd        (502) staff       (20)       12 2024-05-08 06:26:04.000000 NorrisUtils-1.4.6/NorrisUtils.egg-info/top_level.txt
+-rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 06:26:04.601956 NorrisUtils-1.4.6/PKG-INFO
+-rw-r--r--   0 htd        (502) staff       (20)       60 2022-12-21 09:04:02.000000 NorrisUtils-1.4.6/README.md
+-rw-r--r--   0 htd        (502) staff       (20)       38 2024-05-08 06:26:04.602710 NorrisUtils-1.4.6/setup.cfg
+-rw-r--r--   0 htd        (502) staff       (20)     1256 2024-05-08 06:26:01.000000 NorrisUtils-1.4.6/setup.py
```

### Comparing `NorrisUtils-1.4.5/NorrisUtils/DingTalkGenius.py` & `NorrisUtils-1.4.6/NorrisUtils/DingTalkGenius.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,28 +256,29 @@
             token=kwargs["token"]
         )
     if image_url is None or image_url == "":
         logfunc("未能成功上传图片，请检查！")
         if callback:
             callback()
         return False
-    markdown = f"阿斯顿法师打发![image]({image_url})"
-    # 构建请求数据，采用JSON格式封装文本消息
-    data = {
-        "msgtype": "markdown",
-        "at": {
-            "isAtAll": kwargs["isAtAll"],
-            "atMobiles": kwargs["atMobiles"],
-        },
-        "markdown": {
-            "title": "图片",
-            "text": markdown
-        }
-    }
-    return send_to_dingtalk(
+    markdown = f"markdown图片![image]({image_url})"
+    # # 构建请求数据，采用JSON格式封装文本消息
+    # data = {
+    #     "msgtype": "markdown",
+    #     "at": {
+    #         "isAtAll": kwargs["isAtAll"],
+    #         "atMobiles": kwargs["atMobiles"],
+    #     },
+    #     "markdown": {
+    #         "title": "图片",
+    #         "text": markdown
+    #     }
+    # }
+    return send_dingtalk_markdown(
         url_webhook,
         secret=kwargs["secret"],
         atMobiles=kwargs["atMobiles"],
         isAtAll=kwargs["isAtAll"],
-        data=data,
+        title="markdown图片",
+        markdown=markdown,
     )
```

### Comparing `NorrisUtils-1.4.5/NorrisUtils/FileUtil.py` & `NorrisUtils-1.4.6/NorrisUtils/FileUtil.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.5/NorrisUtils/GarbageGenius.py` & `NorrisUtils-1.4.6/NorrisUtils/GarbageGenius.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.5/NorrisUtils/ImageUploadUtils.py` & `NorrisUtils-1.4.6/NorrisUtils/ImageUploadUtils.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.5/NorrisUtils/RawUtil.py` & `NorrisUtils-1.4.6/NorrisUtils/RawUtil.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.5/NorrisUtils/RawUtils.py` & `NorrisUtils-1.4.6/NorrisUtils/RawUtils.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.5/NorrisUtils/RequestUtils.py` & `NorrisUtils-1.4.6/NorrisUtils/RequestUtils.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.5/NorrisUtils.egg-info/PKG-INFO` & `NorrisUtils-1.4.6/NorrisUtils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NorrisUtils
-Version: 1.4.5
+Version: 1.4.6
 Summary: 图床工具包，支持上传到sm.ms图床，支持发送钉钉消息
 Home-page: https://www.baidu.com
 Author: AlaricNorris
 Author-email: norris.sly@gmail.com
 Maintainer: AlaricNorris
 Maintainer-email: norris.sly@gmail.com
 License: BSD License
```

### Comparing `NorrisUtils-1.4.5/PKG-INFO` & `NorrisUtils-1.4.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NorrisUtils
-Version: 1.4.5
+Version: 1.4.6
 Summary: 图床工具包，支持上传到sm.ms图床，支持发送钉钉消息
 Home-page: https://www.baidu.com
 Author: AlaricNorris
 Author-email: norris.sly@gmail.com
 Maintainer: AlaricNorris
 Maintainer-email: norris.sly@gmail.com
 License: BSD License
```

### Comparing `NorrisUtils-1.4.5/setup.py` & `NorrisUtils-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='NorrisUtils',
-    version='1.4.5',
+    version='1.4.6',
     description=(
         '图床工具包，支持上传到sm.ms图床，支持发送钉钉消息'
     ),
     long_description=open('README.md').read(),
     author='AlaricNorris',
     author_email='norris.sly@gmail.com',
     maintainer='AlaricNorris',
```

