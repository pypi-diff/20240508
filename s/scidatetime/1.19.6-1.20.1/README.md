# Comparing `tmp/scidatetime-1.19.6.tar.gz` & `tmp/scidatetime-1.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scidatetime-1.19.6.tar", last modified: Thu Jan 18 04:27:44 2024, max compression
+gzip compressed data, was "scidatetime-1.20.1.tar", last modified: Wed May  8 06:23:43 2024, max compression
```

## Comparing `scidatetime-1.19.6.tar` & `scidatetime-1.20.1.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 04:27:44.143972 scidatetime-1.19.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-18 04:27:32.000000 scidatetime-1.19.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-01-18 04:27:44.143972 scidatetime-1.19.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-01-18 04:27:32.000000 scidatetime-1.19.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 04:27:44.135972 scidatetime-1.19.6/scidatetime/
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 04:27:44.139972 scidatetime-1.19.6/scidatetime/dateutil/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/_common.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/easter.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/easter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 04:27:44.139972 scidatetime-1.19.6/scidatetime/dateutil/parser/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/parser/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    58803 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/parser/_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/parser/isoparser.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/parser/isoparser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24905 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/relativedelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/relativedelta.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    66567 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/rrule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/rrule.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 04:27:44.143972 scidatetime-1.19.6/scidatetime/dateutil/tz/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/tz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/tz/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/tz/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/tz/_common.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/tz/_factories.py
--rw-r--r--   0 runner    (1001) docker     (127)    62868 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/tz/tz.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/tz/tz.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12937 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/tz/win.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/tzwin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 04:27:44.143972 scidatetime-1.19.6/scidatetime/dateutil/zoneinfo/
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/zoneinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-01-18 04:27:32.000000 scidatetime-1.19.6/scidatetime/dateutil/zoneinfo/rebuild.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 04:27:44.143972 scidatetime-1.19.6/scidatetime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-01-18 04:27:44.000000 scidatetime-1.19.6/scidatetime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-01-18 04:27:44.000000 scidatetime-1.19.6/scidatetime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 04:27:44.000000 scidatetime-1.19.6/scidatetime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 04:27:44.000000 scidatetime-1.19.6/scidatetime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-18 04:27:44.000000 scidatetime-1.19.6/scidatetime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-18 04:27:44.000000 scidatetime-1.19.6/scidatetime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 04:27:44.143972 scidatetime-1.19.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-01-18 04:27:32.000000 scidatetime-1.19.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 04:27:44.143972 scidatetime-1.19.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-01-18 04:27:32.000000 scidatetime-1.19.6/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-18 04:27:32.000000 scidatetime-1.19.6/tests/test_origin_polute.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-01-18 04:27:32.000000 scidatetime-1.19.6/tests/test_timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.035148 scidatetime-1.20.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-08 06:23:34.000000 scidatetime-1.20.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-08 06:23:43.035148 scidatetime-1.20.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-08 06:23:34.000000 scidatetime-1.20.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.027148 scidatetime-1.20.1/scidatetime/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/DateTimeParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/MdlDateTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.031148 scidatetime-1.20.1/scidatetime/dateutil/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/_common.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/easter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/easter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.031148 scidatetime-1.20.1/scidatetime/dateutil/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/parser/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    58803 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/parser/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/parser/isoparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/parser/isoparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24905 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/relativedelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/relativedelta.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    66567 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/rrule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/rrule.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.035148 scidatetime-1.20.1/scidatetime/dateutil/tz/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/_common.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/_factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62868 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/tz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/tz.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12937 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tz/win.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/tzwin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.035148 scidatetime-1.20.1/scidatetime/dateutil/zoneinfo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/zoneinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-08 06:23:34.000000 scidatetime-1.20.1/scidatetime/dateutil/zoneinfo/rebuild.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.035148 scidatetime-1.20.1/scidatetime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-08 06:23:43.000000 scidatetime-1.20.1/scidatetime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-08 06:23:43.000000 scidatetime-1.20.1/scidatetime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 06:23:43.000000 scidatetime-1.20.1/scidatetime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 06:23:43.000000 scidatetime-1.20.1/scidatetime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 06:23:43.000000 scidatetime-1.20.1/scidatetime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 06:23:43.000000 scidatetime-1.20.1/scidatetime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 06:23:43.035148 scidatetime-1.20.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-08 06:23:34.000000 scidatetime-1.20.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:23:43.035148 scidatetime-1.20.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-08 06:23:34.000000 scidatetime-1.20.1/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 06:23:34.000000 scidatetime-1.20.1/tests/test_origin_polute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-08 06:23:34.000000 scidatetime-1.20.1/tests/test_timestamp.py
```

### Comparing `scidatetime-1.19.6/LICENSE` & `scidatetime-1.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/PKG-INFO` & `scidatetime-1.20.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scidatetime
-Version: 1.19.6
+Version: 1.20.1
 Summary: scidatetime is python module for DateTime handle.
 Home-page: https://github.com/serfend/scidatetime
 Author: serfend
 Author-email: serfend@foxmail.com
 License: MIT Licence
 Keywords: lib,utils
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scidatetime Version: 1.19.6 Summary: scidatetime is
+Metadata-Version: 2.1 Name: scidatetime Version: 1.20.1 Summary: scidatetime is
 python module for DateTime handle. Home-page: https://github.com/serfend/
 scidatetime Author: serfend Author-email: serfend@foxmail.com License: MIT
 Licence Keywords: lib,utils Platform: any Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Web Environment Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
