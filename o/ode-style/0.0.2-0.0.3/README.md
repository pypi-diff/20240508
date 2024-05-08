# Comparing `tmp/ode-style-0.0.2.tar.gz` & `tmp/ode_style-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ode-style-0.0.2.tar", last modified: Tue Apr  2 16:34:01 2024, max compression
+gzip compressed data, was "ode_style-0.0.3.tar", last modified: Wed May  8 10:55:27 2024, max compression
```

## Comparing `ode-style-0.0.2.tar` & `ode_style-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:34:01.880241 ode-style-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 16:34:01.880241 ode-style-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:33:49.000000 ode-style-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:34:01.880241 ode-style-0.0.2/ode/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/authentication_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/base_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/callback_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/chained_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/composite_job_disposable.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/error_output.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/guard_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/http_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/internet_connection_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/sequence_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/use_case_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/use_case_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/use_case_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/value_out_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:34:01.880241 ode-style-0.0.2/ode_style.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 16:34:01.000000 ode-style-0.0.2/ode_style.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-02 16:34:01.000000 ode-style-0.0.2/ode_style.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:34:01.000000 ode-style-0.0.2/ode_style.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 16:34:01.000000 ode-style-0.0.2/ode_style.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 16:34:01.880241 ode-style-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-02 16:33:49.000000 ode-style-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:55:27.308650 ode_style-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 10:55:27.308650 ode_style-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 10:55:23.000000 ode_style-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:55:27.304650 ode_style-0.0.3/ode/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/authentication_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/base_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/callback_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/chained_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/composite_job_disposable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/error_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/guard_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/http_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/internet_connection_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/sequence_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/use_case_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/use_case_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/use_case_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-08 10:55:23.000000 ode_style-0.0.3/ode/value_out_put.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:55:27.304650 ode_style-0.0.3/ode_style.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 10:55:27.000000 ode_style-0.0.3/ode_style.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-08 10:55:27.000000 ode_style-0.0.3/ode_style.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:55:27.000000 ode_style-0.0.3/ode_style.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 10:55:27.000000 ode_style-0.0.3/ode_style.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 10:55:27.308650 ode_style-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-08 10:55:23.000000 ode_style-0.0.3/setup.py
```

### Comparing `ode-style-0.0.2/ode/base_controller.py` & `ode_style-0.0.3/ode/base_controller.py`

 * *Files identical despite different names*

### Comparing `ode-style-0.0.2/ode/callback_decorator.py` & `ode_style-0.0.3/ode/callback_decorator.py`

 * *Files identical despite different names*

### Comparing `ode-style-0.0.2/ode/chained_use_case.py` & `ode_style-0.0.3/ode/chained_use_case.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import TypeVar
 from ode.use_case import UseCase
-from output import Output
-from error_output import ErrorOutput
+from ode.output import Output
+from ode.error_output import ErrorOutput
 
 P = TypeVar('P')
 R = TypeVar('R')
 T = TypeVar('T')
 
 class ChainedUseCase(UseCase[P, T]):
     def __init__(self, first: UseCase[P, R], second: UseCase[R, T]):
```

### Comparing `ode-style-0.0.2/ode/composite_job_disposable.py` & `ode_style-0.0.3/ode/composite_job_disposable.py`

 * *Files identical despite different names*

### Comparing `ode-style-0.0.2/ode/sequence_use_case.py` & `ode_style-0.0.3/ode/sequence_use_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TypeVar, List, Optional
 from ode.use_case import UseCase
-from output import Output
-from value_out_put import ValueOutput
-from use_case_unit import UseCaseUnit
+from ode.output import Output
+from ode.value_out_put import ValueOutput
+from ode.use_case_unit import UseCaseUnit
 
 P = TypeVar('P')
 R = TypeVar('R')
 T = TypeVar('T')
 
 class SequenceUseCase(UseCase[None, List[Output[T]]]):
     def __init__(self, units: List[UseCaseUnit[P, T]]):
```

### Comparing `ode-style-0.0.2/ode/use_case.py` & `ode_style-0.0.3/ode/use_case.py`

 * *Files identical despite different names*

### Comparing `ode-style-0.0.2/ode/use_case_decorator.py` & `ode_style-0.0.3/ode/use_case_decorator.py`

 * *Files identical despite different names*

### Comparing `ode-style-0.0.2/ode/use_case_dispatcher.py` & `ode_style-0.0.3/ode/use_case_dispatcher.py`

 * *Files identical despite different names*

### Comparing `ode-style-0.0.2/ode/use_case_unit.py` & `ode_style-0.0.3/ode/use_case_unit.py`

 * *Files identical despite different names*

### Comparing `ode-style-0.0.2/ode_style.egg-info/SOURCES.txt` & `ode_style-0.0.3/ode_style.egg-info/SOURCES.txt`

 * *Files identical despite different names*

