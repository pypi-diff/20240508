# Comparing `tmp/civilpy-0.0.80.tar.gz` & `tmp/civilpy-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civilpy-0.0.80.tar", last modified: Thu May  2 14:46:11 2024, max compression
+gzip compressed data, was "civilpy-0.0.81.tar", last modified: Wed May  8 03:53:21 2024, max compression
```

## Comparing `civilpy-0.0.80.tar` & `civilpy-0.0.81.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:46:11.523491 civilpy-0.0.80/
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-03-08 14:57:28.000000 civilpy-0.0.80/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6695 2024-05-02 14:46:11.523491 civilpy-0.0.80/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4397 2024-03-08 14:57:28.000000 civilpy-0.0.80/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 14:46:11.523491 civilpy-0.0.80/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3060 2024-05-02 12:47:43.000000 civilpy-0.0.80/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:46:11.515491 civilpy-0.0.80/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:46:11.519491 civilpy-0.0.80/src/civilpy/
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/CLI.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:46:11.519491 civilpy-0.0.80/src/civilpy/construction/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/construction/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:46:11.519491 civilpy-0.0.80/src/civilpy/environmental/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/environmental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:46:11.519491 civilpy-0.0.80/src/civilpy/general/
--rw-rw-rw-   0 root         (0) root         (0)      274 2024-03-27 10:49:10.000000 civilpy-0.0.80/src/civilpy/general/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      853 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/general/database_tools.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 14:45:44.000000 civilpy-0.0.80/src/civilpy/general/gis.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 14:45:44.000000 civilpy-0.0.80/src/civilpy/general/kml_tools.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 14:45:44.000000 civilpy-0.0.80/src/civilpy/general/math.py
--rw-rw-rw-   0 root         (0) root         (0)     5919 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/general/microstation.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 14:45:44.000000 civilpy-0.0.80/src/civilpy/general/pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     9875 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/general/photos.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 14:45:44.000000 civilpy-0.0.80/src/civilpy/general/physics.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 14:45:44.000000 civilpy-0.0.80/src/civilpy/general/plan_development.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/general/pointclouds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:46:11.519491 civilpy-0.0.80/src/civilpy/geotechnical/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/geotechnical/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:46:11.519491 civilpy-0.0.80/src/civilpy/state/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 14:45:44.000000 civilpy-0.0.80/src/civilpy/state/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:46:11.519491 civilpy-0.0.80/src/civilpy/state/ohio/
--rw-rw-rw-   0 root         (0) root         (0)     2607 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/state/ohio/D6_file_explorer.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/state/ohio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42166 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/state/ohio/dot.py
--rw-rw-rw-   0 root         (0) root         (0)    16531 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/state/ohio/search_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    91957 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/state/ohio/snbi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:46:11.523491 civilpy-0.0.80/src/civilpy/structural/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 14:45:44.000000 civilpy-0.0.80/src/civilpy/structural/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14167 2024-04-04 19:12:50.000000 civilpy-0.0.80/src/civilpy/structural/arema.py
--rw-rw-rw-   0 root         (0) root         (0)    20863 2024-04-04 19:12:50.000000 civilpy-0.0.80/src/civilpy/structural/beam_bending.py
--rw-rw-rw-   0 root         (0) root         (0)     8467 2024-04-11 05:46:12.000000 civilpy-0.0.80/src/civilpy/structural/midas.py
--rw-rw-rw-   0 root         (0) root         (0)    75517 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/structural/rail_tpg_design.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:46:11.523491 civilpy-0.0.80/src/civilpy/structural/res/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 14:45:44.000000 civilpy-0.0.80/src/civilpy/structural/res/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6559 2024-04-10 14:26:23.000000 civilpy-0.0.80/src/civilpy/structural/res/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)    18307 2024-04-10 14:26:23.000000 civilpy-0.0.80/src/civilpy/structural/steel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:46:11.523491 civilpy-0.0.80/src/civilpy/transportation/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/transportation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:46:11.523491 civilpy-0.0.80/src/civilpy/water_resources/
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/water_resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18050 2024-03-08 14:57:32.000000 civilpy-0.0.80/src/civilpy/water_resources/hydraulics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:46:11.523491 civilpy-0.0.80/src/civilpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6695 2024-05-02 14:46:11.000000 civilpy-0.0.80/src/civilpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1334 2024-05-02 14:46:11.000000 civilpy-0.0.80/src/civilpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 14:46:11.000000 civilpy-0.0.80/src/civilpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      719 2024-05-02 14:46:11.000000 civilpy-0.0.80/src/civilpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-02 14:46:11.000000 civilpy-0.0.80/src/civilpy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.297059 civilpy-0.0.81/
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-03-08 14:57:28.000000 civilpy-0.0.81/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6696 2024-05-08 03:53:21.293059 civilpy-0.0.81/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4397 2024-03-08 14:57:28.000000 civilpy-0.0.81/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 03:53:21.297059 civilpy-0.0.81/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2024-05-08 00:47:47.000000 civilpy-0.0.81/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.285059 civilpy-0.0.81/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.289059 civilpy-0.0.81/src/civilpy/
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-08 00:47:47.000000 civilpy-0.0.81/src/civilpy/CLI.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.289059 civilpy-0.0.81/src/civilpy/construction/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/construction/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.289059 civilpy-0.0.81/src/civilpy/environmental/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/environmental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.289059 civilpy-0.0.81/src/civilpy/general/
+-rw-rw-rw-   0 root         (0) root         (0)      274 2024-03-27 10:49:10.000000 civilpy-0.0.81/src/civilpy/general/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      853 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/general/database_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/general/gis.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/general/kml_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/general/math.py
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/general/microstation.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/general/pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     9875 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/general/photos.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/general/physics.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/general/plan_development.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/general/pointclouds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.289059 civilpy-0.0.81/src/civilpy/geotechnical/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/geotechnical/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.289059 civilpy-0.0.81/src/civilpy/state/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/state/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.289059 civilpy-0.0.81/src/civilpy/state/ohio/
+-rw-rw-rw-   0 root         (0) root         (0)     2607 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/state/ohio/D6_file_explorer.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/state/ohio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42166 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/state/ohio/dot.py
+-rw-rw-rw-   0 root         (0) root         (0)    16531 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/state/ohio/search_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    91957 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/state/ohio/snbi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.293059 civilpy-0.0.81/src/civilpy/structural/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/structural/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14167 2024-04-04 19:12:50.000000 civilpy-0.0.81/src/civilpy/structural/arema.py
+-rw-rw-rw-   0 root         (0) root         (0)    20863 2024-04-04 19:12:50.000000 civilpy-0.0.81/src/civilpy/structural/beam_bending.py
+-rw-rw-rw-   0 root         (0) root         (0)     8467 2024-04-11 05:46:12.000000 civilpy-0.0.81/src/civilpy/structural/midas.py
+-rw-rw-rw-   0 root         (0) root         (0)    75517 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/structural/rail_tpg_design.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.293059 civilpy-0.0.81/src/civilpy/structural/res/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/structural/res/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6559 2024-04-10 14:26:23.000000 civilpy-0.0.81/src/civilpy/structural/res/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)    18307 2024-04-10 14:26:23.000000 civilpy-0.0.81/src/civilpy/structural/steel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.293059 civilpy-0.0.81/src/civilpy/transportation/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/transportation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.293059 civilpy-0.0.81/src/civilpy/water_resources/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/water_resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18050 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/water_resources/hydraulics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.293059 civilpy-0.0.81/src/civilpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6696 2024-05-08 03:53:21.000000 civilpy-0.0.81/src/civilpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1334 2024-05-08 03:53:21.000000 civilpy-0.0.81/src/civilpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 03:53:21.000000 civilpy-0.0.81/src/civilpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      720 2024-05-08 03:53:21.000000 civilpy-0.0.81/src/civilpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-08 03:53:21.000000 civilpy-0.0.81/src/civilpy.egg-info/top_level.txt
```

### Comparing `civilpy-0.0.80/LICENSE` & `civilpy-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/PKG-INFO` & `civilpy-0.0.81/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.80
+Version: 0.0.81
 Summary: Civil Engineering Tools in Python
 Home-page: https://daneparks.com/Dane/civilpy
 Author: Dane Parks
 Author-email: Dane@daneparks.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -15,15 +15,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console :: Curses
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.14.5
 Requires-Dist: folium>=0.12.1
 Requires-Dist: pandas>=1.1.5
