# Comparing `tmp/desalsim-0.7.3.tar.gz` & `tmp/desalsim-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desalsim-0.7.3.tar", last modified: Wed May  8 12:36:23 2024, max compression
+gzip compressed data, was "desalsim-0.7.4.tar", last modified: Wed May  8 12:45:11 2024, max compression
```

## Comparing `desalsim-0.7.3.tar` & `desalsim-0.7.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 12:36:23.792408 desalsim-0.7.3/
-drwxrwxrwx   0        0        0        0 2024-05-08 12:36:23.789924 desalsim-0.7.3/DesalSim.egg-info/
--rw-rw-rw-   0        0        0    10096 2024-05-08 12:36:23.000000 desalsim-0.7.3/DesalSim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1295 2024-05-08 12:36:23.000000 desalsim-0.7.3/DesalSim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 12:36:23.000000 desalsim-0.7.3/DesalSim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-05-08 12:36:23.000000 desalsim-0.7.3/DesalSim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-08 12:36:23.000000 desalsim-0.7.3/DesalSim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 12:36:23.738947 desalsim-0.7.3/Desalsim/
--rw-rw-rw-   0        0        0      786 2024-05-08 06:53:28.000000 desalsim-0.7.3/Desalsim/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.7.3/Desalsim/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.3/Desalsim/density_calc.py
--rw-rw-rw-   0        0        0     8836 2024-05-08 07:40:34.000000 desalsim-0.7.3/Desalsim/economic_f.py
--rw-rw-rw-   0        0        0     3007 2024-05-08 12:26:00.000000 desalsim-0.7.3/Desalsim/ed_unit_f.py
--rw-rw-rw-   0        0        0    11748 2024-05-08 08:38:05.000000 desalsim-0.7.3/Desalsim/edbm_unit_f.py
--rw-rw-rw-   0        0        0    46932 2024-05-08 09:51:24.000000 desalsim-0.7.3/Desalsim/efc_unit_f.py
--rw-rw-rw-   0        0        0     4504 2024-05-08 07:58:46.000000 desalsim-0.7.3/Desalsim/med_unit_f.py
--rw-rw-rw-   0        0        0    10088 2024-05-08 07:58:46.000000 desalsim-0.7.3/Desalsim/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     7011 2024-05-08 07:40:14.000000 desalsim-0.7.3/Desalsim/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-0.7.3/Desalsim/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.3/Desalsim/scaleup.py
--rw-rw-rw-   0        0        0     8749 2024-05-08 07:58:46.000000 desalsim-0.7.3/Desalsim/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-0.7.3/LICENSE
--rw-rw-rw-   0        0        0    10096 2024-05-08 12:36:23.791035 desalsim-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     9618 2024-05-08 07:10:33.000000 desalsim-0.7.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 12:36:23.763409 desalsim-0.7.3/example/
--rw-rw-rw-   0        0        0      786 2024-05-08 06:53:49.000000 desalsim-0.7.3/example/__init__.py
--rw-rw-rw-   0        0        0     4531 2024-05-08 09:04:36.000000 desalsim-0.7.3/example/comparison.py
--rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-0.7.3/example/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.3/example/density_calc.py
--rw-rw-rw-   0        0        0    11995 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/economic_f.py
--rw-rw-rw-   0        0        0     8681 2024-05-08 08:11:06.000000 desalsim-0.7.3/example/ed_unit_f.py
--rw-rw-rw-   0        0        0    17109 2024-05-08 08:09:55.000000 desalsim-0.7.3/example/edbm_unit_f.py
--rw-rw-rw-   0        0        0    49455 2024-05-08 09:52:39.000000 desalsim-0.7.3/example/efc_unit_f.py
--rw-rw-rw-   0        0        0    33308 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/example_1.py
--rw-rw-rw-   0        0        0    21717 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/example_2.py
--rw-rw-rw-   0        0        0     8542 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/med_unit_f.py
--rw-rw-rw-   0        0        0    14939 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     9445 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     7020 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/ro_unit.py
--rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.3/example/scaleup.py
--rw-rw-rw-   0        0        0    12280 2024-05-08 08:07:20.000000 desalsim-0.7.3/example/thermal_cryst_f.py
--rw-rw-rw-   0        0        0       42 2024-05-08 12:36:23.792909 desalsim-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0      811 2024-05-08 12:36:17.000000 desalsim-0.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:36:23.788087 desalsim-0.7.3/tests/
--rw-rw-rw-   0        0        0      790 2024-05-08 06:54:08.000000 desalsim-0.7.3/tests/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.7.3/tests/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.3/tests/density_calc.py
--rw-rw-rw-   0        0        0     9108 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/economic_f.py
--rw-rw-rw-   0        0        0     2060 2024-05-08 12:33:36.000000 desalsim-0.7.3/tests/economic_unittest.py
--rw-rw-rw-   0        0        0     3040 2024-05-08 12:31:10.000000 desalsim-0.7.3/tests/ed_unit_f.py
--rw-rw-rw-   0        0        0     3249 2024-05-08 12:30:44.000000 desalsim-0.7.3/tests/ed_unittest.py
--rw-rw-rw-   0        0        0    12683 2024-05-08 08:13:45.000000 desalsim-0.7.3/tests/edbm_unit_f.py
--rw-rw-rw-   0        0        0     8395 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/edbm_unittest.py
--rw-rw-rw-   0        0        0     4508 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/med_unit_f.py
--rw-rw-rw-   0        0        0     1564 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/med_unittest.py
--rw-rw-rw-   0        0        0    10426 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     2752 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/mfpfr_unittest.py
--rw-rw-rw-   0        0        0     6984 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     1786 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/nanofiltration_unittest.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.3/tests/scaleup.py
--rw-rw-rw-   0        0        0     8730 2024-05-08 08:01:54.000000 desalsim-0.7.3/tests/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     4611 2024-05-08 08:01:32.000000 desalsim-0.7.3/tests/thermal_cryst_unittest.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:45:11.384623 desalsim-0.7.4/
+drwxrwxrwx   0        0        0        0 2024-05-08 12:45:11.382629 desalsim-0.7.4/DesalSim.egg-info/
+-rw-rw-rw-   0        0        0    10096 2024-05-08 12:45:11.000000 desalsim-0.7.4/DesalSim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1295 2024-05-08 12:45:11.000000 desalsim-0.7.4/DesalSim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 12:45:11.000000 desalsim-0.7.4/DesalSim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-05-08 12:45:11.000000 desalsim-0.7.4/DesalSim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-08 12:45:11.000000 desalsim-0.7.4/DesalSim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 12:45:11.345709 desalsim-0.7.4/Desalsim/
+-rw-rw-rw-   0        0        0      786 2024-05-08 06:53:28.000000 desalsim-0.7.4/Desalsim/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.7.4/Desalsim/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.4/Desalsim/density_calc.py
+-rw-rw-rw-   0        0        0     8836 2024-05-08 07:40:34.000000 desalsim-0.7.4/Desalsim/economic_f.py
+-rw-rw-rw-   0        0        0     3007 2024-05-08 12:26:00.000000 desalsim-0.7.4/Desalsim/ed_unit_f.py
+-rw-rw-rw-   0        0        0    11748 2024-05-08 08:38:05.000000 desalsim-0.7.4/Desalsim/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    46932 2024-05-08 09:51:24.000000 desalsim-0.7.4/Desalsim/efc_unit_f.py
+-rw-rw-rw-   0        0        0     4504 2024-05-08 07:58:46.000000 desalsim-0.7.4/Desalsim/med_unit_f.py
+-rw-rw-rw-   0        0        0    10067 2024-05-08 12:42:08.000000 desalsim-0.7.4/Desalsim/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     7011 2024-05-08 07:40:14.000000 desalsim-0.7.4/Desalsim/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-0.7.4/Desalsim/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.4/Desalsim/scaleup.py
+-rw-rw-rw-   0        0        0     8749 2024-05-08 07:58:46.000000 desalsim-0.7.4/Desalsim/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-0.7.4/LICENSE
+-rw-rw-rw-   0        0        0    10096 2024-05-08 12:45:11.383625 desalsim-0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9618 2024-05-08 07:10:33.000000 desalsim-0.7.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 12:45:11.363662 desalsim-0.7.4/example/
+-rw-rw-rw-   0        0        0      786 2024-05-08 06:53:49.000000 desalsim-0.7.4/example/__init__.py
+-rw-rw-rw-   0        0        0     4531 2024-05-08 09:04:36.000000 desalsim-0.7.4/example/comparison.py
+-rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-0.7.4/example/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.4/example/density_calc.py
+-rw-rw-rw-   0        0        0    11995 2024-05-08 07:58:46.000000 desalsim-0.7.4/example/economic_f.py
+-rw-rw-rw-   0        0        0     8681 2024-05-08 08:11:06.000000 desalsim-0.7.4/example/ed_unit_f.py
+-rw-rw-rw-   0        0        0    17109 2024-05-08 08:09:55.000000 desalsim-0.7.4/example/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    49455 2024-05-08 09:52:39.000000 desalsim-0.7.4/example/efc_unit_f.py
+-rw-rw-rw-   0        0        0    33308 2024-05-08 07:58:46.000000 desalsim-0.7.4/example/example_1.py
+-rw-rw-rw-   0        0        0    21717 2024-05-08 07:58:46.000000 desalsim-0.7.4/example/example_2.py
+-rw-rw-rw-   0        0        0     8542 2024-05-08 07:58:46.000000 desalsim-0.7.4/example/med_unit_f.py
+-rw-rw-rw-   0        0        0    14939 2024-05-08 07:58:46.000000 desalsim-0.7.4/example/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     9445 2024-05-08 07:58:46.000000 desalsim-0.7.4/example/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     7020 2024-05-08 07:58:46.000000 desalsim-0.7.4/example/ro_unit.py
+-rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-0.7.4/example/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.4/example/scaleup.py
+-rw-rw-rw-   0        0        0    12280 2024-05-08 08:07:20.000000 desalsim-0.7.4/example/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 12:45:11.384623 desalsim-0.7.4/setup.cfg
+-rw-rw-rw-   0        0        0      811 2024-05-08 12:45:02.000000 desalsim-0.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:45:11.381631 desalsim-0.7.4/tests/
+-rw-rw-rw-   0        0        0      790 2024-05-08 06:54:08.000000 desalsim-0.7.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.7.4/tests/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.4/tests/density_calc.py
+-rw-rw-rw-   0        0        0     9108 2024-05-08 07:58:46.000000 desalsim-0.7.4/tests/economic_f.py
+-rw-rw-rw-   0        0        0     2060 2024-05-08 12:33:36.000000 desalsim-0.7.4/tests/economic_unittest.py
+-rw-rw-rw-   0        0        0     3040 2024-05-08 12:31:10.000000 desalsim-0.7.4/tests/ed_unit_f.py
+-rw-rw-rw-   0        0        0     3249 2024-05-08 12:30:44.000000 desalsim-0.7.4/tests/ed_unittest.py
+-rw-rw-rw-   0        0        0    12683 2024-05-08 08:13:45.000000 desalsim-0.7.4/tests/edbm_unit_f.py
+-rw-rw-rw-   0        0        0     8395 2024-05-08 07:58:46.000000 desalsim-0.7.4/tests/edbm_unittest.py
+-rw-rw-rw-   0        0        0     4508 2024-05-08 07:58:46.000000 desalsim-0.7.4/tests/med_unit_f.py
+-rw-rw-rw-   0        0        0     1564 2024-05-08 07:58:46.000000 desalsim-0.7.4/tests/med_unittest.py
+-rw-rw-rw-   0        0        0    10426 2024-05-08 07:58:46.000000 desalsim-0.7.4/tests/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     2752 2024-05-08 07:58:46.000000 desalsim-0.7.4/tests/mfpfr_unittest.py
+-rw-rw-rw-   0        0        0     6984 2024-05-08 07:58:46.000000 desalsim-0.7.4/tests/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     1786 2024-05-08 07:58:46.000000 desalsim-0.7.4/tests/nanofiltration_unittest.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.4/tests/scaleup.py
+-rw-rw-rw-   0        0        0     8730 2024-05-08 08:01:54.000000 desalsim-0.7.4/tests/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0     4611 2024-05-08 08:01:32.000000 desalsim-0.7.4/tests/thermal_cryst_unittest.py
```

### Comparing `desalsim-0.7.3/DesalSim.egg-info/PKG-INFO` & `desalsim-0.7.4/DesalSim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DesalSim
-Version: 0.7.3
+Version: 0.7.4
 Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 Author: rodoulak
 Author-email: r.ktori@tudelft.nl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.0
