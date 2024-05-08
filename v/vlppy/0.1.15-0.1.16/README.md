# Comparing `tmp/vlppy-0.1.15.tar.gz` & `tmp/vlppy-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\vlppy_lib\dist\.tmp-n05743yy\vlppy-0.1.15.tar", last modified: Tue Mar 19 06:39:50 2024, max compression
+gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\vlppy_lib\dist\.tmp-mr97ik0g\vlppy-0.1.16.tar", last modified: Wed May  8 10:21:57 2024, max compression
```

## Comparing `vlppy-0.1.15.tar` & `vlppy-0.1.16.tar`

### file list

```diff
@@ -1,73 +1,69 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 06:39:50.968193 vlppy-0.1.15/
--rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 vlppy-0.1.15/LICENSE
--rw-rw-rw-   0        0        0      294 2023-06-04 07:31:04.000000 vlppy-0.1.15/MANIFEST.in
--rw-rw-rw-   0        0        0     5387 2024-03-19 06:39:50.966192 vlppy-0.1.15/PKG-INFO
--rw-rw-rw-   0        0        0     3552 2024-01-10 02:28:01.000000 vlppy-0.1.15/README.md
--rw-rw-rw-   0        0        0      634 2024-03-16 13:49:07.000000 vlppy-0.1.15/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-19 06:39:50.968193 vlppy-0.1.15/setup.cfg
--rw-rw-rw-   0        0        0      931 2024-03-16 13:49:11.000000 vlppy-0.1.15/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 06:39:50.849374 vlppy-0.1.15/vlppy/
--rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 vlppy-0.1.15/vlppy/LICENSE.txt
--rw-rw-rw-   0        0        0      283 2024-03-08 09:08:54.000000 vlppy-0.1.15/vlppy/__init__.py
--rw-rw-rw-   0        0        0      174 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/__init__.pyi
-drwxrwxrwx   0        0        0        0 2024-03-19 06:39:50.871180 vlppy-0.1.15/vlppy/demo/
--rw-rw-rw-   0        0        0     2764 2023-12-27 05:23:12.000000 vlppy-0.1.15/vlppy/demo/README.md
--rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 vlppy-0.1.15/vlppy/demo/__init__.py
--rw-rw-rw-   0        0        0      101 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/demo/__init__.pyi
--rw-rw-rw-   0        0        0     1620 2023-12-27 06:45:16.000000 vlppy-0.1.15/vlppy/demo/demo_filter.py
--rw-rw-rw-   0        0        0       80 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/demo/demo_filter.pyi
--rw-rw-rw-   0        0        0     2759 2023-12-27 06:49:09.000000 vlppy-0.1.15/vlppy/demo/demo_main.py
--rw-rw-rw-   0        0        0      287 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/demo/demo_main.pyi
--rw-rw-rw-   0        0        0     2824 2023-12-27 06:15:32.000000 vlppy-0.1.15/vlppy/demo/vlp_model.py
--rw-rw-rw-   0        0        0      385 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/demo/vlp_model.pyi
-drwxrwxrwx   0        0        0        0 2024-03-19 06:39:50.875064 vlppy-0.1.15/vlppy/error/
--rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 vlppy-0.1.15/vlppy/error/__init__.py
--rw-rw-rw-   0        0        0       22 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/error/__init__.pyi
--rw-rw-rw-   0        0        0     1629 2024-01-04 13:02:39.000000 vlppy-0.1.15/vlppy/error/error.py
--rw-rw-rw-   0        0        0      437 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/error/error.pyi
--rw-rw-rw-   0        0        0      129 2024-03-16 13:49:01.000000 vlppy-0.1.15/vlppy/info.py
--rw-rw-rw-   0        0        0       62 2024-03-19 06:38:21.000000 vlppy-0.1.15/vlppy/info.pyi
-drwxrwxrwx   0        0        0        0 2024-03-19 06:39:50.887730 vlppy-0.1.15/vlppy/io/
--rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 vlppy-0.1.15/vlppy/io/__init__.py
--rw-rw-rw-   0        0        0       26 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/io/__init__.pyi
--rw-rw-rw-   0        0        0     4481 2023-12-27 06:05:58.000000 vlppy-0.1.15/vlppy/io/io.py
--rw-rw-rw-   0        0        0     1644 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/io/io.pyi
-drwxrwxrwx   0        0        0        0 2024-03-19 06:39:50.916510 vlppy-0.1.15/vlppy/model/
--rw-rw-rw-   0        0        0       88 2023-11-22 05:37:05.000000 vlppy-0.1.15/vlppy/model/__init__.py
--rw-rw-rw-   0        0        0      116 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/model/__init__.pyi
--rw-rw-rw-   0        0        0     7130 2024-02-05 07:35:21.000000 vlppy-0.1.15/vlppy/model/led.py
--rw-rw-rw-   0        0        0     1035 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/model/led.pyi
--rw-rw-rw-   0        0        0    21169 2024-03-19 06:37:04.000000 vlppy-0.1.15/vlppy/model/pd.py
--rw-rw-rw-   0        0        0     1677 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/model/pd.pyi
--rw-rw-rw-   0        0        0    27608 2024-03-16 13:55:04.000000 vlppy-0.1.15/vlppy/model/pd2.py
--rw-rw-rw-   0        0        0     2279 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/model/pd2.pyi
--rw-rw-rw-   0        0        0    24921 2024-03-08 09:05:12.000000 vlppy-0.1.15/vlppy/model/room.py
--rw-rw-rw-   0        0        0     1887 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/model/room.pyi
-drwxrwxrwx   0        0        0        0 2024-03-19 06:39:50.921234 vlppy-0.1.15/vlppy/setting/
--rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 vlppy-0.1.15/vlppy/setting/__init__.py
--rw-rw-rw-   0        0        0       48 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/setting/__init__.pyi
--rw-rw-rw-   0        0        0     2894 2023-12-27 05:28:09.000000 vlppy-0.1.15/vlppy/setting/json_setting.py
--rw-rw-rw-   0        0        0      354 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/setting/json_setting.pyi
--rw-rw-rw-   0        0        0     1797 2023-12-27 05:57:23.000000 vlppy-0.1.15/vlppy/setting/settings.json
-drwxrwxrwx   0        0        0        0 2024-03-19 06:39:50.950115 vlppy-0.1.15/vlppy/signal/
--rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 vlppy-0.1.15/vlppy/signal/__init__.py
--rw-rw-rw-   0        0        0       44 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/signal/__init__.pyi
--rw-rw-rw-   0        0        0     8842 2023-12-27 05:29:53.000000 vlppy-0.1.15/vlppy/signal/filter.py
--rw-rw-rw-   0        0        0     1342 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/signal/filter.pyi
--rw-rw-rw-   0        0        0     3821 2023-12-27 05:30:44.000000 vlppy-0.1.15/vlppy/signal/plot.py
--rw-rw-rw-   0        0        0      440 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/signal/plot.pyi
-drwxrwxrwx   0        0        0        0 2024-03-19 06:39:50.954010 vlppy-0.1.15/vlppy/tools/
--rw-rw-rw-   0        0        0       26 2023-04-18 03:21:34.000000 vlppy-0.1.15/vlppy/tools/__init__.py
--rw-rw-rw-   0        0        0       26 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/tools/__init__.pyi
--rw-rw-rw-   0        0        0      307 2023-12-27 05:30:49.000000 vlppy-0.1.15/vlppy/tools/decorator.py
--rw-rw-rw-   0        0        0       22 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/tools/decorator.pyi
-drwxrwxrwx   0        0        0        0 2024-03-19 06:39:50.963528 vlppy-0.1.15/vlppy/vis/
--rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 vlppy-0.1.15/vlppy/vis/__init__.py
--rw-rw-rw-   0        0        0       20 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/vis/__init__.pyi
--rw-rw-rw-   0        0        0     3574 2024-01-04 13:12:34.000000 vlppy-0.1.15/vlppy/vis/vis.py
--rw-rw-rw-   0        0        0      458 2024-03-19 06:37:38.000000 vlppy-0.1.15/vlppy/vis/vis.pyi
-drwxrwxrwx   0        0        0        0 2024-03-19 06:39:50.965192 vlppy-0.1.15/vlppy.egg-info/
--rw-rw-rw-   0        0        0     5387 2024-03-19 06:39:50.000000 vlppy-0.1.15/vlppy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2024-03-19 06:39:50.000000 vlppy-0.1.15/vlppy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 06:39:50.000000 vlppy-0.1.15/vlppy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-19 06:39:50.000000 vlppy-0.1.15/vlppy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 10:21:57.263789 vlppy-0.1.16/
+-rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 vlppy-0.1.16/LICENSE
+-rw-rw-rw-   0        0        0      294 2023-06-04 07:31:04.000000 vlppy-0.1.16/MANIFEST.in
+-rw-rw-rw-   0        0        0     5387 2024-05-08 10:21:57.263789 vlppy-0.1.16/PKG-INFO
+-rw-rw-rw-   0        0        0     3552 2024-01-10 02:28:01.000000 vlppy-0.1.16/README.md
+-rw-rw-rw-   0        0        0      634 2024-03-25 11:36:28.000000 vlppy-0.1.16/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 10:21:57.263789 vlppy-0.1.16/setup.cfg
+-rw-rw-rw-   0        0        0      931 2024-03-25 11:36:22.000000 vlppy-0.1.16/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:21:57.147309 vlppy-0.1.16/vlppy/
+-rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 vlppy-0.1.16/vlppy/LICENSE.txt
+-rw-rw-rw-   0        0        0      283 2024-03-08 09:08:54.000000 vlppy-0.1.16/vlppy/__init__.py
+-rw-rw-rw-   0        0        0      174 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/__init__.pyi
+drwxrwxrwx   0        0        0        0 2024-05-08 10:21:57.175496 vlppy-0.1.16/vlppy/demo/
+-rw-rw-rw-   0        0        0     2764 2023-12-27 05:23:12.000000 vlppy-0.1.16/vlppy/demo/README.md
+-rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 vlppy-0.1.16/vlppy/demo/__init__.py
+-rw-rw-rw-   0        0        0     1620 2023-12-27 06:45:16.000000 vlppy-0.1.16/vlppy/demo/demo_filter.py
+-rw-rw-rw-   0        0        0     2759 2023-12-27 06:49:09.000000 vlppy-0.1.16/vlppy/demo/demo_main.py
+-rw-rw-rw-   0        0        0     2824 2023-12-27 06:15:32.000000 vlppy-0.1.16/vlppy/demo/vlp_model.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:21:57.180609 vlppy-0.1.16/vlppy/error/
+-rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 vlppy-0.1.16/vlppy/error/__init__.py
+-rw-rw-rw-   0        0        0       22 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/error/__init__.pyi
+-rw-rw-rw-   0        0        0     1629 2024-01-04 13:02:39.000000 vlppy-0.1.16/vlppy/error/error.py
+-rw-rw-rw-   0        0        0      437 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/error/error.pyi
+-rw-rw-rw-   0        0        0      129 2024-03-25 11:36:48.000000 vlppy-0.1.16/vlppy/info.py
+-rw-rw-rw-   0        0        0       66 2024-04-13 04:05:43.000000 vlppy-0.1.16/vlppy/info.pyi
+drwxrwxrwx   0        0        0        0 2024-05-08 10:21:57.192253 vlppy-0.1.16/vlppy/io/
+-rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 vlppy-0.1.16/vlppy/io/__init__.py
+-rw-rw-rw-   0        0        0       26 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/io/__init__.pyi
+-rw-rw-rw-   0        0        0     4485 2024-04-28 05:09:15.000000 vlppy-0.1.16/vlppy/io/io.py
+-rw-rw-rw-   0        0        0     1644 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/io/io.pyi
+drwxrwxrwx   0        0        0        0 2024-05-08 10:21:57.211175 vlppy-0.1.16/vlppy/model/
+-rw-rw-rw-   0        0        0       88 2023-11-22 05:37:05.000000 vlppy-0.1.16/vlppy/model/__init__.py
+-rw-rw-rw-   0        0        0      116 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/model/__init__.pyi
+-rw-rw-rw-   0        0        0     7130 2024-02-05 07:35:21.000000 vlppy-0.1.16/vlppy/model/led.py
+-rw-rw-rw-   0        0        0     1035 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/model/led.pyi
+-rw-rw-rw-   0        0        0    36752 2024-04-13 04:07:22.000000 vlppy-0.1.16/vlppy/model/pd.py
+-rw-rw-rw-   0        0        0     2368 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/model/pd.pyi
+-rw-rw-rw-   0        0        0    27782 2024-03-25 07:22:07.000000 vlppy-0.1.16/vlppy/model/pd2.py
+-rw-rw-rw-   0        0        0     2443 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/model/pd2.pyi
+-rw-rw-rw-   0        0        0    24921 2024-03-08 09:05:12.000000 vlppy-0.1.16/vlppy/model/room.py
+-rw-rw-rw-   0        0        0     1887 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/model/room.pyi
+drwxrwxrwx   0        0        0        0 2024-05-08 10:21:57.221082 vlppy-0.1.16/vlppy/setting/
+-rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 vlppy-0.1.16/vlppy/setting/__init__.py
+-rw-rw-rw-   0        0        0       48 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/setting/__init__.pyi
+-rw-rw-rw-   0        0        0     2894 2023-12-27 05:28:09.000000 vlppy-0.1.16/vlppy/setting/json_setting.py
+-rw-rw-rw-   0        0        0      354 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/setting/json_setting.pyi
+-rw-rw-rw-   0        0        0     1797 2023-12-27 05:57:23.000000 vlppy-0.1.16/vlppy/setting/settings.json
+drwxrwxrwx   0        0        0        0 2024-05-08 10:21:57.239707 vlppy-0.1.16/vlppy/signal/
+-rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 vlppy-0.1.16/vlppy/signal/__init__.py
+-rw-rw-rw-   0        0        0       44 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/signal/__init__.pyi
+-rw-rw-rw-   0        0        0     8842 2023-12-27 05:29:53.000000 vlppy-0.1.16/vlppy/signal/filter.py
+-rw-rw-rw-   0        0        0     1342 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/signal/filter.pyi
+-rw-rw-rw-   0        0        0     3821 2023-12-27 05:30:44.000000 vlppy-0.1.16/vlppy/signal/plot.py
+-rw-rw-rw-   0        0        0      440 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/signal/plot.pyi
+drwxrwxrwx   0        0        0        0 2024-05-08 10:21:57.247088 vlppy-0.1.16/vlppy/tools/
+-rw-rw-rw-   0        0        0       26 2023-04-18 03:21:34.000000 vlppy-0.1.16/vlppy/tools/__init__.py
+-rw-rw-rw-   0        0        0       26 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/tools/__init__.pyi
+-rw-rw-rw-   0        0        0      307 2023-12-27 05:30:49.000000 vlppy-0.1.16/vlppy/tools/decorator.py
+-rw-rw-rw-   0        0        0       22 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/tools/decorator.pyi
+drwxrwxrwx   0        0        0        0 2024-05-08 10:21:57.260879 vlppy-0.1.16/vlppy/vis/
+-rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 vlppy-0.1.16/vlppy/vis/__init__.py
+-rw-rw-rw-   0        0        0       20 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/vis/__init__.pyi
+-rw-rw-rw-   0        0        0     3574 2024-01-04 13:12:34.000000 vlppy-0.1.16/vlppy/vis/vis.py
+-rw-rw-rw-   0        0        0      458 2024-04-13 04:05:02.000000 vlppy-0.1.16/vlppy/vis/vis.pyi
+drwxrwxrwx   0        0        0        0 2024-05-08 10:21:57.261877 vlppy-0.1.16/vlppy.egg-info/
+-rw-rw-rw-   0        0        0     5387 2024-05-08 10:21:57.000000 vlppy-0.1.16/vlppy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2024-05-08 10:21:57.000000 vlppy-0.1.16/vlppy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 10:21:57.000000 vlppy-0.1.16/vlppy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-08 10:21:57.000000 vlppy-0.1.16/vlppy.egg-info/top_level.txt
```

### Comparing `vlppy-0.1.15/LICENSE` & `vlppy-0.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/PKG-INFO` & `vlppy-0.1.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlppy
-Version: 0.1.15
+Version: 0.1.16
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/vlppy.git
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `vlppy-0.1.15/README.md` & `vlppy-0.1.16/README.md`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/pyproject.toml` & `vlppy-0.1.16/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vlppy"
-version = "0.1.15"
+version = "0.1.16"
 authors = [
   { name="yangwuju", email="1424134319@qq.com" },
 ]
 description = "Construction of visible light positioning model"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.5"
