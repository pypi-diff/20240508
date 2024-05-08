# Comparing `tmp/ait_openapi-0.0.1.17.tar.gz` & `tmp/ait_openapi-0.0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ait_openapi-0.0.1.17.tar", last modified: Tue May  7 02:06:15 2024, max compression
+gzip compressed data, was "dist/ait_openapi-0.0.1.18.tar", last modified: Wed May  8 11:28:32 2024, max compression
```

## Comparing `ait_openapi-0.0.1.17.tar` & `ait_openapi-0.0.1.18.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 fanqw     (1003) fanqw     (1003)        0 2024-05-07 02:06:15.000000 ait_openapi-0.0.1.17/
-drwxrwxr-x   0 fanqw     (1003) fanqw     (1003)        0 2024-05-07 02:06:15.000000 ait_openapi-0.0.1.17/src/
-drwxrwxr-x   0 fanqw     (1003) fanqw     (1003)        0 2024-05-07 02:06:15.000000 ait_openapi-0.0.1.17/src/ait_openapi/
-drwxrwxr-x   0 fanqw     (1003) fanqw     (1003)        0 2024-05-07 02:06:15.000000 ait_openapi-0.0.1.17/src/ait_openapi/middleware/
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)      157 2024-04-07 07:20:21.000000 ait_openapi-0.0.1.17/src/ait_openapi/middleware/__init__.py
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     3878 2024-04-07 07:20:21.000000 ait_openapi-0.0.1.17/src/ait_openapi/middleware/context_middleware.py
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)      897 2024-05-07 01:55:19.000000 ait_openapi-0.0.1.17/src/ait_openapi/__init__.py
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     3070 2024-05-07 01:53:01.000000 ait_openapi-0.0.1.17/src/ait_openapi/auth_billing.py
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     2246 2024-04-29 12:04:50.000000 ait_openapi-0.0.1.17/src/ait_openapi/authorize.py
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)      280 2024-04-07 07:20:21.000000 ait_openapi-0.0.1.17/src/ait_openapi/config.py
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)      305 2024-04-07 07:20:21.000000 ait_openapi-0.0.1.17/src/ait_openapi/exception.py
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     7198 2024-04-07 07:20:21.000000 ait_openapi-0.0.1.17/src/ait_openapi/log.py
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)      321 2024-04-07 07:20:21.000000 ait_openapi-0.0.1.17/src/ait_openapi/openapi_contexvar.py
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     2436 2024-04-07 07:20:21.000000 ait_openapi-0.0.1.17/src/ait_openapi/schema.py
-drwxrwxr-x   0 fanqw     (1003) fanqw     (1003)        0 2024-05-07 02:06:15.000000 ait_openapi-0.0.1.17/src/ait_openapi.egg-info/
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     8477 2024-05-07 02:06:07.000000 ait_openapi-0.0.1.17/src/ait_openapi.egg-info/PKG-INFO
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)      568 2024-05-07 02:06:07.000000 ait_openapi-0.0.1.17/src/ait_openapi.egg-info/SOURCES.txt
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)        1 2024-05-07 02:06:07.000000 ait_openapi-0.0.1.17/src/ait_openapi.egg-info/dependency_links.txt
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)        1 2024-04-07 07:22:32.000000 ait_openapi-0.0.1.17/src/ait_openapi.egg-info/not-zip-safe
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)       39 2024-05-07 02:06:07.000000 ait_openapi-0.0.1.17/src/ait_openapi.egg-info/requires.txt
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)       12 2024-05-07 02:06:07.000000 ait_openapi-0.0.1.17/src/ait_openapi.egg-info/top_level.txt
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     8183 2024-04-29 12:04:50.000000 ait_openapi-0.0.1.17/README.md
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)      821 2024-05-07 01:57:26.000000 ait_openapi-0.0.1.17/setup.py
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     8477 2024-05-07 02:06:15.000000 ait_openapi-0.0.1.17/PKG-INFO
--rw-rw-r--   0 fanqw     (1003) fanqw     (1003)       38 2024-05-07 02:06:15.000000 ait_openapi-0.0.1.17/setup.cfg
+drwxrwxr-x   0 fanqw     (1003) fanqw     (1003)        0 2024-05-08 11:28:32.000000 ait_openapi-0.0.1.18/
+drwxrwxr-x   0 fanqw     (1003) fanqw     (1003)        0 2024-05-08 11:28:32.000000 ait_openapi-0.0.1.18/src/
+drwxrwxr-x   0 fanqw     (1003) fanqw     (1003)        0 2024-05-08 11:28:32.000000 ait_openapi-0.0.1.18/src/ait_openapi/
+drwxrwxr-x   0 fanqw     (1003) fanqw     (1003)        0 2024-05-08 11:28:32.000000 ait_openapi-0.0.1.18/src/ait_openapi/middleware/
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)      157 2024-04-07 07:20:21.000000 ait_openapi-0.0.1.18/src/ait_openapi/middleware/__init__.py
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     3878 2024-04-07 07:20:21.000000 ait_openapi-0.0.1.18/src/ait_openapi/middleware/context_middleware.py
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)      897 2024-05-07 01:55:19.000000 ait_openapi-0.0.1.18/src/ait_openapi/__init__.py
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     3571 2024-05-07 12:29:28.000000 ait_openapi-0.0.1.18/src/ait_openapi/auth_billing.py
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     2246 2024-04-29 12:04:50.000000 ait_openapi-0.0.1.18/src/ait_openapi/authorize.py
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)      280 2024-04-07 07:20:21.000000 ait_openapi-0.0.1.18/src/ait_openapi/config.py
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)      305 2024-04-07 07:20:21.000000 ait_openapi-0.0.1.18/src/ait_openapi/exception.py
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     7198 2024-04-07 07:20:21.000000 ait_openapi-0.0.1.18/src/ait_openapi/log.py
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)      321 2024-04-07 07:20:21.000000 ait_openapi-0.0.1.18/src/ait_openapi/openapi_contexvar.py
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     2436 2024-04-07 07:20:21.000000 ait_openapi-0.0.1.18/src/ait_openapi/schema.py
+drwxrwxr-x   0 fanqw     (1003) fanqw     (1003)        0 2024-05-08 11:28:32.000000 ait_openapi-0.0.1.18/src/ait_openapi.egg-info/
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     8477 2024-05-08 11:28:32.000000 ait_openapi-0.0.1.18/src/ait_openapi.egg-info/PKG-INFO
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)      568 2024-05-08 11:28:32.000000 ait_openapi-0.0.1.18/src/ait_openapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)        1 2024-05-08 11:28:32.000000 ait_openapi-0.0.1.18/src/ait_openapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)        1 2024-04-07 07:22:32.000000 ait_openapi-0.0.1.18/src/ait_openapi.egg-info/not-zip-safe
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)       39 2024-05-08 11:28:32.000000 ait_openapi-0.0.1.18/src/ait_openapi.egg-info/requires.txt
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)       12 2024-05-08 11:28:32.000000 ait_openapi-0.0.1.18/src/ait_openapi.egg-info/top_level.txt
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     8183 2024-04-29 12:04:50.000000 ait_openapi-0.0.1.18/README.md
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)      821 2024-05-08 11:27:44.000000 ait_openapi-0.0.1.18/setup.py
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)     8477 2024-05-08 11:28:32.000000 ait_openapi-0.0.1.18/PKG-INFO
+-rw-rw-r--   0 fanqw     (1003) fanqw     (1003)       38 2024-05-08 11:28:32.000000 ait_openapi-0.0.1.18/setup.cfg
```

### Comparing `ait_openapi-0.0.1.17/src/ait_openapi/middleware/context_middleware.py` & `ait_openapi-0.0.1.18/src/ait_openapi/middleware/context_middleware.py`

 * *Files identical despite different names*

### Comparing `ait_openapi-0.0.1.17/src/ait_openapi/__init__.py` & `ait_openapi-0.0.1.18/src/ait_openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ait_openapi-0.0.1.17/src/ait_openapi/auth_billing.py` & `ait_openapi-0.0.1.18/src/ait_openapi/auth_billing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 from .log import operation_log
 from .authorize import validate_token, check_configuration, account_balance_enough
 from .openapi_contexvar import trace_id_context, caller_id_context, request_url_context
 from pydantic import BaseModel
 import uuid
 from fastapi import Request
