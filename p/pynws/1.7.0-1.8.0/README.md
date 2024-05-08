# Comparing `tmp/pynws-1.7.0.tar.gz` & `tmp/pynws-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynws-1.7.0.tar", last modified: Mon Apr 29 23:20:33 2024, max compression
+gzip compressed data, was "pynws-1.8.0.tar", last modified: Wed May  8 10:03:20 2024, max compression
```

## Comparing `pynws-1.7.0.tar` & `pynws-1.8.0.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.446124 pynws-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 23:20:28.000000 pynws-1.7.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.438125 pynws-1.7.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-29 23:20:28.000000 pynws-1.7.0/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      163 2024-04-29 23:20:28.000000 pynws-1.7.0/.devcontainer/postcreatecommand.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.438125 pynws-1.7.0/.devcontainer/python3.9/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-29 23:20:28.000000 pynws-1.7.0/.devcontainer/python3.9/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 23:20:28.000000 pynws-1.7.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.438125 pynws-1.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-29 23:20:28.000000 pynws-1.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.438125 pynws-1.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-29 23:20:28.000000 pynws-1.7.0/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-29 23:20:28.000000 pynws-1.7.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 23:20:28.000000 pynws-1.7.0/.github/workflows/typing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-29 23:20:28.000000 pynws-1.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-29 23:20:28.000000 pynws-1.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-29 23:20:28.000000 pynws-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-29 23:20:28.000000 pynws-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-29 23:20:33.446124 pynws-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-29 23:20:28.000000 pynws-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-29 23:20:28.000000 pynws-1.7.0/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-04-29 23:20:28.000000 pynws-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-29 23:20:28.000000 pynws-1.7.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 23:20:33.446124 pynws-1.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.434125 pynws-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.442124 pynws-1.7.0/src/pynws/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 23:20:33.000000 pynws-1.7.0/src/pynws/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.442124 pynws-1.7.0/src/pynws/backports/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/backports/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/nws.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/raw_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15711 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/simple_nws.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-29 23:20:28.000000 pynws-1.7.0/src/pynws/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.446124 pynws-1.7.0/src/pynws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-29 23:20:33.000000 pynws-1.7.0/src/pynws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-29 23:20:33.000000 pynws-1.7.0/src/pynws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 23:20:33.000000 pynws-1.7.0/src/pynws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-29 23:20:33.000000 pynws-1.7.0/src/pynws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 23:20:33.000000 pynws-1.7.0/src/pynws.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.442124 pynws-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:20:33.446124 pynws-1.7.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/alerts_active_zone.json
--rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/alerts_active_zone_second.json
--rw-r--r--   0 runner    (1001) docker     (127)   132083 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/detailed_forecast.json
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/gridpoints_forecast.json
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/gridpoints_forecast_empty.json
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/gridpoints_forecast_hourly.json
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/gridpoints_forecast_strings.json
--rw-r--r--   0 runner    (1001) docker     (127)    45128 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/gridpoints_stations.json
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/points.json
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations.json
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_alternate_units.json
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_empty.json
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_latest.json
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_metar.json
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_metar_noparse.json
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_missing_value.json
--rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_multiple.json
--rw-r--r--   0 runner    (1001) docker     (127)    10282 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_multiple_unsorted.json
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_noprop.json
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_other_unitcode.json
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/fixtures/stations_observations_strings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/test_nws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    13726 2024-04-29 23:20:28.000000 pynws-1.7.0/tests/test_simple_nws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.705052 pynws-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 10:03:13.000000 pynws-1.8.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.697053 pynws-1.8.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-08 10:03:13.000000 pynws-1.8.0/.devcontainer/devcontainer.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      212 2024-05-08 10:03:13.000000 pynws-1.8.0/.devcontainer/postcreatecommand.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.697053 pynws-1.8.0/.devcontainer/python3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 10:03:13.000000 pynws-1.8.0/.devcontainer/python3.9/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 10:03:13.000000 pynws-1.8.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.697053 pynws-1.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-08 10:03:13.000000 pynws-1.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.697053 pynws-1.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-08 10:03:13.000000 pynws-1.8.0/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-08 10:03:13.000000 pynws-1.8.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-08 10:03:13.000000 pynws-1.8.0/.github/workflows/typing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 10:03:13.000000 pynws-1.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-08 10:03:13.000000 pynws-1.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-08 10:03:13.000000 pynws-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-08 10:03:13.000000 pynws-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-08 10:03:20.705052 pynws-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-08 10:03:13.000000 pynws-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-08 10:03:13.000000 pynws-1.8.0/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-08 10:03:13.000000 pynws-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-08 10:03:13.000000 pynws-1.8.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 10:03:20.705052 pynws-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.693053 pynws-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.697053 pynws-1.8.0/src/pynws/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 10:03:20.000000 pynws-1.8.0/src/pynws/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.697053 pynws-1.8.0/src/pynws/backports/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/backports/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/nws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/raw_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/simple_nws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.705052 pynws-1.8.0/src/pynws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-08 10:03:20.000000 pynws-1.8.0/src/pynws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-08 10:03:20.000000 pynws-1.8.0/src/pynws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:03:20.000000 pynws-1.8.0/src/pynws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 10:03:20.000000 pynws-1.8.0/src/pynws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 10:03:20.000000 pynws-1.8.0/src/pynws.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.701053 pynws-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.705052 pynws-1.8.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/alerts_active_zone.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/alerts_active_zone_second.json
+-rw-r--r--   0 runner    (1001) docker     (127)   132083 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/detailed_forecast.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/gridpoints_forecast.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/gridpoints_forecast_empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/gridpoints_forecast_hourly.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/gridpoints_forecast_hourly_empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/gridpoints_forecast_strings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    45128 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/gridpoints_stations.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/points.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_alternate_units.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_latest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_metar.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_metar_noparse.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_missing_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_multiple.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10282 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_multiple_unsorted.json
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_noprop.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_other_unitcode.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_strings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/test_nws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18416 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/test_simple_nws.py
```

### Comparing `pynws-1.7.0/.github/dependabot.yml` & `pynws-1.8.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/.github/workflows/pythonpublish.yml` & `pynws-1.8.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/.github/workflows/typing.yml` & `pynws-1.8.0/.github/workflows/typing.yml`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/LICENSE` & `pynws-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/PKG-INFO` & `pynws-1.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynws
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python library to retrieve observations and forecasts from NWS/NOAA
 Author-email: Matthew Flamm <matthewhflamm0@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/MatthewFlamm/pynws
 Project-URL: Bug Tracker, https://github.com/MatthewFlamm/pynws/issues
 Keywords: nws,weather
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pynws-1.7.0/README.md` & `pynws-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/example.py` & `pynws-1.8.0/example.py`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/pyproject.toml` & `pynws-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/src/pynws/backports/enum.py` & `pynws-1.8.0/src/pynws/backports/enum.py`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/src/pynws/const.py` & `pynws-1.8.0/src/pynws/const.py`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/src/pynws/forecast.py` & `pynws-1.8.0/src/pynws/forecast.py`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/src/pynws/nws.py` & `pynws-1.8.0/src/pynws/nws.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     """Error in Nws Class"""
 
     def __init__(self: NwsError, message: str):
         super().__init__(message)
         self.message = message
 
 
+class NwsNoDataError(NwsError):
+    """No data was returned."""
+
+
 class Nws:
     """Class to more easily get data for one location."""
 
     def __init__(
         self: Nws,
         session: ClientSession,
         userid: str,
```

