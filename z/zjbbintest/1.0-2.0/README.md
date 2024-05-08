# Comparing `tmp/zjbbintest-1.0.tar.gz` & `tmp/zjbbintest-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zjbbintest-1.0.tar", last modified: Tue May  7 12:36:05 2024, max compression
+gzip compressed data, was "dist/zjbbintest-2.0.tar", last modified: Wed May  8 07:06:01 2024, max compression
```

## Comparing `zjbbintest-1.0.tar` & `zjbbintest-2.0.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-07 12:36:05.694549 zjbbintest-1.0/
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-07 12:36:05.690551 zjbbintest-1.0/Actuator/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:19:26.000000 zjbbintest-1.0/Actuator/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      746 2024-04-21 08:57:59.000000 zjbbintest-1.0/Actuator/actuator.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-07 12:36:05.690877 zjbbintest-1.0/Actuator/bin_test_case/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-21 09:12:36.000000 zjbbintest-1.0/Actuator/bin_test_case/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)    12670 2024-05-07 08:32:04.000000 zjbbintest-1.0/Actuator/bin_test_case/bin_test_case.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-07 12:36:05.691532 zjbbintest-1.0/Actuator/bin_test_exception/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)       60 2024-04-16 07:11:01.000000 zjbbintest-1.0/Actuator/bin_test_exception/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3663 2024-04-30 03:43:11.000000 zjbbintest-1.0/Actuator/bin_test_exception/bin_test_exception.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-07 12:36:05.693374 zjbbintest-1.0/Actuator/utils/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:21:41.000000 zjbbintest-1.0/Actuator/utils/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      962 2024-04-24 12:48:19.000000 zjbbintest-1.0/Actuator/utils/action_execution.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     6339 2024-05-07 07:36:53.000000 zjbbintest-1.0/Actuator/utils/assert_execution.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3703 2024-04-21 14:20:00.000000 zjbbintest-1.0/Actuator/utils/format_check.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1110 2024-04-22 09:45:48.000000 zjbbintest-1.0/Actuator/utils/processing_path.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     7975 2024-05-07 07:19:41.000000 zjbbintest-1.0/Actuator/utils/requestor.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     9005 2024-05-07 06:09:28.000000 zjbbintest-1.0/Actuator/utils/string_dynamic_run.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      133 2024-05-07 12:36:05.694348 zjbbintest-1.0/PKG-INFO
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      514 2024-05-07 11:52:14.000000 zjbbintest-1.0/README.md
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)       38 2024-05-07 12:36:05.694591 zjbbintest-1.0/setup.cfg
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      613 2024-05-07 12:32:23.000000 zjbbintest-1.0/setup.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-07 12:36:05.694176 zjbbintest-1.0/zjbbintest.egg-info/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      133 2024-05-07 12:36:05.000000 zjbbintest-1.0/zjbbintest.egg-info/PKG-INFO
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      621 2024-05-07 12:36:05.000000 zjbbintest-1.0/zjbbintest.egg-info/SOURCES.txt
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        1 2024-05-07 12:36:05.000000 zjbbintest-1.0/zjbbintest.egg-info/dependency_links.txt
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      293 2024-05-07 12:36:05.000000 zjbbintest-1.0/zjbbintest.egg-info/requires.txt
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        9 2024-05-07 12:36:05.000000 zjbbintest-1.0/zjbbintest.egg-info/top_level.txt
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:06:01.017897 zjbbintest-2.0/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-08 07:06:01.017654 zjbbintest-2.0/PKG-INFO
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      514 2024-05-07 11:52:14.000000 zjbbintest-2.0/README.md
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)       38 2024-05-08 07:06:01.017942 zjbbintest-2.0/setup.cfg
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      727 2024-05-08 07:05:41.000000 zjbbintest-2.0/setup.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:06:01.014267 zjbbintest-2.0/zjbbintest/
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:06:01.015413 zjbbintest-2.0/zjbbintest/Actuator/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:19:26.000000 zjbbintest-2.0/zjbbintest/Actuator/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      746 2024-04-21 08:57:59.000000 zjbbintest-2.0/zjbbintest/Actuator/actuator.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:06:01.015705 zjbbintest-2.0/zjbbintest/Actuator/bin_test_case/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:16.000000 zjbbintest-2.0/zjbbintest/Actuator/bin_test_case/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)    12711 2024-05-08 05:24:56.000000 zjbbintest-2.0/zjbbintest/Actuator/bin_test_case/bin_test_case.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:06:01.015999 zjbbintest-2.0/zjbbintest/Actuator/bin_test_exception/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:22.000000 zjbbintest-2.0/zjbbintest/Actuator/bin_test_exception/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3663 2024-04-30 03:43:11.000000 zjbbintest-2.0/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:06:01.017249 zjbbintest-2.0/zjbbintest/Actuator/utils/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:21:41.000000 zjbbintest-2.0/zjbbintest/Actuator/utils/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      973 2024-05-08 05:24:56.000000 zjbbintest-2.0/zjbbintest/Actuator/utils/action_execution.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     6391 2024-05-08 06:54:18.000000 zjbbintest-2.0/zjbbintest/Actuator/utils/assert_execution.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3733 2024-05-08 06:54:26.000000 zjbbintest-2.0/zjbbintest/Actuator/utils/format_check.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1110 2024-04-22 09:45:48.000000 zjbbintest-2.0/zjbbintest/Actuator/utils/processing_path.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     8016 2024-05-08 06:54:35.000000 zjbbintest-2.0/zjbbintest/Actuator/utils/requestor.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     9046 2024-05-08 06:54:04.000000 zjbbintest-2.0/zjbbintest/Actuator/utils/string_dynamic_run.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:06:01.017467 zjbbintest-2.0/zjbbintest/Template/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 05:24:09.000000 zjbbintest-2.0/zjbbintest/Template/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1261 2024-05-07 09:04:47.000000 zjbbintest-2.0/zjbbintest/Template/bintest_template.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:50:15.000000 zjbbintest-2.0/zjbbintest/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     9912 2024-05-08 06:57:05.000000 zjbbintest-2.0/zjbbintest/bintest.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      501 2024-04-23 04:49:02.000000 zjbbintest-2.0/zjbbintest/bintest_data.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 07:06:01.015160 zjbbintest-2.0/zjbbintest.egg-info/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-08 07:06:00.000000 zjbbintest-2.0/zjbbintest.egg-info/PKG-INFO
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      908 2024-05-08 07:06:00.000000 zjbbintest-2.0/zjbbintest.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        1 2024-05-08 07:06:00.000000 zjbbintest-2.0/zjbbintest.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      293 2024-05-08 07:06:00.000000 zjbbintest-2.0/zjbbintest.egg-info/requires.txt
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)       11 2024-05-08 07:06:00.000000 zjbbintest-2.0/zjbbintest.egg-info/top_level.txt
```

### Comparing `zjbbintest-1.0/Actuator/actuator.py` & `zjbbintest-2.0/zjbbintest/Actuator/actuator.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-1.0/Actuator/bin_test_case/bin_test_case.py` & `zjbbintest-2.0/zjbbintest/Actuator/bin_test_case/bin_test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 This module provide configigure file management service in i18n environment.
 
 Authors: zhangjiabin01
 Date: 2024/4/21 16:56:00
 """
 import logging
 
-import Actuator.bin_test_exception as bt_exception
-from Actuator.utils.action_execution import BatchActionExecutor
-from Actuator.utils.assert_execution import BatchAssertExecutor
-from Actuator.utils.format_check import check_case
-from Actuator.utils.requestor import RequestObject
+from zjbbintest import Actuator as bt_exception
+from zjbbintest.Actuator.utils.action_execution import BatchActionExecutor
+from zjbbintest.Actuator.utils.assert_execution import BatchAssertExecutor
+from zjbbintest.Actuator.utils.format_check import check_case
+from zjbbintest.Actuator.utils.requestor import RequestObject
 from enum import Enum
 import json
 
 
 class CaseRunStatus(Enum):
     """
     case执行状态枚举，
