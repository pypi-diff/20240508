# Comparing `tmp/desalsim-0.7.2.tar.gz` & `tmp/desalsim-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desalsim-0.7.2.tar", last modified: Wed May  8 07:34:08 2024, max compression
+gzip compressed data, was "desalsim-0.7.3.tar", last modified: Wed May  8 12:36:23 2024, max compression
```

## Comparing `desalsim-0.7.2.tar` & `desalsim-0.7.3.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 07:34:08.887733 desalsim-0.7.2/
-drwxrwxrwx   0        0        0        0 2024-05-08 07:34:08.883504 desalsim-0.7.2/DesalSim.egg-info/
--rw-rw-rw-   0        0        0     9945 2024-05-08 07:34:08.000000 desalsim-0.7.2/DesalSim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1276 2024-05-08 07:34:08.000000 desalsim-0.7.2/DesalSim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 07:34:08.000000 desalsim-0.7.2/DesalSim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-08 07:34:08.000000 desalsim-0.7.2/DesalSim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-08 07:34:08.000000 desalsim-0.7.2/DesalSim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 07:34:08.799259 desalsim-0.7.2/Desalsim/
--rw-rw-rw-   0        0        0      786 2024-05-08 06:54:35.000000 desalsim-0.7.2/Desalsim/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.7.2/Desalsim/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.2/Desalsim/density_calc.py
--rw-rw-rw-   0        0        0     8821 2024-05-06 16:12:13.000000 desalsim-0.7.2/Desalsim/economic_f.py
--rw-rw-rw-   0        0        0     2950 2024-04-29 20:32:39.000000 desalsim-0.7.2/Desalsim/ed_unit_f.py
--rw-rw-rw-   0        0        0    11744 2024-04-29 21:17:33.000000 desalsim-0.7.2/Desalsim/edbm_unit_f.py
--rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.7.2/Desalsim/efc_unit_f.py
--rw-rw-rw-   0        0        0     4494 2024-04-29 20:24:16.000000 desalsim-0.7.2/Desalsim/med_unit_f.py
--rw-rw-rw-   0        0        0    10049 2024-04-29 21:14:03.000000 desalsim-0.7.2/Desalsim/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     6997 2024-05-08 07:33:43.000000 desalsim-0.7.2/Desalsim/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.7.2/Desalsim/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.2/Desalsim/scaleup.py
--rw-rw-rw-   0        0        0     8692 2024-04-29 19:44:35.000000 desalsim-0.7.2/Desalsim/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-0.7.2/LICENSE
--rw-rw-rw-   0        0        0     9945 2024-05-08 07:34:08.885680 desalsim-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     9618 2024-05-08 07:10:33.000000 desalsim-0.7.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 07:34:08.837142 desalsim-0.7.2/example/
--rw-rw-rw-   0        0        0      786 2024-05-08 06:57:43.000000 desalsim-0.7.2/example/__init__.py
--rw-rw-rw-   0        0        0     4531 2024-04-11 13:19:36.000000 desalsim-0.7.2/example/comparison.py
--rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-0.7.2/example/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.2/example/density_calc.py
--rw-rw-rw-   0        0        0    11978 2024-05-06 16:09:51.000000 desalsim-0.7.2/example/economic_f.py
--rw-rw-rw-   0        0        0     8663 2024-04-29 21:33:04.000000 desalsim-0.7.2/example/ed_unit_f.py
--rw-rw-rw-   0        0        0    17118 2024-04-29 21:35:34.000000 desalsim-0.7.2/example/edbm_unit_f.py
--rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.7.2/example/efc_unit_f.py
--rw-rw-rw-   0        0        0    33181 2024-05-06 17:04:03.000000 desalsim-0.7.2/example/example_1.py
--rw-rw-rw-   0        0        0    21599 2024-05-06 16:29:23.000000 desalsim-0.7.2/example/example_2.py
--rw-rw-rw-   0        0        0     8532 2024-04-29 21:36:53.000000 desalsim-0.7.2/example/med_unit_f.py
--rw-rw-rw-   0        0        0    14921 2024-05-03 08:06:32.000000 desalsim-0.7.2/example/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     9421 2024-05-06 08:39:39.000000 desalsim-0.7.2/example/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.7.2/example/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.2/example/scaleup.py
--rw-rw-rw-   0        0        0    12262 2024-04-29 21:44:17.000000 desalsim-0.7.2/example/thermal_cryst_f.py
--rw-rw-rw-   0        0        0       42 2024-05-08 07:34:08.888490 desalsim-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0      611 2024-05-08 07:33:59.000000 desalsim-0.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:34:08.880512 desalsim-0.7.2/tests/
--rw-rw-rw-   0        0        0      790 2024-05-08 06:58:06.000000 desalsim-0.7.2/tests/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.7.2/tests/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.2/tests/density_calc.py
--rw-rw-rw-   0        0        0     9094 2024-05-06 16:12:45.000000 desalsim-0.7.2/tests/economic_f.py
--rw-rw-rw-   0        0        0     2527 2024-05-06 16:15:02.000000 desalsim-0.7.2/tests/economic_unittest.py
--rw-rw-rw-   0        0        0     3255 2024-05-03 14:14:54.000000 desalsim-0.7.2/tests/ed_unit_f.py
--rw-rw-rw-   0        0        0     3316 2024-05-03 14:16:37.000000 desalsim-0.7.2/tests/ed_unittest.py
--rw-rw-rw-   0        0        0    12680 2024-05-03 13:51:25.000000 desalsim-0.7.2/tests/edbm_unit_f.py
--rw-rw-rw-   0        0        0     8386 2024-05-03 13:50:48.000000 desalsim-0.7.2/tests/edbm_unittest.py
--rw-rw-rw-   0        0        0     4496 2024-05-02 14:39:30.000000 desalsim-0.7.2/tests/med_unit_f.py
--rw-rw-rw-   0        0        0     1555 2024-05-03 14:28:38.000000 desalsim-0.7.2/tests/med_unittest.py
--rw-rw-rw-   0        0        0    10407 2024-05-03 12:57:15.000000 desalsim-0.7.2/tests/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     2743 2024-05-03 12:56:18.000000 desalsim-0.7.2/tests/mfpfr_unittest.py
--rw-rw-rw-   0        0        0     6961 2024-05-06 08:40:27.000000 desalsim-0.7.2/tests/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     1777 2024-05-06 08:40:55.000000 desalsim-0.7.2/tests/nanofiltration_unittest.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.2/tests/scaleup.py
--rw-rw-rw-   0        0        0     8687 2024-05-05 10:31:06.000000 desalsim-0.7.2/tests/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     4560 2024-05-05 10:30:42.000000 desalsim-0.7.2/tests/thermal_cryst_unittest.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:36:23.792408 desalsim-0.7.3/
+drwxrwxrwx   0        0        0        0 2024-05-08 12:36:23.789924 desalsim-0.7.3/DesalSim.egg-info/
+-rw-rw-rw-   0        0        0    10096 2024-05-08 12:36:23.000000 desalsim-0.7.3/DesalSim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1295 2024-05-08 12:36:23.000000 desalsim-0.7.3/DesalSim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 12:36:23.000000 desalsim-0.7.3/DesalSim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-05-08 12:36:23.000000 desalsim-0.7.3/DesalSim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-08 12:36:23.000000 desalsim-0.7.3/DesalSim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 12:36:23.738947 desalsim-0.7.3/Desalsim/
+-rw-rw-rw-   0        0        0      786 2024-05-08 06:53:28.000000 desalsim-0.7.3/Desalsim/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.7.3/Desalsim/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.3/Desalsim/density_calc.py
+-rw-rw-rw-   0        0        0     8836 2024-05-08 07:40:34.000000 desalsim-0.7.3/Desalsim/economic_f.py
+-rw-rw-rw-   0        0        0     3007 2024-05-08 12:26:00.000000 desalsim-0.7.3/Desalsim/ed_unit_f.py
+-rw-rw-rw-   0        0        0    11748 2024-05-08 08:38:05.000000 desalsim-0.7.3/Desalsim/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    46932 2024-05-08 09:51:24.000000 desalsim-0.7.3/Desalsim/efc_unit_f.py
+-rw-rw-rw-   0        0        0     4504 2024-05-08 07:58:46.000000 desalsim-0.7.3/Desalsim/med_unit_f.py
+-rw-rw-rw-   0        0        0    10088 2024-05-08 07:58:46.000000 desalsim-0.7.3/Desalsim/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     7011 2024-05-08 07:40:14.000000 desalsim-0.7.3/Desalsim/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-0.7.3/Desalsim/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.3/Desalsim/scaleup.py
+-rw-rw-rw-   0        0        0     8749 2024-05-08 07:58:46.000000 desalsim-0.7.3/Desalsim/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-0.7.3/LICENSE
+-rw-rw-rw-   0        0        0    10096 2024-05-08 12:36:23.791035 desalsim-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9618 2024-05-08 07:10:33.000000 desalsim-0.7.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 12:36:23.763409 desalsim-0.7.3/example/
+-rw-rw-rw-   0        0        0      786 2024-05-08 06:53:49.000000 desalsim-0.7.3/example/__init__.py
+-rw-rw-rw-   0        0        0     4531 2024-05-08 09:04:36.000000 desalsim-0.7.3/example/comparison.py
+-rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-0.7.3/example/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.3/example/density_calc.py
+-rw-rw-rw-   0        0        0    11995 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/economic_f.py
+-rw-rw-rw-   0        0        0     8681 2024-05-08 08:11:06.000000 desalsim-0.7.3/example/ed_unit_f.py
+-rw-rw-rw-   0        0        0    17109 2024-05-08 08:09:55.000000 desalsim-0.7.3/example/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    49455 2024-05-08 09:52:39.000000 desalsim-0.7.3/example/efc_unit_f.py
+-rw-rw-rw-   0        0        0    33308 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/example_1.py
+-rw-rw-rw-   0        0        0    21717 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/example_2.py
+-rw-rw-rw-   0        0        0     8542 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/med_unit_f.py
+-rw-rw-rw-   0        0        0    14939 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     9445 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     7020 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/ro_unit.py
+-rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-0.7.3/example/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.3/example/scaleup.py
+-rw-rw-rw-   0        0        0    12280 2024-05-08 08:07:20.000000 desalsim-0.7.3/example/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 12:36:23.792909 desalsim-0.7.3/setup.cfg
+-rw-rw-rw-   0        0        0      811 2024-05-08 12:36:17.000000 desalsim-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:36:23.788087 desalsim-0.7.3/tests/
+-rw-rw-rw-   0        0        0      790 2024-05-08 06:54:08.000000 desalsim-0.7.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.7.3/tests/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.3/tests/density_calc.py
+-rw-rw-rw-   0        0        0     9108 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/economic_f.py
+-rw-rw-rw-   0        0        0     2060 2024-05-08 12:33:36.000000 desalsim-0.7.3/tests/economic_unittest.py
+-rw-rw-rw-   0        0        0     3040 2024-05-08 12:31:10.000000 desalsim-0.7.3/tests/ed_unit_f.py
+-rw-rw-rw-   0        0        0     3249 2024-05-08 12:30:44.000000 desalsim-0.7.3/tests/ed_unittest.py
+-rw-rw-rw-   0        0        0    12683 2024-05-08 08:13:45.000000 desalsim-0.7.3/tests/edbm_unit_f.py
+-rw-rw-rw-   0        0        0     8395 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/edbm_unittest.py
+-rw-rw-rw-   0        0        0     4508 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/med_unit_f.py
+-rw-rw-rw-   0        0        0     1564 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/med_unittest.py
+-rw-rw-rw-   0        0        0    10426 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     2752 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/mfpfr_unittest.py
+-rw-rw-rw-   0        0        0     6984 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     1786 2024-05-08 07:58:46.000000 desalsim-0.7.3/tests/nanofiltration_unittest.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.3/tests/scaleup.py
+-rw-rw-rw-   0        0        0     8730 2024-05-08 08:01:54.000000 desalsim-0.7.3/tests/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0     4611 2024-05-08 08:01:32.000000 desalsim-0.7.3/tests/thermal_cryst_unittest.py
```

### Comparing `desalsim-0.7.2/DesalSim.egg-info/PKG-INFO` & `desalsim-0.7.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: DesalSim
-Version: 0.7.2
-Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
-Author: rodoulak
-Author-email: r.ktori@tudelft.nl
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.0
-Requires-Dist: pandas>=1.0
-
 # DesalSim: Desalination and Brine Treatment simulation model
 
  
 ## Overview 
 This project comprises a package of simulation models for desalination and brine treatment technologies, including reverse osmosis, nanofiltration, multi-effect distillation, chemical precipitation, eutectic freeze crystallization, electrodialysis, and thermal crystallization. These technologies are utilized for desalination, ion separation, and salt recovery processes in various industrial and environmental applications.
 
 The simulation models implemented here calculate various parameters such as salt concentration profiles, ion fluxes, energy consumption, chemical consumption, and operational costs. They provide insights into the performance and economics of the technologies under different operating conditions and input parameters. Additionally, the models allow for the integration of different technologies in various configurations to optimize process efficiency and resource utilization.
