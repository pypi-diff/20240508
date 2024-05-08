# Comparing `tmp/lasertram-0.1.2.tar.gz` & `tmp/lasertram-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lasertram-0.1.2.tar", last modified: Wed May  1 23:01:30 2024, max compression
+gzip compressed data, was "lasertram-0.1.3.tar", last modified: Wed May  8 00:18:27 2024, max compression
```

## Comparing `lasertram-0.1.2.tar` & `lasertram-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:30.568239 lasertram-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 23:01:26.000000 lasertram-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-01 23:01:30.568239 lasertram-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-01 23:01:26.000000 lasertram-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:30.564239 lasertram-0.1.2/lasertram/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:30.564239 lasertram-0.1.2/lasertram/calc/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31599 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/calc/calc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:30.568239 lasertram-0.1.2/lasertram/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/helpers/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/helpers/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:30.568239 lasertram-0.1.2/lasertram/tram/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/tram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11682 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/tram/tram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:30.568239 lasertram-0.1.2/lasertram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-01 23:01:30.000000 lasertram-0.1.2/lasertram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-01 23:01:30.000000 lasertram-0.1.2/lasertram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 23:01:30.000000 lasertram-0.1.2/lasertram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-01 23:01:30.000000 lasertram-0.1.2/lasertram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 23:01:30.000000 lasertram-0.1.2/lasertram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 23:01:26.000000 lasertram-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-01 23:01:30.568239 lasertram-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:30.568239 lasertram-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-05-01 23:01:26.000000 lasertram-0.1.2/tests/test_lasertram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:18:27.831731 lasertram-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-08 00:18:23.000000 lasertram-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-08 00:18:27.831731 lasertram-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-08 00:18:23.000000 lasertram-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:18:27.827731 lasertram-0.1.3/lasertram/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 00:18:23.000000 lasertram-0.1.3/lasertram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:18:27.831731 lasertram-0.1.3/lasertram/calc/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 00:18:23.000000 lasertram-0.1.3/lasertram/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31599 2024-05-08 00:18:23.000000 lasertram-0.1.3/lasertram/calc/calc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:18:27.831731 lasertram-0.1.3/lasertram/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:18:23.000000 lasertram-0.1.3/lasertram/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-08 00:18:23.000000 lasertram-0.1.3/lasertram/helpers/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-08 00:18:23.000000 lasertram-0.1.3/lasertram/helpers/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:18:27.831731 lasertram-0.1.3/lasertram/tram/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 00:18:23.000000 lasertram-0.1.3/lasertram/tram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11682 2024-05-08 00:18:23.000000 lasertram-0.1.3/lasertram/tram/tram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:18:27.831731 lasertram-0.1.3/lasertram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-08 00:18:27.000000 lasertram-0.1.3/lasertram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-08 00:18:27.000000 lasertram-0.1.3/lasertram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:18:27.000000 lasertram-0.1.3/lasertram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-08 00:18:27.000000 lasertram-0.1.3/lasertram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 00:18:27.000000 lasertram-0.1.3/lasertram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 00:18:23.000000 lasertram-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-08 00:18:27.831731 lasertram-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:18:27.831731 lasertram-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    42438 2024-05-08 00:18:24.000000 lasertram-0.1.3/tests/test_lasertram.py
```

### Comparing `lasertram-0.1.2/PKG-INFO` & `lasertram-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasertram
-Version: 0.1.2
+Version: 0.1.3
 Summary: For processing LA-ICP-MS data
 Home-page: https://github.com/jlubbersgeo/lasertram
 Author: Jordan Lubbers
 Author-email: jelubber@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,30 +19,27 @@
 Requires-Dist: mendeleev>=0.14.0
 Requires-Dist: numpy>=1.25.2
 Requires-Dist: pandas>=2.0.3
 Requires-Dist: scipy>=1.11.1
 Requires-Dist: statsmodels>=0.14.0
 Requires-Dist: openpyxl>=3.0.0
 
