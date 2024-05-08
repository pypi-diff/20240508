# Comparing `tmp/desalsim-0.5.tar.gz` & `tmp/desalsim-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desalsim-0.5.tar", last modified: Tue May  7 13:42:02 2024, max compression
+gzip compressed data, was "desalsim-0.6.tar", last modified: Wed May  8 07:02:14 2024, max compression
```

## Comparing `desalsim-0.5.tar` & `desalsim-0.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 13:42:02.531330 desalsim-0.5/
-drwxrwxrwx   0        0        0        0 2024-05-07 13:42:02.523122 desalsim-0.5/DesalSim.egg-info/
--rw-rw-rw-   0        0        0     9718 2024-05-07 13:42:02.000000 desalsim-0.5/DesalSim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1276 2024-05-07 13:42:02.000000 desalsim-0.5/DesalSim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 13:42:02.000000 desalsim-0.5/DesalSim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-07 13:42:02.000000 desalsim-0.5/DesalSim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-07 13:42:02.000000 desalsim-0.5/DesalSim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 13:42:02.477235 desalsim-0.5/Desalsim/
--rw-rw-rw-   0        0        0      797 2024-05-07 12:54:09.000000 desalsim-0.5/Desalsim/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.5/Desalsim/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.5/Desalsim/density_calc.py
--rw-rw-rw-   0        0        0     8821 2024-05-06 16:12:13.000000 desalsim-0.5/Desalsim/economic_f.py
--rw-rw-rw-   0        0        0     2950 2024-04-29 20:32:39.000000 desalsim-0.5/Desalsim/ed_unit_f.py
--rw-rw-rw-   0        0        0    11744 2024-04-29 21:17:33.000000 desalsim-0.5/Desalsim/edbm_unit_f.py
--rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.5/Desalsim/efc_unit_f.py
--rw-rw-rw-   0        0        0     4494 2024-04-29 20:24:16.000000 desalsim-0.5/Desalsim/med_unit_f.py
--rw-rw-rw-   0        0        0    10049 2024-04-29 21:14:03.000000 desalsim-0.5/Desalsim/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     6987 2024-05-06 08:40:06.000000 desalsim-0.5/Desalsim/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.5/Desalsim/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.5/Desalsim/scaleup.py
--rw-rw-rw-   0        0        0     8692 2024-04-29 19:44:35.000000 desalsim-0.5/Desalsim/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-0.5/LICENSE
--rw-rw-rw-   0        0        0     9718 2024-05-07 13:42:02.529106 desalsim-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     9393 2024-05-07 13:37:34.000000 desalsim-0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 13:42:02.498543 desalsim-0.5/example/
--rw-rw-rw-   0        0        0      797 2024-05-07 13:01:36.000000 desalsim-0.5/example/__init__.py
--rw-rw-rw-   0        0        0     4531 2024-04-11 13:19:36.000000 desalsim-0.5/example/comparison.py
--rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-0.5/example/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.5/example/density_calc.py
--rw-rw-rw-   0        0        0    11978 2024-05-06 16:09:51.000000 desalsim-0.5/example/economic_f.py
--rw-rw-rw-   0        0        0     8663 2024-04-29 21:33:04.000000 desalsim-0.5/example/ed_unit_f.py
--rw-rw-rw-   0        0        0    17118 2024-04-29 21:35:34.000000 desalsim-0.5/example/edbm_unit_f.py
--rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.5/example/efc_unit_f.py
--rw-rw-rw-   0        0        0    33181 2024-05-06 17:04:03.000000 desalsim-0.5/example/example_1.py
--rw-rw-rw-   0        0        0    21599 2024-05-06 16:29:23.000000 desalsim-0.5/example/example_2.py
--rw-rw-rw-   0        0        0     8532 2024-04-29 21:36:53.000000 desalsim-0.5/example/med_unit_f.py
--rw-rw-rw-   0        0        0    14921 2024-05-03 08:06:32.000000 desalsim-0.5/example/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     9421 2024-05-06 08:39:39.000000 desalsim-0.5/example/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.5/example/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.5/example/scaleup.py
--rw-rw-rw-   0        0        0    12262 2024-04-29 21:44:17.000000 desalsim-0.5/example/thermal_cryst_f.py
--rw-rw-rw-   0        0        0       42 2024-05-07 13:42:02.531330 desalsim-0.5/setup.cfg
--rw-rw-rw-   0        0        0      609 2024-05-07 13:41:53.000000 desalsim-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:42:02.522125 desalsim-0.5/tests/
--rw-rw-rw-   0        0        0      799 2024-05-07 12:54:02.000000 desalsim-0.5/tests/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.5/tests/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.5/tests/density_calc.py
--rw-rw-rw-   0        0        0     9094 2024-05-06 16:12:45.000000 desalsim-0.5/tests/economic_f.py
--rw-rw-rw-   0        0        0     2527 2024-05-06 16:15:02.000000 desalsim-0.5/tests/economic_unittest.py
--rw-rw-rw-   0        0        0     3255 2024-05-03 14:14:54.000000 desalsim-0.5/tests/ed_unit_f.py
--rw-rw-rw-   0        0        0     3316 2024-05-03 14:16:37.000000 desalsim-0.5/tests/ed_unittest.py
--rw-rw-rw-   0        0        0    12680 2024-05-03 13:51:25.000000 desalsim-0.5/tests/edbm_unit_f.py
--rw-rw-rw-   0        0        0     8386 2024-05-03 13:50:48.000000 desalsim-0.5/tests/edbm_unittest.py
--rw-rw-rw-   0        0        0     4496 2024-05-02 14:39:30.000000 desalsim-0.5/tests/med_unit_f.py
--rw-rw-rw-   0        0        0     1555 2024-05-03 14:28:38.000000 desalsim-0.5/tests/med_unittest.py
--rw-rw-rw-   0        0        0    10407 2024-05-03 12:57:15.000000 desalsim-0.5/tests/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     2743 2024-05-03 12:56:18.000000 desalsim-0.5/tests/mfpfr_unittest.py
--rw-rw-rw-   0        0        0     6961 2024-05-06 08:40:27.000000 desalsim-0.5/tests/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     1777 2024-05-06 08:40:55.000000 desalsim-0.5/tests/nanofiltration_unittest.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.5/tests/scaleup.py
--rw-rw-rw-   0        0        0     8687 2024-05-05 10:31:06.000000 desalsim-0.5/tests/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     4560 2024-05-05 10:30:42.000000 desalsim-0.5/tests/thermal_cryst_unittest.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:02:14.593114 desalsim-0.6/
+drwxrwxrwx   0        0        0        0 2024-05-08 07:02:14.588121 desalsim-0.6/DesalSim.egg-info/
+-rw-rw-rw-   0        0        0     9943 2024-05-08 07:02:14.000000 desalsim-0.6/DesalSim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1276 2024-05-08 07:02:14.000000 desalsim-0.6/DesalSim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 07:02:14.000000 desalsim-0.6/DesalSim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-08 07:02:14.000000 desalsim-0.6/DesalSim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-08 07:02:14.000000 desalsim-0.6/DesalSim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 07:02:14.495993 desalsim-0.6/Desalsim/
+-rw-rw-rw-   0        0        0      786 2024-05-08 06:54:35.000000 desalsim-0.6/Desalsim/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.6/Desalsim/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.6/Desalsim/density_calc.py
+-rw-rw-rw-   0        0        0     8821 2024-05-06 16:12:13.000000 desalsim-0.6/Desalsim/economic_f.py
+-rw-rw-rw-   0        0        0     2950 2024-04-29 20:32:39.000000 desalsim-0.6/Desalsim/ed_unit_f.py
+-rw-rw-rw-   0        0        0    11744 2024-04-29 21:17:33.000000 desalsim-0.6/Desalsim/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.6/Desalsim/efc_unit_f.py
+-rw-rw-rw-   0        0        0     4494 2024-04-29 20:24:16.000000 desalsim-0.6/Desalsim/med_unit_f.py
+-rw-rw-rw-   0        0        0    10049 2024-04-29 21:14:03.000000 desalsim-0.6/Desalsim/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     6987 2024-05-06 08:40:06.000000 desalsim-0.6/Desalsim/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.6/Desalsim/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.6/Desalsim/scaleup.py
+-rw-rw-rw-   0        0        0     8692 2024-04-29 19:44:35.000000 desalsim-0.6/Desalsim/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-0.6/LICENSE
+-rw-rw-rw-   0        0        0     9943 2024-05-08 07:02:14.589120 desalsim-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9618 2024-05-07 15:23:34.000000 desalsim-0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 07:02:14.541303 desalsim-0.6/example/
+-rw-rw-rw-   0        0        0      786 2024-05-08 06:57:43.000000 desalsim-0.6/example/__init__.py
+-rw-rw-rw-   0        0        0     4531 2024-04-11 13:19:36.000000 desalsim-0.6/example/comparison.py
+-rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-0.6/example/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.6/example/density_calc.py
+-rw-rw-rw-   0        0        0    11978 2024-05-06 16:09:51.000000 desalsim-0.6/example/economic_f.py
+-rw-rw-rw-   0        0        0     8663 2024-04-29 21:33:04.000000 desalsim-0.6/example/ed_unit_f.py
+-rw-rw-rw-   0        0        0    17118 2024-04-29 21:35:34.000000 desalsim-0.6/example/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    49286 2024-02-14 10:34:47.000000 desalsim-0.6/example/efc_unit_f.py
+-rw-rw-rw-   0        0        0    33181 2024-05-06 17:04:03.000000 desalsim-0.6/example/example_1.py
+-rw-rw-rw-   0        0        0    21599 2024-05-06 16:29:23.000000 desalsim-0.6/example/example_2.py
+-rw-rw-rw-   0        0        0     8532 2024-04-29 21:36:53.000000 desalsim-0.6/example/med_unit_f.py
+-rw-rw-rw-   0        0        0    14921 2024-05-03 08:06:32.000000 desalsim-0.6/example/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     9421 2024-05-06 08:39:39.000000 desalsim-0.6/example/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     4366 2024-04-29 21:19:41.000000 desalsim-0.6/example/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.6/example/scaleup.py
+-rw-rw-rw-   0        0        0    12262 2024-04-29 21:44:17.000000 desalsim-0.6/example/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 07:02:14.594110 desalsim-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      609 2024-05-08 07:02:04.000000 desalsim-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:02:14.585159 desalsim-0.6/tests/
+-rw-rw-rw-   0        0        0      790 2024-05-08 06:58:06.000000 desalsim-0.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-0.6/tests/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-0.6/tests/density_calc.py
+-rw-rw-rw-   0        0        0     9094 2024-05-06 16:12:45.000000 desalsim-0.6/tests/economic_f.py
+-rw-rw-rw-   0        0        0     2527 2024-05-06 16:15:02.000000 desalsim-0.6/tests/economic_unittest.py
+-rw-rw-rw-   0        0        0     3255 2024-05-03 14:14:54.000000 desalsim-0.6/tests/ed_unit_f.py
+-rw-rw-rw-   0        0        0     3316 2024-05-03 14:16:37.000000 desalsim-0.6/tests/ed_unittest.py
+-rw-rw-rw-   0        0        0    12680 2024-05-03 13:51:25.000000 desalsim-0.6/tests/edbm_unit_f.py
+-rw-rw-rw-   0        0        0     8386 2024-05-03 13:50:48.000000 desalsim-0.6/tests/edbm_unittest.py
+-rw-rw-rw-   0        0        0     4496 2024-05-02 14:39:30.000000 desalsim-0.6/tests/med_unit_f.py
+-rw-rw-rw-   0        0        0     1555 2024-05-03 14:28:38.000000 desalsim-0.6/tests/med_unittest.py
+-rw-rw-rw-   0        0        0    10407 2024-05-03 12:57:15.000000 desalsim-0.6/tests/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     2743 2024-05-03 12:56:18.000000 desalsim-0.6/tests/mfpfr_unittest.py
+-rw-rw-rw-   0        0        0     6961 2024-05-06 08:40:27.000000 desalsim-0.6/tests/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     1777 2024-05-06 08:40:55.000000 desalsim-0.6/tests/nanofiltration_unittest.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-0.6/tests/scaleup.py
+-rw-rw-rw-   0        0        0     8687 2024-05-05 10:31:06.000000 desalsim-0.6/tests/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0     4560 2024-05-05 10:30:42.000000 desalsim-0.6/tests/thermal_cryst_unittest.py
```

### Comparing `desalsim-0.5/DesalSim.egg-info/PKG-INFO` & `desalsim-0.6/DesalSim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DesalSim
-Version: 0.5
+Version: 0.6
 Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 Author: rodoulak
 Author-email: r.ktori@tudelft.nl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.0
