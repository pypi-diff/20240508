# Comparing `tmp/cjops-1.0.3.tar.gz` & `tmp/cjops-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjops-1.0.3.tar", last modified: Wed May  8 00:50:08 2024, max compression
+gzip compressed data, was "cjops-1.0.4.tar", last modified: Wed May  8 03:15:09 2024, max compression
```

## Comparing `cjops-1.0.3.tar` & `cjops-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 00:50:08.239874 cjops-1.0.3/
--rw-r--r--   0 caojie     (501) staff       (20)     1068 2024-03-15 01:36:01.000000 cjops-1.0.3/LICENSE
--rw-r--r--   0 caojie     (501) staff       (20)     2179 2024-05-08 00:50:08.239314 cjops-1.0.3/PKG-INFO
--rw-r--r--   0 caojie     (501) staff       (20)     1483 2024-04-25 10:03:23.000000 cjops-1.0.3/README.md
--rw-r--r--   0 caojie     (501) staff       (20)       38 2024-05-08 00:50:08.240064 cjops-1.0.3/setup.cfg
--rw-r--r--   0 caojie     (501) staff       (20)     2874 2024-05-07 08:48:04.000000 cjops-1.0.3/setup.py
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 00:50:08.225489 cjops-1.0.3/src/
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 00:50:08.234413 cjops-1.0.3/src/cjops/
--rw-r--r--   0 caojie     (501) staff       (20)      200 2024-05-08 00:48:52.000000 cjops-1.0.3/src/cjops/__init__.py
--rw-r--r--   0 caojie     (501) staff       (20)      333 2024-05-08 00:49:57.000000 cjops-1.0.3/src/cjops/__version__.py
--rw-r--r--   0 caojie     (501) staff       (20)     4488 2024-05-08 00:48:52.000000 cjops-1.0.3/src/cjops/aliyun.py
--rw-r--r--   0 caojie     (501) staff       (20)     2157 2024-04-15 06:29:32.000000 cjops-1.0.3/src/cjops/command.py
--rw-r--r--   0 caojie     (501) staff       (20)     4791 2024-05-07 07:49:15.000000 cjops-1.0.3/src/cjops/domain.py
--rw-r--r--   0 caojie     (501) staff       (20)     1795 2024-04-19 07:29:32.000000 cjops-1.0.3/src/cjops/email.py
--rw-r--r--   0 caojie     (501) staff       (20)     8459 2024-04-25 02:58:56.000000 cjops-1.0.3/src/cjops/excel.py
--rw-r--r--   0 caojie     (501) staff       (20)      127 2024-05-08 00:48:52.000000 cjops-1.0.3/src/cjops/info.py
--rw-r--r--   0 caojie     (501) staff       (20)      870 2024-04-12 07:35:23.000000 cjops-1.0.3/src/cjops/qw.py
--rw-r--r--   0 caojie     (501) staff       (20)     1411 2024-04-19 08:45:16.000000 cjops-1.0.3/src/cjops/sql.py
--rw-r--r--   0 caojie     (501) staff       (20)     2078 2024-05-07 09:24:16.000000 cjops-1.0.3/src/cjops/time.py
--rw-r--r--   0 caojie     (501) staff       (20)     6456 2024-05-07 07:55:52.000000 cjops-1.0.3/src/cjops/utils.py
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 00:50:08.238469 cjops-1.0.3/src/cjops.egg-info/
--rw-r--r--   0 caojie     (501) staff       (20)     2179 2024-05-08 00:50:08.000000 cjops-1.0.3/src/cjops.egg-info/PKG-INFO
--rw-r--r--   0 caojie     (501) staff       (20)      456 2024-05-08 00:50:08.000000 cjops-1.0.3/src/cjops.egg-info/SOURCES.txt
--rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-08 00:50:08.000000 cjops-1.0.3/src/cjops.egg-info/dependency_links.txt
--rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-07 08:48:08.000000 cjops-1.0.3/src/cjops.egg-info/not-zip-safe
--rw-r--r--   0 caojie     (501) staff       (20)      146 2024-05-08 00:50:08.000000 cjops-1.0.3/src/cjops.egg-info/requires.txt
--rw-r--r--   0 caojie     (501) staff       (20)        6 2024-05-08 00:50:08.000000 cjops-1.0.3/src/cjops.egg-info/top_level.txt
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 03:15:09.672115 cjops-1.0.4/
+-rw-r--r--   0 caojie     (501) staff       (20)     1068 2024-03-15 01:36:01.000000 cjops-1.0.4/LICENSE
+-rw-r--r--   0 caojie     (501) staff       (20)     2179 2024-05-08 03:15:09.671526 cjops-1.0.4/PKG-INFO
+-rw-r--r--   0 caojie     (501) staff       (20)     1483 2024-04-25 10:03:23.000000 cjops-1.0.4/README.md
+-rw-r--r--   0 caojie     (501) staff       (20)       38 2024-05-08 03:15:09.672238 cjops-1.0.4/setup.cfg
+-rw-r--r--   0 caojie     (501) staff       (20)     2874 2024-05-07 08:48:04.000000 cjops-1.0.4/setup.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 03:15:09.656712 cjops-1.0.4/src/
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 03:15:09.666446 cjops-1.0.4/src/cjops/
+-rw-r--r--   0 caojie     (501) staff       (20)      200 2024-05-08 00:48:52.000000 cjops-1.0.4/src/cjops/__init__.py
+-rw-r--r--   0 caojie     (501) staff       (20)      333 2024-05-08 03:14:58.000000 cjops-1.0.4/src/cjops/__version__.py
+-rw-r--r--   0 caojie     (501) staff       (20)     4608 2024-05-08 03:14:13.000000 cjops-1.0.4/src/cjops/aliyun.py
+-rw-r--r--   0 caojie     (501) staff       (20)     2157 2024-04-15 06:29:32.000000 cjops-1.0.4/src/cjops/command.py
+-rw-r--r--   0 caojie     (501) staff       (20)     4791 2024-05-07 07:49:15.000000 cjops-1.0.4/src/cjops/domain.py
+-rw-r--r--   0 caojie     (501) staff       (20)     1795 2024-04-19 07:29:32.000000 cjops-1.0.4/src/cjops/email.py
+-rw-r--r--   0 caojie     (501) staff       (20)     8459 2024-04-25 02:58:56.000000 cjops-1.0.4/src/cjops/excel.py
+-rw-r--r--   0 caojie     (501) staff       (20)      127 2024-05-08 00:48:52.000000 cjops-1.0.4/src/cjops/info.py
+-rw-r--r--   0 caojie     (501) staff       (20)      870 2024-04-12 07:35:23.000000 cjops-1.0.4/src/cjops/qw.py
+-rw-r--r--   0 caojie     (501) staff       (20)     1411 2024-04-19 08:45:16.000000 cjops-1.0.4/src/cjops/sql.py
+-rw-r--r--   0 caojie     (501) staff       (20)     2078 2024-05-07 09:24:16.000000 cjops-1.0.4/src/cjops/time.py
+-rw-r--r--   0 caojie     (501) staff       (20)     6456 2024-05-07 07:55:52.000000 cjops-1.0.4/src/cjops/utils.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 03:15:09.670627 cjops-1.0.4/src/cjops.egg-info/
+-rw-r--r--   0 caojie     (501) staff       (20)     2179 2024-05-08 03:15:09.000000 cjops-1.0.4/src/cjops.egg-info/PKG-INFO
+-rw-r--r--   0 caojie     (501) staff       (20)      456 2024-05-08 03:15:09.000000 cjops-1.0.4/src/cjops.egg-info/SOURCES.txt
+-rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-08 03:15:09.000000 cjops-1.0.4/src/cjops.egg-info/dependency_links.txt
+-rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-07 08:48:08.000000 cjops-1.0.4/src/cjops.egg-info/not-zip-safe
+-rw-r--r--   0 caojie     (501) staff       (20)      146 2024-05-08 03:15:09.000000 cjops-1.0.4/src/cjops.egg-info/requires.txt
+-rw-r--r--   0 caojie     (501) staff       (20)        6 2024-05-08 03:15:09.000000 cjops-1.0.4/src/cjops.egg-info/top_level.txt
```

### Comparing `cjops-1.0.3/LICENSE` & `cjops-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cjops-1.0.3/PKG-INFO` & `cjops-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjops
-Version: 1.0.3
+Version: 1.0.4
 Summary: cj ops.
 Author: chenxing
 Author-email: chenxing@cjdropshipping.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
