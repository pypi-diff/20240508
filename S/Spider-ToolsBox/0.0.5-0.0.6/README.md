# Comparing `tmp/Spider_ToolsBox-0.0.5.tar.gz` & `tmp/Spider_ToolsBox-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Spider_ToolsBox-0.0.5.tar", last modified: Wed May  8 10:08:03 2024, max compression
+gzip compressed data, was "dist\Spider_ToolsBox-0.0.6.tar", last modified: Wed May  8 10:09:32 2024, max compression
```

## Comparing `Spider_ToolsBox-0.0.5.tar` & `Spider_ToolsBox-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 10:08:03.000000 Spider_ToolsBox-0.0.5/
--rw-rw-rw-   0        0        0     1094 2024-05-07 12:20:53.000000 Spider_ToolsBox-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      910 2024-05-08 10:08:03.000000 Spider_ToolsBox-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      425 2024-05-07 11:22:55.000000 Spider_ToolsBox-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 10:08:03.000000 Spider_ToolsBox-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      987 2024-05-08 10:07:55.000000 Spider_ToolsBox-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:08:03.000000 Spider_ToolsBox-0.0.5/spidertools/
--rw-rw-rw-   0        0        0    26786 2024-05-07 14:26:43.000000 Spider_ToolsBox-0.0.5/spidertools/spider_tools.py
--rw-rw-rw-   0        0        0      204 2024-05-07 14:26:43.000000 Spider_ToolsBox-0.0.5/spidertools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:08:03.000000 Spider_ToolsBox-0.0.5/Spider_ToolsBox.egg-info/
--rw-rw-rw-   0        0        0        1 2024-05-08 10:08:02.000000 Spider_ToolsBox-0.0.5/Spider_ToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      910 2024-05-08 10:08:02.000000 Spider_ToolsBox-0.0.5/Spider_ToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      107 2024-05-08 10:08:02.000000 Spider_ToolsBox-0.0.5/Spider_ToolsBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0      276 2024-05-08 10:08:02.000000 Spider_ToolsBox-0.0.5/Spider_ToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2024-05-08 10:08:02.000000 Spider_ToolsBox-0.0.5/Spider_ToolsBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 10:09:32.000000 Spider_ToolsBox-0.0.6/
+-rw-rw-rw-   0        0        0     1094 2024-05-07 12:20:53.000000 Spider_ToolsBox-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      910 2024-05-08 10:09:32.000000 Spider_ToolsBox-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2024-05-07 11:22:55.000000 Spider_ToolsBox-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 10:09:32.000000 Spider_ToolsBox-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      945 2024-05-08 10:09:28.000000 Spider_ToolsBox-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:09:32.000000 Spider_ToolsBox-0.0.6/spidertools/
+-rw-rw-rw-   0        0        0    26786 2024-05-07 14:26:43.000000 Spider_ToolsBox-0.0.6/spidertools/spider_tools.py
+-rw-rw-rw-   0        0        0      204 2024-05-07 14:26:43.000000 Spider_ToolsBox-0.0.6/spidertools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:09:32.000000 Spider_ToolsBox-0.0.6/Spider_ToolsBox.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-08 10:09:32.000000 Spider_ToolsBox-0.0.6/Spider_ToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      910 2024-05-08 10:09:32.000000 Spider_ToolsBox-0.0.6/Spider_ToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       65 2024-05-08 10:09:32.000000 Spider_ToolsBox-0.0.6/Spider_ToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      276 2024-05-08 10:09:32.000000 Spider_ToolsBox-0.0.6/Spider_ToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2024-05-08 10:09:32.000000 Spider_ToolsBox-0.0.6/Spider_ToolsBox.egg-info/top_level.txt
```

### Comparing `Spider_ToolsBox-0.0.5/LICENSE.txt` & `Spider_ToolsBox-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Spider_ToolsBox-0.0.5/PKG-INFO` & `Spider_ToolsBox-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Spider_ToolsBox
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package For Crawler
 Home-page: https://github.com/JOUUUSKA/SpiderToolBox.git
 Author: JOUUUSKA
 Author-email: 1393827820@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Spider_ToolsBox-0.0.5/setup.py` & `Spider_ToolsBox-0.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Spider_ToolsBox",
-    version="0.0.5",
+    version="0.0.6",
     author="JOUUUSKA",
     author_email="1393827820@qq.com",
     description="Package For Crawler",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JOUUUSKA/SpiderToolBox.git",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    install_requires=['requests', 'opencv-python @https://pypi.tuna.tsinghua.edu.cn/simple','ddddocr','execjs','fake_useragent','loguru','lxml']
+    install_requires=['requests', 'opencv-python','ddddocr','execjs','fake_useragent','loguru','lxml']
 )
```

### Comparing `Spider_ToolsBox-0.0.5/spidertools/spider_tools.py` & `Spider_ToolsBox-0.0.6/spidertools/spider_tools.py`

 * *Files identical despite different names*

### Comparing `Spider_ToolsBox-0.0.5/Spider_ToolsBox.egg-info/PKG-INFO` & `Spider_ToolsBox-0.0.6/Spider_ToolsBox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Spider-ToolsBox
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package For Crawler
 Home-page: https://github.com/JOUUUSKA/SpiderToolBox.git
 Author: JOUUUSKA
 Author-email: 1393827820@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