### Comparing `pynws-1.7.0/src/pynws/raw_data.py` & `pynws-1.8.0/src/pynws/raw_data.py`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/src/pynws/simple_nws.py` & `pynws-1.8.0/src/pynws/simple_nws.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     from datetime import timedelta
 
 from aiohttp import ClientResponseError, ClientSession
 from metar import Metar
 
 from .const import ALERT_ID, API_WEATHER_CODE, Final
 from .forecast import DetailedForecast
-from .nws import Nws, NwsError
+from .nws import Nws, NwsError, NwsNoDataError
 from .units import convert_unit
 
 WIND_DIRECTIONS: Final = [
     "N",
     "NNE",
     "NE",
     "ENE",
@@ -48,59 +48,87 @@
     "NNW",
 ]
 
 
 WIND: Final = {name: idx * 360 / 16 for idx, name in enumerate(WIND_DIRECTIONS)}
 
 
-def _is_500_error(error: BaseException) -> bool:
-    """Return True if error is ClientResponseError and has a 5xx status."""
-    return isinstance(error, ClientResponseError) and error.status >= 500
+def _nws_retry_func(retry_no_data: bool):
+    """
+    Return function used for tenacity.retry.
+
+    Retry if:
+        - if error is ClientResponseError and has a 5xx status.
+        - if error is NwsNoDataError, the behavior is determined by retry_no_data
+
+    Parameters
+    ----------
+    retry_no_data : bool
+        Whether to retry when `NwsNoDataError` is raised.
+
+    """
+
+    def _retry(error: BaseException) -> bool:
+        """Whether to retry based on execptions."""
+        if isinstance(error, ClientResponseError) and error.status >= 500:
+            return True
+        if retry_no_data and isinstance(error, NwsNoDataError):
+            return True
+        return False
+
+    return _retry
 
 
 def _setup_retry_func(
     func: Callable[[Any, Any], Awaitable[Any]],
     interval: Union[float, timedelta],
     stop: Union[float, timedelta],
-) -> Callable[[Any, Any], Awaitable[Any]]:
+    *,
+    retry_no_data=False,
+) -> Callable[..., Awaitable[Any]]:
     from tenacity import retry, retry_if_exception, stop_after_delay, wait_fixed
 
