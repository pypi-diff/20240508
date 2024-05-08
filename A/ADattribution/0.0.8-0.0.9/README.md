# Comparing `tmp/ADattribution-0.0.8.tar.gz` & `tmp/ADattribution-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ADattribution-0.0.8.tar", last modified: Thu Jan 18 07:57:47 2024, max compression
+gzip compressed data, was "ADattribution-0.0.9.tar", last modified: Wed May  8 03:11:35 2024, max compression
```

## Comparing `ADattribution-0.0.8.tar` & `ADattribution-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-01-18 07:57:47.297045 ADattribution-0.0.8/
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-01-18 07:57:47.296087 ADattribution-0.0.8/ADattribution/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     5897 2023-09-09 02:46:51.000000 ADattribution-0.0.8/ADattribution/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1107 2023-02-28 08:40:57.000000 ADattribution-0.0.8/ADattribution/adq_postback.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2210 2024-01-18 07:57:07.000000 ADattribution-0.0.8/ADattribution/baidu_postback.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     4514 2023-07-18 08:25:38.000000 ADattribution-0.0.8/ADattribution/oceanengine_postback.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-01-18 07:57:47.296759 ADattribution-0.0.8/ADattribution.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      756 2024-01-18 07:57:47.000000 ADattribution-0.0.8/ADattribution.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      336 2024-01-18 07:57:47.000000 ADattribution-0.0.8/ADattribution.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-01-18 07:57:47.000000 ADattribution-0.0.8/ADattribution.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       34 2024-01-18 07:57:47.000000 ADattribution-0.0.8/ADattribution.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       14 2024-01-18 07:57:47.000000 ADattribution-0.0.8/ADattribution.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1067 2023-04-06 06:34:13.000000 ADattribution-0.0.8/LICENSE
--rw-r--r--   0 zeroseeker   (501) staff       (20)      756 2024-01-18 07:57:47.296943 ADattribution-0.0.8/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      390 2023-04-06 06:35:18.000000 ADattribution-0.0.8/README.md
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-01-18 07:57:47.297089 ADattribution-0.0.8/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      914 2024-01-18 07:57:07.000000 ADattribution-0.0.8/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-05-08 03:11:35.931637 ADattribution-0.0.9/
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-05-08 03:11:35.930446 ADattribution-0.0.9/ADattribution/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     5897 2023-09-09 02:46:51.000000 ADattribution-0.0.9/ADattribution/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1107 2023-02-28 08:40:57.000000 ADattribution-0.0.9/ADattribution/adq_postback.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3492 2024-05-08 03:10:59.000000 ADattribution-0.0.9/ADattribution/baidu_postback.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     4514 2023-07-18 08:25:38.000000 ADattribution-0.0.9/ADattribution/oceanengine_postback.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-05-08 03:11:35.931306 ADattribution-0.0.9/ADattribution.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      756 2024-05-08 03:11:35.000000 ADattribution-0.0.9/ADattribution.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      336 2024-05-08 03:11:35.000000 ADattribution-0.0.9/ADattribution.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-05-08 03:11:35.000000 ADattribution-0.0.9/ADattribution.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       34 2024-05-08 03:11:35.000000 ADattribution-0.0.9/ADattribution.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       14 2024-05-08 03:11:35.000000 ADattribution-0.0.9/ADattribution.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1067 2023-04-06 06:34:13.000000 ADattribution-0.0.9/LICENSE
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      756 2024-05-08 03:11:35.931505 ADattribution-0.0.9/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      390 2023-04-06 06:35:18.000000 ADattribution-0.0.9/README.md
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-05-08 03:11:35.931690 ADattribution-0.0.9/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      914 2024-05-08 03:10:59.000000 ADattribution-0.0.9/setup.py
```

### Comparing `ADattribution-0.0.8/ADattribution/__init__.py` & `ADattribution-0.0.9/ADattribution/__init__.py`

 * *Files identical despite different names*

### Comparing `ADattribution-0.0.8/ADattribution/adq_postback.py` & `ADattribution-0.0.9/ADattribution/adq_postback.py`

 * *Files identical despite different names*

### Comparing `ADattribution-0.0.8/ADattribution/oceanengine_postback.py` & `ADattribution-0.0.9/ADattribution/oceanengine_postback.py`

 * *Files identical despite different names*

### Comparing `ADattribution-0.0.8/ADattribution.egg-info/PKG-INFO` & `ADattribution-0.0.9/ADattribution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ADattribution
-Version: 0.0.8
+Version: 0.0.9
 Summary: make it easy to use AD postback
 Home-page: https://gitee.com/ZeroSeeker/ADattribution
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ADattribution-0.0.8/LICENSE` & `ADattribution-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ADattribution-0.0.8/PKG-INFO` & `ADattribution-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ADattribution
-Version: 0.0.8
+Version: 0.0.9
 Summary: make it easy to use AD postback
 Home-page: https://gitee.com/ZeroSeeker/ADattribution
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ADattribution-0.0.8/setup.py` & `ADattribution-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ADattribution",
-    version="0.0.8",
+    version="0.0.9",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     description="make it easy to use AD postback",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ZeroSeeker/ADattribution",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         # "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'ua-parser==0.10.0',
-        'lazysdk>=0.1.82'
+        'lazysdk>=0.1.91'
     ]
 )
```

