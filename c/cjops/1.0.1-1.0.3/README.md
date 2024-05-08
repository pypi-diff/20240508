# Comparing `tmp/cjops-1.0.1.tar.gz` & `tmp/cjops-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjops-1.0.1.tar", last modified: Tue May  7 08:48:08 2024, max compression
+gzip compressed data, was "cjops-1.0.3.tar", last modified: Wed May  8 00:50:08 2024, max compression
```

## Comparing `cjops-1.0.1.tar` & `cjops-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-07 08:48:08.793130 cjops-1.0.1/
--rw-r--r--   0 caojie     (501) staff       (20)     1068 2024-03-15 01:36:01.000000 cjops-1.0.1/LICENSE
--rw-r--r--   0 caojie     (501) staff       (20)     2179 2024-05-07 08:48:08.792473 cjops-1.0.1/PKG-INFO
--rw-r--r--   0 caojie     (501) staff       (20)     1483 2024-04-25 10:03:23.000000 cjops-1.0.1/README.md
--rw-r--r--   0 caojie     (501) staff       (20)       38 2024-05-07 08:48:08.793265 cjops-1.0.1/setup.cfg
--rw-r--r--   0 caojie     (501) staff       (20)     2874 2024-05-07 08:48:04.000000 cjops-1.0.1/setup.py
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-07 08:48:08.782437 cjops-1.0.1/src/
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-07 08:48:08.788815 cjops-1.0.1/src/cjops/
--rw-r--r--   0 caojie     (501) staff       (20)      206 2024-05-07 08:13:43.000000 cjops-1.0.1/src/cjops/__init__.py
--rw-r--r--   0 caojie     (501) staff       (20)      333 2024-05-07 08:48:04.000000 cjops-1.0.1/src/cjops/__version__.py
--rw-r--r--   0 caojie     (501) staff       (20)     4446 2024-04-19 05:47:59.000000 cjops-1.0.1/src/cjops/aliyun.py
--rw-r--r--   0 caojie     (501) staff       (20)     2157 2024-04-15 06:29:32.000000 cjops-1.0.1/src/cjops/command.py
--rw-r--r--   0 caojie     (501) staff       (20)     4791 2024-05-07 07:49:15.000000 cjops-1.0.1/src/cjops/domain.py
--rw-r--r--   0 caojie     (501) staff       (20)     1795 2024-04-19 07:29:32.000000 cjops-1.0.1/src/cjops/email.py
--rw-r--r--   0 caojie     (501) staff       (20)     8459 2024-04-25 02:58:56.000000 cjops-1.0.1/src/cjops/excel.py
--rw-r--r--   0 caojie     (501) staff       (20)      870 2024-04-12 07:35:23.000000 cjops-1.0.1/src/cjops/qw.py
--rw-r--r--   0 caojie     (501) staff       (20)     1411 2024-04-19 08:45:16.000000 cjops-1.0.1/src/cjops/sql.py
--rw-r--r--   0 caojie     (501) staff       (20)     2078 2024-05-06 08:57:53.000000 cjops-1.0.1/src/cjops/time.py
--rw-r--r--   0 caojie     (501) staff       (20)     6456 2024-05-07 07:55:52.000000 cjops-1.0.1/src/cjops/utils.py
--rw-r--r--   0 caojie     (501) staff       (20)       74 2024-05-07 08:13:36.000000 cjops-1.0.1/src/cjops/version.py
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-07 08:48:08.791741 cjops-1.0.1/src/cjops.egg-info/
--rw-r--r--   0 caojie     (501) staff       (20)     2179 2024-05-07 08:48:08.000000 cjops-1.0.1/src/cjops.egg-info/PKG-INFO
--rw-r--r--   0 caojie     (501) staff       (20)      459 2024-05-07 08:48:08.000000 cjops-1.0.1/src/cjops.egg-info/SOURCES.txt
--rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-07 08:48:08.000000 cjops-1.0.1/src/cjops.egg-info/dependency_links.txt
--rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-07 08:48:08.000000 cjops-1.0.1/src/cjops.egg-info/not-zip-safe
--rw-r--r--   0 caojie     (501) staff       (20)      146 2024-05-07 08:48:08.000000 cjops-1.0.1/src/cjops.egg-info/requires.txt
--rw-r--r--   0 caojie     (501) staff       (20)        6 2024-05-07 08:48:08.000000 cjops-1.0.1/src/cjops.egg-info/top_level.txt
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 00:50:08.239874 cjops-1.0.3/
+-rw-r--r--   0 caojie     (501) staff       (20)     1068 2024-03-15 01:36:01.000000 cjops-1.0.3/LICENSE
+-rw-r--r--   0 caojie     (501) staff       (20)     2179 2024-05-08 00:50:08.239314 cjops-1.0.3/PKG-INFO
+-rw-r--r--   0 caojie     (501) staff       (20)     1483 2024-04-25 10:03:23.000000 cjops-1.0.3/README.md
+-rw-r--r--   0 caojie     (501) staff       (20)       38 2024-05-08 00:50:08.240064 cjops-1.0.3/setup.cfg
+-rw-r--r--   0 caojie     (501) staff       (20)     2874 2024-05-07 08:48:04.000000 cjops-1.0.3/setup.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 00:50:08.225489 cjops-1.0.3/src/
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 00:50:08.234413 cjops-1.0.3/src/cjops/
+-rw-r--r--   0 caojie     (501) staff       (20)      200 2024-05-08 00:48:52.000000 cjops-1.0.3/src/cjops/__init__.py
+-rw-r--r--   0 caojie     (501) staff       (20)      333 2024-05-08 00:49:57.000000 cjops-1.0.3/src/cjops/__version__.py
+-rw-r--r--   0 caojie     (501) staff       (20)     4488 2024-05-08 00:48:52.000000 cjops-1.0.3/src/cjops/aliyun.py
+-rw-r--r--   0 caojie     (501) staff       (20)     2157 2024-04-15 06:29:32.000000 cjops-1.0.3/src/cjops/command.py
+-rw-r--r--   0 caojie     (501) staff       (20)     4791 2024-05-07 07:49:15.000000 cjops-1.0.3/src/cjops/domain.py
+-rw-r--r--   0 caojie     (501) staff       (20)     1795 2024-04-19 07:29:32.000000 cjops-1.0.3/src/cjops/email.py
+-rw-r--r--   0 caojie     (501) staff       (20)     8459 2024-04-25 02:58:56.000000 cjops-1.0.3/src/cjops/excel.py
+-rw-r--r--   0 caojie     (501) staff       (20)      127 2024-05-08 00:48:52.000000 cjops-1.0.3/src/cjops/info.py
+-rw-r--r--   0 caojie     (501) staff       (20)      870 2024-04-12 07:35:23.000000 cjops-1.0.3/src/cjops/qw.py
+-rw-r--r--   0 caojie     (501) staff       (20)     1411 2024-04-19 08:45:16.000000 cjops-1.0.3/src/cjops/sql.py
+-rw-r--r--   0 caojie     (501) staff       (20)     2078 2024-05-07 09:24:16.000000 cjops-1.0.3/src/cjops/time.py
+-rw-r--r--   0 caojie     (501) staff       (20)     6456 2024-05-07 07:55:52.000000 cjops-1.0.3/src/cjops/utils.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 00:50:08.238469 cjops-1.0.3/src/cjops.egg-info/
+-rw-r--r--   0 caojie     (501) staff       (20)     2179 2024-05-08 00:50:08.000000 cjops-1.0.3/src/cjops.egg-info/PKG-INFO
+-rw-r--r--   0 caojie     (501) staff       (20)      456 2024-05-08 00:50:08.000000 cjops-1.0.3/src/cjops.egg-info/SOURCES.txt
+-rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-08 00:50:08.000000 cjops-1.0.3/src/cjops.egg-info/dependency_links.txt
+-rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-07 08:48:08.000000 cjops-1.0.3/src/cjops.egg-info/not-zip-safe
+-rw-r--r--   0 caojie     (501) staff       (20)      146 2024-05-08 00:50:08.000000 cjops-1.0.3/src/cjops.egg-info/requires.txt
+-rw-r--r--   0 caojie     (501) staff       (20)        6 2024-05-08 00:50:08.000000 cjops-1.0.3/src/cjops.egg-info/top_level.txt
```

### Comparing `cjops-1.0.1/LICENSE` & `cjops-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cjops-1.0.1/PKG-INFO` & `cjops-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjops
-Version: 1.0.1
+Version: 1.0.3
 Summary: cj ops.
 Author: chenxing
 Author-email: chenxing@cjdropshipping.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
