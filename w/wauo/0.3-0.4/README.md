# Comparing `tmp/wauo-0.3.tar.gz` & `tmp/wauo-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wauo-0.3.tar", last modified: Tue May  7 13:16:24 2024, max compression
+gzip compressed data, was "wauo-0.4.tar", last modified: Tue May  7 15:46:30 2024, max compression
```

## Comparing `wauo-0.3.tar` & `wauo-0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 13:16:24.953046 wauo-0.3/
--rw-r--r--   0 wangtuo    (501) staff       (20)     1600 2024-05-07 13:16:24.952782 wauo-0.3/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)     1335 2024-04-28 13:29:40.000000 wauo-0.3/README.md
--rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-07 13:16:24.953091 wauo-0.3/setup.cfg
--rw-r--r--   0 wangtuo    (501) staff       (20)      602 2024-05-07 13:16:18.000000 wauo-0.3/setup.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 13:16:24.951698 wauo-0.3/wauo/
--rw-r--r--   0 wangtuo    (501) staff       (20)       95 2024-05-03 02:43:04.000000 wauo-0.3/wauo/__init__.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      345 2023-11-08 06:17:07.000000 wauo-0.3/wauo/exceptions.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      789 2024-05-03 11:40:02.000000 wauo-0.3/wauo/response.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     4733 2024-05-03 14:42:18.000000 wauo-0.3/wauo/spiders.py
--rw-r--r--   0 wangtuo    (501) staff       (20)      351 2024-05-03 14:44:50.000000 wauo-0.3/wauo/test.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 13:16:24.952617 wauo-0.3/wauo.egg-info/
--rw-r--r--   0 wangtuo    (501) staff       (20)     1600 2024-05-07 13:16:24.000000 wauo-0.3/wauo.egg-info/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)      266 2024-05-07 13:16:24.000000 wauo-0.3/wauo.egg-info/SOURCES.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-07 13:16:24.000000 wauo-0.3/wauo.egg-info/dependency_links.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-07 13:16:24.000000 wauo-0.3/wauo.egg-info/not-zip-safe
--rw-r--r--   0 wangtuo    (501) staff       (20)       31 2024-05-07 13:16:24.000000 wauo-0.3/wauo.egg-info/requires.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        5 2024-05-07 13:16:24.000000 wauo-0.3/wauo.egg-info/top_level.txt
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 15:46:30.664675 wauo-0.4/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1592 2024-05-07 15:46:30.664473 wauo-0.4/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1335 2024-04-28 13:29:40.000000 wauo-0.4/README.md
+-rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-07 15:46:30.664712 wauo-0.4/setup.cfg
+-rw-r--r--   0 wangtuo    (501) staff       (20)      591 2024-05-07 15:46:29.000000 wauo-0.4/setup.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 15:46:30.663268 wauo-0.4/wauo/
+-rw-r--r--   0 wangtuo    (501) staff       (20)       95 2024-05-03 02:43:04.000000 wauo-0.4/wauo/__init__.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      345 2023-11-08 06:17:07.000000 wauo-0.4/wauo/exceptions.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      789 2024-05-03 11:40:02.000000 wauo-0.4/wauo/response.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     4733 2024-05-03 14:42:18.000000 wauo-0.4/wauo/spiders.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)      351 2024-05-03 14:44:50.000000 wauo-0.4/wauo/test.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-07 15:46:30.664312 wauo-0.4/wauo.egg-info/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1592 2024-05-07 15:46:30.000000 wauo-0.4/wauo.egg-info/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)      266 2024-05-07 15:46:30.000000 wauo-0.4/wauo.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-07 15:46:30.000000 wauo-0.4/wauo.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-07 15:46:30.000000 wauo-0.4/wauo.egg-info/not-zip-safe
+-rw-r--r--   0 wangtuo    (501) staff       (20)       31 2024-05-07 15:46:30.000000 wauo-0.4/wauo.egg-info/requires.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        5 2024-05-07 15:46:30.000000 wauo-0.4/wauo.egg-info/top_level.txt
```

### Comparing `wauo-0.3/PKG-INFO` & `wauo-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wauo
-Version: 0.3
-Summary: 爬虫者的贴手助手
+Version: 0.4
+Summary: 爬虫者的贴心助手
 Home-page: https://github.com/markadc/wauo
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
-Keywords: python,python3,requests,spider
+Keywords: python,requests,spider
 Description-Content-Type: text/markdown
 
 # 项目说明
 
 - 基于requests封装的一个爬虫类
 
 # Python解释器
```

### Comparing `wauo-0.3/README.md` & `wauo-0.4/README.md`

 * *Files identical despite different names*

### Comparing `wauo-0.3/setup.py` & `wauo-0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='wauo',
-    version='0.3',
-    description='爬虫者的贴手助手',
+    version='0.4',
+    description='爬虫者的贴心助手',
     url='https://github.com/markadc/wauo',
     author='WangTuo',
     author_email='markadc@126.com',
     packages=['wauo'],
     license='MIT',
     zip_safe=False,
     install_requires=['requests', 'fake_useragent', 'loguru'],
-    keywords=['python', 'python3', 'requests', 'spider'],
+    keywords=['python', 'requests', 'spider'],
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

### Comparing `wauo-0.3/wauo/response.py` & `wauo-0.4/wauo/response.py`

 * *Files identical despite different names*

### Comparing `wauo-0.3/wauo/spiders.py` & `wauo-0.4/wauo/spiders.py`

 * *Files identical despite different names*

### Comparing `wauo-0.3/wauo.egg-info/PKG-INFO` & `wauo-0.4/wauo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wauo
-Version: 0.3
-Summary: 爬虫者的贴手助手
+Version: 0.4
+Summary: 爬虫者的贴心助手
 Home-page: https://github.com/markadc/wauo
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
-Keywords: python,python3,requests,spider
+Keywords: python,requests,spider
 Description-Content-Type: text/markdown
 
 # 项目说明
 
 - 基于requests封装的一个爬虫类
 
 # Python解释器
```

