# Comparing `tmp/desalsim-1.0.tar.gz` & `tmp/desalsim-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desalsim-1.0.tar", last modified: Wed May  8 12:58:28 2024, max compression
+gzip compressed data, was "desalsim-1.0.1.tar", last modified: Wed May  8 13:06:26 2024, max compression
```

## Comparing `desalsim-1.0.tar` & `desalsim-1.0.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 12:58:28.781559 desalsim-1.0/
-drwxrwxrwx   0        0        0        0 2024-05-08 12:58:28.779564 desalsim-1.0/DesalSim.egg-info/
--rw-rw-rw-   0        0        0    10094 2024-05-08 12:58:28.000000 desalsim-1.0/DesalSim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1295 2024-05-08 12:58:28.000000 desalsim-1.0/DesalSim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 12:58:28.000000 desalsim-1.0/DesalSim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-05-08 12:58:28.000000 desalsim-1.0/DesalSim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-08 12:58:28.000000 desalsim-1.0/DesalSim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 12:58:28.743659 desalsim-1.0/Desalsim/
--rw-rw-rw-   0        0        0      786 2024-05-08 06:53:28.000000 desalsim-1.0/Desalsim/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-1.0/Desalsim/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-1.0/Desalsim/density_calc.py
--rw-rw-rw-   0        0        0     8836 2024-05-08 07:40:34.000000 desalsim-1.0/Desalsim/economic_f.py
--rw-rw-rw-   0        0        0     3007 2024-05-08 12:26:00.000000 desalsim-1.0/Desalsim/ed_unit_f.py
--rw-rw-rw-   0        0        0    11748 2024-05-08 08:38:05.000000 desalsim-1.0/Desalsim/edbm_unit_f.py
--rw-rw-rw-   0        0        0    46932 2024-05-08 09:51:24.000000 desalsim-1.0/Desalsim/efc_unit_f.py
--rw-rw-rw-   0        0        0     4504 2024-05-08 07:58:46.000000 desalsim-1.0/Desalsim/med_unit_f.py
--rw-rw-rw-   0        0        0    10067 2024-05-08 12:42:08.000000 desalsim-1.0/Desalsim/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     7011 2024-05-08 07:40:14.000000 desalsim-1.0/Desalsim/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-1.0/Desalsim/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0/Desalsim/scaleup.py
--rw-rw-rw-   0        0        0     8749 2024-05-08 07:58:46.000000 desalsim-1.0/Desalsim/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-1.0/LICENSE
--rw-rw-rw-   0        0        0    10094 2024-05-08 12:58:28.780925 desalsim-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     9618 2024-05-08 07:10:33.000000 desalsim-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 12:58:28.760615 desalsim-1.0/example/
--rw-rw-rw-   0        0        0      786 2024-05-08 06:53:49.000000 desalsim-1.0/example/__init__.py
--rw-rw-rw-   0        0        0     4531 2024-05-08 09:04:36.000000 desalsim-1.0/example/comparison.py
--rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-1.0/example/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-1.0/example/density_calc.py
--rw-rw-rw-   0        0        0    11995 2024-05-08 07:58:46.000000 desalsim-1.0/example/economic_f.py
--rw-rw-rw-   0        0        0     8681 2024-05-08 08:11:06.000000 desalsim-1.0/example/ed_unit_f.py
--rw-rw-rw-   0        0        0    17109 2024-05-08 08:09:55.000000 desalsim-1.0/example/edbm_unit_f.py
--rw-rw-rw-   0        0        0    49455 2024-05-08 09:52:39.000000 desalsim-1.0/example/efc_unit_f.py
--rw-rw-rw-   0        0        0    33308 2024-05-08 07:58:46.000000 desalsim-1.0/example/example_1.py
--rw-rw-rw-   0        0        0    21717 2024-05-08 07:58:46.000000 desalsim-1.0/example/example_2.py
--rw-rw-rw-   0        0        0     8542 2024-05-08 07:58:46.000000 desalsim-1.0/example/med_unit_f.py
--rw-rw-rw-   0        0        0    14939 2024-05-08 07:58:46.000000 desalsim-1.0/example/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     9445 2024-05-08 07:58:46.000000 desalsim-1.0/example/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     7020 2024-05-08 07:58:46.000000 desalsim-1.0/example/ro_unit.py
--rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-1.0/example/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0/example/scaleup.py
--rw-rw-rw-   0        0        0    12280 2024-05-08 08:07:20.000000 desalsim-1.0/example/thermal_cryst_f.py
--rw-rw-rw-   0        0        0       42 2024-05-08 12:58:28.781559 desalsim-1.0/setup.cfg
--rw-rw-rw-   0        0        0      809 2024-05-08 12:58:06.000000 desalsim-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:58:28.778567 desalsim-1.0/tests/
--rw-rw-rw-   0        0        0      790 2024-05-08 06:54:08.000000 desalsim-1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-1.0/tests/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-1.0/tests/density_calc.py
--rw-rw-rw-   0        0        0     9108 2024-05-08 07:58:46.000000 desalsim-1.0/tests/economic_f.py
--rw-rw-rw-   0        0        0     2060 2024-05-08 12:33:36.000000 desalsim-1.0/tests/economic_unittest.py
--rw-rw-rw-   0        0        0     3040 2024-05-08 12:31:10.000000 desalsim-1.0/tests/ed_unit_f.py
--rw-rw-rw-   0        0        0     3249 2024-05-08 12:30:44.000000 desalsim-1.0/tests/ed_unittest.py
--rw-rw-rw-   0        0        0    12683 2024-05-08 08:13:45.000000 desalsim-1.0/tests/edbm_unit_f.py
--rw-rw-rw-   0        0        0     8395 2024-05-08 07:58:46.000000 desalsim-1.0/tests/edbm_unittest.py
--rw-rw-rw-   0        0        0     4508 2024-05-08 07:58:46.000000 desalsim-1.0/tests/med_unit_f.py
--rw-rw-rw-   0        0        0     1564 2024-05-08 07:58:46.000000 desalsim-1.0/tests/med_unittest.py
--rw-rw-rw-   0        0        0    10426 2024-05-08 07:58:46.000000 desalsim-1.0/tests/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     2752 2024-05-08 07:58:46.000000 desalsim-1.0/tests/mfpfr_unittest.py
--rw-rw-rw-   0        0        0     6984 2024-05-08 07:58:46.000000 desalsim-1.0/tests/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     1786 2024-05-08 07:58:46.000000 desalsim-1.0/tests/nanofiltration_unittest.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0/tests/scaleup.py
--rw-rw-rw-   0        0        0     8730 2024-05-08 08:01:54.000000 desalsim-1.0/tests/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     4611 2024-05-08 08:01:32.000000 desalsim-1.0/tests/thermal_cryst_unittest.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:06:26.157386 desalsim-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-05-08 13:06:26.156390 desalsim-1.0.1/DesalSim.egg-info/
+-rw-rw-rw-   0        0        0    10098 2024-05-08 13:06:26.000000 desalsim-1.0.1/DesalSim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1295 2024-05-08 13:06:26.000000 desalsim-1.0.1/DesalSim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 13:06:26.000000 desalsim-1.0.1/DesalSim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-05-08 13:06:26.000000 desalsim-1.0.1/DesalSim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-08 13:06:26.000000 desalsim-1.0.1/DesalSim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 13:06:26.121482 desalsim-1.0.1/Desalsim/
+-rw-rw-rw-   0        0        0      786 2024-05-08 06:53:28.000000 desalsim-1.0.1/Desalsim/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-1.0.1/Desalsim/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-1.0.1/Desalsim/density_calc.py
+-rw-rw-rw-   0        0        0     8836 2024-05-08 07:40:34.000000 desalsim-1.0.1/Desalsim/economic_f.py
+-rw-rw-rw-   0        0        0     3007 2024-05-08 12:26:00.000000 desalsim-1.0.1/Desalsim/ed_unit_f.py
+-rw-rw-rw-   0        0        0    11748 2024-05-08 08:38:05.000000 desalsim-1.0.1/Desalsim/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    46932 2024-05-08 09:51:24.000000 desalsim-1.0.1/Desalsim/efc_unit_f.py
+-rw-rw-rw-   0        0        0     4504 2024-05-08 07:58:46.000000 desalsim-1.0.1/Desalsim/med_unit_f.py
+-rw-rw-rw-   0        0        0    10067 2024-05-08 12:42:08.000000 desalsim-1.0.1/Desalsim/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     7011 2024-05-08 07:40:14.000000 desalsim-1.0.1/Desalsim/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-1.0.1/Desalsim/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0.1/Desalsim/scaleup.py
+-rw-rw-rw-   0        0        0     8749 2024-05-08 07:58:46.000000 desalsim-1.0.1/Desalsim/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    10098 2024-05-08 13:06:26.157252 desalsim-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9620 2024-05-08 13:01:14.000000 desalsim-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 13:06:26.137440 desalsim-1.0.1/example/
+-rw-rw-rw-   0        0        0      786 2024-05-08 06:53:49.000000 desalsim-1.0.1/example/__init__.py
+-rw-rw-rw-   0        0        0     4531 2024-05-08 09:04:36.000000 desalsim-1.0.1/example/comparison.py
+-rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-1.0.1/example/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-1.0.1/example/density_calc.py
+-rw-rw-rw-   0        0        0    11995 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/economic_f.py
+-rw-rw-rw-   0        0        0     8681 2024-05-08 08:11:06.000000 desalsim-1.0.1/example/ed_unit_f.py
+-rw-rw-rw-   0        0        0    17109 2024-05-08 08:09:55.000000 desalsim-1.0.1/example/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    49455 2024-05-08 09:52:39.000000 desalsim-1.0.1/example/efc_unit_f.py
+-rw-rw-rw-   0        0        0    33308 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/example_1.py
+-rw-rw-rw-   0        0        0    21717 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/example_2.py
+-rw-rw-rw-   0        0        0     8542 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/med_unit_f.py
+-rw-rw-rw-   0        0        0    14939 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     9445 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     7020 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/ro_unit.py
+-rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0.1/example/scaleup.py
+-rw-rw-rw-   0        0        0    12280 2024-05-08 08:07:20.000000 desalsim-1.0.1/example/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 13:06:26.157386 desalsim-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-05-08 13:06:16.000000 desalsim-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:06:26.155391 desalsim-1.0.1/tests/
+-rw-rw-rw-   0        0        0      790 2024-05-08 06:54:08.000000 desalsim-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-1.0.1/tests/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-1.0.1/tests/density_calc.py
+-rw-rw-rw-   0        0        0     9108 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/economic_f.py
+-rw-rw-rw-   0        0        0     2060 2024-05-08 12:33:36.000000 desalsim-1.0.1/tests/economic_unittest.py
+-rw-rw-rw-   0        0        0     3040 2024-05-08 12:31:10.000000 desalsim-1.0.1/tests/ed_unit_f.py
+-rw-rw-rw-   0        0        0     3249 2024-05-08 12:30:44.000000 desalsim-1.0.1/tests/ed_unittest.py
+-rw-rw-rw-   0        0        0    12683 2024-05-08 08:13:45.000000 desalsim-1.0.1/tests/edbm_unit_f.py
+-rw-rw-rw-   0        0        0     8395 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/edbm_unittest.py
+-rw-rw-rw-   0        0        0     4508 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/med_unit_f.py
+-rw-rw-rw-   0        0        0     1564 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/med_unittest.py
+-rw-rw-rw-   0        0        0    10426 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     2752 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/mfpfr_unittest.py
+-rw-rw-rw-   0        0        0     6984 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     1786 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/nanofiltration_unittest.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0.1/tests/scaleup.py
+-rw-rw-rw-   0        0        0     8730 2024-05-08 08:01:54.000000 desalsim-1.0.1/tests/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0     4611 2024-05-08 08:01:32.000000 desalsim-1.0.1/tests/thermal_cryst_unittest.py
```

### Comparing `desalsim-1.0/DesalSim.egg-info/PKG-INFO` & `desalsim-1.0.1/DesalSim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DesalSim
-Version: 1.0
+Version: 1.0.1
 Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 Author: rodoulak
 Author-email: r.ktori@tudelft.nl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.0
