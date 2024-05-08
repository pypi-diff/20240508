# Comparing `tmp/eq3btsmart-1.1.6.tar.gz` & `tmp/eq3btsmart-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eq3btsmart-1.1.6.tar", max compression
+gzip compressed data, was "eq3btsmart-1.1.7.tar", max compression
```

## Comparing `eq3btsmart-1.1.6.tar` & `eq3btsmart-1.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1061 2024-02-06 17:49:16.747365 eq3btsmart-1.1.6/LICENSE.md
--rw-r--r--   0        0        0     1923 2024-02-06 17:49:16.747365 eq3btsmart-1.1.6/README.md
--rw-r--r--   0        0        0       59 2024-02-06 17:49:16.747365 eq3btsmart-1.1.6/eq3btsmart/__init__.py
--rw-r--r--   0        0        0        0 2024-02-06 17:49:16.747365 eq3btsmart-1.1.6/eq3btsmart/adapter/__init__.py
--rw-r--r--   0        0        0     1806 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/adapter/base_adapter.py
--rw-r--r--   0        0        0     1102 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/adapter/eq3_away_time.py
--rw-r--r--   0        0        0      632 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/adapter/eq3_duration.py
--rw-r--r--   0        0        0      461 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/adapter/eq3_schedule_time.py
--rw-r--r--   0        0        0      394 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/adapter/eq3_serial.py
--rw-r--r--   0        0        0      611 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/adapter/eq3_temperature.py
--rw-r--r--   0        0        0      644 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/adapter/eq3_temperature_offset.py
--rw-r--r--   0        0        0      753 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/adapter/eq3_time.py
--rw-r--r--   0        0        0     1814 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/const.py
--rw-r--r--   0        0        0      130 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/exceptions.py
--rw-r--r--   0        0        0      445 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/models/__init__.py
--rw-r--r--   0        0        0      718 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/models/base_model.py
--rw-r--r--   0        0        0      624 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/models/device_data.py
--rw-r--r--   0        0        0     1064 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/models/presets.py
--rw-r--r--   0        0        0     2783 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/models/schedule.py
--rw-r--r--   0        0        0     1343 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/models/schedule_day.py
--rw-r--r--   0        0        0      270 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/models/schedule_hour.py
--rw-r--r--   0        0        0     2028 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/models/status.py
--rw-r--r--   0        0        0     6349 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/structures.py
--rw-r--r--   0        0        0    13651 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/thermostat.py
--rw-r--r--   0        0        0       92 2024-02-06 17:49:16.751365 eq3btsmart-1.1.6/eq3btsmart/thermostat_config.py
--rw-r--r--   0        0        0      980 2024-02-06 17:49:22.727338 eq3btsmart-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     2535 1970-01-01 00:00:00.000000 eq3btsmart-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/LICENSE.md
+-rw-r--r--   0        0        0     1800 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/README.md
+-rw-r--r--   0        0        0       59 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/adapter/__init__.py
+-rw-r--r--   0        0        0     1806 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/adapter/base_adapter.py
+-rw-r--r--   0        0        0     1102 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/adapter/eq3_away_time.py
+-rw-r--r--   0        0        0      632 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/adapter/eq3_duration.py
+-rw-r--r--   0        0        0      461 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/adapter/eq3_schedule_time.py
+-rw-r--r--   0        0        0      394 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/adapter/eq3_serial.py
+-rw-r--r--   0        0        0      611 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/adapter/eq3_temperature.py
+-rw-r--r--   0        0        0      644 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/adapter/eq3_temperature_offset.py
+-rw-r--r--   0        0        0      753 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/adapter/eq3_time.py
+-rw-r--r--   0        0        0     1814 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/const.py
+-rw-r--r--   0        0        0      130 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/exceptions.py
+-rw-r--r--   0        0        0      445 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/models/__init__.py
+-rw-r--r--   0        0        0      718 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/models/base_model.py
+-rw-r--r--   0        0        0      624 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/models/device_data.py
+-rw-r--r--   0        0        0     1064 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/models/presets.py
+-rw-r--r--   0        0        0     2783 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/models/schedule.py
+-rw-r--r--   0        0        0     1343 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/models/schedule_day.py
+-rw-r--r--   0        0        0      270 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/models/schedule_hour.py
+-rw-r--r--   0        0        0     2028 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/models/status.py
+-rw-r--r--   0        0        0     6349 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/structures.py
+-rw-r--r--   0        0        0    13651 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/thermostat.py
+-rw-r--r--   0        0        0       92 2024-05-08 00:01:21.670802 eq3btsmart-1.1.7/eq3btsmart/thermostat_config.py
+-rw-r--r--   0        0        0      981 2024-05-08 00:01:30.530726 eq3btsmart-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 eq3btsmart-1.1.7/PKG-INFO
```

### Comparing `eq3btsmart-1.1.6/LICENSE.md` & `eq3btsmart-1.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/README.md` & `eq3btsmart-1.1.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-![My Home Assistant](https://img.shields.io/badge/Home%20Assistant-%2341BDF5.svg?style=flat&logo=home-assistant&label=My)
-
 ![PyPI - Version](https://img.shields.io/pypi/v/eq3btsmart?logo=python&logoColor=green&color=blue)
 ![GitHub License](https://img.shields.io/github/license/eulemitkeule/eq3btsmart)
 ![GitHub Sponsors](https://img.shields.io/github/sponsors/eulemitkeule?logo=GitHub-Sponsors)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=EuleMitKeule_eq3btsmart&metric=coverage)](https://sonarcloud.io/summary/new_code?id=EuleMitKeule_eq3btsmart)
 
 [![Code Quality](https://github.com/EuleMitKeule/eq3btsmart/actions/workflows/quality.yml/badge.svg)](https://github.com/EuleMitKeule/eq3btsmart/actions/workflows/quality.yml)
 [![Publish](https://github.com/EuleMitKeule/eq3btsmart/actions/workflows/publish.yml/badge.svg)](https://github.com/EuleMitKeule/eq3btsmart/actions/workflows/publish.yml)
```

### Comparing `eq3btsmart-1.1.6/eq3btsmart/adapter/base_adapter.py` & `eq3btsmart-1.1.7/eq3btsmart/adapter/base_adapter.py`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/eq3btsmart/adapter/eq3_away_time.py` & `eq3btsmart-1.1.7/eq3btsmart/adapter/eq3_away_time.py`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/eq3btsmart/adapter/eq3_duration.py` & `eq3btsmart-1.1.7/eq3btsmart/adapter/eq3_duration.py`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/eq3btsmart/adapter/eq3_temperature.py` & `eq3btsmart-1.1.7/eq3btsmart/adapter/eq3_temperature.py`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/eq3btsmart/adapter/eq3_temperature_offset.py` & `eq3btsmart-1.1.7/eq3btsmart/adapter/eq3_temperature_offset.py`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/eq3btsmart/adapter/eq3_time.py` & `eq3btsmart-1.1.7/eq3btsmart/adapter/eq3_time.py`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/eq3btsmart/const.py` & `eq3btsmart-1.1.7/eq3btsmart/const.py`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/eq3btsmart/models/base_model.py` & `eq3btsmart-1.1.7/eq3btsmart/models/base_model.py`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/eq3btsmart/models/device_data.py` & `eq3btsmart-1.1.7/eq3btsmart/models/device_data.py`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/eq3btsmart/models/presets.py` & `eq3btsmart-1.1.7/eq3btsmart/models/presets.py`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/eq3btsmart/models/schedule.py` & `eq3btsmart-1.1.7/eq3btsmart/models/schedule.py`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/eq3btsmart/models/schedule_day.py` & `eq3btsmart-1.1.7/eq3btsmart/models/schedule_day.py`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/eq3btsmart/models/status.py` & `eq3btsmart-1.1.7/eq3btsmart/models/status.py`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/eq3btsmart/structures.py` & `eq3btsmart-1.1.7/eq3btsmart/structures.py`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/eq3btsmart/thermostat.py` & `eq3btsmart-1.1.7/eq3btsmart/thermostat.py`

 * *Files identical despite different names*

### Comparing `eq3btsmart-1.1.6/pyproject.toml` & `eq3btsmart-1.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "eq3btsmart"
-version = "1.1.6"
+version = "1.1.7"
 description = ""
 authors = ["Lennard Beers"]
 readme = "README.md"
 repository = "https://github.com/eulemitkeule/eq3btsmart"
 packages = [
     { include = "eq3btsmart" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
-bleak = "^0.21.1"
+bleak = ">=0.21.0"
 construct = "^2.10.68"
 construct-typing = "^0.6.2"
 pytest-asyncio = "^0.23.3"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.13"
 mypy = "^1.8.0"
```

### Comparing `eq3btsmart-1.1.6/PKG-INFO` & `eq3btsmart-1.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: eq3btsmart
-Version: 1.1.6
+Version: 1.1.7
 Summary: 
 Home-page: https://github.com/eulemitkeule/eq3btsmart
 Author: Lennard Beers
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: bleak (>=0.21.1,<0.22.0)
+Requires-Dist: bleak (>=0.21.0)
 Requires-Dist: construct (>=2.10.68,<3.0.0)
 Requires-Dist: construct-typing (>=0.6.2,<0.7.0)
 Requires-Dist: pytest-asyncio (>=0.23.3,<0.24.0)
 Project-URL: Repository, https://github.com/eulemitkeule/eq3btsmart
 Description-Content-Type: text/markdown
 
-![My Home Assistant](https://img.shields.io/badge/Home%20Assistant-%2341BDF5.svg?style=flat&logo=home-assistant&label=My)
-
 ![PyPI - Version](https://img.shields.io/pypi/v/eq3btsmart?logo=python&logoColor=green&color=blue)
 ![GitHub License](https://img.shields.io/github/license/eulemitkeule/eq3btsmart)
 ![GitHub Sponsors](https://img.shields.io/github/sponsors/eulemitkeule?logo=GitHub-Sponsors)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=EuleMitKeule_eq3btsmart&metric=coverage)](https://sonarcloud.io/summary/new_code?id=EuleMitKeule_eq3btsmart)
 
 [![Code Quality](https://github.com/EuleMitKeule/eq3btsmart/actions/workflows/quality.yml/badge.svg)](https://github.com/EuleMitKeule/eq3btsmart/actions/workflows/quality.yml)
 [![Publish](https://github.com/EuleMitKeule/eq3btsmart/actions/workflows/publish.yml/badge.svg)](https://github.com/EuleMitKeule/eq3btsmart/actions/workflows/publish.yml)
```