@@ -61,21 +61,21 @@
 - `density_calc.py`: This file contains the main script for calculating density of a solution based on the tempretaure and the concentration of the solution.
 - `scaleup.py`: This file contains the main script for scaling-up a technology with known capacity using the six-tenths factor rule (m=0.6).
 - `LICENSE`: License file containing the MIT License terms.
 
 ## Installation  
 The easiest way is through pip, in command-line interface:   
 ```
-pip install DesalSim==0.2
+pip install DesalSim==0.5
 ```
 
 If you want to install the latest GitHub verstion:
-1. Clone the repository to your local machine:
+1. Download the repository to your local machine:
 ```
-git clone https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main
+https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 ```
 2. Install the required dependencies:
  ```
 pip install -r requirements.txt
  ```
 
 ## Usage 
@@ -97,14 +97,16 @@
 2. [Tutorial for Example 1](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Example_1_Tutorial.md)
 3. [Economic Tutorial](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Economic_Tutorial.md)
 4. The mathematical description of each technology is given in [Mathematical description](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/paper/Mathematical_description.pdf)
 5. [Example 1](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/example_1.py)
 6. [Example 2](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/example_2.py)
 7. [Scenarios comparison](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/comparison.py)
 
+Additionally, you can find tests for every process unit and the economic model in the [tests folder](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/tests) that verify that the code is running properly. 
+
 
 ## Contributing
 Contributions to the project are welcome! If you'd like to contribute, please follow the standard GitHub workflow:
 1. Fork the repository.
 2. Create a new branch (git checkout -b feature/improvement).
 3. Make your changes and commit them (git commit -am 'Add new feature').
 4. Push to the branch (git push origin feature/improvement).
