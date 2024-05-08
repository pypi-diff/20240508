# Comparing `tmp/Spider_ToolsBox-0.0.2.tar.gz` & `tmp/Spider_ToolsBox-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Spider_ToolsBox-0.0.2.tar", last modified: Tue May  7 14:56:39 2024, max compression
+gzip compressed data, was "dist\Spider_ToolsBox-0.0.3.tar", last modified: Tue May  7 15:06:58 2024, max compression
```

## Comparing `Spider_ToolsBox-0.0.2.tar` & `Spider_ToolsBox-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/
--rw-rw-rw-   0        0        0     1094 2024-05-07 12:20:53.000000 Spider_ToolsBox-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      910 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      425 2024-05-07 11:22:55.000000 Spider_ToolsBox-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      876 2024-05-07 14:56:29.000000 Spider_ToolsBox-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/spidertools/
--rw-rw-rw-   0        0        0    26786 2024-05-07 14:26:43.000000 Spider_ToolsBox-0.0.2/spidertools/spider_tools.py
--rw-rw-rw-   0        0        0      204 2024-05-07 14:26:43.000000 Spider_ToolsBox-0.0.2/spidertools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/Spider_ToolsBox.egg-info/
--rw-rw-rw-   0        0        0        1 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/Spider_ToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      910 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/Spider_ToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        9 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/Spider_ToolsBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0      276 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/Spider_ToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2024-05-07 14:56:39.000000 Spider_ToolsBox-0.0.2/Spider_ToolsBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 15:06:58.000000 Spider_ToolsBox-0.0.3/
+-rw-rw-rw-   0        0        0     1094 2024-05-07 12:20:53.000000 Spider_ToolsBox-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      910 2024-05-07 15:06:58.000000 Spider_ToolsBox-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2024-05-07 11:22:55.000000 Spider_ToolsBox-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 15:06:58.000000 Spider_ToolsBox-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      944 2024-05-07 15:06:28.000000 Spider_ToolsBox-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:06:58.000000 Spider_ToolsBox-0.0.3/spidertools/
+-rw-rw-rw-   0        0        0    26786 2024-05-07 14:26:43.000000 Spider_ToolsBox-0.0.3/spidertools/spider_tools.py
+-rw-rw-rw-   0        0        0      204 2024-05-07 14:26:43.000000 Spider_ToolsBox-0.0.3/spidertools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:06:58.000000 Spider_ToolsBox-0.0.3/Spider_ToolsBox.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-07 15:06:57.000000 Spider_ToolsBox-0.0.3/Spider_ToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      910 2024-05-07 15:06:57.000000 Spider_ToolsBox-0.0.3/Spider_ToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       65 2024-05-07 15:06:57.000000 Spider_ToolsBox-0.0.3/Spider_ToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      276 2024-05-07 15:06:57.000000 Spider_ToolsBox-0.0.3/Spider_ToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2024-05-07 15:06:57.000000 Spider_ToolsBox-0.0.3/Spider_ToolsBox.egg-info/top_level.txt
```

### Comparing `Spider_ToolsBox-0.0.2/LICENSE.txt` & `Spider_ToolsBox-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Spider_ToolsBox-0.0.2/PKG-INFO` & `Spider_ToolsBox-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Spider_ToolsBox
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package For Crawler
 Home-page: https://github.com/JOUUUSKA/SpiderToolBox.git
 Author: JOUUUSKA
 Author-email: 1393827820@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Spider_ToolsBox-0.0.2/setup.py` & `Spider_ToolsBox-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Spider_ToolsBox",
-    version="0.0.2",
+    version="0.0.3",
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
-    install_requires=['requests']
+    install_requires=['requests','opencv-python','ddddocr','execjs','fake_useragent','loguru','lxml']
 )
```

### Comparing `Spider_ToolsBox-0.0.2/spidertools/spider_tools.py` & `Spider_ToolsBox-0.0.3/spidertools/spider_tools.py`

 * *Files identical despite different names*

### Comparing `Spider_ToolsBox-0.0.2/Spider_ToolsBox.egg-info/PKG-INFO` & `Spider_ToolsBox-0.0.3/Spider_ToolsBox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Spider-ToolsBox
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package For Crawler
 Home-page: https://github.com/JOUUUSKA/SpiderToolBox.git
 Author: JOUUUSKA
 Author-email: 1393827820@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