+import logging
+# 创建一个日志记录器
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)  # 设置日志级别为INFO
+
+# 创建一个控制台处理器，并设置其级别和格式
+console_handler = logging.StreamHandler()
+console_handler.setLevel(logging.INFO)
+formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
+console_handler.setFormatter(formatter)
+
+# 将处理器添加到日志记录器
+logger.addHandler(console_handler)
 
 class ErrorInfo(BaseModel):
     task_id: str = ""
     result: str = ""
     status: int = 40000001
     message: str = ""
 
@@ -25,15 +38,15 @@
                 if not supported:
                     return error_json
                 t_token, c_token, r_token = set_context(task_id, caller_id, end_point)
                 result = await func(*args, **kwargs)
                 clean_context(t_token, c_token, r_token)
                 return result
             else:
-                print("please check your request param,have not a param's type is Request of fastapi!")
+                logger.warn("please check your request param,have not a param's type is Request of fastapi!")
             return func(*args, **kwargs)
         return wrapper
     return async_authenticate_decorator
 
 
 def authenticate_user(token, task_id):
     if check_configuration():
@@ -52,15 +65,15 @@
 
 @operation_log(op_type='upload_cost_log', is_cost_log=True)
 def upload_cost_log(result_obejct):
     response = result_obejct.dict()
     return response
 
 def print_context(log):