+    retry_func = _nws_retry_func(retry_no_data=retry_no_data)
+
     return retry(
         reraise=True,
         wait=wait_fixed(interval),
         stop=stop_after_delay(stop),
-        retry=retry_if_exception(_is_500_error),
+        retry=retry_if_exception(retry_func),
     )(func)
 
 
 async def call_with_retry(
     func: Callable[[Any, Any], Awaitable[Any]],
     interval: Union[float, timedelta],
     stop: Union[float, timedelta],
     /,
     *args,
+    retry_no_data=False,
     **kwargs,
 ) -> Callable[[Any, Any], Awaitable[Any]]:
     """Call an update function with retries.
 
     Parameters
     ----------
     func : Callable
         An awaitable coroutine to retry.
     interval : float, datetime.datetime.timedelta
         Time interval for retry.
     stop : float, datetime.datetime.timedelta
         Time interval to stop retrying.
+    retry_no_data : bool
+         Whether to retry when no data is returned.
     args : Any
         Positional args to pass to func.
     kwargs : Any
         Keyword args to pass to func.
     """
-    retried_func = _setup_retry_func(func, interval, stop)
-    return await retried_func(*args, **kwargs)
+    retried_func = _setup_retry_func(func, interval, stop, retry_no_data=retry_no_data)
+    return await retried_func(*args, raise_no_data=retry_no_data, **kwargs)
 
 
 class MetarParam(NamedTuple):
     """METAR conversion parameter"""
 
     attr: str
     units: Optional[str] = None
@@ -215,32 +243,55 @@
             except Metar.ParserError:
                 metar_obs = None
         else:
             metar_obs = None
         return metar_obs
 
     async def update_observation(
-        self: SimpleNWS, limit: int = 0, start_time: Optional[datetime] = None
+        self: SimpleNWS,
+        limit: int = 0,
+        start_time: Optional[datetime] = None,
+        *,
+        raise_no_data: bool = False,
     ) -> None:
         """Update observation."""
         obs = await self.get_stations_observations(limit, start_time=start_time)
         if obs:
             self._observation = obs
             self._metar_obs = [self.extract_metar(iobs) for iobs in self._observation]
+        elif raise_no_data:
+            raise NwsNoDataError("Observation received with no data.")
 
-    async def update_forecast(self: SimpleNWS) -> None:
+    async def update_forecast(self: SimpleNWS, *, raise_no_data: bool = False) -> None:
         """Update forecast."""
         self._forecast = await self.get_gridpoints_forecast()
+        if not self.forecast and raise_no_data:
+            raise NwsNoDataError("Forecast received with no data.")
 
-    async def update_forecast_hourly(self: SimpleNWS) -> None:
+    async def update_forecast_hourly(
+        self: SimpleNWS, *, raise_no_data: bool = False
+    ) -> None:
         """Update forecast hourly."""
         self._forecast_hourly = await self.get_gridpoints_forecast_hourly()
