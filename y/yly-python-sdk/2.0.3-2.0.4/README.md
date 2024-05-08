# Comparing `tmp/yly-python-sdk-2.0.3.tar.gz` & `tmp/yly-python-sdk-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yly-python-sdk-2.0.3.tar", last modified: Thu Nov  2 05:43:54 2023, max compression
+gzip compressed data, was "yly-python-sdk-2.0.4.tar", last modified: Wed May  8 03:22:02 2024, max compression
```

## Comparing `yly-python-sdk-2.0.3.tar` & `yly-python-sdk-2.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 05:43:54.172721 yly-python-sdk-2.0.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 05:43:54.168721 yly-python-sdk-2.0.3/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 05:43:54.168721 yly-python-sdk-2.0.3/Lib/Api/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-12 06:01:33.000000 yly-python-sdk-2.0.3/Lib/Api/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1200 2023-06-13 09:19:49.000000 yly-python-sdk-2.0.3/Lib/Api/yly_express_print.py
--rw-rw-r--   0 root         (0) root         (0)      546 2021-05-12 06:01:33.000000 yly-python-sdk-2.0.3/Lib/Api/yly_oauth.py
--rw-rw-r--   0 root         (0) root         (0)      794 2023-06-13 09:20:20.000000 yly-python-sdk-2.0.3/Lib/Api/yly_picture_print.py
--rw-rw-r--   0 root         (0) root         (0)      887 2023-06-13 09:19:49.000000 yly-python-sdk-2.0.3/Lib/Api/yly_print.py
--rw-rw-r--   0 root         (0) root         (0)      527 2021-05-12 06:01:33.000000 yly-python-sdk-2.0.3/Lib/Api/yly_print_menu.py
--rw-rw-r--   0 root         (0) root         (0)     8632 2023-11-02 04:02:10.000000 yly-python-sdk-2.0.3/Lib/Api/yly_printer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 05:43:54.168721 yly-python-sdk-2.0.3/Lib/Config/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-12 06:01:33.000000 yly-python-sdk-2.0.3/Lib/Config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      635 2023-06-13 09:00:02.000000 yly-python-sdk-2.0.3/Lib/Config/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 05:43:54.168721 yly-python-sdk-2.0.3/Lib/Oauth/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-12 06:01:33.000000 yly-python-sdk-2.0.3/Lib/Oauth/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1879 2023-06-13 09:02:12.000000 yly-python-sdk-2.0.3/Lib/Oauth/oauth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 05:43:54.172721 yly-python-sdk-2.0.3/Lib/Protocol/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-12 06:01:33.000000 yly-python-sdk-2.0.3/Lib/Protocol/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1267 2023-06-13 09:06:45.000000 yly-python-sdk-2.0.3/Lib/Protocol/rpc_client.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-12 06:01:33.000000 yly-python-sdk-2.0.3/Lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-11-02 05:43:54.172721 yly-python-sdk-2.0.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2823 2023-11-02 05:35:36.000000 yly-python-sdk-2.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-02 05:43:54.172721 yly-python-sdk-2.0.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      341 2023-11-02 05:35:36.000000 yly-python-sdk-2.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-02 05:43:54.172721 yly-python-sdk-2.0.3/yly_python_sdk.egg-info/
--rw-rw-r--   0 root         (0) root         (0)      233 2023-11-02 05:43:54.000000 yly-python-sdk-2.0.3/yly_python_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      492 2023-11-02 05:43:54.000000 yly-python-sdk-2.0.3/yly_python_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-11-02 05:43:54.000000 yly-python-sdk-2.0.3/yly_python_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)        4 2023-11-02 05:43:54.000000 yly-python-sdk-2.0.3/yly_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:22:02.258479 yly-python-sdk-2.0.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:22:02.254480 yly-python-sdk-2.0.4/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:22:02.254480 yly-python-sdk-2.0.4/Lib/Api/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-12 06:01:33.000000 yly-python-sdk-2.0.4/Lib/Api/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1200 2023-06-13 09:19:49.000000 yly-python-sdk-2.0.4/Lib/Api/yly_express_print.py
+-rw-rw-r--   0 root         (0) root         (0)      546 2021-05-12 06:01:33.000000 yly-python-sdk-2.0.4/Lib/Api/yly_oauth.py
+-rw-rw-r--   0 root         (0) root         (0)      794 2023-06-13 09:20:20.000000 yly-python-sdk-2.0.4/Lib/Api/yly_picture_print.py
+-rw-rw-r--   0 root         (0) root         (0)      887 2023-06-13 09:19:49.000000 yly-python-sdk-2.0.4/Lib/Api/yly_print.py
+-rw-rw-r--   0 root         (0) root         (0)      527 2021-05-12 06:01:33.000000 yly-python-sdk-2.0.4/Lib/Api/yly_print_menu.py
+-rw-rw-r--   0 root         (0) root         (0)     8687 2024-05-08 03:19:07.000000 yly-python-sdk-2.0.4/Lib/Api/yly_printer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:22:02.254480 yly-python-sdk-2.0.4/Lib/Config/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-12 06:01:33.000000 yly-python-sdk-2.0.4/Lib/Config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      635 2023-06-13 09:00:02.000000 yly-python-sdk-2.0.4/Lib/Config/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:22:02.254480 yly-python-sdk-2.0.4/Lib/Oauth/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-12 06:01:33.000000 yly-python-sdk-2.0.4/Lib/Oauth/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1879 2023-06-13 09:02:12.000000 yly-python-sdk-2.0.4/Lib/Oauth/oauth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:22:02.254480 yly-python-sdk-2.0.4/Lib/Protocol/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-12 06:01:33.000000 yly-python-sdk-2.0.4/Lib/Protocol/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1267 2023-06-13 09:06:45.000000 yly-python-sdk-2.0.4/Lib/Protocol/rpc_client.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-05-12 06:01:33.000000 yly-python-sdk-2.0.4/Lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      233 2024-05-08 03:22:02.258479 yly-python-sdk-2.0.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2823 2023-11-02 05:35:36.000000 yly-python-sdk-2.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 03:22:02.258479 yly-python-sdk-2.0.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      341 2024-05-08 03:19:07.000000 yly-python-sdk-2.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:22:02.258479 yly-python-sdk-2.0.4/yly_python_sdk.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)      233 2024-05-08 03:22:02.000000 yly-python-sdk-2.0.4/yly_python_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      492 2024-05-08 03:22:02.000000 yly-python-sdk-2.0.4/yly_python_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-05-08 03:22:02.000000 yly-python-sdk-2.0.4/yly_python_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)        4 2024-05-08 03:22:02.000000 yly-python-sdk-2.0.4/yly_python_sdk.egg-info/top_level.txt
```

### Comparing `yly-python-sdk-2.0.3/Lib/Api/yly_express_print.py` & `yly-python-sdk-2.0.4/Lib/Api/yly_express_print.py`

 * *Files identical despite different names*

### Comparing `yly-python-sdk-2.0.3/Lib/Api/yly_oauth.py` & `yly-python-sdk-2.0.4/Lib/Api/yly_oauth.py`

 * *Files identical despite different names*

### Comparing `yly-python-sdk-2.0.3/Lib/Api/yly_picture_print.py` & `yly-python-sdk-2.0.4/Lib/Api/yly_picture_print.py`

 * *Files identical despite different names*

### Comparing `yly-python-sdk-2.0.3/Lib/Api/yly_print.py` & `yly-python-sdk-2.0.4/Lib/Api/yly_print.py`

 * *Files identical despite different names*

### Comparing `yly-python-sdk-2.0.3/Lib/Api/yly_print_menu.py` & `yly-python-sdk-2.0.4/Lib/Api/yly_print_menu.py`

 * *Files identical despite different names*

### Comparing `yly-python-sdk-2.0.3/Lib/Api/yly_printer.py` & `yly-python-sdk-2.0.4/Lib/Api/yly_printer.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,24 +239,26 @@
         :return:
         """
         params = {
             'machine_code': machine_code
         }
         return self.__client.call('printer/getprintstatus', params)
 
-    def push_switch(self, machine_code, status):
+    def push_switch(self, machine_code, status, mode= 1):
         """
         K8 推送开关设置接口
         :param machine_code:
         :param status:
+        :param mode
         :return:
         """
         params = {
             'machine_code': machine_code,
-            'status': status
+            'status': status,
+            'mode': mode
         }
         return self.__client.call('printer/pushswitch', params)
 
 
     def set_keywords(self, machine_code, keys, type, content):
         """
         K8关键词设置接口
```

### Comparing `yly-python-sdk-2.0.3/Lib/Config/config.py` & `yly-python-sdk-2.0.4/Lib/Config/config.py`

 * *Files identical despite different names*

### Comparing `yly-python-sdk-2.0.3/Lib/Oauth/oauth.py` & `yly-python-sdk-2.0.4/Lib/Oauth/oauth.py`

 * *Files identical despite different names*

### Comparing `yly-python-sdk-2.0.3/Lib/Protocol/rpc_client.py` & `yly-python-sdk-2.0.4/Lib/Protocol/rpc_client.py`

 * *Files identical despite different names*

### Comparing `yly-python-sdk-2.0.3/README.md` & `yly-python-sdk-2.0.4/README.md`

 * *Files identical despite different names*