@@ -66,15 +66,15 @@
 - `density_calc.py`: This file contains the main script for calculating density of a solution based on the tempretaure and the concentration of the solution.
 - `scaleup.py`: This file contains the main script for scaling-up a technology with known capacity using the six-tenths factor rule (m=0.6).
 - `LICENSE`: License file containing the MIT License terms.
 
 ## Installation  
 The easiest way is through pip, in command-line interface:   
 ```
-pip install DesalSim==0.7
+pip install DesalSim==1.0.1
 ```
 
 If you want to install the latest GitHub verstion:
 1. Download the repository to your local machine:
 ```
 https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 ```
```

### Comparing `desalsim-1.0/DesalSim.egg-info/SOURCES.txt` & `desalsim-1.0.1/DesalSim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/Desalsim/__init__.py` & `desalsim-1.0.1/Desalsim/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/Desalsim/constants.py` & `desalsim-1.0.1/Desalsim/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/Desalsim/economic_f.py` & `desalsim-1.0.1/Desalsim/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/Desalsim/ed_unit_f.py` & `desalsim-1.0.1/Desalsim/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/Desalsim/edbm_unit_f.py` & `desalsim-1.0.1/Desalsim/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/Desalsim/efc_unit_f.py` & `desalsim-1.0.1/Desalsim/efc_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/Desalsim/med_unit_f.py` & `desalsim-1.0.1/Desalsim/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/Desalsim/mfpfr_unit_f.py` & `desalsim-1.0.1/Desalsim/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/Desalsim/nanofiltration_unit_f.py` & `desalsim-1.0.1/Desalsim/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/Desalsim/ro_unit_f.py` & `desalsim-1.0.1/Desalsim/ro_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/Desalsim/thermal_cryst_f.py` & `desalsim-1.0.1/Desalsim/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/LICENSE` & `desalsim-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/PKG-INFO` & `desalsim-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DesalSim
-Version: 1.0
+Version: 1.0.1
 Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 Author: rodoulak
 Author-email: r.ktori@tudelft.nl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.0