```

### Comparing `desalsim-0.7.2/DesalSim.egg-info/SOURCES.txt` & `desalsim-0.7.3/DesalSim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 example/edbm_unit_f.py
 example/efc_unit_f.py
 example/example_1.py
 example/example_2.py
 example/med_unit_f.py
 example/mfpfr_unit_f.py
 example/nanofiltration_unit_f.py
+example/ro_unit.py
 example/ro_unit_f.py
 example/scaleup.py
 example/thermal_cryst_f.py
 tests/__init__.py
 tests/constants.py
 tests/density_calc.py
 tests/economic_f.py
```

### Comparing `desalsim-0.7.2/Desalsim/__init__.py` & `desalsim-0.7.3/example/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.2/Desalsim/constants.py` & `desalsim-0.7.3/Desalsim/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.2/Desalsim/economic_f.py` & `desalsim-0.7.3/Desalsim/economic_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #costs calculations functions 
-import constants
+from Desalsim import constants 
 #%%
 #symbols:
 #hr-> hours
 #lf -> lifetime 
 #el -> electricity
 #s-> steam
 #pr -> price
```

### Comparing `desalsim-0.7.2/Desalsim/ed_unit_f.py` & `desalsim-0.7.3/tests/ed_unit_f.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
-import scaleup
-import constants
 import math
-import density_calc
+from  Desalsim.density_calc import density_calc
+from Desalsim import constants
+from Desalsim import scaleup
 
 #%% Calculations 
 """
 A class used to represent Mass Balance for Electrodialysis
 
 ...
 
@@ -71,40 +71,41 @@
     dC(Ts_cp): 
         Change in concentration
 """
 class ElectrodialysisCalc:
     def __init__(self):
         pass
 
-    def Ts_cp(S):
+
+    def Ts_cp(self,S):
         """Transport number for salt in concentrate compartment"""
         Ts_cp=-4e-6*S**2 + 4e-5*S + 0.96
         return Ts_cp
     
-    def Tw_cp(Sc,Sd):
+    def Tw_cp(self,Sc,Sd):
         """Transport number for water in concentrate compartment"""
         return -4e-5*Sc**2 - 1.9e-2*Sd + 11.2
     
-    def Ls_cp(Sc, Sd):
+    def Ls_cp(self,Sc, Sd):
         """Permeability for salt in concentrate compartment"""
         return min(2e-12*Sd**2 - 3e-10*Sd + 6e-8, 2e-12*Sc**2 - 3e-10*Sc + 6e-8)
     
-    def Lw_cp(S):
+    def Lw_cp(self,S):
         """Permeability for water in concentrate compartment"""
         return 5*S**(-0.416)
     
     
-    def p_osmo(S, T, MWs): 
+    def p_osmo(self, S, T, MWs): 
         """calculation for Osmotic pressure in concentrate compartment"""
         C1=S/MWs*constants.MW_Na/constants.MW_Na
         C2=S/MWs*constants.MW_cl/constants.MW_cl
         sum_Ci=sum([C1, C2])
         p_osmo=0.0831446261815324*sum_Ci*T
         return p_osmo
     
-    def dC(Ts_cp, tcu, D, Ij,  h, Sh ):
+    def dC(self, Ts_cp, tcu, D, Ij,  h, Sh ):
         """Change in concentration"""
         F = 96485.3329  # Faraday constant (C/mol)
         Tcu=(Ts_cp+1)/2
         dC=-(Tcu-tcu)/D*(Ij/F)*(2*h/1000/Sh)
         return dC
```

### Comparing `desalsim-0.7.2/Desalsim/edbm_unit_f.py` & `desalsim-0.7.3/Desalsim/edbm_unit_f.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math 
 import numpy as np
-import scaleup 
-import density_calc
-import constants
+from Desalsim import scaleup
+from Desalsim.density_calc import density_calc 
+from Desalsim import constants 
 
 #%%
 #Molecular weight 
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
@@ -100,17 +100,17 @@
         self.CCa_s_in=Cc5/MW_Ca #Ca concentration (g/l) to (mol/l)
         self.CSO4_s_in=Cc6/MW_SO4 #SO4 concentration (g/l) to (mol/l)
         self.CHCO3_s_in=Cc6/MW_HCO3 #HCO3 concentration (g/l) to (mol/l)      
         self.COH_s_in=COH/MW_OH
         self.CH_s_in=CH/MW_H
         self.PM_i=[MW_Na, MW_Cl, MW_K, MW_Mg, MW_Ca, MW_SO4, MW_HCO3, MW_H, MW_OH]
         
