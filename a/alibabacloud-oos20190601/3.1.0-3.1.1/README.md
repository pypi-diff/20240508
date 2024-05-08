# Comparing `tmp/alibabacloud_oos20190601-3.1.0.tar.gz` & `tmp/alibabacloud_oos20190601-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_oos20190601-3.1.0.tar", last modified: Thu Apr 18 17:13:21 2024, max compression
+gzip compressed data, was "dist/alibabacloud_oos20190601-3.1.1.tar", last modified: Wed May  8 17:09:55 2024, max compression
```

## Comparing `alibabacloud_oos20190601-3.1.0.tar` & `alibabacloud_oos20190601-3.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2429 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/alibabacloud_oos20190601/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/alibabacloud_oos20190601/__init__.py
--rw-r--r--   0 root         (0) root         (0)   326897 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/alibabacloud_oos20190601/client.py
--rw-r--r--   0 root         (0) root         (0)   776825 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/alibabacloud_oos20190601/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/alibabacloud_oos20190601.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2429 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/alibabacloud_oos20190601.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/alibabacloud_oos20190601.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/alibabacloud_oos20190601.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/alibabacloud_oos20190601.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/alibabacloud_oos20190601.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2639 2024-04-18 17:13:21.000000 alibabacloud_oos20190601-3.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 17:09:55.000000 alibabacloud_oos20190601-3.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1370 2024-05-08 17:09:54.000000 alibabacloud_oos20190601-3.1.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-08 17:09:54.000000 alibabacloud_oos20190601-3.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-08 17:09:54.000000 alibabacloud_oos20190601-3.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-05-08 17:09:55.000000 alibabacloud_oos20190601-3.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-08 17:09:54.000000 alibabacloud_oos20190601-3.1.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-05-08 17:09:54.000000 alibabacloud_oos20190601-3.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 17:09:55.000000 alibabacloud_oos20190601-3.1.1/alibabacloud_oos20190601/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-08 17:09:54.000000 alibabacloud_oos20190601-3.1.1/alibabacloud_oos20190601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   326897 2024-05-08 17:09:54.000000 alibabacloud_oos20190601-3.1.1/alibabacloud_oos20190601/client.py
+-rw-r--r--   0 root         (0) root         (0)   776825 2024-05-08 17:09:54.000000 alibabacloud_oos20190601-3.1.1/alibabacloud_oos20190601/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 17:09:55.000000 alibabacloud_oos20190601-3.1.1/alibabacloud_oos20190601.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-05-08 17:09:54.000000 alibabacloud_oos20190601-3.1.1/alibabacloud_oos20190601.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-05-08 17:09:55.000000 alibabacloud_oos20190601-3.1.1/alibabacloud_oos20190601.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 17:09:54.000000 alibabacloud_oos20190601-3.1.1/alibabacloud_oos20190601.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-08 17:09:54.000000 alibabacloud_oos20190601-3.1.1/alibabacloud_oos20190601.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-08 17:09:54.000000 alibabacloud_oos20190601-3.1.1/alibabacloud_oos20190601.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-08 17:09:55.000000 alibabacloud_oos20190601-3.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2639 2024-05-08 17:09:54.000000 alibabacloud_oos20190601-3.1.1/setup.py
```

### Comparing `alibabacloud_oos20190601-3.1.0/LICENSE` & `alibabacloud_oos20190601-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_oos20190601-3.1.0/PKG-INFO` & `alibabacloud_oos20190601-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_oos20190601
-Version: 3.1.0
+Version: 3.1.1
 Summary: Alibaba Cloud Operation Orchestration Service (20190601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oos20190601-3.1.0/README-CN.md` & `alibabacloud_oos20190601-3.1.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oos20190601-3.1.0/README.md` & `alibabacloud_oos20190601-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oos20190601-3.1.0/alibabacloud_oos20190601/client.py` & `alibabacloud_oos20190601-3.1.1/alibabacloud_oos20190601/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_oos20190601-3.1.0/alibabacloud_oos20190601/models.py` & `alibabacloud_oos20190601-3.1.1/alibabacloud_oos20190601/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_oos20190601-3.1.0/alibabacloud_oos20190601.egg-info/PKG-INFO` & `alibabacloud_oos20190601-3.1.1/alibabacloud_oos20190601.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-oos20190601
-Version: 3.1.0
+Version: 3.1.1
 Summary: Alibaba Cloud Operation Orchestration Service (20190601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oos20190601-3.1.0/setup.py` & `alibabacloud_oos20190601-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_oos20190601.
 
-Created on 18/04/2024
+Created on 08/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_oos20190601"
 NAME = "alibabacloud_oos20190601" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Operation Orchestration Service (20190601) SDK Library for Python"
```