@@ -66,15 +66,15 @@
 - `density_calc.py`: This file contains the main script for calculating density of a solution based on the tempretaure and the concentration of the solution.
 - `scaleup.py`: This file contains the main script for scaling-up a technology with known capacity using the six-tenths factor rule (m=0.6).
 - `LICENSE`: License file containing the MIT License terms.
 
 ## Installation  
 The easiest way is through pip, in command-line interface:   
 ```
-pip install DesalSim==0.7
+pip install DesalSim==1.0.1
 ```
 
 If you want to install the latest GitHub verstion:
 1. Download the repository to your local machine:
 ```
 https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 ```
```

### Comparing `desalsim-1.0/README.md` & `desalsim-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 - `density_calc.py`: This file contains the main script for calculating density of a solution based on the tempretaure and the concentration of the solution.
 - `scaleup.py`: This file contains the main script for scaling-up a technology with known capacity using the six-tenths factor rule (m=0.6).
 - `LICENSE`: License file containing the MIT License terms.
 
 ## Installation  
 The easiest way is through pip, in command-line interface:   
 ```
-pip install DesalSim==0.7
+pip install DesalSim==1.0.1
 ```
 
 If you want to install the latest GitHub verstion:
 1. Download the repository to your local machine:
 ```
 https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 ```
