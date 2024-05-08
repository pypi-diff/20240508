# Comparing `tmp/sparkproxy-0.4.3.tar.gz` & `tmp/sparkproxy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkproxy-0.4.3.tar", last modified: Tue Apr 16 14:03:00 2024, max compression
+gzip compressed data, was "sparkproxy-1.0.0.tar", last modified: Wed May  8 11:04:28 2024, max compression
```

## Comparing `sparkproxy-0.4.3.tar` & `sparkproxy-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-16 14:03:00.533330 sparkproxy-0.4.3/
--rw-r--r--   0 huanghy    (501) staff       (20)     1063 2024-04-09 02:02:16.000000 sparkproxy-0.4.3/LICENSE
--rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-16 14:03:00.533170 sparkproxy-0.4.3/PKG-INFO
--rw-r--r--   0 huanghy    (501) staff       (20)     4831 2024-04-11 07:31:06.000000 sparkproxy-0.4.3/README.md
--rw-r--r--   0 huanghy    (501) staff       (20)       38 2024-04-16 14:03:00.533376 sparkproxy-0.4.3/setup.cfg
--rw-r--r--   0 huanghy    (501) staff       (20)     2362 2024-04-09 03:18:58.000000 sparkproxy-0.4.3/setup.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-16 14:03:00.529661 sparkproxy-0.4.3/sparkproxy/
--rw-r--r--   0 huanghy    (501) staff       (20)      346 2024-04-16 13:53:34.000000 sparkproxy-0.4.3/sparkproxy/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     3098 2024-04-10 04:59:43.000000 sparkproxy-0.4.3/sparkproxy/auth.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1666 2024-04-08 13:34:09.000000 sparkproxy-0.4.3/sparkproxy/compat.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1341 2024-04-16 14:01:23.000000 sparkproxy-0.4.3/sparkproxy/config.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-16 14:03:00.531231 sparkproxy-0.4.3/sparkproxy/http/
--rw-r--r--   0 huanghy    (501) staff       (20)     3137 2024-04-10 05:00:18.000000 sparkproxy-0.4.3/sparkproxy/http/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     5000 2024-04-08 13:48:17.000000 sparkproxy-0.4.3/sparkproxy/http/client.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-16 14:03:00.532183 sparkproxy-0.4.3/sparkproxy/http/middleware/
--rw-r--r--   0 huanghy    (501) staff       (20)      246 2024-04-08 13:34:09.000000 sparkproxy-0.4.3/sparkproxy/http/middleware/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)      875 2024-04-08 13:34:09.000000 sparkproxy-0.4.3/sparkproxy/http/middleware/base.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2611 2024-04-08 13:48:17.000000 sparkproxy-0.4.3/sparkproxy/http/middleware/retry_domains.py
--rw-r--r--   0 huanghy    (501) staff       (20)      608 2024-04-08 15:18:23.000000 sparkproxy-0.4.3/sparkproxy/http/middleware/ua.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2520 2024-04-08 15:21:24.000000 sparkproxy-0.4.3/sparkproxy/http/response.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2973 2024-04-10 05:09:23.000000 sparkproxy-0.4.3/sparkproxy/rsa.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-16 14:03:00.532516 sparkproxy-0.4.3/sparkproxy/services/
--rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.4.3/sparkproxy/services/__init__.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-16 14:03:00.532726 sparkproxy-0.4.3/sparkproxy/services/openapi/
--rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.4.3/sparkproxy/services/openapi/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     8299 2024-04-16 13:58:07.000000 sparkproxy-0.4.3/sparkproxy/services/openapi/client.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-16 14:03:00.530610 sparkproxy-0.4.3/sparkproxy.egg-info/
--rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-16 14:03:00.000000 sparkproxy-0.4.3/sparkproxy.egg-info/PKG-INFO
--rw-r--r--   0 huanghy    (501) staff       (20)      677 2024-04-16 14:03:00.000000 sparkproxy-0.4.3/sparkproxy.egg-info/SOURCES.txt
--rw-r--r--   0 huanghy    (501) staff       (20)        1 2024-04-16 14:03:00.000000 sparkproxy-0.4.3/sparkproxy.egg-info/dependency_links.txt
--rw-r--r--   0 huanghy    (501) staff       (20)       54 2024-04-16 14:03:00.000000 sparkproxy-0.4.3/sparkproxy.egg-info/entry_points.txt
--rw-r--r--   0 huanghy    (501) staff       (20)      209 2024-04-16 14:03:00.000000 sparkproxy-0.4.3/sparkproxy.egg-info/requires.txt
--rw-r--r--   0 huanghy    (501) staff       (20)       11 2024-04-16 14:03:00.000000 sparkproxy-0.4.3/sparkproxy.egg-info/top_level.txt
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-05-08 11:04:28.541839 sparkproxy-1.0.0/
+-rw-r--r--   0 huanghy    (501) staff       (20)     1063 2024-04-09 02:02:16.000000 sparkproxy-1.0.0/LICENSE
+-rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-05-08 11:04:28.541706 sparkproxy-1.0.0/PKG-INFO
+-rw-r--r--   0 huanghy    (501) staff       (20)     4971 2024-05-08 11:04:25.000000 sparkproxy-1.0.0/README.md
+-rw-r--r--   0 huanghy    (501) staff       (20)       38 2024-05-08 11:04:28.541880 sparkproxy-1.0.0/setup.cfg
+-rw-r--r--   0 huanghy    (501) staff       (20)     2362 2024-04-09 03:18:58.000000 sparkproxy-1.0.0/setup.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-05-08 11:04:28.538149 sparkproxy-1.0.0/sparkproxy/
+-rw-r--r--   0 huanghy    (501) staff       (20)      346 2024-05-08 11:03:37.000000 sparkproxy-1.0.0/sparkproxy/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     3098 2024-04-10 04:59:43.000000 sparkproxy-1.0.0/sparkproxy/auth.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1666 2024-04-08 13:34:09.000000 sparkproxy-1.0.0/sparkproxy/compat.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1323 2024-05-08 10:59:54.000000 sparkproxy-1.0.0/sparkproxy/config.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-05-08 11:04:28.539636 sparkproxy-1.0.0/sparkproxy/http/
+-rw-r--r--   0 huanghy    (501) staff       (20)     3137 2024-04-10 05:00:18.000000 sparkproxy-1.0.0/sparkproxy/http/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     5000 2024-04-08 13:48:17.000000 sparkproxy-1.0.0/sparkproxy/http/client.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-05-08 11:04:28.540642 sparkproxy-1.0.0/sparkproxy/http/middleware/
+-rw-r--r--   0 huanghy    (501) staff       (20)      246 2024-04-08 13:34:09.000000 sparkproxy-1.0.0/sparkproxy/http/middleware/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)      875 2024-04-08 13:34:09.000000 sparkproxy-1.0.0/sparkproxy/http/middleware/base.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2611 2024-04-08 13:48:17.000000 sparkproxy-1.0.0/sparkproxy/http/middleware/retry_domains.py
+-rw-r--r--   0 huanghy    (501) staff       (20)      608 2024-04-08 15:18:23.000000 sparkproxy-1.0.0/sparkproxy/http/middleware/ua.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2520 2024-04-08 15:21:24.000000 sparkproxy-1.0.0/sparkproxy/http/response.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2973 2024-04-10 05:09:23.000000 sparkproxy-1.0.0/sparkproxy/rsa.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-05-08 11:04:28.541067 sparkproxy-1.0.0/sparkproxy/services/
+-rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-1.0.0/sparkproxy/services/__init__.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-05-08 11:04:28.541242 sparkproxy-1.0.0/sparkproxy/services/openapi/
+-rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-1.0.0/sparkproxy/services/openapi/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     8299 2024-04-16 13:58:07.000000 sparkproxy-1.0.0/sparkproxy/services/openapi/client.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-05-08 11:04:28.538955 sparkproxy-1.0.0/sparkproxy.egg-info/
+-rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-05-08 11:04:28.000000 sparkproxy-1.0.0/sparkproxy.egg-info/PKG-INFO
+-rw-r--r--   0 huanghy    (501) staff       (20)      677 2024-05-08 11:04:28.000000 sparkproxy-1.0.0/sparkproxy.egg-info/SOURCES.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)        1 2024-05-08 11:04:28.000000 sparkproxy-1.0.0/sparkproxy.egg-info/dependency_links.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)       54 2024-05-08 11:04:28.000000 sparkproxy-1.0.0/sparkproxy.egg-info/entry_points.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)      209 2024-05-08 11:04:28.000000 sparkproxy-1.0.0/sparkproxy.egg-info/requires.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)       11 2024-05-08 11:04:28.000000 sparkproxy-1.0.0/sparkproxy.egg-info/top_level.txt
```

### Comparing `sparkproxy-0.4.3/LICENSE` & `sparkproxy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.3/PKG-INFO` & `sparkproxy-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkproxy
-Version: 0.4.3
+Version: 1.0.0
 Summary: Spark proxy OpenApi SDK
 Home-page: https://github.com/yungoo/spark-sdk-python
 Author: Spark Proxy Co., Ltd.
 Author-email: sdk@sparkproxy.com
 Maintainer-email: support@sparkproxy.com
 License: MIT
 Platform: any