-        self.d_a=density_calc.density_calc(self.T,sum(C_a_in) )/1000
-        self.d_b=density_calc.density_calc(self.T,sum(C_b_in) )/1000
-        self.d_s=density_calc.density_calc(self.T,sum(C_s_in) )/1000
+        self.d_a=density_calc(self.T,sum(C_a_in) )/1000
+        self.d_b=density_calc(self.T,sum(C_b_in) )/1000
+        self.d_s=density_calc(self.T,sum(C_s_in) )/1000
         
         #Create lists for initial concentration in each channel 
         self.Ci_s_in=[self.CNa_s_in,self.CCl_s_in,self.CK_s_in,self.CMg_s_in,self.CCa_s_in,self.CSO4_s_in,self.CHCO3_s_in, self.CH_s_in,self.COH_s_in]
         self.Ci_b_in=[Cb1/MW_Na, Cb2/ MW_Cl,Cb3/MW_K,Cb4/MW_Mg,Cb5/MW_Ca,Cb6/MW_SO4,Cb7/MW_HCO3,Cb8/MW_H,Cb9/MW_OH]
         self.Ci_a_in=[Ca1/MW_Na,Ca2/MW_Cl,Ca3/MW_K,Ca4/MW_Mg,Ca5/MW_Ca,Ca6/MW_SO4,Ca7/MW_HCO3,Ca8/MW_H,Ca9/MW_OH]
         
         #save initial concentration before recirculation: 
@@ -206,15 +206,15 @@
         self.M_b_out_t=self.M_h2o_b_out+self.M_b_out[7]+self.M_b_out[1]+self.M_b_out[8]+self.M_b_out[0]
  
         #Calculation of outlet mass flow rate for other ionic species in channel 
         for i in range(2,7):
             self.M_b_out[i]=self.M_b_in[i]  
             self.M_b_out_t=self.M_b_out_t+self.M_b_out[i]
             
-        d_s_new=density_calc.density_calc(25, self.M_b_out_t)/1000
+        d_s_new=density_calc(25, self.M_b_out_t)/1000
         #Calculate of volumetric outlet flow rate
         self.Q1_b_out=self.M_b_out_t/d_s_new #assume density is 1kg/l
         
         #Calculation of outlet concentration of single ions in channel 
         for i in range(0,9):
             self.Ci_b_out[i]=self.M_b_out[i]/(self.Q1_b_out*self.PM_i[i]/1000)
```

### Comparing `desalsim-0.7.2/Desalsim/efc_unit_f.py` & `desalsim-0.7.3/example/efc_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,28 +27,28 @@
 
 import time
 import numpy as np
 from scipy import interpolate
 import scipy.interpolate as interpolate
 from sklearn.linear_model import LinearRegression
 from collections import namedtuple
-import scaleup
-import density_calc
+from Desalsim import scaleup
+from Desalsim.density_calc import density_calc 
 # import pitzer_model_3phases_w
-import constants
+from Desalsim import constants 
 #Set initial time to calculate the elapsed time of the calculations
 time0=time.time()
 MW_so4=32.064+4*15.999
 
 #input data
 Qf=100 #m3/hr
 C_i_in=[20.16, 27.87, 0.50, 0.0, 0.12, 14.66]
 
 T_initial =273+25
-d_in=density_calc.density_calc(25, sum(C_i_in))
+d_in=density_calc(25, sum(C_i_in))
 #%%
 
 #Declaration of constant process parameters - Part 1: Process Parameters
 
 Vreactor=Qf/0.7            #Volume of the reactor : m^3
 
 #Influx
@@ -240,31 +240,44 @@
         
     #Initial concentration of Compound 1
     C_compound1_initial=C_Na2SO4_initial
     print("C_compound1_initial is "+str(C_compound1_initial))
     T_Na2SO4_sol_line=[]
     C_Na2SO4_sol_line=[]
     #Interpolation/Extrapolation of the Na2SO4 solubility line with a cubic spline 
-     
+    import os
+    import pandas as pd
+
+    # Get the directory where the script is located
+    current_directory = os.path.dirname(__file__)
+
+    #   Define the filename 
+    filename = "efc_results.xlsx"
+
+    # Combine the directory path with the filename
+    file_path = os.path.join(current_directory, filename)
+
+    # Read the Excel file
+    df = pd.read_excel(file_path, sheet_name="C_Na2SO4_sol_line")
+
     #Sodium sulfate (Mirabilite) Solubility Line, Data from source: The solution ref on dropbox (1100-1200; P.1120)
-    df = pd.read_excel('C:\\Users\\rodoulaktori\\surfdrive\\PhD\\Process_modelling\\python\\efc_results.xlsx', sheet_name="C_Na2SO4_sol_line")
     T_Na2SO4_sol_line= df.iloc[:, 1].tolist()
     C_Na2SO4_sol_line=df.iloc[:, 0].tolist()
     C_Na2SO4_sol_line=np.array(C_Na2SO4_sol_line)
 
     print("T_Na2SO4_sol_line "+str(T_Na2SO4_sol_line))
 
     print("C_Na2SO4_sol_line "+str(C_Na2SO4_sol_line))
                                                             
 
     tck= interpolate.splrep(T_Na2SO4_sol_line, C_Na2SO4_sol_line, k=1)
     print("tck is " +str(tck))
 
     #Interpolation/Extrapolation of the ice line using linear regression
-    df2 = pd.read_excel('C:\\Users\\rodoulaktori\\surfdrive\\PhD\\Process_modelling\\python\\efc_results.xlsx', sheet_name="ICE_sol_line")
+    df2 = pd.read_excel(file_path, sheet_name="ICE_sol_line")
 
     Fr_point_depr_Na2SO4= np.array(df2.iloc[:, 1].tolist())
     C_Na2SO4_ice_line=df2.iloc[:, 0].tolist()    
     print("C_Na2SO4_ice_line is "+str(C_Na2SO4_ice_line))
     #Ice line in the Na2SO4-Water phase diagram : Source : CONCENTRATIVE PROPERTIES OF AQUEOUS SOLUTIONS:DENSITY, REFRACTIVE INDEX, FREEZING POINT DEPRESSION, AND VISCOSITY
 
     T_fr_Na2SO4=273+Fr_point_depr_Na2SO4    
@@ -826,17 +839,16 @@
 E_t=Q_t+E_p+E_fil
 print("E_t"+str(E_t))
 sec_f=E_t/Qf
 sec_eff=E_t/(Mout/1020)
 sec_product=E_t/M_compound1_cr
 w_in_cryst=M_compound1_cr*10*18.01528/MW_Na2SO4_10H2O
 print(w_in_cryst)
-bal=Qf-M_ice*res-Mout*res-M_compound1_cr*res
 print("M_ice*res is "+str(M_ice*res))
 print("Mout*res is "+str(Mout*res))
 print("M_compound1_cr*res is "+str(M_compound1_cr*res))
-print("bal is "+str(bal))
+
 M_efc_out=Var.M_liquid_tot.item()
 M_compound1_cr=M_compound1_cr*res+bal
 M_ice=M_ice*res
 bal=Qf-M_ice -Var.M_liquid_tot.item() -M_compound1_cr
 print("bal is "+str(bal))
```

### Comparing `desalsim-0.7.2/Desalsim/med_unit_f.py` & `desalsim-0.7.3/tests/med_unit_f.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from density_calc import density_calc
+from  Desalsim.density_calc import density_calc
+
 #%%calculations 
 class MEDCalculator:
     """
     A class used to represent Mass Balance for Multi-Effect Distillation 
 
     ...
 
@@ -130,7 +131,8 @@
         # Calculate concentrations in the output, g/l
         self.CNa_out=self.CNa_in*self.Mf/self.Bn 
         self.CCl_out=self.CCl_in*self.Mf/self.Bn 
         self.CK_out=self.CK_in*self.Mf/self.Bn 
         self.CMg_out=self.CMg_in*self.Mf/self.Bn 
         self.CCa_out=self.CCa_in*self.Mf/self.Bn  
         self.CSO4_out=self.CSO4_in*self.Mf/self.Bn  
+
```

### Comparing `desalsim-0.7.2/Desalsim/mfpfr_unit_f.py` & `desalsim-0.7.3/Desalsim/mfpfr_unit_f.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 import density_calc
-import scaleup
-from density_calc import density_calc
+from Desalsim import scaleup
+from Desalsim.density_calc import density_calc 
 import math
-import constants
+from Desalsim import constants 
 #%%
     #molecular weight
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
 MW_Ca=constants.MW_Ca
```

### Comparing `desalsim-0.7.2/Desalsim/nanofiltration_unit_f.py` & `desalsim-0.7.3/Desalsim/nanofiltration_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 import numpy as np
 from Desalsim.density_calc import density_calc 
-import constants 
+from Desalsim import constants 
 import math
 #
     #molecular weight
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
```

### Comparing `desalsim-0.7.2/Desalsim/ro_unit_f.py` & `desalsim-0.7.3/Desalsim/ro_unit_f.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
-import constants
-import density_calc
+from Desalsim import constants 
+from Desalsim.density_calc import density_calc 
 #%%
 #%%constants
 R=8.31446261815324 #gas constant
 T=20+273.15 #K
 MW_Na=22.99
 MW_cl=35.453
 MW_so4=32.064+4*15.999
```

### Comparing `desalsim-0.7.2/Desalsim/thermal_cryst_f.py` & `desalsim-0.7.3/tests/thermal_cryst_f.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
-import density_calc
-import constants
-import scaleup
+from  Desalsim.density_calc import density_calc
+from Desalsim import constants
+from Desalsim import scaleup
 
 #%%
     #Molecular weight 
 MW_Na=constants.MW_Na
 MW_cl=constants.MW_cl
 MW_so4=constants.MW_so4
 MW_K=constants.MW_K
@@ -68,15 +68,15 @@
         self.T_op = T_op 
         self.Qf = Qf 
         self.Cf_s = Cf_s 
         self.Cf_caso4 = Cf_caso4
         self.T_in = T_in
         self.Cf_in = Cf_in
         self.nacl_sat_wt = salt_mois
-        self.d_sol=density_calc.density_calc(T_in, Cf_s)
+        self.d_sol=density_calc(T_in, Cf_s)
         self.LHV_v=LHV_v
         self.LHV_s =LHV_s 
         self.T_cw_o=T_cw_o
         self.T_cw_f=T_cw_f
         
     def mass_bal_cryst(self):
         """