```

### Comparing `desalsim-0.5/DesalSim.egg-info/SOURCES.txt` & `desalsim-0.6/DesalSim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/Desalsim/__init__.py` & `desalsim-0.6/Desalsim/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # __init__.py
+from Desalsim import density_calc
+from Desalsim import constants
+
 from Desalsim.nanofiltration_unit_f import NFMass
 from Desalsim.nanofiltration_unit_f import OsmoticPressure
 from Desalsim.nanofiltration_unit_f import NfEnergy
 
 from Desalsim.med_unit_f import MEDCalculator
 
 from Desalsim.thermal_cryst_f import thermal_calc
@@ -16,14 +19,12 @@
 from Desalsim.ed_unit_f import ElectrodialysisCalc
 
 from Desalsim.edbm_unit_f import EDBMCalc
 
 from Desalsim.economic_f import econom
 from Desalsim.economic_f import revenue
 
-from Desalsim.density_calc import density_calc
-from Desalsim import constants
```

### Comparing `desalsim-0.5/Desalsim/constants.py` & `desalsim-0.6/Desalsim/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/Desalsim/economic_f.py` & `desalsim-0.6/Desalsim/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/Desalsim/ed_unit_f.py` & `desalsim-0.6/Desalsim/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/Desalsim/edbm_unit_f.py` & `desalsim-0.6/Desalsim/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/Desalsim/efc_unit_f.py` & `desalsim-0.6/Desalsim/efc_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/Desalsim/med_unit_f.py` & `desalsim-0.6/Desalsim/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/Desalsim/mfpfr_unit_f.py` & `desalsim-0.6/Desalsim/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/Desalsim/nanofiltration_unit_f.py` & `desalsim-0.6/Desalsim/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/Desalsim/ro_unit_f.py` & `desalsim-0.6/Desalsim/ro_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/Desalsim/thermal_cryst_f.py` & `desalsim-0.6/Desalsim/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/LICENSE` & `desalsim-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/PKG-INFO` & `desalsim-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DesalSim
-Version: 0.5
+Version: 0.6
 Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 Author: rodoulak
 Author-email: r.ktori@tudelft.nl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.0
