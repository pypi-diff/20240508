# Comparing `tmp/lazysdk-0.1.90.tar.gz` & `tmp/lazysdk-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazysdk-0.1.90.tar", last modified: Wed Apr 24 09:31:29 2024, max compression
+gzip compressed data, was "lazysdk-0.1.91.tar", last modified: Tue May  7 04:00:37 2024, max compression
```

## Comparing `lazysdk-0.1.90.tar` & `lazysdk-0.1.91.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-24 09:31:29.453055 lazysdk-0.1.90/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1088 2023-12-14 08:15:44.000000 lazysdk-0.1.90/LICENSE
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1898 2024-04-24 09:31:29.452845 lazysdk-0.1.90/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1073 2023-12-30 02:37:03.000000 lazysdk-0.1.90/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-24 09:31:29.451857 lazysdk-0.1.90/lazysdk/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      184 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      389 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyCrypto.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2797 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazy_id_card.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      669 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazybase64.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      571 2024-02-02 03:54:22.000000 lazysdk-0.1.90/lazysdk/lazycache.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    15383 2023-12-25 11:22:47.000000 lazysdk-0.1.90/lazysdk/lazychromedriver.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      414 2024-02-01 03:07:43.000000 lazysdk-0.1.90/lazysdk/lazydecode.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     8883 2024-01-09 11:35:26.000000 lazysdk-0.1.90/lazysdk/lazydict.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3024 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyenv.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    15835 2024-02-02 07:00:02.000000 lazysdk-0.1.90/lazysdk/lazyexcel.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    20263 2024-02-04 08:23:46.000000 lazysdk-0.1.90/lazysdk/lazyfile.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      727 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyflask.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1867 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyhtml.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1287 2024-01-27 02:46:52.000000 lazysdk-0.1.90/lazysdk/lazyid.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3673 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyinfo.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1364 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyip.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      867 2024-01-18 03:56:02.000000 lazysdk-0.1.90/lazysdk/lazyjson.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      363 2024-04-24 09:30:41.000000 lazysdk-0.1.90/lazysdk/lazylist.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    31937 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazym3u8.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1112 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazymd5.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     5922 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazypath.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    17702 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyprocess.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      546 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyproxies.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1420 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyrandom.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    37918 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyredis.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3750 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyrequests.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2627 2024-03-22 06:24:43.000000 lazysdk-0.1.90/lazysdk/lazytext.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    26530 2024-02-02 08:29:53.000000 lazysdk-0.1.90/lazysdk/lazytime.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     4827 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyua.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1550 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyurl.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     8386 2024-02-05 09:57:19.000000 lazysdk-0.1.90/lazysdk/lazywebhook.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      716 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazywifi.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      770 2024-03-22 06:19:36.000000 lazysdk-0.1.90/lazysdk/lazyxml.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1683 2023-12-26 07:19:36.000000 lazysdk-0.1.90/lazysdk/showdata.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-24 09:31:29.452586 lazysdk-0.1.90/lazysdk.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1898 2024-04-24 09:31:29.000000 lazysdk-0.1.90/lazysdk.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      887 2024-04-24 09:31:29.000000 lazysdk-0.1.90/lazysdk.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-04-24 09:31:29.000000 lazysdk-0.1.90/lazysdk.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)      216 2024-04-24 09:31:29.000000 lazysdk-0.1.90/lazysdk.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        8 2024-04-24 09:31:29.000000 lazysdk-0.1.90/lazysdk.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-04-24 09:31:29.453105 lazysdk-0.1.90/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1208 2024-04-24 09:30:41.000000 lazysdk-0.1.90/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-05-07 04:00:37.361200 lazysdk-0.1.91/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1088 2023-12-14 08:15:44.000000 lazysdk-0.1.91/LICENSE
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1898 2024-05-07 04:00:37.360974 lazysdk-0.1.91/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1073 2023-12-30 02:37:03.000000 lazysdk-0.1.91/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-05-07 04:00:37.360008 lazysdk-0.1.91/lazysdk/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      184 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      389 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazyCrypto.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2797 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazy_id_card.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      669 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazybase64.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      571 2024-02-02 03:54:22.000000 lazysdk-0.1.91/lazysdk/lazycache.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    15383 2023-12-25 11:22:47.000000 lazysdk-0.1.91/lazysdk/lazychromedriver.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      414 2024-02-01 03:07:43.000000 lazysdk-0.1.91/lazysdk/lazydecode.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     8883 2024-01-09 11:35:26.000000 lazysdk-0.1.91/lazysdk/lazydict.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3024 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazyenv.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    15835 2024-02-02 07:00:02.000000 lazysdk-0.1.91/lazysdk/lazyexcel.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    20263 2024-02-04 08:23:46.000000 lazysdk-0.1.91/lazysdk/lazyfile.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      727 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazyflask.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1867 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazyhtml.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1287 2024-01-27 02:46:52.000000 lazysdk-0.1.91/lazysdk/lazyid.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3673 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazyinfo.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1364 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazyip.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      867 2024-01-18 03:56:02.000000 lazysdk-0.1.91/lazysdk/lazyjson.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      363 2024-04-24 09:30:41.000000 lazysdk-0.1.91/lazysdk/lazylist.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    31937 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazym3u8.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1112 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazymd5.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     5922 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazypath.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    17702 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazyprocess.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      546 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazyproxies.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1420 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazyrandom.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    37918 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazyredis.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3750 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazyrequests.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2627 2024-03-22 06:24:43.000000 lazysdk-0.1.91/lazysdk/lazytext.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    26530 2024-02-02 08:29:53.000000 lazysdk-0.1.91/lazysdk/lazytime.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     4827 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazyua.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1550 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazyurl.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     8937 2024-05-07 04:00:07.000000 lazysdk-0.1.91/lazysdk/lazywebhook.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      716 2023-12-14 08:15:44.000000 lazysdk-0.1.91/lazysdk/lazywifi.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      770 2024-03-22 06:19:36.000000 lazysdk-0.1.91/lazysdk/lazyxml.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1683 2023-12-26 07:19:36.000000 lazysdk-0.1.91/lazysdk/showdata.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-05-07 04:00:37.360725 lazysdk-0.1.91/lazysdk.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1898 2024-05-07 04:00:37.000000 lazysdk-0.1.91/lazysdk.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      887 2024-05-07 04:00:37.000000 lazysdk-0.1.91/lazysdk.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-05-07 04:00:37.000000 lazysdk-0.1.91/lazysdk.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      216 2024-05-07 04:00:37.000000 lazysdk-0.1.91/lazysdk.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        8 2024-05-07 04:00:37.000000 lazysdk-0.1.91/lazysdk.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-05-07 04:00:37.361251 lazysdk-0.1.91/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1208 2024-05-07 03:57:45.000000 lazysdk-0.1.91/setup.py
```

### Comparing `lazysdk-0.1.90/LICENSE` & `lazysdk-0.1.91/LICENSE`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/PKG-INFO` & `lazysdk-0.1.91/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazysdk
-Version: 0.1.90
+Version: 0.1.91
 Summary: 基于Python的懒人包
 Home-page: https://gitee.com/ZeroSeeker/lazysdk
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lazysdk-0.1.90/README.md` & `lazysdk-0.1.91/README.md`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazy_id_card.py` & `lazysdk-0.1.91/lazysdk/lazy_id_card.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazybase64.py` & `lazysdk-0.1.91/lazysdk/lazybase64.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazycache.py` & `lazysdk-0.1.91/lazysdk/lazycache.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazychromedriver.py` & `lazysdk-0.1.91/lazysdk/lazychromedriver.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazydict.py` & `lazysdk-0.1.91/lazysdk/lazydict.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyenv.py` & `lazysdk-0.1.91/lazysdk/lazyenv.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyexcel.py` & `lazysdk-0.1.91/lazysdk/lazyexcel.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyfile.py` & `lazysdk-0.1.91/lazysdk/lazyfile.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyflask.py` & `lazysdk-0.1.91/lazysdk/lazyflask.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyhtml.py` & `lazysdk-0.1.91/lazysdk/lazyhtml.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyid.py` & `lazysdk-0.1.91/lazysdk/lazyid.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyinfo.py` & `lazysdk-0.1.91/lazysdk/lazyinfo.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyip.py` & `lazysdk-0.1.91/lazysdk/lazyip.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyjson.py` & `lazysdk-0.1.91/lazysdk/lazyjson.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazym3u8.py` & `lazysdk-0.1.91/lazysdk/lazym3u8.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazymd5.py` & `lazysdk-0.1.91/lazysdk/lazymd5.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazypath.py` & `lazysdk-0.1.91/lazysdk/lazypath.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyprocess.py` & `lazysdk-0.1.91/lazysdk/lazyprocess.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyproxies.py` & `lazysdk-0.1.91/lazysdk/lazyproxies.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyrandom.py` & `lazysdk-0.1.91/lazysdk/lazyrandom.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyredis.py` & `lazysdk-0.1.91/lazysdk/lazyredis.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyrequests.py` & `lazysdk-0.1.91/lazysdk/lazyrequests.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazytext.py` & `lazysdk-0.1.91/lazysdk/lazytext.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazytime.py` & `lazysdk-0.1.91/lazysdk/lazytime.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyua.py` & `lazysdk-0.1.91/lazysdk/lazyua.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyurl.py` & `lazysdk-0.1.91/lazysdk/lazyurl.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazywebhook.py` & `lazysdk-0.1.91/lazysdk/lazywebhook.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # coding = utf8
 """
 @ Author : ZeroSeeker
 @ e-mail : zeroseeker@foxmail.com
 @ GitHub : https://github.com/ZeroSeeker
 @ Gitee : https://gitee.com/ZeroSeeker
 """
