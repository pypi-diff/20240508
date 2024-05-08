# Comparing `tmp/alibabacloud_mns-open20220119-1.0.1.tar.gz` & `tmp/alibabacloud_mns-open20220119-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_mns-open20220119-1.0.1.tar", last modified: Wed Apr 10 10:13:58 2024, max compression
+gzip compressed data, was "dist/alibabacloud_mns-open20220119-1.0.2.tar", last modified: Wed May  8 17:09:39 2024, max compression
```

## Comparing `alibabacloud_mns-open20220119-1.0.1.tar` & `alibabacloud_mns-open20220119-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       54 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48282 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119/client.py
--rw-r--r--   0 root         (0) root         (0)    96228 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2638 2024-04-10 10:13:58.000000 alibabacloud_mns-open20220119-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      125 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48282 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119/client.py
+-rw-r--r--   0 root         (0) root         (0)    96763 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2638 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/setup.py
```

### Comparing `alibabacloud_mns-open20220119-1.0.1/LICENSE` & `alibabacloud_mns-open20220119-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_mns-open20220119-1.0.1/PKG-INFO` & `alibabacloud_mns-open20220119-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_mns-open20220119
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud Mns-open (20220119) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mns-open20220119-1.0.1/README-CN.md` & `alibabacloud_mns-open20220119-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mns-open20220119-1.0.1/README.md` & `alibabacloud_mns-open20220119-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119/client.py` & `alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119/models.py` & `alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1919,23 +1919,27 @@
         self,
         create_time: int = None,
         last_modify_time: int = None,
         logging_enabled: bool = None,
         max_message_size: int = None,
         message_count: int = None,
         message_retention_period: int = None,
+        topic_inner_url: str = None,
         topic_name: str = None,
+        topic_url: str = None,
     ):
         self.create_time = create_time
         self.last_modify_time = last_modify_time
         self.logging_enabled = logging_enabled
         self.max_message_size = max_message_size
         self.message_count = message_count
         self.message_retention_period = message_retention_period
+        self.topic_inner_url = topic_inner_url
         self.topic_name = topic_name
+        self.topic_url = topic_url
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -1950,16 +1954,20 @@
             result['LoggingEnabled'] = self.logging_enabled
         if self.max_message_size is not None:
             result['MaxMessageSize'] = self.max_message_size
         if self.message_count is not None:
             result['MessageCount'] = self.message_count
         if self.message_retention_period is not None:
             result['MessageRetentionPeriod'] = self.message_retention_period
+        if self.topic_inner_url is not None:
+            result['TopicInnerUrl'] = self.topic_inner_url
         if self.topic_name is not None:
             result['TopicName'] = self.topic_name
+        if self.topic_url is not None:
+            result['TopicUrl'] = self.topic_url
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('LastModifyTime') is not None:
@@ -1968,16 +1976,20 @@
             self.logging_enabled = m.get('LoggingEnabled')
         if m.get('MaxMessageSize') is not None:
             self.max_message_size = m.get('MaxMessageSize')
         if m.get('MessageCount') is not None:
             self.message_count = m.get('MessageCount')
         if m.get('MessageRetentionPeriod') is not None:
             self.message_retention_period = m.get('MessageRetentionPeriod')
+        if m.get('TopicInnerUrl') is not None:
+            self.topic_inner_url = m.get('TopicInnerUrl')
         if m.get('TopicName') is not None:
             self.topic_name = m.get('TopicName')
+        if m.get('TopicUrl') is not None:
+            self.topic_url = m.get('TopicUrl')
         return self
 
 
 class ListTopicResponseBodyData(TeaModel):
     def __init__(
         self,
         page_data: List[ListTopicResponseBodyDataPageData] = None,
```

### Comparing `alibabacloud_mns-open20220119-1.0.1/alibabacloud_mns_open20220119.egg-info/PKG-INFO` & `alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-mns-open20220119
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud Mns-open (20220119) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mns-open20220119-1.0.1/setup.py` & `alibabacloud_mns-open20220119-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_mns-open20220119.
 
-Created on 10/04/2024
+Created on 08/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_mns_open20220119"
 NAME = "alibabacloud_mns-open20220119" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Mns-open (20220119) SDK Library for Python"
```

