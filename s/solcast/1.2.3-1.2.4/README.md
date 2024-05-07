# Comparing `tmp/solcast-1.2.3.tar.gz` & `tmp/solcast-1.2.4.tar.gz`

## Comparing `solcast-1.2.3.tar` & `solcast-1.2.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 solcast-1.2.3/.gitattributes
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 solcast-1.2.3/CHANGELOG.md
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 solcast-1.2.3/mkdocs.yml
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 solcast-1.2.3/.github/workflows/black.yml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 solcast-1.2.3/.github/workflows/docs.yml
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 solcast-1.2.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 solcast-1.2.3/.github/workflows/test.yml
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/forecast.md
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/historic.md
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/index.md
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/live.md
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/pv_power_sites.md
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/tmy.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/api/client.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/api/response.md
--rw-r--r--   0        0        0   699355 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/img/logo.png
--rw-r--r--   0        0        0    64800 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/notebooks/1.1 Getting Data - Historic Solar Radiation.ipynb
--rw-r--r--   0        0        0    86081 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/notebooks/1.2 Getting Data - TMY in your local timezone.ipynb
--rw-r--r--   0        0        0   113441 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/notebooks/1.3 Getting Data - Make Concurrent Requests.ipynb
--rw-r--r--   0        0        0    56985 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/notebooks/2.1 PVLib - ModelChain with Solcast weather data.ipynb
--rw-r--r--   0        0        0   204573 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/notebooks/3.1 Comparing to Measurements - Timezone and Time Period alignment.ipynb
--rw-r--r--   0        0        0   278553 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/notebooks/3.2 Comparing to Measurements [GHI] - Quality Controlling and Gap Filling Measurements with Solcast Actuals.ipynb
--rw-r--r--   0        0        0   341076 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/notebooks/3.2b Comparing to Measurements [GTI] - Quality Controlling and Gap Filling Measurements with Solcast Actuals.ipynb
--rw-r--r--   0        0        0   186799 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/notebooks/3.3 Comparing to Measurements - Accuracy Metrics.ipynb
--rw-r--r--   0        0        0   339569 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/notebooks/4.1 Setting up and Using PV Sites.ipynb
--rw-r--r--   0        0        0    15596 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/notebooks/data/3.1_sample_measurements.csv
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/notebooks/data/3.2_sample_measurements.csv
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/notebooks/data/3.2b_sample_measurements.csv
--rw-r--r--   0        0        0    16751 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/notebooks/data/3.3_sample_forecasts.csv
--rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 solcast-1.2.3/docs/notebooks/data/3.3_sample_measurements.csv
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 solcast-1.2.3/solcast/__init__.py
--rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 solcast-1.2.3/solcast/api.py
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 solcast-1.2.3/solcast/forecast.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 solcast-1.2.3/solcast/historic.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 solcast-1.2.3/solcast/live.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 solcast-1.2.3/solcast/pv_power_sites.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 solcast-1.2.3/solcast/tmy.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 solcast-1.2.3/solcast/unmetered_locations.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 solcast-1.2.3/solcast/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solcast-1.2.3/tests/__init__.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 solcast-1.2.3/tests/test_client.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 solcast-1.2.3/tests/test_forecast.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 solcast-1.2.3/tests/test_historic.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 solcast-1.2.3/tests/test_live.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 solcast-1.2.3/tests/test_pv_power_sites.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 solcast-1.2.3/tests/test_tmy.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 solcast-1.2.3/.gitignore
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 solcast-1.2.3/LICENSE
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 solcast-1.2.3/README.md
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 solcast-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 solcast-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 solcast-1.2.4/.gitattributes
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 solcast-1.2.4/CHANGELOG.md
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 solcast-1.2.4/mkdocs.yml
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 solcast-1.2.4/.github/workflows/black.yml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 solcast-1.2.4/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 solcast-1.2.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 solcast-1.2.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/forecast.md
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/historic.md
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/index.md
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/live.md
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/pv_power_sites.md
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/tmy.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/api/client.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/api/response.md
+-rw-r--r--   0        0        0   699355 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/img/logo.png
+-rw-r--r--   0        0        0    64800 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/notebooks/1.1 Getting Data - Historic Solar Radiation.ipynb
+-rw-r--r--   0        0        0    86081 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/notebooks/1.2 Getting Data - TMY in your local timezone.ipynb
+-rw-r--r--   0        0        0   113441 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/notebooks/1.3 Getting Data - Make Concurrent Requests.ipynb
+-rw-r--r--   0        0        0    56985 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/notebooks/2.1 PVLib - ModelChain with Solcast weather data.ipynb
+-rw-r--r--   0        0        0   204573 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/notebooks/3.1 Comparing to Measurements - Timezone and Time Period alignment.ipynb
+-rw-r--r--   0        0        0   278553 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/notebooks/3.2 Comparing to Measurements [GHI] - Quality Controlling and Gap Filling Measurements with Solcast Actuals.ipynb
+-rw-r--r--   0        0        0   341076 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/notebooks/3.2b Comparing to Measurements [GTI] - Quality Controlling and Gap Filling Measurements with Solcast Actuals.ipynb
+-rw-r--r--   0        0        0   186799 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/notebooks/3.3 Comparing to Measurements - Accuracy Metrics.ipynb
+-rw-r--r--   0        0        0   339569 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/notebooks/4.1 Setting up and Using PV Sites.ipynb
+-rw-r--r--   0        0        0    15596 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/notebooks/data/3.1_sample_measurements.csv
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/notebooks/data/3.2_sample_measurements.csv
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/notebooks/data/3.2b_sample_measurements.csv
+-rw-r--r--   0        0        0    16751 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/notebooks/data/3.3_sample_forecasts.csv
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 solcast-1.2.4/docs/notebooks/data/3.3_sample_measurements.csv
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 solcast-1.2.4/solcast/__init__.py
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 solcast-1.2.4/solcast/api.py
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 solcast-1.2.4/solcast/forecast.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 solcast-1.2.4/solcast/historic.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 solcast-1.2.4/solcast/live.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 solcast-1.2.4/solcast/pv_power_sites.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 solcast-1.2.4/solcast/tmy.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 solcast-1.2.4/solcast/unmetered_locations.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 solcast-1.2.4/solcast/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solcast-1.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 solcast-1.2.4/tests/test_client.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 solcast-1.2.4/tests/test_forecast.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 solcast-1.2.4/tests/test_historic.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 solcast-1.2.4/tests/test_live.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 solcast-1.2.4/tests/test_pv_power_sites.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 solcast-1.2.4/tests/test_tmy.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 solcast-1.2.4/.gitignore
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 solcast-1.2.4/LICENSE
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 solcast-1.2.4/README.md
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 solcast-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 solcast-1.2.4/PKG-INFO
```

### Comparing `solcast-1.2.3/mkdocs.yml` & `solcast-1.2.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/.github/workflows/docs.yml` & `solcast-1.2.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/.github/workflows/publish-to-pypi.yml` & `solcast-1.2.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/.github/workflows/test.yml` & `solcast-1.2.4/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 on: [push]
 
 jobs:
   build:
     strategy:
       matrix:
-        os: ['ubuntu-latest', 'macos-latest', 'windows-latest']
+        os: ['ubuntu-latest', 'macos-13', 'windows-latest']
         python-version: ["3.7", "3.11"]
     runs-on: ${{ matrix.os }}
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
```

### Comparing `solcast-1.2.3/docs/forecast.md` & `solcast-1.2.4/docs/forecast.md`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/historic.md` & `solcast-1.2.4/docs/historic.md`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/index.md` & `solcast-1.2.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/live.md` & `solcast-1.2.4/docs/live.md`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/pv_power_sites.md` & `solcast-1.2.4/docs/pv_power_sites.md`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/tmy.md` & `solcast-1.2.4/docs/tmy.md`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/img/logo.png` & `solcast-1.2.4/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/notebooks/1.1 Getting Data - Historic Solar Radiation.ipynb` & `solcast-1.2.4/docs/notebooks/1.1 Getting Data - Historic Solar Radiation.ipynb`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/notebooks/1.2 Getting Data - TMY in your local timezone.ipynb` & `solcast-1.2.4/docs/notebooks/1.2 Getting Data - TMY in your local timezone.ipynb`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/notebooks/1.3 Getting Data - Make Concurrent Requests.ipynb` & `solcast-1.2.4/docs/notebooks/1.3 Getting Data - Make Concurrent Requests.ipynb`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/notebooks/2.1 PVLib - ModelChain with Solcast weather data.ipynb` & `solcast-1.2.4/docs/notebooks/2.1 PVLib - ModelChain with Solcast weather data.ipynb`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/notebooks/3.1 Comparing to Measurements - Timezone and Time Period alignment.ipynb` & `solcast-1.2.4/docs/notebooks/3.1 Comparing to Measurements - Timezone and Time Period alignment.ipynb`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/notebooks/3.2 Comparing to Measurements [GHI] - Quality Controlling and Gap Filling Measurements with Solcast Actuals.ipynb` & `solcast-1.2.4/docs/notebooks/3.2 Comparing to Measurements [GHI] - Quality Controlling and Gap Filling Measurements with Solcast Actuals.ipynb`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/notebooks/3.2b Comparing to Measurements [GTI] - Quality Controlling and Gap Filling Measurements with Solcast Actuals.ipynb` & `solcast-1.2.4/docs/notebooks/3.2b Comparing to Measurements [GTI] - Quality Controlling and Gap Filling Measurements with Solcast Actuals.ipynb`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/notebooks/3.3 Comparing to Measurements - Accuracy Metrics.ipynb` & `solcast-1.2.4/docs/notebooks/3.3 Comparing to Measurements - Accuracy Metrics.ipynb`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/notebooks/4.1 Setting up and Using PV Sites.ipynb` & `solcast-1.2.4/docs/notebooks/4.1 Setting up and Using PV Sites.ipynb`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/notebooks/data/3.1_sample_measurements.csv` & `solcast-1.2.4/docs/notebooks/data/3.1_sample_measurements.csv`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/notebooks/data/3.2_sample_measurements.csv` & `solcast-1.2.4/docs/notebooks/data/3.2_sample_measurements.csv`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/notebooks/data/3.2b_sample_measurements.csv` & `solcast-1.2.4/docs/notebooks/data/3.2b_sample_measurements.csv`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/notebooks/data/3.3_sample_forecasts.csv` & `solcast-1.2.4/docs/notebooks/data/3.3_sample_forecasts.csv`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/docs/notebooks/data/3.3_sample_measurements.csv` & `solcast-1.2.4/docs/notebooks/data/3.3_sample_measurements.csv`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/solcast/api.py` & `solcast-1.2.4/solcast/api.py`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/solcast/forecast.py` & `solcast-1.2.4/solcast/forecast.py`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/solcast/historic.py` & `solcast-1.2.4/solcast/historic.py`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/solcast/live.py` & `solcast-1.2.4/solcast/live.py`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/solcast/pv_power_sites.py` & `solcast-1.2.4/solcast/pv_power_sites.py`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/solcast/tmy.py` & `solcast-1.2.4/solcast/tmy.py`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/solcast/unmetered_locations.py` & `solcast-1.2.4/solcast/unmetered_locations.py`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/solcast/urls.py` & `solcast-1.2.4/solcast/urls.py`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/tests/test_client.py` & `solcast-1.2.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/tests/test_forecast.py` & `solcast-1.2.4/tests/test_forecast.py`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/tests/test_historic.py` & `solcast-1.2.4/tests/test_historic.py`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/tests/test_live.py` & `solcast-1.2.4/tests/test_live.py`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/tests/test_pv_power_sites.py` & `solcast-1.2.4/tests/test_pv_power_sites.py`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/tests/test_tmy.py` & `solcast-1.2.4/tests/test_tmy.py`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/LICENSE` & `solcast-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/README.md` & `solcast-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/pyproject.toml` & `solcast-1.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `solcast-1.2.3/PKG-INFO` & `solcast-1.2.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: solcast
-Version: 1.2.3
+Version: 1.2.4
 Summary: a simple Python SDK for the Solcast API
 Project-URL: Homepage, https://pypi.org/project/solcast/
 Project-URL: Documentation, https://solcast.github.io/solcast-api-python-sdk
 Project-URL: Repository, https://github.com/Solcast/solcast-api-python-sdk
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -25,18 +25,23 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Provides-Extra: all
 Requires-Dist: black; extra == 'all'
+Requires-Dist: kaleido; extra == 'all'
 Requires-Dist: matplotlib; extra == 'all'
+Requires-Dist: mkdocs; extra == 'all'
+Requires-Dist: mkdocs-jupyter; extra == 'all'
+Requires-Dist: mkdocs-material; extra == 'all'
+Requires-Dist: mkdocstrings[python]==0.22; extra == 'all'
 Requires-Dist: notebook; extra == 'all'
 Requires-Dist: pandas; extra == 'all'
-Requires-Dist: solcast[docs]; extra == 'all'
+Requires-Dist: pytest; extra == 'all'
 Provides-Extra: docs
 Requires-Dist: kaleido; extra == 'docs'
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-jupyter; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocstrings[python]==0.22; extra == 'docs'
 Requires-Dist: pytest; extra == 'docs'
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: solcast Version: 1.2.3 Summary: a simple Python SDK
+Metadata-Version: 2.3 Name: solcast Version: 1.2.4 Summary: a simple Python SDK
 for the Solcast API Project-URL: Homepage, https://pypi.org/project/solcast/
 Project-URL: Documentation, https://solcast.github.io/solcast-api-python-sdk
 Project-URL: Repository, https://github.com/Solcast/solcast-api-python-sdk
 License-Expression: Apache-2.0 License-File: LICENSE Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
@@ -12,16 +12,19 @@
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Internet Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Software Development Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Typing :: Typed Requires-Python: >=3.7
 Provides-Extra: all Requires-Dist: black; extra == 'all' Requires-Dist:
-matplotlib; extra == 'all' Requires-Dist: notebook; extra == 'all' Requires-
-Dist: pandas; extra == 'all' Requires-Dist: solcast[docs]; extra == 'all'
+kaleido; extra == 'all' Requires-Dist: matplotlib; extra == 'all' Requires-
+Dist: mkdocs; extra == 'all' Requires-Dist: mkdocs-jupyter; extra == 'all'
+Requires-Dist: mkdocs-material; extra == 'all' Requires-Dist: mkdocstrings
+[python]==0.22; extra == 'all' Requires-Dist: notebook; extra == 'all'
+Requires-Dist: pandas; extra == 'all' Requires-Dist: pytest; extra == 'all'
 Provides-Extra: docs Requires-Dist: kaleido; extra == 'docs' Requires-Dist:
 mkdocs; extra == 'docs' Requires-Dist: mkdocs-jupyter; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs' Requires-Dist: mkdocstrings
 [python]==0.22; extra == 'docs' Requires-Dist: pytest; extra == 'docs'
 Description-Content-Type: text/markdown [https://github.com/Solcast/solcast-
 api-python-sdk/blob/main/docs/img/logo.png?raw=true]# Solcast API Python SDK
 PPyytthhoonn SSDDKK ttoo aacccceessss tthhee SSoollccaasstt AAPPII [![Docs](https://github.com/Solcast/
```