-# lasertram
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) !['coverage'](/images/COVERAGE.svg)
-
+# ```lasertram```
 
 Welcome to the repository for `lasertram`, a package for the time resolved analysis for processing laser ablation inductively coupled plasma mass spectrometry (LA-ICP-MS) data. It is utilized heavily in the dashboard [LaserTRAM-DB](https://github.com/jlubbersgeo/laserTRAM-DB).
 
 ## Documentation
 
-please see the [Documentation](https://jlubbersgeo.github.io/lasertram/) for more!
+please see the [Documentation](https://code.usgs.gov/jlubbers/lasertram/-/wikis/Home) for more!
 
 ## Installation
 [![PyPI](https://img.shields.io/pypi/v/lasertram.svg?style=flat)](https://pypi.python.org/pypi/lasertram)
 [![Compatible Python Versions](https://img.shields.io/pypi/pyversions/lasertram.svg?style=flat)](https://pypi.org/project/lasertram/)
 ```
 pip install lasertram
 ```
 
 ## Contributing
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Code Quality](https://api.codacy.com/project/badge/Grade/fd9912a3faae43bf84a47e3da685d84c)](https://app.codacy.com/gh/jlubbersgeo/lasertram/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=jlubbersgeo/lasertram&amp;utm_campaign=Badge_Grade)
 
 If you have features you'd like to see please open an issue or consider contributing yourself! I'm always happy to have help.
 
 **Maintainer** Jordan Lubbers (jlubbers _at_ usgs.gov)
```

### Comparing `lasertram-0.1.2/lasertram/calc/calc.py` & `lasertram-0.1.3/lasertram/calc/calc.py`

 * *Files identical despite different names*

### Comparing `lasertram-0.1.2/lasertram/helpers/batch.py` & `lasertram-0.1.3/lasertram/helpers/batch.py`

 * *Files identical despite different names*

### Comparing `lasertram-0.1.2/lasertram/helpers/conversions.py` & `lasertram-0.1.3/lasertram/helpers/conversions.py`

 * *Files identical despite different names*

### Comparing `lasertram-0.1.2/lasertram/tram/tram.py` & `lasertram-0.1.3/lasertram/tram/tram.py`

 * *Files identical despite different names*

### Comparing `lasertram-0.1.2/lasertram.egg-info/PKG-INFO` & `lasertram-0.1.3/lasertram.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasertram
-Version: 0.1.2
+Version: 0.1.3
 Summary: For processing LA-ICP-MS data
 Home-page: https://github.com/jlubbersgeo/lasertram
 Author: Jordan Lubbers
 Author-email: jelubber@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,30 +19,27 @@
 Requires-Dist: mendeleev>=0.14.0
 Requires-Dist: numpy>=1.25.2
 Requires-Dist: pandas>=2.0.3
 Requires-Dist: scipy>=1.11.1
 Requires-Dist: statsmodels>=0.14.0
 Requires-Dist: openpyxl>=3.0.0
 
-# lasertram
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) !['coverage'](/images/COVERAGE.svg)
-
+# ```lasertram```
 
 Welcome to the repository for `lasertram`, a package for the time resolved analysis for processing laser ablation inductively coupled plasma mass spectrometry (LA-ICP-MS) data. It is utilized heavily in the dashboard [LaserTRAM-DB](https://github.com/jlubbersgeo/laserTRAM-DB).
 
 ## Documentation
 
-please see the [Documentation](https://jlubbersgeo.github.io/lasertram/) for more!
+please see the [Documentation](https://code.usgs.gov/jlubbers/lasertram/-/wikis/Home) for more!
 
 ## Installation
 [![PyPI](https://img.shields.io/pypi/v/lasertram.svg?style=flat)](https://pypi.python.org/pypi/lasertram)
 [![Compatible Python Versions](https://img.shields.io/pypi/pyversions/lasertram.svg?style=flat)](https://pypi.org/project/lasertram/)
 ```
 pip install lasertram
 ```
 
 ## Contributing
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Code Quality](https://api.codacy.com/project/badge/Grade/fd9912a3faae43bf84a47e3da685d84c)](https://app.codacy.com/gh/jlubbersgeo/lasertram/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=jlubbersgeo/lasertram&amp;utm_campaign=Badge_Grade)
 
 If you have features you'd like to see please open an issue or consider contributing yourself! I'm always happy to have help.
 
 **Maintainer** Jordan Lubbers (jlubbers _at_ usgs.gov)
```

### Comparing `lasertram-0.1.2/setup.cfg` & `lasertram-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `lasertram-0.1.2/tests/test_lasertram.py` & `lasertram-0.1.3/tests/test_lasertram.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from lasertram import LaserCalc, LaserTRAM, batch, conversions
 
+
 ###########LASERTRAM UNIT TESTS##############
-spreadsheet_path = r"tests\spot_test_timestamp_raw_data.xlsx"
+spreadsheet_path = r"./tests/spot_test_timestamp_raw_data.xlsx"
 
 
 @pytest.fixture
 def load_data():
     data = pd.read_excel(spreadsheet_path).set_index("SampleLabel")
     return data
 
@@ -435,24 +436,24 @@
 
     assert (
         result == expected
     ), "concentrations from oxides not being calculated properly"
 
 
 ###############LASERCALC UNIT TESTS#########################
-SRM_path = r"tests\laicpms_stds_tidy.xlsx"
+SRM_path = r"./tests/laicpms_stds_tidy.xlsx"
 
 
 @pytest.fixture
 def load_SRM_data():
     data = pd.read_excel(SRM_path)
     return data
 
 
-LT_complete_path = r"tests\spot_test_timestamp_lasertram_complete.xlsx"
+LT_complete_path = r"./tests/spot_test_timestamp_lasertram_complete.xlsx"
 
 
 @pytest.fixture
 def load_LTcomplete_data():
     data = pd.read_excel(LT_complete_path)
     return data
```