```

### Comparing `sparkproxy-0.4.3/README.md` & `sparkproxy-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,50 +13,52 @@
 $ pip install sparkproxy
 ```
 
 ## 运行环境
 
 | sparkproxy SDK版本 |              Python 版本               |
 |:----------------:| :------------------------------------: |
-|       0.x        | 2.7, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9 |
+|      1.0.0       | 2.7, 3.3, 3.4, 3.5, 3.6, 3.7, 3.8, 3.9 |
 
 ## 使用方法
 
 ### 检查接口是否已经配置好
 
 ```python
 from sparkproxy import Auth
 from sparkproxy import SparkProxyClient
+from sparkproxy.config import SANDBOX_API_HOST
 
 supplier_no = 'test0001'
 with open("key.pem", 'rb') as pem_file:
     private_key = pem_file.read()
 with open("spark.pub", 'rb') as pem_file:
     rsa_public_key = pem_file.read()
-client = SparkProxyClient(Auth(supplier_no=supplier_no, private_key=private_key, public_key=rsa_public_key))
+client = SparkProxyClient(Auth(supplier_no=supplier_no, private_key=private_key, public_key=rsa_public_key), host=SANDBOX_API_HOST)
 
 # 获取订单&实例信息
 ret, info = client.check_available()
 print(ret)
 print(info)
 ```
 
 ### 调用sparkproxy的开放接口
 
 ```python
 from sparkproxy import Auth
 from sparkproxy import SparkProxyClient