+        if not self.forecast_hourly and raise_no_data:
+            raise NwsNoDataError("Forecast hourly received with no data.")
+
+    async def update_detailed_forecast(
+        self: SimpleNWS, *, raise_no_data: bool = False
+    ) -> None:
+        """Update forecast.
+
+        Note:
+        `raise_no_data`currently can only be set to `False`.
+        """
+        if raise_no_data:
+            raise NotImplementedError(
+                "raise_no_data=True not implemented for update_detailed_forecast"
+            )
 
-    async def update_detailed_forecast(self: SimpleNWS) -> None:
-        """Update forecast."""
         self._detailed_forecast = await self.get_detailed_forecast()
 
     @staticmethod
     def _unique_alert_ids(alerts: List[Dict[str, Any]]) -> Set[str]:
         """Return set of unique alert_ids."""
         return {alert[ALERT_ID] for alert in alerts}
 
@@ -249,30 +300,60 @@
         alerts: List[Dict[str, Any]],
         current_alerts: List[Dict[str, Any]],
     ) -> List[Dict[str, Any]]:
         """Return new alerts."""
         current_alert_ids = self._unique_alert_ids(current_alerts)
         return [alert for alert in alerts if alert[ALERT_ID] not in current_alert_ids]
 
-    async def update_alerts_forecast_zone(self: SimpleNWS) -> List[Dict[str, Any]]:
-        """Update alerts zone."""
+    async def update_alerts_forecast_zone(
+        self: SimpleNWS, *, raise_no_data: bool = False
+    ) -> List[Dict[str, Any]]:
+        """Update alerts zone.
+
+        Note:
+        `raise_no_data`currently can only be set to `False`.
+        """
+        if raise_no_data:
+            raise NotImplementedError(
+                "raise_no_data=True not implemented for update_alerts_forecast_zone"
+            )
         alerts = await self.get_alerts_forecast_zone()
         new_alerts = self._new_alerts(alerts, self._alerts_forecast_zone)
         self._alerts_forecast_zone = alerts
         return new_alerts
 
-    async def update_alerts_county_zone(self: SimpleNWS) -> List[Dict[str, Any]]:
-        """Update alerts zone."""
+    async def update_alerts_county_zone(
+        self: SimpleNWS, *, raise_no_data: bool = False
+    ) -> List[Dict[str, Any]]:
+        """Update alerts zone.
+
+        Note:
+        `raise_no_data`currently can only be set to `False`.
+        """
+        if raise_no_data:
+            raise NotImplementedError(
+                "raise_no_data=True not implemented for update_alerts_county_zone"
+            )
         alerts = await self.get_alerts_county_zone()
         new_alerts = self._new_alerts(alerts, self._alerts_county_zone)
         self._alerts_county_zone = alerts
         return new_alerts
 
-    async def update_alerts_fire_weather_zone(self: SimpleNWS) -> List[Dict[str, Any]]:
-        """Update alerts zone."""
+    async def update_alerts_fire_weather_zone(
+        self: SimpleNWS, *, raise_no_data: bool = False
+    ) -> List[Dict[str, Any]]:
+        """Update alerts zone.
+
+        Note:
+        `raise_no_data`currently can only be set to `False`.
+        """
+        if raise_no_data:
+            raise NotImplementedError(
+                "raise_no_data=True not implemented for update_alerts_fire_weather_zone"
+            )
         alerts = await self.get_alerts_fire_weather_zone()
         new_alerts = self._new_alerts(alerts, self._alerts_fire_weather_zone)
         self._alerts_fire_weather_zone = alerts
         return new_alerts
 
     async def update_alerts_all_zones(self: SimpleNWS) -> List[Dict[str, Any]]:
         """Update all alerts zones."""
```

### Comparing `pynws-1.7.0/src/pynws/units.py` & `pynws-1.8.0/src/pynws/units.py`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/src/pynws/urls.py` & `pynws-1.8.0/src/pynws/urls.py`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/src/pynws.egg-info/PKG-INFO` & `pynws-1.8.0/src/pynws.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynws
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python library to retrieve observations and forecasts from NWS/NOAA
 Author-email: Matthew Flamm <matthewhflamm0@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/MatthewFlamm/pynws
 Project-URL: Bug Tracker, https://github.com/MatthewFlamm/pynws/issues
 Keywords: nws,weather
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pynws-1.7.0/src/pynws.egg-info/SOURCES.txt` & `pynws-1.8.0/src/pynws.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 tests/fixtures/__init__.py
 tests/fixtures/alerts_active_zone.json
 tests/fixtures/alerts_active_zone_second.json
 tests/fixtures/detailed_forecast.json
 tests/fixtures/gridpoints_forecast.json
 tests/fixtures/gridpoints_forecast_empty.json
 tests/fixtures/gridpoints_forecast_hourly.json
