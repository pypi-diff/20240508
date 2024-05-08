# Comparing `tmp/safeheron_api_sdk_python-1.0.3.tar.gz` & `tmp/safeheron_api_sdk_python-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safeheron_api_sdk_python-1.0.3.tar", last modified: Thu Nov 23 08:29:56 2023, max compression
+gzip compressed data, was "safeheron_api_sdk_python-1.0.4.tar", last modified: Wed May  8 10:19:05 2024, max compression
```

## Comparing `safeheron_api_sdk_python-1.0.3.tar` & `safeheron_api_sdk_python-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2023-11-23 08:29:56.296542 safeheron_api_sdk_python-1.0.3/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1071 2023-09-12 03:12:36.000000 safeheron_api_sdk_python-1.0.3/LICENSE
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      405 2023-11-23 08:29:56.295561 safeheron_api_sdk_python-1.0.3/PKG-INFO
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     4109 2023-11-23 08:10:47.000000 safeheron_api_sdk_python-1.0.3/README.md
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       30 2023-09-14 07:14:46.000000 safeheron_api_sdk_python-1.0.3/README.rst
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2023-11-23 08:29:56.293878 safeheron_api_sdk_python-1.0.3/safeheron_api_sdk_python.egg-info/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      405 2023-11-23 08:29:56.000000 safeheron_api_sdk_python-1.0.3/safeheron_api_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      229 2023-11-23 08:29:56.000000 safeheron_api_sdk_python-1.0.3/safeheron_api_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2023-11-23 08:29:56.000000 safeheron_api_sdk_python-1.0.3/safeheron_api_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2023-11-23 08:29:56.000000 safeheron_api_sdk_python-1.0.3/safeheron_api_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       38 2023-11-23 08:29:56.296817 safeheron_api_sdk_python-1.0.3/setup.cfg
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      668 2023-11-23 07:56:20.000000 safeheron_api_sdk_python-1.0.3/setup.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:19:05.479512 safeheron_api_sdk_python-1.0.4/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1071 2023-09-12 03:12:36.000000 safeheron_api_sdk_python-1.0.4/LICENSE
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      405 2024-05-08 10:19:05.478812 safeheron_api_sdk_python-1.0.4/PKG-INFO
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     4109 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.4/README.md
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       30 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.4/README.rst
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:19:05.457304 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1166 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python/client.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     8494 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python/tools.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:19:05.477659 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python.egg-info/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      405 2024-05-08 10:19:05.000000 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      298 2024-05-08 10:19:05.000000 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2024-05-08 10:19:05.000000 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       25 2024-05-08 10:19:05.000000 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       38 2024-05-08 10:19:05.479659 safeheron_api_sdk_python-1.0.4/setup.cfg
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      681 2024-05-08 10:16:18.000000 safeheron_api_sdk_python-1.0.4/setup.py
```

### Comparing `safeheron_api_sdk_python-1.0.3/LICENSE` & `safeheron_api_sdk_python-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.3/README.md` & `safeheron_api_sdk_python-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.3/setup.py` & `safeheron_api_sdk_python-1.0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from distutils.core import setup
 from setuptools import find_packages
 with open("README.rst", "r") as f:
     long_description = f.read()
 setup(name='safeheron_api_sdk_python',
-      version='1.0.3',
+      version='1.0.4',
       description='Python for Safeheron API',
       long_description=long_description,
       author='safeheron',
       author_email='support@safeheron.com',
       url='https://github.com/Safeheron/safeheron-api-sdk-python',
       install_requires=[],
       license='MIT License',
-      packages=find_packages(),
+      packages=['safeheron_api_sdk_python'],
       platforms=["all"],
       classifiers=[
           'Operating System :: OS Independent',
           'Programming Language :: Python :: 3'
       ],
       )
```

