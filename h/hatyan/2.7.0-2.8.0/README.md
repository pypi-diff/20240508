# Comparing `tmp/hatyan-2.7.0.tar.gz` & `tmp/hatyan-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatyan-2.7.0.tar", last modified: Thu Aug  3 10:48:34 2023, max compression
+gzip compressed data, was "hatyan-2.8.0.tar", last modified: Wed May  8 11:48:30 2024, max compression
```

## Comparing `hatyan-2.7.0.tar` & `hatyan-2.8.0.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 10:48:34.814918 hatyan-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-08-03 10:48:16.000000 hatyan-2.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3790 2023-08-03 10:48:34.814918 hatyan-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2730 2023-08-03 10:48:16.000000 hatyan-2.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 10:48:34.810918 hatyan-2.7.0/hatyan/
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    30963 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/analysis_prediction.py
--rw-r--r--   0 runner    (1001) docker     (122)    57251 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/astrog.py
--rw-r--r--   0 runner    (1001) docker     (122)    10775 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/components.py
--rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 10:48:34.810918 hatyan-2.7.0/hatyan/data/
--rw-r--r--   0 runner    (1001) docker     (122)     1453 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/data/data_M2phasediff_perstation.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/data/data_foreman_frequencies.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4857 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/data/data_foreman_harmonic.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4004 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/data/data_foreman_shallowrelations.txt
--rw-r--r--   0 runner    (1001) docker     (122)    10407 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/data/data_schureman_harmonic.csv
--rw-r--r--   0 runner    (1001) docker     (122)     6918 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/data/data_schureman_shallowrelations.csv
--rw-r--r--   0 runner    (1001) docker     (122)    10666 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/data/leap-seconds.list
--rw-r--r--   0 runner    (1001) docker     (122)    19158 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/foreman.py
--rw-r--r--   0 runner    (1001) docker     (122)    25385 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/getonlinedata.py
--rw-r--r--   0 runner    (1001) docker     (122)    26586 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/hatyan_core.py
--rw-r--r--   0 runner    (1001) docker     (122)     7360 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/kw_gemgetij.py
--rw-r--r--   0 runner    (1001) docker     (122)     9960 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/kw_havengetallen.py
--rw-r--r--   0 runner    (1001) docker     (122)    18245 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/kw_overschrijding.py
--rw-r--r--   0 runner    (1001) docker     (122)    11554 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/kw_slotgemiddelden.py
--rw-r--r--   0 runner    (1001) docker     (122)    17662 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/schureman.py
--rw-r--r--   0 runner    (1001) docker     (122)    87281 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (122)     6547 2023-08-03 10:48:16.000000 hatyan-2.7.0/hatyan/wrapper_RWS.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 10:48:34.810918 hatyan-2.7.0/hatyan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3790 2023-08-03 10:48:34.000000 hatyan-2.7.0/hatyan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-08-03 10:48:34.000000 hatyan-2.7.0/hatyan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 10:48:34.000000 hatyan-2.7.0/hatyan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 10:48:34.000000 hatyan-2.7.0/hatyan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-08-03 10:48:34.000000 hatyan-2.7.0/hatyan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-08-03 10:48:34.000000 hatyan-2.7.0/hatyan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-08-03 10:48:16.000000 hatyan-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-08-03 10:48:16.000000 hatyan-2.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-08-03 10:48:34.814918 hatyan-2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-08-03 10:48:16.000000 hatyan-2.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 10:48:34.814918 hatyan-2.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 10:48:16.000000 hatyan-2.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-08-03 10:48:16.000000 hatyan-2.7.0/tests/test_astrog_main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1618 2023-08-03 10:48:16.000000 hatyan-2.7.0/tests/test_hatyan_examples.py
--rw-r--r--   0 runner    (1001) docker     (122)    60311 2023-08-03 10:48:16.000000 hatyan-2.7.0/tests/test_hatyan_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:48:30.367514 hatyan-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-08 11:47:54.000000 hatyan-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-08 11:47:54.000000 hatyan-2.8.0/LICENSE.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-08 11:48:30.367514 hatyan-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-08 11:47:54.000000 hatyan-2.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:48:30.363514 hatyan-2.8.0/hatyan/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29715 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/analysis_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56606 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/astrog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17446 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:48:30.363514 hatyan-2.8.0/hatyan/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/data/data_M2phasediff_perstation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/data/data_foreman_frequencies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/data/data_foreman_harmonic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/data/data_foreman_shallowrelations.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10407 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/data/data_schureman_harmonic.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/data/data_schureman_shallowrelations.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/data/leap-seconds.list
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/ddlpy_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18222 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/foreman.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23661 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/hatyan_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16842 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/schureman.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89004 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-08 11:47:54.000000 hatyan-2.8.0/hatyan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:48:30.367514 hatyan-2.8.0/hatyan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-08 11:48:30.000000 hatyan-2.8.0/hatyan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-08 11:48:30.000000 hatyan-2.8.0/hatyan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:48:30.000000 hatyan-2.8.0/hatyan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-08 11:48:30.000000 hatyan-2.8.0/hatyan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 11:48:30.000000 hatyan-2.8.0/hatyan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 11:48:30.000000 hatyan-2.8.0/hatyan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-08 11:47:54.000000 hatyan-2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 11:48:30.367514 hatyan-2.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:48:30.367514 hatyan-2.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    33351 2024-05-08 11:47:54.000000 hatyan-2.8.0/tests/test_analysis_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-08 11:47:54.000000 hatyan-2.8.0/tests/test_astrog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-08 11:47:54.000000 hatyan-2.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-08 11:47:54.000000 hatyan-2.8.0/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-08 11:47:54.000000 hatyan-2.8.0/tests/test_ddlpy_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-08 11:47:54.000000 hatyan-2.8.0/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-08 11:47:54.000000 hatyan-2.8.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43925 2024-05-08 11:47:54.000000 hatyan-2.8.0/tests/test_hatyan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-05-08 11:47:54.000000 hatyan-2.8.0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19347 2024-05-08 11:47:54.000000 hatyan-2.8.0/tests/test_timeseries.py
```

### Comparing `hatyan-2.7.0/README.md` & `hatyan-2.8.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,19 @@
+[![pytest](https://github.com/Deltares/hatyan/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest.yml)
 [![codecov](https://img.shields.io/codecov/c/github/deltares/hatyan.svg?style=flat-square)](https://app.codecov.io/gh/deltares/hatyan)
-[![pytest-hmcenv](https://github.com/Deltares/hatyan/actions/workflows/pytest-hmcenv.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest-devenv.yml)
-[![pytest-py38](https://github.com/Deltares/hatyan/actions/workflows/pytest-py38.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest-py38.yml)
-[![pytest-py39](https://github.com/Deltares/hatyan/actions/workflows/pytest-py39.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest-py39.yml)
-[![pytest-py310](https://github.com/Deltares/hatyan/actions/workflows/pytest-py310.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest-py310.yml)
-[![pytest-py311](https://github.com/Deltares/hatyan/actions/workflows/pytest-py311.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/pytest-py311.yml)
-[![sigrid-publish](https://github.com/Deltares/hatyan/actions/workflows/sigrid-publish.yml/badge.svg?branch=main)](https://github.com/Deltares/hatyan/actions/workflows/sigrid-publish.yml)
-[![pypi-upload](https://github.com/Deltares/hatyan/actions/workflows/pypi-upload.yml/badge.svg?event=release)](https://github.com/Deltares/hatyan/actions/workflows/pypi-upload.yml)
-[![Supported versions](https://img.shields.io/pypi/pyversions/hatyan.svg)](https://pypi.org/project/hatyan)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_hatyan&metric=alert_status)](https://sonarcloud.io/dashboard?id=Deltares_hatyan)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/hatyan/HEAD?urlpath=/tree/docs/notebooks)
+[![Available on pypi](https://img.shields.io/pypi/v/hatyan.svg)](https://pypi.python.org/pypi/hatyan)
+[![Supported versions](https://img.shields.io/pypi/pyversions/hatyan.svg)](https://pypi.org/project/hatyan)
+[![Downloads](https://img.shields.io/pypi/dm/hatyan.svg)](https://pypistats.org/packages/hatyan)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6885342.svg)](https://doi.org/10.5281/zenodo.6885342)
 
 # hatyan
 
-A Python package for harmonic tidal analysis and prediction, based on the FORTRAN version and developed for Rijkswaterstaat. Hatyan contains the methods to derive water level extremes (high and low waters) and several other water level indicators (Kenmerkende Waarden). Furthermore, hatyan provides easier access to Rijkswaterstaat data via their data distribution layer (DataDistributieLaag, DDL).
+A Python package for harmonic tidal analysis and prediction, based on the FORTRAN version and developed for Rijkswaterstaat. Hatyan also contains methods to derive water level extremes (high and low waters) and it is a dependency to derive the [Kenmerkende Waarden](https://github.com/Deltares-research/kenmerkendewaarden).
 
 ## Information
 
 - install with ``pip install hatyan -U``
-- [online documentation](https://deltares.github.io/hatyan) with contributing guide, tutorials/examples, API reference and a convenient search box.
+- [online documentation](https://deltares.github.io/hatyan) with contributing guide, tutorials/examples and an API reference.
 - [docs folder](https://github.com/Deltares/hatyan/tree/main/docs) with background information
-- Bug or feature request? Create a [GitHub issue](https://github.com/Deltares/dfm_tools/issues)
+- Bug or feature request? Create a [GitHub issue](https://github.com/Deltares/hatyan/issues)
```

### Comparing `hatyan-2.7.0/hatyan/__init__.py` & `hatyan-2.8.0/hatyan/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # -*- coding: utf-8 -*-
 """
-.. include:: ../README.md
+Tidal analysis and prediction tool of Rijkswaterstaat
 """
 
 __author__ = """Jelmer Veenstra"""
-__email__ = 'jelmer.veenstra@deltares.nl'
-__version__ = '2.7.0'
+__email__ = "jelmer.veenstra@deltares.nl"
+__version__ = "2.8.0"
 
 from hatyan.analysis_prediction import *
 from hatyan.astrog import *
 from hatyan.components import *
+from hatyan.deprecated import *
+from hatyan.ddlpy_helpers import *
 from hatyan.hatyan_core import *
-from hatyan.foreman import *
-from hatyan.schureman import *
 from hatyan.timeseries import *
-from hatyan.wrapper_RWS import *
-from hatyan.getonlinedata import *
-from hatyan.convert import *
-from hatyan.kw_slotgemiddelden import *
-from hatyan.kw_havengetallen import *
-from hatyan.kw_gemgetij import *
-from hatyan.kw_overschrijding import *
+from hatyan.utils import close
+
+import warnings
+warnings.filterwarnings(action='always', category=DeprecationWarning)
```

### Comparing `hatyan-2.7.0/hatyan/analysis_prediction.py` & `hatyan-2.8.0/hatyan/analysis_prediction.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 # -*- coding: utf-8 -*-
 """
 analysis_prediction.py contains hatyan definitions related to tidal analysis and prediction. 
-
-hatyan is a Python program for tidal analysis and prediction, based on the FORTRAN version. 
-Copyright (C) 2019-2021 Rijkswaterstaat.  Maintained by Deltares, contact: Jelmer Veenstra (jelmer.veenstra@deltares.nl). 
-Source code available at: https://github.com/Deltares/hatyan
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Lesser General Public License for more details.
-
-You should have received a copy of the GNU Lesser General Public License
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
 """
 
 import numpy as np
 import pandas as pd
 import datetime as dt
-import warnings
-warnings.filterwarnings(action='always', category=DeprecationWarning)
+import logging
 
-from hatyan.hatyan_core import get_const_list_hatyan, sort_const_list, robust_timedelta_sec, robust_daterange_fromtimesextfreq
+from hatyan.hatyan_core import get_const_list_hatyan, sort_const_list, robust_timedelta_sec
 from hatyan.hatyan_core import get_freqv0_generic, get_uf_generic
-from hatyan.timeseries import check_ts, nyquist_folding, check_rayleigh
+from hatyan.timeseries import Timeseries_Statistics, nyquist_folding, check_rayleigh
+from hatyan.metadata import metadata_from_obj, metadata_add_to_obj
+from hatyan.deprecated import (deprecated_python_option,
+                               DEPRECATED_OPTIONS_PREDICTION_DICT,
+                               DEPRECATED_OPTIONS_ANALYSIS_DICT)
+
+__all__ = ["analysis",
+           "prediction",
+           ]
+
+logger = logging.getLogger(__name__)
 
 
 class PydanticConfig:
     #https://docs.pydantic.dev/usage/model_config/
     arbitrary_types_allowed = True #necessary to allow for pd.DataFrame etc
 
 
@@ -42,106 +33,73 @@
 
 
 class HatyanSettings:
     """
     Settings class containing default hatyan settings, to be overwritten by input, initiate with:
     hatyan_settings = hatyan.HatyanSettings(nodalfactors=False)
 
-    source : TYPE, optional
-        DESCRIPTION. The default is 'schureman'.
-    nodalfactors : bool, optional
-        Whether or not to apply nodal factors. The default is True.
-    fu_alltimes : bool, optional
-        Whether to calculate nodal factors in middle of the analysis/prediction period (default) or on every timestep. The default is True.
-    xfac : bool, optional
-        Whether or not to apply x-factors. The default is False.
-    
-    #following are only for analysis
-    CS_comps : pandas.DataFrame, optional
-        contains the from/derive component lists for components splitting, as well as the amplitude factor and the increase in degrees. The default is None.
-    
-    #following are only for get_components_from_ts
-    analysis_perperiod : False or Y/Q/W, optional
-        caution, it tries to analyse each year/quarter/month, but skips if it fails. The default is False.
-    return_allperiods : bool, optional
-        DESCRIPTION. The default is False.
-    return_prediction : bool, optional
-        Whether to generate a prediction for the ts time array. The default is False.
-    
     """
-    #TODO: analysis_peryear,analysis_permonth,return_allyears only for get_components_from_ts, return_prediction only for analysis. Merge analysis and get_components_from_ts? Remove some from HatyanSettings class or maybe split? Add const_list to HatyanSettings?
-    
-    def __init__(self, source='schureman', nodalfactors=True, fu_alltimes=True, xfac=False, #prediction/analysis 
-                 CS_comps=None, analysis_perperiod=False, return_allperiods=False, 
-                 analysis_peryear=None, analysis_permonth=None, return_allyears=None,  #TODO: should be phased out, replaced by analysis_perperiod and return_allperiods
-                 return_prediction=False,
-                 xTxmat_condition_max=12): #analysis only
-        if not isinstance(source,str):
-            raise Exception('invalid source type, should be str')
-        source = source.lower()
-        if source not in ['schureman','foreman']:
-            raise Exception('invalid source {source}, should be schureman or foreman)')
-        
-        #for arguments that will be phased out, are now written to newer arguments and overwritten with None #TODO: phase out arguments
-        if analysis_peryear is not None:
-            if analysis_peryear:
-                warnings.warn("WARNING: argument analysis_peryear will be phased out, use analysis_perperiod='Y' instead", category=DeprecationWarning)
-                analysis_perperiod = 'Y'
-            else:
-                warnings.warn("WARNING: argument analysis_peryear will be phased out, use analysis_perperiod=False instead", category=DeprecationWarning)
-            analysis_peryear = None
-        if analysis_permonth is not None:
-            if analysis_permonth:
-                warnings.warn("WARNING: argument analysis_permonth will be phased out, use analysis_perperiod='M' instead", category=DeprecationWarning)
-                analysis_perperiod = 'M'
-            else:
-                warnings.warn("WARNING: argument analysis_permonth will be phased out, use analysis_perperiod=False instead", category=DeprecationWarning)
-            analysis_permonth = None
-        if return_allyears is not None:
-            warnings.warn("WARNING: argument return_allyears will be phased out, use return_allperiods instead", category=DeprecationWarning)
-            return_allperiods = return_allyears
-            return_allyears = None
-        
-        for var_in in [nodalfactors,fu_alltimes,return_allperiods,return_prediction]:
-            if not isinstance(var_in,bool):
-                raise Exception(f'invalid {var_in} type, should be bool')
+    
+    def __init__(self, 
+                 nodalfactors, fu_alltimes, xfac, source, #prediction/analysis 
+                 cs_comps=None, analysis_perperiod=None, return_allperiods=None, #analysis only
+                 max_matrix_condition=None): #analysis only
         
-        if not (isinstance(xfac,bool) or isinstance(xfac,dict)):
-            raise Exception(f'invalid xfac={xfac} type, should be bool or dict')
+        if not isinstance(nodalfactors,bool):
+            raise TypeError(f'invalid nodalfactors={nodalfactors} type, should be bool')
+        self.nodalfactors = nodalfactors
         
-        if not ((analysis_perperiod is False) or (analysis_perperiod in ['Y','Q','M'])):
-            raise Exception(f'invalid analysis_perperiod={analysis_perperiod} type, should be False or Y/Q/M')
+        if not isinstance(fu_alltimes,bool):
+            raise TypeError(f'invalid fu_alltimes={fu_alltimes} type, should be bool')
+        self.fu_alltimes = fu_alltimes
         
-        if CS_comps is not None:
-            if not isinstance(CS_comps,(dict,pd.DataFrame)):
-                raise Exception('invalid CS_comps type, should be dict')
-            CS_comps = pd.DataFrame(CS_comps) #TODO: convert all to dict or pd.DataFrame
-            CS_comps_expectedkeys = ['CS_comps_derive', 'CS_comps_from', 'CS_ampfacs', 'CS_degincrs']
-            for CS_comps_key in CS_comps_expectedkeys:
-                if CS_comps_key not in CS_comps.keys():
-                    raise Exception(f'CS_comps does not contain {CS_comps_key}')
-            CS_comps_lenvals = [len(CS_comps[key]) for key in CS_comps]
-            if len(np.unique(CS_comps_lenvals)) != 1:
-                raise Exception(f'CS_comps keys do not have equal lengths:\n{CS_comps}')
+        if not (isinstance(xfac,bool) or isinstance(xfac,dict)):
+            raise TypeError(f'invalid xfac={xfac} type, should be bool or dict')
+        self.xfac = xfac
         
+        if not isinstance(source,str):
+            raise TypeError(f'invalid source={source} type, should be str')
+        source = source.lower()
+        if source not in ['schureman','foreman']:
+            raise TypeError(f'invalid source {source}, should be "schureman" or "foreman"')
         self.source = source
-        self.nodalfactors = nodalfactors
-        self.fu_alltimes = fu_alltimes
-        self.xfac = xfac
-        self.CS_comps = CS_comps
-        self.analysis_perperiod = analysis_perperiod
-        self.return_allperiods = return_allperiods
-        self.return_prediction = return_prediction
-        self.xTxmat_condition_max = xTxmat_condition_max
+                
+        if return_allperiods is not None:
+            if not isinstance(return_allperiods,bool):
+                raise TypeError(f'invalid return_allperiods={return_allperiods} type, should be bool')
+            self.return_allperiods = return_allperiods
+        
+        if analysis_perperiod is not None:
+            if not ((analysis_perperiod is False) or (analysis_perperiod in ['Y','Q','M'])):
+                raise TypeError(f'invalid analysis_perperiod={analysis_perperiod} type, should be False or Y/Q/M')
+            self.analysis_perperiod = analysis_perperiod
+        
+        if cs_comps is not None:
+            if not isinstance(cs_comps,(dict,pd.DataFrame)):
+                raise TypeError('invalid cs_comps type, should be dict')
+            cs_comps = pd.DataFrame(cs_comps) #TODO: convert all to dict or pd.DataFrame
+            cs_comps_expectedkeys = ['CS_comps_derive', 'CS_comps_from', 'CS_ampfacs', 'CS_degincrs']
+            for cs_comps_key in cs_comps_expectedkeys:
+                if cs_comps_key not in cs_comps.keys():
+                    raise KeyError(f'cs_comps does not contain {cs_comps_key}')
+            cs_comps_lenvals = [len(cs_comps[key]) for key in cs_comps]
+            if len(np.unique(cs_comps_lenvals)) != 1:
+                raise ValueError(f'cs_comps keys do not have equal lengths:\n{cs_comps}')
+            self.cs_comps = cs_comps
+        
+        if max_matrix_condition is not None:
+            if not isinstance(max_matrix_condition,int) or isinstance(max_matrix_condition,float):
+                raise TypeError(f'invalid {max_matrix_condition} type, should be int or float')
+            self.max_matrix_condition = max_matrix_condition
         
     def __str__(self):
         self_dict = vars(self)
         str_append = ''
         for key,val in self_dict.items():
-            if key=='CS_comps' and self.CS_comps is not None:
+            if key=='cs_comps':
                 str_append += f'{key:20s} = \n{val}\n'
             else:
                 str_append += f'{key:20s} = {val}\n'
         return str_append
 
 
 def vectoravg(A_all, phi_deg_all):
@@ -172,174 +130,187 @@
     mean_v_cos = np.mean(v_cos,axis=1)
     mean_v_sin = np.mean(v_sin,axis=1)
     A_mean = np.sqrt(mean_v_cos**2 + mean_v_sin**2)
     phi_rad_mean = np.arctan2(mean_v_sin,mean_v_cos)
     phi_rad_mean[phi_rad_mean<0] = phi_rad_mean[phi_rad_mean<0]+(2*np.pi)
     
     #if phases of all years are exactly 0, it is the A0 component. Overwrite this A0 with mean amplitude and zero phase if present, otherwise negative values will become positive with 180 phase
-    idx_A0 = np.where((phi_deg_all==0).any(axis=1))[0]
+    idx_A0 = np.nonzero((phi_deg_all==0).any(axis=1))[0]
     A_mean[idx_A0] = np.mean(A_all[idx_A0,:])
     phi_rad_mean[idx_A0] = 0
     
     phi_deg_mean = np.rad2deg(phi_rad_mean)
     
     return A_mean, phi_deg_mean
 
 
-def get_components_from_ts(ts, const_list, hatyan_settings=None, **kwargs):#nodalfactors=True, xfac=False, fu_alltimes=True, CS_comps=None, analysis_peryear=False, analysis_permonth=False, source='schureman'):
-    """
-    Wrapper around the analysis() function, 
-    it optionally processes a timeseries per year and vector averages the results afterwards, 
-    passes the rest of the arguments on to analysis function
-    The timezone of the timeseries, will also be reflected in the phases of the resulting component set, so the resulting component set can be used to make a prediction in the original timezone.
+@deprecated_python_option(**DEPRECATED_OPTIONS_ANALYSIS_DICT)
+def analysis(ts, const_list, 
+             nodalfactors=True, fu_alltimes=True, xfac=False, 
+             source='schureman',
+             cs_comps=None,
+             analysis_perperiod=False, return_allperiods=False,
+             max_matrix_condition=12):
+    """
+    Analysis of timeseries.
+    Optionally processes a timeseries per year and vector averages the results afterwards.
+    The timezone of the timeseries, will also be reflected in the phases of the resulting component set, 
+    so the resulting component set can be used to make a prediction in the original timezone.
     
     Parameters
     ----------
     ts : pandas.DataFrame
         The DataFrame should contain a 'values' column and a pd.DatetimeIndex as index, it contains the timeseries to be analysed, as obtained from e.g. readts_*.
     const_list : list, pandas.Series or str
         list or pandas.Series: contains the tidal constituent names for which to analyse the provided timeseries ts. 
         str: a predefined name of a component set for hatyan_core.get_const_list_hatyan()
-    hatyan_settings : hatyan.HatyanSettings()
-        Contains the used settings
-
-    Raises
-    ------
-    Exception
-        DESCRIPTION.
+    nodalfactors : bool
+        Whether or not to apply nodal factors. The default is True.
+    fu_alltimes : bool
+        Whether to calculate nodal factors in middle of the analysis/prediction period (default) or on every timestep. The default is True.
+    xfac : bool
+        Whether or not to apply x-factors. The default is False.
+    source : TYPE
+        DESCRIPTION. The default is 'schureman'.
+    cs_comps : pandas.DataFrame, optional
+        contains the from/derive component lists for components splitting, as well as the amplitude factor and the increase in degrees. Only relevant for analysis. The default is None.
+    max_matrix_condition: float or int
+        the maximum condition of the xTx matrix. The default is 12.
+    analysis_perperiod : False or Y/Q/W, optional
+        caution, it tries to analyse each year/quarter/month, but skips if it fails. The default is False.
+    return_allperiods : bool, optional
+        Only relevant if analysis_perperiod is not None. The default is False.
+    
 
     Returns
     -------
     COMP_mean_pd : pandas.DataFrame
         The DataFrame contains the component data with component names as index, and colums 'A' and 'phi_deg'.
     COMP_all_pd : pandas.DataFrame, optional
         The same as COMP_mean_pd, but with all years added with MultiIndex
     """
-    ts_pd = ts #TODO: this is not necessary
-    
-    if hatyan_settings is None:
-        hatyan_settings = HatyanSettings(**kwargs)
-    elif len(kwargs)>0:
-        raise Exception('both arguments hatyan_settings and other settings (e.g. nodalfactors) are provided, this is not valid')
+    # check ts.index type, this works better than isinstance(ts.index,pd.DatetimeIndex) since 1018 time indexes are Index instead of DatetimeIndex
+    if not (isinstance(ts.index[0],pd.Timestamp) or isinstance(ts.index[0],dt.datetime)):
+        raise TypeError(f'ts.index is not of expected type ({type(ts.index[0])} instead of pd.Timestamp or dt.datetime)')
     
-    print('running: get_components_from_ts')
+    # remove timezone from timeseries (is added to components dataframe after analysis)
+    ts_pd = ts.copy()
+    ts_pd.index = ts_pd.index.tz_localize(None)
+    
+    # validate settings
+    hatyan_settings = HatyanSettings(source=source, nodalfactors=nodalfactors, fu_alltimes=fu_alltimes, xfac=xfac,
+                                     analysis_perperiod=analysis_perperiod, return_allperiods=return_allperiods,
+                                     cs_comps=cs_comps, max_matrix_condition=max_matrix_condition)
     
+    logger.info(f'ANALYSIS initializing\n{hatyan_settings}')
+        
+    #retrieving and sorting const_list
     if type(const_list) is str:
         const_list = get_const_list_hatyan(const_list)
-    elif type(const_list) is not list:
-        const_list = const_list.tolist()
-    if hatyan_settings.CS_comps is None:
-        n_const = len(const_list)
-    else:
-        n_const = len(const_list) + len(hatyan_settings.CS_comps)
+    const_list = sort_const_list(const_list)
+    logger.info(f'n components analyzed  = {len(const_list)}')
+    
+    #check for duplicate components (results in singular matrix)
+    if len(const_list) != len(np.unique(const_list)):
+        const_list_uniq, const_list_uniq_counts = np.unique(const_list,return_counts=True)
+        const_list_counts = pd.DataFrame({'constituent':const_list_uniq,'occurences':const_list_uniq_counts})
+        raise ValueError('remove duplicate constituents from const_list:\n%s'%(const_list_counts.loc[const_list_counts['occurences']>1]))
+    
+    n_const = len(const_list)
+    if hasattr(hatyan_settings, "cs_comps"):
+        n_const = len(const_list) + len(hatyan_settings.cs_comps)
 
     if hatyan_settings.analysis_perperiod:
         period = hatyan_settings.analysis_perperiod
-        print(f'analysis_perperiod={hatyan_settings.analysis_perperiod}, separate periods are automatically determined from timeseries')
-        ts_periods_dt = ts_pd.index.to_period(period).unique() # TODO: to_period is not limited to Y/Q/M, there are more options that are now blocked: https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#offset-aliases
+        logger.info(f'analysis_perperiod={period}, separate periods are automatically determined from timeseries')
+        ts_periods_dt_all = ts_pd.index.to_period(period)
+        ts_periods_dt = ts_periods_dt_all.unique() # TODO: to_period is not limited to Y/Q/M, there are more options that are now blocked: https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#offset-aliases
         ts_periods_strlist = [str(x) for x in ts_periods_dt]
         
         n_periods = len(ts_periods_dt)
         A_i_all = np.zeros((n_const,n_periods))*np.nan
         phi_i_deg_all = np.zeros((n_const,n_periods))*np.nan
         for iP, period_dt in enumerate(ts_periods_dt):
-            print('analyzing %s of sequence %s'%(period_dt,ts_periods_strlist))
-            ts_oneperiod_pd = ts_pd[ts_pd.index.to_period(period)==period_dt]
+            logger.info('analyzing %s of sequence %s'%(period_dt,ts_periods_strlist))
+            ts_oneperiod_pd = ts_pd[ts_periods_dt_all==period_dt]
             try:
-                COMP_one = analysis(ts_oneperiod_pd, const_list=const_list, hatyan_settings=hatyan_settings)
+                COMP_one = analysis_singleperiod(ts_oneperiod_pd, const_list=const_list, hatyan_settings=hatyan_settings)
                 A_i_all[:,iP] = COMP_one.loc[:,'A']
                 phi_i_deg_all[:,iP] = COMP_one.loc[:,'phi_deg']
             except MatrixConditionTooHigh: # accept exception if matrix condition is too high, since some years can then be skipped
-                print(f'WARNING: analysis of {period_dt} failed because MatrixConditionTooHigh, check if const_list is appropriate for timeseries lenght.')
+                logger.warning(f'analysis of {period_dt} failed because MatrixConditionTooHigh, check if const_list is appropriate for timeseries lenght.')
         if np.isnan(A_i_all).all():
-            raise Exception('analysis peryear or permonth failed for all years/months, check warnings above')
+            raise ValueError('all nans: analysis perperiod failed for all periods, check warnings above')
         
         COMP_all_pd = pd.DataFrame(data=np.hstack([A_i_all,phi_i_deg_all]), columns=pd.MultiIndex.from_product([['A','phi_deg'],ts_periods_dt]), index=COMP_one.index)
-        print('vector averaging analysis results')
+        logger.info('vector averaging analysis results')
         A_i_mean, phi_i_deg_mean = vectoravg(A_all=A_i_all, phi_deg_all=phi_i_deg_all)
         COMP_mean_pd = pd.DataFrame({ 'A': A_i_mean, 'phi_deg': phi_i_deg_mean},index=COMP_one.index)
-
     else: #dummy values, COMP_years should be equal to COMP_mean
-        COMP_mean_pd = analysis(ts_pd, const_list=const_list, hatyan_settings=hatyan_settings)
+        COMP_mean_pd = analysis_singleperiod(ts_pd, const_list=const_list, hatyan_settings=hatyan_settings)
         COMP_all_pd = None
     
+    #add metadata
+    metadata = metadata_from_obj(ts_pd)
+    metadata['nodalfactors'] = hatyan_settings.nodalfactors
+    metadata['xfac'] = hatyan_settings.xfac
+    metadata['fu_alltimes'] = hatyan_settings.fu_alltimes
+    metadata['source'] = hatyan_settings.source
+    metadata['tzone'] = ts.index.tz
+    COMP_mean_pd = metadata_add_to_obj(COMP_mean_pd, metadata)
+    
     if hatyan_settings.return_allperiods:
+        COMP_all_pd = metadata_add_to_obj(COMP_all_pd, metadata)
         return COMP_mean_pd, COMP_all_pd
-    else:
-        return COMP_mean_pd
+    
+    logger.info('ANALYSIS finished')
+    
+    return COMP_mean_pd
 
 
-def analysis(ts, const_list, hatyan_settings=None, **kwargs):#nodalfactors=True, xfac=False, fu_alltimes=True, CS_comps=None, return_prediction=False, source='schureman'):
+def analysis_singleperiod(ts, const_list, hatyan_settings):
     """
     harmonic analysis with matrix transformations (least squares fit), optionally with component splitting
-    for details about arguments and return variables, see get_components_from_ts() definition
+    for details about arguments and return variables, see analysis() definition
     
     """
     
-    if hatyan_settings is None:
-        hatyan_settings = HatyanSettings(**kwargs)
-    elif len(kwargs)>0:
-        raise Exception('both arguments hatyan_settings and other settings (e.g. nodalfactors) are provided, this is not valid')
-
-    print('ANALYSIS initializing')
-    print(hatyan_settings)
-        
     #drop duplicate times
     bool_ts_duplicated = ts.index.duplicated(keep='first')
     ts_pd = ts.copy() #TODO: this is not necessary
-    if not (isinstance(ts.index[0],pd.Timestamp) or isinstance(ts.index[0],dt.datetime)): #works better than isinstance(ts.index,pd.DatetimeIndex) since 1018 time indexes are Index instead of DatetimeIndex
-        raise TypeError(f'ts.index is not of expected type ({type(ts.index[0])} instead of pd.Timestamp or dt.datetime)')
     if bool_ts_duplicated.any():
-        raise Exception(f'ERROR: {bool_ts_duplicated.sum()} duplicate timesteps in provided timeseries, remove them e.g. with: ts = ts[~ts.index.duplicated(keep="first")]')
-    print(f'#timesteps           = {len(ts)}')
-    print(f'tstart               = {ts.index[0].strftime("%Y-%m-%d %H:%M:%S")}')
-    print(f'tstop                = {ts.index[-1].strftime("%Y-%m-%d %H:%M:%S")}')
-    if hasattr(ts.index,'freq'):
-        print(f'timestep             = {ts.index.freq}')
-    
-    #retrieving and sorting const_list
-    if type(const_list) is str:
-        const_list = get_const_list_hatyan(const_list)
-    elif type(const_list) is not list:
-        const_list = const_list.tolist()
-    const_list = sort_const_list(const_list)
-    print(f'components analyzed  = {len(const_list)}')
-    
-    #check for duplicate components (results in singular matrix)
-    if len(const_list) != len(np.unique(const_list)):
-        const_list_uniq, const_list_uniq_counts = np.unique(const_list,return_counts=True)
-        const_list_counts = pd.DataFrame({'constituent':const_list_uniq,'occurences':const_list_uniq_counts})
-        raise Exception('remove duplicate constituents from const_list:\n%s'%(const_list_counts.loc[const_list_counts['occurences']>1]))
-    
-    #check for length
-    if len(ts_pd)<2:
-        raise Exception('provided timeseries is less than 2 timesteps long, analysis not possible')
+        raise ValueError(f'{bool_ts_duplicated.sum()} duplicate timesteps in provided timeseries, remove them e.g. with: ts = ts[~ts.index.duplicated(keep="first")]')
+    message = (f'#timesteps    = {len(ts)}\n'
+               f'tstart        = {ts.index[0].strftime("%Y-%m-%d %H:%M:%S")}\n'
+               f'tstop         = {ts.index[-1].strftime("%Y-%m-%d %H:%M:%S")}\n'
+               f'timestep      = {ts.index.freq}')
+    logger.info(message)
 
     #remove nans
     ts_pd_nonan = ts_pd[~ts_pd['values'].isna()]
-    if len(ts_pd_nonan)==0:
-        raise Exception('provided timeseries only contains nan values, analysis not possible')
+    if len(ts_pd_nonan)<2:
+        raise ValueError(f'provided timeseries is less than 2 timesteps long (after dropping potential nans), analysis not possible:\n{ts_pd_nonan}')
     times_pred_all_pdDTI = ts_pd_nonan.index.copy() #pd.DatetimeIndex(ts_pd_nonan.index) #TODO: this will not work for OutOfBoundsDatetime
     percentage_nan = 100-len(ts_pd_nonan['values'])/len(ts_pd['values'])*100
-    print(f'percentage_nan in values_meas_sel: {percentage_nan:.2f}%')
+    logger.info(f'percentage_nan in values_meas_sel: {percentage_nan:.2f}%')
     
     #get times and time array
-    dood_date_mid = pd.Index([ts_pd.index[len(ts_pd.index)//2]]) #middle of analysis period (2july in case of 1jan-1jan), zoals bij hatyan #TODO: this is incorrect in case of e.g. more missings in first half of year than second half
+    dood_date_mid = ts_pd.index[[len(ts_pd.index)//2]] #middle of analysis period (2july in case of 1jan-1jan), zoals bij hatyan #TODO: this is incorrect in case of e.g. more missings in first half of year than second half
     dood_date_start = ts_pd.index[[0]] #first date (for v0, also freq?)
     if hatyan_settings.fu_alltimes:
         dood_date_fu = times_pred_all_pdDTI
     else:
         dood_date_fu = dood_date_mid
     times_from0_s = robust_timedelta_sec(ts_pd_nonan.index,refdate_dt=dood_date_start[0])
     times_from0_s = times_from0_s[:,np.newaxis]
     
     #get frequency and v0
-    t_const_freq_pd, v_0i_rad = get_freqv0_generic(hatyan_settings, const_list, dood_date_mid, dood_date_start)
+    t_const_freq_pd, v_0i_rad = get_freqv0_generic(const_list, dood_date_mid, dood_date_start, hatyan_settings.source)
     omega_i_rads = t_const_freq_pd[['freq']].values.T*(2*np.pi)/3600 #angular frequency, 2pi/T, in rad/s, https://en.wikipedia.org/wiki/Angular_frequency (2*np.pi)/(1/x*3600) = 2*np.pi*x/3600
-    u_i_rad, f_i = get_uf_generic(hatyan_settings, const_list, dood_date_fu)
+    u_i_rad, f_i = get_uf_generic(const_list, dood_date_fu, hatyan_settings.nodalfactors, hatyan_settings.xfac, hatyan_settings.source)
     v_u = v_0i_rad.values + u_i_rad.values
     
     #check rayleigh frequency after nyquist frequency folding process.
     freq_rem = nyquist_folding(ts_pd,t_const_freq_pd)
     check_rayleigh(ts_pd,freq_rem) #TODO: maybe sometimes valuable to not fold with nyquist (eg with strongly varying time interval), in that case: check_rayleigh(ts_pd,t_const_freq_pd)
 
     #### TIMESERIES ANALYSIS
@@ -348,192 +319,149 @@
     
     # get xmat and make dot product
     xmat = np.zeros((m,2*N))
     xmat[:,:N] = f_i.values * np.cos(omega_i_rads*times_from0_s+v_u)
     xmat[:,N:] = f_i.values * np.sin(omega_i_rads*times_from0_s+v_u)
     
     xTmat = xmat.T
-    print('calculating xTx matrix')
+    logger.info('calculating xTx matrix')
     tic = dt.datetime.now()
     xTxmat = np.dot(xTmat,xmat)
     
     if 'A0' in const_list: #correct center value [N,N] for better matrix condition
         xTxmat_condition = np.linalg.cond(xTxmat)
-        print('condition of xTx matrix before center adjustment for A0: %.2f'%(xTxmat_condition))
+        logger.debug('condition of xTx matrix before center adjustment for A0: %.2f'%(xTxmat_condition))
         xTxmat[N,N] = m
     xTxmat_condition = np.linalg.cond(xTxmat)
-    print('condition of xTx matrix: %.2f'%(xTxmat_condition))
-    if xTxmat_condition > hatyan_settings.xTxmat_condition_max:#10:#100: #random treshold
-        raise MatrixConditionTooHigh(f'ERROR: condition of xTx matrix is too high ({xTxmat_condition:.2f}), check your timeseries length, try different (shorter) component set or componentsplitting.\nAnalysed {check_ts(ts_pd)}')
+    logger.info('condition of xTx matrix: %.2f'%(xTxmat_condition))
+    if xTxmat_condition > hatyan_settings.max_matrix_condition:#10:#100: #random treshold
+        raise MatrixConditionTooHigh(f'ERROR: condition of xTx matrix is too high ({xTxmat_condition:.2f}), check your timeseries length, try different (shorter) component set or componentsplitting.\nAnalysed {Timeseries_Statistics(ts_pd)}')
     xTymat = np.dot(xTmat,ts_pd_nonan['values'].values)
     
     #solve matrix to get beta_roof_mat (and thus a, b)
     beta_roof_mat = np.linalg.solve(xTxmat,xTymat)
-    print('matrix system solved, elapsed time: %s'%(dt.datetime.now()-tic))
+    logger.info('matrix system solved, elapsed time: %s'%(dt.datetime.now()-tic))
 
     phi_i_rad = np.arctan2(beta_roof_mat[N:],beta_roof_mat[:N]) #(a,b) arctan_ab
     A_i = np.sqrt(beta_roof_mat[N:]**2 + beta_roof_mat[:N]**2) #(a,b) sqsqrt_ab
 
     COMP_pd = pd.DataFrame({'A': A_i, 'phi_deg': np.rad2deg(phi_i_rad%(2*np.pi))}, index=const_list)
     if 'A0' in COMP_pd.index: #correct 180 degrees A0 phase by making amplitude value negative
         if COMP_pd.loc['A0','phi_deg']==180:
             COMP_pd.loc['A0','A'] = -COMP_pd.loc['A0','A']
             COMP_pd.loc['A0','phi_deg'] = 0
     
-    if hatyan_settings.CS_comps is not None:
+    if hasattr(hatyan_settings, "cs_comps"):
         COMP_pd = split_components(comp=COMP_pd, dood_date_mid=dood_date_mid, hatyan_settings=hatyan_settings)
         
-    print('ANALYSIS finished')
-    
-    if hatyan_settings.return_prediction:
-        print('immediately generating a prediction for the same time array as the input ts')
-        ts_prediction = prediction(comp=COMP_pd, times_pred_all=ts_pd.index, hatyan_settings=hatyan_settings)
-        return COMP_pd, ts_prediction
-    else:
-        return COMP_pd
+    return COMP_pd
 
 
-def split_components(comp, dood_date_mid, hatyan_settings=None, **kwargs):
+def split_components(comp, dood_date_mid, hatyan_settings):
     """
     component splitting function
-    for details about arguments and return variables, see get_components_from_ts() definition
+    for details about arguments and return variables, see analysis() definition
 
     """
     
-    if hatyan_settings is None:
-        hatyan_settings = HatyanSettings(**kwargs)
-    elif len(kwargs)>0:
-        raise Exception('both arguments hatyan_settings and other settings (e.g. nodalfactors) are provided, this is not valid')
-        
+    for cs_compname in hatyan_settings.cs_comps['CS_comps_derive']:
+        if cs_compname in comp.index:
+            raise ValueError(f"component {cs_compname} requested via component splitting, but already present in const_list")
+    
     #create sorted and complete component list
-    const_list_inclCS_raw = comp.index.tolist() + hatyan_settings.CS_comps['CS_comps_derive'].tolist()
-    const_list_inclCS = sort_const_list(const_list=const_list_inclCS_raw)
+    const_list_inclcs_raw = comp.index.tolist() + hatyan_settings.cs_comps['CS_comps_derive'].tolist()
+    const_list_inclcs = sort_const_list(const_list=const_list_inclcs_raw)
 
     #retrieve freq and speed
-    _, CS_v_0i_rad = get_freqv0_generic(hatyan_settings, const_list=const_list_inclCS, dood_date_mid=dood_date_mid, dood_date_start=dood_date_mid) # with split_components, v0 is calculated on the same timestep as u and f (middle of original series)
-    CS_u_i_rad, CS_f_i = get_uf_generic(hatyan_settings, const_list=const_list_inclCS, dood_date_fu=dood_date_mid)
+    _, cs_v_0i_rad = get_freqv0_generic(const_list=const_list_inclcs, dood_date_mid=dood_date_mid, dood_date_start=dood_date_mid, source=hatyan_settings.source) # with split_components, v0 is calculated on the same timestep as u and f (middle of original series)
+    cs_u_i_rad, cs_f_i = get_uf_generic(const_list=const_list_inclcs, dood_date_fu=dood_date_mid, nodalfactors=hatyan_settings.nodalfactors, xfac=hatyan_settings.xfac, source=hatyan_settings.source)
     
-    comp_inclCS = pd.DataFrame(comp,index=const_list_inclCS,columns=comp.columns)
-    #comp_inclCS_preCS = comp_inclCS.copy()
+    comp_inclcs = pd.DataFrame(comp,index=const_list_inclcs,columns=comp.columns)
         
-    for comp_main in np.unique(hatyan_settings.CS_comps['CS_comps_from']):
-        bool_CS_maincomp = hatyan_settings.CS_comps['CS_comps_from'] == comp_main #boolean of which rows of CS_comps dataframe corresponds to a main constituent, also makes it possible to select two rows
-        CS_comps_formain = hatyan_settings.CS_comps.loc[bool_CS_maincomp]
-        comp_slave_list = CS_comps_formain['CS_comps_derive'].tolist()
-        print(f'splitting component {comp_main} into {comp_slave_list}')
+    for comp_main in np.unique(hatyan_settings.cs_comps['CS_comps_from']):
+        # boolean of which rows of cs_comps dataframe corresponds to a main constituent, also makes it possible to select two rows
+        bool_cs_maincomp = hatyan_settings.cs_comps['CS_comps_from'] == comp_main
+        cs_comps_formain = hatyan_settings.cs_comps.loc[bool_cs_maincomp]
+        comp_slave_list = cs_comps_formain['CS_comps_derive'].tolist()
+        logger.info(f'splitting component {comp_main} into {comp_slave_list}')
         
         #first update main components based on degincrs/ampfacs of all components that are to be derived
         DBETA = 0
-        for iR, CS_comps_row in CS_comps_formain.iterrows():
-            comp_slave = CS_comps_row['CS_comps_derive']
+        for iR, cs_comps_row in cs_comps_formain.iterrows():
+            comp_slave = cs_comps_row['CS_comps_derive']
             #code from resuda.f, line 440 to 455
-            DMU = CS_f_i.loc[0,comp_slave]/CS_f_i.loc[0,comp_main]
-            DTHETA = CS_comps_row['CS_ampfacs']
-            DGAMMA = np.deg2rad(CS_comps_row['CS_degincrs'])-DBETA-(CS_v_0i_rad.loc[0,comp_slave]+CS_u_i_rad.loc[0,comp_slave])+(CS_v_0i_rad.loc[0,comp_main]+CS_u_i_rad.loc[0,comp_main]) #in FORTRAN code, CS_f_i slave/main is also added, this seems wrong
+            DMU = cs_f_i.loc[0,comp_slave]/cs_f_i.loc[0,comp_main]
+            DTHETA = cs_comps_row['CS_ampfacs']
+            DGAMMA = (np.deg2rad(cs_comps_row['CS_degincrs']) - 
+                      DBETA - 
+                      (cs_v_0i_rad.loc[0,comp_slave] + cs_u_i_rad.loc[0,comp_slave]) + 
+                      (cs_v_0i_rad.loc[0,comp_main] + cs_u_i_rad.loc[0,comp_main])) #in FORTRAN code, CS_f_i slave/main is also added, this seems wrong
             DREEEL = 1+DMU*DTHETA*np.cos(DGAMMA)
             DIMAGI = DMU*DTHETA*np.sin(DGAMMA)  
             DALPHA = np.sqrt(DREEEL*DREEEL+DIMAGI*DIMAGI)
             if DALPHA < 1e-50:
                 raise Exception('ERROR: DALPHA too small, component splitting failed?')
             DBETA = np.arctan2(DIMAGI,DREEEL)
             
-            comp_inclCS.loc[comp_main,'A'] = comp_inclCS.loc[comp_main,'A']/DALPHA
-            comp_inclCS.loc[comp_main,'phi_deg'] = (comp_inclCS.loc[comp_main,'phi_deg']-np.rad2deg(DBETA))%360 
+            comp_inclcs.loc[comp_main,'A'] = comp_inclcs.loc[comp_main,'A']/DALPHA
+            comp_inclcs.loc[comp_main,'phi_deg'] = (comp_inclcs.loc[comp_main,'phi_deg']-np.rad2deg(DBETA))%360 
         
         #updating slave components after updating main components, this makes a difference when splitting a component into more than two
-        for iR, CS_comps_row in CS_comps_formain.iterrows():
-            comp_slave = CS_comps_row['CS_comps_derive']
-            comp_inclCS.loc[comp_slave,'A'] = comp_inclCS.loc[comp_main,'A'] * CS_comps_row['CS_ampfacs']
-            comp_inclCS.loc[comp_slave,'phi_deg'] = (comp_inclCS.loc[comp_main,'phi_deg'] + CS_comps_row['CS_degincrs'])%360
+        for iR, cs_comps_row in cs_comps_formain.iterrows():
+            comp_slave = cs_comps_row['CS_comps_derive']
+            comp_inclcs.loc[comp_slave,'A'] = comp_inclcs.loc[comp_main,'A'] * cs_comps_row['CS_ampfacs']
+            comp_inclcs.loc[comp_slave,'phi_deg'] = (comp_inclcs.loc[comp_main,'phi_deg'] + cs_comps_row['CS_degincrs'])%360
             
-    return comp_inclCS
-
+    return comp_inclcs
 
-def prediction(comp, times_pred_all=None, times_ext=None, timestep_min=None, hatyan_settings=None, **kwargs):
-    """
-    generates a tidal prediction from a set of components A and phi values.
-    The component set has the same timezone as the timeseries used to create it, therefore the resulting prediction will also be in that original timezone.
-    
-    Parameters
-    ----------
-    comp : pandas.DataFrame
-        The DataFrame contains the component data with component names as index, and colums 'A' and 'phi_deg'.
-    times_pred_all : pandas.DatetimeIndex, optional
-        Prediction timeseries. The default is None.
-    times_ext : list of datetime.datetime, optional
-        Prediction time extents (list of start time and stop time). The default is None.
-    timestep_min : int, optional
-        Prediction timestep in minutes. The default is None.
-    hatyan_settings : hatyan.HatyanSettings()
-        Contains the used settings
-
-    Raises
-    ------
-    Exception
-        DESCRIPTION.
 
-    Returns
-    -------
-    ts_prediction_pd : pandas.DataFrame
-        The DataFrame should contain a 'values' column and a pd.DatetimeIndex as index, it contains the prediction times and values.
-    
-    """
-    
-    if hatyan_settings is None:
-        hatyan_settings = HatyanSettings(**kwargs)
-    elif len(kwargs)>0:
-        raise Exception('both arguments hatyan_settings and other settings (e.g. nodalfactors) are provided, this is not valid')
+def prediction_singleperiod(comp:pd.DataFrame, times:pd.DatetimeIndex, hatyan_settings) -> pd.DataFrame:
     
-    print('PREDICTION initializing')
-    print(hatyan_settings)
+    metadata_comp = metadata_from_obj(comp)
+    tzone_comp = metadata_comp.pop("tzone")
     
-    if times_pred_all is None:
-        if times_ext is None or timestep_min is None:
-            raise Exception('if argument times_pred_all is not provided, the arguments times_ext and timestep_min are obligatory')
-        else:
-            times_pred_all = robust_daterange_fromtimesextfreq(times_ext,timestep_min)
-    else:
-        if times_ext is not None or timestep_min is not None:
-            raise Exception('if argument times_pred_all is provided, the arguments times_ext and timestep_min are not allowed')
-    
-    if not len(times_pred_all) > 1:
-        raise Exception('ERROR: requested prediction period is not more than one timestep_min')
+    if not isinstance(times, pd.DatetimeIndex):
+        raise TypeError(f'times argument can be of type pd.DatetimeIndex or slice, not {type(times)}')
+    times_pred_all_pdDTI = times
     
-    if isinstance(times_pred_all, pd.core.indexes.datetimes.DatetimeIndex) or isinstance(times_pred_all, pd.core.indexes.base.Index): #TODO: this is probably not necessary, maybe only in case of Index (year 1600 compatibility)
-        times_pred_all_pdDTI = times_pred_all
-    else:
-        times_pred_all_pdDTI = pd.DatetimeIndex(times_pred_all)
+    # localize times datetimeindex, first convert times to tzone of components, then drop timezone
+    if times_pred_all_pdDTI.tz is not None:
+        times_pred_all_pdDTI = times_pred_all_pdDTI.tz_convert(tzone_comp)
+        times_pred_all_pdDTI = times_pred_all_pdDTI.tz_localize(None)
     
-    print('%-20s = %s'%('components used',len(comp)))
-    print('%-20s = %s'%('tstart',times_pred_all_pdDTI[0].strftime('%Y-%m-%d %H:%M:%S')))
-    print('%-20s = %s'%('tstop',times_pred_all_pdDTI[-1].strftime('%Y-%m-%d %H:%M:%S')))
+    message = (f'components used = {len(comp)}\n'
+               f'tstart = {times_pred_all_pdDTI[0].strftime("%Y-%m-%d %H:%M:%S")}\n'
+               f'tstop = {times_pred_all_pdDTI[-1].strftime("%Y-%m-%d %H:%M:%S")}')
     if hasattr(times_pred_all_pdDTI,'freq'):
-        print('%-20s = %s'%('timestep',times_pred_all_pdDTI.freq))
+        message += f'\ntimestep = {times_pred_all_pdDTI.freq}'
+    logger.info(message)
     
-    dood_date_mid = pd.Index([times_pred_all_pdDTI[len(times_pred_all_pdDTI)//2]]) #middle of analysis period (2july in case of 1jan-1jan), zoals bij hatyan.
-    dood_date_start = times_pred_all_pdDTI[:1] #first date (for v0, also freq?)
+    # middle of analysis period (2july in case of 1jan-1jan), zoals bij hatyan.
+    dood_date_mid = times_pred_all_pdDTI[[len(times_pred_all_pdDTI)//2]]
+    # first date (for v0, also freq?)
+    dood_date_start = times_pred_all_pdDTI[:1]
     
-    #sort component list and component dataframe
+    # sort component list and component dataframe
     if np.isnan(comp.values).any():
         raise Exception('provided component set contains nan values, prediction not possible')
     const_list = sort_const_list(comp.index.tolist())
     COMP = comp.loc[const_list]
     A = np.array(COMP['A'])
     phi_rad = np.array(np.deg2rad(COMP['phi_deg']))
 
-    t_const_freq_pd, v_0i_rad = get_freqv0_generic(hatyan_settings, const_list, dood_date_mid, dood_date_start)
+    t_const_freq_pd, v_0i_rad = get_freqv0_generic(const_list, dood_date_mid, dood_date_start, hatyan_settings.source)
     t_const_speed_all = t_const_freq_pd['freq'].values[:,np.newaxis]*(2*np.pi)
 
     if hatyan_settings.fu_alltimes:
         dood_date_fu = times_pred_all_pdDTI
     else:
         dood_date_fu = dood_date_mid
-    u_i_rad, f_i = get_uf_generic(hatyan_settings, const_list, dood_date_fu)
+    u_i_rad, f_i = get_uf_generic(const_list, dood_date_fu, hatyan_settings.nodalfactors, hatyan_settings.xfac, hatyan_settings.source)
 
-    print('PREDICTION started')
+    logger.info('PREDICTION started')
     omega_i_rads = t_const_speed_all.T/3600 #angular frequency, 2pi/T, in rad/s, https://en.wikipedia.org/wiki/Angular_frequency (2*np.pi)/(1/x*3600) = 2*np.pi*x/3600
     if not isinstance(times_pred_all_pdDTI,pd.DatetimeIndex): #support for years<1677, have to use Index instead of DatetimeIndex (DatetimeIndex is also Index, so isinstance(times_pred_all_pdDTI,pd.Index) does not work
         tdiff = pd.TimedeltaIndex(times_pred_all_pdDTI-dood_date_start) #pd.TimedeltaIndex is around it to avoid it being an Index in case of outofbounds timesteps (necessary from pandas 2.0.0)
     else:
         tdiff = pd.TimedeltaIndex(times_pred_all_pdDTI-dood_date_start[0]) #pd.TimedeltaIndex is not necessary here, but for conformity with above
     times_from0allpred_s_orig = tdiff.total_seconds().values
     times_from0allpred_s = np.transpose(times_from0allpred_s_orig[np.newaxis])
@@ -541,58 +469,105 @@
     f_A = np.multiply(f_i.values,A)
     omeg_t = np.multiply(times_from0allpred_s,omega_i_rads)
     v_u_phi = np.subtract(np.add(v_0i_rad.values,u_i_rad.values),phi_rad)
     omeg_t_v_u_phi = np.add(omeg_t,v_u_phi)
     ht_res = np.sum(np.multiply(f_A,np.cos(omeg_t_v_u_phi)),axis=1) #not necessary to add A0, since it is already part of the component list
     
     ts_prediction_pd = pd.DataFrame({'values': ht_res},index=times_pred_all_pdDTI)
-    print('PREDICTION finished')
+    logger.info('PREDICTION finished')
+    
+    # add timezone to timeseries again
+    ts_prediction_pd.index = ts_prediction_pd.index.tz_localize(tzone_comp)
     
     return ts_prediction_pd
 
 
-def prediction_peryear(comp_allyears, timestep_min, hatyan_settings=None, **kwargs):
-    raise Exception('ERROR: prediction_peryear() is deprecated, use prediction_perperiod() instead')
-
-
-def prediction_perperiod(comp_allperiods, timestep_min, hatyan_settings=None, **kwargs):
+@deprecated_python_option(**DEPRECATED_OPTIONS_PREDICTION_DICT)
+def prediction(comp, times=None, timestep=None):
     """
-    Wrapper around prediction(), to use component set of multiple years/months to generate multi-year/month timeseries.
+    generates a tidal prediction from a set of components A and phi values.
+    The component set has the same timezone as the timeseries used to create it, 
+    therefore the resulting prediction will also be in that original timezone.
+    If a components dataframe contains multiple column levels (multiple periods),
+    The prediction is a concatenation of predictions of all periods (based on the respective A/phi values).
 
     Parameters
     ----------
-    comp_allperiods : TYPE
-        DESCRIPTION.
-    timestep_min : TYPE
-        DESCRIPTION.
-    hatyan_settings : hatyan.HatyanSettings()
-        Contains the used settings
-        
+    comp : pd.DataFrame
+        The DataFrame contains the component data with component names as index, and colums 'A' and 'phi_deg'.
+    times : (pd.DatetimeIndex,slice), optional
+        pd.DatetimeIndex with prediction timeseries or slice(tstart,stop,timestep) to construct it from. 
+        If None, pd.DatetimeIndex is constructed from the tstart/tstop/timestep metadata attrs of the comp object. 
+        Only allowed/relevant for component dataframes with single-level columns (single period). The default is None.
+    timestep : str
+        Only allowed/relevant for component dataframes with multi-level columns (different periods). 
+        The string is parsed with pandas.tseries.frequencies.to_offset(). The default is None.
+
     Returns
     -------
-    ts_prediction_peryear : TYPE
-        DESCRIPTION.
+    ts_prediction : TYPE
+        The DataFrame contains a 'values' column and a pd.DatetimeIndex as index, it contains the prediction times and values.
 
     """
     
-    if hatyan_settings is None:
-        hatyan_settings = HatyanSettings(**kwargs)
-    elif len(kwargs)>0:
-        raise Exception('both arguments hatyan_settings and other settings (e.g. nodalfactors) are provided, this is not valid')
-
-    ts_periods_dt = comp_allperiods.columns.levels[1]
-    ts_periods_strlist = [str(x) for x in ts_periods_dt]
-    
-    ts_prediction_perperiod = pd.DataFrame()
-    for period_dt in ts_periods_dt:
-        print(f'generating prediction {period_dt} of sequence {ts_periods_strlist}')
-        comp_oneyear = comp_allperiods.loc[:,(slice(None),period_dt)]
-        comp_oneyear.columns = comp_oneyear.columns.droplevel(1)
-        if period_dt.freqstr in ['A-DEC']: #year frequency
-            times_ext = [dt.datetime(period_dt.year,1,1),dt.datetime(period_dt.year+1,1,1)-dt.timedelta(minutes=timestep_min)]
-        elif period_dt.freqstr in ['M']: #month frequency
-            times_ext = [period_dt.to_timestamp().to_pydatetime(),period_dt.to_timestamp().to_pydatetime()+dt.timedelta(days=period_dt.days_in_month)-dt.timedelta(minutes=timestep_min)]
-        else:
-            raise Exception(f'unknown freqstr: {period_dt.freqstr}')
-        ts_prediction_oneperiod = prediction(comp=comp_oneyear,times_ext=times_ext, timestep_min=timestep_min, hatyan_settings=hatyan_settings)
-        ts_prediction_perperiod = pd.concat([ts_prediction_perperiod,ts_prediction_oneperiod])
-    return ts_prediction_perperiod
+    # get settings from component attribute and validate their values
+    settings_kwargs = {}
+    for setting in ['nodalfactors', 'xfac', 'fu_alltimes', 'source']:
+        settings_kwargs[setting] = comp.attrs[setting]
+    hatyan_settings = HatyanSettings(**settings_kwargs)
+    
+    logger.info(f'PREDICTION initializing\n{hatyan_settings}')
+    
+    if hasattr(comp.columns,"levels"):
+        logger.info('prediction() per period due to levels in component dataframe columns')
+        if timestep is None:
+            raise TypeError("prediction() per period, so 'timestep' argument should not be None")
+        if times is not None:
+            raise TypeError("prediction() per period, so 'times' argument not allowed")
+        # convert timestep to tstep of proper type
+        tstep = pd.tseries.frequencies.to_offset(timestep)
+        
+        ts_periods_dt = comp.columns.levels[1]
+        ts_periods_strlist = [str(x) for x in ts_periods_dt]
+        
+        ts_prediction_perperiod_list = []
+        for period_dt in ts_periods_dt:
+            logger.info(f'generating prediction {period_dt} of sequence {ts_periods_strlist}')
+            comp_oneyear = comp.loc[:,(slice(None),period_dt)]
+            comp_oneyear.columns = comp_oneyear.columns.droplevel(1)
+            if period_dt.freqstr in ['A-DEC','Y-DEC']: #year frequency
+                tstart = pd.Timestamp(period_dt.year,1,1)
+                tstop = pd.Timestamp(period_dt.year+1,1,1) - pd.Timedelta(tstep)
+            elif period_dt.freqstr in ['M']: #month frequency
+                tstart = period_dt.to_timestamp()
+                tstop = period_dt.to_timestamp() + pd.Timedelta(days=period_dt.days_in_month) - pd.Timedelta(tstep)
+            else:
+                raise Exception(f'unknown freqstr: {period_dt.freqstr}')
+            # generate date range and do prediction
+            times_pred = pd.date_range(start=tstart, end=tstop, freq=tstep, unit="us")
+            ts_prediction_oneperiod = prediction_singleperiod(comp=comp_oneyear, times=times_pred, hatyan_settings=hatyan_settings)
+            ts_prediction_perperiod_list.append(ts_prediction_oneperiod)
+        ts_prediction = pd.concat(ts_prediction_perperiod_list)
+    else:
+        logger.info('prediction() atonce')
+        if timestep is not None:
+            raise TypeError("prediction() atonce, so 'timestep' argument not allowed")
+        if times is None:
+            raise TypeError("prediction() atonce, so 'times' argument should not be None")
+        if isinstance(times,slice):
+            tstart = pd.Timestamp(times.start)
+            tstop = pd.Timestamp(times.stop)
+            tstep = pd.tseries.frequencies.to_offset(times.step)
+            times = pd.date_range(start=tstart, end=tstop, freq=tstep, unit="us")
+        ts_prediction = prediction_singleperiod(comp=comp, times=times, hatyan_settings=hatyan_settings)
+    
+    # add metadata (and update grootheid)
+    metadata_comp = metadata_from_obj(comp)
+    if 'grootheid' in metadata_comp:
+        # update metadata
+        if metadata_comp['grootheid'] == 'WATHTE':
+            metadata_comp['grootheid'] = 'WATHTBRKD'
+    if 'tzone' in metadata_comp.keys():
+        metadata_comp.pop('tzone')
+    ts_prediction = metadata_add_to_obj(ts_prediction, metadata_comp)
+
+    return ts_prediction
```

### Comparing `hatyan-2.7.0/hatyan/astrog.py` & `hatyan-2.8.0/hatyan/astrog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 # -*- coding: utf-8 -*-
 """
 astrog.py contains all astro-related definitions, previously embedded in a separate program but now part of hatyan.
-
-hatyan is a Python program for tidal analysis and prediction, based on the FORTRAN version. 
-Copyright (C) 2019-2021 Rijkswaterstaat.  Maintained by Deltares, contact: Jelmer Veenstra (jelmer.veenstra@deltares.nl). 
-Source code available at: https://github.com/Deltares/hatyan
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Lesser General Public License for more details.
-
-You should have received a copy of the GNU Lesser General Public License
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
 """
 
 import os
 import functools
 import pandas as pd
 import numpy as np
 import datetime as dt
 import requests
 import warnings
 import matplotlib.pyplot as plt
+import logging
 
 from hatyan.schureman import get_schureman_freqs
-    
 
+__all__ = ["astrog_culminations",
+           "astrog_phases",
+           "astrog_sunriseset",           
+           "astrog_moonriseset",
+           "astrog_anomalies",
+           "astrog_seasons",
+           "convert2perday",
+           "plot_astrog_diff",
+           ]
+
+
+logger = logging.getLogger(__name__)
 file_path = os.path.realpath(__file__)
 
 
 def astrog_culminations(tFirst,tLast,dT_fortran=False,tzone='UTC'): #TODO: add simple lon correction at end of definition, currenty calculating culmination at lon=0
     """
     Makes use of the definitions dT, astrab and astrac.
     Calculates lunar culminations, parallax and declination. By default the lunar culmination is calculated at coordinates lon=0 (Greenwich), since EHMOON is used to calculate it. Possible to add lon-correction at end of definition.
@@ -71,22 +65,23 @@
     tFirst,tLast = convert_str2datetime(tFirst,tLast)
     
     # constants
     EHMINC       = 346.8 # increment of ephemeris hour angle of moon (deg/day)
     M2_period_hr = get_schureman_freqs(['M2']).loc['M2','period [hr]'] # interval between lunar culminations (hours)
     
     # first and last datetime in calculation (add enough margin, and an extra day for timezone differences)
-    date_first = tFirst-dt.timedelta(hours=M2_period_hr+1*24)
-    date_last = tLast+dt.timedelta(hours=M2_period_hr+1*24)
+    date_first = tFirst - pd.Timedelta(hours=M2_period_hr+1*24)
+    date_last = tLast + pd.Timedelta(hours=M2_period_hr+1*24)
 
     # estimate culminations (time and type)
     astrabOutput = astrab(date_first,dT_fortran=dT_fortran)
     EHMOON = astrabOutput['EHMOON']
     ICUL = np.floor(EHMOON[0]%360/180).astype(int)+1 # ICUL=1: next culmination is lower culmination, ICUL=2: next culmination is upper culmination
-    CULEST = pd.date_range(start=date_first+dt.timedelta(days=(180.*ICUL-EHMOON[0])/EHMINC), end=date_last, freq='%iN'%(M2_period_hr*3600*1e9)) #defined freq as M2_period in nanoseconds
+    date_start = date_first + pd.Timedelta(days=(180.*ICUL-EHMOON[0])/EHMINC)
+    CULEST = pd.date_range(start=date_start, end=date_last, freq='%ins'%(M2_period_hr*3600*1e9)) #defined freq as M2_period in nanoseconds
     CULTYP = np.zeros(len(CULEST),dtype=int)
     CULTYP[::2] = ICUL
     CULTYP[1::2] = (ICUL%2)+1
     
     # calculate exact time of culminations
     CULTIM = astrac(CULEST, dT_fortran=dT_fortran, mode=CULTYP) #TODO: no correction with dT necessary?
     astrabOutput = astrab(CULTIM, dT_fortran=dT_fortran)
@@ -136,37 +131,37 @@
     tFirst,tLast = convert_str2datetime(tFirst,tLast)
         
     # constants
     ELOINC = 12.2           # increment of ELONG ecliptic elongation of moon-sun (deg/day)
     FASINT = 29.530587981/4 # quarter of a lunar synodic month (days)
 
     # first and last datetime in calculation (add enough margin (done later), and an extra day for timezone differences)
-    date_first = tFirst-dt.timedelta(days=FASINT+1)
-    date_last = tLast+dt.timedelta(days=FASINT+1)
+    date_first = tFirst - pd.Timedelta(days=FASINT+1)
+    date_last = tLast + pd.Timedelta(days=FASINT+1)
 
     # estimate first lunar phase (time and type), correct first date (FAEST_first to 45 deg from there)
     astrabOutput = astrab(date_first,dT_fortran=dT_fortran)
     ELONG = astrabOutput['ELONG']
-    FAEST_first = date_first - pd.TimedeltaIndex((ELONG-45)/ELOINC, unit='D')
+    FAEST_first = date_first - pd.to_timedelta((ELONG-45)/ELOINC, unit='D')
 
     # use the first date to create a new daterange from the correct starting time. The frequency is 29 days, 12 hours and 44 minutes, following from dood_S-dood_H
-    date = pd.date_range(start=FAEST_first[0],end=date_last,freq='%iN'%(FASINT*24*3600*1e9))
+    date = pd.date_range(start=FAEST_first[0],end=date_last,freq='%ins'%(FASINT*24*3600*1e9))
 
     # estimate all lunar phases (time and type)
     astrabOutput = astrab(date,dT_fortran=dT_fortran)
     ELONG = astrabOutput['ELONG']
     FATYP = (np.floor(ELONG/90).astype(int)+3)%4+1 #make sure the next phase is searched for (modulus to use 'FATYP-1')
-    FAEST = date - pd.TimedeltaIndex((90*FATYP-ELONG%360)/ELOINC, unit='D')
+    FAEST = date - pd.to_timedelta((90*FATYP-ELONG%360)/ELOINC, unit='D')
 
     # calculate exact time of phase, loop until date_last
-    TIMDIF = pd.TimedeltaIndex(-dT(FAEST,dT_fortran=dT_fortran),unit='S')
+    TIMDIF = pd.to_timedelta(-dT(FAEST,dT_fortran=dT_fortran),unit='s')
     FATIM = astrac(FAEST,dT_fortran=dT_fortran,mode=FATYP+2) + TIMDIF
 
     # make dataframe
-    astrog_df = pd.DataFrame({'datetime':FATIM.round('S'),'type':FATYP})
+    astrog_df = pd.DataFrame({'datetime':FATIM.round('s'),'type':FATYP})
     astrog_df['type_str'] = astrog_df['type'].astype(str).replace('1','FQ').replace('2','FM').replace('3','LQ').replace('4','NM')
 
     #set timezone, check datetime order and filter datetimerange
     astrog_df = check_crop_dataframe(astrog_df, tFirst, tLast, tzone)
 
     return astrog_df
 
@@ -204,30 +199,30 @@
 
     """
 
     # check input times (datetime or string)
     tFirst,tLast = convert_str2datetime(tFirst,tLast)
 
     # first and last datetime in calculation (add enough margin, and an extra day for timezone differences)
-    date_first = tFirst - dt.timedelta(days=1)
-    date_last = tLast + dt.timedelta(days=1)
+    date_first = tFirst - pd.Timedelta(days=1)
+    date_last = tLast + pd.Timedelta(days=1)
     
     # --- sunrise and -set ---
     # estimate times: starting at tFirst, 0h local solar time
-    DAYEST = pd.date_range(start=date_first,end=date_last,freq='%iN'%(24*3600*1e9))
-    OPEST  = DAYEST + dt.timedelta(days=-lon/360.+.25) # correct for longitude and 'floor' date to 00:00 +6h
-    ONEST  = DAYEST + dt.timedelta(days=-lon/360.+.75) # correct for longitude and 'floor' date to 00:00 +18h
+    DAYEST = pd.date_range(start=date_first,end=date_last,freq='%ins'%(24*3600*1e9))
+    OPEST  = DAYEST + pd.Timedelta(days=-lon/360.+.25) # correct for longitude and 'floor' date to 00:00 +6h
+    ONEST  = DAYEST + pd.Timedelta(days=-lon/360.+.75) # correct for longitude and 'floor' date to 00:00 +18h
 
     # calculate exact times
-    TIMDIF = pd.TimedeltaIndex(-dT(OPEST,dT_fortran=dT_fortran),unit='S')
+    TIMDIF = pd.to_timedelta(-dT(OPEST,dT_fortran=dT_fortran),unit='s')
     OPTIM  = astrac(OPEST,dT_fortran=dT_fortran,mode=np.array(9),lon=lon,lat=lat) + TIMDIF
     ONTIM  = astrac(ONEST,dT_fortran=dT_fortran,mode=np.array(10),lon=lon,lat=lat) + TIMDIF
 
     # make dataframe
-    astrog_df = pd.DataFrame({'datetime':np.concatenate((OPTIM.round('S'),ONTIM.round('S'))),'type':np.repeat([1,2],len(OPTIM))})
+    astrog_df = pd.DataFrame({'datetime':np.concatenate((OPTIM.round('s'),ONTIM.round('s'))),'type':np.repeat([1,2],len(OPTIM))})
     astrog_df = astrog_df.sort_values('datetime').reset_index(drop=True)
     astrog_df['type_str'] = astrog_df['type'].astype(str).replace('1','sunrise').replace('2','sunset')
 
     #set timezone, check datetime order and filter datetimerange
     astrog_df = check_crop_dataframe(astrog_df, tFirst, tLast, tzone)
     
     return astrog_df
@@ -271,37 +266,37 @@
 
     # constants
     from hatyan.schureman import get_schureman_freqs
     M2_period_hr = get_schureman_freqs(['M2']).loc['M2','period [hr]'] # CULINT
     EHMINC = 346.8 # increment of EHMOON ephemeris hour angle of moon (deg/day) TODO: 360/(M2_period_hr*2/24) = 347.8092506037627
 
     # first and last datetime in calculation (add enough margin, and an extra day for timezone differences)
-    date_first = tFirst-dt.timedelta(hours=M2_period_hr+1*24)
-    date_last = tLast+dt.timedelta(hours=M2_period_hr+1*24)
+    date_first = tFirst - pd.Timedelta(hours=M2_period_hr+1*24)
+    date_last = tLast + pd.Timedelta(hours=M2_period_hr+1*24)
 
     # --- moonrise and -set ---
     # estimate times
     astrabOutput = astrab(date_first,dT_fortran=dT_fortran,lon=lon,lat=lat)
     ALTMOO = astrabOutput['ALTMOO']
     EHMOON = astrabOutput['EHMOON']
 
     if ALTMOO < -(0.5667+(0.08+0.2725*astrabOutput['PARLAX'])/3600): # first phenomenon is moonrise #the PARLAX output is in arcseconds, so /3600 is conversion to degrees
-        OPEST = pd.date_range(start=date_first+dt.timedelta(days=(270-EHMOON[0])/EHMINC), end=date_last, freq='%iN'%(M2_period_hr*2*3600*1e9))
-        ONEST = OPEST + dt.timedelta(hours=M2_period_hr)
+        date_first_plus = date_first + pd.Timedelta(days=(270-EHMOON[0])/EHMINC)
     else: # first phenomenon is moonset
-        ONEST = pd.date_range(start=date_first+dt.timedelta(days=(90-EHMOON[0])/EHMINC), end=date_last, freq='%iN'%(M2_period_hr*2*3600*1e9))
-        OPEST = ONEST + dt.timedelta(hours=M2_period_hr)
+        date_first_plus = date_first + pd.Timedelta(days=(90-EHMOON[0])/EHMINC)
+    ONEST = pd.date_range(start=date_first_plus, end=date_last, freq='%ins'%(M2_period_hr*2*3600*1e9))
+    OPEST = ONEST + pd.Timedelta(hours=M2_period_hr)
 
     # calculate exact times
-    TIMDIF = pd.TimedeltaIndex(-dT(OPEST,dT_fortran=dT_fortran),unit='S')
+    TIMDIF = pd.to_timedelta(-dT(OPEST,dT_fortran=dT_fortran),unit='s')
     OPTIM  = astrac(OPEST,dT_fortran=dT_fortran,mode=np.array(7),lon=lon,lat=lat) + TIMDIF
     ONTIM  = astrac(ONEST,dT_fortran=dT_fortran,mode=np.array(8),lon=lon,lat=lat) + TIMDIF
 
     # make dataframe
-    astrog_df = pd.DataFrame({'datetime':np.concatenate((OPTIM.round('S'),ONTIM.round('S'))),'type':np.repeat([1,2],len(OPTIM))})
+    astrog_df = pd.DataFrame({'datetime':np.concatenate((OPTIM.round('s'),ONTIM.round('s'))),'type':np.repeat([1,2],len(OPTIM))})
     astrog_df = pd.DataFrame(astrog_df).sort_values('datetime').reset_index(drop=True)
     astrog_df['type_str'] = astrog_df['type'].astype(str).replace('1','moonrise').replace('2','moonset')
 
     #set timezone, check datetime order and filter datetimerange
     astrog_df = check_crop_dataframe(astrog_df, tFirst, tLast, tzone)
 
     return astrog_df
@@ -340,38 +335,39 @@
     tFirst,tLast = convert_str2datetime(tFirst,tLast)
 
     # constants
     ANMINC = 13.06       # increment of ANM anomaly of moon (deg/day)
     ANOINT = 27.554551/2 # half of a lunar anomalistic month (days)
 
     # first and last datetime in calculation (add enough margin, and an extra day for timezone differences)
-    date_first = tFirst-dt.timedelta(days=ANOINT+1)
-    date_last = tLast+dt.timedelta(days=ANOINT+1)
+    date_first = tFirst - pd.Timedelta(days=ANOINT+1)
+    date_last = tLast + pd.Timedelta(days=ANOINT+1)
 
     # estimate first lunar anomaly (time and type)
     astrabOutput = astrab(date_first,dT_fortran=dT_fortran)
     DPAXDT = astrabOutput['DPAXDT']
     ANM = astrabOutput['ANM']
     if DPAXDT>0: # ANOTYP=1: perigeum first
         ref_deg = 360    
         IANO = 1
     elif DPAXDT<=0: # ANOTYP=2: apogeum first
         ref_deg = 180    
         IANO = 2
-    ANOEST = pd.date_range(start=date_first+dt.timedelta(days=(ref_deg-ANM[0])/ANMINC),end=date_last,freq='%iN'%(ANOINT*24*3600*1e9))
+    date_first_plus = date_first + pd.Timedelta(days=(ref_deg-ANM[0])/ANMINC)
+    ANOEST = pd.date_range(start=date_first_plus,end=date_last,freq='%ins'%(ANOINT*24*3600*1e9))
     ANOTYP = np.zeros(len(ANOEST),dtype=int)
     ANOTYP[::2] = IANO
     ANOTYP[1::2] = (IANO%2)+1
 
     # calculate exact times
-    TIMDIF = pd.TimedeltaIndex(-dT(ANOEST,dT_fortran=dT_fortran),unit='S')
+    TIMDIF = pd.to_timedelta(-dT(ANOEST,dT_fortran=dT_fortran),unit='s')
     ANOTIM = astrac(ANOEST,dT_fortran=dT_fortran,mode=ANOTYP+14) + TIMDIF
 
     # make dataframe
-    astrog_df = pd.DataFrame({'datetime':ANOTIM.round('S'),'type':ANOTYP})
+    astrog_df = pd.DataFrame({'datetime':ANOTIM.round('s'),'type':ANOTYP})
     astrog_df['type_str'] = astrog_df['type'].astype(str).replace('1','perigeum').replace('2','apogeum')
 
     #set timezone, check datetime order and filter datetimerange
     astrog_df = check_crop_dataframe(astrog_df, tFirst, tLast, tzone)
     
     return astrog_df
 
@@ -405,23 +401,25 @@
 
     """
 
     # check input times (datetime or string)
     tFirst,tLast = convert_str2datetime(tFirst,tLast)
 
     # estimate start of seasons (time and type)
-    SEIEST = pd.date_range(start=dt.datetime(tFirst.year,int(np.ceil(tFirst.month/3)*3),1),end=tLast+dt.timedelta(days=1),freq='%iMS'%(3))+dt.timedelta(days=20)
+    date_start = dt.datetime(tFirst.year,int(np.ceil(tFirst.month/3)*3),1)
+    date_end = tLast + pd.Timedelta(days=1)
+    SEIEST = pd.date_range(start=date_start, end=date_end, freq='3MS') + pd.Timedelta(days=20)
     SEITYP = np.floor(SEIEST.month/3).astype(int)
 
     # calculate exact times, loop until tLast
-    TIMDIF = pd.TimedeltaIndex(-dT(SEIEST,dT_fortran=dT_fortran),unit='S')
+    TIMDIF = pd.to_timedelta(-dT(SEIEST,dT_fortran=dT_fortran),unit='s')
     SEITIM = astrac(SEIEST,dT_fortran=dT_fortran,mode=SEITYP+10) + TIMDIF
 
     # make dataframe
-    astrog_df = pd.DataFrame({'datetime':SEITIM.round('S'),'type':SEITYP})
+    astrog_df = pd.DataFrame({'datetime':SEITIM.round('s'),'type':SEITYP})
     astrog_df['type_str'] = astrog_df['type'].astype(str).replace('1','spring').replace('2','summer').replace('3','autumn').replace('4','winter')
     
     #set timezone, check datetime order and filter datetimerange
     astrog_df = check_crop_dataframe(astrog_df, tFirst, tLast, tzone)
     
     return astrog_df
 
@@ -807,16 +805,17 @@
     PNEW = astrabOutput[IPAR]
     # iterate until criterium is reached or max 20 times (including catch for sunrise and moonrise)
     while (abs(ANG-PNEW) > CRIT).any():# and ITER <=20:
         TOLD = TNEW.copy()
         POLD = PNEW.copy()
         if IPAR=='ALTMOO': # correction for semidiameter moon #TODO, might not be necessary to put in loop since PARLAX is not that variable over iterations
             ANG = itertargets_pd.loc[mode,'ANGLE']-(0.08+0.2725*astrabOutput['PARLAX'])/3600. # ANGLE in degrees and PARLAX in arcseconds (/3600 gives degrees)
-        addtime = pd.TimedeltaIndex(np.nan_to_num((ANG-POLD)/RATE,0),unit='D') #nan_to_num to make sure no NaT output in next iteration
-        #print(f'{ITER} timediff in hours:\n%s'%(np.array(addtime.total_seconds()/3600).round(2)))
+        # nan_to_num to make sure no NaT/inf output in next iteration
+        addtime_nonan = np.nan_to_num((ANG-POLD)/RATE, nan=0, posinf=0, neginf=0)
+        addtime = pd.to_timedelta(addtime_nonan, unit='D')
         if IPAR in ['ALTMOO','ALTSUN'] and (np.abs(np.array(addtime.total_seconds()/3600)) > 24).any(): #catch for ALTMOO and ALTSUN to let the iteration process stop before it escalates
             raise Exception(f'Iteration step resulted in time changes larger than 24 hours (max {np.abs(addtime.total_seconds()).max()/3600:.2f} hours), try using a lower latitude')
         TNEW = TOLD + addtime
         ITER = ITER+1
         astrabOutput = astrab(TNEW,dT_fortran=dT_fortran,lon=lon,lat=lat)
         PNEW = astrabOutput[IPAR]
         RATE = np.array((PNEW-POLD)/((TNEW-TOLD).total_seconds()/86400))
@@ -855,30 +854,30 @@
     try:
         resp = requests.get(url_leap_seconds_list)
         if resp.status_code==404:
             resp.raise_for_status()
         with open(file_leap_seconds_list, 'wb') as f:
             f.write(resp.content)
     except requests.HTTPError as e: #catch raised 404 error
-        print(f'WARNING: leap-seconds.list not retrieved, using local copy. Error message: "{e}"')
+        logger.warning(f'WARNING: leap-seconds.list not retrieved, using local copy. Error message: "{e}"')
     except (FileNotFoundError, PermissionError) as e: #catch problems with writing to file
-        print(f'WARNING: leap-seconds.list not written, using local copy. Error message: "{e}"')
+        logger.warning(f'leap-seconds.list not written, using local copy. Error message: "{e}"')
         
     #get expiry date from file
     with open(file_leap_seconds_list) as f:
         resp_pd_all = pd.Series(f.readlines())
     expirydate_linestart = '#@'
     expirydate_line = resp_pd_all.loc[resp_pd_all.str.startswith(expirydate_linestart)]
     if len(expirydate_line) != 1:
         raise Exception('less or more than 1 expirydate line found with "{expirydate_linestart}": {expirydate_line}')
-    expirydate = refdate + dt.timedelta(seconds=int(expirydate_line.iloc[0].split()[1]))
+    expirydate = refdate + pd.Timedelta(seconds=int(expirydate_line.iloc[0].split()[1]))
     
     #get leapsecond list from file
-    resp_pd = pd.read_csv(file_leap_seconds_list,comment='#',names=['seconds_since_19000101','leap_seconds'],delim_whitespace=True)
-    resp_pd['datetime'] = refdate + pd.to_timedelta(resp_pd['seconds_since_19000101'],unit='S')
+    resp_pd = pd.read_csv(file_leap_seconds_list, comment='#', names=['seconds_since_19000101','leap_seconds'], sep="\\s+")
+    resp_pd['datetime'] = refdate + pd.to_timedelta(resp_pd['seconds_since_19000101'],unit='s')
     resp_pd['datetime_str'] = resp_pd['datetime'].dt.strftime('%Y-%m-%d')
     leap_seconds_pd = resp_pd.set_index('datetime_str')
     
     return leap_seconds_pd, expirydate
 
 
 def dT(dateIn,dT_fortran=False):
@@ -889,15 +888,16 @@
     Uses the international definition unless dT_fortran=True. 
     
     Parameters
     ----------
     dateIn : datetime.datetime or pandas.DatetimeIndex
         Date for correction. Definition makes use of provided year.
     dT_fortran : boolean, optional
-        When True, use latest fortran dT and increment value instead of default international definition. The default is False.
+        If True, use latest fortran dT and increment value, which is not accurate for years that are far away from 2012. 
+        Use the default dT_fortran=False to use the automatically updated list of leap-seconds instead. The default is False.
     Raises
     ------
     Warning
         Checks if hard-coded values can still be used.
 
     Returns
     -------
@@ -908,27 +908,26 @@
     
     if isinstance(dateIn, dt.datetime):
         dateIn = pd.DatetimeIndex([dateIn])
     elif not isinstance(dateIn, pd.DatetimeIndex):
         raise Exception('Input variable date should be datetime or pd.DateTimeIndex')
     
     if dT_fortran: # reproduce fortran dT_TT values with latest dT and increment values from fortran code
-        warnings.warn('WARNING: If dT_fortran=True, the last values for dT and its increment are used from the fortran code, this is not accurate for years that are far away from 2012. Use dT_fortran=False since the default approach uses an automatically updated list of leap-seconds instead')
         # historical hard-coded values (taken from FORTRAN comments) from Astronomical Almanac - Reduction of time scales (only last ones are used to reproduce fortran code)
         dT_TTyear     = [ 1980,  1993,  2002,  2012 ] # year of used dT_TTval value
         dT_TTval      = [50.97, 59.35, 64.90, 67.184] # difference between TT and UT1 (32.184s + leap seconds)
         dT_TTinc      = [0.998,  0.70,  0.42,  0.676] # yearly increment of dT curve: (dT_last-dT_5yBefore)/5
         
         # approximation of dT in requested year (dT = TT-UT1)
         dT_TT = (dT_TTval[-1]+dT_TTinc[-1]*(np.array(dateIn.year)-dT_TTyear[-1]))#/86400 
 
     else: #use most exact approximation
         # get list with leap seconds
         if (dateIn<dt.datetime(1972,1,1)).any():
-            warnings.warn('WARNING: The current definition of the relationship between UTC and TAI dates from 1 January 1972. This first dT value is also applied before that date even though this might not be accurate.')
+            warnings.warn(UserWarning('The current definition of the relationship between UTC and TAI dates from 1 January 1972. This first dT value is also applied before that date even though this might not be accurate.'))
         leap_seconds_pd, expirydate = get_leapsecondslist_fromurlorfile()
 
         NTP_date = leap_seconds_pd['datetime'].values#tolist()
         leap_sec = leap_seconds_pd['leap_seconds'].values#.tolist()
         #import matplotlib.pyplot as plt
         #fig,ax=plt.subplots()
         #ax.plot(leap_seconds_pd['datetime'], leap_seconds_pd['leap_seconds'])
@@ -1021,15 +1020,15 @@
     dataframeOut.drop(['type','type_str'],axis='columns',inplace=True)
     dataframeOut = dataframeOut[~dataframeOut.index.duplicated(keep='first')]
     dataframeOut['datetime'] = dataframeOut.index #overwrite datetime with dates
     
     return dataframeOut
 
 
-def plot_astrog_diff(pd_python, pd_fortran, typeUnit='-', typeLab=None, typeBand=None, timeBand=None):
+def plot_astrog_diff(pd_python, pd_fortran, typeCol="type", typeUnit='-', typeLab=None, typeBand=None, timeBand=None):
     """
     Plots results of FORTRAN and python verison of astrog for visual inspection.
     Top plot shows values or type, middle plot shows time difference, bottom plot shows value/type difference.
 
     Parameters
     ----------
     pd_python : pandas DataFrame
@@ -1056,40 +1055,43 @@
 
     """
     
     if hasattr(pd_python['datetime'].dtype,'tz'):
         pd_python = pd_python.copy() #do not overwrite original dataframe, so make a copy
         pd_python['datetime'] = pd_python['datetime'].dt.tz_localize(None) #Passing None will remove the time zone information preserving local time. https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Series.dt.tz_localize.html#pandas.Series.dt.tz_localize
     
-    typeName = pd_python.columns[1]
+    # reset index
+    pd_python = pd_python.reset_index(drop=True)
+    pd_fortran = pd_fortran.reset_index(drop=True)
+    
     fig, (ax1,ax2,ax3) = plt.subplots(3,1,figsize=(15,9),sharex=True)
-    ax1.set_title('%s'%(typeName))
-    ax1.plot(pd_python['datetime'], pd_python[typeName], label='python')
-    ax1.plot(pd_fortran['datetime'],pd_fortran[typeName],label='FORTRAN',linestyle='dashed')
-    if typeName == 'type':
+    ax1.set_title('%s'%(typeCol))
+    ax1.plot(pd_python['datetime'], pd_python[typeCol], label='python')
+    ax1.plot(pd_fortran['datetime'],pd_fortran[typeCol],label='FORTRAN',linestyle='dashed')
+    if typeCol == 'type':
         if typeLab is not None:
             ax1.set_ylim(1,len(typeLab))
             ax1.set_yticks(np.arange(1,len(typeLab)+1,step=1))
             ax1.set_yticklabels(typeLab)
-    ax1.set_ylabel('%s [%s]'%(typeName, typeUnit))
+    ax1.set_ylabel('%s [%s]'%(typeCol, typeUnit))
     ax1.legend(loc=1)
 
     ax2.plot(pd_python['datetime'],(pd_python['datetime'] - pd.to_datetime(pd_fortran['datetime'])).dt.total_seconds())
     if timeBand is not None:
         ax2.plot(pd_python['datetime'].iloc[[0,-1]],[timeBand[0],timeBand[0]],color='k',linestyle='dashed')
         ax2.plot(pd_python['datetime'].iloc[[0,-1]],[timeBand[1],timeBand[1]],color='k',linestyle='dashed')
     ax2.set_ylabel('python - FORTRAN [seconds]')
     ax2.set_title('time difference [seconds]')
 
-    ax3.plot(pd_python['datetime'],pd_python[typeName] - pd_fortran[typeName])
+    ax3.plot(pd_python['datetime'],pd_python[typeCol] - pd_fortran[typeCol])
     if typeBand is not None:
         ax3.plot(pd_python['datetime'].iloc[[0,-1]],[typeBand[0],typeBand[0]],color='k',linestyle='dashed')
         ax3.plot(pd_python['datetime'].iloc[[0,-1]],[typeBand[1],typeBand[1]],color='k',linestyle='dashed')
     ax3.set_ylabel('python - FORTRAN [%s]'%(typeUnit))
-    ax3.set_title('%s difference [%s]'%(typeName, typeUnit))
+    ax3.set_title('%s difference [%s]'%(typeCol, typeUnit))
 
     ax1.set_xlim(pd_python['datetime'].iloc[[0,-1]])
     fig.tight_layout()
 
     axs = (ax1,ax2,ax3)
     return fig, axs
```

### Comparing `hatyan-2.7.0/hatyan/data/data_M2phasediff_perstation.txt` & `hatyan-2.8.0/hatyan/data/data_M2phasediff_perstation.txt`

 * *Files identical despite different names*

### Comparing `hatyan-2.7.0/hatyan/data/data_foreman_frequencies.txt` & `hatyan-2.8.0/hatyan/data/data_foreman_frequencies.txt`

 * *Files identical despite different names*

### Comparing `hatyan-2.7.0/hatyan/data/data_foreman_harmonic.txt` & `hatyan-2.8.0/hatyan/data/data_foreman_harmonic.txt`

 * *Files identical despite different names*

### Comparing `hatyan-2.7.0/hatyan/data/data_foreman_shallowrelations.txt` & `hatyan-2.8.0/hatyan/data/data_foreman_shallowrelations.txt`

 * *Files identical despite different names*

### Comparing `hatyan-2.7.0/hatyan/data/data_schureman_harmonic.csv` & `hatyan-2.8.0/hatyan/data/data_schureman_harmonic.csv`

 * *Files identical despite different names*

### Comparing `hatyan-2.7.0/hatyan/data/data_schureman_shallowrelations.csv` & `hatyan-2.8.0/hatyan/data/data_schureman_shallowrelations.csv`

 * *Files identical despite different names*

### Comparing `hatyan-2.7.0/hatyan/foreman.py` & `hatyan-2.8.0/hatyan/foreman.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,10 @@
 # -*- coding: utf-8 -*-
 """
 foreman.py contains all foreman definitions now embedded in hatyan. The dataset is derived from "M.G.G. Foreman (2004), Manual for Tidal Heights Analysis and Prediction, Institute of Ocean Sciences (Patricia Bay, Sidney B.C. Canada)"
-
-hatyan is a Python program for tidal analysis and prediction, based on the FORTRAN version. 
-Copyright (C) 2019-2021 Rijkswaterstaat.  Maintained by Deltares, contact: Jelmer Veenstra (jelmer.veenstra@deltares.nl). 
-Source code available at: https://github.com/Deltares/hatyan
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Lesser General Public License for more details.
-
-You should have received a copy of the GNU Lesser General Public License
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
 """
 
 import os
 import pandas as pd
 import numpy as np
 import functools
 import datetime as dt
@@ -57,15 +39,15 @@
         DESCRIPTION.
     foreman_harmonic_nodal : TYPE
         DESCRIPTION.
 
     """
     
     foreman_file = os.path.join(os.path.dirname(file_path),'data','data_foreman_harmonic.txt')
-    foreman_harmonic_raw = pd.read_csv(foreman_file, comment='#', names=range(16), index_col=0, skip_blank_lines=True, delim_whitespace=True)
+    foreman_harmonic_raw = pd.read_csv(foreman_file, comment='#', names=range(16), index_col=0, skip_blank_lines=True, sep="\\s+")
     bool_dupl_index = foreman_harmonic_raw.index.duplicated(keep='first')
     
     lat_rad = np.deg2rad(lat_deg)
     
     R1 = 0.36309*(1.-5.*np.sin(lat_rad)*np.sin(lat_rad))/np.sin(lat_rad) #-1 #for lat=50N
     R2 = 2.59808*np.sin(lat_rad) #2 #for lat=50N
     
@@ -111,15 +93,15 @@
     -------
     foreman_shallowrelations : TYPE
         DESCRIPTION.
 
     """
     
     foreman_file = os.path.join(os.path.dirname(file_path),'data','data_foreman_shallowrelations.txt')
-    foreman_shallowrelations = pd.read_csv(foreman_file, comment='#', names=range(10), index_col=0, delim_whitespace=True)
+    foreman_shallowrelations = pd.read_csv(foreman_file, comment='#', names=range(10), index_col=0, sep="\\s+")
     foreman_shallowrelations.index.name = None
     
     #check for internal numdependencies consistency
     for const in foreman_shallowrelations.index:
         foreman_shallow_const = foreman_shallowrelations.loc[const].dropna().values
         num_dependencies = foreman_shallow_const[0]
         list_shallow_facs = foreman_shallow_const[1::2]
```

### Comparing `hatyan-2.7.0/hatyan/hatyan_core.py` & `hatyan-2.8.0/hatyan/hatyan_core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,25 @@
 # -*- coding: utf-8 -*-
 """
 hatyan_core.py contains core components that wrap around schureman/foreman definitions
-
-hatyan is a Python program for tidal analysis and prediction, based on the FORTRAN version. 
-Copyright (C) 2019-2021 Rijkswaterstaat.  Maintained by Deltares, contact: Jelmer Veenstra (jelmer.veenstra@deltares.nl). 
-Source code available at: https://github.com/Deltares/hatyan
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Lesser General Public License for more details.
-
-You should have received a copy of the GNU Lesser General Public License
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
 """
 
 import pandas as pd
 import datetime as dt
 import numpy as np
 import functools
+import logging
 
 from hatyan.schureman import get_schureman_freqs, get_schureman_v0, get_schureman_u, get_schureman_f, get_schureman_table
 from hatyan.foreman import get_foreman_v0_freq, get_foreman_doodson_nodal_harmonic, get_foreman_shallowrelations, get_foreman_nodalfactors
 
+__all__ = ["get_const_list_hatyan"]
+
+logger = logging.getLogger(__name__)
+
 
 @functools.lru_cache()
 def check_requestedconsts(const_list_tuple,source):
     #TODO: move check to central location when part of hatyan_settings()?
     if source=='schureman':
         const_list_allforsource = get_schureman_table().index
     elif source=='foreman':
@@ -41,49 +28,49 @@
         const_list_allforsource = pd.Series(foreman_doodson_harmonic.index.append(foreman_shallowrelations.index))
     
     bool_constavailable = pd.Series(const_list_tuple).isin(const_list_allforsource)   
     if not bool_constavailable.all():
         raise Exception(f'ERROR: not all requested components available in schureman harmonics or shallowrelations:\n{pd.Series(const_list_tuple).loc[~bool_constavailable]}')
 
 
-def get_freqv0_generic(hatyan_settings, const_list, dood_date_mid, dood_date_start):
+def get_freqv0_generic(const_list, dood_date_mid, dood_date_start, source):
 
     if type(const_list) is str:
         const_list = get_const_list_hatyan(const_list)
 
     #retrieve frequency and v0
-    print(f'freq is calculated at mid of period: {dood_date_mid[0]}')
-    print(f'v0 is calculated for start of period: {dood_date_start[0]}')
-    if hatyan_settings.source=='schureman':
+    logger.debug(f'freq is calculated at mid of period: {dood_date_mid[0]}')
+    logger.debug(f'v0 is calculated for start of period: {dood_date_start[0]}')
+    if source=='schureman':
         t_const_freq_pd = get_schureman_freqs(const_list, dood_date=dood_date_mid)
         v_0i_rad = get_schureman_v0(const_list, dood_date_start).T #at start of timeseries
-    elif hatyan_settings.source=='foreman': #TODO: this is probably quite slow since foreman is not cached
+    elif source=='foreman': #TODO: this is probably quite slow since foreman is not cached
         dummy, t_const_freq_pd = get_foreman_v0_freq(const_list=const_list, dood_date=dood_date_mid) #TODO: does this really matter, maybe just retrieve on dood_date_start? Otherwise maybe split definition?
         v_0i_rad, dummy = get_foreman_v0_freq(const_list=const_list, dood_date=dood_date_start)
         v_0i_rad = v_0i_rad.T
     
     return t_const_freq_pd, v_0i_rad
 
 
-def get_uf_generic(hatyan_settings, const_list, dood_date_fu):
+def get_uf_generic(const_list, dood_date_fu, nodalfactors, xfac, source):
 
     #get f and u
-    if hatyan_settings.nodalfactors:
+    if nodalfactors:
         if len(dood_date_fu)==1: #dood_date_mid
-            print('nodal factors (f and u) are calculated for center of period: %s'%(dood_date_fu[0]))
+            logger.info('nodal factors (f and u) are calculated for center of period: %s'%(dood_date_fu[0]))
         else: #times_pred_all_pdDTI
-            print('nodal factors (f and u) are calculated for all timesteps')
-        if hatyan_settings.source=='schureman':
-            f_i = get_schureman_f(xfac=hatyan_settings.xfac, const_list=const_list, dood_date=dood_date_fu).T
+            logger.info('nodal factors (f and u) are calculated for all timesteps')
+        if source=='schureman':
+            f_i = get_schureman_f(xfac=xfac, const_list=const_list, dood_date=dood_date_fu).T
             u_i_rad = get_schureman_u(const_list=const_list, dood_date=dood_date_fu).T
-        elif hatyan_settings.source=='foreman': #TODO: this is probably quite slow since foreman is not cached
+        elif source=='foreman': #TODO: this is probably quite slow since foreman is not cached
             f_i, u_i_rad = get_foreman_nodalfactors(const_list=const_list, dood_date=dood_date_fu)
             f_i, u_i_rad = f_i.T, u_i_rad.T
     else:
-        print('no nodal factors (f and u) correction applied (f=1, u=0)')
+        logger.info('no nodal factors (f and u) correction applied (f=1, u=0)')
         f_i = pd.DataFrame(np.ones(len(const_list)),index=const_list).T
         u_i_rad = pd.DataFrame(np.zeros(len(const_list)),index=const_list).T
     return u_i_rad, f_i
 
 
 def get_doodson_eqvals(dood_date, mode=None):
     """
@@ -138,45 +125,14 @@
         dood_P1_rad = (4.9082295 + 0.0300053*dood_Tj    + 0.0000079*dood_Tj**2)
         #from SLS table 4.2: pd.DataFrame(dict(const=[218.32,280.47,83.35,125.04,282.94],T=[481267.88,36000.77,4069.01,-1934.14,1.72]),index=['S','H','P','N','P1'])#/180*np.pi
     doodson_pd = pd.DataFrame(np.stack([dood_T_rad, dood_S_rad, dood_H_rad, dood_P_rad, dood_N_rad, dood_P1_rad]),
                               index=['T','S','H','P','N','P1'])
     return doodson_pd
 
 
-def robust_daterange_fromtimesextfreq(times_ext,timestep_min):
-    """
-    Generate daterange. Pandas pd.date_range and pd.DatetimeIndex only support times between 1677-09-21 and 2262-04-11, because of its ns accuracy.
-    For dates outside this period, a list is generated and converted to a pd.Index instead.
-
-    Parameters
-    ----------
-    times_ext : list of datetime.datetime
-        DESCRIPTION.
-    timestep_min : int
-        DESCRIPTION.
-
-    Returns
-    -------
-    times_pred_all_pdDTI : pd.DatetimeIndex or pd.Index
-        DESCRIPTION.
-
-    """
-    
-    try:
-        times_pred_all = pd.date_range(start=times_ext[0], end=times_ext[-1], freq='%imin'%(timestep_min))
-        times_pred_all_pdDTI = pd.DatetimeIndex(times_pred_all)
-    except pd._libs.tslibs.np_datetime.OutOfBoundsDatetime as e: #OutOfBoundsDatetime: Out of bounds nanosecond timestamp
-        print(f'WARNING: "{e}". Falling back to less fancy (slower) datetime ranges. Fancy ones are possible between {pd.Timestamp.min} and {pd.Timestamp.max}')
-        td_mins = (times_ext[-1]-times_ext[0]).total_seconds()/60
-        nsteps = int(td_mins/timestep_min)
-        times_pred_all = pd.Series([times_ext[0]+dt.timedelta(minutes=x*timestep_min) for x in range(nsteps+1)])
-        times_pred_all_pdDTI = pd.Index(times_pred_all)
-    return times_pred_all_pdDTI
-
-
 def robust_timedelta_sec(dood_date,refdate_dt=None):
     """
     Generate timedelta. Pandas pd.DatetimeIndex subtraction only supports times between 1677-09-21 and 2262-04-11, because of its ns accuracy.
     For dates outside this period, a list subtraction is generated.
     
     Parameters
     ----------
@@ -189,24 +145,19 @@
     -------
     dood_tstart_sec : np.array
         DESCRIPTION.
     fancy_pddt : bool
         DESCRIPTION.
 
     """
-    #TODO: check if this is still necessary in newer pandas versions (might account for out of bounds timestamps automatically)
-    #TODO: merging with robust_daterange_fromtimesextfreq() possible?
     
     if refdate_dt is None:
-        refdate_dt = dt.datetime(1900,1,1)
-        
-    if isinstance(dood_date,pd.core.indexes.datetimes.DatetimeIndex): # not OutOfBoundsDatetime datetime result in default DatetimeIndex
-        dood_tstart_sec = ( dood_date-refdate_dt ).total_seconds().values
-    else: #in case of OutOfBoundsDatetime it is an Index instead of a DatetimeIndex (following from hatyan.robust_daterange_fromtimesextfreq())
-        dood_tstart_sec = np.array([(x-refdate_dt).total_seconds() for x in dood_date])
+        refdate_dt = pd.Timestamp(1900,1,1)
+    
+    dood_tstart_sec = ( dood_date-refdate_dt ).total_seconds().values
     return dood_tstart_sec
 
 
 def get_lunarSLSIHO_fromsolar(v0uf_base): #TODO: iets simpeler implementatie in foreman.get_foreman_doodson_nodal_harmonic(), maar dit is ook prima
     
     #conversion to lunar for comparison with SLS and IHO
     v0uf_baseT_solar = v0uf_base.loc[['T','S','H','P','N','P1','EDN']].T
@@ -247,15 +198,15 @@
 
 def sort_const_list(const_list):
     full_const_list_withfreqs = get_full_const_list_withfreqs()
     const_list_sorted = full_const_list_withfreqs.loc[const_list].sort_values('freq').index.tolist()
     return const_list_sorted
 
 
-def get_const_list_hatyan(listtype, return_listoptions=False):
+def get_const_list_hatyan(listtype):
     """
     Definition of several hatyan components lists, taken from the tidegui initializetide.m code, often originating from corresponcence with Koos Doekes
 
     Parameters
     ----------
     listtype : str
         The type of the components list to be retrieved, options:
@@ -265,14 +216,15 @@
             - 'halfyear': list of 88 components to be used when analyzing approximately half a year of data
             - 'month': list of 21 components to be used when analyzing one month of data. If desired, the K1 component can be splitted in P1/K1, N2 in N2/Nu2, S2 in T2/S2/K2 and 2MN2 in Labda2/2MN2.
             - 'month_deepwater': list of 21 components to be used when analyzing one month of data for deep water (from tidegui).
             - 'springneap': list of 14 components to be used when analyzing one spring neap period (approximately 15 days) of data
             - 'day': list of 10 components to be used when analyzing one day
             - 'day_tidegui': list of 5 components to be used when analyzing one day ir two tidal cycles (from tidegui)
             - 'tidalcycle': list of 6 components to be used when analyzing one tidal cycle (approximately 12 hours and 25 minutes)
+    
     Raises
     ------
     Exception
         DESCRIPTION.
 
     Returns
     -------
@@ -445,18 +397,12 @@
                         'tidalcycle':
                             #harmonic constituents for 1-tide analysis
                             #A0 en 6 componenten
                             ['A0','M2','M4','M6','M8','M10','M12']
                         }
     
     const_list_options = const_lists_dict.keys()
-    if listtype in const_list_options:
-        const_list_hatyan = const_lists_dict[listtype]
-    else:
-        raise Exception('ERROR: listtype "%s" is not implemented in get_const_list_hatyan, choose from: %s'%(str(listtype),const_list_options))
-        
-    if return_listoptions:
-        return const_list_hatyan, const_list_options
-    else:
-        return const_list_hatyan
-
-
+    if listtype not in const_list_options:
+        raise KeyError(f'listtype "{listtype}" is not implemented in hatyan.get_const_list_hatyan(), choose from: [{", ".join(const_list_options)}]')
+    
+    const_list_hatyan = const_lists_dict[listtype]
+    return const_list_hatyan
```

### Comparing `hatyan-2.7.0/hatyan/schureman.py` & `hatyan-2.8.0/hatyan/schureman.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,21 @@
 # - * - coding: utf - 8 - * - 
 """
 schureman.py contains definitions with data for the schureman constituents.
-
-hatyan is a Python program for tidal analysis and prediction, based on the FORTRAN version. 
-Copyright (C) 2019-2021 Rijkswaterstaat.  Maintained by Deltares, contact: Jelmer Veenstra (jelmer.veenstra@deltares.nl). 
-Source code available at: https://github.com/Deltares/hatyan
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Lesser General Public License for more details.
-
-You should have received a copy of the GNU Lesser General Public License
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
 """
 
 import os
 import pandas as pd
 import functools #to Memoize v0uf table (https://en.wikipedia.org/wiki/Memoization)
 import numpy as np
 import datetime as dt
+import logging
 
 file_path = os.path.realpath(__file__)
+logger = logging.getLogger(__name__)
 
 
 @functools.lru_cache()
 def get_schureman_shallowrelations():
     file_schureman_shallowrelations = os.path.join(os.path.dirname(file_path),'data','data_schureman_shallowrelations.csv')
     shallow_eqs_pd = pd.read_csv(file_schureman_shallowrelations,comment='#',skipinitialspace=True,index_col=0,names=['shallow_eq'])
     shallow_eqs_pd['shallow_eq'] = shallow_eqs_pd['shallow_eq'].str.strip() #remove spaces after
@@ -64,17 +48,17 @@
     #v0uf_base.index = index_v0 + index_u + index_f + index_fstr
     
     shallow_eqs_pd = get_schureman_shallowrelations()
     shallow_eqs_pd_str = '\n'.join(f'{key} = {val}' for key, val in shallow_eqs_pd['shallow_eq'].items()) 
 
     #calculate shallow water components and rename back to original component name
     v0uf_base_forv0u = v0uf_base.loc[index_v0+index_u,:].astype(int)
-    v0uf_base_forv0u.eval(shallow_eqs_pd_str, inplace=True)
+    v0uf_base_forv0u = v0uf_base_forv0u.eval(shallow_eqs_pd_str, inplace=False)
     v0uf_base_forf = v0uf_base.loc[index_f,:].astype(float)
-    v0uf_base_forf.eval(shallow_eqs_pd_str.replace('-','+'), inplace=True) #for f only multiplication is applied, never division
+    v0uf_base_forf = v0uf_base_forf.eval(shallow_eqs_pd_str.replace('-','+'), inplace=False) #for f only multiplication is applied, never division
     v0uf_all = pd.concat([v0uf_base_forv0u,v0uf_base_forf])
     v0uf_all.rename(columns=shallow_eqs_pd['shallow_const'],inplace=True)
     v0uf_allT = v0uf_all.T
     
     #from hatyan.hatyan_core import get_lunarSLSIHO_fromsolar # local import since otherwise cross-dependency
     #v0uf_allT_lunar, v0uf_allT_lunar_SLS, v0uf_allT_lunar_IHO = get_lunarSLSIHO_fromsolar(v0uf_all)
     
@@ -404,15 +388,15 @@
     -------
     f_i_pd : TYPE
         DESCRIPTION.
 
     """
     
     if isinstance(xfac,dict):
-        print('xfac dictionary provided: %s'%(xfac))
+        logger.info(f'xfac dictionary provided: {xfac}')
         xfac_values = xfac
     else: #use default xfactor values
         xfac_values = {'MU2': 0.00, # 0 betekent knoopfactor uit, 1 is helemaal aan
                        'N2':  0.00,
                        'NU2': 0.80,
                        'M2':  0.53,
                        '2MN2':0.20,
```

### Comparing `hatyan-2.7.0/hatyan/timeseries.py` & `hatyan-2.8.0/hatyan/timeseries.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 # -*- coding: utf-8 -*-
 """
 timeseries.py contains all definitions related to hatyan timeseries.
-
-hatyan is a Python program for tidal analysis and prediction, based on the FORTRAN version. 
-Copyright (C) 2019-2021 Rijkswaterstaat.  Maintained by Deltares, contact: Jelmer Veenstra (jelmer.veenstra@deltares.nl). 
-Source code available at: https://github.com/Deltares/hatyan
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Lesser General Public License for more details.
-
-You should have received a copy of the GNU Lesser General Public License
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
 """
 
 import os
 import io
+import glob
 import numpy as np
 import pandas as pd
 import datetime as dt
+import pytz
 import scipy.signal as ssig
-file_path = os.path.realpath(__file__)
 import matplotlib.pyplot as plt
 from scipy.fft import fft, fftfreq
-from netCDF4 import Dataset, date2num, stringtoarr#, num2date
+from netCDF4 import Dataset, date2num, stringtoarr
+import logging
+from pyproj import Transformer
+
 from hatyan.foreman import get_foreman_v0_freq
 from hatyan.schureman import get_schureman_freqs
 from hatyan.hatyan_core import get_const_list_hatyan
+from hatyan.metadata import (metadata_from_diablocks, metadata_add_to_obj, 
+                             metadata_from_obj, metadata_compare, 
+                             wns_from_metadata)
+
+__all__ = ["get_diaxycoords",
+           "read_dia",
+           "read_noos",
+           "write_dia",
+           "write_noos",
+           "write_netcdf",
+           "plot_timeseries",
+           "plot_HWLW_validatestats",
+           "resample_timeseries",
+           "crop_timeseries",
+           "timeseries_fft",
+           "Timeseries_Statistics",
+           "calc_HWLW",
+           "calc_HWLWnumbering",
+           "calc_HWLW12345to12",
+           ]
+
+file_path = os.path.realpath(__file__)
+logger = logging.getLogger(__name__)
 
 
-def calc_HWLW(ts, calc_HWLW345=False, calc_HWLW1122=False, debug=False, buffer_hr=6):
+def calc_HWLW(ts, calc_HWLW345=False, buffer_hr=6):
     """
     
     Calculates extremes (high and low waters) for the provided timeseries. 
     This definition uses scipy.signal.find_peaks() with arguments 'distance' and 'prominence'. 
     The minimal 'distance' between two high or low water peaks is based on the M2 period: 12.42/1.5=8.28 hours for HW and 12.42/1.7=7.30 hours for LW (larger because of aggers). 
     The prominence for local extremes is set to 0.01m, to filter out very minor dips in the timeseries.
     If there are two equal high or low water values, the first one is taken. 
@@ -51,54 +60,46 @@
     ----------
     ts : pandas.DataFrame
         The DataFrame should contain a 'values' column and a pd.DatetimeIndex as index, it contains the timeseries with a tidal prediction or water level measurements.
     calc_HWLW345 : boolean, optional
         Whether to also calculate local extremes, first/second low waters and 'aggers'. 
         The default is False, in which case only extremes per tidal period are calculated.
         When first/second low waters and aggers are calculated, the local extremes around highwater (eg double highwaters and dips) are filtered out first.
-    calc_HWLW345_cleanup1122 : boolean, optional
-        Whether to remove HWLWcodes 11 and 22 from DataFrame. The default is True.
-    debug : boolean, optional
-        Whether to print debug information. The default is False.
-    
-    Raises
-    ------
-    Exception
-        DESCRIPTION.
     
     Returns
     -------
     data_pd_HWLW : pandas.DataFrame
         The DataFrame contains colums 'times', 'values' and 'HWLWcode', it contains the times, values and codes of the timeseries that are extremes.
         1 (high water) and 2 (low water). And if calc_HWLW345=True also 3 (first low water), 4 (agger) and 5 (second low water).
 
     """
     
     if not ts.index.is_monotonic_increasing:
-        raise Exception('ERROR: timeseries is not monotonic increasing, supply sorted timeseries (ts = ts.index.sort_index()') #otherwise "ValueError: 'list' argument must have no negative elements"
+        raise Exception('timeseries is not monotonic increasing, supply sorted timeseries (ts = ts.index.sort_index()') #otherwise "ValueError: 'list' argument must have no negative elements"
     
     #calculate the amount of steps in a M2 period, based on the most occurring timestep 
     M2_period_sec = get_schureman_freqs(['M2']).loc['M2','period [hr]']*3600
-    ts_steps_sec_most = np.argmax(np.bincount((ts.index.to_series().diff().iloc[1:].dt.total_seconds()).astype(int).values))
+    
+    ts_steps_sec_most = np.argmax(np.bincount(pd.Series(np.diff(ts.index)).dt.total_seconds().astype(int).values))
     if ts_steps_sec_most > 60:
-        print(f'WARNING: the timestep of the series for which to calculate extremes/HWLW is {ts_steps_sec_most/60:.2f} minutes, but 1 minute is recommended')
+        logger.warning(f'the timestep of the series for which to calculate extremes/HWLW is {ts_steps_sec_most/60:.2f} minutes, but 1 minute is recommended')
     elif ts_steps_sec_most == 0:
-        raise Exception('ERROR: ts_steps_sec_most=0, check rounding issue')
+        raise ValueError('ts_steps_sec_most=0, check rounding issue')
     M2period_numsteps = M2_period_sec/ts_steps_sec_most
     minwidth_numsteps = 2*3600/ts_steps_sec_most # minimal width of 2 hours makes peakfinding more robust: https://github.com/Deltares/hatyan/issues/85
 
     data_pd_HWLW = pd.DataFrame({'times':ts.index,'values':ts['values'],'HWLWcode':np.nan}).reset_index(drop=True)
     #create empty HWLW dataframe
     if data_pd_HWLW['values'].isnull().any():
         data_pd_HWLW = data_pd_HWLW[~data_pd_HWLW['values'].isnull()].reset_index(drop=True)
-        print('WARNING: the provided ts for extreme/HWLW calculation contained NaN values. To avoid unexpected results from scipy.signal.find_peaks(), the %i NaN values were removed from the ts (%.2f%%) before calculating extremes/HWLW.'%(len(ts)-len(data_pd_HWLW), (len(ts)-len(data_pd_HWLW))/len(ts)*100))
+        logger.warning('the provided ts for extreme/HWLW calculation contained NaN values. To avoid unexpected results from scipy.signal.find_peaks(), the %i NaN values were removed from the ts (%.2f%%) before calculating extremes/HWLW.'%(len(ts)-len(data_pd_HWLW), (len(ts)-len(data_pd_HWLW))/len(ts)*100))
 
     min_prominence = 0.01 #minimal prominence to exclude very minor dips/peaks from being seen as aggers.
     
-    if calc_HWLW345 or calc_HWLW1122:
+    if calc_HWLW345:
         #get all local extremes, including aggers and second high waters (1/2/11/22) #takes first value of two equal peaks
         LWid_all, LWid_all_properties = ssig.find_peaks(-data_pd_HWLW['values'].values, prominence=(min_prominence,None), width=(None,None), distance=None)
         HWid_all, HWid_all_properties = ssig.find_peaks(data_pd_HWLW['values'].values, prominence=(min_prominence,None), width=(None,None), distance=None)
         data_pd_HWLW.loc[LWid_all,'HWLWcode'] = 22 #all LW
         data_pd_HWLW.loc[HWid_all,'HWLWcode'] = 11 #all HW
 
     #get HWLW (extremes per tidal period).
@@ -112,33 +113,38 @@
     data_pd_HWLW.loc[LWid_main,'HWLWcode'] = 2
     data_pd_HWLW.loc[HWid_main,'HWLWcode'] = 1
     
     #drop all non-(local)extreme timesteps and convert HWLWcode column to integers
     data_pd_HWLW = data_pd_HWLW.dropna(subset=['HWLWcode'])
     data_pd_HWLW['HWLWcode'] = data_pd_HWLW['HWLWcode'].astype(int)
 
-    if debug: #debug statistics
-        prop_list = ['prominences','widths']
-        data_pd_HWLW.loc[data_pd_HWLW['HWLWcode']==2,prop_list] = pd.DataFrame(LWid_main_properties,index=LWid_main_raw).loc[LWid_main,prop_list]
-        print('LW values:\n%s\n'%(data_pd_HWLW[data_pd_HWLW['HWLWcode']==2]))
-        data_pd_HWLW.loc[data_pd_HWLW['HWLWcode']==1,prop_list] = pd.DataFrame(HWid_main_properties,index=HWid_main_raw).loc[HWid_main,prop_list]
-        print('HW values:\n%s\n'%(data_pd_HWLW[data_pd_HWLW['HWLWcode']==1]))
-        if calc_HWLW345 or calc_HWLW1122:
-            LW_local_bool = ~np.in1d(LWid_all, LWid_main)
-            data_pd_HWLW.loc[data_pd_HWLW['HWLWcode']==22,prop_list] = pd.DataFrame(LWid_all_properties,index=LWid_all).loc[LW_local_bool,prop_list]
-            print('LW_local values:\n%s\n'%(data_pd_HWLW[data_pd_HWLW['HWLWcode']==22]))
-            HW_local_bool = ~np.in1d(HWid_all, HWid_main)
-            data_pd_HWLW.loc[data_pd_HWLW['HWLWcode']==11,prop_list] = pd.DataFrame(HWid_all_properties,index=HWid_all).loc[HW_local_bool,prop_list]
-            print('HW_local values:\n%s\n'%(data_pd_HWLW[data_pd_HWLW['HWLWcode']==11]))
+    # extensive debugging statistics
+    prop_list = ['prominences','widths']
+    data_pd_HWLW.loc[data_pd_HWLW['HWLWcode']==2,prop_list] = pd.DataFrame(LWid_main_properties,index=LWid_main_raw).loc[LWid_main,prop_list]
+    logger.debug('LW values:\n%s\n'%(data_pd_HWLW[data_pd_HWLW['HWLWcode']==2]))
+    data_pd_HWLW.loc[data_pd_HWLW['HWLWcode']==1,prop_list] = pd.DataFrame(HWid_main_properties,index=HWid_main_raw).loc[HWid_main,prop_list]
+    logger.debug('HW values:\n%s\n'%(data_pd_HWLW[data_pd_HWLW['HWLWcode']==1]))
+    if calc_HWLW345:
+        LW_local_bool = ~np.in1d(LWid_all, LWid_main)
+        data_pd_HWLW.loc[data_pd_HWLW['HWLWcode']==22,prop_list] = pd.DataFrame(LWid_all_properties,index=LWid_all).loc[LW_local_bool,prop_list]
+        logger.debug('LW_local values:\n%s\n'%(data_pd_HWLW[data_pd_HWLW['HWLWcode']==22]))
+        HW_local_bool = ~np.in1d(HWid_all, HWid_main)
+        data_pd_HWLW.loc[data_pd_HWLW['HWLWcode']==11,prop_list] = pd.DataFrame(HWid_all_properties,index=HWid_all).loc[HW_local_bool,prop_list]
+        logger.debug('HW_local values:\n%s\n'%(data_pd_HWLW[data_pd_HWLW['HWLWcode']==11]))
     
     if calc_HWLW345: #recalculate local LW/HWs between two main HWs to firstLW/agger/secondLW
         data_pd_HWLW = calc_HWLWlocalto345(data_pd_HWLW,HWid_main)
     
     #return to normal time-index
     data_pd_HWLW = data_pd_HWLW.set_index('times')
+    
+    # add metadata #TODO: update metadata for extremes?
+    metadata = metadata_from_obj(ts)
+    data_pd_HWLW = metadata_add_to_obj(data_pd_HWLW,metadata)
+    
     return data_pd_HWLW
 
 
 def calc_HWLWlocalto345(data_pd_HWLW,HWid_main):
     """
     Recalculate local LW/HWs between two main HWs to firstLW/agger/secondLW
 
@@ -157,27 +163,27 @@
     Returns
     -------
     data_pd_HWLW : TYPE
         DESCRIPTION.
 
     """
     
-    print('calculating 1stLW/agger/2ndLW for all tidalperiods (between two HW values)...')
+    logger.info('calculating 1stLW/agger/2ndLW for all tidalperiods (between two HW values)...')
     for iTide, dummy in enumerate(HWid_main[:-1]):
         data_pd_HWLW_1tide = data_pd_HWLW.loc[HWid_main[iTide]:HWid_main[iTide+1],:]
         
         #filter local extremes around HW (only interested in aggers, so LW), this is necessary for eg DENHDR and PETTZD, otherwise second HW is seen as first LW
-        data_pd_HWLW_1tide_minHW = data_pd_HWLW_1tide.loc[data_pd_HWLW_1tide['HWLWcode']==1,['values']].min()[0]
+        data_pd_HWLW_1tide_minHW = data_pd_HWLW_1tide.loc[data_pd_HWLW_1tide['HWLWcode']==1,'values'].min()
         data_pd_HWLW_1tide_min = data_pd_HWLW_1tide['values'].min()
         data_pd_HWLW_1tide_mid = np.mean([data_pd_HWLW_1tide_minHW,data_pd_HWLW_1tide_min])
         bool_LWs = data_pd_HWLW_1tide['values']<data_pd_HWLW_1tide_mid
         data_pd_HWLW_1tide_noHWs = data_pd_HWLW_1tide[bool_LWs]
         
         if len(data_pd_HWLW_1tide_noHWs) > 3: #(attempt to) reduce to three values between two HWs
-            print('WARNING: more than 3 values between HWs, removing part of them')
+            logger.warning('more than 3 values between HWs, removing part of them')
             agger35_prim = data_pd_HWLW_1tide_noHWs[data_pd_HWLW_1tide_noHWs['HWLWcode']==2]
             if len(agger35_prim)>1:
                 raise Exception('should be only one HWLWcode=2 per tide period')
             agger35_prim_loc = agger35_prim.index[0]
             agger35_sec_loc = data_pd_HWLW_1tide_noHWs.loc[data_pd_HWLW_1tide_noHWs['HWLWcode']==22,'values'].idxmin()
             agger35_loc = np.sort([agger35_prim_loc,agger35_sec_loc])
             data_pd_HWLW_1tide_noHWs = data_pd_HWLW_1tide_noHWs.loc[agger35_loc.min():agger35_loc.max(),:]
@@ -191,23 +197,23 @@
             if not data_pd_HWLW_1tide_noHWs['values'].argmax() == 1:
                 raise Exception('3 values between two HW values, but center one is not the largest:\n%s'%(data_pd_HWLW_1tide))
             agger345_loc = data_pd_HWLW_1tide_noHWs.index
             if not (data_pd_HWLW.loc[agger345_loc[0],'HWLWcode'] in [2,22] and data_pd_HWLW.loc[agger345_loc[1],'HWLWcode'] in [11] and data_pd_HWLW.loc[agger345_loc[2],'HWLWcode'] in [2,22]):
                 raise Exception('3 values between two HW values, but do not correspond to LW/agger/LW:\n%s'%(data_pd_HWLW_1tide))
             data_pd_HWLW.loc[agger345_loc,'HWLWcode'] = [3,4,5]
         elif len(data_pd_HWLW_1tide_noHWs) == 2:
-            print('WARNING: 2 values left between two HWs (slightly unexpected):\n%s'%(data_pd_HWLW_1tide))
+            logger.warning('2 values left between two HWs (slightly unexpected):\n%s'%(data_pd_HWLW_1tide))
         else:
             raise Exception('unexpected number of values between two HWs (0 or more than 3):\n%s'%(data_pd_HWLW_1tide))
     
     #remove remaining 11 and 22 values from array
     data_pd_HWLW = data_pd_HWLW.drop(data_pd_HWLW[data_pd_HWLW['HWLWcode']==11].index)
     data_pd_HWLW = data_pd_HWLW.drop(data_pd_HWLW[data_pd_HWLW['HWLWcode']==22].index)
     
-    print('finished calculating 1stLW/agger/2ndLW for all tidalperiods')
+    logger.info('finished calculating 1stLW/agger/2ndLW for all tidalperiods')
     
     return data_pd_HWLW
 
 
 def calc_HWLW12345to12(data_HWLW_12345):
     """
     
@@ -219,18 +225,18 @@
     
     Returns
     -------
     None.
     
     """
     if len(data_HWLW_12345['HWLWcode'].unique()) <= 2:
-        print('skipping HWLW 12345 to 12 correction since no 345 found, returning input df')
+        logger.info('skipping HWLW 12345 to 12 correction since no 345 found, returning input df')
         return data_HWLW_12345.copy()
     
-    print('starting HWLW 12345 to 12 correction')
+    logger.info('starting HWLW 12345 to 12 correction')
     times_LWmin = []
     data_HW1 = data_HWLW_12345.loc[data_HWLW_12345['HWLWcode']==1]
     #computing minimum waterlevels after each HW. Using hardcoded 12hour period instead of from one HW to next HW since then we can also assess last LW values
     for timeHW in data_HW1.index: #np.arange(0,len(data_HW1)-1):
         if timeHW==data_HWLW_12345.index[-1]: #if last HW is last time of input dataframe
             continue
         #tide_afterHW = data_HWLW_12345.loc[data_HW1.index[iHW]:data_HW1.index[iHW+1]]
@@ -249,15 +255,15 @@
         firstlast.append(data_HWLW_12345.iloc[[0]])
     
     data_HWLW_12 = pd.concat(firstlast+[data_HW1,data_LW2]).sort_index()
     
     return data_HWLW_12
 
 
-def calc_HWLWnumbering(ts_ext, station=None, corr_tideperiods=None, mode='M2phase', doHWLWcheck=True):
+def calc_HWLWnumbering(ts_ext, station=None, doHWLWcheck=True):
     """
     For calculation of the extremes numbering, w.r.t. the first high water at Cadzand in 2000 (occurred on 1-1-2000 at approximately 9:45). 
     The number of every high and low water is calculated by taking the time difference between itself and the first high water at Cadzand, correcting it with the station phase difference (M2phasediff). 
     Low waters are searched for half an M2 period from the high waters. 
     By adding a search window of half the period of M2 (searchwindow_hr), even strong time variance between consecutive high or low waters should be caputered. 
     
     Parameters
@@ -265,74 +271,70 @@
     ts_ext : pandas.DataFrame
         The DataFrame should contain a 'values' and 'HWLWcode' column and a pd.DatetimeIndex as index, it contains the times, values and codes of the timeseries that are extremes.
     station: string, optional
         The station for which the M2 phase difference should be retrieved from data_M2phasediff_perstation.txt.
         This value is the phase difference in degrees of the occurrence of the high water generated by the same tidal wave as the first high water in 2000 at Cadzand (actually difference between M2 phases of stations).
         This value is used to correct the search window of high/low water numbering. The default is None.
         Providing a value will result in a proper HWLWno, corresponing to CADZD. Providing None will result in a HWLWno that is a multiple of 360degrees/M2_period_hr off (positive or negative). This is only an issue when comparing different stations, not comparing e.g. measured and predicted HW values of one station.
-    corr_tideperiods : integer, optional
-        Test keyword to derive HWLWnumbering with a n*360 degrees offset on top of what is calculated automatically. The default is None.    
+    
     Raises
     ------
     Exception
         DESCRIPTION.
 
     Returns
     -------
     ts_ext : pandas.DataFrame
         The input DataFrame with the column 'HWLWno' added, which contains the numbers of the extremes.
 
     """
         
     M2_period_hr = get_schureman_freqs(['M2']).loc['M2','period [hr]']
-    firstHWcadz_fixed = dt.datetime(2000, 1, 1, 9, 45)
+    firstHWcadz_fixed = pd.Timestamp("2000-01-01 09:45:00 +01:00") #dt.datetime(2000, 1, 1, 9, 45)
+    firstHWcadz_fixed = firstHWcadz_fixed.tz_convert(ts_ext.index.tz)
     searchwindow_hr = M2_period_hr/2
     
     if len(ts_ext) == 0:
         raise Exception('length of provided ts_ext is zero')
     
     if not all((ts_ext['HWLWcode']==1) | (ts_ext['HWLWcode']==2) | (ts_ext['HWLWcode']==3) | (ts_ext['HWLWcode']==4) | (ts_ext['HWLWcode']==5)):
         raise Exception('calc_HWLWnumbering() not implemented for HWLWcode other than 1,2,3,4,5 (so no HWLWcode 11 or 22 supported), provide extreme timeseries derived with Timeseries.calc_HWLW(calc_HWLW345=False) or Timeseries.calc_HWLW(calc_HWLW345=True, calc_HWLW345_cleanup1122=True)')
+    
+    # copy object but retain metadata
+    metadata_ext = metadata_from_obj(ts_ext)
     ts_ext = ts_ext.copy()
+    ts_ext = metadata_add_to_obj(ts_ext, metadata_ext) # otherwise M2-analysis fails
     
     HW_bool = ts_ext['HWLWcode']==1
     HW_tdiff_cadzdraw = (ts_ext.loc[HW_bool].index.to_series()-firstHWcadz_fixed).dt.total_seconds()/3600
     if station is None:
-        if mode=='M2phase':
-            from hatyan.analysis_prediction import analysis #TODO: local import since Importerror: cannot import name 'analysis' from partially initialized module 'hatyan.analysis_prediction' (most likely due to a circular import) 
-            M2phase_cadzd = 48.81 #from analyse waterlevels CADZD over 2009 t/m 2012
-            comp_M2 = analysis(ts_ext,const_list=['M2'],xTxmat_condition_max=250) ##TODO: high condition value necessary for some english stations. Not a big issue since it should provide a phasediff also in case of only one HW+LW. However, maybe HWtimediff mode is more robust
-            print(comp_M2.loc['M2','phi_deg'],M2phase_cadzd)
-            M2phasediff_deg = (comp_M2.loc['M2','phi_deg'] - M2phase_cadzd+90)%360-90
-        elif mode=='HWtimediff': #TODO: in principle this code is not necesary anymore
-            HW_tdiff_cadzdraw_M2remainders = (HW_tdiff_cadzdraw)%M2_period_hr
-            if HW_tdiff_cadzdraw_M2remainders.std()>3: #arbitrary value, but at least catches if all values are around 11/12/0/1 (rather have it around -2/-1/0/1)
-                HW_tdiff_cadzdraw_M2remainders = (HW_tdiff_cadzdraw+3)%M2_period_hr-3
-            M2phasediff_hr = (HW_tdiff_cadzdraw_M2remainders).median()
-            M2phasediff_deg = M2phasediff_hr/M2_period_hr*360
-        print(f'no value or None for argument M2phasediff provided, automatically calculated correction w.r.t. Cadzand (mode={mode}): ',end='')
-        if corr_tideperiods is not None:
-            M2phasediff_deg += corr_tideperiods
+        from hatyan.analysis_prediction import analysis #TODO: local import since Importerror: cannot import name 'analysis' from partially initialized module 'hatyan.analysis_prediction' (most likely due to a circular import) 
+        M2phase_cadzd = 48.81 #from analyse waterlevels CADZD over 2009 t/m 2012
+        # high max_matrix_condition value necessary for some english stations. Not a big issue since it should provide a phasediff also in case of only one HW+LW.
+        comp_M2 = analysis(ts_ext,const_list=['M2'],max_matrix_condition=250)
+        logger.debug(f"M2phase: {comp_M2.loc['M2','phi_deg']}, comp_M2_cadzd: {M2phase_cadzd}")
+        M2phasediff_deg = (comp_M2.loc['M2','phi_deg'] - M2phase_cadzd+90)%360-90
+        message_prefix = 'no value or None for argument M2phasediff provided, automatically calculated correction w.r.t. Cadzand based on M2phase:'
     else:
         file_M2phasediff = os.path.join(os.path.dirname(file_path),'data','data_M2phasediff_perstation.txt')
-        stations_M2phasediff = pd.read_csv(file_M2phasediff, names=['M2phasediff'], comment='#', delim_whitespace=True)
+        stations_M2phasediff = pd.read_csv(file_M2phasediff, names=['M2phasediff'], comment='#', sep="\\s+")
         if station not in stations_M2phasediff.index:
             raise Exception(f'ERROR: station "{station}" not in file_M2phasediff ({file_M2phasediff})')
         M2phasediff_deg = stations_M2phasediff.loc[station,'M2phasediff']
-        print('M2phasediff retrieved from file, correction w.r.t. Cadzand: ',end='')
+        message_prefix = 'M2phasediff retrieved from file, correction w.r.t. Cadzand:'
     M2phasediff_hr = M2phasediff_deg/360*M2_period_hr
-    print(f'{M2phasediff_hr:.2f} hours ({M2phasediff_deg:.2f} degrees)')
+    logger.info(f'{message_prefix} {M2phasediff_hr:.2f} hours ({M2phasediff_deg:.2f} degrees)')
     HW_tdiff_cadzd = HW_tdiff_cadzdraw - M2phasediff_hr + searchwindow_hr
     HW_tdiff_div, HW_tdiff_mod_searchwindow = np.divmod(HW_tdiff_cadzd.values, M2_period_hr)
     HW_tdiff_mod = HW_tdiff_mod_searchwindow - searchwindow_hr
     ts_ext.loc[HW_bool,'HWLWno'] = HW_tdiff_div
     if not all(np.diff(HW_tdiff_div) > 0):
-        idx_toosmall = np.where((np.diff(HW_tdiff_div) <= 0))[0]
-        print(idx_toosmall)
-        print(ts_ext.loc[HW_bool,['values','HWLWcode','HWLWno']].iloc[idx_toosmall[0]:])
+        idx_toosmall = np.nonzero((np.diff(HW_tdiff_div) <= 0))[0]
+        logger.info(idx_toosmall)
+        logger.info(ts_ext.loc[HW_bool,['values','HWLWcode','HWLWno']].iloc[idx_toosmall[0]:])
         raise Exception('tidal wave numbering: HW numbers not always increasing')
     if not all(np.abs(HW_tdiff_mod)<searchwindow_hr):
         raise Exception('tidal wave numbering: not all HW fall into hardcoded search window')
     
     for LWcode_2345 in [2,3,4,5]:
         LW_bool = ts_ext['HWLWcode']==LWcode_2345
         LW_tdiff_cadzdraw = (ts_ext.loc[LW_bool].index.to_series()-firstHWcadz_fixed).dt.total_seconds()/3600
@@ -353,30 +355,17 @@
             raise Exception('tidal wave numbering: first LW does not match first HW')
     
     ts_ext['HWLWno'] = ts_ext['HWLWno'].astype(int)
     
     return ts_ext
 
 
-def calc_HWLWtidalrange(ts_ext):
-    """
-    creates column 'tidalrange' in ts_ext dataframe
-    """
-    ts_ext = calc_HWLWnumbering(ts_ext=ts_ext)
-    ts_ext['times_backup'] = ts_ext.index
-    ts_ext_idxHWLWno = ts_ext.set_index('HWLWno',drop=False)
-    ts_ext_idxHWLWno['tidalrange'] = ts_ext_idxHWLWno.loc[ts_ext_idxHWLWno['HWLWcode']==1,'values'] - ts_ext_idxHWLWno.loc[ts_ext_idxHWLWno['HWLWcode']==2,'values']
-    ts_ext = ts_ext_idxHWLWno.set_index('times_backup')
-    ts_ext.index.name = 'times'
-    return ts_ext
-
-
 def timeseries_fft(ts_residue, min_prominence=10**3, max_freqdiff=None, plot_fft=True, source='schureman'):
     
-    print('analyzing timeseries with fft and fftfreq')
+    logger.info('analyzing timeseries with fft and fftfreq')
     
     if ts_residue['values'].isnull().sum() > 0:
         raise Exception('supplied timeseries contains nan values, use pd.interpolate first (dropping them will result in non-constant timestep which is also not possible for fft)')
     y = ts_residue['values'].values
     N = len(y)
     T = np.unique((ts_residue.index[1:]-ts_residue.index[:-1])).astype(float)/1e9/3600 #timestep in hours.
     if len(T)!=1:
@@ -410,15 +399,15 @@
     hatyan_freqs_suggestions = hatyan_freqs.loc[const_closest,['freq','period [hr]']]
     hatyan_freqs_suggestions['peak_freq'] = peak_freq
     hatyan_freqs_suggestions['peak_freqdiff'] = (hatyan_freqs_suggestions['freq'] - hatyan_freqs_suggestions['peak_freq']).abs()
     hatyan_freqs_suggestions['peak_prominences'] = peaks_properties['prominences']
     if max_freqdiff is not None:
         #select below freqdiff treshold
         hatyan_freqs_suggestions = hatyan_freqs_suggestions.loc[hatyan_freqs_suggestions['peak_freqdiff']<max_freqdiff]
-    print('suggested constituents+freqs from hatyan:\n%s'%(hatyan_freqs_suggestions))
+    logger.info('suggested constituents+freqs from hatyan:\n%s'%(hatyan_freqs_suggestions))
     
     return hatyan_freqs_suggestions
 
 
 def plot_timeseries(ts, ts_validation=None, ts_ext=None, ts_ext_validation=None):
     """
     Creates a plot with the provided timeseries
@@ -457,18 +446,18 @@
 
     fig, (ax1, ax2) = plt.subplots(2,1,figsize=size_figure, sharex=True, gridspec_kw={'height_ratios':[2,1]})
     
     ax1.set_title('hatyan timeseries')
     ax1.plot(ts.index, ts['values'],'o-',linewidth=size_line_ts,markersize=size_marker_ts, label='ts')
     if ts_validation is not None:
         if ts.index.duplicated().sum() + ts_validation.index.duplicated().sum() >0:
-            print(f'WARNING: duplicated timesteps in ts ({ts.index.duplicated().sum()}) or ts_validation ({ts_validation.index.duplicated().sum()}), timeseries difference computation will probably fail')
+            logger.warning(f'duplicated timesteps in ts ({ts.index.duplicated().sum()}) or ts_validation ({ts_validation.index.duplicated().sum()}), timeseries difference computation will probably fail')
         #overlap between timeseries for difference plots
-        times_id_validationinpred = np.where(ts_validation.index.isin(ts.index))[0]
-        times_id_predinvalidation = np.where(ts.index.isin(ts_validation.index))[0]
+        times_id_validationinpred = np.nonzero(ts_validation.index.isin(ts.index))[0]
+        times_id_predinvalidation = np.nonzero(ts.index.isin(ts_validation.index))[0]
         ax1.plot(ts_validation.index, ts_validation['values'],'o-',linewidth=size_line_ts,markersize=size_marker_ts, label='ts_validation', alpha=0.7)
         ax1.plot(ts.index[times_id_predinvalidation], ts['values'].iloc[times_id_predinvalidation].values-ts_validation['values'].iloc[times_id_validationinpred].values,'go-',linewidth=size_line_ts,markersize=size_marker_ts, label='difference', alpha=0.7)
     ax1.plot(times_predval_ext,[0,0],'-k',linewidth=size_line_ts)
     ts_mean = np.mean(ts['values'])
     ax1.plot(ts.index[[0,-1]],[ts_mean,ts_mean],'-r',linewidth=size_line_ts,label='mean of ts')
     if ts_ext is not None:
         HWLW_codesnames = {1:'HW (1)',
@@ -489,115 +478,102 @@
     if ts_ext_validation is not None:
         vali_codes = [1,2,3,4,5]
         vali_codenames = ['vali_HW','vali_LW','vali_LW1','vali_topagger','vali_LW2']
         for vali_code, vali_codename in zip(vali_codes,vali_codenames):
             vali_code_ids = ts_ext_validation['HWLWcode'].values==vali_code
             if any(vali_code_ids): #only plot vali_code in legend if present in HWLW_timeseries
                 ax1.plot(ts_ext_validation.index[vali_code_ids],ts_ext_validation['values'][vali_code_ids],'1',markersize=10,label=vali_codename)
-        #print HWLW statistics
-        try:
-            plot_HWLW_validatestats(ts_ext=ts_ext, ts_ext_validation=ts_ext_validation, create_plot=False)        
-        except: #TODO: replace this generic except with specific ones, but first convert 'raise Exception()' in plot_HWLW_validatestats() to more specific (maybe custom) ones
-            print('WARNING: plot_HWLW_validatestats() failed, probably due to missing HWLWno where autocalculation failed. Consider adding HWLWno to ts_ext and ts_ext_validation with calc_HWLWnumbering() before plotting.')
     ax1.set_ylim(figure_ylim_ts)
     ax2.set_xlabel('Time')
     ax1.set_ylabel('waterlevel [m]')
     ax1.legend(loc='lower right')
     ax1.grid()
     if ts_validation is not None:
         ax2.plot(ts.index[times_id_predinvalidation], ts['values'].iloc[times_id_predinvalidation].values-ts_validation['values'].iloc[times_id_validationinpred].values,'go-',linewidth=size_line_ts,markersize=size_marker_ts, label='difference')
+        ax2.legend(loc='lower right') # create legend only if diff is plotted
     ax2.plot(times_predval_ext,[0,0],'-k',linewidth=size_line_ts)
     ax2.set_ylim(figure_ylim_tsdiff)
     rmse = np.nan
     if ts_validation is not None:
         overlapdiff = ts['values'].iloc[times_id_predinvalidation].values-ts_validation['values'].iloc[times_id_validationinpred].values
         if len(overlapdiff) != 0:
             rmse = np.sqrt(np.nanmean(overlapdiff ** 2))
     ax2.set_ylabel('timeseries difference [m], RMSE = %.5f'%(rmse))
-    ax2.legend(loc='lower right')
     ax2.grid()
     fig.tight_layout()
     
     axs = (ax1,ax2)
     return fig, axs
 
 
-def plot_HWLW_validatestats(ts_ext, ts_ext_validation, create_plot=True):
+def plot_HWLW_validatestats(ts_ext, ts_ext_validation):
     """
     This definition calculates (and plots and prints) some statistics when comparing extreme values.
     This is done by calculating the extreme number (sort of relative to Cadzand 1jan2000, but see 'warning') and subtracting the ts_ext and ts_ext_validation dataframes based on these numbers (and HWLWcode).
     It will only result in values for the overlapping extremes, other values will be NaN and are not considered for the statistics.
     Warning: the calculated extreme numbers in this definition are not corrected for the real phase difference with the M2phasediff argument, the calculated extreme are fine for internal use (to match corresponding extremes) but the absolute number might be incorrect.
 
     Parameters
     ----------
     ts_ext : pandas.DataFrame
         The DataFrame should contain a 'values' and 'HWLW_code' column and a pd.DatetimeIndex as index, it contains the times, values and codes of the timeseries that are extremes.
     ts_ext_validation : pandas.DataFrame
         The DataFrame should contain a 'values' and 'HWLW_code' column and a pd.DatetimeIndex as index, values and codes of the timeseries that are extremes.
-    create_plot : boolean, optional
-        Whether to plot the time/value differences or only print the statistics. The default is True.
 
     Returns
     -------
     fig : matplotlib.figure.Figure
         The generated figure handle, with which the figure can be adapted and saved.
     axs : (tuple of) matplotlib.axes._subplots.AxesSubplot
         The generated axis handle, whith which the figure can be adapted.
 
     """
     
-    print('Calculating comparison statistics for extremes')
+    logger.info('Calculating comparison statistics for extremes')
     if 'HWLWno' not in ts_ext.columns or 'HWLWno' not in ts_ext_validation.columns:
-        print('HWLWno is not present in ts_ext or ts_ext_validation, trying to automatically derive it without M2phasediff argument (this might fail)')
-        try:
-            ts_ext_nrs = calc_HWLWnumbering(ts_ext=ts_ext)
-            ts_ext_validation_nrs = calc_HWLWnumbering(ts_ext=ts_ext_validation)
-        except: #TODO: replace this generic except with specific ones, but first convert 'raise Exception()' in calc_HWLWnumbering() to more specific (maybe custom) ones
-            raise Exception('ERROR: deriving HWLWno failed, so HWLW statistics cannot be calculated. Add HWLWno with calc_HWLWnumbering() before calling plot_HWLW_validatestats().')
-    else:
-        ts_ext_nrs = ts_ext.copy()
-        ts_ext_validation_nrs = ts_ext_validation.copy()
+        logger.info('HWLWno is not present in ts_ext or ts_ext_validation, trying to automatically derive it without M2phasediff argument (this might fail)')
+        ts_ext = calc_HWLWnumbering(ts_ext=ts_ext)
+        ts_ext_validation = calc_HWLWnumbering(ts_ext=ts_ext_validation)
     
     #set HWLWcode and HWLWno as index, to make easy subtraction possible
-    ts_ext_nrs['times'] = ts_ext_nrs.index
-    ts_ext_nrs = ts_ext_nrs.set_index(['HWLWcode','HWLWno'],drop=False)
-    ts_ext_validation_nrs['times'] = ts_ext_validation_nrs.index
-    ts_ext_validation_nrs = ts_ext_validation_nrs.set_index(['HWLWcode','HWLWno'],drop=False)
-    HWLW_diff = ts_ext_nrs.sub(ts_ext_validation_nrs)
+    ts_ext['times'] = ts_ext.index
+    ts_ext = ts_ext.set_index(['HWLWcode','HWLWno'],drop=False)
+    ts_ext_validation['times'] = ts_ext_validation.index
+    ts_ext_validation = ts_ext_validation.set_index(['HWLWcode','HWLWno'],drop=False)
+    HWLW_diff = ts_ext.sub(ts_ext_validation)
     
     tdiff_minutes = HWLW_diff['times'].dt.total_seconds()/60
     vdiff_cm = HWLW_diff['values']*100
-    print('Time differences [minutes]')
-    print('    RMSE: %.2f'%(np.sqrt(np.mean(tdiff_minutes**2))))
-    print('    std: %.2f'%(tdiff_minutes.std()))
-    print('    abs max: %.2f'%(tdiff_minutes.abs().max()))
-    print('    abs mean: %.2f'%(tdiff_minutes.abs().mean()))
-    print('    #NaN: %i of %i'%(tdiff_minutes.isnull().sum(),len(vdiff_cm)))
-    print('Value differences [cm]')
-    print('    RMSE: %.2f'%(np.sqrt(np.mean(vdiff_cm**2))))
-    print('    std: %.2f'%(vdiff_cm.std()))
-    print('    abs max: %.2f'%(vdiff_cm.abs().max()))
-    print('    abs mean: %.2f'%(vdiff_cm.abs().mean()))
-    print('    #NaN: %i of %i'%(vdiff_cm.isnull().sum(),len(vdiff_cm)))
-    
-    if create_plot:
-        fig, ax1 = plt.subplots()
-        ax1.plot(HWLW_diff.loc[1,'times'].dt.total_seconds()/60,HWLW_diff.loc[1,'values']*100,'+',label='HWdiff')
-        ax1.plot(HWLW_diff.loc[2,'times'].dt.total_seconds()/60,HWLW_diff.loc[2,'values']*100,'.',label='LWdiff')
-        ax1.set_xlabel('Time difference [minutes]')
-        ax1.set_ylabel('Value difference [cm]')
-        ax1.legend(loc=1)
-        ax1.grid()
-    
-        axs = (ax1)
-        return fig, axs
+    message = ('Time differences [minutes]\n'
+               f'  RMSE: {(np.sqrt(np.mean(tdiff_minutes**2))):.2f}\n'
+               f'  std: {tdiff_minutes.std():.2f}\n'
+               f'  abs max: {tdiff_minutes.abs().max():.2f}\n'
+               f'  abs mean: {tdiff_minutes.abs().mean():.2f}\n'
+               f'  #NaN: {tdiff_minutes.isnull().sum()} of {len(vdiff_cm)}')
+    logger.info(message)
+    message = ('Value differences [cm]\n'
+               f'  RMSE: {(np.sqrt(np.mean(vdiff_cm**2))):.2f}\n'
+               f'  std: {vdiff_cm.std():.2f}\n'
+               f'  abs max: {vdiff_cm.abs().max():.2f}\n'
+               f'  abs mean: {vdiff_cm.abs().mean():.2f}\n'
+               f'  #NaN: {vdiff_cm.isnull().sum()} of {len(vdiff_cm)}')
+    logger.info(message)
+    
+    fig, ax = plt.subplots()
+    ax.plot(HWLW_diff.loc[1,'times'].dt.total_seconds()/60,HWLW_diff.loc[1,'values']*100,'+',label='HWdiff')
+    ax.plot(HWLW_diff.loc[2,'times'].dt.total_seconds()/60,HWLW_diff.loc[2,'values']*100,'.',label='LWdiff')
+    ax.set_xlabel('Time difference [minutes]')
+    ax.set_ylabel('Value difference [cm]')
+    ax.legend(loc=1)
+    ax.grid()
+
+    return fig, ax
 
 
-def write_tsnetcdf(ts, station, vertref, filename, ts_ext=None, tzone_hr=1, nosidx=False, mode='w'):
+def write_netcdf(ts, filename, ts_ext=None, nosidx=False, mode='w'):
     """
     Writes the timeseries to a netCDF file
 
     Parameters
     ----------
     ts : pandas.DataFrame
         The DataFrame should contain a 'values' column and a pd.DatetimeIndex as index, it contains the timeseries.
@@ -617,14 +593,25 @@
     None.
     
     """
     
     import hatyan
     version_no = hatyan.__version__
     
+    # get metadata from ts dataframe
+    metadata_ts = metadata_from_obj(ts)
+    station = metadata_ts.pop("station")
+    vertref = metadata_ts.pop("vertref")
+    if ts_ext is not None:
+        metadata_ext = metadata_from_obj(ts_ext)
+        station_ext = metadata_ext.pop("station")
+        vertref_ext = metadata_ext.pop("vertref")
+        assert station==station_ext
+        assert vertref==vertref_ext
+    
     times_all = ts.index
     timeseries = ts['values']
     times_stepmin = (ts.index[1]-ts.index[0]).total_seconds()/60
     dt_analysistime = dt.datetime.now()
     data_nc = Dataset(filename, mode, format="NETCDF3_CLASSIC")
     attr_dict = {'title': 'tidal prediction for %s to %s'%(times_all[0].strftime('%Y-%m-%d %H:%M:%S'), times_all[-1].strftime('%Y-%m-%d %H:%M:%S')),
                  'institution': 'Rijkswaterstaat',
@@ -641,15 +628,15 @@
     if 'statname_len' not in ncdimlist:
         data_nc.createDimension('statname_len',statname_len)
     if 'time' not in ncdimlist:
         data_nc.createDimension('time',len(times_all.tolist()))
     if 'analysis_time' not in ncdimlist:
         data_nc.createDimension('analysis_time',1)
     
-    refdate_tz = dt.datetime(1900,1,1,tzinfo=dt.timezone(dt.timedelta(hours=tzone_hr)))
+    refdate_tz = dt.datetime(1900,1,1,tzinfo=ts.index.tz)
     dict_statattr = {'cf_role': 'timeseries_id'}
     dict_anatimattr = {'units': 'minutes since %s'%(refdate_tz.strftime('%Y-%m-%d %H:%M:%S %z')), 'standard_name':'forecast_reference_time', 'long_name':'forecast_reference_time'}
     dict_timattr = {'units': 'minutes since %s'%(refdate_tz.strftime('%Y-%m-%d %H:%M:%S %z'))}
     dict_wlattr = {'units':'m', 'vertical_reference': vertref, 'standard_name': 'sea_surface_height_above_geopotential_datum', 'long_name': 'astronomical prediction of water level above reference level'}
     dict_HWattr = {'units':'m', 'vertical_reference': vertref, 'standard_name': 'sea_surface_height_above_geopotential_datum', 'long_name': 'astronomical prediction of high water extremes above reference level'}
     dict_LWattr = {'units':'m', 'vertical_reference': vertref, 'standard_name': 'sea_surface_height_above_geopotential_datum', 'long_name': 'astronomical prediction of low water extremes above reference level'}
     dict_HWLWnoattr = {'units':'n-th tidal wave since reference wave at Cadzand on 1-1-2000'} #, 'standard_name': '', 'long_name': ''}
@@ -676,15 +663,15 @@
         data_nc.variables['time'][:] = date2num(times_all.tolist(),units=data_nc.variables['time'].units)
     if 'waterlevel_astro' not in ncvarlist:
         nc_newvar = data_nc.createVariable('waterlevel_astro','f8',('stations','time',))
         nc_newvar.setncatts(dict_wlattr)
     data_nc.variables['waterlevel_astro'][nstat,:] = timeseries
     
     if ts_ext is None:
-        print('no HWLW prediction written')
+        logger.info('no HWLW prediction written')
         data_nc.close()
         return #this skips the HWLW part of the definition
     
     #HWLW prediction
     if nosidx:
         #convert index from time to HWLWno
         data_HWLW_nosidx = ts_ext.copy()
@@ -766,22 +753,26 @@
                 #nc_newvar.setncatts(dict_LWattr)
             data_nc.variables['waterlevel_astro_LW_numbers'][nstat,:] = data_LW['HWLWno']
     
     data_nc.close()
     return
 
 
-def write_tsdia(ts, station, vertref, filename, headerformat='dia'):
+def write_dia(ts, filename, headerformat='dia'):
     """
-    Writes the timeseries to an equidistant dia file
+    Writes the timeseries to an equidistant dia file or the extremes to 
+    a non-equidistant dia file. This is only supported 
+    for timeseries with a UTC+1 timestamp, since DONAR (and therefore dia)
+    data is always in UTC+1 (MET/CET), also during summertime periods.
 
     Parameters
     ----------
     ts : pandas.DataFrame
-        The DataFrame should contain a 'values' column and a pd.DatetimeIndex as index, it contains the timeseries.
+        The DataFrame should contain a 'values' column and a pd.DatetimeIndex as index, it contains the timeseries. 
+        In case of extremes, the DataFrame should also contain a 'HWLW_code' column.
     station : TYPE
         DESCRIPTION.
     vertref : TYPE
         DESCRIPTION.
     filename : TYPE
         DESCRIPTION.
 
@@ -791,24 +782,43 @@
         DESCRIPTION.
 
     Returns
     -------
     None.
 
     """
+    if "HWLWcode" in ts.columns:
+        write_dia_HWLW(ts_ext=ts, filename=filename, headerformat=headerformat)
+    else:
+        write_dia_ts(ts=ts, filename=filename, headerformat=headerformat)
+
+    
+def write_dia_ts(ts, filename, headerformat='dia'):
+    if "HWLWcode" in ts.columns:
+        raise TypeError("a timeseries with extremes (HWLW) was passed to write_dia, use `write_dia_HWLW()` instead")
+    metadata = metadata_from_obj(ts)
+    waarnemingssoort = wns_from_metadata(metadata)
+    vertref = metadata['vertref']
+    station = metadata['station']
+    quantity = metadata['grootheid']
+    if quantity != 'WATHTBRKD': #TODO: remove this after hardcoding in this function is fixed
+        raise ValueError(f'write_dia() expects quantity WATHTBRKD, but {quantity} was provided.')
+    tzone = ts.index.tz
+    if tzone != pytz.FixedOffset(60):
+        raise ValueError(f'write_dia() expects tzone pytz.FixedOffset(60) (since tzone is not defined in dia-header), but {tzone} was provided.')
     
     if vertref == 'NAP':
-        waarnemingssoort = 18
         vertreflong = 'T.o.v. Normaal Amsterdams Peil'
     elif vertref == 'MSL':
-        waarnemingssoort = 55
         vertreflong = 'T.o.v. Mean Sea Level'
     else:
         raise Exception('ERROR: currently only vertref="NAP" and vertref="MSL" are supported for writing diafiles')
+    
     grootheid = 'WATHTBRKD;Waterhoogte berekend;J'
+
     ana = 'F012;Waterhoogte astronomisch mbv harmonische analyse' #TODO: dit is niet per se generiek geldig, alleen in getijpredictieproces RWS
     
     time_today = dt.datetime.today().strftime('%Y%m%d')
     tstart_str = ts.index[0].strftime('%Y%m%d;%H%M')
     tstop_str = ts.index[-1].strftime('%Y%m%d;%H%M')
     timestep_min = (ts.index[1]-ts.index[0]).total_seconds()/60
     
@@ -865,46 +875,31 @@
     
     with io.open(filename,'w', newline='\n') as f: #open file and set linux newline style
         for metaline in metadata_pd:
             f.write('%s\n'%(metaline))
         data_todia.to_csv(f,index=False,header=False)
 
 
-def write_tsdia_HWLW(ts_ext, station, vertref, filename, headerformat='dia'):
-    """
-    writes the extremes timeseries to a non-equidistant dia file
-
-    Parameters
-    ----------
-    ts_ext : pandas.DataFrame
-        The DataFrame should contain a 'values' and 'HWLW_code' column and a pd.DatetimeIndex as index, it contains the times, values and codes of the timeseries that are extremes.
-    station : TYPE
-        DESCRIPTION.
-    vertref : TYPE
-        DESCRIPTION.
-    filename : TYPE
-        DESCRIPTION.
-
-    Raises
-    ------
-    Exception
-        DESCRIPTION.
-
-    Returns
-    -------
-    None.
-
-    """
+def write_dia_HWLW(ts_ext, filename, headerformat='dia'):
+    
+    metadata = metadata_from_obj(ts_ext)
+    waarnemingssoort = wns_from_metadata(metadata)
+    vertref = metadata['vertref']
+    station = metadata['station']
+    quantity = metadata['grootheid']
+    if quantity != 'WATHTBRKD': #TODO: remove this after hardcoding in this function is fixed
+        raise ValueError(f'write_dia() expects quantity WATHTBRKD, but {quantity} was provided.')
+    tzone = ts_ext.index.tz
+    if tzone != pytz.FixedOffset(60):
+        raise ValueError(f'write_dia() expects tzone pytz.FixedOffset(60) (since tzone is not defined in dia-header), but {tzone} was provided.')
     
     if vertref == 'NAP':
-        waarnemingssoort = 18
         vertreflong = 'T.o.v. Normaal Amsterdams Peil'
         parameterX = 'GETETBRKD2;Getijextreem berekend'
     elif vertref == 'MSL':
-        waarnemingssoort = 55
         vertreflong = 'T.o.v. Mean Sea Level'
         parameterX = 'GETETBRKDMSL2;Getijextreem berekend t.o.v. MSL'
     else:
         raise Exception('ERROR: currently only vertref="NAP" and vertref="MSL" are supported for writing diafiles')
     grootheid = 'WATHTBRKD;Waterhoogte berekend;J'
     ana = 'F012;Waterhoogte astronomisch mbv harmonische analyse' #HW en LW uit 1 min. waterhoogten gefilterd uit 10 min. gem.  #TODO: dit is niet per se generiek geldig, alleen in getijpredictieproces RWS
     time_today = dt.datetime.today().strftime('%Y%m%d')
@@ -979,15 +974,15 @@
 
     with io.open(filename,'w', newline='\n') as f: #open file and set linux newline style
         for metaline in metadata_pd:
             f.write('%s\n'%(metaline))
         data_todia.to_csv(f,index=False,header=False)
 
 
-def writets_noos(ts, filename, metadata=None):
+def write_noos(ts, filename):
     """
     Writes the timeseries to a noos file
 
     Parameters
     ----------
     ts : pandas.DataFrame
         The DataFrame should contain a 'values' column and a pd.DatetimeIndex as index, it contains the timeseries.
@@ -996,14 +991,16 @@
 
     Returns
     -------
     None.
 
     """
     
+    metadata = ts.attrs
+    
     timestamp = dt.datetime.now().strftime('%c')
     ts_out = pd.DataFrame({'times':ts.index.strftime('%Y%m%d%H%M'),'values':ts['values']})
     
     if metadata is None:
         header_txt = f"""------------------------------------------------------
         Timeseries written by hatyan
         Created at {timestamp}
@@ -1019,51 +1016,57 @@
         header_txt = f"""------------------------------------------------------\nTimeseries written by hatyan\nCreated at {timestamp}\n------------------------------------------------------\n"""
         for key in metadata.keys():
             header_txt = header_txt+('%-12s: %s\n'%(key, metadata[key]))
         header_txt = header_txt+'------------------------------------------------------'
     np.savetxt(filename,ts_out,fmt='%s %7.4f',header=header_txt)
 
 
-def crop_timeseries(ts, times_ext, onlyfull=True):
+def crop_timeseries(ts, times, onlyfull=True):
     """
     Crops the provided timeseries
 
     Parameters
     ----------
     ts : pandas.DataFrame
         The DataFrame should contain a 'values' column and a pd.DatetimeIndex as index, it contains the timeseries.
-    times_ext : TYPE
-        DESCRIPTION.
+    times : slice
+        slice(tstart,tstop).
 
     Raises
     ------
     Exception
         DESCRIPTION.
 
     Returns
     -------
     ts_pd_out : TYPE
         DESCRIPTION.
 
     """
     ts_pd_in = ts
+    tstart = pd.Timestamp(times.start)
+    tstop = pd.Timestamp(times.stop)
     
-    print('cropping timeseries')
-    if not times_ext[0]<times_ext[1]:
-        raise Exception('ERROR: the two times times_ext should be increasing, but they are not: %s.'%(times_ext))
-    if (times_ext[0] < ts_pd_in.index.min()) or (times_ext[-1] > ts_pd_in.index.max()):
-        message = 'imported timeseries is not available within entire requested period:\nrequested period:    %s to %s\nimported timeseries: %s to %s'%(times_ext[0],times_ext[-1],ts_pd_in.index[0],ts_pd_in.index[-1])
+    logger.info('cropping timeseries')
+    if tstart >= tstop:
+        raise ValueError(f'the tstart and tstop should be increasing, but they are not: {times}.')
+    if (tstart < ts_pd_in.index.min()) or (tstop > ts_pd_in.index.max()):
+        message = 'imported timeseries is not available within entire requested period:\nrequested period:    %s to %s\nimported timeseries: %s to %s'%(tstart,tstop,ts_pd_in.index[0],ts_pd_in.index[-1])
         if onlyfull:
-            raise Exception('ERROR: %s'%(message))
+            raise Exception(message)
         else:
-            print('WARNING: %s'%(message))
+            logger.warning(message)
             
-    #times_selected_bool = (ts_pd_in.index >= times_ext[0]) & (ts_pd_in.index <= times_ext[-1])
-    #ts_pd_out = ts_pd_in.loc[times_selected_bool]
-    ts_pd_out = ts_pd_in.loc[times_ext[0]:times_ext[1]]
+    ts_pd_out = ts_pd_in.loc[tstart:tstop]
+    
+    # add metadata
+    metadata = metadata_from_obj(ts)
+    metadata['tstart'] = pd.Timestamp(tstart)
+    metadata['tstop'] = pd.Timestamp(tstop)
+    ts_pd_out = metadata_add_to_obj(ts_pd_out,metadata)
     
     return ts_pd_out
 
 
 def resample_timeseries(ts, timestep_min, tstart=None, tstop=None):
     """
     resamples the provided timeseries, only overlapping timesteps are selected, so no interpolation. with tstart/tstop it is possible to extend the timeseries with NaN values.
@@ -1082,44 +1085,54 @@
     Returns
     -------
     data_pd_resample : pandas.DataFrame with a 'values' column and a pd.DatetimeIndex as index
         the resampled timeseries.
 
     """
     
-    print('resampling timeseries to %i minutes'%(timestep_min))
+    logger.info(f'resampling timeseries to {timestep_min} minutes')
     
     bool_duplicated_index = ts.index.duplicated()
     if bool_duplicated_index.sum()>0:
         raise Exception('there are duplicated values in the ts DatetimeIndex, this is not supported by Timeseries.resample_timeseries(). Try "ts_nodupl = ts[~ts.index.duplicated()]"')
     
     if tstart is None:
         tstart = ts.index[0]
     if tstop is None:
         tstop = ts.index[-1]
     data_pd_resample = pd.DataFrame({},index=pd.date_range(tstart,tstop,freq='%dmin'%(timestep_min))) #generate timeseries with correct tstart/tstop and interval
     data_pd_resample['values'] = ts['values'] #put measurements into this timeseries, matches to correct index automatically
     
+    # add metadata
+    metadata = metadata_from_obj(ts)
+    metadata['tstart'] = pd.Timestamp(tstart)
+    metadata['tstop'] = pd.Timestamp(tstop)
+    metadata['timestep_min'] = timestep_min
+    data_pd_resample = metadata_add_to_obj(data_pd_resample,metadata)
+    
     return data_pd_resample
 
 
 def nyquist_folding(ts_pd,t_const_freq_pd):
     #deriving dominant timestep, sampling frequency and nyquist frequency
     timestep_hr_all = ((ts_pd.index[1:]-ts_pd.index[:-1]).total_seconds()/3600)#.astype(int).values
     uniq_vals, uniq_counts = np.unique(timestep_hr_all,return_counts=True)
     timestep_hr_dominant = uniq_vals[np.argmax(uniq_counts)]
     fs_phr = 1/timestep_hr_dominant #sampling freq [1/hr]
     fn_phr = fs_phr/2 #nyquist freq [1/hr]
     
     #check if there is a component with exactly the same frequency as the nyquist frequency #TODO: or its multiples (but with remainder, A0 also gets flagged)
     bool_isnyquist = t_const_freq_pd['freq']==fn_phr
     if bool_isnyquist.any():
-        raise Exception(f'there is a component on the Nyquist frequency ({fn_phr} [1/hr]), this not possible:\n{t_const_freq_pd.loc[bool_isnyquist]}')
+        raise ValueError(f'there is a component on the Nyquist frequency ({fn_phr} [1/hr]), '
+                        f'this not possible:\n{t_const_freq_pd.loc[bool_isnyquist]}')
     
-    print(f'folding frequencies over Nyquist frequency, which is half of the dominant timestep ({timestep_hr_dominant} hour), there are {len(uniq_counts)} unique timesteps)')
+    logger.info('folding frequencies over Nyquist frequency, which is half '
+                f'of the dominant timestep ({timestep_hr_dominant} hour), '
+                f'there are {len(uniq_counts)} unique timesteps)')
     #folding frequencies over nyquist frequency: https://users.encs.concordia.ca/~kadem/CHAPTER%20V.pdf (fig 5.6)
     freq_div,freq_rem = np.divmod(t_const_freq_pd[['freq']],fn_phr) # remainder gives folded frequencies for even divisions (freqs for odd divisions are not valid yet)
     freq_div_isodd = (freq_div%2).astype(bool)
     freq_rem[freq_div_isodd] = fn_phr-freq_rem[freq_div_isodd] # fn-remainder gives folded frequencies for odd divisions
     return freq_rem
 
 
@@ -1146,52 +1159,46 @@
         return #Rayleigh check is only relevant (and possible) if there more than one non-A0 component, otherwise stop.
     freq_diffs = np.diff(t_const_freq)
     ts_period_hr = (ts_pd.index.max()-ts_pd.index.min()).total_seconds()/3600
     rayleigh_tresh = 0.7 #0.99 # Koos Doekes: "Bij het algoritme dat HATYAN gebruikt mag men in de praktijk het Rayleigh-criterium enigszins schenden, tot zo'n 0,7 van de theoretisch vereiste reekslengte. "
     rayleigh = ts_period_hr*freq_diffs #TODO: might be better to drop timeseries nan-values first, especially from start/end of series since it decreases ts_period_hr
     freq_diff_phr_minimum = rayleigh_tresh/ts_period_hr
     rayleigh_bool = rayleigh>rayleigh_tresh
-    rayleigh_bool_id = np.where(~rayleigh_bool)[0]
+    rayleigh_bool_id = np.nonzero(~rayleigh_bool)[0]
     
     if rayleigh_bool.all():
-        print('Rayleigh criterion OK (always>%.2f, minimum is %.2f)'%(rayleigh_tresh, np.min(rayleigh)))
-        print('Frequencies are far enough apart (always >%.6f, minimum is %.6f)'%(freq_diff_phr_minimum,np.min(freq_diffs)))
+        logger.info('Rayleigh criterion OK (always>%.2f, minimum is %.2f)'%(rayleigh_tresh, np.min(rayleigh)))
+        logger.info('Frequencies are far enough apart (always >%.6f, minimum is %.6f)'%(freq_diff_phr_minimum,np.min(freq_diffs)))
     else:
-        print('Rayleigh criterion vandalised (not always>%.2f, minimum is %.2f)'%(rayleigh_tresh, np.min(rayleigh)))
-        print('Frequencies with not enough difference (not always >%.6f, minimum is %.6f)'%(freq_diff_phr_minimum,np.min(freq_diffs)))
+        logger.info('Rayleigh criterion vandalised (not always>%.2f, minimum is %.2f)'%(rayleigh_tresh, np.min(rayleigh)))
+        logger.info('Frequencies with not enough difference (not always >%.6f, minimum is %.6f)'%(freq_diff_phr_minimum,np.min(freq_diffs)))
         for ray_id in rayleigh_bool_id:
             t_const_freq_sel = t_const_freq.iloc[[ray_id,ray_id+1]]
             t_const_freq_sel['diff'] = np.diff(t_const_freq_sel.values)[0]
             t_const_freq_sel['ndays min'] = rayleigh_tresh/np.diff(t_const_freq_sel.values)[0]/24
-            print(t_const_freq_sel)
+            logger.info(t_const_freq_sel)
             if t_const_freq_sel['diff'] < 1e-9:
-                print(f'WARNING: frequency difference between {t_const_freq_sel.index[0]} and {t_const_freq_sel.index[1]} almost zero, will result in ill conditioned matrix')
-        
+                logger.warning(f'frequency difference between {t_const_freq_sel.index[0]} and {t_const_freq_sel.index[1]} almost zero, will result in ill conditioned matrix')
+
 
-def check_ts(ts):
+class Timeseries_Statistics:
     """
     returns several statistics of the provided timeseries as a Timeseries_Statistics class, which is a like a dict that pretty prints automatically.
 
     Parameters
     ----------
     ts : pandas.DataFrame
         The DataFrame should contain a 'values' column and a pd.DatetimeIndex as index, it contains the timeseries to be checked.
 
     Returns
     -------
     stats: class Timeseries_Statistics
         Timeseries_Statistics is a like a dict that pretty prints automatically.
 
     """
-    
-    stats = Timeseries_Statistics(ts=ts)
-    return stats
-
-
-class Timeseries_Statistics:
     #TODO: make like a dict with different __str__ method, instead of this mess https://stackoverflow.com/questions/4014621/a-python-class-that-acts-like-dict
     #TODO: improve output dict, keys are now not convenient to use. Maybe make keys and longname?
     def __init__(self,ts):
         timesteps_min_all = ts.index.to_series().diff()[1:].dt.total_seconds()/60
         bool_int = np.abs(timesteps_min_all-timesteps_min_all.round(0))<1e-9
         if bool_int.all():
             timesteps_min_all = timesteps_min_all.astype(int)
@@ -1247,14 +1254,36 @@
     
     
 ###############################
 ################# READING FILES
 ###############################
 
 
+def get_diaxycoords(filename, crs):
+    diablocks_pd_extra = get_diablocks(filename=filename)
+    dia_x = diablocks_pd_extra['x'].values
+    dia_y = diablocks_pd_extra['y'].values
+    dia_epsg = diablocks_pd_extra['epsg'].astype(int).values
+    
+    # check if all epsg codes are the same
+    if not (dia_epsg==dia_epsg[0]).all():
+        raise ValueError(f"The diafile contains multiple EPSG codes, not supported yet: {dia_epsg}")
+    dia_epsg = dia_epsg[0]
+    
+    if len(dia_x)==1:
+        # to avoid DeprecationWarning: Conversion of an array with ndim > 0 to a scalar is deprecated, and will error in future.
+        dia_x = dia_x[0]
+        dia_y = dia_y[0]
+    
+    transformer = Transformer.from_crs(f'epsg:{dia_epsg}', f'epsg:{crs}', always_xy=True)
+    stat_x, stat_y = transformer.transform(dia_x, dia_y)
+    
+    return stat_x, stat_y
+
+
 def get_diablocks_startstopstation(filename):
     """
     Gets information about the data blocks present in a dia file
 
     Parameters
     ----------
     filename : TYPE
@@ -1272,14 +1301,17 @@
 
     """
     
     #get list of starts/ends of datasets in diafile
     linenum_colnames = ['block_starts','data_starts','data_ends']
     diablocks_pd_startstopstation = pd.DataFrame({},columns=linenum_colnames)
     
+    # add str type columns to avoid "FutureWarning: Setting an item of incompatible dtype is deprecated and will raise in a future error of pandas. Value 'min' has dtype incompatible with float64, please explicitly cast to a compatible dtype first."
+    diablocks_pd_startstopstation['station'] = ""
+    
     with open(filename, encoding='latin1') as f: #'latin1 is nodig om predictie diafile die rechtstreeks uit hatyan komen in te lezen (validatietijdserie met op regel 4 (PAR) ongeldige tekens aan het einde)
         block_id = -1
         for linenum, line in enumerate(f, 1):
             if '[W3H]' in line:
                 block_id += 1
                 diablocks_pd_startstopstation.loc[block_id,'block_starts'] = linenum
             elif '[WRD]' in line:
@@ -1296,16 +1328,22 @@
     diablocks_pd_startstopstation[linenum_colnames] = diablocks_pd_startstopstation[linenum_colnames].astype(int)
     
     return diablocks_pd_startstopstation
 
 
 def get_diablocks(filename):
     
-    print('reading file: %s'%(filename))
+    logger.info('reading file: %s'%(filename))
     diablocks_pd = get_diablocks_startstopstation(filename)
+    # add str type columns to avoid "FutureWarning: Setting an item of incompatible dtype is deprecated and will raise in a future error of pandas. Value 'min' has dtype incompatible with float64, please explicitly cast to a compatible dtype first."
+    columns_str = ['TYP','groepering','grootheid','coordsys',
+                   'eenheid','vertref',
+                   'timestep_unit',
+                   'STA']
+    diablocks_pd[columns_str] = ""
     for block_id in diablocks_pd.index.tolist():
         #read diafile metadata as pandas series, prevent splitting of combined paramater names like MXH;2 by replacing ; with !
         data_meta_nrows = diablocks_pd.loc[block_id,'data_starts'] - diablocks_pd.loc[block_id,'block_starts']
         data_meta_series = pd.read_table(filename,skiprows=diablocks_pd.loc[block_id,'block_starts'],nrows=data_meta_nrows,header=None)[0] #series of metadata
         if not data_meta_series.str.contains('GHD|MXG;2').any(): #wia files contain these parameters, dia files don't. Replace dia names with wia names (wia files also contain PAR and MXP;2, but they should not be replaced)
             data_meta_series = data_meta_series.str.replace('PAR','GHD').str.replace('MXP;2','MXG;2')
         bool_combinedparname = (data_meta_series.str[3:6]==';1;') | (data_meta_series.str[3:6]==';2;')
@@ -1317,18 +1355,18 @@
         diablocks_pd.loc[block_id,'TYP'] = row_TYP
         if row_TYP=='TN': #bool_startswithmux.any(): #extreme waterlevel timeseries (non-equidistant)
             mincontent = ['MXG;2','LOC','MXH;2','MXE;2','TYD','STA']
             if bool_startswithmux.sum()==0:
                 raise Exception(f'ERROR: block_id={block_id} is of TYP={row_TYP} (non-equidistant, extreme waterlevels), but no MUX is available in metadata header so the file cannot be read:\n{diablocks_pd}')
             diablocks_pd.loc[block_id,'groepering'] = data_meta_series.loc[bool_startswithmux].iloc[0].split(';')[1]
         elif row_TYP=='TE': #normal waterlevel timeseries (equidistant)
-            mincontent = ['GHD',  'LOC','HDH',  'EHD',  'TYD','STA'] #WNS,CPM,HDH,ANA
+            mincontent = ['GHD',  'LOC','HDH',  'EHD',  'TYD','STA'] #,WNSCPM,HDH,ANA
             diablocks_pd.loc[block_id,'groepering'] = 'NVT'
         else:
-            raise Exception(f'TYP "{row_TYP}" not implemented in hatyan.readts_dia()')
+            raise Exception(f'TYP "{row_TYP}" not implemented in hatyan.read_dia()')
         
         #read all required metadata
         for get_content_sel in mincontent:
             bool_mincontent = data_meta_series.str.replace('!',';').str.startswith(get_content_sel)
             if bool_mincontent.sum()!=1:
                 if get_content_sel!='STA':
                     raise Exception(f'unexpected amount of matched metadatalines ({bool_mincontent.sum()}) for {get_content_sel}')
@@ -1338,15 +1376,15 @@
                 valid_grootheidnames = ['WATHTE','WATHTBRKD','NVT'] #NVT in wia files
                 if file_grootheidname not in valid_grootheidnames:
                     raise Exception('ERROR: grootheid name (%s) should be in %s but is %s'%(get_content_sel, valid_grootheidnames, file_grootheidname))
                 diablocks_pd.loc[block_id,'grootheid'] = file_grootheidname
             elif get_content_sel in ['LOC']: # Locatie. same in all files
                 coords_pd = pd.DataFrame({'epsg_in':[28992,4326,4230], 'factor':[100,1000000,1000000]}, index=['RD','W84','E50'])
                 if len(data_meta_mincontent)<7:
-                    print('no coordinate data available in LOC line of dia file')
+                    logger.warning('no coordinate data available in LOC line of dia file')
                     continue
                 coordsys_str, coord_x, coord_y = data_meta_mincontent[4:]
                 if coordsys_str not in coords_pd.index:
                     raise Exception('unknown coordinate system string in diafile ({coordsys_str})')
                 diablocks_pd.loc[block_id,'x'] = int(coord_x)/coords_pd.loc[coordsys_str,'factor']
                 diablocks_pd.loc[block_id,'y'] = int(coord_y)/coords_pd.loc[coordsys_str,'factor']
                 diablocks_pd.loc[block_id,'coordsys'] = coordsys_str
@@ -1358,36 +1396,43 @@
                 diablocks_pd.loc[block_id,'eenheid'] = file_eenheid
             elif get_content_sel in ['HDH','MXH;2']: # Hoedanigheid (NAP/MSL). equidistant dia/wia, non-equidistant dia/wia
                 diablocks_pd.loc[block_id,'vertref'] = data_meta_mincontent[1]
             elif get_content_sel in ['TYD']: #Tijdstip. same in all files
                 datestart = dt.datetime.strptime(data_meta_mincontent[1]+data_meta_mincontent[2], "%Y%m%d%H%M")
                 datestop = dt.datetime.strptime(data_meta_mincontent[3]+data_meta_mincontent[4], "%Y%m%d%H%M")
                 if len(data_meta_mincontent)==5: #nonequidistant timeseries
-                    timestep_value = None
-                    timestep_unit = None
+                    timestep_value = np.nan #TODO: None is supported by pandas 2.1.2 and maybe earlier versions, but not 2.0.3 (py39 only)
+                    timestep_unit = np.nan
                 elif len(data_meta_mincontent)==7: #equidistant timeseries contains also timeunit and timestep
                     timestep_unit = data_meta_mincontent[6]
                     if timestep_unit not in ['min','cs']: #minutes and 1/100 sec
                         raise Exception(f'ERROR: time unit from TYD is in unknown format (not "min" or "cs"): {timestep_unit}')
-                    timestep_value = int(data_meta_mincontent[5]) #int(timestep_value_raw)
+                    timestep_value = int(data_meta_mincontent[5])
                 else:
                     raise Exception(f'ERROR: time metadata is not understood: {data_meta_mincontent}')
                 diablocks_pd.loc[block_id,'tstart'] = datestart
                 diablocks_pd.loc[block_id,'tstop'] = datestop
                 diablocks_pd.loc[block_id,'timestep_min'] = timestep_value
                 diablocks_pd.loc[block_id,'timestep_unit'] = timestep_unit
             elif get_content_sel in ['STA']: #Status. same in all files
                 diablocks_pd.loc[block_id,'STA'] = '!'.join(data_meta_series.loc[bool_mincontent].tolist())
     return diablocks_pd
 
 
-def readts_dia_nonequidistant(filename, diablocks_pd, block_id):
+def read_dia_nonequidistant(filename, diablocks_pd, block_id):
 
     data_nrows = diablocks_pd.loc[block_id,'data_ends'] - diablocks_pd.loc[block_id,'data_starts']
-    data_pd_HWLW = pd.read_csv(filename,skiprows=diablocks_pd.loc[block_id,'data_starts'],nrows=data_nrows, header=None, names=['date','time','HWLWcode/qualitycode','valuecm:'], sep=';', parse_dates={'times':[0,1]})
+    skiprows = diablocks_pd.loc[block_id,'data_starts']
+    data_pd_HWLW = pd.read_csv(filename, skiprows=skiprows,nrows=data_nrows, header=None, sep=';',
+                               names=['date','time','HWLWcode/qualitycode','valuecm:'], 
+                               dtype={'date':str,'time':str},
+                               )
+    dates_pd = data_pd_HWLW.pop('date')
+    times_pd = data_pd_HWLW.pop('time')
+    data_pd_HWLW['times'] = pd.to_datetime(dates_pd+times_pd)
     
     #convert HWLW+quality code to separate columns
     data_pd_HWLWtemp = data_pd_HWLW.loc[:,'HWLWcode/qualitycode'].str.split('/', expand=True)
     data_pd_HWLW['HWLWcode'] = data_pd_HWLWtemp.iloc[:,0].astype('int')
     data_pd_HWLW['qualitycode'] = data_pd_HWLWtemp.iloc[:,1].astype('int')
     data_pd_HWLW = data_pd_HWLW.drop('HWLWcode/qualitycode',axis='columns')
 
@@ -1396,154 +1441,172 @@
     data_pd_HWLW = data_pd_HWLW.drop('valuecm:',axis='columns')
     
     bool_hiaat = data_pd_HWLW['qualitycode'] == 99
     data_pd_HWLW.loc[bool_hiaat,'values'] = np.nan
     
     data_pd = data_pd_HWLW
     data_pd = data_pd.set_index('times')
+    data_pd.index = data_pd.index.tz_localize(pytz.FixedOffset(60))
+    
+    # add metadata
+    metadata = metadata_from_diablocks(diablocks_pd, block_id)
+    data_pd = metadata_add_to_obj(data_pd,metadata)
     
     return data_pd
 
 
-def readts_dia_equidistant(filename, diablocks_pd, block_id):
+def read_dia_equidistant(filename, diablocks_pd, block_id):
     
     datestart = diablocks_pd.loc[block_id,'tstart']
     datestop = diablocks_pd.loc[block_id,'tstop']
     timestep_min = diablocks_pd.loc[block_id,'timestep_min']
     timestep_unit = diablocks_pd.loc[block_id,'timestep_unit']
+    tzone = pytz.FixedOffset(60)
     if timestep_unit=='min':
-        times_fromfile = pd.date_range(start=datestart,end=datestop,freq='%dmin'%(timestep_min))
+        times_fromfile = pd.date_range(start=datestart,end=datestop,freq='%dmin'%(timestep_min), tz=tzone)
     else:
-        times_fromfile = pd.date_range(start=datestart,end=datestop,freq=f'{timestep_min*10000000} ns')
+        times_fromfile = pd.date_range(start=datestart,end=datestop,freq=f'{timestep_min*10000000} ns', tz=tzone)
     
-    #get data for station
+    # get data for station
     data_nrows = diablocks_pd.loc[block_id,'data_ends'] - diablocks_pd.loc[block_id,'data_starts']
     data_pd = pd.read_csv(filename,skiprows=diablocks_pd.loc[block_id,'data_starts'],nrows=data_nrows, header=None)
     data_pdser = data_pd[0].str.strip()
     data = data_pdser.str.cat()
     data = data.strip(':') #remove first and/or last colon if present
     data = data.split(':')
     
     if len(times_fromfile) != len(data):
         raise Exception(f'ERROR: times and values for block_id={block_id} are not of equal length\nlen(times_fromfile): %d\nlen(data): %d'%(len(times_fromfile),len(data)))
-    data_pd = pd.DataFrame({'times':times_fromfile,'valuecm/qualitycode':data})
     
-    #convert HWLW+quality code to separate columns
+    # construct pandas dataframe (has equidistant index, so has freq property)
+    data_pd = pd.DataFrame({'valuecm/qualitycode':data},index=times_fromfile)
+    data_pd.index.name = 'times'
+    
+    # convert HWLW+quality code to separate columns
     data_pd_temp = data_pd.loc[:,'valuecm/qualitycode'].str.split('/', expand=True)
     data_pd['values'] = data_pd_temp.iloc[:,0].astype('int')/100
     data_pd['qualitycode'] = data_pd_temp.iloc[:,1].astype('int')
     data_pd = data_pd.drop('valuecm/qualitycode',axis='columns')
-
+    
+    # replace missing values with nan
     bool_hiaat = data_pd['qualitycode'] == 99
     data_pd.loc[bool_hiaat,'values'] = np.nan
-    data_pd = data_pd.set_index('times')
     
+    # add metadata
+    metadata = metadata_from_diablocks(diablocks_pd, block_id)
+    data_pd = metadata_add_to_obj(data_pd,metadata)
     return data_pd
 
 
-def readts_dia(filename, station=None, block_ids=None, get_status=False, allow_duplicates=False):
+def read_dia(filename, station=None, block_ids=None, allow_duplicates=False):
     """
     Reads an equidistant or non-equidistant dia file, or a list of dia files. Also works for diafiles containing multiple blocks for one station.
 
     Parameters
     ----------
     filename : TYPE
         DESCRIPTION.
     station : TYPE
         DESCRIPTION. The default is None.
     block_ids : int, list of int or 'allstation', optional
         DESCRIPTION. The default is None.
 
-    Raises
-    ------
-    Exception
-        DESCRIPTION.
-
     Returns
     -------
     data_pd : pandas.core.frame.DataFrame
         DataFrame with a 'values' column and a pd.DatetimeIndex as index in case of an equidistant file, or more columns in case of a non-equidistant file.
 
     """
     
     if not isinstance(filename,list):
-        filename = [filename]
+        # solve wildcards and convert to list
+        filename = glob.glob(filename)
+        filename.sort()
+    
     if len(filename)==0:
-        raise Exception('ERROR: filename list is empty')
+        raise FileNotFoundError('Filename list is empty')
     
-    data_pd_all = pd.DataFrame()
-    for iF, filename_one in enumerate(filename):    
+    data_pd_list = []
+    metadata_list = []
+    for filename_one in filename:    
         diablocks_pd = get_diablocks(filename_one)
         pd.set_option('display.max_columns', 6) #default was 0, but need more to display groepering
         pd.set_option('display.width', 200) #default was 80, but need more to display groepering
         print_cols = ['block_starts', 'station', 'grootheid', 'groepering', 'tstart', 'tstop']
-        print('blocks in diafile:\n%s'%(diablocks_pd[print_cols]))
+        logger.info('blocks in diafile:\n%s'%(diablocks_pd[print_cols]))
         str_getdiablockspd = 'A summary of the available blocks is printed above, obtain a full DataFrame of available diablocks with "diablocks_pd=hatyan.get_diablocks(filename)"'
         
         #get equidistant timeseries from metadata
         if block_ids is None or block_ids=='allstation':
             if station is None:
                 if len(diablocks_pd)==1:
                     station = diablocks_pd.loc[0,'station']
                 else:
-                    raise Exception('ERROR: if block_ids argument is not provided (or None) or is "allstation", station argument should be provided.')
+                    raise ValueError(('If block_ids argument is not provided (or None) or is "allstation", station '
+                                      f'argument should be provided.\n{diablocks_pd[print_cols]}'))
             bool_station = diablocks_pd['station']==station
             ids_station = diablocks_pd[bool_station].index.tolist()
             if len(ids_station)<1:
-                raise Exception('ERROR: no data block with requested station (%s) present in dia file. %s'%(station, str_getdiablockspd))
+                raise ValueError(f"No data block with requested station ({station}) present in dia file. {str_getdiablockspd}")
             elif len(ids_station)>1 and block_ids is None:
-                raise Exception('ERROR: more than one data block with requested station (%s) present in dia file. Provide block_ids argument to readts_dia() (int, list of int or "allstation"). %s'%(station, str_getdiablockspd))
+                raise ValueError(f"More than one data block with requested station ({station}) "
+                                 "present in dia file. Provide block_ids argument to read_dia() (int, list of int or 'allstation'). "
+                                 f"{str_getdiablockspd}")
             else: #exactly one occurrence or block_ids is provided or block_ids='allstation'
                 block_ids = ids_station
         
         #check validity of blockids of type listlist
         if isinstance(block_ids,int):
             block_ids = [block_ids]
         if not isinstance(block_ids,list):
-            raise Exception('ERROR: invalid type for block_ids (should be int, list of int or "allstation")')
+            raise TypeError('Invalid type for block_ids (should be int, list of int or "allstation")')
         if not pd.Series(block_ids).isin(diablocks_pd.index).all():
-            raise Exception(f'ERROR: invalid values in block_ids list ({block_ids}), possible are {diablocks_pd.index.tolist()} (all integers)')
+            raise ValueError(f"Invalid values in block_ids list ({block_ids}), "
+                             f"possible are {diablocks_pd.index.tolist()} (all integers)")
             
         if station is not None:
             if not isinstance(station,str):
-                raise Exception('ERROR: station argument should be of type string')
+                raise TypeError('Station argument should be of type string')
             bool_samestation = diablocks_pd.loc[block_ids,'station']==station
             if not bool_samestation.all():
-                raise Exception('ERROR: both the arguments station and block_ids are provided, but at least one of the requested block_ids corresponds to a different station. %s'%(str_getdiablockspd))
+                raise ValueError("Both the arguments station and block_ids are provided, "
+                                 "but at least one of the requested block_ids corresponds to a different station. "
+                                 f"{str_getdiablockspd}")
             
-        data_pd_allblocks = pd.DataFrame()
         for block_id in block_ids:
-            if np.isnan(diablocks_pd.loc[block_id,'timestep_min']): #non-equidistant
-                data_pd_oneblock = readts_dia_nonequidistant(filename_one, diablocks_pd, block_id)
+            if np.isnan(diablocks_pd.loc[block_id,'timestep_min']):
+                data_pd_oneblock = read_dia_nonequidistant(filename_one, diablocks_pd, block_id)
             else: #equidistant
-                data_pd_oneblock = readts_dia_equidistant(filename_one, diablocks_pd, block_id)
-            if get_status: #TODO: this can be more generic (eg add additional metadata) or more neat. Also in get_diablocks()
-                block_status_list = diablocks_pd.loc[block_id,'STA'].split('!')
-                for block_status_one in block_status_list:
-                    status_tstart = dt.datetime.strptime(block_status_one[4:17],'%Y%m%d;%H%M')
-                    status_tstop = dt.datetime.strptime(block_status_one[18:31],'%Y%m%d;%H%M')
-                    status_val = block_status_one[-1]
-                    data_pd_oneblock.loc[status_tstart:status_tstop,'Status'] = status_val
-            data_pd_allblocks = pd.concat([data_pd_allblocks,data_pd_oneblock], ignore_index=False)
-        
-        #append to allyears dataset
-        data_pd_all = pd.concat([data_pd_all,data_pd_allblocks], ignore_index=False)
-
+                data_pd_oneblock = read_dia_equidistant(filename_one, diablocks_pd, block_id)
+            data_pd_list.append(data_pd_oneblock)
+            metadata = metadata_from_obj(data_pd_oneblock)
+            metadata_list.append(metadata)
+    
+    #concat allyears dataset
+    data_pd_all = pd.concat(data_pd_list)
+    metadata_compare(metadata_list)
+    metadata = metadata_list[0].copy()
+    metadata['tstart'] = metadata_list[0]['tstart']
+    metadata['tstop'] = metadata_list[-1]['tstop']
+    data_pd_all = metadata_add_to_obj(data_pd_all,metadata)
+    
     if allow_duplicates:
         return data_pd_all
     
-    #check overlapping timesteps, sort values on time and check_ts
-    if len(data_pd_all) != len(data_pd_all.index.unique()):
-        raise Exception('ERROR: merged datasets have duplicate/overlapping timesteps, clean up your input data or provide one file instead of a list')
-    data_pd_all = data_pd_all.sort_index(axis=0)
+    #check overlapping timesteps, sort values on time
+    if data_pd_all.index.duplicated().any():
+        raise ValueError("Merged datasets have duplicate/overlapping timesteps, "
+                         "clean up your input data or provide one file instead of a list")
+    if not data_pd_all.index.is_monotonic_increasing:
+        data_pd_all = data_pd_all.sort_index()
     
     return data_pd_all
 
 
-def readts_noos(filename, datetime_format='%Y%m%d%H%M', na_values=None):
+def read_noos(filename, datetime_format='%Y%m%d%H%M', na_values=None):
     """
     Reads a noos file
 
     Parameters
     ----------
     filename : TYPE
         DESCRIPTION.
@@ -1555,15 +1618,15 @@
     Returns
     -------
     data_pd : TYPE
         DESCRIPTION.
 
     """
     
-    print('reading file: %s'%(filename))
+    logger.info('reading file: %s'%(filename))
     noosheader = []
     noosheader_dict = {} #TODO: this is not returned, could be valuable to do so
     with open(filename) as f:
         for linenum, line in enumerate(f, 0):
             if '#' in line:
                 noosheader.append(line)
                 comment_stripped = line.strip('#').strip().split(': ')
@@ -1571,15 +1634,18 @@
                     if comment_stripped[0] != '':
                         noosheader_dict[comment_stripped[0]] = ''
                 else:
                     noosheader_dict[comment_stripped[0].strip()] = comment_stripped[1].strip()
             else:
                 startdata = linenum
                 break
-    
-    content_pd = pd.read_csv(filename,header=startdata-1,delim_whitespace=True,names=['times_str','values'], na_values=na_values)
+        
+    content_pd = pd.read_csv(filename,header=startdata-1, sep="\\s+",names=['times_str','values'], na_values=na_values)
     noos_datetime = pd.to_datetime(content_pd['times_str'],format=datetime_format)
     data_pd = pd.DataFrame({'values':content_pd['values'].values},index=noos_datetime)
     
-    print(check_ts(data_pd))
+    # clean noos metadata and add as attrs
+    noosheader_dict_clean = {k:v for k,v in noosheader_dict.items() if v!=''}
+    data_pd.attrs = noosheader_dict_clean
+    
     return data_pd
```

### Comparing `hatyan-2.7.0/tests/test_astrog_main.py` & `hatyan-2.8.0/tests/test_astrog.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,42 +13,42 @@
 import datetime as dt
 import hatyan
 
 
 @pytest.mark.systemtest
 def test_astrog_dT():
     # 1. Input
-    timeInput = pd.date_range(start=dt.datetime(1970,12,31,12,31),end=dt.datetime(2020,12,31,12,31),freq='Y')
+    timeInput = pd.date_range(start=dt.datetime(1970,12,31,12,31),end=dt.datetime(2020,12,31,12,31),freq='YS')
     
     # 2. Expectations
-    dTLastExp = np.array([38.792, 39.468, 40.144, 40.82 , 41.496, 42.172, 42.848, 43.524,
-                           44.2  , 44.876, 45.552, 46.228, 46.904, 47.58 , 48.256, 48.932,
-                           49.608, 50.284, 50.96 , 51.636, 52.312, 52.988, 53.664, 54.34 ,
-                           55.016, 55.692, 56.368, 57.044, 57.72 , 58.396, 59.072, 59.748,
-                           60.424, 61.1  , 61.776, 62.452, 63.128, 63.804, 64.48 , 65.156,
-                           65.832, 66.508, 67.184, 67.86 , 68.536, 69.212, 69.888, 70.564,
-                           71.24 , 71.916, 72.592])
-    dTExctExp = np.array([42.184, 42.184, 43.184, 44.184, 45.184, 46.184, 47.184, 48.184,
-                            49.184, 50.184, 51.184, 52.184, 53.184, 54.184, 54.184, 55.184,
-                            55.184, 55.184, 56.184, 56.184, 57.184, 58.184, 59.184, 60.184,
-                            61.184, 61.184, 62.184, 63.184, 63.184, 64.184, 64.184, 64.184,
-                            64.184, 64.184, 64.184, 64.184, 65.184, 65.184, 65.184, 66.184,
-                            66.184, 66.184, 67.184, 67.184, 67.184, 68.184, 68.184, 69.184,
-                            69.184, 69.184, 69.184])
+    dTLastExp = np.array([39.468, 40.144, 40.82 , 41.496, 42.172, 42.848, 43.524, 44.2  ,
+           44.876, 45.552, 46.228, 46.904, 47.58 , 48.256, 48.932, 49.608,
+           50.284, 50.96 , 51.636, 52.312, 52.988, 53.664, 54.34 , 55.016,
+           55.692, 56.368, 57.044, 57.72 , 58.396, 59.072, 59.748, 60.424,
+           61.1  , 61.776, 62.452, 63.128, 63.804, 64.48 , 65.156, 65.832,
+           66.508, 67.184, 67.86 , 68.536, 69.212, 69.888, 70.564, 71.24 ,
+           71.916, 72.592])
+    dTExctExp = np.array([42.184, 42.184, 44.184, 45.184, 46.184, 47.184, 48.184, 49.184,
+           50.184, 51.184, 51.184, 52.184, 53.184, 54.184, 54.184, 55.184,
+           55.184, 56.184, 56.184, 57.184, 58.184, 58.184, 59.184, 60.184,
+           61.184, 62.184, 62.184, 63.184, 64.184, 64.184, 64.184, 64.184,
+           64.184, 64.184, 64.184, 65.184, 65.184, 65.184, 66.184, 66.184,
+           66.184, 66.184, 67.184, 67.184, 67.184, 68.184, 69.184, 69.184,
+           69.184, 69.184])
     
     # 3. Run test
-    dTLastOut = hatyan.dT(timeInput,dT_fortran=True)
-    dTExctOut = hatyan.dT(timeInput,dT_fortran=False)
+    dTLastOut = hatyan.astrog.dT(timeInput,dT_fortran=True)
+    dTExctOut = hatyan.astrog.dT(timeInput,dT_fortran=False)
     
     # 4. Vefication
     assert type(dTLastOut) == np.ndarray
     assert type(dTExctOut) == np.ndarray
-    assert (abs(dTLastExp-dTLastOut) < 10E-9).all()
-    assert (abs(dTExctExp-dTExctOut) < 10E-9).all()
-    
+    assert np.allclose(dTLastExp, dTLastOut)
+    assert np.allclose(dTExctExp, dTExctOut)
+
 
 @pytest.mark.systemtest
 def test_astrog_astrab():
     
     # 1. Input
     timeInput = dt.datetime(2008,1,1,12,31)
     
@@ -69,15 +69,15 @@
                  'EHSUN':  np.array([6.92014497]),
                  'LONMOO': np.array([203.54708946]),
                  'LATMOO': np.array([-4.18226297]),
                  'RAMOON': np.array([200.20845513]),
                  'ANM':    np.array([151.15606465])}
     
     # 3. Run test
-    parOutput = hatyan.astrab(timeInput,hatyan.dT(timeInput,dT_fortran=True))
+    parOutput = hatyan.astrog.astrab(timeInput,hatyan.astrog.dT(timeInput,dT_fortran=True))
     
     # 4. Vefication
     assert type(parOutput) == dict
     assert len(parOutput)  == 18
     for parName in parExpect:
         assert len(parOutput[parName]) == 1
         assert abs(parExpect[parName][0]-parOutput[parName][0]) < 10E-9
@@ -106,20 +106,38 @@
                   pd.DatetimeIndex(['2007-12-22 06:08:46.055884800']),
                   pd.DatetimeIndex(['2008-01-03 08:22:45.903254400']),
                   pd.DatetimeIndex(['2008-01-03 08:22:45.696239999'])]
      
     # 3. Run test
     timeOutput = []
     for iMode in range(1,17):
-        timeOutput.append(hatyan.astrac(timeInput,dT_fortran=False,mode=np.array(iMode)))
+        timeOutput.append(hatyan.astrog.astrac(timeInput,dT_fortran=False,mode=np.array(iMode)))
     
     # 4. Vefication
     for iMode in range(1,17):
         print(iMode)
         assert type(timeOutput[iMode-1]) == pd.DatetimeIndex
         assert abs(timeExpect[iMode-1]-timeOutput[iMode-1]).total_seconds() < 10E-5
 
 
+def test_astrog_moonriseset():
+    """
+    This part of code resulted in timesteps being dropped in newer pandas versions.
+    This was due to 0 RATES in astract, resulting in inf values in 'addtime'.
+    This is solved by supplying posinf=0 to np.nan_to_num().
+    This test therefore checks if the length of the resulting dataframe is correct.
+    """
+    
+    # script settings
+    tstart = dt.datetime(2003,1,1)
+    tstop = dt.datetime(2003,6,1)
+    
+    # moonrise and -set
+    moonriseset_python = hatyan.astrog_moonriseset(tFirst=tstart, tLast=tstop)
+    
+    assert len(moonriseset_python) == 292
+
+
 @pytest.mark.systemtest
 def test_astrog_leapsecondslist():
-    leap_seconds_pd, expirydate = hatyan.get_leapsecondslist_fromurlorfile()
+    leap_seconds_pd, expirydate = hatyan.astrog.get_leapsecondslist_fromurlorfile()
```

### Comparing `hatyan-2.7.0/tests/test_hatyan_main.py` & `hatyan-2.8.0/tests/test_hatyan.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,282 +7,31 @@
 """
 
 import pytest
 import os
 import numpy as np
 import pandas as pd
 import datetime as dt
-from netCDF4 import Dataset, num2date
 import hatyan
+import pytz
 
 dir_tests = os.path.dirname(__file__) #F9 doesnt work, only F5 (F5 also only method to reload external definition scripts)
 dir_testdata = os.path.join(dir_tests,'data_unitsystemtests')
-modulename_list = ['os','sys','glob','shutil','scipy','numpy','datetime','pandas','pyproj','matplotlib','netCDF4','hatyan']
-
-
-@pytest.mark.parametrize("modulename", [pytest.param('%s'%(stat), id='%s'%(stat)) for stat in modulename_list])
-@pytest.mark.unittest
-def test_import_libraries(modulename):
-    exec('import %s'%(modulename))
-    if modulename == 'pyproj':
-        exec('from pyproj import Transformer')
-
-
-@pytest.mark.unittest
-def test_readts_dia_multifile():
-    file_data_comp0 = [os.path.join(dir_testdata,'%s_obs%i.txt'%('VLISSGN', file_id)) for file_id in [1,2,3,4]]
-    ts_measurements_group0 = hatyan.readts_dia(filename=file_data_comp0, station='VLISSGN')
-    
-    assert len(ts_measurements_group0) == 35064
-
-
-@pytest.mark.unittest
-def test_readts_dia_multiblock():
-    
-    file1 = os.path.join(dir_testdata,'hoek_har.dia')
-    #ts_measurements_group0_extno = hatyan.readts_dia(filename=file1, station='HOEKVHLD')
-    ts_measurements_group0_ext0 = hatyan.readts_dia(filename=file1, station='HOEKVHLD', block_ids=0)
-    ts_measurements_group0_ext1 = hatyan.readts_dia(filename=file1, station='HOEKVHLD', block_ids=1)
-    ts_measurements_group0_ext2 = hatyan.readts_dia(filename=file1, station='HOEKVHLD', block_ids=2)
-    ts_measurements_group0_ext012 = hatyan.readts_dia(filename=file1, station='HOEKVHLD', block_ids=[0,1,2])
-    ts_measurements_group0_extall = hatyan.readts_dia(filename=file1, station='HOEKVHLD', block_ids='allstation')
-    
-    assert len(ts_measurements_group0_ext0) == 3977
-    assert len(ts_measurements_group0_ext1) == 9913
-    assert len(ts_measurements_group0_ext2) == 9403
-    assert len(ts_measurements_group0_ext012) == 23293
-    assert len(ts_measurements_group0_extall) == 23293
-
-
-@pytest.mark.unittest
-def test_readts_noos_resamplecrop():
-
-    file_data_comp0 = os.path.join(dir_testdata,'VLISSGN_waterlevel_20180101_20180401.noos')
-    times_ext_comp0 = [dt.datetime(2018,1,1),dt.datetime(2018,4,1)]
-
-    #component groups
-    ts_measurements_group0 = hatyan.readts_noos(filename=file_data_comp0)
-    ts_measurements_group0_res = hatyan.resample_timeseries(ts_measurements_group0, timestep_min=10)
-    ts_measurements_group0_rescrop = hatyan.crop_timeseries(ts_measurements_group0_res, times_ext=times_ext_comp0)
-    
-    assert len(ts_measurements_group0) == 12752
-    assert len(ts_measurements_group0_res) == 12961
-    assert len(ts_measurements_group0_rescrop) == 12961
-    assert ts_measurements_group0_rescrop.index[0] == pd.Timestamp('2018-01-01')
-    assert ts_measurements_group0_rescrop.index[-1] == pd.Timestamp('2018-04-01')
-    assert ts_measurements_group0_rescrop['values'][0] == 2.5
-    assert ts_measurements_group0_rescrop['values'][-1] == 1.05
-
-
-@pytest.mark.unittest
-def test_writenetcdf():
-    
-    current_station = 'VLISSGN'
-    times_ext=[dt.datetime(2019,1,1),dt.datetime(2019,6,1)]
-    
-    file_pred = os.path.join(dir_testdata,f'{current_station}_pre.txt')
-    ts_prediction = hatyan.readts_dia(filename=file_pred, station=current_station)
-    ts_prediction = hatyan.crop_timeseries(ts_prediction, times_ext=times_ext)
-    ts_ext_prediction = hatyan.calc_HWLW(ts=ts_prediction)
-    
-    file_nc = 'prediction_10m_%s.nc'%(current_station)
-    hatyan.write_tsnetcdf(ts=ts_prediction, ts_ext=ts_ext_prediction, station=current_station, vertref='NAP', filename=file_nc, tzone_hr=1)
-    
-    data_nc = Dataset(file_nc,'r')
-    
-    timevar = data_nc.variables['time']
-    timevar_dt = num2date(timevar[:],units=timevar.units, only_use_cftime_datetimes=False, only_use_python_datetimes=True)
-    
-    #put netcdf file contents in pandas DataFrame for usage in hatyan
-    ts_pd = pd.DataFrame({'values':data_nc.variables['waterlevel_astro'][:,0]}, index=timevar_dt)
-    print(ts_pd)
-    
-    assert list(data_nc.dimensions.keys()) == ['stations', 'statname_len', 'time', 'analysis_time', 'time_HW', 'time_LW']
-    assert list(data_nc.variables.keys()) == ['stations', 'analysis_time', 'time', 'waterlevel_astro', 'time_HW', 'waterlevel_astro_HW', 'time_LW', 'waterlevel_astro_LW']
-    assert timevar_dt[0] == times_ext[0]
-    assert timevar_dt[-1] == times_ext[-1]
-    assert 'title' in data_nc.__dict__.keys()
-    assert 'institution' in data_nc.__dict__.keys()
-    assert 'source' in data_nc.__dict__.keys()
-    assert timevar.units == 'minutes since 1900-01-01 00:00:00 +0100'
-
-    data_nc.close()
-    os.remove(file_nc)
-
-
-@pytest.mark.unittest
-def test_analysis_settings():
-    
-    current_station = 'VLISSGN'
-    
-    #comp0
-    file_data_comp0 = [os.path.join(dir_testdata,'%s_obs%i.txt'%(current_station, file_id)) for file_id in [1]]
-    ts_measurements_group0 = hatyan.readts_dia(filename=file_data_comp0, station=current_station)
-    
-    ts_comp_nfac1_fualltimes0_xfac1_peryear0 = hatyan.get_components_from_ts(ts=ts_measurements_group0, const_list='month', nodalfactors=True, fu_alltimes=False, xfac=True, analysis_perperiod=False)
-    
-    ts_comp_onecomp = hatyan.analysis(ts=ts_measurements_group0, const_list=['M2'], nodalfactors=True, fu_alltimes=True, xfac=True)
-    
-    ts_comp_nfac1_fualltimes1_xfac1 = hatyan.analysis(ts=ts_measurements_group0, const_list='month', nodalfactors=True, fu_alltimes=True, xfac=True)
-    ts_comp_nfac1_fualltimes0_xfac1 = hatyan.analysis(ts=ts_measurements_group0, const_list='month', nodalfactors=True, fu_alltimes=False, xfac=True)
-    ts_comp_nfac1_fualltimes1_xfac0 = hatyan.analysis(ts=ts_measurements_group0, const_list='month', nodalfactors=True, fu_alltimes=True, xfac=False)
-    ts_comp_nfac1_fualltimes0_xfac0 = hatyan.analysis(ts=ts_measurements_group0, const_list='month', nodalfactors=True, fu_alltimes=False, xfac=False)
-    ts_comp_nfac0_fualltimes0_xfac0 = hatyan.analysis(ts=ts_measurements_group0, const_list='month', nodalfactors=False, fu_alltimes=False, xfac=False)
-    
-    comp_A_expected = np.array([9.92687566e-04, 3.11039747e-02, 9.73652407e-02, 6.68645368e-02,
-                                4.02714135e-02, 2.44247279e-02, 1.34401343e-01, 2.69848016e-01,
-                                1.74658516e+00, 1.33037114e-01, 4.78882284e-01, 4.42634321e-02,
-                                1.93477077e-02, 4.29425377e-02, 1.28103067e-01, 8.89165480e-02,
-                                4.66780541e-02, 8.50788597e-02, 9.01287840e-02, 3.06546626e-02,
-                                4.72786278e-02, 1.47588322e-02])
-    
-    comp_phi_expected = np.array([  0.        , 141.78046951, 188.22394202,   7.35166063,
-                                  279.19176166, 122.65613222, 159.77053294,  33.54516691,
-                                   59.02752661, 256.04742485, 117.45538945, 345.62388999,
-                                  200.90891452,  92.80114988, 115.31391482, 176.58434752,
-                                   77.32631928, 103.4830287 , 153.94793646, 110.76924584,
-                                  157.3933541 , 220.41306556])
-    
-    assert (np.abs(ts_comp_nfac1_fualltimes0_xfac1_peryear0-ts_comp_nfac1_fualltimes0_xfac1) < 10E-9).all().all()
-    assert (np.abs(ts_comp_nfac1_fualltimes0_xfac1_peryear0['phi_deg'].values-comp_phi_expected) < 10E-9).all()
-    assert (np.abs(ts_comp_nfac1_fualltimes0_xfac1_peryear0['A'].values-comp_A_expected) < 10E-9).all()
-
-
-@pytest.mark.unittest
-def test_analysis_foreman():
-    current_station = 'VLISSGN'
-    
-    #comp0
-    file_data_comp0 = [os.path.join(dir_testdata,'%s_obs%i.txt'%(current_station, file_id)) for file_id in [1]]
-    ts_measurements_group0 = hatyan.readts_dia(filename=file_data_comp0, station=current_station)
-    
-    comp_frommeas_SCHU = hatyan.get_components_from_ts(ts=ts_measurements_group0, const_list='month', nodalfactors=True, fu_alltimes=True, xfac=True, source='schureman')
-    comp_frommeas_FOR = hatyan.get_components_from_ts(ts=ts_measurements_group0, const_list='month', nodalfactors=True, fu_alltimes=True, xfac=True, source='foreman')
-    SCHU_comp_phi_expected =  np.array([  0.        , 141.68386391, 188.27101759,   7.3992028 ,
-                                       279.17807514, 122.81257343, 159.77061119,  33.51788732,
-                                        59.01827634, 256.05796043, 117.47528038, 345.63438447,
-                                       201.05307505,  92.81986396, 115.2820895 , 176.56952991,
-                                        77.30925229, 103.43837741, 153.90952097, 110.64017054,
-                                       157.30038107, 220.24021917])
-    SCHU_comp_A_expected =    np.array([9.93677030e-04, 3.11102518e-02, 9.74940999e-02, 6.69089179e-02,
-                                       4.01204828e-02, 2.43192049e-02, 1.34386805e-01, 2.69878623e-01,
-                                       1.74649803e+00, 1.32976762e-01, 4.79019453e-01, 4.42086557e-02,
-                                       1.92695651e-02, 4.29786476e-02, 1.28078709e-01, 8.89513755e-02,
-                                       4.67055728e-02, 8.50832246e-02, 9.01742533e-02, 3.06526796e-02,
-                                       4.72907179e-02, 1.47366661e-02])
-    FOR_comp_phi_expected =  np.array([  0.        , 321.7403689 ,   8.15729584, 187.40999172,
-                                       279.42669414, 122.65017113, 160.05967765,  33.32750808,
-                                        59.01572119, 256.18495318, 117.35826025, 345.41402817,
-                                       201.17575979,  92.60563462, 115.27544986, 176.43679913,
-                                        77.08771066, 103.42351654, 153.76456299, 110.600143  ,
-                                       157.16101443, 220.13261581])
-    FOR_comp_A_expected =    np.array([9.96058525e-04, 3.01459094e-02, 9.72007804e-02, 6.69287134e-02,
-                                       3.99816712e-02, 2.42471615e-02, 1.33778086e-01, 2.75247289e-01,
-                                       1.76155491e+00, 1.39007149e-01, 4.85825897e-01, 4.40858825e-02,
-                                       1.92198515e-02, 4.29817009e-02, 1.29452749e-01, 9.04975848e-02,
-                                       4.66816274e-02, 8.62181973e-02, 9.27486375e-02, 3.13117938e-02,
-                                       4.82570962e-02, 1.46874202e-02])
-    
-    assert (np.abs(comp_frommeas_SCHU['phi_deg'].values-SCHU_comp_phi_expected) < 10E-9).all()
-    assert (np.abs(comp_frommeas_SCHU['A'].values-SCHU_comp_A_expected) < 10E-9).all()
-    assert (np.abs(comp_frommeas_FOR['phi_deg'].values-FOR_comp_phi_expected) < 10E-9).all()
-    assert (np.abs(comp_frommeas_FOR['A'].values-FOR_comp_A_expected) < 10E-9).all()
-
-
-@pytest.mark.unittest
-def test_getcomponentsfromts_settings():
-    
-    current_station = 'VLISSGN'
-    
-    #comp0
-    file_data_comp0 = [os.path.join(dir_testdata,'%s_obs%i.txt'%(current_station, file_id)) for file_id in [1,2]]
-    ts_measurements_group0 = hatyan.readts_dia(filename=file_data_comp0, station=current_station)
-    
-    ts_comp_nfac1_fualltimes1_xfac1_peryear0 = hatyan.get_components_from_ts(ts=ts_measurements_group0, const_list='month', nodalfactors=True, fu_alltimes=True, xfac=True, analysis_perperiod=False)
-    
-    ts_comp_nfac1_fualltimes1_xfac1_permonth0 = hatyan.get_components_from_ts(ts=ts_measurements_group0, const_list='month', nodalfactors=True, fu_alltimes=True, xfac=True, analysis_perperiod='M')
-    
-    ts_comp_nfac1_fualltimes1_xfac1 = hatyan.get_components_from_ts(ts=ts_measurements_group0, const_list='month', nodalfactors=True, fu_alltimes=True, xfac=True, analysis_perperiod='Y')
-    ts_comp_nfac1_fualltimes0_xfac1 = hatyan.get_components_from_ts(ts=ts_measurements_group0, const_list='month', nodalfactors=True, fu_alltimes=False, xfac=True, analysis_perperiod='Y')
-    ts_comp_nfac1_fualltimes1_xfac0 = hatyan.get_components_from_ts(ts=ts_measurements_group0, const_list='month', nodalfactors=True, fu_alltimes=True, xfac=False, analysis_perperiod='Y')
-    ts_comp_nfac1_fualltimes0_xfac0 = hatyan.get_components_from_ts(ts=ts_measurements_group0, const_list='month', nodalfactors=True, fu_alltimes=False, xfac=False, analysis_perperiod='Y')
-    ts_comp_nfac0_fualltimes0_xfac0 = hatyan.get_components_from_ts(ts=ts_measurements_group0, const_list='month', nodalfactors=False, fu_alltimes=False, xfac=False, analysis_perperiod='Y')
-
-
-@pytest.mark.unittest
-def test_predictionsettings():
-    times_ext_pred_HWLWno = [dt.datetime(2009,12,31,14),dt.datetime(2010,1,2,12)]
-    times_step_pred = 1
-    current_station = 'DENHDR'
-    
-    file_data_comp0 = os.path.join(dir_testdata,'%s_ana.txt'%(current_station))
-    COMP_merged = hatyan.read_components(filename=file_data_comp0)
-    ts_prediction_nfac1_fualltimes1_xfac1 = hatyan.prediction(comp=COMP_merged, nodalfactors=True, fu_alltimes=True, xfac=True, times_ext=times_ext_pred_HWLWno, timestep_min=times_step_pred)
-    ts_prediction_nfac1_fualltimes0_xfac1 = hatyan.prediction(comp=COMP_merged, nodalfactors=True, fu_alltimes=False, xfac=True, times_ext=times_ext_pred_HWLWno, timestep_min=times_step_pred)
-    ts_prediction_nfac1_fualltimes1_xfac0 = hatyan.prediction(comp=COMP_merged, nodalfactors=True, fu_alltimes=True, xfac=False, times_ext=times_ext_pred_HWLWno, timestep_min=times_step_pred)
-    ts_prediction_nfac1_fualltimes0_xfac0 = hatyan.prediction(comp=COMP_merged, nodalfactors=True, fu_alltimes=False, xfac=False, times_ext=times_ext_pred_HWLWno, timestep_min=times_step_pred)
-    ts_prediction_nfac0_fualltimes0_xfac0 = hatyan.prediction(comp=COMP_merged, nodalfactors=False, fu_alltimes=False, xfac=False, times_ext=times_ext_pred_HWLWno, timestep_min=times_step_pred)
-
-
-@pytest.mark.unittest
-def test_prediction_1018():
-    current_station = 'DENHDR'
-    nodalfactors = True
-    xfac=True
-    
-    times_ext_pred = [dt.datetime(1018,7,21),dt.datetime(1018,7,21,3)]
-    times_step_pred = 10
-    
-    file_data_comp0 = os.path.join(dir_testdata,'%s_ana.txt'%(current_station))
-    COMP_merged = hatyan.read_components(filename=file_data_comp0)
-    
-    #prediction
-    ts_prediction = hatyan.prediction(comp=COMP_merged, nodalfactors=nodalfactors, xfac=xfac, fu_alltimes=False, times_ext=times_ext_pred, timestep_min=times_step_pred)
-    
-    ts_prediction_times = np.array([dt.datetime(1018, 7, 21, 0, 0),
-                                    dt.datetime(1018, 7, 21, 0, 10),
-                                    dt.datetime(1018, 7, 21, 0, 20),
-                                    dt.datetime(1018, 7, 21, 0, 30),
-                                    dt.datetime(1018, 7, 21, 0, 40),
-                                    dt.datetime(1018, 7, 21, 0, 50),
-                                    dt.datetime(1018, 7, 21, 1, 0),
-                                    dt.datetime(1018, 7, 21, 1, 10),
-                                    dt.datetime(1018, 7, 21, 1, 20),
-                                    dt.datetime(1018, 7, 21, 1, 30),
-                                    dt.datetime(1018, 7, 21, 1, 40),
-                                    dt.datetime(1018, 7, 21, 1, 50),
-                                    dt.datetime(1018, 7, 21, 2, 0),
-                                    dt.datetime(1018, 7, 21, 2, 10),
-                                    dt.datetime(1018, 7, 21, 2, 20),
-                                    dt.datetime(1018, 7, 21, 2, 30),
-                                    dt.datetime(1018, 7, 21, 2, 40),
-                                    dt.datetime(1018, 7, 21, 2, 50),
-                                    dt.datetime(1018, 7, 21, 3, 0)], dtype=object)
-    ts_prediction_vals = np.array([-0.77416669, -0.78821831, -0.79718123, -0.80126649, -0.80055319,
-                                   -0.79466499, -0.78252257, -0.76226094, -0.73136835, -0.68705389,
-                                   -0.62679467, -0.54896408, -0.4534113 , -0.34185962, -0.218017  ,
-                                   -0.08734459,  0.04350389,  0.16749106,  0.27811846])
-    
-    assert (np.abs(ts_prediction['values'].values-ts_prediction_vals) < 10E-9).all()
-    assert (np.abs(ts_prediction.index.values-ts_prediction_times) < dt.timedelta(days=10E-9)).all()
 
 
 @pytest.mark.systemtest
 def test_frommergedcomp():
     # 1. define test data
-    nodalfactors = True
-    xfac = True
     current_station = 'VLISSGN'
     
     #comp
     file_data_comp = os.path.join(dir_testdata,'%s_ana.txt'%(current_station))
     
     #pred
-    times_ext_pred = [dt.datetime(2019,1,1),dt.datetime(2019,1,1,12)]
-    timestep_pred = 10
+    times_pred = slice(dt.datetime(2019,1,1),dt.datetime(2019,1,1,12), "10min")
     
     # 2. define initial expectations
     expected_ts_prediction_data_pd_values = np.array([1.00809295,  0.89565827,  0.77557688,  0.64880508,  0.51669927,
                                                       0.38083644,  0.24282757,  0.1041679 , -0.03384444, -0.17011025,
                                                      -0.3036618 , -0.43355561, -0.55876447, -0.67810779, -0.79024821,
                                                      -0.89376351, -0.98728197, -1.06965037, -1.14009357, -1.19832413,
                                                      -1.2445716 , -1.27952004, -1.30416467, -1.31961912, -1.32691704,
@@ -295,21 +44,22 @@
                                                       1.30605751,  1.42377775,  1.52525728,  1.60791471,  1.66976848,
                                                       1.70970034,  1.72765351,  1.72471102,  1.70301805,  1.66554205,
                                                       1.61569821,  1.55689834,  1.49210117,  1.42344542,  1.35203362,
                                                       1.27790547,  1.20020227,  1.11748521])
     
     # 3. run test
     COMP_mergedfromfile = hatyan.read_components(filename=file_data_comp)
-    ts_prediction_direct = hatyan.prediction(COMP_mergedfromfile, nodalfactors=nodalfactors, xfac=xfac, fu_alltimes=False, times_ext=times_ext_pred, timestep_min=timestep_pred)
+    ts_prediction_direct = hatyan.prediction(COMP_mergedfromfile, times=times_pred)
     ts_prediction_direct_values = ts_prediction_direct['values'].values
     
     # 4. Vefiry final expectations
     assert type(ts_prediction_direct) == pd.core.frame.DataFrame
-    assert ts_prediction_direct.index[0].to_pydatetime() == times_ext_pred[0]
-    assert ts_prediction_direct.index[-1].to_pydatetime() == times_ext_pred[-1]
+    assert ts_prediction_direct.index.tz==pytz.FixedOffset(60)
+    assert ts_prediction_direct.index[0].tz_localize(None) == times_pred.start
+    assert ts_prediction_direct.index[-1].tz_localize(None) == times_pred.stop
     assert len(ts_prediction_direct_values) == len(expected_ts_prediction_data_pd_values)
     assert type(ts_prediction_direct_values) == type(expected_ts_prediction_data_pd_values)
     assert (np.abs(ts_prediction_direct_values - expected_ts_prediction_data_pd_values) < 10E-9).all()
 
 
 @pytest.mark.systemtest
 def test_meas_HWLW_toomuch():
@@ -343,15 +93,14 @@
             0.8648,  0.9185,  0.955 ,  0.9721,  0.971 ,  0.9652,  0.9486,
             0.9194,  0.8885,  0.8618,  0.8491,  0.8154,  0.7478,  0.7017,
             0.6724,  0.6105,  0.5356,  0.4669,  0.3918,  0.323 ,  0.2405])
     wl_times = pd.date_range('2023-06-13 21:00','2023-06-15 02:00',freq='10min')
 
     # Then store it as a pandas dataframe and compute extremes
     wl_pd = pd.DataFrame({'values':wl_vals},index=wl_times)
-
     wl_pd_ext = hatyan.calc_HWLW(wl_pd)
 
     assert len(wl_pd_ext) == 3
     assert (wl_pd_ext['HWLWcode'] == [2,1,2]).all()
 
 
 @pytest.mark.systemtest
@@ -360,59 +109,79 @@
     Additional testcase for https://github.com/Deltares/hatyan/issues/85
     The min_width parameter for calc_HWLW() has to be approx 2hrs to properly compute and number almost all of the 19y timeseries
     Stations HELLVSS/KRIMPADLK/RAKND still fail, but it seems arbitrary and sometimes computing+numbering extremes per year does work
     """
     current_station = 'HOEKVHLD'
     file_dia = os.path.join(dir_testdata,f'{current_station}_obs19.txt')
     
-    wl_pd = hatyan.readts_dia(file_dia)
+    wl_pd = hatyan.read_dia(file_dia)
     
     wl_pd_ext = hatyan.calc_HWLW(wl_pd)
     
     # For testing: plot water level timeseries with peaks identified and labeled. 
     #hatyan.plot_timeseries(ts=wl_pd,ts_ext=wl_pd_ext)
     
     # RUN HATYAN: Assign numbers to the extremes
     wl_pd_ext = hatyan.calc_HWLWnumbering(wl_pd_ext,station=current_station)
 
+    
+@pytest.mark.systemtest
+def test_calc_HWLW_ts_with_gap():
+    """
+    testcase that checks if no extreme is computed at the start/end of a gap
+    like was documented in https://github.com/Deltares/hatyan/issues/97
+    """
+    
+    current_station = 'VLISSGN'
+    
+    file_pred = os.path.join(dir_testdata,f'{current_station}_pre.txt')
+    ts_prediction = hatyan.read_dia(filename=file_pred, station=current_station)
+    ts_prediction = ts_prediction.loc[slice("2019-01","2019-01")]
+    ts_prediction.loc[slice("2019-01-12 04:00", "2019-01-19 04:00")] = np.nan
+    
+    ts_ext_prediction = hatyan.calc_HWLW(ts=ts_prediction)
+    
+    # assert the number of extremes, was 91 before the fix of the issue
+    assert len(ts_ext_prediction) == 90
+
 
 @pytest.mark.systemtest
 def test_frommergedcomp_HWLW_toomuch():
     """
     This test produces a very short prediction for DENHDR, based on an imported component list. It then calculates extremes (HW/LW) and numbers them both.
     This test is meant to tweak the prominence parameter of scipy.signal.find_peaks() in hatyan.calc_HWLW() and it fails when the prominence is not set or is too small.
     A prominence value of None works for most stations, but fails for DENHDR in this period since a local dip is interpreted as a low water.
     This incorrect LW has a prominence of ~0.03, other peaks in this timeseries have a prominence of >1 and even when lowering M2 to an unrealistic value (0.5*M2) the prominence of peaks is >0.2
     A prominence value of 0.1 makes sure this test succeeds.
     
     """
     
     #for testing occurance of invalid low water at start of denhelder timeseries
-    times_ext_pred_HWLWno = [dt.datetime(2009,12,31,14),dt.datetime(2010,1,2,12)]
-    times_step_pred = 1
+    times_pred = slice(dt.datetime(2009,12,31,14),dt.datetime(2010,1,2,12), "1min")
     current_station = 'DENHDR'
 
     file_data_comp0 = os.path.join(dir_testdata,'%s_ana.txt'%(current_station))
-    COMP_merged = hatyan.read_components(filename=file_data_comp0)
-    COMP_merged_temp = COMP_merged.copy()
-    #COMP_merged_temp.loc['M2','A']=0.05
-    ts_prediction_HWLWno = hatyan.prediction(comp=COMP_merged_temp, nodalfactors=True, xfac=True, fu_alltimes=True, times_ext=times_ext_pred_HWLWno, timestep_min=times_step_pred)
-    ts_ext_prediction_HWLWno_pre = hatyan.calc_HWLW(ts=ts_prediction_HWLWno, debug=True)
+    comp_merged = hatyan.read_components(filename=file_data_comp0)
+    
+    ts_prediction_HWLWno = hatyan.prediction(comp=comp_merged, times=times_pred)
+    ts_ext_prediction_HWLWno_pre = hatyan.calc_HWLW(ts=ts_prediction_HWLWno)
     
     ts_ext_prediction_HWLWno = hatyan.calc_HWLWnumbering(ts_ext=ts_ext_prediction_HWLWno_pre, station=current_station)
-    #fig,(ax1,ax2) = hatyan.plot_timeseries(ts=ts_prediction_HWLWno, ts_ext=ts_ext_prediction_HWLWno_pre)
-    #for irow, pdrow in ts_ext_prediction_HWLWno.iterrows():
-    #    ax1.text(pdrow.index,pdrow['values'],pdrow['HWLWno'], color='k')
-
+    
+    values_actual = ts_ext_prediction_HWLWno_pre['values'].values
+    values_expected = np.array([-0.80339617,  0.61842454, -0.76465349,  0.79758517, -0.87872312])
+    hwlwcodes_actual = ts_ext_prediction_HWLWno_pre['HWLWcode'].values
+    hwlwcodes_expected = np.array([2, 1, 2, 1, 2])
+    hwlwnos_actual = ts_ext_prediction_HWLWno['HWLWno'].values
+    hwlwnos_expected = np.array([7057, 7058, 7058, 7059, 7059])
+    
     assert len(ts_ext_prediction_HWLWno_pre) == 5
-    assert (np.abs(ts_ext_prediction_HWLWno_pre['HWLWcode'].values-np.array([2, 1, 2, 1, 2])) < 10E-9).all()
-    assert (np.abs(ts_ext_prediction_HWLWno_pre['values'].values-np.array([-0.80339484,  0.61842428, -0.76465391,  0.79758734, -0.87872493 ])) < 10E-9).all()
-
-    assert len(ts_ext_prediction_HWLWno['HWLWno']) == 5
-    assert (np.abs(ts_ext_prediction_HWLWno['HWLWno'].values -np.array([7057, 7058, 7058, 7059, 7059])) < 10E-9).all()
+    assert np.allclose(values_actual, values_expected)
+    assert np.allclose(hwlwcodes_actual, hwlwcodes_expected)
+    assert np.allclose(hwlwnos_actual, hwlwnos_expected)
 
 
 @pytest.mark.systemtest
 #@pytest.mark.parametrize("current_station, yr", [pytest.param(x, y, id='%s %d'%(x,y))  for y in range(1999,2022) for x in ['WICK','ABDN','LEITH','WHITBY','IMMHM','CROMR','FELSWE','CADZD','VLISSGN','TERNZN','ROOMPBTN','HARVT10','HOEKVHLD','ROTTDM','DORDT','SCHEVNGN','IJMDBTHVN','PETTZD','DENHDR','DENOVBTN','HARLGN','HOLWD','SCHIERMNOG','LAUWOG','EEMSHVN','DELFZL','CUXHVN']])
 @pytest.mark.parametrize("current_station, yr", [pytest.param(x, y, id='%s_%d'%(x,y)) for y in [2018,2022] for x in ['HOEKVHLD','ROTTDM','DENHDR','LITHDP']])
 def test_frommergedcomp_HWLW_toolittle(current_station, yr):
     """
@@ -463,25 +232,25 @@
     #constituent list
     #const_list = hatyan.get_const_list_hatyan('year') #94 const
     #vertical reference
     #vertref='NAP'
     #END OF STATION SETTINGS
     
     file_data_comp0 = os.path.join(dir_testdata,'%s_ana.txt'%(current_station))
-    times_ext_pred = [dt.datetime(yr,1,1),dt.datetime(yr+1,1,1)]
-    times_step_pred = 1
+    times_pred = slice(dt.datetime(yr,1,1),dt.datetime(yr+1,1,1), "1min")
     
     #component groups
     COMP_merged = hatyan.read_components(filename=file_data_comp0)
+    assert COMP_merged.attrs["xfac"] == xfac
     
     #prediction and validation
-    ts_prediction = hatyan.prediction(comp=COMP_merged, nodalfactors=True, xfac=xfac, fu_alltimes=False, times_ext=times_ext_pred, timestep_min=times_step_pred)
-    #ts_validation = hatyan.readts_dia(filename=file_data_predvali, station=current_station)
-    #ts_ext_validation = hatyan.readts_dia(filename=file_data_predvaliHWLW, station=current_station)
-    ts_ext_prediction = hatyan.calc_HWLW(ts=ts_prediction, debug=True)
+    ts_prediction = hatyan.prediction(comp=COMP_merged, times=times_pred)
+    #ts_validation = hatyan.read_dia(filename=file_data_predvali, station=current_station)
+    #ts_ext_validation = hatyan.read_dia(filename=file_data_predvaliHWLW, station=current_station)
+    ts_ext_prediction = hatyan.calc_HWLW(ts=ts_prediction)
     
     #calculate tidal wave number
     ts_ext_prediction_HWLWno = hatyan.calc_HWLWnumbering(ts_ext=ts_ext_prediction, station=current_station)
     #print(ts_ext_prediction_HWLWno)
     #for irow, pdrow in ts_ext_prediction_HWLWno.iterrows():
     #    ax1.text(pdrow.index,pdrow['values'],pdrow['HWLWno'], color=colors[i_stat])
     
@@ -494,23 +263,23 @@
     print('all HWLW values:')
     print(ts_ext_prediction_HWLWno)
     
     HW_data = ts_ext_prediction_HWLWno[ts_ext_prediction_HWLWno['HWLWcode']==1]
     HW_data_diff1bool = (HW_data['HWLWno'].diff().iloc[1:].values==1)
     print('%i parts of HW array containing gaps:'%((~HW_data_diff1bool).sum()))
     if not HW_data_diff1bool.all():
-        ids_false = np.where(~HW_data_diff1bool)[0]
+        ids_false = np.nonzero(~HW_data_diff1bool)[0]
         for id_false in ids_false: 
             print(HW_data.iloc[id_false-1:id_false+3])
     
     LW_data = ts_ext_prediction_HWLWno[ts_ext_prediction_HWLWno['HWLWcode']==2]
     LW_data_diff1bool = (LW_data['HWLWno'].diff().iloc[1:].values==1)
     print('%i parts of LW array containing gaps:'%((~LW_data_diff1bool).sum()))
     if not LW_data_diff1bool.all():
-        ids_false = np.where(~LW_data_diff1bool)[0]
+        ids_false = np.nonzero(~LW_data_diff1bool)[0]
         for id_false in ids_false: 
             print(LW_data.iloc[id_false-1:id_false+3])
     
     assert HW_data_diff1bool.all()
     assert LW_data_diff1bool.all()
     
     #ax1.set_xlim(times_ext_pred)
@@ -528,29 +297,27 @@
     This test produces a prediction for a period for HOEKVHLD, based on an imported component list. It then calculates extremes (HW/LW) with several settings and numbers them both (including 3/4/5 HWLWcodes around aggers, excluding 11/22 HWLWcodes). 
     #HOEKVHLD has alternating aggers, DENHDR has double HW's (which should not be numbered as aggers)
     
     current_station = 'HOEKVHLD'
     current_station = 'DENHDR'
     """
     
-    times_step_pred = 1
-    
     file_data_comp0 = os.path.join(dir_testdata,'%s_ana.txt'%(current_station))
-    COMP_merged = hatyan.read_components(filename=file_data_comp0)
-    COMP_merged_temp = COMP_merged.copy()
+    comp_merged = hatyan.read_components(filename=file_data_comp0)
     
-    times_ext_pred_HWLWno = [dt.datetime(2010,1,31,3),dt.datetime(2010,2,17,12)] #longer period with alternating aggers and no aggers, also eerste HW wordt als lokaal ipv primair HW gezien, also extra agger outside of 1stLW/agger/2ndLW sequence
-    #times_ext_pred_HWLWno = [dt.datetime(2010,1,31),dt.datetime(2010,2,3)] #extra agger outside of 1stLW/agger/2ndLW sequence
-    #times_ext_pred_HWLWno = [dt.datetime(2010,6,26),dt.datetime(2010,6,28)] #lokale extremen tussen twee laagste LWs
-    #times_ext_pred_HWLWno = [dt.datetime(2019,2,1),dt.datetime(2019,2,2)] #eerste HW wordt als lokaal ipv primair HW gezien (lage prominence door dicht op begin tijdserie) >> warning
-    
-    ts_prediction_HWLWno = hatyan.prediction(comp=COMP_merged_temp, nodalfactors=True, xfac=True, fu_alltimes=True, times_ext=times_ext_pred_HWLWno, timestep_min=times_step_pred)
-    ts_ext_prediction_main = hatyan.calc_HWLW(ts=ts_prediction_HWLWno)#, debug=True)
-    #ts_ext_prediction_all = hatyan.calc_HWLW(ts=ts_prediction_HWLWno, calc_HWLW345=True, calc_HWLW345_cleanup1122=False)#, debug=True)
+    times_pred = slice(dt.datetime(2010,1,31,3),dt.datetime(2010,2,17,12), "1min") #longer period with alternating aggers and no aggers, also eerste HW wordt als lokaal ipv primair HW gezien, also extra agger outside of 1stLW/agger/2ndLW sequence
+    # times_pred = slice(dt.datetime(2010,1,31),dt.datetime(2010,2,3), "1min") #extra agger outside of 1stLW/agger/2ndLW sequence
+    # times_pred = slice(dt.datetime(2010,6,26),dt.datetime(2010,6,28), "1min") #lokale extremen tussen twee laagste LWs
+    # times_pred = slice(dt.datetime(2019,2,1),dt.datetime(2019,2,2), "1min") #eerste HW wordt als lokaal ipv primair HW gezien (lage prominence door dicht op begin tijdserie) >> warning
+    
+    ts_prediction_HWLWno = hatyan.prediction(comp=comp_merged, times=times_pred)
+    ts_ext_prediction_main = hatyan.calc_HWLW(ts=ts_prediction_HWLWno)
+    #ts_ext_prediction_all = hatyan.calc_HWLW(ts=ts_prediction_HWLWno, calc_HWLW345=True, calc_HWLW345_cleanup1122=False)
     ts_ext_prediction_clean = hatyan.calc_HWLW(ts=ts_prediction_HWLWno, calc_HWLW345=True)#, calc_HWLW345_cleanup1122=True) #for numbering, cannot cope with 11/22 HWLWcodes
+    ts_ext_prediction_clean_tomain = hatyan.calc_HWLW12345to12(ts_ext_prediction_clean)
     
     ts_ext_prediction_main_HWLWno = hatyan.calc_HWLWnumbering(ts_ext=ts_ext_prediction_main, station=current_station)
     ts_ext_prediction_clean_HWLWno = hatyan.calc_HWLWnumbering(ts_ext=ts_ext_prediction_clean, station=current_station)
     
     #fig, (ax1,ax2) = hatyan.plot_timeseries(ts=ts_prediction_HWLWno, ts_ext=ts_ext_prediction_all)#, ts_ext_validation=ts_ext_validation)
     #for irow, pdrow in ts_ext_prediction_clean_HWLWno.iterrows():
     #    ax1.text(pdrow.index,pdrow['values'],pdrow['HWLWno'])
@@ -615,46 +382,77 @@
         expected_ts_ext_prediction_clean_HWLWno_HWLWno = np.array([7116, 7116, 7117, 7117, 7118, 7118, 7119, 7119, 7120, 7120, 7121,
                                                                    7121, 7122, 7122, 7123, 7123, 7124, 7124, 7125, 7125, 7126, 7126,
                                                                    7127, 7127, 7128, 7128, 7129, 7129, 7130, 7130, 7131, 7131, 7132,
                                                                    7132, 7133, 7133, 7134, 7134, 7135, 7135, 7136, 7136, 7137, 7137,
                                                                    7138, 7138, 7139, 7139, 7140, 7140, 7141, 7141, 7142, 7142, 7143,
                                                                    7143, 7144, 7144, 7145, 7145, 7146, 7146, 7147, 7147, 7148, 7148])
     
-    assert (np.abs(ts_ext_prediction_main_HWLWno['HWLWno'].values - expected_ts_ext_prediction_main_HWLWno_HWLWno) < 10E-9).all()
-    assert (np.abs(ts_ext_prediction_main['HWLWcode'].values - expected_ts_ext_prediction_main_HWLWcode) < 10E-9).all()
-    #assert (np.abs(ts_ext_prediction_all['HWLWcode'].values - expected_ts_ext_prediction_all_HWLWcode) < 10E-9).all()
-    assert (np.abs(ts_ext_prediction_clean_HWLWno['HWLWcode'].values - expected_ts_ext_prediction_clean_HWLWno_HWLWcode) < 10E-9).all()
-    assert (np.abs(ts_ext_prediction_clean_HWLWno['HWLWno'].values - expected_ts_ext_prediction_clean_HWLWno_HWLWno) < 10E-9).all()
+    assert np.allclose(ts_ext_prediction_main_HWLWno['HWLWno'].values, expected_ts_ext_prediction_main_HWLWno_HWLWno)
+    assert np.allclose(ts_ext_prediction_main['HWLWcode'].values, expected_ts_ext_prediction_main_HWLWcode)
+    assert np.allclose(ts_ext_prediction_clean_tomain['HWLWcode'].values, expected_ts_ext_prediction_main_HWLWcode)
+    assert np.allclose(ts_ext_prediction_clean_HWLWno['HWLWcode'].values, expected_ts_ext_prediction_clean_HWLWno_HWLWcode)
+    assert np.allclose(ts_ext_prediction_clean_HWLWno['HWLWno'].values, expected_ts_ext_prediction_clean_HWLWno_HWLWno)
+
 
+@pytest.mark.systemtest
+def test_hwlw_numbering_aggers():
+    """
+    This is probably already tested with other hwlw tests
+    """
+    
+    times_pred = slice(dt.datetime(2010,1,31,3),dt.datetime(2010,2,17,12), "1min") #longer period with alternating aggers and no aggers, also eerste HW wordt als lokaal ipv primair HW gezien, also extra agger outside of 1stLW/agger/2ndLW sequence
+    #HOEKVHLD has alternating aggers, DENHDR has double HW's
+    expect_345_len = {'HOEKVHLD':99,'DENHDR':66}
+    expect_345_code_sum = {'HOEKVHLD':267,'DENHDR':99}
+    expect_345_nos_sum = {'HOEKVHLD':706061,'DENHDR':470712}
+    
+    for current_station in expect_345_len.keys():
+    
+        file_data_comp0 = os.path.join(dir_testdata,'%s_ana.txt'%(current_station))
+        comp_merged = hatyan.read_components(filename=file_data_comp0)
+        
+        ts_prediction_HWLWno = hatyan.prediction(comp=comp_merged, times=times_pred)
+        ts_ext_prediction_345 = hatyan.calc_HWLW(ts=ts_prediction_HWLWno, calc_HWLW345=True)
+        ts_ext_prediction_345_HWLWno = hatyan.calc_HWLWnumbering(ts_ext=ts_ext_prediction_345, station=current_station)
+        
+        assert len(ts_ext_prediction_345_HWLWno) == expect_345_len[current_station]
+        assert ts_ext_prediction_345_HWLWno["HWLWcode"].sum() == expect_345_code_sum[current_station]
+        assert ts_ext_prediction_345_HWLWno["HWLWno"].sum() == expect_345_nos_sum[current_station]
+        
+        fig, (ax1,ax2) = hatyan.plot_timeseries(ts=ts_prediction_HWLWno, ts_ext=ts_ext_prediction_345)
+        for irow, pdrow in ts_ext_prediction_345_HWLWno.iterrows():
+            ax1.text(pdrow.name,pdrow['values'],pdrow['HWLWno'].astype(int))
+        ax1.set_ylim(-1.2,1.7)
+        hatyan.close()
+        
 
 @pytest.mark.systemtest
 def test_19Ycomp4Ydia():
     # 1. define test data
     nodalfactors = True
     xfac = True
     const_list = hatyan.get_const_list_hatyan('year')
     current_station = 'VLISSGN'
     
     #comp0
-    file_data_comp0 = [os.path.join(dir_testdata,'%s_obs%i.txt'%(current_station, file_id)) for file_id in [1,2,3,4]]
-    ts_measurements_group0 = hatyan.readts_dia(filename=file_data_comp0, station=current_station)
-    comp_frommeasurements_avg_group0 = hatyan.get_components_from_ts(ts=ts_measurements_group0, const_list=const_list, nodalfactors=nodalfactors, xfac=xfac, fu_alltimes=False, analysis_perperiod='Y')
+    file_data_comp0 = os.path.join(dir_testdata,f'{current_station}_obs?.txt')
+    ts_measurements_group0 = hatyan.read_dia(filename=file_data_comp0, station=current_station)
+    comp_frommeasurements_avg_group0 = hatyan.analysis(ts=ts_measurements_group0, const_list=const_list, nodalfactors=nodalfactors, xfac=xfac, fu_alltimes=False, analysis_perperiod='Y')
     comp_frommeasurements_avg_group0.station = current_station
     
     #comp1
     file_data_comp1 = os.path.join(dir_testdata,'%s_ana.txt'%(current_station))
     comp_fromfile_group1 = hatyan.read_components(filename=file_data_comp1)
     
     #merge component groups (SA/SM from 19Y, rest from 4Y)
-    COMP_merged = hatyan.merge_componentgroups(comp_main=comp_frommeasurements_avg_group0, comp_sec=comp_fromfile_group1, comp_sec_list=['SA','SM'])
+    COMP_merged = hatyan.merge_componentgroups(comp_main=comp_frommeasurements_avg_group0, comp_sec=comp_fromfile_group1.loc[['SA','SM']])
     
     #prediction and validation
-    times_ext_pred = [dt.datetime(2019,1,1),dt.datetime(2019,1,1,12)]
-    times_step_pred = 10
-    ts_prediction = hatyan.prediction(COMP_merged, nodalfactors=nodalfactors, xfac=xfac, fu_alltimes=False, times_ext=times_ext_pred, timestep_min=times_step_pred)
+    times_pred = slice(dt.datetime(2019,1,1),dt.datetime(2019,1,1,12), "10min")
+    ts_prediction = hatyan.prediction(COMP_merged, times=times_pred)
     ts_prediction_values = ts_prediction['values'].values
     
     # 2. define initial expectations (VLISSGN)
     expected_ts_prediction_data_pd_values = np.array([1.00071654,  0.88827903,  0.76819314,  0.64141558,  0.5093034 ,
                                                       0.37343441,  0.23542045,  0.09675753, -0.04125568, -0.17751967,
                                                      -0.31106673, -0.44095367, -0.56615373, -0.68548689, -0.79761632,
                                                      -0.9011202 , -0.99462701, -1.07698355, -1.14741452, -1.2056322 ,
@@ -678,33 +476,34 @@
 def test_19Ycomp4Ydia_compsplitsing():
     # 1. define test data
     nodalfactors = True
     xfac = False
     const_list = hatyan.get_const_list_hatyan('month')
     current_station = 'D15'
     file_data_comp0 = os.path.join(dir_testdata,'%s_obs1.txt'%(current_station))
-    CS_comps = pd.DataFrame({'CS_comps_from':['K1','N2','2MN2','S2','S2'],
+    cs_comps = pd.DataFrame({'CS_comps_from':['K1','N2','2MN2','S2','S2'],
                              'CS_comps_derive':['P1','NU2','LABDA2','K2','T2'],
                              'CS_ampfacs':[0.33,0.22,0.48,0.29,0.05],
                              'CS_degincrs':[-11,-24,174,1,-24]})
     file_data_comp1 = os.path.join(dir_testdata,'%s_ana.txt'%(current_station))
-    times_ext_pred = [dt.datetime(2019,1,1),dt.datetime(2019,1,1,12)]
-    times_step_pred = 10
+    times_pred = slice(dt.datetime(2019,1,1),dt.datetime(2019,1,1,12), "10min")
     
     # 3. run test
     #component groups
-    ts_measurements_group0 = hatyan.readts_dia(filename=file_data_comp0, station=current_station)
-    comp_frommeasurements_avg_group0 = hatyan.get_components_from_ts(ts=ts_measurements_group0, nodalfactors=nodalfactors, xfac=xfac, const_list=const_list, analysis_perperiod=False, fu_alltimes=False, CS_comps=CS_comps)
+    ts_measurements_group0 = hatyan.read_dia(filename=file_data_comp0, station=current_station)
+    comp_frommeasurements_avg_group0 = hatyan.analysis(ts=ts_measurements_group0, nodalfactors=nodalfactors, xfac=xfac, 
+                                                       const_list=const_list, analysis_perperiod=False, fu_alltimes=False, 
+                                                       cs_comps=cs_comps)
     comp_fromfile_group1 = hatyan.read_components(filename=file_data_comp1)
     
     #merge component groups (SA/SM from 19Y, rest from 4Y)
-    COMP_merged = hatyan.merge_componentgroups(comp_main=comp_frommeasurements_avg_group0, comp_sec=comp_fromfile_group1, comp_sec_list=['SA','SM'])
+    COMP_merged = hatyan.merge_componentgroups(comp_main=comp_frommeasurements_avg_group0, comp_sec=comp_fromfile_group1.loc[['SA','SM']])
     
     #prediction and validation
-    ts_prediction = hatyan.prediction(COMP_merged, nodalfactors=nodalfactors, xfac=xfac, fu_alltimes=False, times_ext=times_ext_pred, timestep_min=times_step_pred)
+    ts_prediction = hatyan.prediction(COMP_merged, times=times_pred)
     ts_prediction_values = ts_prediction['values'].values
     
     # 2. define initial expectations (D15)
     expected_ts_prediction_data_pd_values = np.array([0.21208738,  0.26853271,  0.32342168,  0.37563977,  0.4242852 ,
                                                       0.46874611,  0.50873038,  0.54424431,  0.57552477,  0.60293749,
                                                       0.6268598 ,  0.64756857,  0.66515311,  0.67946822,  0.69013541,
                                                       0.69659205,  0.6981796 ,  0.69425554,  0.68430933,  0.66806236,
@@ -717,40 +516,39 @@
                                                      -0.59205869, -0.61124872, -0.62760946, -0.64057802, -0.64961524,
                                                      -0.65429615, -0.65438144, -0.64985669, -0.64093152, -0.62799831,
                                                      -0.61155776, -0.59212467, -0.57013128, -0.54584644, -0.5193262 ,
                                                      -0.49040627, -0.45873912, -0.42387076, -0.38534492, -0.3428169 ,
                                                      -0.29615745, -0.24552815, -0.19141437])
     
     # 4. Vefiry final expectations
-    assert (np.abs(ts_prediction_values - expected_ts_prediction_data_pd_values) < 10E-9).all()        
+    assert (np.abs(ts_prediction_values - expected_ts_prediction_data_pd_values) < 10E-9).all()
 
 
 @pytest.mark.systemtest
 def test_allfromdia():
     # 1. define test data
     nodalfactors = True
     xfac = True
     const_list = hatyan.get_const_list_hatyan('year')
     current_station = 'VLISSGN'
     file_data_comp0 = [os.path.join(dir_testdata,'%s_obs%i.txt'%(current_station, file_id)) for file_id in [1,2,3,4]]
     file_data_comp1 = os.path.join(dir_testdata,'%s_obs19.txt'%(current_station))
-    times_ext_pred = [dt.datetime(2019,1,1),dt.datetime(2019,1,1,12)]
-    times_step_pred = 10
+    times_pred = slice(dt.datetime(2019,1,1),dt.datetime(2019,1,1,12), "10min")
 
     #component groups
-    ts_measurements_group0 = hatyan.readts_dia(filename=file_data_comp0, station=current_station)
-    comp_frommeasurements_avg_group0 = hatyan.get_components_from_ts(ts=ts_measurements_group0, nodalfactors=nodalfactors, xfac=xfac, const_list=const_list, analysis_perperiod='Y', fu_alltimes=False)
-    ts_measurements_group1 = hatyan.readts_dia(filename=file_data_comp1, station=current_station)
-    comp_frommeasurements_avg_group1 = hatyan.get_components_from_ts(ts=ts_measurements_group1, nodalfactors=nodalfactors, xfac=xfac, const_list=const_list, analysis_perperiod=False, fu_alltimes=False)
+    ts_measurements_group0 = hatyan.read_dia(filename=file_data_comp0, station=current_station)
+    comp_frommeasurements_avg_group0 = hatyan.analysis(ts=ts_measurements_group0, nodalfactors=nodalfactors, xfac=xfac, const_list=const_list, analysis_perperiod='Y', fu_alltimes=False)
+    ts_measurements_group1 = hatyan.read_dia(filename=file_data_comp1, station=current_station)
+    comp_frommeasurements_avg_group1 = hatyan.analysis(ts=ts_measurements_group1, nodalfactors=nodalfactors, xfac=xfac, const_list=const_list, analysis_perperiod=False, fu_alltimes=False)
     
     #merge component groups (SA/SM from 19Y, rest from 4Y)
-    COMP_merged = hatyan.merge_componentgroups(comp_main=comp_frommeasurements_avg_group0, comp_sec=comp_frommeasurements_avg_group1, comp_sec_list=['SA','SM'])
+    COMP_merged = hatyan.merge_componentgroups(comp_main=comp_frommeasurements_avg_group0, comp_sec=comp_frommeasurements_avg_group1.loc[['SA','SM']])
     
     #prediction and validation
-    ts_prediction = hatyan.prediction(COMP_merged, nodalfactors=nodalfactors, xfac=xfac, fu_alltimes=False, times_ext=times_ext_pred, timestep_min=times_step_pred)
+    ts_prediction = hatyan.prediction(COMP_merged, times=times_pred)
     ts_prediction_values = ts_prediction['values'].values
     
     # 2. define initial expectations
     """expected_ts_prediction_data_pd_values_CADZD = np.array([  0.69689822,  0.58122683,  0.46063218,  0.3366989 ,  0.21084484,
                                                         0.08416485, -0.04259883, -0.16895802, -0.29448491, -0.41858223,
                                                        -0.54028668, -0.65816757, -0.77035852, -0.87472565, -0.96913982,
                                                        -1.05179199, -1.12147718, -1.17777783, -1.22109997, -1.25255039,
@@ -790,23 +588,22 @@
 def test_allfromdia_2008xfac0():
     # 1. define test data
     nodalfactors = True
     xfac = False
     const_list = hatyan.get_const_list_hatyan('year')
     current_station = 'DOVR'
     file_data_comp0 = os.path.join(dir_testdata,'%s_obs1.txt'%(current_station))
-    times_ext_pred = [dt.datetime(2019,1,1),dt.datetime(2019,1,1,12)]
-    times_step_pred = 10
+    times_pred = slice(dt.datetime(2019,1,1),dt.datetime(2019,1,1,12), "10min")
     
     #component groups
-    ts_measurements_group0 = hatyan.readts_dia(filename=file_data_comp0, station=current_station)
-    comp_frommeasurements_avg_group0 = hatyan.get_components_from_ts(ts=ts_measurements_group0, nodalfactors=nodalfactors, xfac=xfac, const_list=const_list, analysis_perperiod='Y', fu_alltimes=False)
+    ts_measurements_group0 = hatyan.read_dia(filename=file_data_comp0, station=current_station)
+    comp_frommeasurements_avg_group0 = hatyan.analysis(ts=ts_measurements_group0, nodalfactors=nodalfactors, xfac=xfac, const_list=const_list, analysis_perperiod='Y', fu_alltimes=False)
     
     #prediction and validation
-    ts_prediction = hatyan.prediction(comp=comp_frommeasurements_avg_group0, nodalfactors=nodalfactors, xfac=xfac, fu_alltimes=False, times_ext=times_ext_pred, timestep_min=times_step_pred)
+    ts_prediction = hatyan.prediction(comp=comp_frommeasurements_avg_group0, times=times_pred)
     ts_prediction_values = ts_prediction['values'].values
     
     # 2. define initial expectations
     expected_ts_prediction_data_pd_values = np.array([-0.60440198, -0.72142681, -0.83581976, -0.94743404, -1.05609766,
                                                       -1.1615773 , -1.2635405 , -1.36152022, -1.45488748, -1.54283832,
                                                       -1.62440113, -1.69846786, -1.76384908, -1.81934804, -1.86384401,
                                                       -1.89637159, -1.91618096, -1.92276574, -1.91584961, -1.89533042,
@@ -822,33 +619,7 @@
                                                        0.63180616,  0.49996392,  0.36753791,  0.23525891,  0.10363497,
                                                       -0.02704478, -0.15668462, -0.28533886])
     
     # 4. Vefiry final expectations
     assert (np.abs(ts_prediction_values - expected_ts_prediction_data_pd_values) < 10E-9).all()
 
 
-@pytest.mark.acceptance
-def test_DDL_QCvalues():
-    tstart_dt = dt.datetime(2019,10,1)
-    tstop_dt = dt.datetime(2019,10,10)
-    tzone = 'UTC+00:00' #'UTC+00:00' for GMT and 'UTC+01:00' for MET
-    
-    catalog_dict = hatyan.get_DDL_catalog(catalog_extrainfo=['WaardeBepalingsmethoden','MeetApparaten','Typeringen'])
-    
-    #HARVT10
-    cat_locatielijst = catalog_dict['LocatieLijst']#.set_index('Locatie_MessageID',drop=True)
-    station_dict = cat_locatielijst[cat_locatielijst['Code']=='HARVT10'].iloc[0]
-    ts_meas_pd, metadata, stationdata = hatyan.get_DDL_data(station_dict=station_dict,tstart_dt=tstart_dt,tstop_dt=tstop_dt,tzone=tzone,
-                                                            meta_dict={'Grootheid.Code':'WATHTE','Groepering.Code':'NVT','WaardeBewerkingsmethode.Code':'NVT'})
-    uniqueQC = ts_meas_pd['QC'].unique() #array([ 0., 99., nan, 25.]), but should be integers without nan array([0, 99, 25])
-    assert uniqueQC.dtype=='float64' #this should be int in the future, if None/nan is not in QC list anymore
-    assert np.isnan(uniqueQC).sum() == 1 #this one should become 0 in the future and then the second assertion should be valid without indexing
-    assert (uniqueQC[~np.isnan(uniqueQC)] == np.array([ 0, 99, 25])).all()
-
-    #STELLDBTN
-    station_dict = cat_locatielijst[cat_locatielijst['Code']=='STELLDBTN'].iloc[0]
-    ts_meas_pd, metadata, stationdata = hatyan.get_DDL_data(station_dict=station_dict,tstart_dt=tstart_dt,tstop_dt=tstop_dt,tzone=tzone,
-                                                            meta_dict={'Grootheid.Code':'WATHTE','Groepering.Code':'NVT','WaardeBewerkingsmethode.Code':'NVT'})
-    uniqueQC = ts_meas_pd['QC'].unique() #array([ 0, 25], dtype=int8)
-    assert uniqueQC.dtype=='int8'
-    assert (uniqueQC == np.array([ 0, 25])).all()
-
```