@@ -61,21 +61,21 @@
 - `density_calc.py`: This file contains the main script for calculating density of a solution based on the tempretaure and the concentration of the solution.
 - `scaleup.py`: This file contains the main script for scaling-up a technology with known capacity using the six-tenths factor rule (m=0.6).
 - `LICENSE`: License file containing the MIT License terms.
 
 ## Installation  
 The easiest way is through pip, in command-line interface:   
 ```
-pip install DesalSim==0.2
+pip install DesalSim==0.5
 ```
 
 If you want to install the latest GitHub verstion:
-1. Clone the repository to your local machine:
+1. Download the repository to your local machine:
 ```
-git clone https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main
+https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 ```
 2. Install the required dependencies:
  ```
 pip install -r requirements.txt
  ```
 
 ## Usage 
@@ -97,14 +97,16 @@
 2. [Tutorial for Example 1](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Example_1_Tutorial.md)
 3. [Economic Tutorial](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Economic_Tutorial.md)
 4. The mathematical description of each technology is given in [Mathematical description](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/paper/Mathematical_description.pdf)
 5. [Example 1](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/example_1.py)
 6. [Example 2](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/example_2.py)
 7. [Scenarios comparison](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/comparison.py)
 
+Additionally, you can find tests for every process unit and the economic model in the [tests folder](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/tests) that verify that the code is running properly. 
+
 
 ## Contributing
 Contributions to the project are welcome! If you'd like to contribute, please follow the standard GitHub workflow:
 1. Fork the repository.
 2. Create a new branch (git checkout -b feature/improvement).
 3. Make your changes and commit them (git commit -am 'Add new feature').
 4. Push to the branch (git push origin feature/improvement).