@@ -232,10 +232,8 @@
     
     return round(E_el_th_Cr,2), round(E_th_th_Cr,2), round(SEC_el_f,2), round(SEC_el_NaCl,2), round(SEC_el_w,2)
 
 def mass_balance(Qf, Cf_in, M_Nacl, Csalt_out, d_sol):
     """Calculate the mass balance."""
     for i in range(len(Cf_in)):
         bal_i=Cf_in[i]*(Qf)/1000 - (M_Nacl*Csalt_out[i]/1000)
-        print(f"For {i}, mass balance equals: {bal_i}")
-
- 
+        print(f"For {i}, mass balance equals: {bal_i}")
```

### Comparing `desalsim-0.7.2/LICENSE` & `desalsim-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.2/PKG-INFO` & `desalsim-0.7.3/DesalSim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: DesalSim
-Version: 0.7.2
+Version: 0.7.3
 Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 Author: rodoulak
 Author-email: r.ktori@tudelft.nl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.0
 Requires-Dist: pandas>=1.0
+Requires-Dist: scipy>=1.0
+Requires-Dist: matplotlib>=1.0
+Requires-Dist: scikit-learn>=1.0
+Requires-Dist: plotly>=1.0
+Requires-Dist: openpyxl>=1.0
 
 # DesalSim: Desalination and Brine Treatment simulation model
 
  
 ## Overview 
 This project comprises a package of simulation models for desalination and brine treatment technologies, including reverse osmosis, nanofiltration, multi-effect distillation, chemical precipitation, eutectic freeze crystallization, electrodialysis, and thermal crystallization. These technologies are utilized for desalination, ion separation, and salt recovery processes in various industrial and environmental applications.
```

### Comparing `desalsim-0.7.2/README.md` & `desalsim-0.7.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: DesalSim
+Version: 0.7.3
+Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
+Author: rodoulak
+Author-email: r.ktori@tudelft.nl
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.0
+Requires-Dist: pandas>=1.0
+Requires-Dist: scipy>=1.0
+Requires-Dist: matplotlib>=1.0
+Requires-Dist: scikit-learn>=1.0
+Requires-Dist: plotly>=1.0
+Requires-Dist: openpyxl>=1.0
+
 # DesalSim: Desalination and Brine Treatment simulation model
 
  
 ## Overview 
 This project comprises a package of simulation models for desalination and brine treatment technologies, including reverse osmosis, nanofiltration, multi-effect distillation, chemical precipitation, eutectic freeze crystallization, electrodialysis, and thermal crystallization. These technologies are utilized for desalination, ion separation, and salt recovery processes in various industrial and environmental applications.
 
 The simulation models implemented here calculate various parameters such as salt concentration profiles, ion fluxes, energy consumption, chemical consumption, and operational costs. They provide insights into the performance and economics of the technologies under different operating conditions and input parameters. Additionally, the models allow for the integration of different technologies in various configurations to optimize process efficiency and resource utilization.
```

### Comparing `desalsim-0.7.2/example/__init__.py` & `desalsim-0.7.3/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,7 +24,9 @@
 from Desalsim.economic_f import revenue
 
 
 
 
 
 
+
+
```

### Comparing `desalsim-0.7.2/example/comparison.py` & `desalsim-0.7.3/example/comparison.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.2/example/constants.py` & `desalsim-0.7.3/example/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.2/example/economic_f.py` & `desalsim-0.7.3/example/economic_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #costs calculations functions 
-import constants
+from Desalsim import constants 
+
 #%%
 #symbols:
 #hr-> hours
 #lf -> lifetime 
 #el -> electricity
 #s-> steam
 #pr -> price
```

### Comparing `desalsim-0.7.2/example/ed_unit_f.py` & `desalsim-0.7.3/example/ed_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
-import scaleup
-import constants
 import math
