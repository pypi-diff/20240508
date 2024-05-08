# Comparing `tmp/migoapiclient-1.2.0.tar.gz` & `tmp/migoapiclient-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migoapiclient-1.2.0.tar", last modified: Mon May  6 01:59:13 2024, max compression
+gzip compressed data, was "migoapiclient-1.2.1.tar", last modified: Wed May  8 09:33:53 2024, max compression
```

## Comparing `migoapiclient-1.2.0.tar` & `migoapiclient-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 01:59:13.035126 migoapiclient-1.2.0/
--rw-rw-rw-   0        0        0     3900 2024-05-06 01:59:13.035126 migoapiclient-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 01:59:13.031127 migoapiclient-1.2.0/migoapiclient/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.2.0/migoapiclient/__init__.py
--rw-rw-rw-   0        0        0    12643 2024-05-06 01:59:05.000000 migoapiclient-1.2.0/migoapiclient/api_client.py
--rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.2.0/migoapiclient/file_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-06 01:59:13.034126 migoapiclient-1.2.0/migoapiclient.egg-info/
--rw-rw-rw-   0        0        0     3900 2024-05-06 01:59:12.000000 migoapiclient-1.2.0/migoapiclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-05-06 01:59:12.000000 migoapiclient-1.2.0/migoapiclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 01:59:12.000000 migoapiclient-1.2.0/migoapiclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-06 01:59:12.000000 migoapiclient-1.2.0/migoapiclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 01:59:13.035126 migoapiclient-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     3898 2024-05-06 01:59:05.000000 migoapiclient-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 01:59:13.033126 migoapiclient-1.2.0/src/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.2.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:33:53.996908 migoapiclient-1.2.1/
+-rw-rw-rw-   0        0        0     3900 2024-05-08 09:33:53.996908 migoapiclient-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 09:33:53.992907 migoapiclient-1.2.1/migoapiclient/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.2.1/migoapiclient/__init__.py
+-rw-rw-rw-   0        0        0    14171 2024-05-08 03:25:26.000000 migoapiclient-1.2.1/migoapiclient/api_client.py
+-rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.2.1/migoapiclient/file_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:33:53.995906 migoapiclient-1.2.1/migoapiclient.egg-info/
+-rw-rw-rw-   0        0        0     3900 2024-05-08 09:33:53.000000 migoapiclient-1.2.1/migoapiclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-05-08 09:33:53.000000 migoapiclient-1.2.1/migoapiclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 09:33:53.000000 migoapiclient-1.2.1/migoapiclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-08 09:33:53.000000 migoapiclient-1.2.1/migoapiclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 09:33:53.996908 migoapiclient-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     3898 2024-05-08 09:26:40.000000 migoapiclient-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:33:53.995906 migoapiclient-1.2.1/src/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.2.1/src/__init__.py
```

### Comparing `migoapiclient-1.2.0/PKG-INFO` & `migoapiclient-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.2.0
+Version: 1.2.1
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.2.0/README.md` & `migoapiclient-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.2.0/migoapiclient/api_client.py` & `migoapiclient-1.2.1/migoapiclient/api_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from datetime import datetime
 
 from dateutil.tz import tz
 from requests import Response
 
-from .file_manager import LogFileManager
+from file_manager import LogFileManager
 import time
 import requests
 
 TZ_NAME = 'Asia/Shanghai'
 ERROR_MSG = """
 ---------------------------------- {0} begin ----------------------------------
 请求URL是：{1}
@@ -185,15 +185,15 @@
             "shopId": migo_shop_id
         }
         uri = '/data-collection-service/node/refresh'
         return self.migo_try_post(self.host + uri, migo_shop_id, '刷新认证数据', json=post_data)
 
     def post_crawl_data(self, crawl_data: dict, data_type: str, migo_shop_id: str = -1):
         """
-        推送采集数据
+        推送采集数据（店铺数据）
         :param crawl_data 采集数据
         :param data_type 业务类型，订单或物流或其他
         :param migo_shop_id 店铺ID
         """
         uri = '/data-collection-service/node/save'
         # 自动修正丢失的店铺ID
         if 'shopId' not in crawl_data:
@@ -201,14 +201,47 @@
 
         if 'tableName' not in crawl_data:
             msg = '表名不能为空'
             self.post_error_log(msg, data_type, migo_shop_id, crawl_data)
             raise Exception(msg)
         return self.migo_try_post(self.host + uri, migo_shop_id, data_type + '推送采集数据', 0, json=crawl_data)
 
+    def post_third_party_data(self, crawl_data: dict, data_type: str, auth_id: str):
+        """
+        推送第三方平台数据
+        :param crawl_data 采集数据
+        :param data_type 业务类型，订单或物流或其他
+        :param auth_id 授权ID
+        """
+        uri = '/data-collection-service/node/save'
+        crawl_data['shopId'] = -1
+        if 'tableName' not in crawl_data:
+            msg = '表名不能为空'
+            self.post_error_log(msg, data_type, auth_id, crawl_data)
+            raise Exception(msg)
+        return self.migo_try_post(self.host + uri, auth_id, data_type + '推送采集数据', 0, json=crawl_data)
+
+    def get_third_party_crawl_data(self, auth_type: str, auth_id: str):
+        """
+        获取第三方平台采集数据
+        :param auth_type 授权类型
+        :param auth_id 授权ID
+        """
+        uri = '/data-collection-service/node/detail'
+        operate_name = f'获取第三方平台授权信息，授权ID为：{auth_id}'
+        post_data = {
+            'nodeConfigId': self.node_id
+        }
+        response = self.migo_try_post(self.host + uri, auth_id, operate_name, json=post_data)
+        node_data = json.loads(response['data']['nodeContext'])
+        for auth_data in node_data[auth_type]:
+            if auth_data['auth_id'] == auth_id:
+                return json.loads(auth_data['crawl_data'])
+        raise Exception(f'找不到该授权信息，授权ID是：{auth_id}')
+
     def get_heartbeat(self):
         """
         发送心跳
         """
         uri = f'/data-collection-service/node/heartbeat/{self.node_id}'
         return self.try_get(self.host + uri, error_count=0)
 
@@ -329,7 +362,8 @@
         :param msg 信息
         :param shop_id 店铺ID
         :param definition_info 策略信息
         :param log_params 其他信息
         """
         data_type = '更新调度策略失败'
         return self.post_error_log(msg, data_type, shop_id, definition_info, log_params)
+
```

### Comparing `migoapiclient-1.2.0/migoapiclient/file_manager.py` & `migoapiclient-1.2.1/migoapiclient/file_manager.py`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.2.0/migoapiclient.egg-info/PKG-INFO` & `migoapiclient-1.2.1/migoapiclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.2.0
+Version: 1.2.1
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.2.0/setup.py` & `migoapiclient-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'migoapiclient'
 DESCRIPTION = '米果请求API客户端'
 URL = 'https://github.com/me/myproject'
 EMAIL = '2920167524@qq.com'
 AUTHOR = 'pykira'
 REQUIRES_PYTHON = '>=3.5.0'
-VERSION = '1.2.0'
+VERSION = '1.2.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

