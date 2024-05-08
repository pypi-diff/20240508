# Comparing `tmp/sparrowDB-0.1.tar.gz` & `tmp/sparrowDB-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparrowDB-0.1.tar", last modified: Mon Apr 15 02:02:37 2024, max compression
+gzip compressed data, was "sparrowDB-0.1.1.tar", last modified: Wed May  8 03:11:24 2024, max compression
```

## Comparing `sparrowDB-0.1.tar` & `sparrowDB-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 02:02:37.329670 sparrowDB-0.1/
--rw-rw-rw-   0        0        0      153 2024-04-15 02:02:37.328669 sparrowDB-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-15 02:02:37.329670 sparrowDB-0.1/setup.cfg
--rw-rw-rw-   0        0        0      259 2024-04-15 02:02:28.000000 sparrowDB-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 02:02:37.318667 sparrowDB-0.1/sparrowDB/
--rw-rw-rw-   0        0        0      155 2024-04-15 01:53:45.000000 sparrowDB-0.1/sparrowDB/__init__.py
--rw-rw-rw-   0        0        0      171 2024-04-15 01:46:09.000000 sparrowDB-0.1/sparrowDB/config.py
--rw-rw-rw-   0        0        0     7208 2024-04-12 08:59:50.000000 sparrowDB-0.1/sparrowDB/sparrow.py
--rw-rw-rw-   0        0        0     2897 2024-04-12 08:59:49.000000 sparrowDB-0.1/sparrowDB/sparrow_clint.py
--rw-rw-rw-   0        0        0     8772 2024-04-15 01:53:45.000000 sparrowDB-0.1/sparrowDB/sparrow_clint_service.py
-drwxrwxrwx   0        0        0        0 2024-04-15 02:02:37.326680 sparrowDB-0.1/sparrowDB.egg-info/
--rw-rw-rw-   0        0        0      153 2024-04-15 02:02:37.000000 sparrowDB-0.1/sparrowDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2024-04-15 02:02:37.000000 sparrowDB-0.1/sparrowDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 02:02:37.000000 sparrowDB-0.1/sparrowDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-15 02:02:37.000000 sparrowDB-0.1/sparrowDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-15 02:02:37.000000 sparrowDB-0.1/sparrowDB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 03:11:24.191118 sparrowDB-0.1.1/
+-rw-rw-rw-   0        0        0      180 2024-05-08 03:11:24.189117 sparrowDB-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-08 03:11:24.191118 sparrowDB-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      273 2024-05-08 03:11:16.000000 sparrowDB-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:11:24.179115 sparrowDB-0.1.1/sparrowDB/
+-rw-rw-rw-   0        0        0      153 2024-05-08 02:24:47.000000 sparrowDB-0.1.1/sparrowDB/__init__.py
+-rw-rw-rw-   0        0        0      327 2024-05-08 03:11:09.000000 sparrowDB-0.1.1/sparrowDB/config.py
+-rw-rw-rw-   0        0        0     8148 2024-05-08 03:11:09.000000 sparrowDB-0.1.1/sparrowDB/sparrow.py
+-rw-rw-rw-   0        0        0     2923 2024-05-08 03:11:09.000000 sparrowDB-0.1.1/sparrowDB/sparrow_clint.py
+-rw-rw-rw-   0        0        0    11734 2024-05-08 03:11:09.000000 sparrowDB-0.1.1/sparrowDB/sparrow_clint_service.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:11:24.188117 sparrowDB-0.1.1/sparrowDB/tools/
+-rw-rw-rw-   0        0        0       57 2024-05-08 02:39:41.000000 sparrowDB-0.1.1/sparrowDB/tools/__init__.py
+-rw-rw-rw-   0        0        0      296 2024-05-08 02:39:41.000000 sparrowDB-0.1.1/sparrowDB/tools/error.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:11:24.186117 sparrowDB-0.1.1/sparrowDB.egg-info/
+-rw-rw-rw-   0        0        0      180 2024-05-08 03:11:24.000000 sparrowDB-0.1.1/sparrowDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2024-05-08 03:11:24.000000 sparrowDB-0.1.1/sparrowDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 03:11:24.000000 sparrowDB-0.1.1/sparrowDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-08 03:11:24.000000 sparrowDB-0.1.1/sparrowDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 03:11:24.000000 sparrowDB-0.1.1/sparrowDB.egg-info/top_level.txt
```

### Comparing `sparrowDB-0.1/sparrowDB/sparrow.py` & `sparrowDB-0.1.1/sparrowDB/sparrow.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import time
-from datetime import datetime, timedelta
+from datetime import datetime
+from datetime import timedelta
 
 
 class SparrowDB(object):
     def __init__(self):
         self._data_key_value_ = {}
         self._data_body_ = {}
 
