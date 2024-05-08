# Comparing `tmp/vnpy_rest-1.0.8.tar.gz` & `tmp/vnpy_rest-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_rest-1.0.8.tar", last modified: Mon May  6 14:00:29 2024, max compression
+gzip compressed data, was "vnpy_rest-1.0.9.tar", last modified: Wed May  8 08:26:45 2024, max compression
```

## Comparing `vnpy_rest-1.0.8.tar` & `vnpy_rest-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 14:00:29.834289 vnpy_rest-1.0.8/
--rw-rw-rw-   0        0        0     1099 2024-05-06 13:59:09.000000 vnpy_rest-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     1789 2024-05-06 14:00:29.835366 vnpy_rest-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      855 2024-05-06 13:59:26.000000 vnpy_rest-1.0.8/README.md
--rw-rw-rw-   0        0        0      988 2024-05-06 14:00:29.859688 vnpy_rest-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0       43 2022-11-14 08:31:48.000000 vnpy_rest-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 14:00:29.758672 vnpy_rest-1.0.8/vnpy_rest/
--rw-rw-rw-   0        0        0     1377 2022-12-13 08:13:01.000000 vnpy_rest-1.0.8/vnpy_rest/__init__.py
--rw-rw-rw-   0        0        0     9687 2024-05-06 13:58:07.000000 vnpy_rest-1.0.8/vnpy_rest/rest_client.py
-drwxrwxrwx   0        0        0        0 2024-05-06 14:00:29.831504 vnpy_rest-1.0.8/vnpy_rest.egg-info/
--rw-rw-rw-   0        0        0     1789 2024-05-06 14:00:29.000000 vnpy_rest-1.0.8/vnpy_rest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-05-06 14:00:29.000000 vnpy_rest-1.0.8/vnpy_rest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 14:00:29.000000 vnpy_rest-1.0.8/vnpy_rest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 14:00:29.000000 vnpy_rest-1.0.8/vnpy_rest.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-05-06 14:00:29.000000 vnpy_rest-1.0.8/vnpy_rest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-06 14:00:29.000000 vnpy_rest-1.0.8/vnpy_rest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 08:26:45.743336 vnpy_rest-1.0.9/
+-rw-rw-rw-   0        0        0     1099 2024-05-06 13:59:09.000000 vnpy_rest-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1789 2024-05-08 08:26:45.743336 vnpy_rest-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      855 2024-05-08 08:25:04.000000 vnpy_rest-1.0.9/README.md
+-rw-rw-rw-   0        0        0      988 2024-05-08 08:26:45.745016 vnpy_rest-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       43 2022-11-14 08:31:48.000000 vnpy_rest-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:26:45.708780 vnpy_rest-1.0.9/vnpy_rest/
+-rw-rw-rw-   0        0        0     1377 2022-12-13 08:13:01.000000 vnpy_rest-1.0.9/vnpy_rest/__init__.py
+-rw-rw-rw-   0        0        0     9720 2024-05-08 08:24:43.000000 vnpy_rest-1.0.9/vnpy_rest/rest_client.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:26:45.741210 vnpy_rest-1.0.9/vnpy_rest.egg-info/
+-rw-rw-rw-   0        0        0     1789 2024-05-08 08:26:45.000000 vnpy_rest-1.0.9/vnpy_rest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-05-08 08:26:45.000000 vnpy_rest-1.0.9/vnpy_rest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 08:26:45.000000 vnpy_rest-1.0.9/vnpy_rest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-08 08:26:45.000000 vnpy_rest-1.0.9/vnpy_rest.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-05-08 08:26:45.000000 vnpy_rest-1.0.9/vnpy_rest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 08:26:45.000000 vnpy_rest-1.0.9/vnpy_rest.egg-info/top_level.txt
```

### Comparing `vnpy_rest-1.0.8/LICENSE` & `vnpy_rest-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_rest-1.0.8/PKG-INFO` & `vnpy_rest-1.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_rest
-Version: 1.0.8
+Version: 1.0.9
 Summary: REST API client for vn.py quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,15 +24,15 @@
 # VeighNa框架的REST API客户端
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.8-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.9-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_rest-1.0.8/README.md` & `vnpy_rest-1.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # VeighNa框架的REST API客户端
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.8-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.9-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_rest-1.0.8/setup.cfg` & `vnpy_rest-1.0.9/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 7265 7374 0d0a 7665   = vnpy_rest..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 380d 0a75  rsion = 1.0.8..u
+00000020: 7273 696f 6e20 3d20 312e 302e 390d 0a75  rsion = 1.0.9..u
 00000030: 726c 203d 2068 7474 7073 3a2f 2f77 7777  rl = https://www
 00000040: 2e76 6e70 792e 636f 6d0d 0a6c 6963 656e  .vnpy.com..licen
 00000050: 7365 203d 204d 4954 0d0a 6175 7468 6f72  se = MIT..author
 00000060: 203d 2058 6961 6f79 6f75 2043 6865 6e0d   = Xiaoyou Chen.
 00000070: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000080: 7869 616f 796f 752e 6368 656e 406d 6169  xiaoyou.chen@mai
 00000090: 6c2e 766e 7079 2e63 6f6d 0d0a 6465 7363  l.vnpy.com..desc
```

### Comparing `vnpy_rest-1.0.8/vnpy_rest/__init__.py` & `vnpy_rest-1.0.9/vnpy_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_rest-1.0.8/vnpy_rest/rest_client.py` & `vnpy_rest-1.0.9/vnpy_rest/rest_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,17 +195,18 @@
     def request(
         self,
         method: str,
         path: str,
         params: dict = None,
         data: dict = None,
         headers: dict = None,
+        json: dict = None
     ) -> Response:
         """同步请求函数"""
-        request: Request = Request(method, path, params, data, headers)
+        request: Request = Request(method, path, params, data, json, headers)
         coro: coroutine = self._get_response(request)
         fut: Future = run_coroutine_threadsafe(coro, self.loop)
         return fut.result()
 
     def sign(self, request: Request) -> None:
         """签名函数（由用户继承实现具体签名逻辑）"""
         return request
```

### Comparing `vnpy_rest-1.0.8/vnpy_rest.egg-info/PKG-INFO` & `vnpy_rest-1.0.9/vnpy_rest.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-rest
-Version: 1.0.8
+Version: 1.0.9
 Summary: REST API client for vn.py quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,15 +24,15 @@
 # VeighNa框架的REST API客户端
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.8-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.9-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