-import density_calc
+from Desalsim.density_calc import density_calc 
+from Desalsim import constants 
+from Desalsim import scaleup
 
 #%% Calculations 
 """
 A class used to represent Mass Balance for Electrodialysis
 
 ...
 
@@ -140,15 +140,15 @@
 Vcp = 8  # Applied voltage (V)
 Vel=2.1 #Voltage across the electrodes 
 Ij=400 #Am2
 Mem_eff=0.64 #Membrane efficiency
 Ncp=1 #Number of identical parallel cell-pairs 
 
 #Feed flow rate L/h
-d_in_ed=(density_calc.density_calc(T-273, Sc_i)/1000)
+d_in_ed=(density_calc(T-273, Sc_i)/1000)
 Qed_in=1000/d_in_ed
 Qed_in_c=Qed_in/17/Ncp
 Qed_in_d=Qed_in*16/17/Ncp
 
 # Effective cell-pair area (m^2)
 Acp =scaleup.scaleup(24, 1000, Qed_in) 
 Acp_tot=Acp
@@ -231,15 +231,15 @@
 Cc_cl_f=Sc[N-1]/MWs*constants.MW_cl
 Sc_out=[Cc_na_f, Cc_cl_f]
 
 #Calculate the concnetrate stream flow rate 
 Mc=(Ns_c[N-1]*MWs/1000+Nw_c[N-1]*MWw/1000) #(kg/hr)
 print("Mass flowrate concentrate stream is "+str(round(Mc,2))+ " kg/hr")
 
-dc_out=density_calc.density_calc(T-273, Sc[N-1])/1000 #(kg/l)
+dc_out=density_calc(T-273, Sc[N-1])/1000 #(kg/l)
 Qc=Mc/dc_out #concnetrate stream volume flow rate (l/hr)
 i=2
 
 for i in range(2,len(Csw)):
     Sc_out.append(Csw[i]*Qed_in_c/Qc)
 
 print("Volume flowrate concentrate stream is "+str(round(Qc,2))+" l/hr")
@@ -249,15 +249,15 @@
 #Calculations for diluate stream 
 Md=(Ns_d[N-1]*MWs/1000+Nw_d[N-1]*MWw/1000) #mass flow rate (kg/hr)
 print("Mass flowrate of diluate stream is "+str(round(Md,2))+" kg/hr")
 
 Sd_f=Sd[N-1]
 Cd_na_f=Sd_f/MWs*constants.MW_Na
 Cd_cl_f=Sd_f/MWs*constants.MW_cl
-dd_out=density_calc.density_calc(T-273, Sd[N-1])/1000 #density of diluate stream
+dd_out=density_calc(T-273, Sd[N-1])/1000 #density of diluate stream
 Qd=Md/dd_out #diluate stream volume flow rate (l/hr)
 
 print("volume flowrate diluate stream is "+str(round(Qd,2))+" l/hr")
 print("The total effluent concentration dilute is " + str(round(Sd[N-1],2))+"g/kg")
 
 Sd_out=[Cd_na_f, Cd_cl_f]
```

### Comparing `desalsim-0.7.2/example/edbm_unit_f.py` & `desalsim-0.7.3/example/edbm_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math 
 import numpy as np
-import scaleup 
-import density_calc
-import constants
+from Desalsim.density_calc import density_calc 
+from Desalsim import constants 
+from Desalsim import scaleup
 
 #%%
 #Molecular weight 
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
@@ -100,17 +100,17 @@
         self.CCa_s_in=Cc5/MW_Ca #Ca concentration (g/l) to (mol/l)
         self.CSO4_s_in=Cc6/MW_SO4 #SO4 concentration (g/l) to (mol/l)
         self.CHCO3_s_in=Cc6/MW_HCO3 #HCO3 concentration (g/l) to (mol/l)      
         self.COH_s_in=COH/MW_OH
         self.CH_s_in=CH/MW_H
         self.PM_i=[MW_Na, MW_Cl, MW_K, MW_Mg, MW_Ca, MW_SO4, MW_HCO3, MW_H, MW_OH]
         
-        self.d_a=density_calc.density_calc(self.T,sum(C_a_in) )/1000
-        self.d_b=density_calc.density_calc(self.T,sum(C_b_in) )/1000
-        self.d_s=density_calc.density_calc(self.T,sum(C_s_in) )/1000
+        self.d_a=density_calc(self.T,sum(C_a_in) )/1000
+        self.d_b=density_calc(self.T,sum(C_b_in) )/1000
+        self.d_s=density_calc(self.T,sum(C_s_in) )/1000
         
         #Create lists for initial concentration in each channel 
         self.Ci_s_in=[self.CNa_s_in,self.CCl_s_in,self.CK_s_in,self.CMg_s_in,self.CCa_s_in,self.CSO4_s_in,self.CHCO3_s_in, self.CH_s_in,self.COH_s_in]
         self.Ci_b_in=[Cb1/MW_Na, Cb2/ MW_Cl,Cb3/MW_K,Cb4/MW_Mg,Cb5/MW_Ca,Cb6/MW_SO4,Cb7/MW_HCO3,Cb8/MW_H,Cb9/MW_OH]
         self.Ci_a_in=[Ca1/MW_Na,Ca2/MW_Cl,Ca3/MW_K,Ca4/MW_Mg,Ca5/MW_Ca,Ca6/MW_SO4,Ca7/MW_HCO3,Ca8/MW_H,Ca9/MW_OH]
         
         #save initial concentration before recirculation: 
@@ -206,15 +206,15 @@
         self.M_b_out_t=self.M_h2o_b_out+self.M_b_out[7]+self.M_b_out[1]+self.M_b_out[8]+self.M_b_out[0]
  
         #Calculation of outlet mass flow rate for other ionic species in channel 
         for i in range(2,7):
             self.M_b_out[i]=self.M_b_in[i]  
             self.M_b_out_t=self.M_b_out_t+self.M_b_out[i]
             
-        d_s_new=density_calc.density_calc(25, self.M_b_out_t)/1000
+        d_s_new=density_calc(25, self.M_b_out_t)/1000
         #Calculate of volumetric outlet flow rate
         self.Q1_b_out=self.M_b_out_t/d_s_new #assume density is 1kg/l
         
         #Calculation of outlet concentration of single ions in channel 
         for i in range(0,9):
             self.Ci_b_out[i]=self.M_b_out[i]/(self.Q1_b_out*self.PM_i[i]/1000)
     
@@ -309,15 +309,15 @@
 d_a=0.997 #density acid channel (units: kg/l)
 #d_s=1 #density salt channel (units: kg/l)
 d_b=0.997 #density base channel (units: kg/l)
 
 
 #Feed concentration g/L
 Cin_edbm=[13.44, 20.725, 1.146, 0, 0, 0.18, 0, 10**(-ph_s), 3.01551E-11] 
-d_in=density_calc.density_calc(25,sum(Cin_edbm))/1000
+d_in=density_calc(25,sum(Cin_edbm))/1000
 d_s=d_in
 
 C_b_in=[0,0,0,0,0,0,0,10**(-ph_b), 10**(-(14-ph_b))]
 C_a_in=[0,0,0,0,0,0,0,10**(-ph_a), 10**(-(14-ph_a))]
 
 #Feed flow rate L/h
 Q_in_edbm=47000
```

### Comparing `desalsim-0.7.2/example/efc_unit_f.py` & `desalsim-0.7.3/Desalsim/efc_unit_f.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,28 +27,28 @@
 
 import time
 import numpy as np
 from scipy import interpolate
 import scipy.interpolate as interpolate
 from sklearn.linear_model import LinearRegression
 from collections import namedtuple
-import scaleup
-import density_calc
+from Desalsim import scaleup
+from Desalsim.density_calc import density_calc 
 # import pitzer_model_3phases_w
-import constants
+from Desalsim import constants 
 #Set initial time to calculate the elapsed time of the calculations
 time0=time.time()
 MW_so4=32.064+4*15.999
 
 #input data
 Qf=100 #m3/hr
 C_i_in=[20.16, 27.87, 0.50, 0.0, 0.12, 14.66]
 
 T_initial =273+25
-d_in=density_calc.density_calc(25, sum(C_i_in))
+d_in=density_calc(25, sum(C_i_in))
 #%%
 
 #Declaration of constant process parameters - Part 1: Process Parameters
 
 Vreactor=Qf/0.7            #Volume of the reactor : m^3
 
 #Influx
@@ -240,31 +240,44 @@
         
     #Initial concentration of Compound 1
     C_compound1_initial=C_Na2SO4_initial
     print("C_compound1_initial is "+str(C_compound1_initial))
     T_Na2SO4_sol_line=[]
     C_Na2SO4_sol_line=[]
     #Interpolation/Extrapolation of the Na2SO4 solubility line with a cubic spline 
-     
+    import os
+    import pandas as pd
+
+    # Get the directory where the script is located
+    current_directory = os.path.dirname(__file__)
+
+    #   Define the filename 
+    filename = "efc_results.xlsx"
+
+    # Combine the directory path with the filename
+    file_path = os.path.join(current_directory, filename)
+
+    # Read the Excel file
+    df = pd.read_excel(file_path, sheet_name="C_Na2SO4_sol_line")
+
     #Sodium sulfate (Mirabilite) Solubility Line, Data from source: The solution ref on dropbox (1100-1200; P.1120)
-    df = pd.read_excel('C:\\Users\\rodoulaktori\\surfdrive\\PhD\\Process_modelling\\python\\efc_results.xlsx', sheet_name="C_Na2SO4_sol_line")
     T_Na2SO4_sol_line= df.iloc[:, 1].tolist()
     C_Na2SO4_sol_line=df.iloc[:, 0].tolist()
     C_Na2SO4_sol_line=np.array(C_Na2SO4_sol_line)
 
     print("T_Na2SO4_sol_line "+str(T_Na2SO4_sol_line))
 
     print("C_Na2SO4_sol_line "+str(C_Na2SO4_sol_line))
                                                             
 
     tck= interpolate.splrep(T_Na2SO4_sol_line, C_Na2SO4_sol_line, k=1)
     print("tck is " +str(tck))
 
     #Interpolation/Extrapolation of the ice line using linear regression
-    df2 = pd.read_excel('C:\\Users\\rodoulaktori\\surfdrive\\PhD\\Process_modelling\\python\\efc_results.xlsx', sheet_name="ICE_sol_line")
+    df2 = pd.read_excel(file_path, sheet_name="ICE_sol_line")
 
     Fr_point_depr_Na2SO4= np.array(df2.iloc[:, 1].tolist())
     C_Na2SO4_ice_line=df2.iloc[:, 0].tolist()    
     print("C_Na2SO4_ice_line is "+str(C_Na2SO4_ice_line))
     #Ice line in the Na2SO4-Water phase diagram : Source : CONCENTRATIVE PROPERTIES OF AQUEOUS SOLUTIONS:DENSITY, REFRACTIVE INDEX, FREEZING POINT DEPRESSION, AND VISCOSITY
 
     T_fr_Na2SO4=273+Fr_point_depr_Na2SO4    
@@ -763,80 +776,8 @@
             else:
                 pass
 Plot()
 print("Var.t is " +str(Var.t))
 print("Var.solids_weight_percentage is " +str(Var.solids_weight_percentage))
 
 #Calculate and print the elapsed time after the calculations
-elapsed=time.time()-time0
-print('Time elapsed : ',elapsed)#Calculate and print the elapsed time after the calculations
-Residence_time=Var.t/3600
-res=Residence_time#Vreactor/(Qf)
-print(res)
-print('Residence Time : ', Residence_time,'hours')
-print('Volume reactor : ', Vreactor*1000,'liters')
-Flow_rate=Qf/(d_in)/Residence_time
-print('Continous Flow Rate : ', Flow_rate,'liters/hour')
-Min=Qf#Residence_time #kg/hr 
-#mass flowrate of na2so4 
-M_compound1_cr=Var.M_compound1_cr*MW_Na2SO4_10H2O/MW_Na2SO4/res#Residence_time
-print("mass flowrate of na2so4 "+ str(M_compound1_cr)+"kg/hr")
-#mass flow rate of ice 
-M_ice= Var.M_ice/res#Residence_time
-print("ice mass flow rate " + str(M_ice)+ "kg/hr")
-#Mass flow rate for effluent
-
-Mout = Var.M_liquid_tot.item() / res # Residence_time
-print("Mass flow rate for effluent is "+ str(Mout)+"kg/hr")
-
-
-conc_f_in=conc_f(C_i_in[0],C_i_in[1], C_i_in[2], C_i_in[3], C_i_in[4], C_i_in[5],Qf/d_in, Qf, Var.M_liquid_tot.item(), M_compound1_cr)
-
-dens=1.02
-conc_f_in.calc_f_c()
-Cout= Var.C_compound1_mliq #out concentration for na2so4. only na, so4 change 
-Cout_so4= Cout.item()
-Cout_cl=Var.C_compound2
-Cout_cl= Cout_cl.item()
-Cout_na= conc_f_in.Cna_out
-Cout_so4= conc_f_in.Cso4_out
-Cout_efc_g=[Cout_na+conc_f_in.Ccl_out/constants.MW_cl*constants.MW_Na, conc_f_in.Ccl_out, conc_f_in.Ck_out, 0, 0, Cout_so4] #g/l 
-print("Cout_efc is "+str(Cout_efc_g))
-
-
-M_solids_tot=Var.M_solids_tot/res#Residence_time
-print("M_solids_tot is "+str(M_solids_tot))
-Mtot=Var.Mtot/res#Residence_time
-print("Mtot is " + str(Mtot))
-M_ice=Var.M_ice/res#Residence_time
-print("M_ice is "+str(M_ice))
-
-V_compound1=Var.V_compound1/res
-print("V_compound1 is "+str(V_compound1))
-
-#operating temperature 
-Treactor=Var.Treactor-273
-print("operating temperature is "+str(*Treactor[0])+"oC")
-
-#required energy 
-E_el=Qtot/1000*res # KW 
-Q_t=abs(Qtot/1000)
-print("Q_t"+str(Q_t))
-E_p=(Min*dp+Mout*dp+(M_ice+M_compound1_cr)*dp_slurry)*1e5/3600/(1000*npump)/1000 #kwh
-E_fil=scaleup.scaleup(0.5, 0.3*1000, Qf)
-E_t=Q_t+E_p+E_fil
-print("E_t"+str(E_t))
-sec_f=E_t/Qf
-sec_eff=E_t/(Mout/1020)
-sec_product=E_t/M_compound1_cr
-w_in_cryst=M_compound1_cr*10*18.01528/MW_Na2SO4_10H2O
-print(w_in_cryst)
-bal=Qf-M_ice*res-Mout*res-M_compound1_cr*res
-print("M_ice*res is "+str(M_ice*res))
-print("Mout*res is "+str(Mout*res))
-print("M_compound1_cr*res is "+str(M_compound1_cr*res))
-print("bal is "+str(bal))
-M_efc_out=Var.M_liquid_tot.item()
-M_compound1_cr=M_compound1_cr*res+bal
-M_ice=M_ice*res
-bal=Qf-M_ice -Var.M_liquid_tot.item() -M_compound1_cr
-print("bal is "+str(bal))
+elapsed=time.time()-time0
```

### Comparing `desalsim-0.7.2/example/example_1.py` & `desalsim-0.7.3/example/example_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #Import functions 
-from nanofiltration_unit_f import OsmoticPressure
-from nanofiltration_unit_f import NFMass
-from nanofiltration_unit_f import NfEnergy
+from Desalsim.nanofiltration_unit_f import OsmoticPressure
+from Desalsim.nanofiltration_unit_f import NFMass
+from Desalsim.nanofiltration_unit_f import NfEnergy
 
-from mfpfr_unit_f import MFPFRCALC
-from mfpfr_unit_f import HClAddition
-from mfpfr_unit_f import energycons
+from Desalsim.mfpfr_unit_f import MFPFRCALC
+from Desalsim.mfpfr_unit_f import HClAddition
+from Desalsim.mfpfr_unit_f import energycons
 
-from ed_unit_f import ElectrodialysisCalc
+from Desalsim.ed_unit_f import ElectrodialysisCalc
 
-from edbm_unit_f import EDBMCalc
+from Desalsim.edbm_unit_f import EDBMCalc
 
-from economic_f import revenue
-from economic_f import econom
+from Desalsim.economic_f import revenue
+from Desalsim.economic_f import econom
 
-from density_calc import density_calc
-import constants
-import scaleup
+from Desalsim.density_calc import density_calc
+from Desalsim import constants
+from Desalsim import scaleup
 import numpy as np
 import pandas as pd
 import math
 
 
 #%%Constants
```

### Comparing `desalsim-0.7.2/example/example_2.py` & `desalsim-0.7.3/example/example_2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #Scenario 2
 ##treatment train: NF-> MED-> THERMAL CRYST                 
-from nanofiltration_unit_f import OsmoticPressure
-from nanofiltration_unit_f import NFMass
-from nanofiltration_unit_f import NfEnergy
+from Desalsim.nanofiltration_unit_f import OsmoticPressure
+from Desalsim.nanofiltration_unit_f import NFMass
+from Desalsim.nanofiltration_unit_f import NfEnergy
 
-from med_unit_f import MEDCalculator
+from Desalsim.med_unit_f import MEDCalculator
 
-from thermal_cryst_f import thermal_calc
-from thermal_cryst_f import conc_cal
-from thermal_cryst_f import calculate_energy
+from Desalsim.thermal_cryst_f import thermal_calc
+from Desalsim.thermal_cryst_f import conc_cal
+from Desalsim.thermal_cryst_f import calculate_energy
 
 
-import constants
+from Desalsim import constants
 
-from economic_f import revenue
-from economic_f import econom
+from Desalsim.economic_f import revenue
+from Desalsim.economic_f import econom
 
-import scaleup
-from density_calc import density_calc
+from Desalsim import scaleup
+from Desalsim.density_calc import density_calc
 import numpy as np
 import pandas as pd
 #%%
 #Molecular weight 
     #molecular weight
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
```

### Comparing `desalsim-0.7.2/example/med_unit_f.py` & `desalsim-0.7.3/example/med_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from density_calc import density_calc
+from Desalsim.density_calc import density_calc 
 #%%calculations 
 class MEDCalculator:
     """
     A class used to represent Mass Balance for Multi-Effect Distillation 
 
     ...