```

### Comparing `cjops-1.0.1/README.md` & `cjops-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cjops-1.0.1/setup.py` & `cjops-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.1/src/cjops/aliyun.py` & `cjops-1.0.3/src/cjops/aliyun.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 "endpoint": "us-west-1.log.aliyuncs.com",
                 "project_name": "usa-k8s",
                 "logstore_name": "usa-ingress"
             }
         }
         endpoint, project_name, logstore_name = config.get(tp).values()
         client = LogClient(endpoint, self._access_key_id, self._access_key_secret)
-        request = GetLogsRequest(project_name, logstore_name, from_timestamp, to_timestamp, query=query)
+        request = GetLogsRequest(project_name, logstore_name, from_timestamp, to_timestamp, query=query, line=-1) # 指定获取所有日志数量
         response = client.get_logs(request)
         for log in response.get_logs():
             result.append(dict(log.contents))
         return result
 
     def _sls_config_res(self, tp, from_timestamp, to_timestamp, query) -> List[Dict]:
         try:
```

### Comparing `cjops-1.0.1/src/cjops/command.py` & `cjops-1.0.3/src/cjops/command.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.1/src/cjops/domain.py` & `cjops-1.0.3/src/cjops/domain.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.1/src/cjops/email.py` & `cjops-1.0.3/src/cjops/email.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.1/src/cjops/excel.py` & `cjops-1.0.3/src/cjops/excel.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.1/src/cjops/qw.py` & `cjops-1.0.3/src/cjops/qw.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.1/src/cjops/sql.py` & `cjops-1.0.3/src/cjops/sql.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.1/src/cjops/time.py` & `cjops-1.0.3/src/cjops/time.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.1/src/cjops/utils.py` & `cjops-1.0.3/src/cjops/utils.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.1/src/cjops.egg-info/PKG-INFO` & `cjops-1.0.3/src/cjops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjops
-Version: 1.0.1
+Version: 1.0.3
 Summary: cj ops.
 Author: chenxing
 Author-email: chenxing@cjdropshipping.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
```