+import time
+
 from lazysdk import lazyrequests
 import showlog
 import json
 import envx
 from urllib.parse import urlparse
 
 """
@@ -198,15 +200,17 @@
         msg: str = None,
 
         env_file_name: str = None,
         webhook: str = None,
         at_ids: list = None,
         at_mobiles: list = None,
         is_at: bool = None,
-        at_all: bool = None
+        at_all: bool = None,
+        ensure_success: bool = False,
+        ensure_success_limit: int = 60
 ):
     """
     在内部实例化，
     首先使用自定义参数，其次使用env参数
     """
     if env_file_name is not None:
         env_con_info = make_con_info(env_file_name=env_file_name)
@@ -229,18 +233,30 @@
         'webhook': webhook,
         'at_ids': at_ids,
         'at_mobiles': at_mobiles
     }
     webhook_hostname = urlparse(webhook).hostname
     if webhook_hostname == 'qyapi.weixin.qq.com':
         webhook_basic = WeixinBasics(con_info=con_info)
-        response = webhook_basic.send_text(
-            msg=msg,
-            con_info=con_info,
-            at_ids=at_ids,
-            at_mobiles=at_mobiles,
-            is_at=is_at,
-            at_all=at_all
-        )
-        return response
+        retry_count = 0
+        while True:
+            response = webhook_basic.send_text(
+                msg=msg,
+                con_info=con_info,
+                at_ids=at_ids,
+                at_mobiles=at_mobiles,
+                is_at=is_at,
+                at_all=at_all
+            )
+            if not ensure_success:
+                return response
+            else:
+                if response.get('errcode') == 0:
+                    return response
+                else:
+                    showlog.warning(response)
+                    retry_count += 1
+                    if retry_count > ensure_success_limit:
+                        return response
+                    time.sleep(1)
     else:
         return {'errcode': -2, 'errmsg': '暂不支持此webhook'}
```

### Comparing `lazysdk-0.1.90/lazysdk/lazywifi.py` & `lazysdk-0.1.91/lazysdk/lazywifi.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/lazyxml.py` & `lazysdk-0.1.91/lazysdk/lazyxml.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk/showdata.py` & `lazysdk-0.1.91/lazysdk/showdata.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/lazysdk.egg-info/PKG-INFO` & `lazysdk-0.1.91/lazysdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazysdk
-Version: 0.1.90
+Version: 0.1.91
 Summary: 基于Python的懒人包
 Home-page: https://gitee.com/ZeroSeeker/lazysdk
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lazysdk-0.1.90/lazysdk.egg-info/SOURCES.txt` & `lazysdk-0.1.91/lazysdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.90/setup.py` & `lazysdk-0.1.91/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazysdk",
-    version="0.1.90",
+    version="0.1.91",
     description="基于Python的懒人包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazysdk",
     packages=setuptools.find_packages(),
```

