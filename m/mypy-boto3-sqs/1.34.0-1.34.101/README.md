# Comparing `tmp/mypy-boto3-sqs-1.34.0.tar.gz` & `tmp/mypy_boto3_sqs-1.34.101.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sqs-1.34.0.tar", last modified: Wed Dec 13 21:23:55 2023, max compression
+gzip compressed data, was "mypy_boto3_sqs-1.34.101.tar", last modified: Wed May  8 19:33:03 2024, max compression
```

## Comparing `mypy-boto3-sqs-1.34.0.tar` & `mypy_boto3_sqs-1.34.101.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:55.507389 mypy-boto3-sqs-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14982 2023-12-13 21:23:55.507389 mypy-boto3-sqs-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13465 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:55.507389 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18113 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18109 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10940 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10938 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19072 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    19063 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20291 2023-12-13 21:20:10.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20290 2023-12-13 21:20:07.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:55.507389 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14982 2023-12-13 21:23:55.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      675 2023-12-13 21:23:55.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:55.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:55.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:55.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-13 21:23:55.000000 mypy-boto3-sqs-1.34.0/mypy_boto3_sqs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:55.507389 mypy-boto3-sqs-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-12-13 21:20:06.000000 mypy-boto3-sqs-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:33:03.620214 mypy_boto3_sqs-1.34.101/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-08 19:32:49.000000 mypy_boto3_sqs-1.34.101/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15008 2024-05-08 19:33:03.620214 mypy_boto3_sqs-1.34.101/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-05-08 19:32:49.000000 mypy_boto3_sqs-1.34.101/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:33:03.620214 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-08 19:32:49.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-08 19:32:49.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-08 19:32:49.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18790 2024-05-08 19:32:50.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18787 2024-05-08 19:32:50.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-08 19:32:50.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-08 19:32:50.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-08 19:32:50.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-08 19:32:50.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:32:49.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19244 2024-05-08 19:32:50.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19236 2024-05-08 19:32:50.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20475 2024-05-08 19:32:50.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20475 2024-05-08 19:32:50.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 19:32:49.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:33:03.620214 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15008 2024-05-08 19:33:03.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-08 19:33:03.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:33:03.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:33:03.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 19:33:03.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 19:33:03.000000 mypy_boto3_sqs-1.34.101/mypy_boto3_sqs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:33:03.624215 mypy_boto3_sqs-1.34.101/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-08 19:32:49.000000 mypy_boto3_sqs-1.34.101/setup.py
```

### Comparing `mypy-boto3-sqs-1.34.0/LICENSE` & `mypy_boto3_sqs-1.34.101/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-sqs-1.34.0/PKG-INFO` & `mypy_boto3_sqs-1.34.101/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sqs
-Version: 1.34.0
-Summary: Type annotations for boto3.SQS 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.101
+Summary: Type annotations for boto3.SQS 1.34.101 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-sqs"></a>
 
 # mypy-boto3-sqs
 
 [![PyPI - mypy-boto3-sqs](https://img.shields.io/pypi/v/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sqs)](https://pepy.tech/project/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.34.101](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sqs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sqs-1.34.0/README.md` & `mypy_boto3_sqs-1.34.101/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sqs)](https://pepy.tech/project/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.34.101](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sqs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/__init__.py` & `mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,18 +26,16 @@
 
 from .client import SQSClient
 from .paginator import ListDeadLetterSourceQueuesPaginator, ListQueuesPaginator
 from .service_resource import SQSServiceResource
 
 Client = SQSClient
 
-
 ServiceResource = SQSServiceResource
 
-
 __all__ = (
     "Client",
     "ListDeadLetterSourceQueuesPaginator",
     "ListQueuesPaginator",
     "SQSClient",
     "SQSServiceResource",
     "ServiceResource",
```

### Comparing `mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/__init__.pyi` & `mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/__main__.py` & `mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SQS 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.SQS 1.34.101\n"
+        "Version:         1.34.101\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.101")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/client.py` & `mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import QueueAttributeFilterType, QueueAttributeNameType
+from .literals import (
+    MessageSystemAttributeNameType,
+    QueueAttributeFilterType,
+    QueueAttributeNameType,
+)
 from .paginator import ListDeadLetterSourceQueuesPaginator, ListQueuesPaginator
 from .type_defs import (
     CancelMessageMoveTaskResultTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
     CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
@@ -31,29 +35,28 @@
     EmptyResponseMetadataTypeDef,
     GetQueueAttributesResultTypeDef,
     GetQueueUrlResultTypeDef,
     ListDeadLetterSourceQueuesResultTypeDef,
     ListMessageMoveTasksResultTypeDef,
     ListQueuesResultTypeDef,
     ListQueueTagsResultTypeDef,
-    MessageAttributeValueTypeDef,
+    MessageAttributeValueUnionTypeDef,
     MessageSystemAttributeValueTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
     StartMessageMoveTaskResultTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SQSClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -62,25 +65,36 @@
 
 
 class Exceptions:
     BatchEntryIdsNotDistinct: Type[BotocoreClientError]
     BatchRequestTooLong: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     EmptyBatchRequest: Type[BotocoreClientError]
+    InvalidAddress: Type[BotocoreClientError]
     InvalidAttributeName: Type[BotocoreClientError]
+    InvalidAttributeValue: Type[BotocoreClientError]
     InvalidBatchEntryId: Type[BotocoreClientError]
     InvalidIdFormat: Type[BotocoreClientError]
     InvalidMessageContents: Type[BotocoreClientError]
+    InvalidSecurity: Type[BotocoreClientError]
+    KmsAccessDenied: Type[BotocoreClientError]
+    KmsDisabled: Type[BotocoreClientError]
+    KmsInvalidKeyUsage: Type[BotocoreClientError]
+    KmsInvalidState: Type[BotocoreClientError]
+    KmsNotFound: Type[BotocoreClientError]
+    KmsOptInRequired: Type[BotocoreClientError]
+    KmsThrottled: Type[BotocoreClientError]
     MessageNotInflight: Type[BotocoreClientError]
     OverLimit: Type[BotocoreClientError]
     PurgeQueueInProgress: Type[BotocoreClientError]
     QueueDeletedRecently: Type[BotocoreClientError]
     QueueDoesNotExist: Type[BotocoreClientError]
     QueueNameExists: Type[BotocoreClientError]
     ReceiptHandleIsInvalid: Type[BotocoreClientError]
+    RequestThrottled: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     TooManyEntriesInBatchRequest: Type[BotocoreClientError]
     UnsupportedOperation: Type[BotocoreClientError]
 
 
 class SQSClient(BaseClient):
     """
@@ -155,15 +169,15 @@
         """
 
     def create_queue(
         self,
         *,
         QueueName: str,
         Attributes: Mapping[QueueAttributeNameType, str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateQueueResultTypeDef:
         """
         Creates a new standard or FIFO queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.create_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#create_queue)
         """
@@ -281,19 +295,20 @@
         """
 
     def receive_message(
         self,
         *,
         QueueUrl: str,
         AttributeNames: Sequence[QueueAttributeFilterType] = ...,
+        MessageSystemAttributeNames: Sequence[MessageSystemAttributeNameType] = ...,
         MessageAttributeNames: Sequence[str] = ...,
         MaxNumberOfMessages: int = ...,
         VisibilityTimeout: int = ...,
         WaitTimeSeconds: int = ...,
-        ReceiveRequestAttemptId: str = ...
+        ReceiveRequestAttemptId: str = ...,
     ) -> ReceiveMessageResultTypeDef:
         """
         Retrieves one or more messages (up to 10), from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.receive_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#receive_message)
         """
@@ -309,20 +324,20 @@
 
     def send_message(
         self,
         *,
         QueueUrl: str,
         MessageBody: str,
         DelaySeconds: int = ...,
-        MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueUnionTypeDef] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
-        MessageGroupId: str = ...
+        MessageGroupId: str = ...,
     ) -> SendMessageResultTypeDef:
         """
         Delivers a message to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message)
         """
@@ -340,15 +355,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message_batch)
         """
 
     def set_queue_attributes(
         self, *, QueueUrl: str, Attributes: Mapping[QueueAttributeNameType, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Sets the value of one or more queue attributes.
+        Sets the value of one or more queue attributes, like a policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.set_queue_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#set_queue_attributes)
         """
 
     def start_message_move_task(
         self, *, SourceArn: str, DestinationArn: str = ..., MaxNumberOfMessagesPerSecond: int = ...
```

### Comparing `mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/client.pyi` & `mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import QueueAttributeFilterType, QueueAttributeNameType
+from .literals import (
+    MessageSystemAttributeNameType,
+    QueueAttributeFilterType,
+    QueueAttributeNameType,
+)
 from .paginator import ListDeadLetterSourceQueuesPaginator, ListQueuesPaginator
 from .type_defs import (
     CancelMessageMoveTaskResultTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
     CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
@@ -31,15 +35,15 @@
     EmptyResponseMetadataTypeDef,
     GetQueueAttributesResultTypeDef,
     GetQueueUrlResultTypeDef,
     ListDeadLetterSourceQueuesResultTypeDef,
     ListMessageMoveTasksResultTypeDef,
     ListQueuesResultTypeDef,
     ListQueueTagsResultTypeDef,
-    MessageAttributeValueTypeDef,
+    MessageAttributeValueUnionTypeDef,
     MessageSystemAttributeValueTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
     StartMessageMoveTaskResultTypeDef,
 )
@@ -59,25 +63,36 @@
         self.operation_name: str
 
 class Exceptions:
     BatchEntryIdsNotDistinct: Type[BotocoreClientError]
     BatchRequestTooLong: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     EmptyBatchRequest: Type[BotocoreClientError]
+    InvalidAddress: Type[BotocoreClientError]
     InvalidAttributeName: Type[BotocoreClientError]
+    InvalidAttributeValue: Type[BotocoreClientError]
     InvalidBatchEntryId: Type[BotocoreClientError]
     InvalidIdFormat: Type[BotocoreClientError]
     InvalidMessageContents: Type[BotocoreClientError]
+    InvalidSecurity: Type[BotocoreClientError]
+    KmsAccessDenied: Type[BotocoreClientError]
+    KmsDisabled: Type[BotocoreClientError]
+    KmsInvalidKeyUsage: Type[BotocoreClientError]
+    KmsInvalidState: Type[BotocoreClientError]
+    KmsNotFound: Type[BotocoreClientError]
+    KmsOptInRequired: Type[BotocoreClientError]
+    KmsThrottled: Type[BotocoreClientError]
     MessageNotInflight: Type[BotocoreClientError]
     OverLimit: Type[BotocoreClientError]
     PurgeQueueInProgress: Type[BotocoreClientError]
     QueueDeletedRecently: Type[BotocoreClientError]
     QueueDoesNotExist: Type[BotocoreClientError]
     QueueNameExists: Type[BotocoreClientError]
     ReceiptHandleIsInvalid: Type[BotocoreClientError]
+    RequestThrottled: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     TooManyEntriesInBatchRequest: Type[BotocoreClientError]
     UnsupportedOperation: Type[BotocoreClientError]
 
 class SQSClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)
@@ -151,15 +166,15 @@
         """
 
     def create_queue(
         self,
         *,
         QueueName: str,
         Attributes: Mapping[QueueAttributeNameType, str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateQueueResultTypeDef:
         """
         Creates a new standard or FIFO queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.create_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#create_queue)
         """
@@ -277,19 +292,20 @@
         """
 
     def receive_message(
         self,
         *,
         QueueUrl: str,
         AttributeNames: Sequence[QueueAttributeFilterType] = ...,
+        MessageSystemAttributeNames: Sequence[MessageSystemAttributeNameType] = ...,
         MessageAttributeNames: Sequence[str] = ...,
         MaxNumberOfMessages: int = ...,
         VisibilityTimeout: int = ...,
         WaitTimeSeconds: int = ...,
-        ReceiveRequestAttemptId: str = ...
+        ReceiveRequestAttemptId: str = ...,
     ) -> ReceiveMessageResultTypeDef:
         """
         Retrieves one or more messages (up to 10), from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.receive_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#receive_message)
         """
@@ -305,20 +321,20 @@
 
     def send_message(
         self,
         *,
         QueueUrl: str,
         MessageBody: str,
         DelaySeconds: int = ...,
-        MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueUnionTypeDef] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
-        MessageGroupId: str = ...
+        MessageGroupId: str = ...,
     ) -> SendMessageResultTypeDef:
         """
         Delivers a message to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message)
         """
@@ -336,15 +352,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message_batch)
         """
 
     def set_queue_attributes(
         self, *, QueueUrl: str, Attributes: Mapping[QueueAttributeNameType, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Sets the value of one or more queue attributes.
+        Sets the value of one or more queue attributes, like a policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.set_queue_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#set_queue_attributes)
         """
 
     def start_message_move_task(
         self, *, SourceArn: str, DestinationArn: str = ..., MaxNumberOfMessagesPerSecond: int = ...
```

### Comparing `mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/literals.py` & `mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,35 +15,34 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListDeadLetterSourceQueuesPaginatorName",
     "ListQueuesPaginatorName",
     "MessageSystemAttributeNameForSendsType",
     "MessageSystemAttributeNameType",
     "QueueAttributeFilterType",
     "QueueAttributeNameType",
     "SQSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListDeadLetterSourceQueuesPaginatorName = Literal["list_dead_letter_source_queues"]
 ListQueuesPaginatorName = Literal["list_queues"]
 MessageSystemAttributeNameForSendsType = Literal["AWSTraceHeader"]
 MessageSystemAttributeNameType = Literal[
     "AWSTraceHeader",
+    "All",
     "ApproximateFirstReceiveTimestamp",
     "ApproximateReceiveCount",
     "DeadLetterQueueSourceArn",
     "MessageDeduplicationId",
     "MessageGroupId",
     "SenderId",
     "SentTimestamp",
@@ -128,14 +127,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -146,14 +146,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -171,14 +172,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -191,24 +193,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -269,15 +273,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -349,17 +352,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -404,14 +409,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -449,19 +455,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -504,14 +512,15 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
+    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/literals.pyi` & `mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 )
 
 ListDeadLetterSourceQueuesPaginatorName = Literal["list_dead_letter_source_queues"]
 ListQueuesPaginatorName = Literal["list_queues"]
 MessageSystemAttributeNameForSendsType = Literal["AWSTraceHeader"]
 MessageSystemAttributeNameType = Literal[
     "AWSTraceHeader",
+    "All",
     "ApproximateFirstReceiveTimestamp",
     "ApproximateReceiveCount",
     "DeadLetterQueueSourceArn",
     "MessageDeduplicationId",
     "MessageGroupId",
     "SenderId",
     "SentTimestamp",
@@ -126,14 +127,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -144,14 +146,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -169,14 +172,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -189,24 +193,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -267,15 +273,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -347,17 +352,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -402,14 +409,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -447,19 +455,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -502,14 +512,15 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
+    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/paginator.py` & `mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -30,40 +30,36 @@
     ListDeadLetterSourceQueuesResultTypeDef,
     ListQueuesResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListDeadLetterSourceQueuesPaginator", "ListQueuesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListDeadLetterSourceQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
     """
 
     def paginate(
         self, *, QueueUrl: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeadLetterSourceQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
         """
 
-
 class ListQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/paginator.pyi` & `mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,34 +32,37 @@
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListDeadLetterSourceQueuesPaginator", "ListQueuesPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListDeadLetterSourceQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
     """
 
     def paginate(
         self, *, QueueUrl: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeadLetterSourceQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
         """
 
+
 class ListQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/service_resource.py` & `mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,28 +32,27 @@
     QueueAttributeNameType,
 )
 from .type_defs import (
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultTypeDef,
-    MessageAttributeValueQueueTypeDef,
+    MessageAttributeValueExtraOutputTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
-    SendMessageBatchRequestEntryQueueTypeDef,
+    SendMessageBatchRequestEntryTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "SQSServiceResource",
     "Message",
     "Queue",
     "ServiceResourceQueuesCollection",
     "QueueDeadLetterSourceQueuesCollection",
 )
@@ -157,17 +156,18 @@
     """
 
     message_id: str
     md5_of_body: str
     body: str
     attributes: Dict[MessageSystemAttributeNameType, str]
     md5_of_message_attributes: str
-    message_attributes: Dict[str, MessageAttributeValueTypeDef]
+    message_attributes: Dict[str, MessageAttributeValueExtraOutputTypeDef]
     queue_url: str
     receipt_handle: str
+    meta: "SQSResourceMeta"
 
     def Queue(self) -> "_Queue":
         """
         Creates a Queue resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Message.Queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#messagequeue-method)
@@ -206,16 +206,17 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Queue)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queue)
     """
 
     attributes: Dict[QueueAttributeNameType, str]
     url: str
     dead_letter_source_queues: QueueDeadLetterSourceQueuesCollection
+    meta: "SQSResourceMeta"
 
-    def Message(self, receipt_handle: str) -> _Message:
+    def Message(self, receipt_handle: str) -> "_Message":
         """
         Creates a Message resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.Message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuemessage-method)
         """
 
@@ -287,20 +288,21 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuepurge-method)
         """
 
     def receive_messages(
         self,
         *,
         AttributeNames: Sequence[QueueAttributeFilterType] = ...,
+        MessageSystemAttributeNames: Sequence[MessageSystemAttributeNameType] = ...,
         MessageAttributeNames: Sequence[str] = ...,
         MaxNumberOfMessages: int = ...,
         VisibilityTimeout: int = ...,
         WaitTimeSeconds: int = ...,
-        ReceiveRequestAttemptId: str = ...
-    ) -> List[_Message]:
+        ReceiveRequestAttemptId: str = ...,
+    ) -> List["_Message"]:
         """
         Retrieves one or more messages (up to 10), from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.receive_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuereceive_messages-method)
         """
 
@@ -324,44 +326,44 @@
         """
 
     def send_message(
         self,
         *,
         MessageBody: str,
         DelaySeconds: int = ...,
-        MessageAttributes: Mapping[str, MessageAttributeValueQueueTypeDef] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
-        MessageGroupId: str = ...
+        MessageGroupId: str = ...,
     ) -> SendMessageResultTypeDef:
         """
         Delivers a message to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_message-method)
         """
 
     def send_messages(
-        self, *, Entries: Sequence[SendMessageBatchRequestEntryQueueTypeDef]
+        self, *, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
         You can use `SendMessageBatch` to send up to 10 messages to the specified queue
         by assigning either identical or different values to each message (or by not
         assigning values at
         all).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_messages-method)
         """
 
     def set_attributes(self, *, Attributes: Mapping[QueueAttributeNameType, str]) -> None:
         """
-        Sets the value of one or more queue attributes.
+        Sets the value of one or more queue attributes, like a policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.set_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queueset_attributes-method)
         """
 
 
 _Queue = Queue
@@ -376,37 +378,37 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/)
     """
 
     meta: "SQSResourceMeta"
     queues: ServiceResourceQueuesCollection
 
-    def Message(self, queue_url: str, receipt_handle: str) -> _Message:
+    def Message(self, queue_url: str, receipt_handle: str) -> "_Message":
         """
         Creates a Message resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#sqsserviceresourcemessage-method)
         """
 
-    def Queue(self, url: str) -> _Queue:
+    def Queue(self, url: str) -> "_Queue":
         """
         Creates a Queue resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#sqsserviceresourcequeue-method)
         """
 
     def create_queue(
         self,
         *,
         QueueName: str,
         Attributes: Mapping[QueueAttributeNameType, str] = ...,
-        tags: Mapping[str, str] = ...
-    ) -> _Queue:
+        tags: Mapping[str, str] = ...,
+    ) -> "_Queue":
         """
         Creates a new standard or FIFO queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.create_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#sqsserviceresourcecreate_queue-method)
         """
 
@@ -414,14 +416,14 @@
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.get_available_subresources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#sqsserviceresourceget_available_subresources-method)
         """
 
-    def get_queue_by_name(self, *, QueueName: str, QueueOwnerAWSAccountId: str = ...) -> _Queue:
+    def get_queue_by_name(self, *, QueueName: str, QueueOwnerAWSAccountId: str = ...) -> "_Queue":
         """
         Returns the URL of an existing Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.get_queue_by_name)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#sqsserviceresourceget_queue_by_name-method)
         """
```

### Comparing `mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/service_resource.pyi` & `mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -32,18 +32,18 @@
     QueueAttributeNameType,
 )
 from .type_defs import (
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultTypeDef,
-    MessageAttributeValueQueueTypeDef,
+    MessageAttributeValueExtraOutputTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
-    SendMessageBatchRequestEntryQueueTypeDef,
+    SendMessageBatchRequestEntryTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
@@ -153,17 +153,18 @@
     """
 
     message_id: str
     md5_of_body: str
     body: str
     attributes: Dict[MessageSystemAttributeNameType, str]
     md5_of_message_attributes: str
-    message_attributes: Dict[str, MessageAttributeValueTypeDef]
+    message_attributes: Dict[str, MessageAttributeValueExtraOutputTypeDef]
     queue_url: str
     receipt_handle: str
+    meta: "SQSResourceMeta"
 
     def Queue(self) -> "_Queue":
         """
         Creates a Queue resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Message.Queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#messagequeue-method)
@@ -200,16 +201,17 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Queue)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queue)
     """
 
     attributes: Dict[QueueAttributeNameType, str]
     url: str
     dead_letter_source_queues: QueueDeadLetterSourceQueuesCollection
+    meta: "SQSResourceMeta"
 
-    def Message(self, receipt_handle: str) -> _Message:
+    def Message(self, receipt_handle: str) -> "_Message":
         """
         Creates a Message resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.Message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuemessage-method)
         """
 
@@ -281,20 +283,21 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuepurge-method)
         """
 
     def receive_messages(
         self,
         *,
         AttributeNames: Sequence[QueueAttributeFilterType] = ...,
+        MessageSystemAttributeNames: Sequence[MessageSystemAttributeNameType] = ...,
         MessageAttributeNames: Sequence[str] = ...,
         MaxNumberOfMessages: int = ...,
         VisibilityTimeout: int = ...,
         WaitTimeSeconds: int = ...,
-        ReceiveRequestAttemptId: str = ...
-    ) -> List[_Message]:
+        ReceiveRequestAttemptId: str = ...,
+    ) -> List["_Message"]:
         """
         Retrieves one or more messages (up to 10), from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.receive_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuereceive_messages-method)
         """
 
@@ -318,44 +321,44 @@
         """
 
     def send_message(
         self,
         *,
         MessageBody: str,
         DelaySeconds: int = ...,
-        MessageAttributes: Mapping[str, MessageAttributeValueQueueTypeDef] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
-        MessageGroupId: str = ...
+        MessageGroupId: str = ...,
     ) -> SendMessageResultTypeDef:
         """
         Delivers a message to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_message-method)
         """
 
     def send_messages(
-        self, *, Entries: Sequence[SendMessageBatchRequestEntryQueueTypeDef]
+        self, *, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
         You can use `SendMessageBatch` to send up to 10 messages to the specified queue
         by assigning either identical or different values to each message (or by not
         assigning values at
         all).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_messages-method)
         """
 
     def set_attributes(self, *, Attributes: Mapping[QueueAttributeNameType, str]) -> None:
         """
-        Sets the value of one or more queue attributes.
+        Sets the value of one or more queue attributes, like a policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.set_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queueset_attributes-method)
         """
 
 _Queue = Queue
 
@@ -367,37 +370,37 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/)
     """
 
     meta: "SQSResourceMeta"
     queues: ServiceResourceQueuesCollection
 
-    def Message(self, queue_url: str, receipt_handle: str) -> _Message:
+    def Message(self, queue_url: str, receipt_handle: str) -> "_Message":
         """
         Creates a Message resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#sqsserviceresourcemessage-method)
         """
 
-    def Queue(self, url: str) -> _Queue:
+    def Queue(self, url: str) -> "_Queue":
         """
         Creates a Queue resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#sqsserviceresourcequeue-method)
         """
 
     def create_queue(
         self,
         *,
         QueueName: str,
         Attributes: Mapping[QueueAttributeNameType, str] = ...,
-        tags: Mapping[str, str] = ...
-    ) -> _Queue:
+        tags: Mapping[str, str] = ...,
+    ) -> "_Queue":
         """
         Creates a new standard or FIFO queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.create_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#sqsserviceresourcecreate_queue-method)
         """
 
@@ -405,14 +408,14 @@
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.get_available_subresources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#sqsserviceresourceget_available_subresources-method)
         """
 
-    def get_queue_by_name(self, *, QueueName: str, QueueOwnerAWSAccountId: str = ...) -> _Queue:
+    def get_queue_by_name(self, *, QueueName: str, QueueOwnerAWSAccountId: str = ...) -> "_Queue":
         """
         Returns the URL of an existing Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.get_queue_by_name)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#sqsserviceresourceget_queue_by_name-method)
         """
```

### Comparing `mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/type_defs.py` & `mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddPermissionRequestQueueAddPermissionTypeDef",
     "AddPermissionRequestRequestTypeDef",
     "BatchResultErrorEntryTypeDef",
     "BlobTypeDef",
     "CancelMessageMoveTaskRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
@@ -59,27 +58,28 @@
     "GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
     "PaginatorConfigTypeDef",
     "ListDeadLetterSourceQueuesRequestRequestTypeDef",
     "ListMessageMoveTasksRequestRequestTypeDef",
     "ListMessageMoveTasksResultEntryTypeDef",
     "ListQueueTagsRequestRequestTypeDef",
     "ListQueuesRequestRequestTypeDef",
-    "MessageAttributeValueTypeDef",
+    "MessageAttributeValueExtraOutputTypeDef",
+    "MessageAttributeValueOutputTypeDef",
     "PurgeQueueRequestRequestTypeDef",
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     "ReceiveMessageRequestRequestTypeDef",
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "SendMessageBatchResultEntryTypeDef",
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     "SetQueueAttributesRequestRequestTypeDef",
     "StartMessageMoveTaskRequestRequestTypeDef",
     "TagQueueRequestRequestTypeDef",
     "UntagQueueRequestRequestTypeDef",
-    "MessageAttributeValueQueueTypeDef",
+    "MessageAttributeValueTypeDef",
     "MessageSystemAttributeValueTypeDef",
     "CancelMessageMoveTaskResultTypeDef",
     "CreateQueueResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetQueueAttributesResultTypeDef",
     "GetQueueUrlResultTypeDef",
     "ListDeadLetterSourceQueuesResultTypeDef",
@@ -94,19 +94,19 @@
     "DeleteMessageBatchRequestRequestTypeDef",
     "DeleteMessageBatchResultTypeDef",
     "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
     "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListMessageMoveTasksResultTypeDef",
     "MessageTypeDef",
     "SendMessageBatchResultTypeDef",
-    "SendMessageBatchRequestEntryQueueTypeDef",
+    "MessageAttributeValueUnionTypeDef",
     "SendMessageBatchRequestEntryTypeDef",
     "SendMessageRequestQueueSendMessageTypeDef",
-    "SendMessageRequestRequestTypeDef",
     "ReceiveMessageResultTypeDef",
+    "SendMessageRequestRequestTypeDef",
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     "SendMessageBatchRequestRequestTypeDef",
 )
 
 AddPermissionRequestQueueAddPermissionTypeDef = TypedDict(
     "AddPermissionRequestQueueAddPermissionTypeDef",
     {
@@ -140,18 +140,18 @@
         "TaskHandle": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 ChangeMessageVisibilityBatchRequestEntryTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchRequestEntryTypeDef",
     {
         "Id": str,
         "ReceiptHandle": str,
@@ -288,16 +288,26 @@
     "ListQueuesRequestRequestTypeDef",
     {
         "QueueNamePrefix": NotRequired[str],
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
     },
 )
-MessageAttributeValueTypeDef = TypedDict(
-    "MessageAttributeValueTypeDef",
+MessageAttributeValueExtraOutputTypeDef = TypedDict(
+    "MessageAttributeValueExtraOutputTypeDef",
+    {
+        "DataType": str,
+        "StringValue": NotRequired[str],
+        "BinaryValue": NotRequired[bytes],
+        "StringListValues": NotRequired[List[str]],
+        "BinaryListValues": NotRequired[List[bytes]],
+    },
+)
+MessageAttributeValueOutputTypeDef = TypedDict(
+    "MessageAttributeValueOutputTypeDef",
     {
         "DataType": str,
         "StringValue": NotRequired[str],
         "BinaryValue": NotRequired[bytes],
         "StringListValues": NotRequired[List[str]],
         "BinaryListValues": NotRequired[List[bytes]],
     },
@@ -308,26 +318,28 @@
         "QueueUrl": str,
     },
 )
 ReceiveMessageRequestQueueReceiveMessagesTypeDef = TypedDict(
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     {
         "AttributeNames": NotRequired[Sequence[QueueAttributeFilterType]],
+        "MessageSystemAttributeNames": NotRequired[Sequence[MessageSystemAttributeNameType]],
         "MessageAttributeNames": NotRequired[Sequence[str]],
         "MaxNumberOfMessages": NotRequired[int],
         "VisibilityTimeout": NotRequired[int],
         "WaitTimeSeconds": NotRequired[int],
         "ReceiveRequestAttemptId": NotRequired[str],
     },
 )
 ReceiveMessageRequestRequestTypeDef = TypedDict(
     "ReceiveMessageRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "AttributeNames": NotRequired[Sequence[QueueAttributeFilterType]],
+        "MessageSystemAttributeNames": NotRequired[Sequence[MessageSystemAttributeNameType]],
         "MessageAttributeNames": NotRequired[Sequence[str]],
         "MaxNumberOfMessages": NotRequired[int],
         "VisibilityTimeout": NotRequired[int],
         "WaitTimeSeconds": NotRequired[int],
         "ReceiveRequestAttemptId": NotRequired[str],
     },
 )
@@ -386,16 +398,16 @@
 UntagQueueRequestRequestTypeDef = TypedDict(
     "UntagQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "TagKeys": Sequence[str],
     },
 )
-MessageAttributeValueQueueTypeDef = TypedDict(
-    "MessageAttributeValueQueueTypeDef",
+MessageAttributeValueTypeDef = TypedDict(
+    "MessageAttributeValueTypeDef",
     {
         "DataType": str,
         "StringValue": NotRequired[str],
         "BinaryValue": NotRequired[BlobTypeDef],
         "StringListValues": NotRequired[Sequence[str]],
         "BinaryListValues": NotRequired[Sequence[BlobTypeDef]],
     },
@@ -444,31 +456,31 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
     "ListDeadLetterSourceQueuesResultTypeDef",
     {
         "queueUrls": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListQueueTagsResultTypeDef = TypedDict(
     "ListQueueTagsResultTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListQueuesResultTypeDef = TypedDict(
     "ListQueuesResultTypeDef",
     {
         "QueueUrls": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SendMessageResultTypeDef = TypedDict(
     "SendMessageResultTypeDef",
     {
         "MD5OfMessageBody": str,
         "MD5OfMessageAttributes": str,
@@ -553,39 +565,28 @@
     {
         "MessageId": NotRequired[str],
         "ReceiptHandle": NotRequired[str],
         "MD5OfBody": NotRequired[str],
         "Body": NotRequired[str],
         "Attributes": NotRequired[Dict[MessageSystemAttributeNameType, str]],
         "MD5OfMessageAttributes": NotRequired[str],
-        "MessageAttributes": NotRequired[Dict[str, MessageAttributeValueTypeDef]],
+        "MessageAttributes": NotRequired[Dict[str, MessageAttributeValueOutputTypeDef]],
     },
 )
 SendMessageBatchResultTypeDef = TypedDict(
     "SendMessageBatchResultTypeDef",
     {
         "Successful": List[SendMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-SendMessageBatchRequestEntryQueueTypeDef = TypedDict(
-    "SendMessageBatchRequestEntryQueueTypeDef",
-    {
-        "Id": str,
-        "MessageBody": str,
-        "DelaySeconds": NotRequired[int],
-        "MessageAttributes": NotRequired[Mapping[str, MessageAttributeValueQueueTypeDef]],
-        "MessageSystemAttributes": NotRequired[
-            Mapping[Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef]
-        ],
-        "MessageDeduplicationId": NotRequired[str],
-        "MessageGroupId": NotRequired[str],
-    },
-)
+MessageAttributeValueUnionTypeDef = Union[
+    MessageAttributeValueTypeDef, MessageAttributeValueExtraOutputTypeDef
+]
 SendMessageBatchRequestEntryTypeDef = TypedDict(
     "SendMessageBatchRequestEntryTypeDef",
     {
         "Id": str,
         "MessageBody": str,
         "DelaySeconds": NotRequired[int],
         "MessageAttributes": NotRequired[Mapping[str, MessageAttributeValueTypeDef]],
@@ -597,47 +598,47 @@
     },
 )
 SendMessageRequestQueueSendMessageTypeDef = TypedDict(
     "SendMessageRequestQueueSendMessageTypeDef",
     {
         "MessageBody": str,
         "DelaySeconds": NotRequired[int],
-        "MessageAttributes": NotRequired[Mapping[str, MessageAttributeValueQueueTypeDef]],
+        "MessageAttributes": NotRequired[Mapping[str, MessageAttributeValueTypeDef]],
         "MessageSystemAttributes": NotRequired[
             Mapping[Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef]
         ],
         "MessageDeduplicationId": NotRequired[str],
         "MessageGroupId": NotRequired[str],
     },
 )
+ReceiveMessageResultTypeDef = TypedDict(
+    "ReceiveMessageResultTypeDef",
+    {
+        "Messages": List[MessageTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 SendMessageRequestRequestTypeDef = TypedDict(
     "SendMessageRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "MessageBody": str,
         "DelaySeconds": NotRequired[int],
-        "MessageAttributes": NotRequired[Mapping[str, MessageAttributeValueTypeDef]],
+        "MessageAttributes": NotRequired[Mapping[str, MessageAttributeValueUnionTypeDef]],
         "MessageSystemAttributes": NotRequired[
             Mapping[Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef]
         ],
         "MessageDeduplicationId": NotRequired[str],
         "MessageGroupId": NotRequired[str],
     },
 )
-ReceiveMessageResultTypeDef = TypedDict(
-    "ReceiveMessageResultTypeDef",
-    {
-        "Messages": List[MessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 SendMessageBatchRequestQueueSendMessagesTypeDef = TypedDict(
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     {
-        "Entries": Sequence[SendMessageBatchRequestEntryQueueTypeDef],
+        "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
     },
 )
 SendMessageBatchRequestRequestTypeDef = TypedDict(
     "SendMessageBatchRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
```

### Comparing `mypy-boto3-sqs-1.34.0/mypy_boto3_sqs/type_defs.pyi` & `mypy_boto3_sqs-1.34.101/mypy_boto3_sqs/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -58,27 +58,28 @@
     "GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
     "PaginatorConfigTypeDef",
     "ListDeadLetterSourceQueuesRequestRequestTypeDef",
     "ListMessageMoveTasksRequestRequestTypeDef",
     "ListMessageMoveTasksResultEntryTypeDef",
     "ListQueueTagsRequestRequestTypeDef",
     "ListQueuesRequestRequestTypeDef",
-    "MessageAttributeValueTypeDef",
+    "MessageAttributeValueExtraOutputTypeDef",
+    "MessageAttributeValueOutputTypeDef",
     "PurgeQueueRequestRequestTypeDef",
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     "ReceiveMessageRequestRequestTypeDef",
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "SendMessageBatchResultEntryTypeDef",
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     "SetQueueAttributesRequestRequestTypeDef",
     "StartMessageMoveTaskRequestRequestTypeDef",
     "TagQueueRequestRequestTypeDef",
     "UntagQueueRequestRequestTypeDef",
-    "MessageAttributeValueQueueTypeDef",
+    "MessageAttributeValueTypeDef",
     "MessageSystemAttributeValueTypeDef",
     "CancelMessageMoveTaskResultTypeDef",
     "CreateQueueResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetQueueAttributesResultTypeDef",
     "GetQueueUrlResultTypeDef",
     "ListDeadLetterSourceQueuesResultTypeDef",
@@ -93,19 +94,19 @@
     "DeleteMessageBatchRequestRequestTypeDef",
     "DeleteMessageBatchResultTypeDef",
     "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
     "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListMessageMoveTasksResultTypeDef",
     "MessageTypeDef",
     "SendMessageBatchResultTypeDef",
-    "SendMessageBatchRequestEntryQueueTypeDef",
+    "MessageAttributeValueUnionTypeDef",
     "SendMessageBatchRequestEntryTypeDef",
     "SendMessageRequestQueueSendMessageTypeDef",
-    "SendMessageRequestRequestTypeDef",
     "ReceiveMessageResultTypeDef",
+    "SendMessageRequestRequestTypeDef",
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     "SendMessageBatchRequestRequestTypeDef",
 )
 
 AddPermissionRequestQueueAddPermissionTypeDef = TypedDict(
     "AddPermissionRequestQueueAddPermissionTypeDef",
     {
@@ -139,18 +140,18 @@
         "TaskHandle": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 ChangeMessageVisibilityBatchRequestEntryTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchRequestEntryTypeDef",
     {
         "Id": str,
         "ReceiptHandle": str,
@@ -287,16 +288,26 @@
     "ListQueuesRequestRequestTypeDef",
     {
         "QueueNamePrefix": NotRequired[str],
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
     },
 )
-MessageAttributeValueTypeDef = TypedDict(
-    "MessageAttributeValueTypeDef",
+MessageAttributeValueExtraOutputTypeDef = TypedDict(
+    "MessageAttributeValueExtraOutputTypeDef",
+    {
+        "DataType": str,
+        "StringValue": NotRequired[str],
+        "BinaryValue": NotRequired[bytes],
+        "StringListValues": NotRequired[List[str]],
+        "BinaryListValues": NotRequired[List[bytes]],
+    },
+)
+MessageAttributeValueOutputTypeDef = TypedDict(
+    "MessageAttributeValueOutputTypeDef",
     {
         "DataType": str,
         "StringValue": NotRequired[str],
         "BinaryValue": NotRequired[bytes],
         "StringListValues": NotRequired[List[str]],
         "BinaryListValues": NotRequired[List[bytes]],
     },
@@ -307,26 +318,28 @@
         "QueueUrl": str,
     },
 )
 ReceiveMessageRequestQueueReceiveMessagesTypeDef = TypedDict(
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     {
         "AttributeNames": NotRequired[Sequence[QueueAttributeFilterType]],
+        "MessageSystemAttributeNames": NotRequired[Sequence[MessageSystemAttributeNameType]],
         "MessageAttributeNames": NotRequired[Sequence[str]],
         "MaxNumberOfMessages": NotRequired[int],
         "VisibilityTimeout": NotRequired[int],
         "WaitTimeSeconds": NotRequired[int],
         "ReceiveRequestAttemptId": NotRequired[str],
     },
 )
 ReceiveMessageRequestRequestTypeDef = TypedDict(
     "ReceiveMessageRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "AttributeNames": NotRequired[Sequence[QueueAttributeFilterType]],
+        "MessageSystemAttributeNames": NotRequired[Sequence[MessageSystemAttributeNameType]],
         "MessageAttributeNames": NotRequired[Sequence[str]],
         "MaxNumberOfMessages": NotRequired[int],
         "VisibilityTimeout": NotRequired[int],
         "WaitTimeSeconds": NotRequired[int],
         "ReceiveRequestAttemptId": NotRequired[str],
     },
 )
@@ -385,16 +398,16 @@
 UntagQueueRequestRequestTypeDef = TypedDict(
     "UntagQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "TagKeys": Sequence[str],
     },
 )
-MessageAttributeValueQueueTypeDef = TypedDict(
-    "MessageAttributeValueQueueTypeDef",
+MessageAttributeValueTypeDef = TypedDict(
+    "MessageAttributeValueTypeDef",
     {
         "DataType": str,
         "StringValue": NotRequired[str],
         "BinaryValue": NotRequired[BlobTypeDef],
         "StringListValues": NotRequired[Sequence[str]],
         "BinaryListValues": NotRequired[Sequence[BlobTypeDef]],
     },
@@ -443,31 +456,31 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
     "ListDeadLetterSourceQueuesResultTypeDef",
     {
         "queueUrls": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListQueueTagsResultTypeDef = TypedDict(
     "ListQueueTagsResultTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListQueuesResultTypeDef = TypedDict(
     "ListQueuesResultTypeDef",
     {
         "QueueUrls": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SendMessageResultTypeDef = TypedDict(
     "SendMessageResultTypeDef",
     {
         "MD5OfMessageBody": str,
         "MD5OfMessageAttributes": str,
@@ -552,39 +565,28 @@
     {
         "MessageId": NotRequired[str],
         "ReceiptHandle": NotRequired[str],
         "MD5OfBody": NotRequired[str],
         "Body": NotRequired[str],
         "Attributes": NotRequired[Dict[MessageSystemAttributeNameType, str]],
         "MD5OfMessageAttributes": NotRequired[str],
-        "MessageAttributes": NotRequired[Dict[str, MessageAttributeValueTypeDef]],
+        "MessageAttributes": NotRequired[Dict[str, MessageAttributeValueOutputTypeDef]],
     },
 )
 SendMessageBatchResultTypeDef = TypedDict(
     "SendMessageBatchResultTypeDef",
     {
         "Successful": List[SendMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-SendMessageBatchRequestEntryQueueTypeDef = TypedDict(
-    "SendMessageBatchRequestEntryQueueTypeDef",
-    {
-        "Id": str,
-        "MessageBody": str,
-        "DelaySeconds": NotRequired[int],
-        "MessageAttributes": NotRequired[Mapping[str, MessageAttributeValueQueueTypeDef]],
-        "MessageSystemAttributes": NotRequired[
-            Mapping[Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef]
-        ],
-        "MessageDeduplicationId": NotRequired[str],
-        "MessageGroupId": NotRequired[str],
-    },
-)
+MessageAttributeValueUnionTypeDef = Union[
+    MessageAttributeValueTypeDef, MessageAttributeValueExtraOutputTypeDef
+]
 SendMessageBatchRequestEntryTypeDef = TypedDict(
     "SendMessageBatchRequestEntryTypeDef",
     {
         "Id": str,
         "MessageBody": str,
         "DelaySeconds": NotRequired[int],
         "MessageAttributes": NotRequired[Mapping[str, MessageAttributeValueTypeDef]],
@@ -596,47 +598,47 @@
     },
 )
 SendMessageRequestQueueSendMessageTypeDef = TypedDict(
     "SendMessageRequestQueueSendMessageTypeDef",
     {
         "MessageBody": str,
         "DelaySeconds": NotRequired[int],
-        "MessageAttributes": NotRequired[Mapping[str, MessageAttributeValueQueueTypeDef]],
+        "MessageAttributes": NotRequired[Mapping[str, MessageAttributeValueTypeDef]],
         "MessageSystemAttributes": NotRequired[
             Mapping[Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef]
         ],
         "MessageDeduplicationId": NotRequired[str],
         "MessageGroupId": NotRequired[str],
     },
 )
+ReceiveMessageResultTypeDef = TypedDict(
+    "ReceiveMessageResultTypeDef",
+    {
+        "Messages": List[MessageTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 SendMessageRequestRequestTypeDef = TypedDict(
     "SendMessageRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "MessageBody": str,
         "DelaySeconds": NotRequired[int],
-        "MessageAttributes": NotRequired[Mapping[str, MessageAttributeValueTypeDef]],
+        "MessageAttributes": NotRequired[Mapping[str, MessageAttributeValueUnionTypeDef]],
         "MessageSystemAttributes": NotRequired[
             Mapping[Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef]
         ],
         "MessageDeduplicationId": NotRequired[str],
         "MessageGroupId": NotRequired[str],
     },
 )
-ReceiveMessageResultTypeDef = TypedDict(
-    "ReceiveMessageResultTypeDef",
-    {
-        "Messages": List[MessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 SendMessageBatchRequestQueueSendMessagesTypeDef = TypedDict(
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     {
-        "Entries": Sequence[SendMessageBatchRequestEntryQueueTypeDef],
+        "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
     },
 )
 SendMessageBatchRequestRequestTypeDef = TypedDict(
     "SendMessageBatchRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
```

### Comparing `mypy-boto3-sqs-1.34.0/mypy_boto3_sqs.egg-info/PKG-INFO` & `mypy_boto3_sqs-1.34.101/mypy_boto3_sqs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sqs
-Version: 1.34.0
-Summary: Type annotations for boto3.SQS 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.101
+Summary: Type annotations for boto3.SQS 1.34.101 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-sqs"></a>
 
 # mypy-boto3-sqs
 
 [![PyPI - mypy-boto3-sqs](https://img.shields.io/pypi/v/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sqs)](https://pepy.tech/project/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.34.101](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sqs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sqs-1.34.0/mypy_boto3_sqs.egg-info/SOURCES.txt` & `mypy_boto3_sqs-1.34.101/mypy_boto3_sqs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.34.0/setup.py` & `mypy_boto3_sqs-1.34.101/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,47 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sqs",
-    version="1.34.0",
+    version="1.34.101",
     packages=["mypy_boto3_sqs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.SQS 1.34.0 service generated with mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.SQS 1.34.101 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 sqs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_sqs": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