```

### Comparing `zjbbintest-1.0/Actuator/bin_test_exception/bin_test_exception.py` & `zjbbintest-2.0/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-1.0/Actuator/utils/action_execution.py` & `zjbbintest-2.0/zjbbintest/Actuator/utils/action_execution.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Copyright (c) 2024 Baidu.com, Inc. All Rights Reserved
 This module provide configigure file management service in i18n environment.
 
 Authors: zhangjiabin01
 Date: 2024/4/20 19:02:00
 """
-from Actuator.utils.string_dynamic_run import StringDynamicRun
+from zjbbintest.Actuator.utils.string_dynamic_run import StringDynamicRun
 
 
 class BatchActionExecutor:
     """
     Batch action executor.
     批量动作执行器
     """
```

### Comparing `zjbbintest-1.0/Actuator/utils/assert_execution.py` & `zjbbintest-2.0/zjbbintest/Actuator/utils/assert_execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Copyright (c) 2024 Baidu.com, Inc. All Rights Reserved
 This module provide configigure file management service in i18n environment.
 
 Authors: zhangjiabin01
 Date: 2024/4/20 17:33:00
 """
-from Actuator.utils.string_dynamic_run import StringDynamicRun
-from bintest_data import BinTestData
-from Actuator.bin_test_exception import AssertFailException, BTAssertNotFoundException, BTAssertDictFormatException
+from zjbbintest.Actuator.utils.string_dynamic_run import StringDynamicRun
+from zjbbintest.bintest_data import BinTestData
+from zjbbintest.Actuator.bin_test_exception.bin_test_exception import AssertFailException, BTAssertNotFoundException, BTAssertDictFormatException
 
 
 class AssertDict:
     """
     常见断言字典
     """
     EQUALS = ["=", "==", "相等", "等于", "一致", "一样"]