-    def _is_key_value_overdue_(self, key):
+    def _is_key_value_overdue_(self, key: str):
         """
         检测key_value的值是否过期，过期就删除
         :param key: 值的key
         :return:
         """
         try:
             valid_time = self._data_key_value_.get(key).get("valid_time")
@@ -23,15 +24,15 @@
                 valid_timestamp = time.mktime(valid_time.timetuple())
                 new_time = time.time()
                 if new_time > valid_timestamp:
                     del self._data_key_value_[key]
         except:
             pass
 
-    def _is_body_overdue_(self, key):
+    def _is_body_overdue_(self, key: str):
         """
         检测body的值是否过期，过期就删除
         :param key: 值的key
         :return:
         """
         try:
             valid_time = self._data_body_.get(key).get("valid_time")
@@ -43,152 +44,168 @@
                 valid_timestamp = time.mktime(valid_time.timetuple())
                 new_time = time.time()
                 if new_time > valid_timestamp:
                     del self._data_body_[key]
         except:
             pass
 
-    def set_key_value(self, key, value, valid_time=None):
+    def set_key_value(self, key: str, value: str, valid_time: float = None):
         """
         向key_value加入数据
-        :param key:
-        :param value:
-        :param valid_time:
+        :param key: 键名
+        :param value: 键值
+        :param valid_time: 过期时间
         :return:
         """
         self._is_key_value_overdue_(key)
         if key in self._data_key_value_.keys():
             return f"{key} already in SparrowDB"
         else:
             self._data_key_value_[key] = {"value": value, "valid_time": valid_time, "set_time": time.time()}
             return self._data_key_value_[key]
 
-    def reset_key_value(self, key, value, valid_time=None):
+    def reset_key_value(self, key: str, value: str, valid_time: float = None):
         """
         重新设置key_value的某个数据的值
-        :param key:
-        :param value:
-        :param valid_time:
+        :param key: 键名
+        :param value: 键值
+        :param valid_time: 过期时间
         :return:
         """
         self._is_key_value_overdue_(key)
         if key in self._data_key_value_.keys():
             self._data_key_value_[key] = {"value": value, "valid_time": valid_time, "set_time": time.time()}
             return self._data_key_value_[key]
         else:
             return f"{key} not found in SparrowDB"
 
-    def get_key_value(self, key):
+    def get_key_value(self, key: str):
         """
         获取key_value中某个数据的值
-        :param key:
+        :param key: 键名
         :return:
         """
         self._is_key_value_overdue_(key)
         if key in self._data_key_value_.keys():
             return {key: self._data_key_value_[key]['value']}
         else:
             return f"{key} not found in SparrowDB"
 
-    def delete_key_value(self, key):
+    def delete_key_value(self, key: str):
         """
         删除key_value中某个数据
-        :param key:
+        :param key: 键名
         :return:
         """
         self._is_key_value_overdue_(key)
         if key in self._data_key_value_.keys():
             data = {"key": key, "value": self._data_key_value_[key]['value']}
             del self._data_key_value_[key]
             return data
         else:
             return f"{key} not found  in SparrowDB"
 
-    def set_body(self, key, body, valid_time=None):
+    def set_body(self, key: str, body: dict, valid_time: float = None):
         """
         行body中加入数据
-        :param key:
-        :param body:
-        :param valid_time:
+        :param key: 键名
+        :param body: 键值
+        :param valid_time: 过期时间
         :return:
         """
         self._is_body_overdue_(key)
         if key in self._data_body_.keys():
 
             return f"{key} already in SparrowDB"
         else:
             self._data_body_[key] = {"value": body, "valid_time": valid_time, "set_time": time.time()}
             return self._data_body_[key]
 
