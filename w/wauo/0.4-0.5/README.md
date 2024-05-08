# Comparing `tmp/wauo-0.4.tar.gz` & `tmp/wauo-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wauo-0.4.tar", last modified: Tue May  7 15:46:30 2024, max compression
+gzip compressed data, was "wauo-0.5.tar", last modified: Wed May  8 14:17:40 2024, max compression
```

## Comparing `wauo-0.4.tar` & `wauo-0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 15:46:30.664675 wauo-0.4/
--rw-r--r--   0 wangtuo    (501) staff       (20)     1592 2024-05-07 15:46:30.664473 wauo-0.4/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)     1335 2024-04-28 13:29:40.000000 wauo-0.4/README.md
--rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-07 15:46:30.664712 wauo-0.4/setup.cfg
--rw-r--r--   0 wangtuo    (501) staff       (20)      591 2024-05-07 15:46:29.000000 wauo-0.4/setup.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 15:46:30.663268 wauo-0.4/wauo/
--rw-r--r--   0 wangtuo    (501) staff       (20)       95 2024-05-03 02:43:04.000000 wauo-0.4/wauo/__init__.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      345 2023-11-08 06:17:07.000000 wauo-0.4/wauo/exceptions.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      789 2024-05-03 11:40:02.000000 wauo-0.4/wauo/response.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     4733 2024-05-03 14:42:18.000000 wauo-0.4/wauo/spiders.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      351 2024-05-03 14:44:50.000000 wauo-0.4/wauo/test.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 15:46:30.664312 wauo-0.4/wauo.egg-info/
--rw-r--r--   0 wangtuo    (501) staff       (20)     1592 2024-05-07 15:46:30.000000 wauo-0.4/wauo.egg-info/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)      266 2024-05-07 15:46:30.000000 wauo-0.4/wauo.egg-info/SOURCES.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-07 15:46:30.000000 wauo-0.4/wauo.egg-info/dependency_links.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-07 15:46:30.000000 wauo-0.4/wauo.egg-info/not-zip-safe
--rw-r--r--   0 wangtuo    (501) staff       (20)       31 2024-05-07 15:46:30.000000 wauo-0.4/wauo.egg-info/requires.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        5 2024-05-07 15:46:30.000000 wauo-0.4/wauo.egg-info/top_level.txt
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-08 14:17:40.508250 wauo-0.5/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1592 2024-05-08 14:17:40.508051 wauo-0.5/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1335 2024-04-28 13:29:40.000000 wauo-0.5/README.md
+-rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-08 14:17:40.508287 wauo-0.5/setup.cfg
+-rw-r--r--   0 wangtuo    (501) staff       (20)      613 2024-05-08 14:17:31.000000 wauo-0.5/setup.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-08 14:17:40.507063 wauo-0.5/wauo/
+-rw-r--r--   0 wangtuo    (501) staff       (20)       95 2024-05-03 02:43:04.000000 wauo-0.5/wauo/__init__.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      345 2023-11-08 06:17:07.000000 wauo-0.5/wauo/exceptions.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      789 2024-05-03 11:40:02.000000 wauo-0.5/wauo/response.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     5228 2024-05-08 14:14:02.000000 wauo-0.5/wauo/spiders.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      351 2024-05-03 14:44:50.000000 wauo-0.5/wauo/test.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-08 14:17:40.507904 wauo-0.5/wauo.egg-info/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1592 2024-05-08 14:17:40.000000 wauo-0.5/wauo.egg-info/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)      266 2024-05-08 14:17:40.000000 wauo-0.5/wauo.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-08 14:17:40.000000 wauo-0.5/wauo.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-08 14:17:40.000000 wauo-0.5/wauo.egg-info/not-zip-safe
+-rw-r--r--   0 wangtuo    (501) staff       (20)       31 2024-05-08 14:17:40.000000 wauo-0.5/wauo.egg-info/requires.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        5 2024-05-08 14:17:40.000000 wauo-0.5/wauo.egg-info/top_level.txt
```

### Comparing `wauo-0.4/PKG-INFO` & `wauo-0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wauo
-Version: 0.4
+Version: 0.5
 Summary: 爬虫者的贴心助手
 Home-page: https://github.com/markadc/wauo
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: python,requests,spider
 Description-Content-Type: text/markdown
```

### Comparing `wauo-0.4/README.md` & `wauo-0.5/README.md`

 * *Files identical despite different names*

### Comparing `wauo-0.4/wauo/response.py` & `wauo-0.5/wauo/response.py`

 * *Files identical despite different names*

### Comparing `wauo-0.4/wauo/spiders.py` & `wauo-0.5/wauo/spiders.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 
+import base64
 import hashlib
 import os
 import random
 import string
 import time
+import uuid
 from datetime import datetime
 from typing import Callable
 
 import requests
 from fake_useragent import UserAgent
 from loguru import logger
 
@@ -16,14 +18,32 @@
 from wauo.response import Response
 
 
 class SpiderTools:
     """爬虫工具"""
 
     @staticmethod
+    def get_uuid():
+        """获取uuid"""
+        uuid4 = str(uuid.uuid4())
+        return uuid4
+
+    @staticmethod
+    def b64_encode(s: str):
+        """base64加密"""
+        encode_value = base64.b64encode(s.encode('utf-8')).decode('utf-8')
+        return encode_value
+
+    @staticmethod
+    def b64_decode(s: str):
+        """base64解密"""
+        decode_value = base64.b64decode(s).decode('utf-8')
+        return decode_value
+
+    @staticmethod
     def make_str(leng=9):
         """获取随机字符串，a-zA-Z0-9"""
         s = "".join(random.sample(string.ascii_letters + string.digits, leng))
         return s
 
     @staticmethod
     def make_md5(s: str) -> str:
@@ -112,15 +132,15 @@
 
     @retry
     def send(
             self, url: str, headers: dict = None, proxies: dict = None, timeout=3,
             data: dict = None, json: dict = None,
             cookie: str = None, codes: list = None, checker: Callable = None,
             **kwargs
-    ):
+    ) -> Response:
         """
         发送请求，获取响应。默认为GET请求，如果传入了data或者json参数则为POST请求。
         """
         proxies = proxies or self.get_proxies()
         headers = headers or self.get_headers()
         headers.setdefault('User-Agent', self.ua.random)
         if cookie:
```

### Comparing `wauo-0.4/wauo.egg-info/PKG-INFO` & `wauo-0.5/wauo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wauo
-Version: 0.4
+Version: 0.5
 Summary: 爬虫者的贴心助手
 Home-page: https://github.com/markadc/wauo
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: python,requests,spider
 Description-Content-Type: text/markdown
```