```

### Comparing `vlppy-0.1.15/setup.py` & `vlppy-0.1.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 path = os.path.join(CUR_PATH, 'build')
 if os.path.isdir(path):
     print('INFO del dir ', path) 
     shutil.rmtree(path)
 
 setup(
     name = 'vlppy', #应用名
-    version = '0.1.15',  #版本号
+    version = '0.1.16',  #版本号
     description = 'Construction of visible light positioning model', 
     packages = find_packages(),  #包括在安装包内的Python包
     include_package_data = True, #启用清单文件MANIFEST.in,包含数据文件
     # exclude_package_data = {'docs':['1.txt']},  #排除文件
     install_requires = [#自动安装依赖
         'numpy>=1.19.0',
         'matplotlib>=3.5.0',
```

### Comparing `vlppy-0.1.15/vlppy/LICENSE.txt` & `vlppy-0.1.16/vlppy/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/demo/README.md` & `vlppy-0.1.16/vlppy/demo/README.md`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/demo/demo_filter.py` & `vlppy-0.1.16/vlppy/demo/demo_filter.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/demo/demo_main.py` & `vlppy-0.1.16/vlppy/demo/demo_main.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/demo/vlp_model.py` & `vlppy-0.1.16/vlppy/demo/vlp_model.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/error/error.py` & `vlppy-0.1.16/vlppy/error/error.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/io/io.py` & `vlppy-0.1.16/vlppy/io/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,18 +30,18 @@
         np.savez(fp, **dataset)
  
     def load_npz(self, fp, **argkeys):
         """加载npz格式数据, 返回numpy类型数据
         """
         return np.load(fp, **argkeys)
 
-    def save_csv(self, fp:str, *dataFrame:dict):
+    def save_csv(self, fp:str, dataFrame:dict):
         """保存为.csv
         """
-        data = pd.DataFrame(data)
+        data = pd.DataFrame(dataFrame)
         data.to_csv(fp) 
 
     def load_csv(self, fp:str):
         """加载.csv文件, 返回numpy类型数据
         """
         return pd.read_csv(fp).to_numpy()
```

### Comparing `vlppy-0.1.15/vlppy/io/io.pyi` & `vlppy-0.1.16/vlppy/io/io.pyi`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/model/led.py` & `vlppy-0.1.16/vlppy/model/led.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/model/led.pyi` & `vlppy-0.1.16/vlppy/model/led.pyi`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/model/pd.py` & `vlppy-0.1.16/vlppy/model/pd.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 from numbers import Number
-from typing import Union
+from typing import Union,Sequence
 from .led import LED
 from .room import Room
 from ..error import VLPSequenceLenError,VLPValueRangeError
-
+from scipy.spatial.transform import Rotation 
+ 
 class PD:
     """光电探测器(PD)
     """
     def __init__(self,
                 n:Number=1.5,
                 fov:Number=60,
                 Ar:Number=1e-4,
@@ -170,18 +171,19 @@
         """
         # 以下是为了兼容交直流信号
         R0 = np.expand_dims(R0, -1)              # 在最后一维扩充一个维度 (l*w*h) -> (l*w*h,1)  <=> H0.reshape(l*w*h,1) <=> H0[...,np.newaxis]
         radiation_intensity = R0 * led.signal    # LED辐射强度[广播机制 (l*w*h,1) * (npt) -> (l*w*h,npt) * (l*w*h,npt) = (l*w*h,npt)]
 
         return np.squeeze(radiation_intensity)   # (l*w*h,npt).如果npt==1,则返回形状为(l*w*h)
 
-    def recv_los_led_signal(self, led:LED):
+    def recv_los_led_signal(self, led:LED, fov_condition=True, *args, **kwargs):
         """计算PD接收LED信号(LOS链路):
         Params
             led: LED实例化
+            fov_condition: 是否添加视场条件(考虑旋转需设为False)
         Return 
             LOS链路中PD探测器接收LED信号
         """
         #⭐ LED -> PD
         # LED发射端
         Vt_r = self.pos - led.pos                                   # LED到PD的方向向量 (l*w*h,3)
         d = np.linalg.norm(Vt_r, axis=-1)                           # 求模:LED到PD的方向向量的模 (l*w*h)
@@ -195,15 +197,16 @@
         # PD接收端
         Vr_t = -Vt_r # PD到LED的方向向量 (l*w*h,3)
         cos_pd_r_angle_rad = np.sum(Vr_t*self.Nv, axis=-1) / d      # PD接收角的余弦值 (l*w*h) 
         pd_r_angle_rad = np.arccos(cos_pd_r_angle_rad)              # PD接收器入射角的大小(弧度制) (l*w*h)
         pd_r_angle = np.degrees(pd_r_angle_rad)                     # 弧度制转为角度制 (l*w*h)
 
         cos_pd_r_angle_rad = np.abs(cos_pd_r_angle_rad)             # 解决PD入射角大于90°,入射角余弦值为负值情况
-        cos_pd_r_angle_rad = np.where((pd_r_angle>=0) & (pd_r_angle<=self.fov), cos_pd_r_angle_rad, 0)  # 满足PD入射条件
+        if fov_condition:
+            cos_pd_r_angle_rad = np.where((pd_r_angle>=0) & (pd_r_angle<=self.fov), cos_pd_r_angle_rad, 0)  # 满足PD入射条件
 
         # 计算信道增益
         H0 = (((led.m + 1) * self.Ar) / (2 * np.pi * d**2)) * cos_led_t_angle_rad**led.m * cos_pd_r_angle_rad * self.Ts * self.G_Con # (l*w*h)
 
         """ y(t) = x(t) * h(t)
         H0 = H0.flatten() # 打平 (l,w) -> (l*w,)
         return np.array([np.convolve(h,led.send_signal) for h in H0])  # 卷积 (l*w,npt)
@@ -211,24 +214,26 @@
         """
         # 以下是为了兼容交直流信号
         H0 = np.expand_dims(H0, axis=-1)  # 在最后一维扩充一个维度 (l*w*h) -> (l*w*h,1)  <=> H0.reshape(l*w*h,1) <=> H0[...,np.newaxis]
         recv_signal = H0 * led.signal     # PD接收信号 [广播机制 (l*w*h,1) * (npt) -> (l*w*h,npt) * (l*w*h,npt) = (l*w*h,npt)]
 
         return np.squeeze(recv_signal)    # (l,w,h,npt).如果npt==1,则返回形状为(l,w,h)
       
-    def recv_nlos_led_signal(self, led:LED, room:Room):
+    def recv_nlos_led_signal(self, led:LED, room:Room, fov_condition=True, *args, **kwargs):
         """计算PD接收LED一次反射信号(NLOS链路):
         Params
             led: LED实例化
             room: Room实例化
+            fov_condition: 是否添加视场条件(考虑旋转需设为False)
         Return 
             NLOS链路中PD探测器接收LED一次反射信号
         """
         # 对PD坐标张量扩充维度,以便使用广播
         pd_pos = np.expand_dims(self.pos, axis=-2)  # (l*w*h,3) -> (l*w*h,1,3) 
+        pd_Nv = np.expand_dims(self.Nv, axis=-2)   # PD法向量 (n,3) -> (n,1,3) or  (3) -> (1,3)
 
         H0 = 0  #反射(LOS)链路信道增益
         # 遍历每一面反射墙壁参数:(l1*w1,3),(l1*w1,2)
         for i, (w_pos, angle) in enumerate(room.get_reflect_wall_args()):
             w_alpha, w_beta = np.split(angle, indices_or_sections=2, axis=-1)   # (l1*w1,2) -> (l1*w1,1) + (l1*w1,1)
             w_alpha, w_beta = np.squeeze([w_alpha, w_beta])                     # (l1*w1,1) -> (l1*w1)
 
@@ -236,19 +241,19 @@
             w_alpha_rad, w_beta_rad = np.radians([w_alpha, w_beta]) # (l1*w1)
             
             # 墙壁反射面元法向量
             Nx = np.cos(w_alpha_rad) * np.sin(w_beta_rad)
             Ny = np.sin(w_alpha_rad) * np.sin(w_beta_rad)
             Nz = np.cos(w_beta_rad)
 
-            Nw = np.stack([Nx,Ny,Nz], axis=-1)             # 墙壁反射点法向量 (l1*w1,3)
-            Nw_norm = np.linalg.norm(Nw, axis=-1)          # 墙壁反射点法向量模 (l1*w1)
+            Nw = np.stack([Nx,Ny,Nz], axis=-1)             # 墙壁反射面元法向量 (l1*w1,3)
+            Nw_norm = np.linalg.norm(Nw, axis=-1)          # 墙壁反射面元法向量模 (l1*w1)
             if Nw.ndim > 1:
                 Nw_norm = np.expand_dims(Nw_norm, axis=-1) # (l1*w1,1)
-            Nw = Nw/Nw_norm                                # 墙壁反射点的单位法向量 (l1*w1,3)
+            Nw = Nw/Nw_norm                                # 墙壁反射面元单位法向量 (l1*w1,3)
 
             #⭐ LED -> 墙壁反射面元
             # LED发射端
             Vt_w = w_pos - led.pos              # LED灯到墙壁反射面元的方向向量 (l1*w1,3)
             d1 = np.linalg.norm(Vt_w, axis=-1)  # 求模:LED灯到墙壁反射面元的距离 (l1*w1)
             mark1 = np.all(Vt_w==0, axis=-1)    # 异常点处理:判断墙壁反射面元和LED是否重合(方向向量是否为零向量) (l1*w1)
             d1 = np.where(mark1, 1, d1)         # 异常点处理:为使cos_led_t_angle_rad分母不为0,让墙壁反射面元和LED重合时的距离不为0 (l1*w1)
@@ -273,20 +278,21 @@
             d2 = np.where(mark2, 1, d2)        # 异常点处理:为使cos_wall_t_angle_rad分母不为0,让墙壁反射面元和参考点重合时的距离不为0
 
             cos_wall_t_angle_rad = np.sum(Vw_r*Nw, axis=-1) / d2                             # 墙壁反射面元发射角 (l*w*h,l1*w1)
             cos_wall_t_angle_rad = np.where(cos_wall_t_angle_rad>0, cos_wall_t_angle_rad, 0) # 满足墙壁反射条件 (发射角小于90)
     
             # PD接收端
             Vr_w = -Vw_r                                             # PD到墙壁反射面元的方向向量 (l*w*h,l1*w1,3)
-            cos_pd_r_angle_rad = np.sum(Vr_w*self.Nv, axis=-1) / d2  # PD接收角的余弦值 (l*w*h,l1*w1)
+            cos_pd_r_angle_rad = np.sum(Vr_w*pd_Nv, axis=-1) / d2    # PD接收角的余弦值 (l*w*h,l1*w1)
             pd_r_angle_rad = np.arccos(cos_pd_r_angle_rad)           # PD接收器入射角(弧度制) (l*w*h,l1*w1)
             pd_r_angle = np.degrees(pd_r_angle_rad)                  # 弧度制转为角度制 (l*w*h,l1*w1)
             
             cos_pd_r_angle_rad = np.abs(cos_pd_r_angle_rad)          # 解决PD入射角大于90°,入射角余弦值为负值情况
-            cos_pd_r_angle_rad = np.where((pd_r_angle>=0) & (pd_r_angle<=self.fov), cos_pd_r_angle_rad, 0)  # 满足PD入射条件
+            if fov_condition:
+                cos_pd_r_angle_rad = np.where((pd_r_angle>=0) & (pd_r_angle<=self.fov), cos_pd_r_angle_rad, 0)  # 满足PD入射条件
 
             rho = room.rho[i]   # 墙壁反射率
             Aw  = room.Aw[i]    # 墙壁反射面元面积
 
             # 反射(NLOS)子链路信道增益  
             Hw = (((led.m + 1) * self.Ar) / (2 * np.pi * d1**2 * d2**2)) * rho * Aw * cos_led_t_angle_rad**led.m * cos_wall_r_angle_rad * cos_wall_t_angle_rad *  cos_pd_r_angle_rad * self.Ts * self.G_Con  # (l*w*h,l1*w1)
             Hw = np.sum(Hw, axis=-1)   # 反射(NLOS)链路信道增益求和 (l*w*h,l1*w1) -> (l*w*h)
@@ -294,16 +300,16 @@
             # 对所有反射墙壁(NLOS)链路信道增益求和  
             H0 += Hw                   # (l*w*h)
 
         # 墙壁一次反射(NLOS)链路信道增益
         H0 = np.expand_dims(H0,-1)     # 在最后一维扩充一个维度 (l*w*h) -> (l*w*h,1)  <=> H0.reshape(l*w*h,1) <=> H0[...,np.newaxis]
         recv_signal = H0 * led.signal  # PD接收信号[广播机制 (l*w*h,1) * (npt) -> (l*w*h,npt) * (l*w*h,npt) = (l*w*h,npt)]
         return np.squeeze(recv_signal) # 去除维度为1的维数
-    
-    def recv_led_signal(self, led:LED, room:Room):
+
+    def recv_led_signal(self, led:LED, room:Room,  *args, **kwargs):
         """计算PD接收LED信号(LOS+NLOS链路):
         Params
             led: LED实例化
             room: Room实例化
         Return 
             LOS+NLOS链路中PD探测器接收LED信号
         """
@@ -347,14 +353,15 @@
             16*np.pi**2*k*Tk*gamma/gm*eta**2*self.Ar**2*I3*B**3
 
     def recv_noise_signal(self, P, *argv, **kwargv):
         """接收噪声信号功率
         """
         return self.shot_noise(P=P, *argv, **kwargv) + self.thermal_noise(*argv, **kwargv)
 
+
     def SNR(self, P, R, dB=True, *argv, **kwargv):
         """信噪比
         Params
             P: PD接收LOS+NLOS链路的光功率
             R: PD的响应度
             dB: 信噪比dB表示
         Return
@@ -475,8 +482,278 @@
     def G_Con(self):
         """获取聚光器增益
         """
         # 角度制转弧度制
         fov_rad = np.radians(self.fov)
 
         return self.n**2 / np.sin(fov_rad)**2  
+    
+    @staticmethod
+    def expand_dims_to_broacast(arr,shape=None,repeat:int=None,axis:int=0):
+        """ arr 维度扩充并广播到指定形状 shape
+        Params:
+            arr: 要扩维的array
+            shape: 添加n个维度需要广播到对应的形状
+            repeat: 重复添加n个维度(并广播到对应的形状)
+            axis: 指定轴
+        """
+        assert repeat or np.all(shape)
+        if isinstance(shape, Number): shape = [shape]
+        if axis >= 0: shape = np.flip(shape)
+        if not repeat: repeat = 1
+        
+        for _ in range(repeat):
+            for i in range(np.size(shape)):
+                arr = np.expand_dims(arr, axis=axis) # 扩维
+                if np.all(shape):
+                    arr = np.repeat(arr, shape[i], axis=axis) # 在axis轴上复制操作【广播】
+        return arr
+    
+    @staticmethod
+    def tp_raw_args(center_tp_pos:tuple, angles:Sequence):
+        """获取PD特征【位置、角度】
+        等效 x, y, z, alpha, beta, gamma = np.meshgrid(x, y, z, alpha, beta, gamma)
+        """
+        pos = np.asarray(center_tp_pos)
+        angles = np.asarray(angles)
+
+        assert len(pos) == 3 or pos.shape[-1] == 3
+        assert len(angles) == 3 or angles.shape[-1] == 3
+
+        if pos.ndim == 1:         # (3) -> (1,3)
+            pos = np.expand_dims(pos, axis=0)
+        else:
+            if len(pos) == 3:     # (3,n) -> (n,3)
+                pos = np.stack(pos, axis=-1)
+
+        if angles.ndim == 1:      # (3) -> (1,3)
+            angles = np.expand_dims(angles, axis=0)
+        else:
+            if len(angles) == 3:  # (3,n) -> (n,3)
+                angles = np.stack(angles, axis=-1)
+        pos_shape, angles_shape = pos.shape[0], angles.shape[0]         # (l*w*h), (a*b*g)
+
+        if angles.ndim > 1: # 动态时PD将会存在角度偏转
+            # 扩维后广播
+            pos = PD.expand_dims_to_broacast(pos, shape=angles_shape, axis=-2)    # (l*w*h, a*b*g, 3) 
+            pos = np.reshape(pos,newshape=(-1,3))                                 # (l*w*h*a*b*g,3) = (n,3)
+
+        if pos.ndim > 1: 
+            # 扩维后广播 
+            angles = PD.expand_dims_to_broacast(angles, shape=pos_shape, axis=0)  # (l*w*h,a*b*g,3) 
+            angles = np.reshape(angles,newshape=(-1,3))                 # (l*w*h*a*b*g,3) = (n,3)
+
+        # 分离轴
+        xr, yr, zr = np.split(pos, indices_or_sections=3, axis=-1)            # (n,1)*3
+        alpha, beta, gamma = np.split(angles, indices_or_sections=3, axis=-1) # (n,1)*3
+
+        # 去除维数为1的维度
+        xr, yr, zr = np.squeeze([xr, yr, zr])                                 # (n)*3 
+        alpha, beta, gamma = alpha.flatten(), beta.flatten(), gamma.flatten() # (n)*3
+
+        return np.array([xr,yr,zr]), np.array([alpha,beta,gamma])
+    
+    @staticmethod
+    def rotation_pd_recv_los_led_signal(P, led:LED, tp_pos, pd_pos, pd_Nv, fov=90, angles=(0,0,0), seq="zxy", *args, **kwargs):
+        """LOS链路,获取旋转后的PD接收功率
+           旋转前后功率的比值: 
+                R_P/P = (d/R_d)**(m+3) * (R_Vtr @ R_Nt/ Vtr @ Nt)**m * (R_Vrt @ R_Nr/ Vrt @ Nr)
+        Params
+            P: 未旋转时PD接收功率(正常定位时的接收功率)
+            led: LED实例化
+            tp_pos: 待测点位置
+            pd_pos: PD位置
+            fov: PD视场角
+            angles: 旋转角度 (单位:度)
+            seq: 旋转顺序
+        Return
+            旋转后的PD接收功率
+        """
+        if not len(P) == len(tp_pos) == len(pd_pos):
+            raise Exception("These arrays have different shapes.")
+
+        # PD法向量单位化
+        pd_Nv_norm = np.linalg.norm(pd_Nv, axis=-1)            # PD法向量模 (l1*w1)
+        if pd_Nv.ndim > 1:
+            pd_Nv_norm = np.expand_dims(pd_Nv_norm, axis=-1)   # (l1*w1,1)
+        pd_Nv = pd_Nv/pd_Nv_norm                               # PD的单位法向量 (l1*w1,3)
+
+        # 旋转角度
+        assert len(angles) == 3 or angles.shape[-1] == 3
+        if len(angles) == 3:
+            alpha, beta, gamma = angles
+            angles = np.stack([alpha, beta, gamma], axis=-1) # 旋转了m次 (m,3)   
+
+        Rmat = Rotation.from_euler(
+            seq, angles, degrees=True).as_matrix()           # 旋转矩阵 (m,3,3) 
+        
+        o_pd_pos = pd_pos - tp_pos                           # PD的相对于旋转中心O的位置 (n,3)
+        R_pd_pos, R_Nv = [], []                              # 旋转后PD的位置和法向量
+        for Vo_pd, o_pos in zip(o_pd_pos, tp_pos):
+            R_pd_pos.append(Rmat @ Vo_pd + o_pos)            # n个待测点,每点旋转m次,旋转后PD位置 (m,3,3) @ n*(3) =(n,m,3)
+        R_Nv = Rmat @ pd_Nv                                  # 旋转后PD的法向量 (n,m,3) or (m,3)
+
+        #⭐未旋转前
+        ## LED 发射端
+        Vtr = pd_pos - led.pos                               # LED到PD方向向量 (n,3)
+        Vtr_dot = np.sum(Vtr * led.Nv, axis=-1)              # 向量内积 (n)
+
+        ## PD 接收端             
+        Vrt = -Vtr                                           # PD到LED方向向量 (n,3)
+        d = np.linalg.norm(Vrt, axis=-1)                     # PD到LED的距离 (n)
+        Vrt_dot = np.sum(Vrt * pd_Nv, axis=-1)               # 向量内积 (n)
+
+        #⭐旋转后
+        ## LED 发射端
+        R_Vtr = R_pd_pos - led.pos                           # 旋转后,LED到PD的方向向量 (n,m,3)
+        R_Vtr_dot = np.sum(R_Vtr * led.Nv, axis=-1)          # 旋转后,向量内积 (n,m)
+
+        ## PD 接收端
+        R_Vrt = -R_Vtr                                       # 旋转后,PD到LED的方向向量 (n,m,3) 
+        R_d = np.linalg.norm(R_Vrt, axis=-1)                 # 旋转后,PD到LED的距离 (n,m)
+        R_Vrt_dot = np.sum(R_Vrt * R_Nv, axis=-1)            # 旋转后,向量内积 (n,m)
+
+        # 预处理,便于矩阵运算
+        d = np.expand_dims(d, axis=-1)                       # (n) -> (n,1)
+        Vrt_dot = np.expand_dims(Vrt_dot, axis=-1)           # (n) -> (n,1)
+        Vtr_dot = np.expand_dims(Vtr_dot, axis=-1)           # (n) -> (n,1)
+        P = np.expand_dims(P, axis=-1)                       # (n) -> (n,1)
+
+        # 代入计算
+        R_P = P * (d/R_d)**(led.m+3) * np.abs(R_Vtr_dot/Vtr_dot)**led.m * np.abs(R_Vrt_dot/Vrt_dot) # (n,m)
+
+        # 满足视场角内接收
+        cos_pd_r_angle_rad = R_Vrt_dot/R_d                   # PD接收入射角余弦值
+        pd_r_angle_rad = np.arccos(cos_pd_r_angle_rad)       # PD接收器入射角(弧度制) (n,l1*w1)
+        pd_r_angle = np.degrees(pd_r_angle_rad)              # 弧度制转为角度制 (n,l1*w1)
+        R_P = np.where((pd_r_angle>=0) & (pd_r_angle<=fov), R_P, 0) # 视场角内接收功率
+        R_P = np.reshape(R_P,-1)                             # (n,m) -> (n*m)
+        
+        return R_P
+    
+    @staticmethod
+    def rotation_pd_recv_nlos_led_signal( P, room:Room, tp_pos, pd_pos, pd_Nv, fov=90, angles=(0,0,0), seq="zxy", *args, **kwargs):
+        """NLOS链路,获取旋转后的PD接收功率
+           旋转前后功率的比值: 
+                R_P/P = Σ( (d2/d2_r)**4 * (R_Vwr@R_Nw/Vwr@Nw) * (R_Vrw@R_Nr/Vrw@Nr) )
+        Params 
+            P: 未旋转时PD接收功率(正常定位时的接收功率)
+            room: Room实例化
+            tp_pos: 待测点位置
+            pd_pos: PD位置
+            fov: PD视场角
+            angles: 旋转角度 (单位:度)
+            seq: 旋转顺序
+        Return 
+            旋转后的PD接收功率 
+        """
+        raise Exception("This function is not implemented, please pay attention to the subsequent version.")
+        # if not len(P) == len(tp_pos) == len(pd_pos) :          # (n)
+        #     raise Exception("These two arrays have different shapes.")
+
+        # # PD法向量单位化
+        # pd_Nv_norm = np.linalg.norm(pd_Nv, axis=-1)            # PD法向量模 (n)
+        # if pd_Nv.ndim > 1:
+        #     pd_Nv_norm = np.expand_dims(pd_Nv_norm, axis=-1)   
+        # pd_Nv = pd_Nv/pd_Nv_norm                               # PD的单位法向量 (n,3) or (3)
+        # pd_Nv = np.broadcast_to(pd_Nv, np.shape(pd_pos))       # (n,3)
+
+        # # 旋转角度
+        # assert len(angles) == 3 or angles.shape[-1] == 3 
+        # if len(angles) == 3:
+        #     alpha, beta, gamma = angles
+        #     angles = np.stack([alpha, beta, gamma], axis=-1)   # (m,3)   
+
+        # Rmat = Rotation.from_euler(
+        #     seq, angles, degrees=True).as_matrix()             # 旋转矩阵 (m,3,3) 
+        
+        # o_pd_pos = pd_pos - tp_pos                             # PD相对于旋转中心O的位置 (n,3)
+
+        # R_pd_pos, R_Nv = [], []                                # 旋转后PD的位置和法向量
+        # for Vo_pd, o_pos, Nv in zip(o_pd_pos, tp_pos, pd_Nv):
+        #     R_pd_pos.append(Rmat @ Vo_pd + o_pos)              # n个待测点,每点旋转m次,旋转后PD位置 (m,3,3) @ n*(3) =(n,m,3)
+        #     R_Nv.append(Rmat @ Nv)                             # (m,3,3) @ n*(3) =(n,m,3)
+        # R_pd_pos, R_Nv = np.asarray(R_pd_pos), np.asarray(R_Nv)   
+
+        # # 对PD坐标张量扩充维度,以便使用广播
+        # pd_pos = np.expand_dims(np.expand_dims(pd_pos, axis=-2), axis=-2)   # (n,3) -> (n,1,1,3) 
+        # tp_pos = np.expand_dims(np.expand_dims(tp_pos, axis=-2), axis=-2)   # (n,3) -> (n,1,1,3) 
+        # pd_Nv  = np.expand_dims(np.expand_dims(pd_Nv, axis=-2), axis=-2)    # (n,3) -> (n,1,1,3) 
+        # R_pd_pos = np.expand_dims(R_pd_pos, axis=-2)                        # (n,m,3) -> (n,m,1,3) 
+        # R_Nv = np.expand_dims(R_Nv, axis=-2)                                # (n,m,3) -> (n,m,1,3) 
+        # P = np.expand_dims(P,-1)                                            # (n,1) -> (n,1)
+
+        # G = 0 # NLOS旋转前后信道增益比例系数 
+        
+        # # 遍历每一面反射墙壁参数:(l1*w1,3), (l1*w1,2)
+        # for w_pos, angle in room.get_reflect_wall_args():
+        #     w_alpha, w_beta = np.split(angle, indices_or_sections=2, axis=-1)   # (l1*w1,2) -> (l1*w1,1) + (l1*w1,1)
+        #     w_alpha, w_beta = np.squeeze([w_alpha, w_beta])                     # (l1*w1,1) -> (l1*w1) 
+
+        #     # 墙壁反射面元法向量与x轴和z轴的夹角,角度制转弧度制
+        #     w_alpha_rad, w_beta_rad = np.radians([w_alpha, w_beta])             # (l1*w1)
+            
+        #     # 墙壁反射面元法向量
+        #     Nx = np.cos(w_alpha_rad) * np.sin(w_beta_rad)
+        #     Ny = np.sin(w_alpha_rad) * np.sin(w_beta_rad)
+        #     Nz = np.cos(w_beta_rad)
+
+        #     Nw = np.stack([Nx,Ny,Nz], axis=-1)               # 墙壁反射面元法向量 (l1*w1,3)
+        #     Nw_norm = np.linalg.norm(Nw, axis=-1)            # 墙壁反射点法向量模 (l1*w1)
+        #     if Nw.ndim > 1:
+        #         Nw_norm = np.expand_dims(Nw_norm, axis=-1)   # (l1*w1,1)
+        #     Nw = Nw/Nw_norm                                  # 墙壁反射点的单位法向量 (l1*w1,3)
+
+        #     #⭐未旋转前
+        #     ## 墙壁面元发射端
+        #     Vwr = pd_pos - w_pos                             # 墙壁面元d到PD的方向向量 (n,1,1,3) - (l1*w1,3) -> (n,1,l1*w1,3)
+        #     d = np.linalg.norm(Vwr, axis=-1)                 # PD到墙壁面元的距离 (n,1,l1*w1)
+        #     Vwr_dot = np.sum(Vwr * Nw, axis=-1)              # 向量内积 (n,1,l1*w1)
+        #     Vwr_dot = np.where(Vwr_dot>0, Vwr_dot, 0)        # 满足墙壁反射条件 (发射角小于90)
+
+        #     ## PD 接收端             
+        #     Vrw = -Vwr                                               # PD到墙壁面元方向向量 (n,1,l1*w1,3)
+        #     Vrw_dot = np.sum(Vrw * pd_Nv, axis=-1)                   # 向量内积 (n,1,l1*w1)
+
+        #     mark1 = np.all(Vrw==0, axis=-1)                          # 异常点处理:判断墙壁反射面元和参考点是否重合(方向向量是否为零向量) (l*w*h,l1*w1)
+        #     cos_pd_r_angle_rad = np.where(mark1, 1, Vrw_dot / d)     # PD接收角的余弦值   (n,l1*w1)
+        #     pd_r_angle_rad = np.arccos(cos_pd_r_angle_rad)           # PD接收器入射角(弧度制) (n,l1*w1)
+        #     pd_r_angle = np.degrees(pd_r_angle_rad)                  # 弧度制转为角度制 (n,l1*w1)
+        #     Vrw_dot = np.where((pd_r_angle>=0) & (pd_r_angle<=fov), Vrw_dot, 0)  # 满足PD入射条件
+
+        #     #⭐旋转后
+        #     ## 墙壁面元发射端
+        #     R_Vwr = R_pd_pos - w_pos                             # 墙壁面元d到PD的方向向量 (n,m,1,3) - (l1*w1,3) -> (n,m,l1*w1,3)
+        #     R_d = np.linalg.norm(R_Vwr, axis=-1)                 # PD到墙壁面元的距离 (n,m,l1*w1)
+        #     R_Vwr_dot = np.sum(R_Vwr * Nw, axis=-1)              # 向量内积 (n,m,l1*w1)
+        #     R_Vwr_dot = np.where(R_Vwr_dot>0, R_Vwr_dot, 0)      # 满足墙壁反射条件 (发射角小于90)
+
+        #     ## PD 接收端             
+        #     R_Vrw = -R_Vwr                                       # PD到墙壁面元方向向量 (n,m,l1*w1,3)
+        #     R_Vrw_dot = np.sum(R_Vrw * R_Nv, axis=-1)            # 向量内积 (n,m,l1*w1) 
+
+        #     mark2 = np.all(R_Vrw==0, axis=-1)                             # 异常点处理:判断墙壁反射面元和参考点是否重合(方向向量是否为零向量) (n,m,l1*w1) 
+        #     R_cos_pd_r_angle_rad = np.where(mark2, 1, R_Vrw_dot / R_d)    # PD接收角的余弦值   (n,l1*w1)
+        #     R_pd_r_angle_rad = np.arccos(R_cos_pd_r_angle_rad)            # PD接收器入射角(弧度制) (n,l1*w1)
+        #     R_pd_r_angle = np.degrees(R_pd_r_angle_rad)                   # 弧度制转为角度制 (n,l1*w1)
+        #     R_Vrw_dot = np.where((R_pd_r_angle>=0) & (R_pd_r_angle<=fov), R_Vrw_dot, 0)  # 满足PD入射条件
+
+        #     # 异常点处理:判断墙壁反射面元和参考点是否重合    
+        #     Vwr_dot = np.where(Vwr_dot==0, 1, Vwr_dot)
+        #     Vrw_dot = np.where(Vrw_dot==0, 1, Vrw_dot)
+        #     d = np.where(Vwr_dot==0, 0, d)      
+        #     R_d = np.where(R_d==0, 1, R_d)       
+        #     R_Vrw_dot = np.where(R_d==0, 0, R_Vrw_dot)       
+            
+        #     # 代入计算 
+        #     Gw = (d/R_d)**4 * np.abs(R_Vwr_dot/Vwr_dot) * np.abs(R_Vrw_dot/Vrw_dot)  # 比例系数值 (n,m,l1*w1)
+
+        #     Gw = np.sum(Gw, axis=-1)    # 反射(NLOS)链路Gw求和 (n,m,l1*w1)-> (n,m) 
+        #     G += Gw                     # 对所有反射面元比例系数值求和 (n,m) 
+
+        # # 计算功率
+        # R_P = G * P                     # (n,m)
+
+        # # 旋转后的PD接收功率 (n,m)
+        # R_P = np.reshape(R_P,-1)        # (n,m) -> (n*m)
 
+        # return R_P
```

### Comparing `vlppy-0.1.15/vlppy/model/pd.pyi` & `vlppy-0.1.16/vlppy/model/pd2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,61 @@
 from ..error import VLPSequenceLenError as VLPSequenceLenError, VLPValueRangeError as VLPValueRangeError
 from .led import LED as LED
 from .room import Room as Room
+from _typeshed import Incomplete
 from numbers import Number
-from typing import Union
+from typing import Sequence, Union
 
-class PD:
-    def __init__(self, n: Number = ..., fov: Number = ..., Ar: Number = ..., Ts: Number = ..., pos: tuple = ..., Nv: tuple = ..., origin: tuple = ..., *args, **kwargs) -> None: ...
+class PD2:
+    def __init__(self, n: Number = ..., fov: Number = ..., Ar: Number = ..., Ts: Number = ..., tp_pos=..., pos: tuple = ..., Nv: tuple = ..., angles: Sequence = ..., seq: str = ..., origin: tuple = ..., *args, **kwargs) -> None: ...
+    @staticmethod
+    def get_euler_angle(alpha, beta, gamma): ...
+    @staticmethod
+    def tp_raw_args(center_tp_pos: tuple, angles: Sequence): ...
     @staticmethod
     def recv_frame_model(l, alpha, beta, center_tp_pos: tuple): ...
     @staticmethod
     def recv_surface_model(r: Union[Number, tuple], alpha, beta, center_tp_pos: tuple): ...
     @staticmethod
     def recv_hemisphere_model(r, l, alpha, center_tp_pos: tuple): ...
     def recv_led_radiation_intensity(self, led: LED): ...
     def recv_los_led_signal(self, led: LED): ...
     def recv_nlos_led_signal(self, led: LED, room: Room): ...
     def recv_led_signal(self, led: LED, room: Room): ...
     def shot_noise(self, P, R: float = ..., Ibg: float = ..., I2: float = ..., B: float = ..., *argv, **kwargv): ...
     def thermal_noise(self, Tk: int = ..., G: int = ..., eta: int = ..., B: float = ..., I2: float = ..., I3: float = ..., gamma: float = ..., gm: int = ..., *argv, **kwargv): ...
     def recv_noise_signal(self, P, *argv, **kwargv): ...
     def SNR(self, P, R, dB: bool = ..., *argv, **kwargv): ...
+    @staticmethod
+    def expand_dims_to_broacast(arr, shape: Incomplete | None = ..., repeat: int = ..., axis: int = ...): ...
     @property
     def origin(self) -> tuple: ...
     @property
+    def tp_pos(self): ...
+    @property
+    def raw_tp_pos(self): ...
+    @property
     def pos(self): ...
     @property
     def Nv(self): ...
     @property
+    def sequence(self): ...
+    @property
+    def angles(self): ...
+    @property
+    def raw_angles(self): ...
+    @property
+    def raw_args(self): ...
+    @property
+    def Rmat(self): ...
+    @property
+    def R_pos(self): ...
+    @property
+    def R_Nv(self): ...
+    @property
     def fov(self): ...
     @property
     def Ar(self): ...
     @property
     def Ts(self): ...
     @property
     def n(self): ...
```

### Comparing `vlppy-0.1.15/vlppy/model/pd2.py` & `vlppy-0.1.16/vlppy/model/pd2.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,20 +82,20 @@
         else:
             if len(angles) == 3:  # (3,n) -> (n,3)
                 angles = np.stack(angles, axis=-1)
         pos_shape, angles_shape = pos.shape[0], angles.shape[0]         # (l*w*h), (a*b*g)
 
         if angles.ndim > 1: # 动态时PD将会存在角度偏转
             # 扩维后广播
-            pos = PD2._expand_dims(pos, shape=angles_shape, axis=-2)    # (l*w*h, a*b*g, 3) 
+            pos = PD2.expand_dims_to_broacast(pos, shape=angles_shape, axis=-2)    # (l*w*h, a*b*g, 3) 
             pos = np.reshape(pos,newshape=(-1,3))                       # (l*w*h*a*b*g,3) = (n,3)
 
         if pos.ndim > 1: 
             # 扩维后广播 
-            angles = PD2._expand_dims(angles, shape=pos_shape, axis=0)  # (l*w*h,a*b*g,3) 
+            angles = PD2.expand_dims_to_broacast(angles, shape=pos_shape, axis=0)  # (l*w*h,a*b*g,3) 
             angles = np.reshape(angles,newshape=(-1,3))                 # (l*w*h*a*b*g,3) = (n,3)
 
         # 分离轴
         xr, yr, zr = np.split(pos, indices_or_sections=3, axis=-1)            # (n,1)*3
         alpha, beta, gamma = np.split(angles, indices_or_sections=3, axis=-1) # (n,1)*3
 
         # 去除维数为1的维度
@@ -431,31 +431,32 @@
             信噪比
         """
         P_noise = self.shot_noise(P=P, R=R, *argv, **kwargv) + self.thermal_noise(*argv, **kwargv)
         snr = (R*P)**2 / P_noise
         return 10*np.log10(snr) if dB else snr
 
     @staticmethod
-    def _expand_dims(arr,n=None,shape=None,axis=0):
+    def expand_dims_to_broacast(arr,shape=None,repeat:int=None,axis:int=0):
         """ arr 维度扩充并广播到指定形状 shape
         Params:
             arr: 要扩维的array
-            n: 需要添加n个维度
             shape: 添加n个维度需要广播到对应的形状
+            repeat: 重复添加n个维度(并广播到对应的形状)
             axis: 指定轴
         """
-        assert n or np.all(shape)
-        if isinstance(shape, Number):
-            shape = [shape]
-        if not n:
-            n = np.size(shape)
-        for i in range(n):
-            arr = np.expand_dims(arr, axis=axis) # 扩维
-            if np.all(shape):
-                arr = np.repeat(arr, shape[i], axis=axis) # 在axis轴上复制操作【广播】
+        assert repeat or np.all(shape)
+        if isinstance(shape, Number): shape = [shape]
+        if axis >= 0: shape = np.flip(shape)
+        if not repeat: repeat = 1
+        
+        for _ in range(repeat):
+            for i in range(np.size(shape)):
+                arr = np.expand_dims(arr, axis=axis) # 扩维
+                if np.all(shape):
+                    arr = np.repeat(arr, shape[i], axis=axis) # 在axis轴上复制操作【广播】
         return arr
 
     @property
     def origin(self) -> tuple:
         """获取原点位置
         """
         return self._origin # (3)
```

### Comparing `vlppy-0.1.15/vlppy/model/room.py` & `vlppy-0.1.16/vlppy/model/room.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/model/room.pyi` & `vlppy-0.1.16/vlppy/model/room.pyi`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/setting/json_setting.py` & `vlppy-0.1.16/vlppy/setting/json_setting.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/setting/settings.json` & `vlppy-0.1.16/vlppy/setting/settings.json`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/signal/filter.py` & `vlppy-0.1.16/vlppy/signal/filter.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/signal/filter.pyi` & `vlppy-0.1.16/vlppy/signal/filter.pyi`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/signal/plot.py` & `vlppy-0.1.16/vlppy/signal/plot.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy/vis/vis.py` & `vlppy-0.1.16/vlppy/vis/vis.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.15/vlppy.egg-info/PKG-INFO` & `vlppy-0.1.16/vlppy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlppy
-Version: 0.1.15
+Version: 0.1.16
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/vlppy.git
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `vlppy-0.1.15/vlppy.egg-info/SOURCES.txt` & `vlppy-0.1.16/vlppy.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,17 @@
 vlppy/info.pyi
 vlppy.egg-info/PKG-INFO
 vlppy.egg-info/SOURCES.txt
 vlppy.egg-info/dependency_links.txt
 vlppy.egg-info/top_level.txt
 vlppy/demo/README.md
 vlppy/demo/__init__.py
-vlppy/demo/__init__.pyi
 vlppy/demo/demo_filter.py
-vlppy/demo/demo_filter.pyi
 vlppy/demo/demo_main.py
-vlppy/demo/demo_main.pyi
 vlppy/demo/vlp_model.py
-vlppy/demo/vlp_model.pyi
 vlppy/error/__init__.py
 vlppy/error/__init__.pyi
 vlppy/error/error.py
 vlppy/error/error.pyi
 vlppy/io/__init__.py
 vlppy/io/__init__.pyi
 vlppy/io/io.py
```

