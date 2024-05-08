# Comparing `tmp/mypy-boto3-ecr-1.33.0.tar.gz` & `tmp/mypy-boto3-ecr-1.34.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecr-1.33.0.tar", last modified: Tue Nov 28 18:29:13 2023, max compression
+gzip compressed data, was "mypy-boto3-ecr-1.34.0.tar", last modified: Wed Dec 13 21:22:32 2023, max compression
```

## Comparing `mypy-boto3-ecr-1.33.0.tar` & `mypy-boto3-ecr-1.34.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:29:13.003260 mypy-boto3-ecr-1.33.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14002 2023-11-28 18:29:12.999261 mypy-boto3-ecr-1.33.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12485 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:29:12.999261 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35340 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    35336 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11788 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11786 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    43236 2023-11-28 18:15:50.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    43235 2023-11-28 18:15:49.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:29:12.999261 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14002 2023-11-28 18:29:12.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2023-11-28 18:29:12.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 18:29:12.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 18:29:12.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-28 18:29:12.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-28 18:29:12.000000 mypy-boto3-ecr-1.33.0/mypy_boto3_ecr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 18:29:13.003260 mypy-boto3-ecr-1.33.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-11-28 18:15:47.000000 mypy-boto3-ecr-1.33.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:32.491199 mypy-boto3-ecr-1.34.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14002 2023-12-13 21:22:32.491199 mypy-boto3-ecr-1.34.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12485 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:32.491199 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35340 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35336 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11950 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11948 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    43236 2023-12-13 21:09:41.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43235 2023-12-13 21:09:40.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:32.491199 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14002 2023-12-13 21:22:32.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2023-12-13 21:22:32.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:32.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:32.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:32.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-13 21:22:32.000000 mypy-boto3-ecr-1.34.0/mypy_boto3_ecr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:32.491199 mypy-boto3-ecr-1.34.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-12-13 21:09:39.000000 mypy-boto3-ecr-1.34.0/setup.py
```

### Comparing `mypy-boto3-ecr-1.33.0/LICENSE` & `mypy-boto3-ecr-1.34.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.33.0/PKG-INFO` & `mypy-boto3-ecr-1.34.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr
-Version: 1.33.0
-Summary: Type annotations for boto3.ECR 1.33.0 service generated with mypy-boto3-builder 7.20.3
+Version: 1.34.0
+Summary: Type annotations for boto3.ECR 1.34.0 service generated with mypy-boto3-builder 7.21.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr)](https://pepy.tech/project/mypy-boto3-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECR 1.33.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[boto3.ECR 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.20.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ecr-1.33.0/README.md` & `mypy-boto3-ecr-1.34.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr)](https://pepy.tech/project/mypy-boto3-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECR 1.33.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[boto3.ECR 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.20.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/__init__.py` & `mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/__init__.pyi` & `mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/__main__.py` & `mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECR 1.33.0\nVersion:         1.33.0\nBuilder version:"
-        " 7.20.3\nDocs:           "
+        "Type annotations for boto3.ECR 1.34.0\nVersion:         1.34.0\nBuilder version:"
+        " 7.21.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.33.0")
+    print("1.34.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/client.py` & `mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/client.pyi` & `mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/literals.py` & `mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,26 +141,29 @@
     "b2bi",
     "backup",
     "backup-gateway",
     "backupstorage",
     "batch",
     "bcm-data-exports",
     "bedrock",
+    "bedrock-agent",
+    "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
+    "cleanroomsml",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudfront-keyvaluestore",
     "cloudhsm",
@@ -320,15 +323,17 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
     "managedblockchain",
     "managedblockchain-query",
+    "marketplace-agreement",
     "marketplace-catalog",
+    "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
@@ -376,14 +381,16 @@
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
     "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
+    "qbusiness",
+    "qconnect",
     "qldb",
     "qldb-session",
     "quicksight",
     "ram",
     "rbin",
     "rds",
     "rds-data",
```

### Comparing `mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/literals.pyi` & `mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -139,26 +139,29 @@
     "b2bi",
     "backup",
     "backup-gateway",
     "backupstorage",
     "batch",
     "bcm-data-exports",
     "bedrock",
+    "bedrock-agent",
+    "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
+    "cleanroomsml",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudfront-keyvaluestore",
     "cloudhsm",
@@ -318,15 +321,17 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
     "managedblockchain",
     "managedblockchain-query",
+    "marketplace-agreement",
     "marketplace-catalog",
+    "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
@@ -374,14 +379,16 @@
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
     "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
+    "qbusiness",
+    "qconnect",
     "qldb",
     "qldb-session",
     "quicksight",
     "ram",
     "rbin",
     "rds",
     "rds-data",
```

### Comparing `mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/paginator.py` & `mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/paginator.pyi` & `mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/type_defs.py` & `mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/type_defs.pyi` & `mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/waiter.py` & `mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.33.0/mypy_boto3_ecr/waiter.pyi` & `mypy-boto3-ecr-1.34.0/mypy_boto3_ecr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.33.0/mypy_boto3_ecr.egg-info/PKG-INFO` & `mypy-boto3-ecr-1.34.0/mypy_boto3_ecr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr
-Version: 1.33.0
-Summary: Type annotations for boto3.ECR 1.33.0 service generated with mypy-boto3-builder 7.20.3
+Version: 1.34.0
+Summary: Type annotations for boto3.ECR 1.34.0 service generated with mypy-boto3-builder 7.21.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr)](https://pepy.tech/project/mypy-boto3-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECR 1.33.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[boto3.ECR 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.20.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ecr-1.33.0/mypy_boto3_ecr.egg-info/SOURCES.txt` & `mypy-boto3-ecr-1.34.0/mypy_boto3_ecr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.33.0/setup.py` & `mypy-boto3-ecr-1.34.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecr",
-    version="1.33.0",
+    version="1.34.0",
     packages=["mypy_boto3_ecr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECR 1.33.0 service generated with mypy-boto3-builder 7.20.3"
+        "Type annotations for boto3.ECR 1.34.0 service generated with mypy-boto3-builder 7.21.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