```

### Comparing `zjbbintest-1.0/Actuator/utils/format_check.py` & `zjbbintest-2.0/zjbbintest/Actuator/utils/format_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This module provide configigure file management service in i18n environment.
 
 Authors: zhangjiabin01
 Date: 2024/4/10 16:00:00
 """
 from jsonschema import validate, ValidationError
 
-from Actuator.bin_test_exception import FormatCheckException
+from zjbbintest.Actuator.bin_test_exception.bin_test_exception import FormatCheckException
 
 case_json_schema = {
     "type": "object",
     "properties": {
         "caseName": {
             "type": "string"
         },
```

### Comparing `zjbbintest-1.0/Actuator/utils/processing_path.py` & `zjbbintest-2.0/zjbbintest/Actuator/utils/processing_path.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-1.0/Actuator/utils/requestor.py` & `zjbbintest-2.0/zjbbintest/Actuator/utils/requestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 Authors: zhangjiabin01
 Date: 2024/4/10 20:25:00
 """
 from urllib.parse import urljoin
 import requests
 import json
 
-from Actuator.bin_test_exception import RequestException
-from Actuator.utils.string_dynamic_run import StringDynamicRun
+from zjbbintest.Actuator.bin_test_exception.bin_test_exception import RequestException
+from zjbbintest.Actuator.utils.string_dynamic_run import StringDynamicRun
 
 
 class RequestObject:
     """
     将请求封装成一个对象，方便后续处理
     """
```

### Comparing `zjbbintest-1.0/Actuator/utils/string_dynamic_run.py` & `zjbbintest-2.0/zjbbintest/Actuator/utils/string_dynamic_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 This module provide configigure file management service in i18n environment.
 
 Authors: zhangjiabin01
 Date: 2024/4/12 19:18:00
 """
 import itertools
 
-from Actuator.bin_test_exception import FormatBTStringException, BTFuncNotFoundException, BTActionNotFoundException
-from bintest_data import BinTestData
+from zjbbintest.Actuator.bin_test_exception.bin_test_exception import FormatBTStringException, BTFuncNotFoundException, BTActionNotFoundException
+from zjbbintest.bintest_data import BinTestData
 
 
 class StringDynamicRun:
     """
     字符串动态执行方法
     主要处理$BT[]中的conf()、func()和var()，通过run方法将字符串变为单纯的纯文本字符串
     """
```

### Comparing `zjbbintest-1.0/README.md` & `zjbbintest-2.0/README.md`

 * *Files identical despite different names*

### Comparing `zjbbintest-1.0/setup.py` & `zjbbintest-2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zjbbintest',
-    version='1.0',
+    version='2.0',
+    author="zhangjiabin01",
+    author_email="zhangjiabin01@baidu.com",
+    description="bintest自动化框架",
     packages=find_packages(),
     install_requires=[
         'attrs==23.2.0',
         'certifi==2024.2.2',
         'charset-normalizer==3.3.2',
         'idna==3.7',
         'importlib_resources==6.4.0',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