```

### Comparing `cjops-1.0.3/README.md` & `cjops-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cjops-1.0.3/setup.py` & `cjops-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.3/src/cjops/aliyun.py` & `cjops-1.0.4/src/cjops/aliyun.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             raise Exception(f"密钥格式不正确: {e}")
 
         access_key_id = cipher_suite.decrypt(encryption_account.get('access_key_id').encode('utf-8')).decode('utf-8')
         access_key_secret = cipher_suite.decrypt(encryption_account.get('access_key_secret').encode('utf-8')).decode('utf-8')
 
         return access_key_id, access_key_secret
 
-    def _get_logs(self, tp, from_timestamp, to_timestamp, query) -> List[Dict]:
+    def _get_logs(self, tp, from_timestamp, to_timestamp, query, **kwargs) -> List[Dict]:
         result = []
         config = {
             "hz_log": {
                 "endpoint": "cn-hangzhou.log.aliyuncs.com",
                 "project_name": "hz-k8s",
                 "logstore_name": "hz-k8s"
             },
@@ -49,59 +49,59 @@
                 "endpoint": "us-west-1.log.aliyuncs.com",
                 "project_name": "usa-k8s",
                 "logstore_name": "usa-ingress"
             }
         }
         endpoint, project_name, logstore_name = config.get(tp).values()
         client = LogClient(endpoint, self._access_key_id, self._access_key_secret)
