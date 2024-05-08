# Comparing `tmp/safeheron_api_sdk_python-1.0.6.tar.gz` & `tmp/safeheron_api_sdk_python-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safeheron_api_sdk_python-1.0.6.tar", last modified: Wed May  8 10:57:51 2024, max compression
+gzip compressed data, was "safeheron_api_sdk_python-1.0.7.tar", last modified: Wed May  8 11:16:52 2024, max compression
```

## Comparing `safeheron_api_sdk_python-1.0.6.tar` & `safeheron_api_sdk_python-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:57:51.249186 safeheron_api_sdk_python-1.0.6/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1071 2023-09-12 03:12:36.000000 safeheron_api_sdk_python-1.0.6/LICENSE
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      405 2024-05-08 10:57:51.248503 safeheron_api_sdk_python-1.0.6/PKG-INFO
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     4109 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/README.md
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       30 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/README.rst
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:57:51.213698 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:57:51.244591 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     9379 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/account_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     2672 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/coin_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3490 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/mpc_sign_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)    13785 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/transaction_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)    11075 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/web3_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1166 2024-05-08 10:39:36.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/client.py
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:57:51.245526 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/cosigner/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3078 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/cosigner/co_signer_converter.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     8494 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/tools.py
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:57:51.246400 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/webhook/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1851 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/webhook/webhook_converter.py
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:57:51.247659 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python.egg-info/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      405 2024-05-08 10:57:51.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      628 2024-05-08 10:57:51.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2024-05-08 10:57:51.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       25 2024-05-08 10:57:51.000000 safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       38 2024-05-08 10:57:51.249326 safeheron_api_sdk_python-1.0.6/setup.cfg
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      783 2024-05-08 10:57:31.000000 safeheron_api_sdk_python-1.0.6/setup.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:16:52.928067 safeheron_api_sdk_python-1.0.7/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1071 2023-09-12 03:12:36.000000 safeheron_api_sdk_python-1.0.7/LICENSE
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      521 2024-05-08 11:16:52.927315 safeheron_api_sdk_python-1.0.7/PKG-INFO
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     4109 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/README.md
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       30 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/README.rst
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:16:52.915387 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:16:52.923842 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     9379 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/account_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     2672 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/coin_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3490 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/mpc_sign_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)    13785 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/transaction_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)    11075 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/web3_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1166 2024-05-08 10:39:36.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/client.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:16:52.924697 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/cosigner/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3078 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/cosigner/co_signer_converter.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     8494 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/tools.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:16:52.925444 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/webhook/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1851 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/webhook/webhook_converter.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:16:52.926466 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python.egg-info/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      521 2024-05-08 11:16:52.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      675 2024-05-08 11:16:52.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2024-05-08 11:16:52.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       41 2024-05-08 11:16:52.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       25 2024-05-08 11:16:52.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       38 2024-05-08 11:16:52.928258 safeheron_api_sdk_python-1.0.7/setup.cfg
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      964 2024-05-08 11:16:47.000000 safeheron_api_sdk_python-1.0.7/setup.py
```

### Comparing `safeheron_api_sdk_python-1.0.6/LICENSE` & `safeheron_api_sdk_python-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.6/README.md` & `safeheron_api_sdk_python-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/account_api.py` & `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/account_api.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/coin_api.py` & `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/coin_api.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/mpc_sign_api.py` & `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/mpc_sign_api.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/transaction_api.py` & `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/transaction_api.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/api/web3_api.py` & `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/web3_api.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/client.py` & `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/client.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/cosigner/co_signer_converter.py` & `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/cosigner/co_signer_converter.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/tools.py` & `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/tools.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python/webhook/webhook_converter.py` & `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/webhook/webhook_converter.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.6/safeheron_api_sdk_python.egg-info/SOURCES.txt` & `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.rst
 setup.py
 safeheron_api_sdk_python/client.py
 safeheron_api_sdk_python/tools.py
 safeheron_api_sdk_python.egg-info/PKG-INFO
 safeheron_api_sdk_python.egg-info/SOURCES.txt
 safeheron_api_sdk_python.egg-info/dependency_links.txt
+safeheron_api_sdk_python.egg-info/requires.txt
 safeheron_api_sdk_python.egg-info/top_level.txt
 safeheron_api_sdk_python/api/account_api.py
 safeheron_api_sdk_python/api/coin_api.py
 safeheron_api_sdk_python/api/mpc_sign_api.py
 safeheron_api_sdk_python/api/transaction_api.py
 safeheron_api_sdk_python/api/web3_api.py
 safeheron_api_sdk_python/cosigner/co_signer_converter.py
```

### Comparing `safeheron_api_sdk_python-1.0.6/setup.py` & `safeheron_api_sdk_python-1.0.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 from distutils.core import setup
 from setuptools import find_packages
 with open("README.rst", "r") as f:
     long_description = f.read()
 setup(name='safeheron_api_sdk_python',
-      version='1.0.6',
+      version='1.0.7',
       description='Python for Safeheron API',
       long_description=long_description,
       author='safeheron',
       author_email='support@safeheron.com',
       url='https://github.com/Safeheron/safeheron-api-sdk-python',
-      install_requires=[],
+      install_requires=[
+            'Cryptodome',
+            'base64',
+            'json',
+            'time',
+            'cryptography'
+      ],
       license='MIT License',
-      packages=['safeheron_api_sdk_python','safeheron_api_sdk_python.api','safeheron_api_sdk_python.cosigner','safeheron_api_sdk_python.webhook'],
+      packages=[
+            'safeheron_api_sdk_python',
+            'safeheron_api_sdk_python.api',
+            'safeheron_api_sdk_python.cosigner',
+            'safeheron_api_sdk_python.webhook'
+      ],
       platforms=["all"],
       classifiers=[
           'Operating System :: OS Independent',
           'Programming Language :: Python :: 3'
       ],
       )
```
