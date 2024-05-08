# Comparing `tmp/aleph-message-0.4.4.tar.gz` & `tmp/aleph-message-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleph-message-0.4.4.tar", last modified: Sat Feb 24 12:36:02 2024, max compression
+gzip compressed data, was "aleph-message-0.4.5.tar", last modified: Wed May  8 13:16:10 2024, max compression
```

## Comparing `aleph-message-0.4.4.tar` & `aleph-message-0.4.5.tar`

### file list

```diff
@@ -1,30 +1,48 @@
-drwxr-xr-x   0 sepal     (1000) sepal      (986)        0 2024-02-24 12:36:02.082619 aleph-message-0.4.4/
--rw-r--r--   0 sepal     (1000) sepal      (986)     1062 2023-01-12 17:02:10.000000 aleph-message-0.4.4/LICENSE
--rw-r--r--   0 sepal     (1000) sepal      (986)     2080 2024-02-24 12:36:02.081619 aleph-message-0.4.4/PKG-INFO
--rw-r--r--   0 sepal     (1000) sepal      (986)     1468 2023-05-12 16:19:21.000000 aleph-message-0.4.4/README.md
-drwxr-xr-x   0 sepal     (1000) sepal      (986)        0 2024-02-24 12:36:02.079619 aleph-message-0.4.4/aleph_message/
--rw-r--r--   0 sepal     (1000) sepal      (986)      123 2024-02-24 12:35:01.000000 aleph-message-0.4.4/aleph_message/__init__.py
--rw-r--r--   0 sepal     (1000) sepal      (986)       40 2024-02-24 12:16:29.000000 aleph-message-0.4.4/aleph_message/exceptions.py
-drwxr-xr-x   0 sepal     (1000) sepal      (986)        0 2024-02-24 12:36:02.080619 aleph-message-0.4.4/aleph_message/models/
--rw-r--r--   0 sepal     (1000) sepal      (986)    12522 2024-02-24 12:16:29.000000 aleph-message-0.4.4/aleph_message/models/__init__.py
--rw-r--r--   0 sepal     (1000) sepal      (986)      698 2023-01-12 17:02:10.000000 aleph-message-0.4.4/aleph_message/models/abstract.py
--rw-r--r--   0 sepal     (1000) sepal      (986)      551 2024-02-24 12:16:29.000000 aleph-message-0.4.4/aleph_message/models/base.py
-drwxr-xr-x   0 sepal     (1000) sepal      (986)        0 2024-02-24 12:36:02.081619 aleph-message-0.4.4/aleph_message/models/execution/
--rw-r--r--   0 sepal     (1000) sepal      (986)      192 2023-05-12 16:19:21.000000 aleph-message-0.4.4/aleph_message/models/execution/__init__.py
--rw-r--r--   0 sepal     (1000) sepal      (986)     1557 2024-02-24 12:16:29.000000 aleph-message-0.4.4/aleph_message/models/execution/abstract.py
--rw-r--r--   0 sepal     (1000) sepal      (986)     1259 2024-02-24 12:16:29.000000 aleph-message-0.4.4/aleph_message/models/execution/base.py
--rw-r--r--   0 sepal     (1000) sepal      (986)     3471 2024-02-24 12:16:29.000000 aleph-message-0.4.4/aleph_message/models/execution/environment.py
--rw-r--r--   0 sepal     (1000) sepal      (986)      903 2024-02-24 12:16:29.000000 aleph-message-0.4.4/aleph_message/models/execution/instance.py
--rw-r--r--   0 sepal     (1000) sepal      (986)     2090 2024-02-24 12:16:29.000000 aleph-message-0.4.4/aleph_message/models/execution/program.py
--rw-r--r--   0 sepal     (1000) sepal      (986)     1585 2024-02-24 12:16:29.000000 aleph-message-0.4.4/aleph_message/models/execution/volume.py
--rw-r--r--   0 sepal     (1000) sepal      (986)     1831 2023-05-12 16:19:21.000000 aleph-message-0.4.4/aleph_message/models/item_hash.py
--rw-r--r--   0 sepal     (1000) sepal      (986)      483 2023-05-12 16:19:21.000000 aleph-message-0.4.4/aleph_message/status.py
--rw-r--r--   0 sepal     (1000) sepal      (986)      505 2023-05-12 16:19:21.000000 aleph-message-0.4.4/aleph_message/utils.py
-drwxr-xr-x   0 sepal     (1000) sepal      (986)        0 2024-02-24 12:36:02.079619 aleph-message-0.4.4/aleph_message.egg-info/
--rw-r--r--   0 sepal     (1000) sepal      (986)     2080 2024-02-24 12:36:01.000000 aleph-message-0.4.4/aleph_message.egg-info/PKG-INFO
--rw-r--r--   0 sepal     (1000) sepal      (986)      737 2024-02-24 12:36:02.000000 aleph-message-0.4.4/aleph_message.egg-info/SOURCES.txt
--rw-r--r--   0 sepal     (1000) sepal      (986)        1 2024-02-24 12:36:01.000000 aleph-message-0.4.4/aleph_message.egg-info/dependency_links.txt
--rw-r--r--   0 sepal     (1000) sepal      (986)       49 2024-02-24 12:36:01.000000 aleph-message-0.4.4/aleph_message.egg-info/requires.txt
--rw-r--r--   0 sepal     (1000) sepal      (986)       14 2024-02-24 12:36:01.000000 aleph-message-0.4.4/aleph_message.egg-info/top_level.txt
--rw-r--r--   0 sepal     (1000) sepal      (986)       38 2024-02-24 12:36:02.082619 aleph-message-0.4.4/setup.cfg
--rw-r--r--   0 sepal     (1000) sepal      (986)     1813 2024-02-24 12:34:30.000000 aleph-message-0.4.4/setup.py
+drwxr-xr-x   0 sepal     (1000) sepal      (986)        0 2024-05-08 13:16:10.008906 aleph-message-0.4.5/
+-rw-r--r--   0 sepal     (1000) sepal      (986)       37 2023-01-12 17:02:10.000000 aleph-message-0.4.5/.dockerignore
+-rw-r--r--   0 sepal     (1000) sepal      (986)      264 2024-02-24 12:16:29.000000 aleph-message-0.4.5/Dockerfile
+-rw-r--r--   0 sepal     (1000) sepal      (986)     1062 2023-01-12 17:02:10.000000 aleph-message-0.4.5/LICENSE
+-rw-r--r--   0 sepal     (1000) sepal      (986)      200 2024-05-08 13:11:17.000000 aleph-message-0.4.5/MANIFEST.in
+-rw-r--r--   0 sepal     (1000) sepal      (986)     2080 2024-05-08 13:16:10.007906 aleph-message-0.4.5/PKG-INFO
+-rw-r--r--   0 sepal     (1000) sepal      (986)     1468 2023-05-12 16:19:21.000000 aleph-message-0.4.5/README.md
+drwxr-xr-x   0 sepal     (1000) sepal      (986)        0 2024-05-08 13:16:09.999906 aleph-message-0.4.5/aleph_message/
+-rw-r--r--   0 sepal     (1000) sepal      (986)      123 2024-05-08 13:13:37.000000 aleph-message-0.4.5/aleph_message/__init__.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)       40 2024-02-24 12:16:29.000000 aleph-message-0.4.5/aleph_message/exceptions.py
+drwxr-xr-x   0 sepal     (1000) sepal      (986)        0 2024-05-08 13:16:10.002906 aleph-message-0.4.5/aleph_message/models/
+-rw-r--r--   0 sepal     (1000) sepal      (986)    12522 2024-02-24 12:16:29.000000 aleph-message-0.4.5/aleph_message/models/__init__.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)      698 2023-01-12 17:02:10.000000 aleph-message-0.4.5/aleph_message/models/abstract.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)      551 2024-02-24 12:16:29.000000 aleph-message-0.4.5/aleph_message/models/base.py
+drwxr-xr-x   0 sepal     (1000) sepal      (986)        0 2024-05-08 13:16:10.004906 aleph-message-0.4.5/aleph_message/models/execution/
+-rw-r--r--   0 sepal     (1000) sepal      (986)      192 2023-05-12 16:19:21.000000 aleph-message-0.4.5/aleph_message/models/execution/__init__.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)     1557 2024-02-24 12:16:29.000000 aleph-message-0.4.5/aleph_message/models/execution/abstract.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)     1259 2024-02-24 12:16:29.000000 aleph-message-0.4.5/aleph_message/models/execution/base.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)     3471 2024-02-24 12:16:29.000000 aleph-message-0.4.5/aleph_message/models/execution/environment.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)      903 2024-02-24 12:16:29.000000 aleph-message-0.4.5/aleph_message/models/execution/instance.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)     2090 2024-02-24 12:16:29.000000 aleph-message-0.4.5/aleph_message/models/execution/program.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)     1585 2024-02-24 12:16:29.000000 aleph-message-0.4.5/aleph_message/models/execution/volume.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)     1831 2023-05-12 16:19:21.000000 aleph-message-0.4.5/aleph_message/models/item_hash.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)        0 2024-05-08 13:11:17.000000 aleph-message-0.4.5/aleph_message/py.typed
+-rw-r--r--   0 sepal     (1000) sepal      (986)      483 2023-05-12 16:19:21.000000 aleph-message-0.4.5/aleph_message/status.py
+drwxr-xr-x   0 sepal     (1000) sepal      (986)        0 2024-05-08 13:16:10.005906 aleph-message-0.4.5/aleph_message/tests/
+-rw-r--r--   0 sepal     (1000) sepal      (986)        0 2023-01-12 17:02:10.000000 aleph-message-0.4.5/aleph_message/tests/__init__.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)      870 2023-01-12 17:02:10.000000 aleph-message-0.4.5/aleph_message/tests/download_messages.py
+drwxr-xr-x   0 sepal     (1000) sepal      (986)        0 2024-05-08 13:16:10.006906 aleph-message-0.4.5/aleph_message/tests/messages/
+-rw-r--r--   0 sepal     (1000) sepal      (986)      898 2023-01-12 17:02:10.000000 aleph-message-0.4.5/aleph_message/tests/messages/forget.json
+-rw-r--r--   0 sepal     (1000) sepal      (986)     3862 2023-07-11 11:00:15.000000 aleph-message-0.4.5/aleph_message/tests/messages/instance_machine.json
+-rw-r--r--   0 sepal     (1000) sepal      (986)     4017 2023-05-10 14:28:55.000000 aleph-message-0.4.5/aleph_message/tests/messages/machine.json
+-rw-r--r--   0 sepal     (1000) sepal      (986)     3962 2023-05-10 14:28:55.000000 aleph-message-0.4.5/aleph_message/tests/messages/machine_named.json
+-rw-r--r--   0 sepal     (1000) sepal      (986)     9953 2024-02-24 12:16:29.000000 aleph-message-0.4.5/aleph_message/tests/test_models.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)      122 2023-05-12 16:19:21.000000 aleph-message-0.4.5/aleph_message/tests/test_status.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)     2412 2023-05-12 16:19:21.000000 aleph-message-0.4.5/aleph_message/tests/test_types.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)      209 2023-05-12 16:19:21.000000 aleph-message-0.4.5/aleph_message/tests/test_utils.py
+-rw-r--r--   0 sepal     (1000) sepal      (986)      505 2023-05-12 16:19:21.000000 aleph-message-0.4.5/aleph_message/utils.py
+drwxr-xr-x   0 sepal     (1000) sepal      (986)        0 2024-05-08 13:16:10.000906 aleph-message-0.4.5/aleph_message.egg-info/
+-rw-r--r--   0 sepal     (1000) sepal      (986)     2080 2024-05-08 13:16:09.000000 aleph-message-0.4.5/aleph_message.egg-info/PKG-INFO
+-rw-r--r--   0 sepal     (1000) sepal      (986)     1209 2024-05-08 13:16:09.000000 aleph-message-0.4.5/aleph_message.egg-info/SOURCES.txt
+-rw-r--r--   0 sepal     (1000) sepal      (986)        1 2024-05-08 13:16:09.000000 aleph-message-0.4.5/aleph_message.egg-info/dependency_links.txt
+-rw-r--r--   0 sepal     (1000) sepal      (986)       49 2024-05-08 13:16:09.000000 aleph-message-0.4.5/aleph_message.egg-info/requires.txt
+-rw-r--r--   0 sepal     (1000) sepal      (986)       14 2024-05-08 13:16:09.000000 aleph-message-0.4.5/aleph_message.egg-info/top_level.txt
+-rw-r--r--   0 sepal     (1000) sepal      (986)       81 2023-01-12 17:02:10.000000 aleph-message-0.4.5/pytest.ini
+-rw-r--r--   0 sepal     (1000) sepal      (986)       38 2024-05-08 13:16:10.008906 aleph-message-0.4.5/setup.cfg
+-rw-r--r--   0 sepal     (1000) sepal      (986)     1813 2024-04-24 18:15:46.000000 aleph-message-0.4.5/setup.py
+-rwxr-xr-x   0 sepal     (1000) sepal      (986)      275 2023-05-31 12:29:26.000000 aleph-message-0.4.5/test.sh
```

### Comparing `aleph-message-0.4.4/LICENSE` & `aleph-message-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.4/PKG-INFO` & `aleph-message-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-message
-Version: 0.4.4
+Version: 0.4.5
 Summary: Aleph.im message specification 
 Home-page: https://github.com/aleph-im/aleph-message
 Author: Hugo Herter
 Author-email: git@hugoherter.com
 License: MIT
 Keywords: aleph.im message validation specification
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aleph-message-0.4.4/README.md` & `aleph-message-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.4/aleph_message/models/__init__.py` & `aleph-message-0.4.5/aleph_message/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.4/aleph_message/models/abstract.py` & `aleph-message-0.4.5/aleph_message/models/abstract.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.4/aleph_message/models/base.py` & `aleph-message-0.4.5/aleph_message/models/base.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.4/aleph_message/models/execution/abstract.py` & `aleph-message-0.4.5/aleph_message/models/execution/abstract.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.4/aleph_message/models/execution/base.py` & `aleph-message-0.4.5/aleph_message/models/execution/base.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.4/aleph_message/models/execution/environment.py` & `aleph-message-0.4.5/aleph_message/models/execution/environment.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.4/aleph_message/models/execution/instance.py` & `aleph-message-0.4.5/aleph_message/models/execution/instance.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.4/aleph_message/models/execution/program.py` & `aleph-message-0.4.5/aleph_message/models/execution/program.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.4/aleph_message/models/execution/volume.py` & `aleph-message-0.4.5/aleph_message/models/execution/volume.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.4/aleph_message/models/item_hash.py` & `aleph-message-0.4.5/aleph_message/models/item_hash.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.4/aleph_message.egg-info/PKG-INFO` & `aleph-message-0.4.5/aleph_message.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-message
-Version: 0.4.4
+Version: 0.4.5
 Summary: Aleph.im message specification 
 Home-page: https://github.com/aleph-im/aleph-message
 Author: Hugo Herter
 Author-email: git@hugoherter.com
 License: MIT
 Keywords: aleph.im message validation specification
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aleph-message-0.4.4/aleph_message.egg-info/SOURCES.txt` & `aleph-message-0.4.5/aleph_message.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+.dockerignore
+Dockerfile
 LICENSE