```

### Comparing `desalsim-0.7.2/example/mfpfr_unit_f.py` & `desalsim-0.7.3/example/mfpfr_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import math
-import density_calc
-import scaleup
-from density_calc import density_calc
+from Desalsim.density_calc import density_calc 
+from Desalsim import constants 
+from Desalsim import scaleup
 import math
-import constants
 #%%
     #molecular weight
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
 MW_Ca=constants.MW_Ca
```

### Comparing `desalsim-0.7.2/example/nanofiltration_unit_f.py` & `desalsim-0.7.3/example/nanofiltration_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 import numpy as np
-from density_calc import density_calc
-import constants 
+from Desalsim.density_calc import density_calc 
+from Desalsim import constants 
 import math
 #
     #molecular weight
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
```

### Comparing `desalsim-0.7.2/example/ro_unit_f.py` & `desalsim-0.7.3/example/ro_unit_f.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
-import constants
-import density_calc
+from Desalsim.density_calc import density_calc 
+from Desalsim import constants 
 #%%
 #%%constants
 R=8.31446261815324 #gas constant
 T=20+273.15 #K
 MW_Na=22.99
 MW_cl=35.453
 MW_so4=32.064+4*15.999
```

### Comparing `desalsim-0.7.2/example/thermal_cryst_f.py` & `desalsim-0.7.3/example/thermal_cryst_f.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
-import density_calc
-import constants
-import scaleup
+from Desalsim.density_calc import density_calc 
+from Desalsim import constants 
+from Desalsim import scaleup
 
 #%%
     #Molecular weight 
 MW_Na=constants.MW_Na
 MW_cl=constants.MW_cl
 MW_so4=constants.MW_so4
 MW_K=constants.MW_K
@@ -68,15 +68,15 @@
         self.T_op = T_op 
         self.Qf = Qf 
         self.Cf_s = Cf_s 
         self.Cf_caso4 = Cf_caso4
         self.T_in = T_in
         self.Cf_in = Cf_in
         self.nacl_sat_wt = salt_mois
