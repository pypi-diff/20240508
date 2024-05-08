# Comparing `tmp/elfws-0.9.0.tar.gz` & `tmp/elfws-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/elfws-0.9.0.tar", last modified: Sun Sep 10 16:01:21 2023, max compression
+gzip compressed data, was "dist/elfws-0.9.1.tar", last modified: Sun Oct  8 02:19:57 2023, max compression
```

## Comparing `elfws-0.9.0.tar` & `elfws-0.9.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-09-10 16:01:21.380000 elfws-0.9.0/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       31 2022-08-09 20:37:16.000000 elfws-0.9.0/MANIFEST.in
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)    11055 2023-09-10 16:01:21.380000 elfws-0.9.0/PKG-INFO
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     8088 2022-08-09 20:37:16.000000 elfws-0.9.0/README.rst
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-09-10 16:01:21.380000 elfws-0.9.0/elfws/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2022-08-09 20:37:16.000000 elfws-0.9.0/elfws/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      749 2022-08-09 20:37:16.000000 elfws-0.9.0/elfws/__main__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2518 2022-08-10 01:29:46.000000 elfws-0.9.0/elfws/cmd_line_args.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     8769 2023-03-11 14:10:10.000000 elfws-0.9.0/elfws/display.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4240 2023-04-15 20:38:59.000000 elfws-0.9.0/elfws/junit.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-09-10 16:01:21.380000 elfws-0.9.0/elfws/report/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2022-08-10 01:29:46.000000 elfws-0.9.0/elfws/report/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2469 2023-07-14 21:12:19.000000 elfws-0.9.0/elfws/report/junit.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-09-10 16:01:21.380000 elfws-0.9.0/elfws/subcommand/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      106 2022-08-09 20:37:16.000000 elfws-0.9.0/elfws/subcommand/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1394 2022-08-09 20:37:16.000000 elfws-0.9.0/elfws/subcommand/create.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2950 2022-08-10 01:29:46.000000 elfws-0.9.0/elfws/subcommand/report.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      525 2022-08-10 01:29:46.000000 elfws-0.9.0/elfws/subcommand/show.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1007 2022-08-09 20:37:16.000000 elfws-0.9.0/elfws/subcommand/suppress.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      143 2022-08-09 20:37:16.000000 elfws-0.9.0/elfws/subcommand/version.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1187 2023-07-14 21:12:19.000000 elfws-0.9.0/elfws/suppression.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1068 2022-08-09 20:37:16.000000 elfws-0.9.0/elfws/suppression_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     8819 2023-09-10 15:58:42.000000 elfws-0.9.0/elfws/utils.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-09-10 16:01:21.380000 elfws-0.9.0/elfws/vendor/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2022-08-09 20:37:16.000000 elfws-0.9.0/elfws/vendor/__init__.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-09-10 16:01:21.380000 elfws-0.9.0/elfws/vendor/mentor_graphics/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2022-08-09 20:37:16.000000 elfws-0.9.0/elfws/vendor/mentor_graphics/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1165 2022-08-09 22:01:43.000000 elfws-0.9.0/elfws/vendor/mentor_graphics/precision.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3732 2023-09-10 15:58:42.000000 elfws-0.9.0/elfws/vendor/mentor_graphics/questa_cdc__cdc_detail_rpt.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2159 2023-09-10 15:58:42.000000 elfws-0.9.0/elfws/vendor/mentor_graphics/questa_cdc__cdc_run_log.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1382 2023-03-11 14:33:31.000000 elfws-0.9.0/elfws/vendor/mentor_graphics/questa_lint.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1084 2023-09-10 15:58:42.000000 elfws-0.9.0/elfws/vendor/mentor_graphics/utils.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-09-10 16:01:21.380000 elfws-0.9.0/elfws/vendor/microsemi/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       23 2022-08-09 20:37:16.000000 elfws-0.9.0/elfws/vendor/microsemi/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1463 2022-08-09 20:37:16.000000 elfws-0.9.0/elfws/vendor/microsemi/designer.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      306 2023-09-10 15:58:42.000000 elfws-0.9.0/elfws/vendor/utils.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-09-10 16:01:21.380000 elfws-0.9.0/elfws/vendor/xilinx/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2022-08-09 20:37:16.000000 elfws-0.9.0/elfws/vendor/xilinx/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1336 2022-08-09 20:37:16.000000 elfws-0.9.0/elfws/vendor/xilinx/vivado.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       18 2023-09-10 15:59:43.000000 elfws-0.9.0/elfws/version.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1138 2023-03-12 16:38:14.000000 elfws-0.9.0/elfws/warning.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1494 2022-08-09 20:37:16.000000 elfws-0.9.0/elfws/warning_list.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-09-10 16:01:21.380000 elfws-0.9.0/elfws.egg-info/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)    11055 2023-09-10 16:01:21.000000 elfws-0.9.0/elfws.egg-info/PKG-INFO
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1125 2023-09-10 16:01:21.000000 elfws-0.9.0/elfws.egg-info/SOURCES.txt
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        1 2023-09-10 16:01:21.000000 elfws-0.9.0/elfws.egg-info/dependency_links.txt
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       47 2023-09-10 16:01:21.000000 elfws-0.9.0/elfws.egg-info/entry_points.txt
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        1 2022-08-10 01:34:19.000000 elfws-0.9.0/elfws.egg-info/not-zip-safe
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        7 2023-09-10 16:01:21.000000 elfws-0.9.0/elfws.egg-info/requires.txt
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       12 2023-09-10 16:01:21.000000 elfws-0.9.0/elfws.egg-info/top_level.txt
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      147 2023-09-10 16:01:21.380000 elfws-0.9.0/setup.cfg
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1310 2022-08-09 20:37:16.000000 elfws-0.9.0/setup.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-10-08 02:19:57.060000 elfws-0.9.1/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       31 2022-08-09 20:37:16.000000 elfws-0.9.1/MANIFEST.in
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)    11055 2023-10-08 02:19:57.060000 elfws-0.9.1/PKG-INFO
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     8088 2022-08-09 20:37:16.000000 elfws-0.9.1/README.rst
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-10-08 02:19:57.050000 elfws-0.9.1/elfws/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2022-08-09 20:37:16.000000 elfws-0.9.1/elfws/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      749 2022-08-09 20:37:16.000000 elfws-0.9.1/elfws/__main__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2518 2022-08-10 01:29:46.000000 elfws-0.9.1/elfws/cmd_line_args.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     8769 2023-03-11 14:10:10.000000 elfws-0.9.1/elfws/display.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4240 2023-04-15 20:38:59.000000 elfws-0.9.1/elfws/junit.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-10-08 02:19:57.050000 elfws-0.9.1/elfws/report/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2022-08-10 01:29:46.000000 elfws-0.9.1/elfws/report/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2469 2023-07-14 21:12:19.000000 elfws-0.9.1/elfws/report/junit.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-10-08 02:19:57.050000 elfws-0.9.1/elfws/subcommand/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      106 2022-08-09 20:37:16.000000 elfws-0.9.1/elfws/subcommand/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1394 2022-08-09 20:37:16.000000 elfws-0.9.1/elfws/subcommand/create.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2950 2022-08-10 01:29:46.000000 elfws-0.9.1/elfws/subcommand/report.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      525 2022-08-10 01:29:46.000000 elfws-0.9.1/elfws/subcommand/show.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1007 2022-08-09 20:37:16.000000 elfws-0.9.1/elfws/subcommand/suppress.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      143 2022-08-09 20:37:16.000000 elfws-0.9.1/elfws/subcommand/version.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1187 2023-07-14 21:12:19.000000 elfws-0.9.1/elfws/suppression.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1068 2022-08-09 20:37:16.000000 elfws-0.9.1/elfws/suppression_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     8819 2023-09-10 15:58:42.000000 elfws-0.9.1/elfws/utils.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-10-08 02:19:57.050000 elfws-0.9.1/elfws/vendor/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2022-08-09 20:37:16.000000 elfws-0.9.1/elfws/vendor/__init__.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-10-08 02:19:57.060000 elfws-0.9.1/elfws/vendor/mentor_graphics/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2022-08-09 20:37:16.000000 elfws-0.9.1/elfws/vendor/mentor_graphics/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1165 2022-08-09 22:01:43.000000 elfws-0.9.1/elfws/vendor/mentor_graphics/precision.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3732 2023-09-10 15:58:42.000000 elfws-0.9.1/elfws/vendor/mentor_graphics/questa_cdc__cdc_detail_rpt.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2184 2023-10-02 18:50:29.000000 elfws-0.9.1/elfws/vendor/mentor_graphics/questa_cdc__cdc_run_log.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1382 2023-03-11 14:33:31.000000 elfws-0.9.1/elfws/vendor/mentor_graphics/questa_lint.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1084 2023-09-10 15:58:42.000000 elfws-0.9.1/elfws/vendor/mentor_graphics/utils.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-10-08 02:19:57.060000 elfws-0.9.1/elfws/vendor/microsemi/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       23 2022-08-09 20:37:16.000000 elfws-0.9.1/elfws/vendor/microsemi/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1463 2022-08-09 20:37:16.000000 elfws-0.9.1/elfws/vendor/microsemi/designer.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      306 2023-09-10 15:58:42.000000 elfws-0.9.1/elfws/vendor/utils.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-10-08 02:19:57.060000 elfws-0.9.1/elfws/vendor/xilinx/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2022-08-09 20:37:16.000000 elfws-0.9.1/elfws/vendor/xilinx/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1336 2022-08-09 20:37:16.000000 elfws-0.9.1/elfws/vendor/xilinx/vivado.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       18 2023-10-02 18:54:55.000000 elfws-0.9.1/elfws/version.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1138 2023-03-12 16:38:14.000000 elfws-0.9.1/elfws/warning.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1494 2022-08-09 20:37:16.000000 elfws-0.9.1/elfws/warning_list.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2023-10-08 02:19:57.050000 elfws-0.9.1/elfws.egg-info/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)    11055 2023-10-08 02:19:57.000000 elfws-0.9.1/elfws.egg-info/PKG-INFO
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1125 2023-10-08 02:19:57.000000 elfws-0.9.1/elfws.egg-info/SOURCES.txt
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        1 2023-10-08 02:19:57.000000 elfws-0.9.1/elfws.egg-info/dependency_links.txt
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       47 2023-10-08 02:19:57.000000 elfws-0.9.1/elfws.egg-info/entry_points.txt
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        1 2022-08-10 01:34:19.000000 elfws-0.9.1/elfws.egg-info/not-zip-safe
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        7 2023-10-08 02:19:57.000000 elfws-0.9.1/elfws.egg-info/requires.txt
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       12 2023-10-08 02:19:57.000000 elfws-0.9.1/elfws.egg-info/top_level.txt
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      147 2023-10-08 02:19:57.060000 elfws-0.9.1/setup.cfg
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1310 2022-08-09 20:37:16.000000 elfws-0.9.1/setup.py
```

### Comparing `elfws-0.9.0/PKG-INFO` & `elfws-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: elfws
-Version: 0.9.0
+Version: 0.9.1
 Summary: EDA Log File Warning Suppressor
 Home-page: https://github.com/jeremiah-c-leary/eda-log-file-warning-suppressor
 Author: Jeremiah C Leary
 Author-email: jeremiah.c.leary@gmail.com
 License: GNU General Public License
 Download-URL: https://github.com/jeremiah-c-leary/eda-log-file-warning-suppressor
 Description: EDA Log File Warning Suppressor (ELFWS)
