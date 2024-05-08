# Comparing `tmp/PypiInstruments-1.0.3.tar.gz` & `tmp/PypiInstruments-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PypiInstruments-1.0.3.tar", last modified: Mon May  6 10:18:59 2024, max compression
+gzip compressed data, was "PypiInstruments-1.0.4.tar", last modified: Wed May  8 01:31:30 2024, max compression
```

## Comparing `PypiInstruments-1.0.3.tar` & `PypiInstruments-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 10:18:59.880344 PypiInstruments-1.0.3/
--rw-rw-rw-   0        0        0       83 2024-05-06 10:18:59.878969 PypiInstruments-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 10:18:59.869808 PypiInstruments-1.0.3/PypiInstruments.egg-info/
--rw-rw-rw-   0        0        0       83 2024-05-06 10:18:59.000000 PypiInstruments-1.0.3/PypiInstruments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      436 2024-05-06 10:18:59.000000 PypiInstruments-1.0.3/PypiInstruments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 10:18:59.000000 PypiInstruments-1.0.3/PypiInstruments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 10:18:59.000000 PypiInstruments-1.0.3/PypiInstruments.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2024-05-06 10:18:59.000000 PypiInstruments-1.0.3/PypiInstruments.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 10:18:59.874185 PypiInstruments-1.0.3/instruments/
--rw-rw-rw-   0        0        0     2132 2024-04-29 07:50:25.000000 PypiInstruments-1.0.3/instruments/DP821A.py
--rw-rw-rw-   0        0        0     3827 2024-05-06 09:48:58.000000 PypiInstruments-1.0.3/instruments/Multimemter.py
--rw-rw-rw-   0        0        0      979 2024-04-30 09:41:34.000000 PypiInstruments-1.0.3/instruments/SMU_Examples.py
--rw-rw-rw-   0        0        0      201 2024-05-06 10:15:57.000000 PypiInstruments-1.0.3/instruments/__init__.py
--rw-rw-rw-   0        0        0      297 2024-04-28 10:28:19.000000 PypiInstruments-1.0.3/instruments/device_scan.py
--rw-rw-rw-   0        0        0      740 2024-04-29 02:13:11.000000 PypiInstruments-1.0.3/instruments/instruments_name.py
--rw-rw-rw-   0        0        0    11510 2024-05-06 09:48:58.000000 PypiInstruments-1.0.3/instruments/smu_keithley_2450.py
-drwxrwxrwx   0        0        0        0 2024-05-06 10:18:59.878969 PypiInstruments-1.0.3/one/
--rw-rw-rw-   0        0        0        0 2024-05-06 09:46:19.000000 PypiInstruments-1.0.3/one/__init__.py
--rw-rw-rw-   0        0        0      104 2024-05-04 13:35:48.000000 PypiInstruments-1.0.3/one/hello.py
--rw-rw-rw-   0        0        0        0 2024-05-04 13:27:19.000000 PypiInstruments-1.0.3/one/main.py
--rw-rw-rw-   0        0        0       42 2024-05-06 10:18:59.880344 PypiInstruments-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      273 2024-05-06 10:18:56.000000 PypiInstruments-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 01:31:30.620801 PypiInstruments-1.0.4/
+-rw-rw-rw-   0        0        0       83 2024-05-08 01:31:30.620801 PypiInstruments-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-08 01:31:30.575800 PypiInstruments-1.0.4/PypiInstruments.egg-info/
+-rw-rw-rw-   0        0        0       83 2024-05-08 01:31:30.000000 PypiInstruments-1.0.4/PypiInstruments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2024-05-08 01:31:30.000000 PypiInstruments-1.0.4/PypiInstruments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 01:31:30.000000 PypiInstruments-1.0.4/PypiInstruments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 10:18:59.000000 PypiInstruments-1.0.4/PypiInstruments.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2024-05-08 01:31:30.000000 PypiInstruments-1.0.4/PypiInstruments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 01:31:30.609801 PypiInstruments-1.0.4/instruments/
+-rw-rw-rw-   0        0        0     2132 2024-04-29 07:50:25.000000 PypiInstruments-1.0.4/instruments/DP821A.py
+-rw-rw-rw-   0        0        0     3827 2024-05-06 09:48:58.000000 PypiInstruments-1.0.4/instruments/Multimemter.py
+-rw-rw-rw-   0        0        0      975 2024-05-08 01:31:27.000000 PypiInstruments-1.0.4/instruments/SMU_Examples.py
+-rw-rw-rw-   0        0        0        2 2024-05-08 01:30:53.000000 PypiInstruments-1.0.4/instruments/__init__.py
+-rw-rw-rw-   0        0        0      297 2024-04-28 10:28:19.000000 PypiInstruments-1.0.4/instruments/device_scan.py
+-rw-rw-rw-   0        0        0      740 2024-04-29 02:13:11.000000 PypiInstruments-1.0.4/instruments/instruments_name.py
+-rw-rw-rw-   0        0        0    11510 2024-05-06 09:48:58.000000 PypiInstruments-1.0.4/instruments/smu_keithley_2450.py
+drwxrwxrwx   0        0        0        0 2024-05-08 01:31:30.619799 PypiInstruments-1.0.4/one/
+-rw-rw-rw-   0        0        0        0 2024-05-06 09:46:19.000000 PypiInstruments-1.0.4/one/__init__.py
+-rw-rw-rw-   0        0        0      104 2024-05-04 13:35:48.000000 PypiInstruments-1.0.4/one/hello.py
+-rw-rw-rw-   0        0        0        0 2024-05-04 13:27:19.000000 PypiInstruments-1.0.4/one/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 01:31:30.620801 PypiInstruments-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      273 2024-05-08 01:31:27.000000 PypiInstruments-1.0.4/setup.py
```

### Comparing `PypiInstruments-1.0.3/instruments/DP821A.py` & `PypiInstruments-1.0.4/instruments/DP821A.py`

 * *Files identical despite different names*

### Comparing `PypiInstruments-1.0.3/instruments/Multimemter.py` & `PypiInstruments-1.0.4/instruments/Multimemter.py`

 * *Files identical despite different names*

### Comparing `PypiInstruments-1.0.3/instruments/SMU_Examples.py` & `PypiInstruments-1.0.4/instruments/SMU_Examples.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import instruments_name
 
 """使用SMU测试的例子"""
 from instruments_name import *
 
 smuid = smu_2460_id
 
-smu = SmuKeithley2450(pyvisa.ResourceManager(), smuid)
+smu = SmuKeithley(pyvisa.ResourceManager(), smuid)
 
 # smu.smu2450_reset()
 
 # smu.sum2450_force_volt_sens_cur_init(3.3,1,5,1,0.01)
 
 # smu.smu2450_set_volt_output(5)
```

### Comparing `PypiInstruments-1.0.3/instruments/instruments_name.py` & `PypiInstruments-1.0.4/instruments/instruments_name.py`

 * *Files identical despite different names*

### Comparing `PypiInstruments-1.0.3/instruments/smu_keithley_2450.py` & `PypiInstruments-1.0.4/instruments/smu_keithley_2450.py`

 * *Files identical despite different names*