+MANIFEST.in
 README.md
+pytest.ini
 setup.py
+test.sh
 aleph_message/__init__.py
 aleph_message/exceptions.py
+aleph_message/py.typed
 aleph_message/status.py
 aleph_message/utils.py
 aleph_message.egg-info/PKG-INFO
 aleph_message.egg-info/SOURCES.txt
 aleph_message.egg-info/dependency_links.txt
 aleph_message.egg-info/requires.txt
 aleph_message.egg-info/top_level.txt
@@ -16,8 +22,18 @@
 aleph_message/models/item_hash.py
 aleph_message/models/execution/__init__.py
 aleph_message/models/execution/abstract.py
 aleph_message/models/execution/base.py
 aleph_message/models/execution/environment.py
 aleph_message/models/execution/instance.py
 aleph_message/models/execution/program.py
-aleph_message/models/execution/volume.py
+aleph_message/models/execution/volume.py
+aleph_message/tests/__init__.py
+aleph_message/tests/download_messages.py
+aleph_message/tests/test_models.py
+aleph_message/tests/test_status.py
+aleph_message/tests/test_types.py
+aleph_message/tests/test_utils.py
+aleph_message/tests/messages/forget.json
+aleph_message/tests/messages/instance_machine.json
+aleph_message/tests/messages/machine.json
+aleph_message/tests/messages/machine_named.json
```

### Comparing `aleph-message-0.4.4/setup.py` & `aleph-message-0.4.5/setup.py`

 * *Files identical despite different names*