-        self.d_sol=density_calc.density_calc(T_in, Cf_s)
+        self.d_sol=density_calc(T_in, Cf_s)
         self.LHV_v=LHV_v
         self.LHV_s =LHV_s 
         self.T_cw_o=T_cw_o
         self.T_cw_f=T_cw_f
         
     def mass_bal_cryst(self):
         """
@@ -140,15 +140,15 @@
         self.Cc1=Cc1
         self.Cc2=Cc2
         self.Cc3=Cc3
         self.Cc4=Cc4
         self.Cc5=Cc5
         self.Cc6=Cc6
         # Calculate the density of the feed solution at T_in 
-        self.d_sol=density_calc.density_calc(T_in, self.cf_in) 
+        self.d_sol=density_calc(T_in, self.cf_in) 
     
     
     def molarity(self):        
         """This method calculates the molarity of different ions in the solution"""
         self.Cc1_mol=self.Cc1/MW_Na
         self.Cc2_mol=self.Cc2/MW_cl
         self.Cc3_mol=self.Cc3/MW_K
@@ -285,15 +285,15 @@
 #Feed flowrate
 Qf=1000 #kg/h
 
 #Feed concentration 
 
 Cf_tcr_in=[80.42, 116.69, 2.29, 0.01, 0.04, 0.54] #[Na, Cl, K, Mg, Ca, SO4 ]
 Cf_s=sum(Cf_tcr_in) #total salt concentration (g/L)
-d_sol=density_calc.density_calc(T_in, Cf_s)/1000 #density of feed
+d_sol=density_calc(T_in, Cf_s)/1000 #density of feed
 Cf_caso4=Cf_tcr_in[4]*MW_Caso4/MW_Ca #CaSO4 concentration in feed solution (g/L)
 
 #Calculation 
 th_cryst_dat=thermal_calc(T_op, Qf, Cf_s, Cf_caso4, T_in, Cf_tcr_in, salt_mois, LHV_v, LHV_s, T_cw_o, T_cw_f)
 th_cryst_dat.mass_bal_cryst()
 th_cryst_dat.heat_bal_cryst()
```

### Comparing `desalsim-0.7.2/tests/__init__.py` & `desalsim-0.7.3/Desalsim/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # __init__.py
 from Desalsim import density_calc
 from Desalsim import constants
-
 from Desalsim.nanofiltration_unit_f import NFMass
 from Desalsim.nanofiltration_unit_f import OsmoticPressure
 from Desalsim.nanofiltration_unit_f import NfEnergy
 
 from Desalsim.med_unit_f import MEDCalculator
 
 from Desalsim.thermal_cryst_f import thermal_calc
@@ -25,8 +24,7 @@
 
 
 
 
 
 
 
-
```

### Comparing `desalsim-0.7.2/tests/constants.py` & `desalsim-0.7.3/tests/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.2/tests/economic_f.py` & `desalsim-0.7.3/tests/economic_f.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #costs calculations functions 
-import constants
+from Desalsim import constants
 #%%
 #symbols:
 #hr-> hours
 #lf -> lifetime 
 #el -> electricity
 #s-> steam
 #pr -> price
```

### Comparing `desalsim-0.7.2/tests/economic_unittest.py` & `desalsim-0.7.3/tests/economic_unittest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
-from  economic_f import econom, revenue
-import density_calc
-import constants
-import scaleup
+from  Desalsim.economic_f import econom, revenue
+from  Desalsim.density_calc import density_calc
+from Desalsim import constants
+from Desalsim import scaleup
 
 class TestEconom(unittest.TestCase):
     def setUp(self):
         # Define sample input data for initialization
         eq_c = 1500000
         el_conc = 10
         s_conc = 0
@@ -14,57 +14,45 @@
         chem1_pr=0.002
         chem2_conc=0
         chem2_pr=0.002
         cw_conc = 0
         wat_conc = 0
         capex_assumptions=[0.25, 0.2, 0.06, 0.15, 0.2]
         
+        prd=10  
+        prd_name= "Water" 
+        
         # Create an instance of the econom class
         self.econom_calc = econom(eq_c, el_conc, s_conc, chem1_conc, chem1_pr, chem2_conc, chem2_pr, cw_conc, wat_conc)
         self.result_capex = self.econom_calc.capex_calc(capex_assumptions)
+        self.revenue_calc = revenue(prd, prd_name)
         
     def test_capex_calc(self):
         capex_result = self.result_capex
         
         # Set CAPEX assumptions 
         capex_assumptions=[0.25, 0.2, 0.06, 0.15, 0.2]
 
         # Call the capex_calc method
         self.result_capex = self.econom_calc.capex_calc(capex_assumptions)
         
         # Assert the correctness of the output
         expected_capex = 3125700  # Assuming this value based on your calculations
-        self.assertAlmostEqual(self.result_capex[0], expected_capex, delta=1000)
+        self.assertAlmostEqual(self.result_capex, expected_capex, delta=expected_capex*0.01)
 
 
     def test_opex_calc(self):
         # Access the stored result from test_capex_calc
         capex_result = self.result_capex
         
         # Call the opex_calc method
         result_opex = self.econom_calc.opex_calc(7200, 0.253, 0, 0.000118, 0.001, [0.03, 0.05, 0.15, 0.15, 0.15, 0.03, 0.05, 0.05, 0.67])
         
         # Assert the correctness of the output
         expected_opex = 148541.66  # Assuming this value based on your calculations
         self.assertAlmostEqual(result_opex, expected_opex, delta=expected_opex*0.01)
 
 
-class TestRevenue(unittest.TestCase):
-    def setUp(self):
-        # Define sample input data for initialization
-        prd=10  
-        prd_name= "Water"  
-        
-        # Create an instance of the revenue class
-        self.revenue_calc = revenue(prd, prd_name)
-
-    def test_rev_water(self):
-        # Call the rev method with Water as product
-        result_rev = self.revenue_calc.rev(7200, 0.001, 0.066, 1.0, 0.12, 7.2, 5.78)
-        
-        # Assert the correctness of the output
-        expected_rev = 72.0  # Assuming this value based on your calculations
-        self.assertAlmostEqual(result_rev, expected_rev, delta=1)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `desalsim-0.7.2/tests/ed_unittest.py` & `desalsim-0.7.3/tests/ed_unittest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 import unittest
-import constants
-from ed_unit_f import ElectrodialysisCalc
+from Desalsim import constants
+from Desalsim.ed_unit_f import ElectrodialysisCalc
+
+# Define the input parameters for testing
+C_feed = [10.36, 15.39, 0.36, 0.028, 0.02, 0.07]  # Feed concentrations in g/L
+Q_feed = 1000  # Feed flow rate in L/hr
+T_feed = 40  # Feed temperature in °C
+T_dial = 25  # Dialysate temperature in °C
+A_membrane = 10  # Membrane area in m^2
+V_cell = 100  # Voltage across the cell in V
+I_current = 50  # Current passing through the cell in A
 
 class TestElectrodialysisCalc(unittest.TestCase):
-    def setUp(self):
-        # Define the input parameters for testing
-        C_feed = [10.36, 15.39, 0.36, 0.028, 0.02, 0.07]  # Feed concentrations in g/L
-        Q_feed = 1000  # Feed flow rate in L/hr
-        T_feed = 40  # Feed temperature in °C
-        T_dial = 25  # Dialysate temperature in °C
-        A_membrane = 10  # Membrane area in m^2
-        V_cell = 100  # Voltage across the cell in V
-        I_current = 50  # Current passing through the cell in A
-        
+    def setUp(self):        
         # Create an instance of the ElectrodialysisCalc class with the defined parameters
-        self.ed_calc = ElectrodialysisCalc(C_feed, Q_feed, T_feed, T_dial, A_membrane, V_cell, I_current)
+        self.ed_calc = ElectrodialysisCalc()
         
     def test_Ts_cp(self):
         # Call the Ts_cp method
-        result = self.ed_calc.Ts_cp(10)
+        result = ElectrodialysisCalc.Ts_cp(10)
         
         # Define the expected value
         expected_result = 0.9676  # Expected result for S=10
         
         # Assert the equality of the calculated value and expected value
         self.assertAlmostEqual(result, expected_result, delta=expected_result*0.01)
 
     def test_Tw_cp(self):
         # Call the Tw_cp method
         Sc=43
         Sd=43
-        result = self.ed_calc.Tw_cp(Sc, Sd)
+        result = ElectrodialysisCalc.Tw_cp(Sc, Sd)
         
         # Define the expected value
         expected_result = 10.3  
         
         # Assert the equality of the calculated value and expected value
         self.assertAlmostEqual(result, expected_result, delta=expected_result*0.01)
         
     def test_Lw_cp(self):
         # Call the Lw_cp method
         S = 43
-        result = self.ed_calc.Lw_cp(S)
+        result = ElectrodialysisCalc.Lw_cp(S)
         
         # Define the expected value
         expected_result = 5 * S ** (-0.416)
         
         # Assert the equality of the calculated value and expected value
         self.assertAlmostEqual(result, expected_result, delta=expected_result*0.01)
 
     def test_p_osmo(self):
         # Call the p_osmo method
         S = 43
         T = 25
         MWs = constants.MW_NaCl
         
-        result = self.ed_calc.p_osmo(S, T, MWs)
+        result = ElectrodialysisCalc.p_osmo(S, T, MWs)
         
         # Define the expected value
         C1 = S / MWs * constants.MW_Na / constants.MW_Na
         C2 = S / MWs * constants.MW_cl / constants.MW_cl
         sum_Ci = C1 + C2
         expected_result = 0.0831446261815324 * sum_Ci * T
         
@@ -73,15 +73,15 @@
         D = 1.61e-9 #Diffusion coefficient (m^2/s)
         Ij = 50
         h = 0.5
         Sh = 18
 
         
         # Call the dC method
-        result = self.ed_calc.dC(Ts_cp, tcu, D, Ij, h, Sh)
+        result = ElectrodialysisCalc.dC(Ts_cp, tcu, D, Ij, h, Sh)
         
         # Define the expected value
         F = 96485.3329  # Faraday constant (C/mol)
         Tcu = (Ts_cp + 1) / 2
         expected_result = -(Tcu - tcu) / D * (Ij / F) * (2 * h / 1000 / Sh)
         
         # Assert the equality of the calculated value and expected value
```

### Comparing `desalsim-0.7.2/tests/edbm_unit_f.py` & `desalsim-0.7.3/tests/edbm_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math 
 import numpy as np
-import scaleup 
-import density_calc
-import constants
+from  Desalsim.density_calc import density_calc
+from Desalsim import constants
+from Desalsim import scaleup
 
 #%%
 #Molecular weight 
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
@@ -100,17 +100,17 @@
         self.CCa_s_in=Cc5/MW_Ca #Ca concentration (g/l) to (mol/l)
         self.CSO4_s_in=Cc6/MW_SO4 #SO4 concentration (g/l) to (mol/l)
         self.CHCO3_s_in=Cc6/MW_HCO3 #HCO3 concentration (g/l) to (mol/l)      
         self.COH_s_in=COH/MW_OH
         self.CH_s_in=CH/MW_H
         self.PM_i=[MW_Na, MW_Cl, MW_K, MW_Mg, MW_Ca, MW_SO4, MW_HCO3, MW_H, MW_OH]
         
-        self.d_a=density_calc.density_calc(self.T,sum(C_a_in) )/1000
-        self.d_b=density_calc.density_calc(self.T,sum(C_b_in) )/1000
-        self.d_s=density_calc.density_calc(self.T,sum(C_s_in) )/1000
+        self.d_a=density_calc(self.T,sum(C_a_in) )/1000
+        self.d_b=density_calc(self.T,sum(C_b_in) )/1000
+        self.d_s=density_calc(self.T,sum(C_s_in) )/1000
         
         #Create lists for initial concentration in each channel 
         self.Ci_s_in=[self.CNa_s_in,self.CCl_s_in,self.CK_s_in,self.CMg_s_in,self.CCa_s_in,self.CSO4_s_in,self.CHCO3_s_in, self.CH_s_in,self.COH_s_in]
         self.Ci_b_in=[Cb1/MW_Na, Cb2/ MW_Cl,Cb3/MW_K,Cb4/MW_Mg,Cb5/MW_Ca,Cb6/MW_SO4,Cb7/MW_HCO3,Cb8/MW_H,Cb9/MW_OH]
         self.Ci_a_in=[Ca1/MW_Na,Ca2/MW_Cl,Ca3/MW_K,Ca4/MW_Mg,Ca5/MW_Ca,Ca6/MW_SO4,Ca7/MW_HCO3,Ca8/MW_H,Ca9/MW_OH]
         
         #save initial concentration before recirculation: 
@@ -206,15 +206,15 @@
         self.M_b_out_t=self.M_h2o_b_out+self.M_b_out[7]+self.M_b_out[1]+self.M_b_out[8]+self.M_b_out[0]
  
         #Calculation of outlet mass flow rate for other ionic species in channel 
         for i in range(2,7):
             self.M_b_out[i]=self.M_b_in[i]  
             self.M_b_out_t=self.M_b_out_t+self.M_b_out[i]
             
-        d_s_new=density_calc.density_calc(25, self.M_b_out_t)/1000
+        d_s_new=density_calc(25, self.M_b_out_t)/1000
         #Calculate of volumetric outlet flow rate
         self.Q1_b_out=self.M_b_out_t/d_s_new #assume density is 1kg/l
         
         #Calculation of outlet concentration of single ions in channel 
         for i in range(0,9):
             self.Ci_b_out[i]=self.M_b_out[i]/(self.Q1_b_out*self.PM_i[i]/1000)
```

### Comparing `desalsim-0.7.2/tests/edbm_unittest.py` & `desalsim-0.7.3/tests/edbm_unittest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from edbm_unit_f import EDBMCalc  
+from Desalsim.edbm_unit_f import EDBMCalc  
 
 class TestEDBMCalc(unittest.TestCase):
     def setUp(self):
         # Define sample input data for initialization
         Qin = 1000
         A = 0.4
         I_d = 400
```

### Comparing `desalsim-0.7.2/tests/med_unit_f.py` & `desalsim-0.7.3/Desalsim/med_unit_f.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from density_calc import density_calc
+from Desalsim.density_calc import density_calc 
 #%%calculations 
 class MEDCalculator:
     """
     A class used to represent Mass Balance for Multi-Effect Distillation 
 
     ...
 
