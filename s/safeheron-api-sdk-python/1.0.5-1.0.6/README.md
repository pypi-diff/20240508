# Comparing `tmp/safeheron_api_sdk_python-1.0.5.tar.gz` & `tmp/safeheron_api_sdk_python-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safeheron_api_sdk_python-1.0.5.tar", last modified: Wed May  8 10:41:50 2024, max compression
+gzip compressed data, was "safeheron_api_sdk_python-1.0.6.tar", last modified: Wed May  8 10:57:51 2024, max compression
```

## Comparing `safeheron_api_sdk_python-1.0.5.tar` & `safeheron_api_sdk_python-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,25 @@
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:41:50.615317 safeheron_api_sdk_python-1.0.5/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1071 2023-09-12 03:12:36.000000 safeheron_api_sdk_python-1.0.5/LICENSE
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      405 2024-05-08 10:41:50.614349 safeheron_api_sdk_python-1.0.5/PKG-INFO
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     4109 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.5/README.md
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       30 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.5/README.rst
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:41:50.608642 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1166 2024-05-08 10:39:36.000000 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python/client.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     8494 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python/tools.py
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:41:50.612756 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python.egg-info/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      405 2024-05-08 10:41:50.000000 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      298 2024-05-08 10:41:50.000000 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2024-05-08 10:41:50.000000 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2024-05-08 10:41:50.000000 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       38 2024-05-08 10:41:50.615513 safeheron_api_sdk_python-1.0.5/setup.cfg
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      734 2024-05-08 10:41:16.000000 safeheron_api_sdk_python-1.0.5/setup.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:57:51.249186 safeheron_api_sdk_python-1.0.6/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1071 2023-09-12 03:12:36.000000 safeheron_api_sdk_python-1.0.6/LICENSE
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      405 2024-05-08 10:57:51.248503 safeheron_api_sdk_python-1.0.6/PKG-INFO
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     4109 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/README.md
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       30 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/README.rst
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:57:51.213698 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:57:51.244591 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     9379 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/account_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     2672 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/coin_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3490 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/mpc_sign_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)    13785 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/transaction_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)    11075 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/web3_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1166 2024-05-08 10:39:36.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/client.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:57:51.245526 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/cosigner/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3078 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/cosigner/co_signer_converter.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     8494 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/tools.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:57:51.246400 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/webhook/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1851 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/webhook/webhook_converter.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:57:51.247659 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python.egg-info/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      405 2024-05-08 10:57:51.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      628 2024-05-08 10:57:51.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2024-05-08 10:57:51.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       25 2024-05-08 10:57:51.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       38 2024-05-08 10:57:51.249326 safeheron_api_sdk_python-1.0.6/setup.cfg
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      783 2024-05-08 10:57:31.000000 safeheron_api_sdk_python-1.0.6/setup.py
```

### Comparing `safeheron_api_sdk_python-1.0.5/LICENSE` & `safeheron_api_sdk_python-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.5/README.md` & `safeheron_api_sdk_python-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python/client.py` & `safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/client.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python/tools.py` & `safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/tools.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.5/setup.py` & `safeheron_api_sdk_python-1.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from distutils.core import setup
 from setuptools import find_packages
 with open("README.rst", "r") as f:
     long_description = f.read()
 setup(name='safeheron_api_sdk_python',
-      version='1.0.5',
+      version='1.0.6',
       description='Python for Safeheron API',
       long_description=long_description,
       author='safeheron',
       author_email='support@safeheron.com',
       url='https://github.com/Safeheron/safeheron-api-sdk-python',
       install_requires=[],
       license='MIT License',
-      packages=find_packages(include=['safeheron_api_sdk_python', 'safeheron_api_sdk_python.*']),
+      packages=['safeheron_api_sdk_python','safeheron_api_sdk_python.api','safeheron_api_sdk_python.cosigner','safeheron_api_sdk_python.webhook'],
       platforms=["all"],
       classifiers=[
           'Operating System :: OS Independent',
           'Programming Language :: Python :: 3'
       ],
       )
```