```

### Comparing `scidatetime-1.19.6/README.md` & `scidatetime-1.20.1/README.md`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/__init__.py` & `scidatetime-1.20.1/scidatetime/MdlDateTime.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
+import typing
 import enum
 from typing import overload
 import datetime
 from time import timezone as time_timezone
 from .dateutil.parser import parser, parserinfo
 _EPOCH = datetime.datetime(1970, 1, 1, tzinfo=datetime.timezone.utc)
 
 
 class DateFormat(enum.Enum):
-    YMD = f'%Y-%m-%d'
-    HMS = f'%H:%M:%S'
+    YMD = '%Y-%m-%d'
+    HMS = '%H:%M:%S'
     DEFAULT = f'{YMD} {HMS}'
     DEFAULT_MIL = f'{DEFAULT}.%f'
     T = f'{YMD}T{HMS}'
     T_MIL = f'{T}.%f'
     UTC = f'{T}%z'
     UTC_MIL = f'{T_MIL}%z'
 
@@ -23,57 +24,88 @@
 datetime_time = datetime.time
 
 TIME_START = 946684800  # 2000-1-1UTC0
 
 
 class DateTime(datetime.datetime):
     Format = DateFormat
+    Default_Format = DateFormat.DEFAULT
+    Default_Format_Converter: typing.Callable = None
 
     @overload
     def __new__(cls, date: datetime.datetime):
         ...
 
     @overload
     def __new__(cls, date: datetime.date):
         ...
 
     @overload
     def __new__(cls, date: str):
         ...
 
     @overload
-    def __new__(cls, year: int, month: int, day: int, hour: int = ..., minute: int = ..., second: int = ..., microsecond: int = ..., tzinfo: datetime.timezone | None = ..., *, fold: int = ...):
+    def __new__(
+            cls, year: int, month: int, day: int,
+            hour: int = ..., minute: int = ..., second: int = ...,
+            microsecond: int = ...,
+            tzinfo: datetime.timezone | None = ..., *, fold: int = ...):
         ...
 
-    def __new__(cls, year: int = ..., month: int = ..., day: int = ..., hour: int = ..., minute: int = ..., second: int = ..., microsecond: int = ..., tzinfo: datetime.timezone | None = ..., *, fold: int = 0):
-        if year == None:
+    def __new__(
+        cls, year: int = ..., month: int = ..., day: int = ...,
+        hour: int = ..., minute: int = ..., second: int = ...,
+        microsecond: int = ...,
+        tzinfo: datetime.timezone | None = ..., *, fold: int = 0,
+    ):
+        if year is None:
             return DateTime('2000-1-1')  # default set timestamp
 
         ii = isinstance
         if year is Ellipsis:
             return DateTime.now()
         if ii(year, float):
             year = int(year)
         if ii(year, int) and month is Ellipsis:
             return DateTime.fromtimestamp(year)
         if ii(year, str):
             x = DateTime.fromstring(year)
             return x
         if ii(year, datetime.datetime):
             x = year
-            return DateTime(x.year, x.month, x.day, x.hour, x.minute, x.second, x.microsecond, x.tzinfo, fold=x.fold)
+            args = (
+                x.year, x.month, x.day,
+                x.hour, x.minute, x.second, x.microsecond,
+                x.tzinfo,
+            )
+            return DateTime(*args, fold=x.fold)
 
         elif ii(year, datetime.date):
             x: datetime.date = year
             return DateTime(x.year, x.month, x.day, 0, 0, 0, 0, None, fold=0)
 
-        if tzinfo is None:  # 无时区时，默认使用当前时区
+        if tzinfo is None or tzinfo is Ellipsis:  # 无时区时，默认使用当前时区
             d = datetime.timedelta(seconds=-time_timezone)
             tzinfo = datetime.timezone(d)
 
+        if year is Ellipsis:
+            year = 2000
+        if month is Ellipsis:
+            month = 1
+        if day is Ellipsis:
+            day = 1
+        if hour is Ellipsis:
+            hour = 0
+        if minute is Ellipsis:
+            minute = 0
+        if second is Ellipsis:
+            second = 0
+        if microsecond is Ellipsis:
+            microsecond = 0
+
         t = super().__new__(cls, year, month, day, hour, minute,
                             second, microsecond, tzinfo, fold=fold)
         return t
 
     @classmethod
     def fromstring(cls, date_str: str, dayfirst=False, yearfirst=False):
         r = parser(info=parserinfo(
@@ -102,29 +134,42 @@
             delta = 0  # self.getDelta()
 
         # 将时间转换为UTC+X
         r = self.timestamp() - delta
         r *= 1e3  # 转换为毫秒
         return int(r)
 
-    def tostring(self, format: str = DateFormat.DEFAULT, tz_info: datetime.timezone = None) -> str:
+    def tostring(
+        self,
+        format: str = None,
+        tz_info: datetime.timezone = None,
+    ) -> str:
         '''
         格式化输出字符串，默认输出UTC+00:00的数值
         @param format:str:输出的格式
         @param tz_info:TzInfo:时区信息
         '''
+        if format is None:
+            format = DateTime.Default_Format
         if isinstance(format, DateFormat):
             format = format.value
-        delta = self.getDelta(tz_info)
-        if delta != 0:
-            x = DateTime.fromtimestamp(self.getTime(delta))
-            return self.strftime(format)
+        if isinstance(DateTime.Default_Format_Converter, typing.Callable):
+            return DateTime.Default_Format_Converter(self)
+
+            # 暂时不考虑时区
+            # delta = self.getDelta(tz_info)
+            # if delta != 0:
+            #     x = DateTime.fromtimestamp(self.getTime(delta))
+            #     return x.strftime(format)
 
         return self.strftime(format)
 
+    def __str__(self) -> str:
+        return self.tostring(None)
+
     def date(self) -> DateTime:
         return DateTime(super().date())
 
     @classmethod
     def now(cls):
         '''
         获取当前DateTime
@@ -153,26 +198,30 @@
         # 将时间转换为UTC+X，不转换，则时间正确
         delta = 0 if tz is None else 0
         t += delta
 
         x = super().fromtimestamp(t, tz)
         return x
 
-    def toRelativeTime(self, target: DateTime = ..., show_full_date_if_over: int = None) -> str:
+    def toRelativeTime(
+        self,
+        target: DateTime = ...,
+        show_full_date_if_over: int = None,
+    ) -> str:
         '''
         转换时间为相对时间
         @param target:DateTime:对比的时间，默认是现在
         @param show_full_date_if_over:int:当相差时间（天数）过多时返回绝对时间
         '''
         if target is Ellipsis:
             target = DateTime(tzinfo=self.tzinfo)
         target = DateTime(target)
         r: timedelta = target - self
         delta_time = r.days + r.seconds / 86400
-        if not show_full_date_if_over is None and delta_time > show_full_date_if_over:
+        if show_full_date_if_over is not None and delta_time > show_full_date_if_over:
             return self.tostring()
         suffix = '后' if delta_time < 0 else '前'
         s_second = 1 / 86400
         v_time = abs(delta_time)
         if v_time < s_second * 60:
             return f'{int(v_time * 86400)}秒{suffix}'
         if v_time < s_second * 3600:
@@ -181,17 +230,17 @@
             return f'{int(v_time * 24)}小时{suffix}'
         if v_time < 14:
             return f'{int(v_time)}天{suffix}'
         if v_time < 30:
             return f'{int(v_time/7)}周{suffix}'
 
         if v_time < 365:
-            v_month = self.month - target.month
-            if v_month < 0:
-                v_month += 12
+            y_month = 12*(target.year - self.year)
+            v_month = y_month + target.month - self.month + 120
+            v_month %= 12
             return f'{v_month}月{suffix}'
 
         v_year = abs(self.year - target.year)
         return f'{v_year}年{suffix}'
 
     def __add__(self, other):
         t = datetime.timedelta
```

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/_common.py` & `scidatetime-1.20.1/scidatetime/dateutil/_common.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/easter.py` & `scidatetime-1.20.1/scidatetime/dateutil/easter.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/parser/__init__.py` & `scidatetime-1.20.1/scidatetime/dateutil/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/parser/__init__.pyi` & `scidatetime-1.20.1/scidatetime/dateutil/parser/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/parser/_parser.py` & `scidatetime-1.20.1/scidatetime/dateutil/parser/_parser.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/parser/isoparser.py` & `scidatetime-1.20.1/scidatetime/dateutil/parser/isoparser.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/parser/isoparser.pyi` & `scidatetime-1.20.1/scidatetime/dateutil/parser/isoparser.pyi`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/relativedelta.py` & `scidatetime-1.20.1/scidatetime/dateutil/relativedelta.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/relativedelta.pyi` & `scidatetime-1.20.1/scidatetime/dateutil/relativedelta.pyi`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/rrule.py` & `scidatetime-1.20.1/scidatetime/dateutil/rrule.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/rrule.pyi` & `scidatetime-1.20.1/scidatetime/dateutil/rrule.pyi`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/tz/_common.py` & `scidatetime-1.20.1/scidatetime/dateutil/tz/_common.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/tz/_common.pyi` & `scidatetime-1.20.1/scidatetime/dateutil/tz/_common.pyi`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/tz/_factories.py` & `scidatetime-1.20.1/scidatetime/dateutil/tz/_factories.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/tz/tz.py` & `scidatetime-1.20.1/scidatetime/dateutil/tz/tz.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/tz/tz.pyi` & `scidatetime-1.20.1/scidatetime/dateutil/tz/tz.pyi`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/tz/win.py` & `scidatetime-1.20.1/scidatetime/dateutil/tz/win.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/utils.py` & `scidatetime-1.20.1/scidatetime/dateutil/utils.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/zoneinfo/__init__.py` & `scidatetime-1.20.1/scidatetime/dateutil/zoneinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime/dateutil/zoneinfo/rebuild.py` & `scidatetime-1.20.1/scidatetime/dateutil/zoneinfo/rebuild.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/scidatetime.egg-info/PKG-INFO` & `scidatetime-1.20.1/scidatetime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scidatetime
-Version: 1.19.6
+Version: 1.20.1
 Summary: scidatetime is python module for DateTime handle.
 Home-page: https://github.com/serfend/scidatetime
 Author: serfend
 Author-email: serfend@foxmail.com
 License: MIT Licence
 Keywords: lib,utils
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scidatetime Version: 1.19.6 Summary: scidatetime is
+Metadata-Version: 2.1 Name: scidatetime Version: 1.20.1 Summary: scidatetime is
 python module for DateTime handle. Home-page: https://github.com/serfend/
 scidatetime Author: serfend Author-email: serfend@foxmail.com License: MIT
 Licence Keywords: lib,utils Platform: any Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Web Environment Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
```

### Comparing `scidatetime-1.19.6/scidatetime.egg-info/SOURCES.txt` & `scidatetime-1.20.1/scidatetime.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE
 README.md
 setup.py
+scidatetime/DateTimeParser.py
+scidatetime/MdlDateTime.py
 scidatetime/__init__.py
 scidatetime/__version__.py
 scidatetime.egg-info/PKG-INFO
 scidatetime.egg-info/SOURCES.txt
 scidatetime.egg-info/dependency_links.txt
 scidatetime.egg-info/not-zip-safe
 scidatetime.egg-info/requires.txt
```

### Comparing `scidatetime-1.19.6/setup.py` & `scidatetime-1.20.1/setup.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/tests/test_date.py` & `scidatetime-1.20.1/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `scidatetime-1.19.6/tests/test_timestamp.py` & `scidatetime-1.20.1/tests/test_timestamp.py`

 * *Files identical despite different names*

