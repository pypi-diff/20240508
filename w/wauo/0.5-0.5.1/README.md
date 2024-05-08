# Comparing `tmp/wauo-0.5.tar.gz` & `tmp/wauo-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wauo-0.5.tar", last modified: Wed May  8 14:17:40 2024, max compression
+gzip compressed data, was "wauo-0.5.1.tar", last modified: Wed May  8 16:39:51 2024, max compression
```

## Comparing `wauo-0.5.tar` & `wauo-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-08 14:17:40.508250 wauo-0.5/
--rw-r--r--   0 wangtuo    (501) staff       (20)     1592 2024-05-08 14:17:40.508051 wauo-0.5/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)     1335 2024-04-28 13:29:40.000000 wauo-0.5/README.md
--rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-08 14:17:40.508287 wauo-0.5/setup.cfg
--rw-r--r--   0 wangtuo    (501) staff       (20)      613 2024-05-08 14:17:31.000000 wauo-0.5/setup.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-08 14:17:40.507063 wauo-0.5/wauo/
--rw-r--r--   0 wangtuo    (501) staff       (20)       95 2024-05-03 02:43:04.000000 wauo-0.5/wauo/__init__.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      345 2023-11-08 06:17:07.000000 wauo-0.5/wauo/exceptions.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      789 2024-05-03 11:40:02.000000 wauo-0.5/wauo/response.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     5228 2024-05-08 14:14:02.000000 wauo-0.5/wauo/spiders.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      351 2024-05-03 14:44:50.000000 wauo-0.5/wauo/test.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-08 14:17:40.507904 wauo-0.5/wauo.egg-info/
--rw-r--r--   0 wangtuo    (501) staff       (20)     1592 2024-05-08 14:17:40.000000 wauo-0.5/wauo.egg-info/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)      266 2024-05-08 14:17:40.000000 wauo-0.5/wauo.egg-info/SOURCES.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-08 14:17:40.000000 wauo-0.5/wauo.egg-info/dependency_links.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-08 14:17:40.000000 wauo-0.5/wauo.egg-info/not-zip-safe
--rw-r--r--   0 wangtuo    (501) staff       (20)       31 2024-05-08 14:17:40.000000 wauo-0.5/wauo.egg-info/requires.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        5 2024-05-08 14:17:40.000000 wauo-0.5/wauo.egg-info/top_level.txt
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-08 16:39:51.708965 wauo-0.5.1/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1594 2024-05-08 16:39:51.708759 wauo-0.5.1/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1335 2024-04-28 13:29:40.000000 wauo-0.5.1/README.md
+-rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-08 16:39:51.709002 wauo-0.5.1/setup.cfg
+-rw-r--r--   0 wangtuo    (501) staff       (20)      638 2024-05-08 16:39:44.000000 wauo-0.5.1/setup.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-08 16:39:51.707699 wauo-0.5.1/wauo/
+-rw-r--r--   0 wangtuo    (501) staff       (20)       95 2024-05-03 02:43:04.000000 wauo-0.5.1/wauo/__init__.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      345 2023-11-08 06:17:07.000000 wauo-0.5.1/wauo/exceptions.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      789 2024-05-03 11:40:02.000000 wauo-0.5.1/wauo/response.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     5228 2024-05-08 14:14:02.000000 wauo-0.5.1/wauo/spiders.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      351 2024-05-03 14:44:50.000000 wauo-0.5.1/wauo/test.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-08 16:39:51.708599 wauo-0.5.1/wauo.egg-info/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1594 2024-05-08 16:39:51.000000 wauo-0.5.1/wauo.egg-info/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)      266 2024-05-08 16:39:51.000000 wauo-0.5.1/wauo.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-08 16:39:51.000000 wauo-0.5.1/wauo.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-08 16:39:51.000000 wauo-0.5.1/wauo.egg-info/not-zip-safe
+-rw-r--r--   0 wangtuo    (501) staff       (20)       54 2024-05-08 16:39:51.000000 wauo-0.5.1/wauo.egg-info/requires.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        5 2024-05-08 16:39:51.000000 wauo-0.5.1/wauo.egg-info/top_level.txt
```

### Comparing `wauo-0.5/PKG-INFO` & `wauo-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wauo
-Version: 0.5
+Version: 0.5.1
 Summary: 爬虫者的贴心助手
 Home-page: https://github.com/markadc/wauo
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: python,requests,spider
 Description-Content-Type: text/markdown
```

### Comparing `wauo-0.5/README.md` & `wauo-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `wauo-0.5/setup.py` & `wauo-0.5.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='wauo',
-    version='0.5',
+    version='0.5.1',
     description='爬虫者的贴心助手',
     url='https://github.com/markadc/wauo',
     author='WangTuo',
     author_email='markadc@126.com',
     packages=find_packages(),
     license='MIT',
     zip_safe=False,
-    install_requires=['requests', 'fake_useragent', 'loguru'],
+    install_requires=['requests==2.28.1', 'fake_useragent==0.1.11', 'loguru==0.5.3'],
     keywords=['python', 'requests', 'spider'],
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

### Comparing `wauo-0.5/wauo/response.py` & `wauo-0.5.1/wauo/response.py`

 * *Files identical despite different names*

### Comparing `wauo-0.5/wauo/spiders.py` & `wauo-0.5.1/wauo/spiders.py`

 * *Files identical despite different names*

### Comparing `wauo-0.5/wauo.egg-info/PKG-INFO` & `wauo-0.5.1/wauo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wauo
-Version: 0.5
+Version: 0.5.1
 Summary: 爬虫者的贴心助手
 Home-page: https://github.com/markadc/wauo
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: python,requests,spider
 Description-Content-Type: text/markdown
```