+tests/fixtures/gridpoints_forecast_hourly_empty.json
 tests/fixtures/gridpoints_forecast_strings.json
 tests/fixtures/gridpoints_stations.json
 tests/fixtures/points.json
 tests/fixtures/stations_observations.json
 tests/fixtures/stations_observations_alternate_units.json
 tests/fixtures/stations_observations_empty.json
 tests/fixtures/stations_observations_latest.json
```

### Comparing `pynws-1.7.0/tests/conftest.py` & `pynws-1.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/alerts_active_zone.json` & `pynws-1.8.0/tests/fixtures/alerts_active_zone.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/alerts_active_zone_second.json` & `pynws-1.8.0/tests/fixtures/alerts_active_zone_second.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/detailed_forecast.json` & `pynws-1.8.0/tests/fixtures/detailed_forecast.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/gridpoints_forecast.json` & `pynws-1.8.0/tests/fixtures/gridpoints_forecast.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/gridpoints_forecast_empty.json` & `pynws-1.8.0/tests/fixtures/gridpoints_forecast_empty.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/gridpoints_forecast_hourly.json` & `pynws-1.8.0/tests/fixtures/gridpoints_forecast_hourly.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/gridpoints_forecast_strings.json` & `pynws-1.8.0/tests/fixtures/gridpoints_forecast_strings.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/gridpoints_stations.json` & `pynws-1.8.0/tests/fixtures/gridpoints_stations.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/points.json` & `pynws-1.8.0/tests/fixtures/points.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/stations_observations.json` & `pynws-1.8.0/tests/fixtures/stations_observations.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/stations_observations_alternate_units.json` & `pynws-1.8.0/tests/fixtures/stations_observations_alternate_units.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/stations_observations_empty.json` & `pynws-1.8.0/tests/fixtures/stations_observations_empty.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/stations_observations_latest.json` & `pynws-1.8.0/tests/fixtures/stations_observations_latest.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/stations_observations_metar.json` & `pynws-1.8.0/tests/fixtures/stations_observations_metar.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/stations_observations_metar_noparse.json` & `pynws-1.8.0/tests/fixtures/stations_observations_metar_noparse.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/stations_observations_missing_value.json` & `pynws-1.8.0/tests/fixtures/stations_observations_missing_value.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/stations_observations_multiple.json` & `pynws-1.8.0/tests/fixtures/stations_observations_multiple.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/stations_observations_multiple_unsorted.json` & `pynws-1.8.0/tests/fixtures/stations_observations_multiple_unsorted.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/stations_observations_other_unitcode.json` & `pynws-1.8.0/tests/fixtures/stations_observations_other_unitcode.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/fixtures/stations_observations_strings.json` & `pynws-1.8.0/tests/fixtures/stations_observations_strings.json`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/helpers.py` & `pynws-1.8.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/test_nws.py` & `pynws-1.8.0/tests/test_nws.py`

 * *Files identical despite different names*

### Comparing `pynws-1.7.0/tests/test_raw.py` & `pynws-1.8.0/tests/test_raw.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,20 +40,19 @@
     app = setup_app()
     client = await aiohttp_client(app)
     with pytest.raises(
         ValueError, match="start parameter needs to be datetime, but got"
     ):
         await raw_data.raw_stations_observations(STATION, client, USERID, start="1PM")
     with pytest.raises(ValueError, match="start parameter must be timezone aware"):
-        # utcnow is confusingly returns naive
         await raw_data.raw_stations_observations(
             STATION,
             client,
             USERID,
-            start=datetime.utcnow(),  # noqa: DTZ003
+            start=datetime.now(),
         )
 
 
 async def test_detailed_forecast(aiohttp_client, mock_urls):
     app = setup_app()
     client = await aiohttp_client(app)
     await raw_data.raw_detailed_forecast(WFO, X, Y, client, USERID)
```

