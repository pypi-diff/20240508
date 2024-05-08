# Comparing `tmp/safeheron_api_sdk_python-1.0.7.tar.gz` & `tmp/safeheron_api_sdk_python-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safeheron_api_sdk_python-1.0.7.tar", last modified: Wed May  8 11:16:52 2024, max compression
+gzip compressed data, was "safeheron_api_sdk_python-1.0.8.tar", last modified: Wed May  8 11:27:38 2024, max compression
```

## Comparing `safeheron_api_sdk_python-1.0.7.tar` & `safeheron_api_sdk_python-1.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:16:52.928067 safeheron_api_sdk_python-1.0.7/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1071 2023-09-12 03:12:36.000000 safeheron_api_sdk_python-1.0.7/LICENSE
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      521 2024-05-08 11:16:52.927315 safeheron_api_sdk_python-1.0.7/PKG-INFO
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     4109 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/README.md
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       30 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/README.rst
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:16:52.915387 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:16:52.923842 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     9379 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/account_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     2672 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/coin_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3490 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/mpc_sign_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)    13785 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/transaction_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)    11075 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/web3_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1166 2024-05-08 10:39:36.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/client.py
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:16:52.924697 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/cosigner/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3078 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/cosigner/co_signer_converter.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     8494 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/tools.py
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:16:52.925444 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/webhook/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1851 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/webhook/webhook_converter.py
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:16:52.926466 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python.egg-info/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      521 2024-05-08 11:16:52.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      675 2024-05-08 11:16:52.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2024-05-08 11:16:52.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       41 2024-05-08 11:16:52.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python.egg-info/requires.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       25 2024-05-08 11:16:52.000000 safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       38 2024-05-08 11:16:52.928258 safeheron_api_sdk_python-1.0.7/setup.cfg
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      964 2024-05-08 11:16:47.000000 safeheron_api_sdk_python-1.0.7/setup.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:27:38.664469 safeheron_api_sdk_python-1.0.8/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1071 2023-09-12 03:12:36.000000 safeheron_api_sdk_python-1.0.8/LICENSE
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      486 2024-05-08 11:27:38.663577 safeheron_api_sdk_python-1.0.8/PKG-INFO
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     4109 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.8/README.md
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       30 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.8/README.rst
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:27:38.643994 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:27:38.656893 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/api/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     9379 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/api/account_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     2672 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/api/coin_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3490 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/api/mpc_sign_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)    13785 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/api/transaction_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)    11075 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/api/web3_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1166 2024-05-08 10:39:36.000000 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/client.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:27:38.658241 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/cosigner/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3078 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/cosigner/co_signer_converter.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     8494 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/tools.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:27:38.660615 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/webhook/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1851 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/webhook/webhook_converter.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 11:27:38.662196 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python.egg-info/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      486 2024-05-08 11:27:38.000000 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      675 2024-05-08 11:27:38.000000 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2024-05-08 11:27:38.000000 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       36 2024-05-08 11:27:38.000000 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       25 2024-05-08 11:27:38.000000 safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       38 2024-05-08 11:27:38.664699 safeheron_api_sdk_python-1.0.8/setup.cfg
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      929 2024-05-08 11:27:29.000000 safeheron_api_sdk_python-1.0.8/setup.py
```

### Comparing `safeheron_api_sdk_python-1.0.7/LICENSE` & `safeheron_api_sdk_python-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.7/README.md` & `safeheron_api_sdk_python-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/account_api.py` & `safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/api/account_api.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/coin_api.py` & `safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/api/coin_api.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/mpc_sign_api.py` & `safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/api/mpc_sign_api.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/transaction_api.py` & `safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/api/transaction_api.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/api/web3_api.py` & `safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/api/web3_api.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/client.py` & `safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/client.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/cosigner/co_signer_converter.py` & `safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/cosigner/co_signer_converter.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/tools.py` & `safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/tools.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python/webhook/webhook_converter.py` & `safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python/webhook/webhook_converter.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.7/safeheron_api_sdk_python.egg-info/SOURCES.txt` & `safeheron_api_sdk_python-1.0.8/safeheron_api_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.7/setup.py` & `safeheron_api_sdk_python-1.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from distutils.core import setup
 from setuptools import find_packages
 with open("README.rst", "r") as f:
     long_description = f.read()
 setup(name='safeheron_api_sdk_python',
-      version='1.0.7',
+      version='1.0.8',
       description='Python for Safeheron API',
       long_description=long_description,
       author='safeheron',
       author_email='support@safeheron.com',
       url='https://github.com/Safeheron/safeheron-api-sdk-python',
       install_requires=[
-            'Cryptodome',
-            'base64',
-            'json',
-            'time',
+            'pyCryptodomex',
+            'requests',
             'cryptography'
       ],
       license='MIT License',
       packages=[
             'safeheron_api_sdk_python',
             'safeheron_api_sdk_python.api',
             'safeheron_api_sdk_python.cosigner',
```

