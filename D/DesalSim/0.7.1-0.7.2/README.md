# Comparing `tmp/desalsim-0.7.1.tar.gz` & `tmp/desalsim-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desalsim-0.7.1.tar", last modified: Wed May  8 07:28:03 2024, max compression
+gzip compressed data, was "desalsim-0.7.2.tar", last modified: Wed May  8 07:34:08 2024, max compression
```

## Comparing `desalsim-0.7.1.tar` & `desalsim-0.7.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 07:28:03.471690 desalsim-0.7.1/
-drwxrwxrwx   0        0        0        0 2024-05-08 07:28:03.464659 desalsim-0.7.1/DesalSim.egg-info/
--rw-rw-rw-   0        0        0     9945 2024-05-08 07:28:03.000000 desalsim-0.7.1/DesalSim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1276 2024-05-08 07:28:03.000000 desalsim-0.7.1/DesalSim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 07:28:03.000000 desalsim-0.7.1/DesalSim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-08 07:28:03.000000 desalsim-0.7.1/DesalSim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-08 07:28:03.000000 desalsim-0.7.1/DesalSim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 07:28:03.354508 desalsim-0.7.1/Desalsim/
--rw-rw-rw-   0        0        0      786 2024-05-08 06:54:35.000000 desalsim-0.7.1/Desalsim/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.7.1/Desalsim/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.1/Desalsim/density_calc.py
--rw-rw-rw-   0        0        0     8821 2024-05-06 16:12:13.000000 desalsim-0.7.1/Desalsim/economic_f.py
--rw-rw-rw-   0        0        0     2950 2024-04-29 20:32:39.000000 desalsim-0.7.1/Desalsim/ed_unit_f.py
--rw-rw-rw-   0        0        0    11744 2024-04-29 21:17:33.000000 desalsim-0.7.1/Desalsim/edbm_unit_f.py
--rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.7.1/Desalsim/efc_unit_f.py
--rw-rw-rw-   0        0        0     4494 2024-04-29 20:24:16.000000 desalsim-0.7.1/Desalsim/med_unit_f.py
--rw-rw-rw-   0        0        0    10049 2024-04-29 21:14:03.000000 desalsim-0.7.1/Desalsim/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     6987 2024-05-06 08:40:06.000000 desalsim-0.7.1/Desalsim/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.7.1/Desalsim/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.1/Desalsim/scaleup.py
--rw-rw-rw-   0        0        0     8692 2024-04-29 19:44:35.000000 desalsim-0.7.1/Desalsim/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-0.7.1/LICENSE
--rw-rw-rw-   0        0        0     9945 2024-05-08 07:28:03.466653 desalsim-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     9618 2024-05-08 07:10:33.000000 desalsim-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 07:28:03.401903 desalsim-0.7.1/example/
--rw-rw-rw-   0        0        0      786 2024-05-08 06:57:43.000000 desalsim-0.7.1/example/__init__.py
--rw-rw-rw-   0        0        0     4531 2024-04-11 13:19:36.000000 desalsim-0.7.1/example/comparison.py
--rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-0.7.1/example/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.1/example/density_calc.py
--rw-rw-rw-   0        0        0    11978 2024-05-06 16:09:51.000000 desalsim-0.7.1/example/economic_f.py
--rw-rw-rw-   0        0        0     8663 2024-04-29 21:33:04.000000 desalsim-0.7.1/example/ed_unit_f.py
--rw-rw-rw-   0        0        0    17118 2024-04-29 21:35:34.000000 desalsim-0.7.1/example/edbm_unit_f.py
--rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.7.1/example/efc_unit_f.py
--rw-rw-rw-   0        0        0    33181 2024-05-06 17:04:03.000000 desalsim-0.7.1/example/example_1.py
--rw-rw-rw-   0        0        0    21599 2024-05-06 16:29:23.000000 desalsim-0.7.1/example/example_2.py
--rw-rw-rw-   0        0        0     8532 2024-04-29 21:36:53.000000 desalsim-0.7.1/example/med_unit_f.py
--rw-rw-rw-   0        0        0    14921 2024-05-03 08:06:32.000000 desalsim-0.7.1/example/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     9421 2024-05-06 08:39:39.000000 desalsim-0.7.1/example/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.7.1/example/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.1/example/scaleup.py
--rw-rw-rw-   0        0        0    12262 2024-04-29 21:44:17.000000 desalsim-0.7.1/example/thermal_cryst_f.py
--rw-rw-rw-   0        0        0       42 2024-05-08 07:28:03.472833 desalsim-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0      611 2024-05-08 07:26:49.000000 desalsim-0.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:28:03.461670 desalsim-0.7.1/tests/
--rw-rw-rw-   0        0        0      790 2024-05-08 06:58:06.000000 desalsim-0.7.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.7.1/tests/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.1/tests/density_calc.py
--rw-rw-rw-   0        0        0     9094 2024-05-06 16:12:45.000000 desalsim-0.7.1/tests/economic_f.py
--rw-rw-rw-   0        0        0     2527 2024-05-06 16:15:02.000000 desalsim-0.7.1/tests/economic_unittest.py
--rw-rw-rw-   0        0        0     3255 2024-05-03 14:14:54.000000 desalsim-0.7.1/tests/ed_unit_f.py
--rw-rw-rw-   0        0        0     3316 2024-05-03 14:16:37.000000 desalsim-0.7.1/tests/ed_unittest.py
--rw-rw-rw-   0        0        0    12680 2024-05-03 13:51:25.000000 desalsim-0.7.1/tests/edbm_unit_f.py
--rw-rw-rw-   0        0        0     8386 2024-05-03 13:50:48.000000 desalsim-0.7.1/tests/edbm_unittest.py
--rw-rw-rw-   0        0        0     4496 2024-05-02 14:39:30.000000 desalsim-0.7.1/tests/med_unit_f.py
--rw-rw-rw-   0        0        0     1555 2024-05-03 14:28:38.000000 desalsim-0.7.1/tests/med_unittest.py
--rw-rw-rw-   0        0        0    10407 2024-05-03 12:57:15.000000 desalsim-0.7.1/tests/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     2743 2024-05-03 12:56:18.000000 desalsim-0.7.1/tests/mfpfr_unittest.py
--rw-rw-rw-   0        0        0     6961 2024-05-06 08:40:27.000000 desalsim-0.7.1/tests/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     1777 2024-05-06 08:40:55.000000 desalsim-0.7.1/tests/nanofiltration_unittest.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.1/tests/scaleup.py
--rw-rw-rw-   0        0        0     8687 2024-05-05 10:31:06.000000 desalsim-0.7.1/tests/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     4560 2024-05-05 10:30:42.000000 desalsim-0.7.1/tests/thermal_cryst_unittest.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:34:08.887733 desalsim-0.7.2/
+drwxrwxrwx   0        0        0        0 2024-05-08 07:34:08.883504 desalsim-0.7.2/DesalSim.egg-info/
+-rw-rw-rw-   0        0        0     9945 2024-05-08 07:34:08.000000 desalsim-0.7.2/DesalSim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1276 2024-05-08 07:34:08.000000 desalsim-0.7.2/DesalSim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 07:34:08.000000 desalsim-0.7.2/DesalSim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-08 07:34:08.000000 desalsim-0.7.2/DesalSim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-08 07:34:08.000000 desalsim-0.7.2/DesalSim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 07:34:08.799259 desalsim-0.7.2/Desalsim/
+-rw-rw-rw-   0        0        0      786 2024-05-08 06:54:35.000000 desalsim-0.7.2/Desalsim/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.7.2/Desalsim/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.2/Desalsim/density_calc.py
+-rw-rw-rw-   0        0        0     8821 2024-05-06 16:12:13.000000 desalsim-0.7.2/Desalsim/economic_f.py
+-rw-rw-rw-   0        0        0     2950 2024-04-29 20:32:39.000000 desalsim-0.7.2/Desalsim/ed_unit_f.py
+-rw-rw-rw-   0        0        0    11744 2024-04-29 21:17:33.000000 desalsim-0.7.2/Desalsim/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.7.2/Desalsim/efc_unit_f.py
+-rw-rw-rw-   0        0        0     4494 2024-04-29 20:24:16.000000 desalsim-0.7.2/Desalsim/med_unit_f.py
+-rw-rw-rw-   0        0        0    10049 2024-04-29 21:14:03.000000 desalsim-0.7.2/Desalsim/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     6997 2024-05-08 07:33:43.000000 desalsim-0.7.2/Desalsim/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.7.2/Desalsim/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.2/Desalsim/scaleup.py
+-rw-rw-rw-   0        0        0     8692 2024-04-29 19:44:35.000000 desalsim-0.7.2/Desalsim/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0     9945 2024-05-08 07:34:08.885680 desalsim-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9618 2024-05-08 07:10:33.000000 desalsim-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 07:34:08.837142 desalsim-0.7.2/example/
+-rw-rw-rw-   0        0        0      786 2024-05-08 06:57:43.000000 desalsim-0.7.2/example/__init__.py
+-rw-rw-rw-   0        0        0     4531 2024-04-11 13:19:36.000000 desalsim-0.7.2/example/comparison.py
+-rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-0.7.2/example/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.2/example/density_calc.py
+-rw-rw-rw-   0        0        0    11978 2024-05-06 16:09:51.000000 desalsim-0.7.2/example/economic_f.py
+-rw-rw-rw-   0        0        0     8663 2024-04-29 21:33:04.000000 desalsim-0.7.2/example/ed_unit_f.py
+-rw-rw-rw-   0        0        0    17118 2024-04-29 21:35:34.000000 desalsim-0.7.2/example/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.7.2/example/efc_unit_f.py
+-rw-rw-rw-   0        0        0    33181 2024-05-06 17:04:03.000000 desalsim-0.7.2/example/example_1.py
+-rw-rw-rw-   0        0        0    21599 2024-05-06 16:29:23.000000 desalsim-0.7.2/example/example_2.py
+-rw-rw-rw-   0        0        0     8532 2024-04-29 21:36:53.000000 desalsim-0.7.2/example/med_unit_f.py
+-rw-rw-rw-   0        0        0    14921 2024-05-03 08:06:32.000000 desalsim-0.7.2/example/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     9421 2024-05-06 08:39:39.000000 desalsim-0.7.2/example/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.7.2/example/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.2/example/scaleup.py
+-rw-rw-rw-   0        0        0    12262 2024-04-29 21:44:17.000000 desalsim-0.7.2/example/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 07:34:08.888490 desalsim-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      611 2024-05-08 07:33:59.000000 desalsim-0.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:34:08.880512 desalsim-0.7.2/tests/
+-rw-rw-rw-   0        0        0      790 2024-05-08 06:58:06.000000 desalsim-0.7.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.7.2/tests/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.7.2/tests/density_calc.py
+-rw-rw-rw-   0        0        0     9094 2024-05-06 16:12:45.000000 desalsim-0.7.2/tests/economic_f.py
+-rw-rw-rw-   0        0        0     2527 2024-05-06 16:15:02.000000 desalsim-0.7.2/tests/economic_unittest.py
+-rw-rw-rw-   0        0        0     3255 2024-05-03 14:14:54.000000 desalsim-0.7.2/tests/ed_unit_f.py
+-rw-rw-rw-   0        0        0     3316 2024-05-03 14:16:37.000000 desalsim-0.7.2/tests/ed_unittest.py
+-rw-rw-rw-   0        0        0    12680 2024-05-03 13:51:25.000000 desalsim-0.7.2/tests/edbm_unit_f.py
+-rw-rw-rw-   0        0        0     8386 2024-05-03 13:50:48.000000 desalsim-0.7.2/tests/edbm_unittest.py
+-rw-rw-rw-   0        0        0     4496 2024-05-02 14:39:30.000000 desalsim-0.7.2/tests/med_unit_f.py
+-rw-rw-rw-   0        0        0     1555 2024-05-03 14:28:38.000000 desalsim-0.7.2/tests/med_unittest.py
+-rw-rw-rw-   0        0        0    10407 2024-05-03 12:57:15.000000 desalsim-0.7.2/tests/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     2743 2024-05-03 12:56:18.000000 desalsim-0.7.2/tests/mfpfr_unittest.py
+-rw-rw-rw-   0        0        0     6961 2024-05-06 08:40:27.000000 desalsim-0.7.2/tests/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     1777 2024-05-06 08:40:55.000000 desalsim-0.7.2/tests/nanofiltration_unittest.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.7.2/tests/scaleup.py
+-rw-rw-rw-   0        0        0     8687 2024-05-05 10:31:06.000000 desalsim-0.7.2/tests/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0     4560 2024-05-05 10:30:42.000000 desalsim-0.7.2/tests/thermal_cryst_unittest.py
```

### Comparing `desalsim-0.7.1/DesalSim.egg-info/PKG-INFO` & `desalsim-0.7.2/DesalSim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DesalSim
-Version: 0.7.1
+Version: 0.7.2
 Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 Author: rodoulak
 Author-email: r.ktori@tudelft.nl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.0