```

### Comparing `desalsim-0.5/README.md` & `desalsim-0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,21 +49,21 @@
 - `density_calc.py`: This file contains the main script for calculating density of a solution based on the tempretaure and the concentration of the solution.
 - `scaleup.py`: This file contains the main script for scaling-up a technology with known capacity using the six-tenths factor rule (m=0.6).
 - `LICENSE`: License file containing the MIT License terms.
 
 ## Installation  
 The easiest way is through pip, in command-line interface:   
 ```
-pip install DesalSim==0.2
+pip install DesalSim==0.5
 ```
 
 If you want to install the latest GitHub verstion:
-1. Clone the repository to your local machine:
+1. Download the repository to your local machine:
 ```
-git clone https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main
+https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 ```
 2. Install the required dependencies:
  ```
 pip install -r requirements.txt
  ```
 
 ## Usage 
@@ -85,14 +85,16 @@
 2. [Tutorial for Example 1](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Example_1_Tutorial.md)
 3. [Economic Tutorial](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Economic_Tutorial.md)
 4. The mathematical description of each technology is given in [Mathematical description](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/paper/Mathematical_description.pdf)
 5. [Example 1](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/example_1.py)
 6. [Example 2](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/example_2.py)
 7. [Scenarios comparison](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/comparison.py)
 
+Additionally, you can find tests for every process unit and the economic model in the [tests folder](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/tests) that verify that the code is running properly. 
+
 
 ## Contributing
 Contributions to the project are welcome! If you'd like to contribute, please follow the standard GitHub workflow:
 1. Fork the repository.
 2. Create a new branch (git checkout -b feature/improvement).
 3. Make your changes and commit them (git commit -am 'Add new feature').
 4. Push to the branch (git push origin feature/improvement).