```

### Comparing `desalsim-0.7.3/DesalSim.egg-info/SOURCES.txt` & `desalsim-0.7.4/DesalSim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/Desalsim/__init__.py` & `desalsim-0.7.4/Desalsim/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/Desalsim/constants.py` & `desalsim-0.7.4/Desalsim/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/Desalsim/economic_f.py` & `desalsim-0.7.4/Desalsim/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/Desalsim/ed_unit_f.py` & `desalsim-0.7.4/Desalsim/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/Desalsim/edbm_unit_f.py` & `desalsim-0.7.4/Desalsim/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/Desalsim/efc_unit_f.py` & `desalsim-0.7.4/Desalsim/efc_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/Desalsim/med_unit_f.py` & `desalsim-0.7.4/Desalsim/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/Desalsim/mfpfr_unit_f.py` & `desalsim-0.7.4/Desalsim/mfpfr_unit_f.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import math
-import density_calc
 from Desalsim import scaleup
 from Desalsim.density_calc import density_calc 
 import math
 from Desalsim import constants 
 #%%
     #molecular weight
 MW_Na=constants.MW_Na
```

### Comparing `desalsim-0.7.3/Desalsim/nanofiltration_unit_f.py` & `desalsim-0.7.4/Desalsim/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/Desalsim/ro_unit_f.py` & `desalsim-0.7.4/Desalsim/ro_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/Desalsim/thermal_cryst_f.py` & `desalsim-0.7.4/Desalsim/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/LICENSE` & `desalsim-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/PKG-INFO` & `desalsim-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DesalSim
-Version: 0.7.3
+Version: 0.7.4
 Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 Author: rodoulak
 Author-email: r.ktori@tudelft.nl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.0