```

### Comparing `desalsim-0.7.1/DesalSim.egg-info/SOURCES.txt` & `desalsim-0.7.2/DesalSim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/Desalsim/__init__.py` & `desalsim-0.7.2/Desalsim/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/Desalsim/constants.py` & `desalsim-0.7.2/Desalsim/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/Desalsim/economic_f.py` & `desalsim-0.7.2/Desalsim/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/Desalsim/ed_unit_f.py` & `desalsim-0.7.2/Desalsim/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/Desalsim/edbm_unit_f.py` & `desalsim-0.7.2/Desalsim/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/Desalsim/efc_unit_f.py` & `desalsim-0.7.2/Desalsim/efc_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/Desalsim/med_unit_f.py` & `desalsim-0.7.2/Desalsim/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/Desalsim/mfpfr_unit_f.py` & `desalsim-0.7.2/Desalsim/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/Desalsim/nanofiltration_unit_f.py` & `desalsim-0.7.2/tests/nanofiltration_unit_f.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
 MW_Ca=constants.MW_Ca
 MW_Mg=constants.MW_Mg
 MW_HCO3=constants.MW_HCO3
 MW_values = [MW_Na, MW_Cl, MW_K, MW_Mg, MW_Ca, MW_SO4]
-                
-        
+
 #%%
 class NFMass:
     """
     A class used to represent Mass Balance for Nanofiltration Unit
 
     ...
```

### Comparing `desalsim-0.7.1/Desalsim/ro_unit_f.py` & `desalsim-0.7.2/Desalsim/ro_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/Desalsim/thermal_cryst_f.py` & `desalsim-0.7.2/Desalsim/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/LICENSE` & `desalsim-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/PKG-INFO` & `desalsim-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DesalSim
-Version: 0.7.1
+Version: 0.7.2
 Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 Author: rodoulak
 Author-email: r.ktori@tudelft.nl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.0
```

### Comparing `desalsim-0.7.1/README.md` & `desalsim-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/example/__init__.py` & `desalsim-0.7.2/example/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/example/comparison.py` & `desalsim-0.7.2/example/comparison.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/example/constants.py` & `desalsim-0.7.2/example/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/example/economic_f.py` & `desalsim-0.7.2/example/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/example/ed_unit_f.py` & `desalsim-0.7.2/example/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/example/edbm_unit_f.py` & `desalsim-0.7.2/example/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/example/efc_unit_f.py` & `desalsim-0.7.2/example/efc_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/example/example_1.py` & `desalsim-0.7.2/example/example_1.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/example/example_2.py` & `desalsim-0.7.2/example/example_2.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/example/med_unit_f.py` & `desalsim-0.7.2/example/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/example/mfpfr_unit_f.py` & `desalsim-0.7.2/example/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/example/nanofiltration_unit_f.py` & `desalsim-0.7.2/example/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/example/ro_unit_f.py` & `desalsim-0.7.2/example/ro_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/example/thermal_cryst_f.py` & `desalsim-0.7.2/example/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/setup.py` & `desalsim-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f: 
     description =f.read()
 
 setup(
       name='DesalSim',
-      version='0.7.1',
+      version='0.7.2',
       packages=find_packages(),
       url="https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-",
       author="rodoulak",
       author_email="r.ktori@tudelft.nl",
       license="MIT",
       install_requires=[
           "numpy>=1.0",
```

### Comparing `desalsim-0.7.1/tests/__init__.py` & `desalsim-0.7.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/tests/constants.py` & `desalsim-0.7.2/tests/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/tests/economic_f.py` & `desalsim-0.7.2/tests/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/tests/economic_unittest.py` & `desalsim-0.7.2/tests/economic_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/tests/ed_unit_f.py` & `desalsim-0.7.2/tests/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/tests/ed_unittest.py` & `desalsim-0.7.2/tests/ed_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/tests/edbm_unit_f.py` & `desalsim-0.7.2/tests/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/tests/edbm_unittest.py` & `desalsim-0.7.2/tests/edbm_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/tests/med_unit_f.py` & `desalsim-0.7.2/tests/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/tests/med_unittest.py` & `desalsim-0.7.2/tests/med_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/tests/mfpfr_unit_f.py` & `desalsim-0.7.2/tests/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/tests/mfpfr_unittest.py` & `desalsim-0.7.2/tests/mfpfr_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/tests/nanofiltration_unit_f.py` & `desalsim-0.7.2/Desalsim/nanofiltration_unit_f.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import math
 import numpy as np
-from density_calc import density_calc
+from Desalsim.density_calc import density_calc 
 import constants 
 import math
 #
     #molecular weight
 MW_Na=constants.MW_Na
 MW_Cl=constants.MW_cl
 MW_SO4=constants.MW_so4
 MW_K=constants.MW_K
 MW_Ca=constants.MW_Ca
 MW_Mg=constants.MW_Mg
 MW_HCO3=constants.MW_HCO3
 MW_values = [MW_Na, MW_Cl, MW_K, MW_Mg, MW_Ca, MW_SO4]
-
+                
+        
 #%%
 class NFMass:
     """
     A class used to represent Mass Balance for Nanofiltration Unit
 
     ...
```

### Comparing `desalsim-0.7.1/tests/nanofiltration_unittest.py` & `desalsim-0.7.2/tests/nanofiltration_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/tests/thermal_cryst_f.py` & `desalsim-0.7.2/tests/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.7.1/tests/thermal_cryst_unittest.py` & `desalsim-0.7.2/tests/thermal_cryst_unittest.py`

 * *Files identical despite different names*