-        request = GetLogsRequest(project_name, logstore_name, from_timestamp, to_timestamp, query=query, line=-1) # 指定获取所有日志数量
+        request = GetLogsRequest(project_name, logstore_name, from_timestamp, to_timestamp, query=query, line=-1, **kwargs) # 指定获取所有日志数量
         response = client.get_logs(request)
         for log in response.get_logs():
             result.append(dict(log.contents))
         return result
 
-    def _sls_config_res(self, tp, from_timestamp, to_timestamp, query) -> List[Dict]:
+    def _sls_config_res(self, tp, from_timestamp, to_timestamp, query, **kwargs) -> List[Dict]:
         try:
-            result = self._get_logs(tp, from_timestamp, to_timestamp, query)
+            result = self._get_logs(tp, from_timestamp, to_timestamp, query, **kwargs)
         except Exception as e:
             raise Exception(f"查询 {tp} 日志失败: {e}")
         return result
 
-    def hz_ingress_log(self, from_timestamp, to_timestamp, query) -> List[Dict]:
+    def hz_ingress_log(self, from_timestamp, to_timestamp, query, **kwargs) -> List[Dict]:
         """
         查询杭州的ingress日志
         @param from_timestamp: 开始时间戳
         @param to_timestamp: 结束时间戳
         @param query: 查询条件
         @return: 查询结果(List类型)
         """
-        return self._sls_config_res('hz_ingress', from_timestamp, to_timestamp, query)
+        return self._sls_config_res('hz_ingress', from_timestamp, to_timestamp, query, **kwargs)
 
-    def hz_service_log(self, from_timestamp, to_timestamp, query) -> List[Dict]:
+    def hz_service_log(self, from_timestamp, to_timestamp, query, **kwargs) -> List[Dict]:
         """
         查询杭州的服务日志
         @param from_timestamp: 开始时间戳
         @param to_timestamp: 结束时间戳
         @param query: 查询条件
         @return: 查询结果(List类型)
         """
-        return self._sls_config_res('hz_log', from_timestamp, to_timestamp, query)
+        return self._sls_config_res('hz_log', from_timestamp, to_timestamp, query, **kwargs)
 
-    def usa_ingress_log(self, from_timestamp, to_timestamp, query) -> List[Dict]:
+    def usa_ingress_log(self, from_timestamp, to_timestamp, query, **kwargs) -> List[Dict]:
         """
         查询美国的ingress日志
         @param from_timestamp: 开始时间戳
         @param to_timestamp: 结束时间戳
         @param query: 查询条件
         @return: 查询结果(List类型)
         """
-        return self._sls_config_res('usa_ingress', from_timestamp, to_timestamp, query)
+        return self._sls_config_res('usa_ingress', from_timestamp, to_timestamp, query, **kwargs)
 
-    def usa_service_log(self, from_timestamp, to_timestamp, query) -> List[Dict]:
+    def usa_service_log(self, from_timestamp, to_timestamp, query, **kwargs) -> List[Dict]:
         """
         查询美国的服务日志
         @param from_timestamp: 开始时间戳
         @param to_timestamp: 结束时间戳
         @param query: 查询条件
         @return: 查询结果(List类型)
         """
-        return self._sls_config_res('usa_log', from_timestamp, to_timestamp, query)
+        return self._sls_config_res('usa_log', from_timestamp, to_timestamp, query, **kwargs)
```

### Comparing `cjops-1.0.3/src/cjops/command.py` & `cjops-1.0.4/src/cjops/command.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.3/src/cjops/domain.py` & `cjops-1.0.4/src/cjops/domain.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.3/src/cjops/email.py` & `cjops-1.0.4/src/cjops/email.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.3/src/cjops/excel.py` & `cjops-1.0.4/src/cjops/excel.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.3/src/cjops/qw.py` & `cjops-1.0.4/src/cjops/qw.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.3/src/cjops/sql.py` & `cjops-1.0.4/src/cjops/sql.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.3/src/cjops/time.py` & `cjops-1.0.4/src/cjops/time.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.3/src/cjops/utils.py` & `cjops-1.0.4/src/cjops/utils.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.3/src/cjops.egg-info/PKG-INFO` & `cjops-1.0.4/src/cjops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjops
-Version: 1.0.3
+Version: 1.0.4
 Summary: cj ops.
 Author: chenxing
 Author-email: chenxing@cjdropshipping.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
```