@@ -130,8 +130,7 @@
         # Calculate concentrations in the output, g/l
         self.CNa_out=self.CNa_in*self.Mf/self.Bn 
         self.CCl_out=self.CCl_in*self.Mf/self.Bn 
         self.CK_out=self.CK_in*self.Mf/self.Bn 
         self.CMg_out=self.CMg_in*self.Mf/self.Bn 
         self.CCa_out=self.CCa_in*self.Mf/self.Bn  
         self.CSO4_out=self.CSO4_in*self.Mf/self.Bn  
-
```

### Comparing `desalsim-0.7.2/tests/med_unittest.py` & `desalsim-0.7.3/tests/med_unittest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from med_unit_f import MEDCalculator, density_calc
+from Desalsim.med_unit_f import MEDCalculator, density_calc
 
 class TestMEDCalculator(unittest.TestCase):
     def setUp(self):
         # Define the input parameters for testing
         Cin_med = [10.36, 15.39, 0.36, 0.028, 0.02, 0.07]
         Qf_med = 1000
         Mf_med = 174.475 # Assuming a density of 1 g/ml
```

### Comparing `desalsim-0.7.2/tests/mfpfr_unit_f.py` & `desalsim-0.7.3/tests/mfpfr_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
-import density_calc
-import scaleup
-from density_calc import density_calc
+from  Desalsim.density_calc import density_calc
+from Desalsim import constants
+from Desalsim import scaleup
 import math
-import constants
+
 #%%
     #molecular weight
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
 MW_Ca=constants.MW_Ca
```

### Comparing `desalsim-0.7.2/tests/mfpfr_unittest.py` & `desalsim-0.7.3/tests/mfpfr_unittest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from mfpfr_unit_f import MFPFRCALC, HClAddition
+from Desalsim.mfpfr_unit_f import MFPFRCALC, HClAddition
 
 class TestMFPFRCALC(unittest.TestCase):
     def setUp(self):
         # Define sample input data for initialization
         Qin = 1000
         Cin_mfpfr = [17.3, 38.6, 0.6, 4.3, 1.2, 9.9]
         C_NaOH_1 = 1
```

### Comparing `desalsim-0.7.2/tests/nanofiltration_unit_f.py` & `desalsim-0.7.3/tests/nanofiltration_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 import numpy as np
-from density_calc import density_calc
-import constants 
+from  Desalsim.density_calc import density_calc
+from Desalsim import constants
 import math
 #
     #molecular weight
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
```

### Comparing `desalsim-0.7.2/tests/nanofiltration_unittest.py` & `desalsim-0.7.3/tests/nanofiltration_unittest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from nanofiltration_unit_f import NFMass, OsmoticPressure, NfEnergy
+from Desalsim.nanofiltration_unit_f import NFMass, OsmoticPressure, NfEnergy
 
 class TestNanofiltrationUnit(unittest.TestCase):
 
     def test_nfmass(self):
         # Test NFMass calculation
         components = ['Na', 'Cl', 'K', 'Mg', 'Ca', 'SO4']
         self.C_in = [12.33, 21.67, 0.45, 1.39, 0.45, 3.28]
```

### Comparing `desalsim-0.7.2/tests/thermal_cryst_f.py` & `desalsim-0.7.3/Desalsim/thermal_cryst_f.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
-import density_calc
-import constants
-import scaleup
+from Desalsim.density_calc import density_calc 
+from Desalsim import constants 
+from Desalsim import scaleup
 
 #%%
     #Molecular weight 
 MW_Na=constants.MW_Na
 MW_cl=constants.MW_cl
 MW_so4=constants.MW_so4
 MW_K=constants.MW_K
@@ -232,8 +232,10 @@
     
     return round(E_el_th_Cr,2), round(E_th_th_Cr,2), round(SEC_el_f,2), round(SEC_el_NaCl,2), round(SEC_el_w,2)
 
 def mass_balance(Qf, Cf_in, M_Nacl, Csalt_out, d_sol):
     """Calculate the mass balance."""
     for i in range(len(Cf_in)):
         bal_i=Cf_in[i]*(Qf)/1000 - (M_Nacl*Csalt_out[i]/1000)
-        print(f"For {i}, mass balance equals: {bal_i}")
+        print(f"For {i}, mass balance equals: {bal_i}")
+
+
```

### Comparing `desalsim-0.7.2/tests/thermal_cryst_unittest.py` & `desalsim-0.7.3/tests/thermal_cryst_unittest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
-from thermal_cryst_f import thermal_calc, conc_cal, calculate_energy
-import density_calc
-import constants
-import scaleup
+from Desalsim.thermal_cryst_f import thermal_calc, conc_cal, calculate_energy
+from Desalsim.density_calc import density_calc
+from Desalsim import constants
+from Desalsim import scaleup
 
 class TestThermalCrystalUnit(unittest.TestCase):
     def setUp(self):
         # Define input parameters for testing
         self.T_op = 60  # Operating temperature (°C)
         self.Qf = 1000  # Inlet flow rate (kg/hr)
         self.Cf_s = 200  # Total ion concentration of solution (g/L)
@@ -14,15 +14,15 @@
         self.T_in = 40  # Inlet feed temperature (°C)
         Cf_in = [80.42, 116.69, 2.29, 0.01, 0.04, 0.54]  # List of concentration of ions in the solution (g/L)
         self.salt_mois = 20  # Weight percent of NaCl at saturation
         self.LHV_v = 2199.7  # Boiling point elevation (°C)
         self.LHV_s = 2357.69  # Steam temperature (°C)
         self.T_cw_o = 40  # Cooling water inlet temperature (°C)
         self.T_cw_f = 25  # Cooling water outlet temperature (°C)
-        self.d_sol=density_calc.density_calc(self.T_in, sum(Cf_in)) 
+        self.d_sol=density_calc(self.T_in, sum(Cf_in)) 
         
         # Create an instance of the thermal_calc class with the defined parameters
         self.thermal_calc_instance = thermal_calc(self.T_op, self.Qf, self.Cf_s, Cf_caso4,self.T_in, Cf_in, self.salt_mois, self.LHV_v, self.LHV_s,self.T_cw_o, self.T_cw_f)
         self.result_mass=self.thermal_calc_instance.mass_bal_cryst()
         self.result_heat=self.thermal_calc_instance.heat_bal_cryst()
```