```

### Comparing `desalsim-0.5/example/__init__.py` & `desalsim-0.6/example/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # __init__.py
+from Desalsim import density_calc
+from Desalsim import constants
+
 from Desalsim.nanofiltration_unit_f import NFMass
 from Desalsim.nanofiltration_unit_f import OsmoticPressure
 from Desalsim.nanofiltration_unit_f import NfEnergy
 
 from Desalsim.med_unit_f import MEDCalculator
 
 from Desalsim.thermal_cryst_f import thermal_calc
@@ -16,14 +19,12 @@
 from Desalsim.ed_unit_f import ElectrodialysisCalc
 
 from Desalsim.edbm_unit_f import EDBMCalc
 
 from Desalsim.economic_f import econom
 from Desalsim.economic_f import revenue
 
-from Desalsim.density_calc import density_calc
-from Desalsim import constants
```

### Comparing `desalsim-0.5/example/comparison.py` & `desalsim-0.6/example/comparison.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/example/constants.py` & `desalsim-0.6/example/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/example/economic_f.py` & `desalsim-0.6/example/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/example/ed_unit_f.py` & `desalsim-0.6/example/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/example/edbm_unit_f.py` & `desalsim-0.6/example/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/example/efc_unit_f.py` & `desalsim-0.6/example/efc_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/example/example_1.py` & `desalsim-0.6/example/example_1.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/example/example_2.py` & `desalsim-0.6/example/example_2.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/example/med_unit_f.py` & `desalsim-0.6/example/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/example/mfpfr_unit_f.py` & `desalsim-0.6/example/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/example/nanofiltration_unit_f.py` & `desalsim-0.6/example/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/example/ro_unit_f.py` & `desalsim-0.6/example/ro_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/example/thermal_cryst_f.py` & `desalsim-0.6/example/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/setup.py` & `desalsim-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f: 
     description =f.read()
 
 setup(
       name='DesalSim',
-      version='0.5',
+      version='0.6',
       packages=find_packages(),
       url="https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-",
       author="rodoulak",
       author_email="r.ktori@tudelft.nl",
       license="MIT",
       install_requires=[
           "numpy>=1.0",
```

### Comparing `desalsim-0.5/tests/__init__.py` & `desalsim-0.6/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # __init__.py
+from Desalsim import density_calc
+from Desalsim import constants
+
 from Desalsim.nanofiltration_unit_f import NFMass
 from Desalsim.nanofiltration_unit_f import OsmoticPressure
 from Desalsim.nanofiltration_unit_f import NfEnergy
 
 from Desalsim.med_unit_f import MEDCalculator
 
 from Desalsim.thermal_cryst_f import thermal_calc
@@ -16,15 +19,14 @@
 from Desalsim.ed_unit_f import ElectrodialysisCalc
 
 from Desalsim.edbm_unit_f import EDBMCalc
 
 from Desalsim.economic_f import econom
 from Desalsim.economic_f import revenue
 
-from Desalsim.density_calc import density_calc
-from Desalsim import constants
+
```

### Comparing `desalsim-0.5/tests/constants.py` & `desalsim-0.6/tests/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/tests/economic_f.py` & `desalsim-0.6/tests/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/tests/economic_unittest.py` & `desalsim-0.6/tests/economic_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/tests/ed_unit_f.py` & `desalsim-0.6/tests/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/tests/ed_unittest.py` & `desalsim-0.6/tests/ed_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/tests/edbm_unit_f.py` & `desalsim-0.6/tests/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/tests/edbm_unittest.py` & `desalsim-0.6/tests/edbm_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/tests/med_unit_f.py` & `desalsim-0.6/tests/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/tests/med_unittest.py` & `desalsim-0.6/tests/med_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/tests/mfpfr_unit_f.py` & `desalsim-0.6/tests/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/tests/mfpfr_unittest.py` & `desalsim-0.6/tests/mfpfr_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/tests/nanofiltration_unit_f.py` & `desalsim-0.6/tests/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/tests/nanofiltration_unittest.py` & `desalsim-0.6/tests/nanofiltration_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/tests/thermal_cryst_f.py` & `desalsim-0.6/tests/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-0.5/tests/thermal_cryst_unittest.py` & `desalsim-0.6/tests/thermal_cryst_unittest.py`

 * *Files identical despite different names*