```

### Comparing `desalsim-0.7.3/README.md` & `desalsim-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/example/__init__.py` & `desalsim-0.7.4/example/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/example/comparison.py` & `desalsim-0.7.4/example/comparison.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/example/constants.py` & `desalsim-0.7.4/example/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/example/economic_f.py` & `desalsim-0.7.4/example/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/example/ed_unit_f.py` & `desalsim-0.7.4/example/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/example/edbm_unit_f.py` & `desalsim-0.7.4/example/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/example/efc_unit_f.py` & `desalsim-0.7.4/example/efc_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/example/example_1.py` & `desalsim-0.7.4/example/example_1.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/example/example_2.py` & `desalsim-0.7.4/example/example_2.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/example/med_unit_f.py` & `desalsim-0.7.4/example/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/example/mfpfr_unit_f.py` & `desalsim-0.7.4/example/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/example/nanofiltration_unit_f.py` & `desalsim-0.7.4/example/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/example/ro_unit.py` & `desalsim-0.7.4/example/ro_unit.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/example/ro_unit_f.py` & `desalsim-0.7.4/example/ro_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/example/thermal_cryst_f.py` & `desalsim-0.7.4/example/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/setup.py` & `desalsim-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f: 
     description =f.read()
 
 setup(
       name='DesalSim',
-      version='0.7.3',
+      version='0.7.4',
       packages=find_packages(),
       url="https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-",
       author="rodoulak",
       author_email="r.ktori@tudelft.nl",
       license="MIT",
       install_requires=[
           "numpy>=1.0",
```

### Comparing `desalsim-0.7.3/tests/__init__.py` & `desalsim-0.7.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/tests/constants.py` & `desalsim-0.7.4/tests/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/tests/economic_f.py` & `desalsim-0.7.4/tests/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/tests/economic_unittest.py` & `desalsim-0.7.4/tests/economic_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/tests/ed_unit_f.py` & `desalsim-0.7.4/tests/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/tests/ed_unittest.py` & `desalsim-0.7.4/tests/ed_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/tests/edbm_unit_f.py` & `desalsim-0.7.4/tests/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/tests/edbm_unittest.py` & `desalsim-0.7.4/tests/edbm_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/tests/med_unit_f.py` & `desalsim-0.7.4/tests/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/tests/med_unittest.py` & `desalsim-0.7.4/tests/med_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/tests/mfpfr_unit_f.py` & `desalsim-0.7.4/tests/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/tests/mfpfr_unittest.py` & `desalsim-0.7.4/tests/mfpfr_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/tests/nanofiltration_unit_f.py` & `desalsim-0.7.4/tests/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/tests/nanofiltration_unittest.py` & `desalsim-0.7.4/tests/nanofiltration_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/tests/thermal_cryst_f.py` & `desalsim-0.7.4/tests/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.3/tests/thermal_cryst_unittest.py` & `desalsim-0.7.4/tests/thermal_cryst_unittest.py`

 * *Files identical despite different names*