-Requires-Dist: Pillow>=9.4.0
+Requires-Dist: Pillow>=10.2.0
 Requires-Dist: Pint>=0.12.2
 Requires-Dist: coverage>=7.1.0
 Requires-Dist: webdriver-manager>=3.8.5
 Requires-Dist: msedge-selenium-tools>=3.141.4
 Requires-Dist: Flask>=2.2.2
 Requires-Dist: PyPDF2>=3.0.1
 Requires-Dist: beautifulsoup4>=4.11.1
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.80 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.81 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
 Parks Author-email: Dane@daneparks.com License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Classifier: Environment :: Console :: Curses
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy>=1.14.5 Requires-Dist: folium>=0.12.1 Requires-Dist: pandas>=1.1.5
-Requires-Dist: Pillow>=9.4.0 Requires-Dist: Pint>=0.12.2 Requires-Dist:
+Requires-Dist: Pillow>=10.2.0 Requires-Dist: Pint>=0.12.2 Requires-Dist:
 coverage>=7.1.0 Requires-Dist: webdriver-manager>=3.8.5 Requires-Dist: msedge-
 selenium-tools>=3.141.4 Requires-Dist: Flask>=2.2.2 Requires-Dist:
 PyPDF2>=3.0.1 Requires-Dist: beautifulsoup4>=4.11.1 Requires-Dist:
 sympy>=1.10.0 Requires-Dist: sshtunnel>=0.4.0 Requires-Dist: termcolor>=1.1.0
 Requires-Dist: icalendar>=4.0.7 Requires-Dist: html5lib>=1.1 Requires-Dist:
 geopandas>=0.6.2 Requires-Dist: fiona>=1.8.22 Requires-Dist: tifftools>=1.3.7
 Requires-Dist: natsort>=8.2.0 Requires-Dist: html5lib>=1.1 Requires-Dist:
```

### Comparing `civilpy-0.0.80/README.md` & `civilpy-0.0.81/README.md`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/setup.py` & `civilpy-0.0.81/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='civilpy',
-    version='0.0.80',
+    version='0.0.81',
     packages=find_packages('src', exclude=['test', 'Notebooks', 'secrets', 'docs', 'res']),
     description='Civil Engineering Tools in Python',
     url="https://daneparks.com/Dane/civilpy",
     author_email="Dane@daneparks.com",
     author="Dane Parks",
     license='MIT',
     py_modules=[
@@ -46,15 +46,15 @@
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "numpy>=1.14.5",
         "folium>=0.12.1",
         "pandas>=1.1.5",
-        "Pillow>=9.4.0",
+        "Pillow>=10.2.0",
         "Pint>=0.12.2",
         "coverage>=7.1.0",
         "webdriver-manager>=3.8.5",
         "msedge-selenium-tools>=3.141.4",
         "Flask>=2.2.2",
         "PyPDF2>=3.0.1",
         "beautifulsoup4>=4.11.1",
```

### Comparing `civilpy-0.0.80/src/civilpy/general/database_tools.py` & `civilpy-0.0.81/src/civilpy/general/database_tools.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/src/civilpy/general/microstation.py` & `civilpy-0.0.81/src/civilpy/general/microstation.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/src/civilpy/general/photos.py` & `civilpy-0.0.81/src/civilpy/general/photos.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/src/civilpy/state/ohio/D6_file_explorer.py` & `civilpy-0.0.81/src/civilpy/state/ohio/D6_file_explorer.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/src/civilpy/state/ohio/dot.py` & `civilpy-0.0.81/src/civilpy/state/ohio/dot.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/src/civilpy/state/ohio/search_tools.py` & `civilpy-0.0.81/src/civilpy/state/ohio/search_tools.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/src/civilpy/state/ohio/snbi.py` & `civilpy-0.0.81/src/civilpy/state/ohio/snbi.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/src/civilpy/structural/arema.py` & `civilpy-0.0.81/src/civilpy/structural/arema.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/src/civilpy/structural/beam_bending.py` & `civilpy-0.0.81/src/civilpy/structural/beam_bending.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/src/civilpy/structural/midas.py` & `civilpy-0.0.81/src/civilpy/structural/midas.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/src/civilpy/structural/rail_tpg_design.py` & `civilpy-0.0.81/src/civilpy/structural/rail_tpg_design.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/src/civilpy/structural/res/definitions.py` & `civilpy-0.0.81/src/civilpy/structural/res/definitions.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/src/civilpy/structural/steel.py` & `civilpy-0.0.81/src/civilpy/structural/steel.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/src/civilpy/water_resources/hydraulics.py` & `civilpy-0.0.81/src/civilpy/water_resources/hydraulics.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/src/civilpy.egg-info/PKG-INFO` & `civilpy-0.0.81/src/civilpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.80
+Version: 0.0.81
 Summary: Civil Engineering Tools in Python
 Home-page: https://daneparks.com/Dane/civilpy
 Author: Dane Parks
 Author-email: Dane@daneparks.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -15,15 +15,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console :: Curses
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.14.5
 Requires-Dist: folium>=0.12.1
 Requires-Dist: pandas>=1.1.5