-    print(f"{log} trace_id:{trace_id_context.get()}, caller_id:{caller_id_context.get()}, end_point:{request_url_context.get()}")
+    logger.info(f"{log} trace_id:{trace_id_context.get()}, caller_id:{caller_id_context.get()}, end_point:{request_url_context.get()}")
 
 def get_context():
     return trace_id_context.get(), caller_id_context.get(), request_url_context.get()
 
 def set_context(trace_id, caller_id, end_point):
     t_token = trace_id_context.set(trace_id)
     c_token = caller_id_context.set(caller_id)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ait_openapi-0.0.1.17/src/ait_openapi/authorize.py` & `ait_openapi-0.0.1.18/src/ait_openapi/authorize.py`

 * *Files identical despite different names*

### Comparing `ait_openapi-0.0.1.17/src/ait_openapi/log.py` & `ait_openapi-0.0.1.18/src/ait_openapi/log.py`

 * *Files identical despite different names*

### Comparing `ait_openapi-0.0.1.17/src/ait_openapi/schema.py` & `ait_openapi-0.0.1.18/src/ait_openapi/schema.py`

 * *Files identical despite different names*

### Comparing `ait_openapi-0.0.1.17/src/ait_openapi.egg-info/PKG-INFO` & `ait_openapi-0.0.1.18/src/ait_openapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ait-openapi
-Version: 0.0.1.17
+Version: 0.0.1.18
 Summary: client for openapi service.
 Home-page: UNKNOWN
 Author: fanqiangwei
 Author-email: fanqiangwei002@ke.com
 License: UNKNOWN
 Platform: any
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `ait_openapi-0.0.1.17/src/ait_openapi.egg-info/SOURCES.txt` & `ait_openapi-0.0.1.18/src/ait_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ait_openapi-0.0.1.17/README.md` & `ait_openapi-0.0.1.18/README.md`

 * *Files identical despite different names*

### Comparing `ait_openapi-0.0.1.17/setup.py` & `ait_openapi-0.0.1.18/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # encoding: utf-8
 from setuptools import setup, find_packages
 
 SHORT = "client for openapi service."
 
-__version__ = "0.0.1.17"
+__version__ = "0.0.1.18"
 __author__ = 'fanqiangwei'
 __email__ = 'fanqiangwei002@ke.com'
 readme_path = 'README.md'
 
 setup(
     name='ait_openapi',
     version=__version__,
```

### Comparing `ait_openapi-0.0.1.17/PKG-INFO` & `ait_openapi-0.0.1.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ait_openapi
-Version: 0.0.1.17
+Version: 0.0.1.18
 Summary: client for openapi service.
 Home-page: UNKNOWN
 Author: fanqiangwei
 Author-email: fanqiangwei002@ke.com
 License: UNKNOWN
 Platform: any
 Classifier: Programming Language :: Python :: 3.5
```