```

### Comparing `desalsim-1.0/example/__init__.py` & `desalsim-1.0.1/example/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/example/comparison.py` & `desalsim-1.0.1/example/comparison.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/example/constants.py` & `desalsim-1.0.1/example/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/example/economic_f.py` & `desalsim-1.0.1/example/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/example/ed_unit_f.py` & `desalsim-1.0.1/example/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/example/edbm_unit_f.py` & `desalsim-1.0.1/example/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/example/efc_unit_f.py` & `desalsim-1.0.1/example/efc_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/example/example_1.py` & `desalsim-1.0.1/example/example_1.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/example/example_2.py` & `desalsim-1.0.1/example/example_2.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/example/med_unit_f.py` & `desalsim-1.0.1/example/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/example/mfpfr_unit_f.py` & `desalsim-1.0.1/example/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/example/nanofiltration_unit_f.py` & `desalsim-1.0.1/example/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/example/ro_unit.py` & `desalsim-1.0.1/example/ro_unit.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/example/ro_unit_f.py` & `desalsim-1.0.1/example/ro_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/example/thermal_cryst_f.py` & `desalsim-1.0.1/example/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/setup.py` & `desalsim-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f: 
     description =f.read()
 
 setup(
       name='DesalSim',
-      version='1.0',
+      version='1.0.1',
       packages=find_packages(),
       url="https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-",
       author="rodoulak",
       author_email="r.ktori@tudelft.nl",
       license="MIT",
       install_requires=[
           "numpy>=1.0",
@@ -20,8 +20,8 @@
           "matplotlib>=1.0", # For figures 
           "scikit-learn>=1.0",
           "plotly>=1.0", 
           "openpyxl>=1.0",  #read data from excel file
       ],
       long_description= description,
       long_description_content_type="text/markdown",
-      )
+      )
```

### Comparing `desalsim-1.0/tests/__init__.py` & `desalsim-1.0.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/tests/constants.py` & `desalsim-1.0.1/tests/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/tests/economic_f.py` & `desalsim-1.0.1/tests/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/tests/economic_unittest.py` & `desalsim-1.0.1/tests/economic_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/tests/ed_unit_f.py` & `desalsim-1.0.1/tests/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/tests/ed_unittest.py` & `desalsim-1.0.1/tests/ed_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/tests/edbm_unit_f.py` & `desalsim-1.0.1/tests/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/tests/edbm_unittest.py` & `desalsim-1.0.1/tests/edbm_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/tests/med_unit_f.py` & `desalsim-1.0.1/tests/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/tests/med_unittest.py` & `desalsim-1.0.1/tests/med_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/tests/mfpfr_unit_f.py` & `desalsim-1.0.1/tests/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/tests/mfpfr_unittest.py` & `desalsim-1.0.1/tests/mfpfr_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/tests/nanofiltration_unit_f.py` & `desalsim-1.0.1/tests/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/tests/nanofiltration_unittest.py` & `desalsim-1.0.1/tests/nanofiltration_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/tests/thermal_cryst_f.py` & `desalsim-1.0.1/tests/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0/tests/thermal_cryst_unittest.py` & `desalsim-1.0.1/tests/thermal_cryst_unittest.py`

 * *Files identical despite different names*