-    def reset_body(self, key, body, valid_time=None):
+    def reset_body(self, key: str, body: dict, valid_time: float = None):
         """
         重新设置body中的某个数据
-        :param key:
-        :param body:
-        :param valid_time:
+        :param key: 键名
+        :param body: 键值
+        :param valid_time: 过期时间
         :return:
         """
         self._is_body_overdue_(key)
         if key in self._data_body_.keys():
             body_key = body.get("key")
             body_value = body.get("value")
             self._data_body_[key]["value"][body_key] = body_value
             self._data_body_[key]["valid_time"] = valid_time
             self._data_body_[key]["set_time"] = time.time()
             return self._data_body_[key]
         else:
             return f"{key} not found in SparrowDB"
 
-    def get_body(self, key):
+    def reset_body_all(self, key: str, body: dict, valid_time: float = None):
+        """
+        重新设置body中的某个数据
+        :param key: 键名
+        :param body: 键值
+        :param valid_time: 过期时间
+        :return:
+        """
+        self._is_body_overdue_(key)
+        if key in self._data_body_.keys():
+            self._data_body_[key]["value"] = body
+            self._data_body_[key]["valid_time"] = valid_time
+            self._data_body_[key]["set_time"] = time.time()
+            return self._data_body_[key]
+        else:
+            return f"{key} not found in SparrowDB"
+
+    def get_body(self, key: str):
         """
         获取body中的某个值
-        :param key:
+        :param key: 键名
         :return:
         """
         self._is_body_overdue_(key)
         if key in self._data_body_.keys():
             return {key: self._data_body_[key]['value']}
         else:
             return f"{key} not found in SparrowDB"
 
-    def delete_body(self, key):
+    def delete_body(self, key: str):
         """
         删除body中的某个值
-        :param key:
+        :param key: 键名
         :return:
         """
         self._is_body_overdue_(key)
         if key in self._data_body_.keys():
             data = {"key": key, "value": self._data_body_[key]['value']}
             del self._data_body_[key]
             return data
         else:
             return f"{key} not found  in SparrowDB"
 
-    def set_key_value_valid_time(self, key, valid_time):
+    def set_key_value_valid_time(self, key: str, valid_time: float):
         """
         重新设置key_value中某个值的过期时间
-        :param key:
-        :param valid_time:
+        :param key: 键名
+        :param valid_time: 过期时间
         :return:
         """
-        print(key)
         self._is_key_value_overdue_(key)
         if key in self._data_key_value_.keys():
             self._data_key_value_[key]["valid_time"] = valid_time
             self._data_key_value_[key]["set_time"] = time.time()
             return self._data_key_value_[key]
         else:
             return f"{key} not found in SparrowDB"
 
-    def set_body_valid_time(self, key, valid_time):
+    def set_body_valid_time(self, key: str, valid_time: float):
         """
         重新设置body中某个值的过期时间
-        :param key:
-        :param valid_time:
+        :param key: 键名
+        :param valid_time: 过期时间
         :return:
         """
         self._is_body_overdue_(key)
         if key in self._data_body_.keys():
             self._data_body_[key]["valid_time"] = valid_time
             self._data_body_[key]["set_time"] = time.time()
             return self._data_body_[key]
```

### Comparing `sparrowDB-0.1/sparrowDB/sparrow_clint.py` & `sparrowDB-0.1.1/sparrowDB/sparrow_clint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 sparrowDB 客服端
 """
 import sys
 import requests
-from colorama import Fore, init
+from colorama import Fore
+from colorama import init
 
 
 class SparrowClint(object):
     def __init__(self):
         self.url = "http://127.0.0.1:712"
         self.headers = {"SparrowApi": "SparrowApi", "Password": "", "Username": ""}
         init(autoreset=True)
 
-    def send_command(self, command):
+    def send_command(self, command: str):
         """
         发送命令
         :param command: 命令
         :return:
         """
         r = requests.post(self.url, data={"command": command}, headers=self.headers)
         return r.json()
```