+from sparkproxy.config import SANDBOX_API_HOST
 
 # 双方协商的商户号
 supplier_no = 'test0001'
 
 # 使用私钥对请求签名（认证）, 生成方式参考 [examples示例](https://github.com/yungoo/spark-sdk-python/tree/master/examples/genrsa.py)。
 with open("key.pem", 'rb') as pem_file:
     private_key = pem_file.read()
-client = SparkProxyClient(Auth(supplier_no=supplier_no, private_key=private_key))
+client = SparkProxyClient(Auth(supplier_no=supplier_no, private_key=private_key), host=SANDBOX_API_HOST)
 
 ret, info = client.get_product_stock(proxy_type=103)
 if ret is not None:
     print('All is OK')
 else:
     print(info) # error message in info
 ```
```

### Comparing `sparkproxy-0.4.3/setup.py` & `sparkproxy-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.3/sparkproxy/auth.py` & `sparkproxy-1.0.0/sparkproxy/auth.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.3/sparkproxy/compat.py` & `sparkproxy-1.0.0/sparkproxy/compat.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.3/sparkproxy/config.py` & `sparkproxy-1.0.0/sparkproxy/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
-API_HOST = 'http://8.130.48.76:16801'  # 数据处理操作Host
-# API_HOST = 'http://127.0.0.1:8080'  # 数据处理操作Host
+SANDBOX_API_HOST = 'http://8.130.48.76:16801'
+PRODUCTION_API_HOST = 'https://oapi.sparkproxy.com'
 
 _config = {
-    'default_api_host': API_HOST,
+    'default_api_host': PRODUCTION_API_HOST,
     'connection_timeout': 30,  # 链接超时为时间为30s
     'connection_retries': 3,  # 链接重试次数为3次
     'connection_pool': 10  # 链接池个数为10
 }
 
 _is_customized_default = {
     'default_api_host': False,
```

### Comparing `sparkproxy-0.4.3/sparkproxy/http/__init__.py` & `sparkproxy-1.0.0/sparkproxy/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.3/sparkproxy/http/client.py` & `sparkproxy-1.0.0/sparkproxy/http/client.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.3/sparkproxy/http/middleware/base.py` & `sparkproxy-1.0.0/sparkproxy/http/middleware/base.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.3/sparkproxy/http/middleware/retry_domains.py` & `sparkproxy-1.0.0/sparkproxy/http/middleware/retry_domains.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.3/sparkproxy/http/middleware/ua.py` & `sparkproxy-1.0.0/sparkproxy/http/middleware/ua.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.3/sparkproxy/http/response.py` & `sparkproxy-1.0.0/sparkproxy/http/response.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.3/sparkproxy/rsa.py` & `sparkproxy-1.0.0/sparkproxy/rsa.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.3/sparkproxy/services/openapi/client.py` & `sparkproxy-1.0.0/sparkproxy/services/openapi/client.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.3/sparkproxy.egg-info/PKG-INFO` & `sparkproxy-1.0.0/sparkproxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkproxy
-Version: 0.4.3
+Version: 1.0.0
 Summary: Spark proxy OpenApi SDK
 Home-page: https://github.com/yungoo/spark-sdk-python
 Author: Spark Proxy Co., Ltd.
 Author-email: sdk@sparkproxy.com
 Maintainer-email: support@sparkproxy.com
 License: MIT
 Platform: any
```

### Comparing `sparkproxy-0.4.3/sparkproxy.egg-info/SOURCES.txt` & `sparkproxy-1.0.0/sparkproxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