```

### Comparing `elfws-0.9.0/README.rst` & `elfws-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/__main__.py` & `elfws-0.9.1/elfws/__main__.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/cmd_line_args.py` & `elfws-0.9.1/elfws/cmd_line_args.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/display.py` & `elfws-0.9.1/elfws/display.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/junit.py` & `elfws-0.9.1/elfws/junit.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/report/junit.py` & `elfws-0.9.1/elfws/report/junit.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/subcommand/create.py` & `elfws-0.9.1/elfws/subcommand/create.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/subcommand/report.py` & `elfws-0.9.1/elfws/subcommand/report.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/subcommand/show.py` & `elfws-0.9.1/elfws/subcommand/show.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/subcommand/suppress.py` & `elfws-0.9.1/elfws/subcommand/suppress.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/suppression.py` & `elfws-0.9.1/elfws/suppression.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/suppression_list.py` & `elfws-0.9.1/elfws/suppression_list.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/utils.py` & `elfws-0.9.1/elfws/utils.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/vendor/mentor_graphics/precision.py` & `elfws-0.9.1/elfws/vendor/mentor_graphics/precision.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/vendor/mentor_graphics/questa_cdc__cdc_detail_rpt.py` & `elfws-0.9.1/elfws/vendor/mentor_graphics/questa_cdc__cdc_detail_rpt.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/vendor/mentor_graphics/questa_cdc__cdc_run_log.py` & `elfws-0.9.1/elfws/vendor/mentor_graphics/questa_cdc__cdc_run_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     return 'questa_cdc'
 
 
 def is_logfile(lFile):
     fToolFound = False
     for iLineNumber, sLine in enumerate(lFile):
         if fToolFound:
-           if sLine.startswith('log created'):
+           if sLine.lstrip().startswith('-tool cdc'):
                return True
-        if sLine.startswith('Command : cdc run'):
+        if sLine.startswith('# Questa Static Verification System'):
             fToolFound = True
         if iLineNumber == 20:
             break
     return False
 
 
 def extract_warnings(lFile):
```

### Comparing `elfws-0.9.0/elfws/vendor/mentor_graphics/questa_lint.py` & `elfws-0.9.1/elfws/vendor/mentor_graphics/questa_lint.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/vendor/mentor_graphics/utils.py` & `elfws-0.9.1/elfws/vendor/mentor_graphics/utils.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/vendor/microsemi/designer.py` & `elfws-0.9.1/elfws/vendor/microsemi/designer.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/vendor/xilinx/vivado.py` & `elfws-0.9.1/elfws/vendor/xilinx/vivado.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/warning.py` & `elfws-0.9.1/elfws/warning.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws/warning_list.py` & `elfws-0.9.1/elfws/warning_list.py`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/elfws.egg-info/PKG-INFO` & `elfws-0.9.1/elfws.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: elfws
-Version: 0.9.0
+Version: 0.9.1
 Summary: EDA Log File Warning Suppressor
 Home-page: https://github.com/jeremiah-c-leary/eda-log-file-warning-suppressor
 Author: Jeremiah C Leary
 Author-email: jeremiah.c.leary@gmail.com
 License: GNU General Public License
 Download-URL: https://github.com/jeremiah-c-leary/eda-log-file-warning-suppressor
 Description: EDA Log File Warning Suppressor (ELFWS)
```

### Comparing `elfws-0.9.0/elfws.egg-info/SOURCES.txt` & `elfws-0.9.1/elfws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elfws-0.9.0/setup.py` & `elfws-0.9.1/setup.py`

 * *Files identical despite different names*