-Requires-Dist: Pillow>=9.4.0
+Requires-Dist: Pillow>=10.2.0
 Requires-Dist: Pint>=0.12.2
 Requires-Dist: coverage>=7.1.0
 Requires-Dist: webdriver-manager>=3.8.5
 Requires-Dist: msedge-selenium-tools>=3.141.4
 Requires-Dist: Flask>=2.2.2
 Requires-Dist: PyPDF2>=3.0.1
 Requires-Dist: beautifulsoup4>=4.11.1
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.80 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.81 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
 Parks Author-email: Dane@daneparks.com License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Classifier: Environment :: Console :: Curses
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy>=1.14.5 Requires-Dist: folium>=0.12.1 Requires-Dist: pandas>=1.1.5
-Requires-Dist: Pillow>=9.4.0 Requires-Dist: Pint>=0.12.2 Requires-Dist:
+Requires-Dist: Pillow>=10.2.0 Requires-Dist: Pint>=0.12.2 Requires-Dist:
 coverage>=7.1.0 Requires-Dist: webdriver-manager>=3.8.5 Requires-Dist: msedge-
 selenium-tools>=3.141.4 Requires-Dist: Flask>=2.2.2 Requires-Dist:
 PyPDF2>=3.0.1 Requires-Dist: beautifulsoup4>=4.11.1 Requires-Dist:
 sympy>=1.10.0 Requires-Dist: sshtunnel>=0.4.0 Requires-Dist: termcolor>=1.1.0
 Requires-Dist: icalendar>=4.0.7 Requires-Dist: html5lib>=1.1 Requires-Dist:
 geopandas>=0.6.2 Requires-Dist: fiona>=1.8.22 Requires-Dist: tifftools>=1.3.7
 Requires-Dist: natsort>=8.2.0 Requires-Dist: html5lib>=1.1 Requires-Dist:
```

### Comparing `civilpy-0.0.80/src/civilpy.egg-info/SOURCES.txt` & `civilpy-0.0.81/src/civilpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.80/src/civilpy.egg-info/requires.txt` & `civilpy-0.0.81/src/civilpy.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 numpy>=1.14.5
 folium>=0.12.1
 pandas>=1.1.5
-Pillow>=9.4.0
+Pillow>=10.2.0
 Pint>=0.12.2
 coverage>=7.1.0
 webdriver-manager>=3.8.5
 msedge-selenium-tools>=3.141.4
 Flask>=2.2.2
 PyPDF2>=3.0.1
 beautifulsoup4>=4.11.1
```

