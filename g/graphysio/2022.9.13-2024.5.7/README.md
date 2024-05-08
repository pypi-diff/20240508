# Comparing `tmp/graphysio-2022.9.13.tar.gz` & `tmp/graphysio-2024.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphysio-2022.9.13.tar", max compression
+gzip compressed data, was "graphysio-2024.5.7.tar", max compression
```

## Comparing `graphysio-2022.9.13.tar` & `graphysio-2024.5.7.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0      750 2019-03-28 09:53:36.213435 graphysio-2022.9.13/LICENSE
--rw-r--r--   0        0        0      817 2022-07-06 20:01:27.455451 graphysio-2022.9.13/README.md
--rw-r--r--   0        0        0      232 2022-06-26 19:35:04.260080 graphysio-2022.9.13/graphysio/__init__.py
--rw-r--r--   0        0        0       62 2021-01-05 09:14:52.946469 graphysio-2022.9.13/graphysio/__main__.py
--rw-r--r--   0        0        0       34 2021-01-05 09:03:42.054048 graphysio-2022.9.13/graphysio/algorithms/__init__.py
--rw-r--r--   0        0        0     9214 2022-03-15 09:26:57.909487 graphysio-2022.9.13/graphysio/algorithms/filters.py
--rw-r--r--   0        0        0     6667 2022-06-25 21:48:35.242539 graphysio-2022.9.13/graphysio/algorithms/waveform.py
--rw-r--r--   0        0        0    16102 2022-06-25 21:38:20.030660 graphysio-2022.9.13/graphysio/dialogs.py
--rw-r--r--   0        0        0      531 2021-01-05 09:03:42.054048 graphysio-2022.9.13/graphysio/legend.py
--rw-r--r--   0        0        0      203 2021-01-05 09:14:52.946469 graphysio-2022.9.13/graphysio/main.py
--rw-r--r--   0        0        0     5527 2022-07-18 13:39:28.978612 graphysio-2022.9.13/graphysio/mainui.py
--rw-r--r--   0        0        0      437 2022-07-05 08:21:04.145573 graphysio-2022.9.13/graphysio/plotwidgets/__init__.py
--rw-r--r--   0        0        0     9519 2022-09-13 12:44:25.672923 graphysio-2022.9.13/graphysio/plotwidgets/curves.py
--rw-r--r--   0        0        0     5464 2022-07-07 21:03:50.819750 graphysio-2022.9.13/graphysio/plotwidgets/plotwidget.py
--rw-r--r--   0        0        0     5304 2022-07-18 13:39:28.978612 graphysio-2022.9.13/graphysio/plotwidgets/poiselector.py
--rw-r--r--   0        0        0     4895 2022-07-18 13:39:28.978612 graphysio-2022.9.13/graphysio/plotwidgets/puplot.py
--rw-r--r--   0        0        0     5236 2022-07-05 08:22:48.518453 graphysio-2022.9.13/graphysio/plotwidgets/spectrogram.py
--rw-r--r--   0        0        0     9788 2022-09-12 14:44:12.242219 graphysio-2022.9.13/graphysio/plotwidgets/tsplot.py
--rw-r--r--   0        0        0     1265 2022-06-25 21:40:27.593723 graphysio-2022.9.13/graphysio/readdata/__init__.py
--rw-r--r--   0        0        0      292 2020-05-22 09:22:57.526000 graphysio-2022.9.13/graphysio/readdata/baseclass.py
--rw-r--r--   0        0        0     9891 2022-07-07 21:24:29.489726 graphysio-2022.9.13/graphysio/readdata/csv.py
--rw-r--r--   0        0        0     1701 2021-08-09 10:40:54.698935 graphysio-2022.9.13/graphysio/readdata/edf.py
--rw-r--r--   0        0        0     1066 2022-07-07 21:27:41.467684 graphysio-2022.9.13/graphysio/readdata/parquet.py
--rw-r--r--   0        0        0     1118 2022-07-18 13:39:28.978612 graphysio-2022.9.13/graphysio/structures.py
--rw-r--r--   0        0        0      282 2022-09-13 12:46:56.489565 graphysio-2022.9.13/graphysio/transformations/__init__.py
--rw-r--r--   0        0        0      916 2022-09-13 09:58:05.446202 graphysio-2022.9.13/graphysio/transformations/feet_to_curve.py
--rw-r--r--   0        0        0     1562 2022-09-13 12:38:38.083443 graphysio-2022.9.13/graphysio/transformations/perfusion_index.py
--rw-r--r--   0        0        0     1644 2022-09-13 12:40:12.047843 graphysio-2022.9.13/graphysio/transformations/precise_feet.py
--rw-r--r--   0        0        0      438 2021-01-05 09:14:52.954469 graphysio-2022.9.13/graphysio/ui/__init__.py
--rw-r--r--   0        0        0      181 2022-07-18 13:39:28.978612 graphysio-2022.9.13/graphysio/ui/convert_ui_to_py.sh
--rw-r--r--   0        0        0    16038 2022-07-18 13:39:28.982612 graphysio-2022.9.13/graphysio/ui/csvrequest.py
--rw-r--r--   0        0        0    14702 2022-07-07 21:16:27.251901 graphysio-2022.9.13/graphysio/ui/csvrequest.ui
--rw-r--r--   0        0        0     6247 2022-07-18 13:39:28.982612 graphysio-2022.9.13/graphysio/ui/curveproperties.py
--rw-r--r--   0        0        0     4481 2019-05-24 13:11:00.148482 graphysio-2022.9.13/graphysio/ui/curveproperties.ui
--rw-r--r--   0        0        0     2724 2022-07-18 13:39:28.982612 graphysio-2022.9.13/graphysio/ui/curveselect.py
--rw-r--r--   0        0        0     1650 2019-03-18 12:32:13.063040 graphysio-2022.9.13/graphysio/ui/curveselect.ui
--rw-r--r--   0        0        0     1822 2022-07-18 13:39:28.982612 graphysio-2022.9.13/graphysio/ui/cycledetect.py
--rw-r--r--   0        0        0     1096 2019-03-18 12:32:13.063040 graphysio-2022.9.13/graphysio/ui/cycledetect.ui
--rw-r--r--   0        0        0     4007 2022-07-18 13:39:28.982612 graphysio-2022.9.13/graphysio/ui/datetime.py
--rw-r--r--   0        0        0     4121 2019-05-24 13:18:41.917107 graphysio-2022.9.13/graphysio/ui/datetime.ui
--rw-r--r--   0        0        0     1920 2022-07-18 13:39:28.982612 graphysio-2022.9.13/graphysio/ui/filter.py
--rw-r--r--   0        0        0     1241 2019-03-18 12:32:13.063040 graphysio-2022.9.13/graphysio/ui/filter.ui
--rw-r--r--   0        0        0     5927 2022-07-18 13:39:28.982612 graphysio-2022.9.13/graphysio/ui/loopwidget.py
--rw-r--r--   0        0        0     5748 2019-03-18 12:32:13.063040 graphysio-2022.9.13/graphysio/ui/loopwidget.ui
--rw-r--r--   0        0        0     3337 2022-07-18 13:39:28.982612 graphysio-2022.9.13/graphysio/ui/mainwindow.py
--rw-r--r--   0        0        0     2700 2019-05-23 08:03:05.751959 graphysio-2022.9.13/graphysio/ui/mainwindow.ui
--rw-r--r--   0        0        0     7158 2022-07-18 13:39:28.982612 graphysio-2022.9.13/graphysio/ui/periodexport.py
--rw-r--r--   0        0        0     4987 2019-03-18 12:32:13.067040 graphysio-2022.9.13/graphysio/ui/periodexport.ui
--rw-r--r--   0        0        0     3459 2022-07-18 13:39:28.982612 graphysio-2022.9.13/graphysio/ui/poiwidget.py
--rw-r--r--   0        0        0     2999 2020-05-28 13:00:26.648398 graphysio-2022.9.13/graphysio/ui/poiwidget.ui
--rw-r--r--   0        0        0     2842 2022-07-18 13:39:28.982612 graphysio-2022.9.13/graphysio/ui/setuppuloop.py
--rw-r--r--   0        0        0     1862 2019-03-18 12:32:13.067040 graphysio-2022.9.13/graphysio/ui/setuppuloop.ui
--rw-r--r--   0        0        0     2247 2022-07-05 08:21:28.817780 graphysio-2022.9.13/graphysio/utils.py
--rw-r--r--   0        0        0      342 2021-08-09 13:12:21.542483 graphysio-2022.9.13/graphysio/writedata/__init__.py
--rwxr-xr-x   0        0        0      470 2021-08-09 17:59:06.654626 graphysio-2022.9.13/graphysio/writedata/csv.py
--rw-r--r--   0        0        0     2096 2022-07-07 20:56:23.258565 graphysio-2022.9.13/graphysio/writedata/edf.py
--rwxr-xr-x   0        0        0     6357 2021-01-05 09:14:52.982470 graphysio-2022.9.13/graphysio/writedata/exporter.py
--rw-r--r--   0        0        0      473 2021-08-09 17:58:53.667685 graphysio-2022.9.13/graphysio/writedata/matlab.py
--rwxr-xr-x   0        0        0      610 2022-06-26 18:24:15.272525 graphysio-2022.9.13/graphysio/writedata/parquet.py
--rw-r--r--   0        0        0      977 2022-09-13 12:49:18.966172 graphysio-2022.9.13/pyproject.toml
--rw-r--r--   0        0        0     1922 2022-09-13 12:50:27.320481 graphysio-2022.9.13/setup.py
--rw-r--r--   0        0        0     1776 2022-09-13 12:50:27.320822 graphysio-2022.9.13/PKG-INFO
+-rw-r--r--   0        0        0      750 2019-03-28 09:53:36.213435 graphysio-2024.5.7/LICENSE
+-rw-r--r--   0        0        0      817 2022-07-06 20:01:27.455451 graphysio-2024.5.7/README.md
+-rw-r--r--   0        0        0      232 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/__init__.py
+-rw-r--r--   0        0        0      516 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/__main__.py
+-rw-r--r--   0        0        0       34 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/algorithms/__init__.py
+-rw-r--r--   0        0        0    10396 2023-11-14 20:24:04.333629 graphysio-2024.5.7/graphysio/algorithms/filters.py
+-rw-r--r--   0        0        0     6667 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/algorithms/waveform.py
+-rw-r--r--   0        0        0    16364 2024-05-07 15:42:35.125241 graphysio-2024.5.7/graphysio/dialogs.py
+-rw-r--r--   0        0        0      531 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/legend.py
+-rw-r--r--   0        0        0      211 2023-11-11 11:36:50.904021 graphysio-2024.5.7/graphysio/main.py
+-rw-r--r--   0        0        0     5661 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/mainui.py
+-rw-r--r--   0        0        0      437 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/plotwidgets/__init__.py
+-rw-r--r--   0        0        0     9681 2024-05-07 15:33:08.814579 graphysio-2024.5.7/graphysio/plotwidgets/curves.py
+-rw-r--r--   0        0        0     5461 2023-11-22 11:41:06.571840 graphysio-2024.5.7/graphysio/plotwidgets/plotwidget.py
+-rw-r--r--   0        0        0     5302 2023-11-14 20:11:39.125200 graphysio-2024.5.7/graphysio/plotwidgets/poiselector.py
+-rw-r--r--   0        0        0     4895 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/plotwidgets/puplot.py
+-rw-r--r--   0        0        0     5236 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/plotwidgets/spectrogram.py
+-rw-r--r--   0        0        0     9698 2023-11-14 20:11:19.909073 graphysio-2024.5.7/graphysio/plotwidgets/tsplot.py
+-rw-r--r--   0        0        0     1265 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/readdata/__init__.py
+-rw-r--r--   0        0        0      292 2020-05-22 09:22:57.526000 graphysio-2024.5.7/graphysio/readdata/baseclass.py
+-rw-r--r--   0        0        0    10332 2024-05-07 15:44:26.754416 graphysio-2024.5.7/graphysio/readdata/csv.py
+-rw-r--r--   0        0        0     1701 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/readdata/edf.py
+-rw-r--r--   0        0        0     1069 2024-05-07 15:45:03.802800 graphysio-2024.5.7/graphysio/readdata/parquet.py
+-rw-r--r--   0        0        0     1251 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/structures.py
+-rw-r--r--   0        0        0      462 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/transformations/__init__.py
+-rw-r--r--   0        0        0      969 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/transformations/feet_time_interval.py
+-rw-r--r--   0        0        0      863 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/transformations/feet_to_curve.py
+-rw-r--r--   0        0        0     1512 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/transformations/perfusion_index.py
+-rw-r--r--   0        0        0     1587 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/transformations/precise_feet.py
+-rw-r--r--   0        0        0     1783 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/transformations/pulse_arrival_time.py
+-rw-r--r--   0        0        0      438 2021-01-05 09:14:52.954469 graphysio-2024.5.7/graphysio/ui/__init__.py
+-rw-r--r--   0        0        0      181 2022-07-18 13:39:28.978612 graphysio-2024.5.7/graphysio/ui/convert_ui_to_py.sh
+-rw-r--r--   0        0        0    16236 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/ui/csvrequest.py
+-rw-r--r--   0        0        0    14702 2022-07-07 21:16:27.251901 graphysio-2024.5.7/graphysio/ui/csvrequest.ui
+-rw-r--r--   0        0        0     6291 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/ui/curveproperties.py
+-rw-r--r--   0        0        0     4481 2019-05-24 13:11:00.148482 graphysio-2024.5.7/graphysio/ui/curveproperties.ui
+-rw-r--r--   0        0        0     2790 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/ui/curveselect.py
+-rw-r--r--   0        0        0     1650 2019-03-18 12:32:13.063040 graphysio-2024.5.7/graphysio/ui/curveselect.ui
+-rw-r--r--   0        0        0     1822 2022-07-18 13:39:28.982612 graphysio-2024.5.7/graphysio/ui/cycledetect.py
+-rw-r--r--   0        0        0     1096 2019-03-18 12:32:13.063040 graphysio-2024.5.7/graphysio/ui/cycledetect.ui
+-rw-r--r--   0        0        0     4117 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/ui/datetime.py
+-rw-r--r--   0        0        0     4121 2019-05-24 13:18:41.917107 graphysio-2024.5.7/graphysio/ui/datetime.ui
+-rw-r--r--   0        0        0     1920 2022-07-18 13:39:28.982612 graphysio-2024.5.7/graphysio/ui/filter.py
+-rw-r--r--   0        0        0     1241 2019-03-18 12:32:13.063040 graphysio-2024.5.7/graphysio/ui/filter.ui
+-rw-r--r--   0        0        0     6039 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/ui/loopwidget.py
+-rw-r--r--   0        0        0     5748 2019-03-18 12:32:13.063040 graphysio-2024.5.7/graphysio/ui/loopwidget.ui
+-rw-r--r--   0        0        0     3381 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/ui/mainwindow.py
+-rw-r--r--   0        0        0     2700 2019-05-23 08:03:05.751959 graphysio-2024.5.7/graphysio/ui/mainwindow.ui
+-rw-r--r--   0        0        0     7312 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/ui/periodexport.py
+-rw-r--r--   0        0        0     4987 2019-03-18 12:32:13.067040 graphysio-2024.5.7/graphysio/ui/periodexport.ui
+-rw-r--r--   0        0        0     3525 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/ui/poiwidget.py
+-rw-r--r--   0        0        0     2999 2020-05-28 13:00:26.648398 graphysio-2024.5.7/graphysio/ui/poiwidget.ui
+-rw-r--r--   0        0        0     2864 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/ui/setuppuloop.py
+-rw-r--r--   0        0        0     1862 2019-03-18 12:32:13.067040 graphysio-2024.5.7/graphysio/ui/setuppuloop.ui
+-rw-r--r--   0        0        0     2278 2023-11-14 20:09:24.028274 graphysio-2024.5.7/graphysio/utils.py
+-rw-r--r--   0        0        0      342 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/writedata/__init__.py
+-rwxr-xr-x   0        0        0      470 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/writedata/csv.py
+-rw-r--r--   0        0        0     2096 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/writedata/edf.py
+-rwxr-xr-x   0        0        0     6357 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/writedata/exporter.py
+-rw-r--r--   0        0        0      476 2024-05-07 15:45:25.551024 graphysio-2024.5.7/graphysio/writedata/matlab.py
+-rwxr-xr-x   0        0        0      624 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/writedata/parquet.py
+-rw-r--r--   0        0        0      923 2024-05-07 15:46:34.255726 graphysio-2024.5.7/pyproject.toml
+-rw-r--r--   0        0        0     1777 1970-01-01 00:00:00.000000 graphysio-2024.5.7/PKG-INFO
```

### Comparing `graphysio-2022.9.13/LICENSE` & `graphysio-2024.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `graphysio-2022.9.13/README.md` & `graphysio-2024.5.7/README.md`

 * *Files identical despite different names*

### Comparing `graphysio-2022.9.13/graphysio/algorithms/filters.py` & `graphysio-2024.5.7/graphysio/algorithms/filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,129 +1,134 @@
+from copy import copy
 from datetime import datetime
+from functools import reduce
 from math import floor
 from typing import Dict
 
 import numexpr as ne
 import numpy as np
 import pandas as pd
-from graphysio.structures import Filter, Parameter
-from graphysio.utils import truncatevecs
 from pint import UnitRegistry
 from scipy import interpolate, signal
 
+from graphysio.structures import Filter, Parameter
+from graphysio.utils import truncatevecs
+
 
 class TF(object):
-    def __init__(self, num, den, name=''):
+    def __init__(self, num, den, name=""):
         self.num = num
         self.den = den
         self.name = name
 
     def discretize(self, samplerate):
         systf = (self.num, self.den)
         (dnum, dden, _) = signal.cont2discrete(systf, 1 / samplerate)
         return (np.squeeze(dnum), np.squeeze(dden))
 
 
-interpkind = ['linear', 'zero', 'pchip', 'nearest']
+interpkind = ["linear", "zero", "pchip", "nearest"]
 Filters = {
-    'Lowpass filter': Filter(
-        name='lowpass',
+    "Lowpass filter": Filter(
+        name="lowpass",
         parameters=[
-            Parameter('Cutoff frequency (Hz)', int),
-            Parameter('Filter order', int),
+            Parameter("Cutoff frequency (Hz)", int),
+            Parameter("Filter order", int),
         ],
     ),
-    'Filter ventilation': Filter(name='ventilation', parameters=[]),
-    'Savitzky-Golay': Filter(
-        name='savgol',
+    "Filter ventilation": Filter(name="ventilation", parameters=[]),
+    "Savitzky-Golay": Filter(
+        name="savgol",
         parameters=[
-            Parameter('Window duration', 'time'),
-            Parameter('Polynomial order', int),
+            Parameter("Window duration", "time"),
+            Parameter("Polynomial order", int),
         ],
     ),
-    'Interpolate': Filter(
-        name='interp',
+    "Interpolate": Filter(
+        name="interp",
         parameters=[
-            Parameter('New sampling rate (Hz)', float),
-            Parameter('Interpolation type', interpkind),
+            Parameter("New sampling rate (Hz)", float),
+            Parameter("Interpolation type", interpkind),
         ],
     ),
-    'Doppler cut': Filter(
-        name='dopplercut', parameters=[Parameter('Minimum value', int)]
+    "Doppler cut": Filter(
+        name="dopplercut", parameters=[Parameter("Minimum value", int)]
     ),
-    'Differentiate': Filter(
-        name='diff',
-        parameters=[Parameter('Order', int), Parameter('Denominator time unit', str)],
+    "Differentiate": Filter(
+        name="diff",
+        parameters=[Parameter("Order", int), Parameter("Denominator time unit", str)],
     ),
-    'Integrate': Filter(
-        name='integrate', parameters=[Parameter('Window duration', 'time')]
+    "Integrate": Filter(
+        name="integrate", parameters=[Parameter("Window duration", "time")]
     ),
-    'Lag': Filter(name='lag', parameters=[Parameter('Time delta', 'time')]),
-    'Normalize': Filter(name='norm1', parameters=[]),
-    'Set start date/time': Filter(
-        name='setdatetime', parameters=[Parameter('DateTime', datetime)]
+    "Lag": Filter(name="lag", parameters=[Parameter("Time delta", "time")]),
+    "Normalize": Filter(name="norm1", parameters=[]),
+    "Set start date/time": Filter(
+        name="setdatetime", parameters=[Parameter("DateTime", datetime)]
     ),
-    'Tolerant Normalize': Filter(name='norm2', parameters=[]),
-    'Enter expression (variable = x)': Filter(
-        name='expression', parameters=[Parameter('Expression', str)]
+    "Tolerant Normalize": Filter(name="norm2", parameters=[]),
+    "Enter expression (variable = x)": Filter(
+        name="expression", parameters=[Parameter("Expression", str)]
     ),
-    'Strided Moving average': Filter(
-        name='sma', parameters=[Parameter('Window duration', 'time')]
+    "Strided Moving average": Filter(
+        name="sma", parameters=[Parameter("Window duration", "time")]
     ),
 }
 
 FeetFilters = {
-    'Short cycles': Filter(
-        name='shortcycles', parameters=[Parameter('Minimum duration', 'time')]
-    )
+    "Short cycles": Filter(
+        name="shortcycles", parameters=[Parameter("Minimum duration", "time")]
+    ),
+    "Extra feet": Filter(name="extrafeet", parameters=[]),
 }
 
 TFs: Dict[str, TF] = {}
 
 
 def updateTFs():
     tflist = list(TFs.keys())
     if not tflist:
         return
-    Filters['Transfer function'] = Filter(
-        name='tf', parameters=[Parameter('Transfer function', tflist)]
+    Filters["Transfer function"] = Filter(
+        name="tf", parameters=[Parameter("Transfer function", tflist)]
     )
 
 
+# -- Curve Filters --
 def norm1(series, samplerate, parameters):
     series -= np.mean(series)
     series /= np.max(series) - np.min(series)
-    newname = f'{series.name}-norm'
+    newname = f"{series.name}-norm"
     return (series.rename(newname), None)
 
 
 def norm2(series, samplerate, parameters):
     series -= np.mean(series)
     series /= np.std(series)
-    newname = f'{series.name}-norm'
+    newname = f"{series.name}-norm"
     return (series.rename(newname), None)
 
 
 def expression(series, samplerate, parameters):
     (express,) = parameters
     try:
-        filtered = ne.evaluate(express, local_dict={'x': series.to_numpy()})
+        filtered = ne.evaluate(express, local_dict={"x": series.to_numpy()})
     except Exception:
         filtered = None
-    newname = f'{series.name}-filtered'
+    newname = f"{series.name}-filtered"
     newseries = pd.Series(filtered, index=series.index, name=newname)
     return (newseries, None)
 
 
 def setdatetime(series, samplerate, parameters):
     (timestamp,) = parameters
     newseries = series.copy()
     diff = timestamp - newseries.index[0]
     newseries.index += diff
-    newseries = newseries.rename(f'{series.name}-{timestamp}')
+    newseries = newseries.rename(f"{series.name}-{timestamp}")
     return (newseries, None)
 
 
 def sma(series, samplerate, parameters):
     (window_s,) = parameters
     serarr = series.to_numpy()
     serlen = len(serarr)
@@ -131,160 +136,197 @@
     nwindows = floor(serlen / winsize)
     valstarts = np.arange(0, serlen - winsize, step=winsize)
     resiter = (
         np.mean(serarr[beg:end]) for beg, end in zip(valstarts, valstarts + winsize)
     )
     result = np.fromiter(resiter, dtype=np.float64, count=nwindows)
     locidx = winsize * np.arange(0, nwindows) + winsize // 2
-    newname = f'{series.name}-sma{window_s}s'
+    newname = f"{series.name}-sma{window_s}s"
     newseries = pd.Series(result, index=series.index[locidx], name=newname)
     newsamplerate = samplerate / winsize
     return (newseries, newsamplerate)
 
 
 def savgol(series, samplerate, parameters):
     window, order = parameters
     window = np.floor(window * samplerate)
     if not window % 2:
         # window is even, we need odd
         window += 1
     filtered = signal.savgol_filter(series.values, int(window), order)
-    newname = f'{series.name}-filtered'
+    newname = f"{series.name}-filtered"
     newseries = pd.Series(filtered, index=series.index, name=newname)
     return (newseries, None)
 
 
 def lag(series, samplerate, parameters):
     (timedelta,) = parameters
     nindex = series.index.values - timedelta * 1e9
-    newname = f'{series.name}-{timedelta}s'
+    newname = f"{series.name}-{timedelta}s"
     newseries = pd.Series(series.values, index=nindex, name=newname)
     return (newseries, None)
 
 
 def tf(series, samplerate, parameters):
     (filtname,) = parameters
     tf = TFs[filtname]
     b, a = tf.discretize(samplerate)
     filtered = signal.lfilter(b, a, series)
-    newname = f'{series.name}-{tf.name}'
+    newname = f"{series.name}-{tf.name}"
     newseries = pd.Series(filtered, index=series.index, name=newname)
     return (newseries, None)
 
 
 def lowpass(series, samplerate, parameters):
     Fc, order = parameters
     Wn = Fc * 2 / samplerate
     b, a = signal.butter(order, Wn)
     filtered = signal.lfilter(b, a, series)
-    newname = f'{series.name}-lp{Fc}'
+    newname = f"{series.name}-lp{Fc}"
     newseries = pd.Series(filtered, index=series.index, name=newname)
     return (newseries, None)
 
 
 def ventilation(series, samplerate, parameters):
     order = 12
     # Filter between 10 and 20 per minute
     bornes_hz = np.array([10, 20]) / 60
     Wn = [Fc * 2 / samplerate for Fc in bornes_hz]
-    b, a = signal.butter(order, Wn, btype='bandstop')
+    b, a = signal.butter(order, Wn, btype="bandstop")
     filtered = signal.filtfilt(b, a, series.values)
-    newname = f'{series.name}-novent'
+    newname = f"{series.name}-novent"
     newseries = pd.Series(filtered, index=series.index, name=newname)
     return (newseries, None)
 
 
 def interp(series, samplerate, parameters):
     newsamplerate, method = parameters
     oldidx = series.index
-    if method == 'pchip':
+    if method == "pchip":
         f = interpolate.PchipInterpolator(oldidx, series.values, extrapolate=True)
     else:
         f = interpolate.interp1d(
-            oldidx, series.values, kind=method, fill_value='extrapolate'
+            oldidx, series.values, kind=method, fill_value="extrapolate"
         )
     step = 1e9 / newsamplerate  # 1e9 to convert Hz to ns
     newidx = np.arange(oldidx[0], oldidx[-1], step, dtype=np.int64)
     resampled = f(newidx)
-    newname = f'{series.name}-{newsamplerate}Hz'
+    newname = f"{series.name}-{newsamplerate}Hz"
     newseries = pd.Series(resampled, index=newidx, name=newname)
     return (newseries, newsamplerate)
 
 
 def dopplercut(series, samplerate, parameters):
     (minvel,) = parameters
     (notlow,) = (series < minvel).to_numpy().nonzero()
-    newname = f'{series.name}-{minvel}+'
+    newname = f"{series.name}-{minvel}+"
     newseries = series.rename(newname)
     newseries.iloc[notlow] = 0
     return (newseries, None)
 
 
 def integrate(series, samplerate, parameters):
     (duration,) = parameters
     window = int(np.floor(duration * samplerate))
     integrated = series.rolling(window, center=True).sum()
-    newname = f'{series.name}-integrate{duration}s'
+    newname = f"{series.name}-integrate{duration}s"
     newseries = integrated.rename(newname)
     return (newseries, None)
 
 
 def diff(series, samplerate, parameters):
     (order, timeunit) = parameters
     timeunit = timeunit.strip()
     dy = np.diff(series.values, order)
     dt = np.diff(series.index.values, order)
     ureg = UnitRegistry()
     ptu = ureg.parse_expression(timeunit)
     conv = ptu.to(ureg.nanosecond).magnitude
     dt = dt.astype(float) / conv
     diffed = dy / dt
-    newname = f'{series.name}-diff{order}(/{timeunit})'
+    newname = f"{series.name}-diff{order}(/{timeunit})"
     newseries = pd.Series(diffed, index=series.index[order:], name=newname)
     return (newseries, None)
 
 
 filtfuncs = {
-    'savgol': savgol,
-    'lag': lag,
-    'tf': tf,
-    'sma': sma,
-    'lowpass': lowpass,
-    'ventilation': ventilation,
-    'interp': interp,
-    'dopplercut': dopplercut,
-    'integrate': integrate,
-    'diff': diff,
-    'norm1': norm1,
-    'norm2': norm2,
-    'expression': expression,
-    'setdatetime': setdatetime,
+    "savgol": savgol,
+    "lag": lag,
+    "tf": tf,
+    "sma": sma,
+    "lowpass": lowpass,
+    "ventilation": ventilation,
+    "interp": interp,
+    "dopplercut": dopplercut,
+    "integrate": integrate,
+    "diff": diff,
+    "norm1": norm1,
+    "norm2": norm2,
+    "expression": expression,
+    "setdatetime": setdatetime,
 }
 
 
 def filter(curve, filtname, paramgetter):
     samplerate = curve.samplerate
     series = curve.series
     filt = Filters[filtname]
     parameters = map(paramgetter, filt.parameters)
     return filtfuncs[filt.name](series, samplerate, parameters)
 
 
-def filterFeet(starts, stops, filtname, paramgetter):
+# -- Feet Filters --
+def shortcycles(feetdict, samplerate, parameters):
+    starts = feetdict["start"]
+    stops = feetdict["stop"]
+    if len(stops) < 1:
+        # No stop information
+        raise ValueError("No stop feet")
+    (minimum_duration,) = parameters
+    minimum_cycle_len = minimum_duration * 1e9  # Transform to ns
+    cycle_durations = (stop - start for start, stop in zip(starts, stops))
+    boolidx = [d >= minimum_cycle_len for d in cycle_durations]
+    starts, stops, boolidx = truncatevecs([starts, stops, boolidx])
+    feetdict["start"] = starts[boolidx]
+    feetdict["stop"] = stops[boolidx]
+    return feetdict
+
+
+def extrafeet(feetdict, samplerate, parameters):
+    starts = feetdict["start"]
+    interval_quant_lo, median_interval, interval_quant_hi = (
+        starts.to_series().diff().quantile([0.1, 0.5, 0.9])
+    )
+    interval_iqr = interval_quant_hi - interval_quant_lo
+
+    # Construct a list of acceptable locations
+    masks = []
+    pos = starts[0]
+    while True:
+        lo = pos - interval_iqr // 2
+        hi = pos + interval_iqr // 2
+        pos += median_interval
+        if lo > starts[-1]:
+            break
+        mask = np.ma.masked_outside(starts.to_numpy(), lo, hi).mask
+        if not isinstance(mask, bool):
+            masks.append(mask)
+
+    # Apply a mask of acceptable locations to input
+    mask = reduce(np.logical_and, masks)
+    valid_starts = starts[~mask]
+    feetdict["start"] = valid_starts
+    return feetdict
+
+
+feetfiltfuncs = {
+    "shortcycles": shortcycles,
+    "extrafeet": extrafeet,
+}
+
+
+def filter_feet(curve, filtname, paramgetter):
+    samplerate = curve.samplerate
+    feetdict = copy(curve.feetitem.indices)
     filt = FeetFilters[filtname]
     parameters = map(paramgetter, filt.parameters)
-
-    if filt.name == 'shortcycles':
-        if len(stops) < 1:
-            # No stop information
-            raise ValueError('No stop feet')
-        (minDuration,) = parameters
-        minCycleLength = minDuration * 1e9  # Transform ms to ns
-        cycleDurations = (stop - start for start, stop in zip(starts, stops))
-        boolidx = [d >= minCycleLength for d in cycleDurations]
-        starts, stops, boolidx = truncatevecs([starts, stops, boolidx])
-        newstarts = starts[boolidx]
-        newstops = stops[boolidx]
-    else:
-        errmsg = f'Unknown filter: {filtname}'
-        raise ValueError(errmsg)
-    return (newstarts, newstops)
+    return feetfiltfuncs[filt.name](feetdict, samplerate, parameters)
```

### Comparing `graphysio-2022.9.13/graphysio/algorithms/waveform.py` & `graphysio-2024.5.7/graphysio/algorithms/waveform.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def performWindowing(sumcoef=4, quantcoef=3):
         # Find pulse rising edge
         winsum = int(samplerate / sumcoef)
         winquant = int(samplerate * quantcoef)
         sndderivsq = sndderiv**2
         integral = sndderivsq.rolling(window=winsum, center=True).sum()
         thres = integral.rolling(window=winquant).quantile(0.7)
-        thres = thres.fillna(method='backfill')
+        thres = thres.fillna(method="backfill")
         risings = (integral > thres).astype(int)
         risingvar = risings.diff()
         (risingStarts,) = (risingvar > 0).to_numpy().nonzero()
         (risingStops,) = (risingvar < 0).to_numpy().nonzero()
         return (risingStarts, risingStops)
 
     found = False
@@ -68,29 +68,29 @@
     cycleStarts = series.iloc[idxstarts]
     cycleStops = series.iloc[idxstops]
 
     # Handle the case where we start within a cycle
     try:
         cycleStops = cycleStops[cycleStops.index > cycleStarts.index[0]]
     except IndexError as e:
-        raise TypeError('No cycle detected') from e
+        raise TypeError("No cycle detected") from e
 
     return (cycleStarts.index, cycleStops.index)
 
 
 def findPressureCycles(curve):
     series = curve.series
 
     cycles = []
     starts, durations = curve.getCycleIndices()
     for start, duration in zip(starts, durations):
         stop = start + duration
         diastop = start - duration
-        dia = findPOI(series, [start, diastop], 'min', windowsize=0.05, forcesign=False)
-        sbp = findPOI(series, [start, stop], 'max', windowsize=0.05)
+        dia = findPOI(series, [start, diastop], "min", windowsize=0.05, forcesign=False)
+        sbp = findPOI(series, [start, stop], "max", windowsize=0.05)
         cycle = (dia, sbp)
         cycles.append(cycle)
     return [pd.Index(idx, dtype=np.int64) for idx in zip(*cycles)]
 
 
 def findPressureFull(curve):
     dia, sbp = findPressureCycles(curve)
@@ -100,19 +100,19 @@
     return [dia, sbp, dic]
 
 
 # Utility function for point placing
 
 
 def isbetter(new, ref, kind, forcesign):
-    if kind == 'max':
+    if kind == "max":
         condition = new > ref
         if forcesign:
             condition = condition or (new < 0)
-    elif kind == 'min':
+    elif kind == "min":
         condition = new < ref
         if forcesign:
             condition = condition or (new > 0)
     else:
         raise ValueError(kind)
     return condition
 
@@ -140,20 +140,20 @@
         window = soi.loc[start:stop]
         if len(window) < 1:
             return
         yield window.index.values
 
 
 def findPOI(soi, interval, kind, windowsize, forcesign=True):
-    if kind not in ['min', 'max']:
+    if kind not in ["min", "max"]:
         raise ValueError(kind)
-    argkind = 'idx' + kind
+    argkind = "idx" + kind
 
     goodwindow = []
-    previous = -np.inf if kind == 'max' else np.inf
+    previous = -np.inf if kind == "max" else np.inf
     for window in genWindows(soi, interval, windowsize):
         zoi = soi.loc[window]
         new = getattr(zoi, kind)()
         if isbetter(new, previous, kind, forcesign):
             goodwindow = window
         else:
             break
@@ -164,24 +164,24 @@
     except ValueError:
         # No POI found
         retidx = None
     return retidx
 
 
 def findPOIGreedy(soi, start, kind):
-    if kind not in ['min', 'max']:
+    if kind not in ["min", "max"]:
         raise ValueError(kind)
-    loc = soi.index.get_loc(start, method='nearest')
+    loc = soi.index.get_loc(start, method="nearest")
     # Find direction
     try:
         finddir = soi.iloc[[loc - 1, loc, loc + 1]]
     except IndexError:
         # We're at the edge of the curve
         return start
-    npminmax = np.argmin if kind == 'min' else np.argmax
+    npminmax = np.argmin if kind == "min" else np.argmax
     direction = npminmax(finddir.values) - 1
     if direction == 0:
         # We're already at the local minimum
         return start
     curloc = loc
     while True:
         nextloc = curloc + direction
```

### Comparing `graphysio-2022.9.13/graphysio/dialogs.py` & `graphysio-2024.5.7/graphysio/dialogs.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,24 +29,26 @@
         self.choices = {}
 
         plotframe = self.parent().tabWidget.currentWidget()
         if plotframe is None:
             return
 
         for n, curvename in enumerate(plotframe.curves.keys()):
-            combo = QtGui.QComboBox()
+            combo = QtWidgets.QComboBox()
             combo.addItems([ft.value for ft in CycleId])
-            curveitem = QtGui.QTableWidgetItem(curvename)
+            curveitem = QtWidgets.QTableWidgetItem(curvename)
 
             self.table.insertRow(n)
             self.table.setItem(n, 0, curveitem)
             self.table.setCellWidget(n, 1, combo)
             self.choices[curvename] = combo
 
-        self.table.horizontalHeader().setResizeMode(QtGui.QHeaderView.ResizeToContents)
+        self.table.horizontalHeader().setSectionResizeMode(
+            QtWidgets.QHeaderView.ResizeToContents
+        )
 
     def accept(self):
         result = {curve: combo.currentText() for (curve, combo) in self.choices.items()}
         self.dlgdata.emit(result)
         super().accept()
 
 
@@ -65,36 +67,38 @@
         plotframe = self.parent().tabWidget.currentWidget()
         if not plotframe:
             return
 
         def fillTable(items, itemtype, filters):
             rowoffset = self.table.rowCount()
             for n, itemname in enumerate(items):
-                combo = QtGui.QComboBox()
+                combo = QtWidgets.QComboBox()
 
-                combo.addItems(['None'])
+                combo.addItems(["None"])
                 filternames = list(filters.keys())
                 combo.addItems(filternames)
 
-                curveitem = QtGui.QTableWidgetItem(itemname)
+                curveitem = QtWidgets.QTableWidgetItem(itemname)
 
                 idx = rowoffset + n
                 self.table.insertRow(idx)
                 self.table.setItem(idx, 0, curveitem)
                 self.table.setCellWidget(idx, 1, combo)
                 self.choices[itemname] = (combo, itemtype)
 
         curves = list(plotframe.curves.keys())
         if filterfeet:
             self.chkNewcurve.hide()
-            fillTable(curves, 'curve', filters.FeetFilters)
+            fillTable(curves, "curve", filters.FeetFilters)
         else:
-            fillTable(curves, 'curve', filters.Filters)
+            fillTable(curves, "curve", filters.Filters)
 
-        self.table.horizontalHeader().setResizeMode(QtGui.QHeaderView.ResizeToContents)
+        self.table.horizontalHeader().setSectionResizeMode(
+            QtWidgets.QHeaderView.ResizeToContents
+        )
 
     def accept(self):
         curvefilters = {}
         for itemname, value in self.choices.items():
             combo, itemtype = value
             curvefilters[itemname] = combo.currentText()
         createnew = self.chkNewcurve.checkState() > QtCore.Qt.Unchecked
@@ -143,22 +147,22 @@
         self.txtPatient.setText(patient)
 
         self.btnOk.clicked.connect(self.accept)
         self.btnCancel.clicked.connect(self.reject)
         self.btnBrowse.clicked.connect(self.selectFile)
 
     def selectFile(self):
-        filepath = QtGui.QFileDialog.getSaveFileName(
+        filepath = QtWidgets.QFileDialog.getSaveFileName(
             caption="Export to",
             filter="CSV files (*.csv *.dat)",
-            options=QtGui.QFileDialog.DontConfirmOverwrite,
+            options=QtWidgets.QFileDialog.DontConfirmOverwrite,
             directory=self.dircache,
         )
         # PyQt5 API change
-        if type(filepath) is not str:
+        if not isinstance(filepath, str):
             filepath = filepath[0]
 
         if filepath:
             self.txtFile.setText(filepath)
             self.dircache = os.path.dirname(filepath)
 
     def accept(self):
@@ -209,26 +213,26 @@
             self.curveproperties[curve] = resultdict
 
         dlg = DlgCurveProperties(curve)
         dlg.dlgdata.connect(cb)
         dlg.exec_()
 
     def addCurve(self, name, checked):
-        item = QtGui.QListWidgetItem()
+        item = QtWidgets.QListWidgetItem()
         item.setText(name)
         item.setFlags(item.flags() | QtCore.Qt.ItemIsUserCheckable)
         if checked:
             item.setCheckState(QtCore.Qt.Checked)
         else:
             item.setCheckState(QtCore.Qt.Unchecked)
         self.lstCurves.addItem(item)
 
     def accept(self):
-        items = self.lstCurves.findItems('', QtCore.Qt.MatchContains)
-        ischecked = lambda item: item.checkState() != QtCore.Qt.Unchecked
+        items = self.lstCurves.findItems("", QtCore.Qt.MatchContains)
+        ischecked = lambda item: item.checkState() != QtCore.Qt.Unchecked  # noqa: E731
         checked = list(filter(ischecked, items))
         visible = {self.curvehash[item.text()] for item in checked}
         result = (visible, self.curveproperties)
         self.dlgdata.emit(result)
         super().accept()
 
 
@@ -241,20 +245,20 @@
 
         self.curve = curve
 
         self.okButton.clicked.connect(self.ok)
         self.cancelButton.clicked.connect(self.reject)
         self.btnColor.clicked.connect(self.chooseColor)
 
-        connect = curve.opts['connect']
-        symbol = curve.opts['symbol']
+        connect = curve.opts["connect"]
+        symbol = curve.opts["symbol"]
         if symbol is None:
-            symbol = 'None'
+            symbol = "None"
 
-        pen = curve.opts['pen']
+        pen = curve.opts["pen"]
         if isinstance(pen, QtGui.QPen):
             color = pen.color()
             width = pen.width()
         else:
             color = pen
             width = 1
         self.color = color
@@ -265,55 +269,55 @@
         idx = self.cmbSymbol.findText(symbol, QtCore.Qt.MatchFixedString)
         self.cmbSymbol.setCurrentIndex(idx)
 
         self.cmbSymbol.setEditText(symbol)
         self.grpName.setTitle(curve.name())
         self.txtName.setText(curve.name())
         self.spnWidth.setValue(width)
-        self.btnColor.setStyleSheet(f'background-color: {color.name()}')
+        self.btnColor.setStyleSheet(f"background-color: {color.name()}")
         self.lblSamplerate.setText(str(curve.samplerate))
 
     def ok(self):
         symbol = self.cmbSymbol.currentText().lower()
-        symbol = None if symbol == 'none' else symbol
+        symbol = None if symbol == "none" else symbol
 
         connect = str(self.cmbConnect.currentText().lower())
-        connect = [0] if connect == 'none' else connect
+        connect = [0] if connect == "none" else connect
 
         result = {
-            'name': self.txtName.text(),
-            'connect': connect,
-            'symbol': symbol,
-            'width': self.spnWidth.value(),
-            'color': self.color,
+            "name": self.txtName.text(),
+            "connect": connect,
+            "symbol": symbol,
+            "width": self.spnWidth.value(),
+            "color": self.color,
         }
         self.dlgdata.emit(result)
         self.accept()
 
     def chooseColor(self):
-        color = QtGui.QColorDialog.getColor()
+        color = QtWidgets.QColorDialog.getColor()
         if not color.isValid():
             return
         self.color = color
-        self.btnColor.setStyleSheet(f'background-color: {color.name()}')
+        self.btnColor.setStyleSheet(f"background-color: {color.name()}")
 
 
 class DlgSetDateTime(ui.Ui_SetDateTime, QtWidgets.QDialog):
     def __init__(self, parent=None, prevdatetime=None):
         super().__init__(parent=parent)
         self.setupUi(self)
 
         self.dlgdata = None
         self.btnOk.clicked.connect(self.ok)
         self.btnCancel.clicked.connect(self.reject)
 
         if prevdatetime is None:
             datetime = QtCore.QDateTime.currentDateTime()
         else:
-            datetime = QtCore.QDateTime.fromMSecsSinceEpoch(prevdatetime / 1e6)
+            datetime = QtCore.QDateTime.fromMSecsSinceEpoch(int(prevdatetime / 1e6))
         curdate = datetime.date()
         curtime = datetime.time()
         self.widgetCalendar.setSelectedDate(curdate)
         self.edDate.setDate(curdate)
         self.edTime.setTime(curtime)
 
     def ok(self):
@@ -333,21 +337,21 @@
         if curvecorr is None:
             curvecorr = {}
         self.setupUi(curvecorr)
 
     def setupUi(self, curvecorr):
         vstack = QtWidgets.QVBoxLayout(self)
 
-        self.lbl = QtWidgets.QLabel('Enter formula for new curve:')
+        self.lbl = QtWidgets.QLabel("Enter formula for new curve:")
         vstack.addWidget(self.lbl)
 
-        self.formula = QtWidgets.QLineEdit('a**2 + log(2*b)')
+        self.formula = QtWidgets.QLineEdit("a**2 + log(2*b)")
         vstack.addWidget(self.formula)
 
-        curveslbl = '\n'.join([f'{x}: {y}' for x, y in curvecorr.items()])
+        curveslbl = "\n".join([f"{x}: {y}" for x, y in curvecorr.items()])
         self.curveletters = QtWidgets.QLabel(curveslbl)
         vstack.addWidget(self.curveletters)
 
         self.buttonbox = QtWidgets.QDialogButtonBox(
             QtWidgets.QDialogButtonBox.Ok | QtWidgets.QDialogButtonBox.Cancel
         )
         vstack.addWidget(self.buttonbox)
@@ -362,15 +366,15 @@
         self.dlgdata.emit(result)
         super().accept()
 
 
 class DlgListChoice(QtWidgets.QDialog):
     dlgdata = QtCore.pyqtSignal(object)
 
-    def __init__(self, items, title='', message='', parent=None):
+    def __init__(self, items, title="", message="", parent=None):
         super().__init__(parent=parent)
         form = QtWidgets.QFormLayout(self)
         form.addRow(QtWidgets.QLabel(message))
         self.listView = QtWidgets.QListView(self)
         form.addRow(self.listView)
         model = QtGui.QStandardItemModel(self.listView)
         self.setWindowTitle(title)
@@ -403,74 +407,80 @@
 
     def accept(self):
         result = self.itemsSelected()
         self.dlgdata.emit(result)
         super().accept()
 
 
-def askUserValue(param):
-    if param.request == 'time':
-        value, isok = QtGui.QInputDialog.getText(None, 'Enter time', param.description)
+def askUserValue(param):  # noqa: C901
+    if param.request == "time":
+        value, isok = QtWidgets.QInputDialog.getText(
+            None, "Enter time", param.description
+        )
         try:
             value = ureg.Quantity(value)
             if value.dimensionless:
                 # Default to second if no unit is specified
-                value = ureg.Quantity(value.magnitude, 's')
+                value = ureg.Quantity(value.magnitude, "s")
             value = value.to_base_units().magnitude
         except (DimensionalityError, UndefinedUnitError, ValueError):
             return None
     elif param.request is str:
-        value, isok = QtGui.QInputDialog.getText(None, 'Enter value', param.description)
+        value, isok = QtWidgets.QInputDialog.getText(
+            None, "Enter value", param.description
+        )
     elif param.request is int:
-        value, isok = QtGui.QInputDialog.getInt(None, 'Enter value', param.description)
+        value, isok = QtWidgets.QInputDialog.getInt(
+            None, "Enter value", param.description
+        )
     elif param.request is float:
-        value, isok = QtGui.QInputDialog.getDouble(
-            None, 'Enter value', param.description, decimals=3
+        value, isok = QtWidgets.QInputDialog.getDouble(
+            None, "Enter value", param.description, decimals=3
         )
     elif param.request is bool:
-        request = ['Yes', 'No']
-        tmpvalue, isok = QtGui.QInputDialog.getItem(
-            None, 'Enter value', param.description, request, editable=False
+        request = ["Yes", "No"]
+        tmpvalue, isok = QtWidgets.QInputDialog.getItem(
+            None, "Enter value", param.description, request, editable=False
         )
-        value = tmpvalue == 'Yes'
+        value = tmpvalue == "Yes"
     elif param.request is datetime:
         dlg = DlgSetDateTime()
         isok = dlg.exec_()
         value = dlg.dlgdata
-    elif type(param.request) is list:
-        value, isok = QtGui.QInputDialog.getItem(
+    elif isinstance(param.request, list):
+        value, isok = QtWidgets.QInputDialog.getItem(
             None,
-            'Choose value',
+            "Choose value",
             param.description,
             param.request,
             editable=False,
         )
     else:
         raise TypeError("Unknown request type")
 
     if isok:
         return value
     else:
         return None
 
 
-def userConfirm(question: str, title: str = '') -> bool:
+def userConfirm(question: str, title: str = "") -> bool:
     if not title:
         title = question
-    reply = QtGui.QMessageBox.question(
-        None, title, question, QtGui.QMessageBox.Yes, QtGui.QMessageBox.No
+    reply = QtWidgets.QMessageBox.question(
+        None, title, question, QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No
     )
-    return reply == QtGui.QMessageBox.Yes
+    return reply == QtWidgets.QMessageBox.Yes
 
 
 def askFilePath(
     func,
     caption: str,
-    filename: str = '',
-    folder: str = '',
+    filename: str = "",
+    folder: str = "",
     filter: str = "CSV files (*.csv *.dat)",
 ) -> Optional[pathlib.Path]:
     default = pathlib.Path(folder) if folder else pathlib.Path.home()
     if filename:
         default = pathlib.Path(default, filename)
 
     fileinfo = func(caption=caption, filter=filter, directory=str(default))
@@ -480,22 +490,22 @@
         return (None, None)
     filepath = sanitize_filepath(filepath)
     filepath = pathlib.Path(filepath).resolve()
     ext = filepath.suffix[1:]
     return (filepath, ext)
 
 
-askOpenFilePath = partial(askFilePath, QtGui.QFileDialog.getOpenFileName)
-askSaveFilePath = partial(askFilePath, QtGui.QFileDialog.getSaveFileName)
+askOpenFilePath = partial(askFilePath, QtWidgets.QFileDialog.getOpenFileName)
+askSaveFilePath = partial(askFilePath, QtWidgets.QFileDialog.getSaveFileName)
 
 
-def askDirPath(caption: str, folder: str = '') -> Optional[pathlib.Path]:
+def askDirPath(caption: str, folder: str = "") -> Optional[pathlib.Path]:
     if not folder:
         folder = str(pathlib.Path.home())
 
-    outdirtmp = QtGui.QFileDialog.getExistingDirectory(
-        caption=caption, directory=folder
+    outdirtmp = QtWidgets.QFileDialog.getExistingDirectory(
+        caption=caption, directory=str(folder)
     )
     if not outdirtmp:
         # Cancel pressed
         return None
     return pathlib.Path(outdirtmp).resolve()
```

### Comparing `graphysio-2022.9.13/graphysio/legend.py` & `graphysio-2024.5.7/graphysio/legend.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,11 +8,11 @@
     def paint(self, p, *args):
         p.setPen(pg.mkPen(0, 0, 0, 255))
         p.setBrush(pg.mkBrush(255, 255, 255, 255))
         p.drawRect(self.boundingRect())
 
     def addItem(self, item, name):
         # Fix the line width bigger
-        pen = pg.mkPen(item.opts['pen'])
+        pen = pg.mkPen(item.opts["pen"])
         pen.setWidth(2)
         newitem = pg.PlotDataItem(pen=pen)
         super().addItem(newitem, name)
```

### Comparing `graphysio-2022.9.13/graphysio/mainui.py` & `graphysio-2024.5.7/graphysio/mainui.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 import itertools
 import os
 import sys
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 from queue import Empty, Queue
+from typing import Optional
 
 from pyqtgraph import QtCore, QtWidgets
 
 from graphysio import dialogs, readdata, ui, utils
 from graphysio.plotwidgets import TimeAxisItem, TSWidget
 
 
 class MainUi(ui.Ui_MainWindow, QtWidgets.QMainWindow):
     setcoords = QtCore.pyqtSignal(float, float)
 
     def __init__(self, parent=None):
         super().__init__(parent=parent)
         self.setupUi(self)
-        self.dircache = os.path.expanduser('~')
+        self.dircache = os.path.expanduser("~")
 
         self.dataq = Queue()
         self.executor = ThreadPoolExecutor()
         self.datahandler = self.createNewPlotWithData
 
         self.tabWidget.tabCloseRequested.connect(self.closeTab)
         self.tabWidget.currentChanged.connect(self.tabChanged)
 
         getCLIShell = partial(utils.getshell, ui=self)
 
         launchNewPlot = partial(self.launchOpenFile, self.createNewPlotWithData)
         launchAppendPlot = partial(self.launchOpenFile, self.appendToPlotWithData)
-        self.menuFile.addAction('New Plot', launchNewPlot)
-        self.menuFile.addAction('Append to Plot', launchAppendPlot)
+        self.menuFile.addAction("New Plot", launchNewPlot)
+        self.menuFile.addAction("Append to Plot", launchAppendPlot)
 
         self.menuFile.addSeparator()
-        self.menuFile.addAction('&Load plugin', self.errguard(utils.loadmodule))
-        self.menuFile.addAction('Get CLI shell', self.errguard(getCLIShell))
+        self.menuFile.addAction("&Load plugin", self.errguard(utils.loadmodule))
+        self.menuFile.addAction("Get CLI shell", self.errguard(getCLIShell))
         self.menuFile.addSeparator()
-        self.menuFile.addAction('&Quit', self.close, QtCore.Qt.CTRL + QtCore.Qt.Key_Q)
+        self.menuFile.addAction("&Quit", self.close, QtCore.Qt.CTRL + QtCore.Qt.Key_Q)
 
         self.setcoords.connect(self.setCoords)
 
         # Launch timer to handle new plot data
         self.data_timer = QtCore.QTimer()
         self.data_timer.timeout.connect(self.read_plot_data)
         self.data_timer.setInterval(1000)  # Milliseconds
         self.data_timer.start()
 
     def setCoords(self, x, y):
         if TimeAxisItem.is_relative_time(x):
             timestr = TimeAxisItem.conv_relative(x)
         else:
             timestr = TimeAxisItem.conv_absolute(x, mainwindow=True)
-        self.lblCoords.setText(f'Time: {timestr}, Value: {y}')
+        self.lblCoords.setText(f"Time: {timestr}, Value: {y}")
 
     def read_plot_data(self):
         try:
             data = self.dataq.get(block=False)
         except Empty:
             return
         # Plotdata can be an object or a list of objects
@@ -86,15 +87,15 @@
         tabnames = []
         for i in range(self.tabWidget.count()):
             tabnames.append(self.tabWidget.tabText(i))
         if tabname in tabnames:
             tmptabname = tabname
             # Duplicate tab name. Add a number to the end
             for i in itertools.count():
-                tmptabname = f'{tabname}{i+1}'
+                tmptabname = f"{tabname}{i+1}"
                 if tmptabname not in tabnames:
                     break
             tabname = tmptabname
         tabindex = self.tabWidget.addTab(widget, tabname)
         self.tabWidget.setCurrentIndex(tabindex)
 
     def closeTab(self, i) -> None:
@@ -125,35 +126,38 @@
             if plotdata:
                 self.dataq.put(plotdata)
 
         self.datahandler = datahandler
         future.add_done_callback(cb)
 
     def createNewPlotWithData(self, plotdata):
-        properties = {'dircache': self.dircache}
+        properties = {"dircache": self.dircache}
         plotwidget = TSWidget(plotdata, parent=self, properties=properties)
         self.addTab(plotwidget, plotdata.name)
         self.lblStatus.setText("Loading... done")
 
-    def appendToPlotWithData(self, plotdata, destidx=None):
+    def appendToPlotWithData(
+        self, plotdata, destidx=None, do_timeshift: Optional[bool] = None
+    ):
         if destidx is None:
             plotwidget = self.tabWidget.currentWidget()
         else:
             plotwidget = self.tabWidget.widget(destidx)
         if plotwidget is None:
-            utils.displayError('No plot selected.')
+            utils.displayError("No plot selected.")
             return
-        dorealign = dialogs.userConfirm(
-            'Timeshift new curves to make the beginnings coincide?',
-            title='Append to plot',
-        )
+        if do_timeshift is None:
+            do_timeshift = dialogs.userConfirm(
+                "Timeshift new curves to make the beginnings coincide?",
+                title="Append to plot",
+            )
 
         for fieldname in plotdata.data:
             newname = plotwidget.validateNewCurveName(fieldname)
             if newname is None:
                 continue
             if newname != fieldname:
                 plotdata.data.rename(columns={fieldname: newname}, inplace=True)
 
-        plotwidget.appendData(plotdata, dorealign)
-        plotwidget.properties['dircache'] = self.dircache
+        plotwidget.appendData(plotdata, do_timeshift)
+        plotwidget.properties["dircache"] = self.dircache
         self.lblStatus.setText("Loading... done")
```

### Comparing `graphysio-2022.9.13/graphysio/plotwidgets/curves.py` & `graphysio-2024.5.7/graphysio/plotwidgets/curves.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 from functools import partial
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 import pyqtgraph as pg
+from physiocurve.pandas import ECG, Pressure
+from pyqtgraph.Qt import QtCore, QtGui
+
 from graphysio import utils
 from graphysio.algorithms import waveform
 from graphysio.structures import CycleId
 from graphysio.utils import estimateSampleRate
-from physiocurve.pandas import ECG, Pressure
-from pyqtgraph.Qt import QtCore, QtGui
 
 
 class CurveItem(pg.PlotDataItem):
     visible = QtCore.pyqtSignal()
     invisible = QtCore.pyqtSignal()
 
     def __init__(self, series, parent, pen=None):
         self.parent = parent
         self.series = self.sanitize_data(series)
         if self.series is None:
-            raise ValueError('Not enough data')
+            raise ValueError("Not enough data")
         self.samplerate = estimateSampleRate(self.series)
         if pen is None:
             pen = QtGui.QColor(QtCore.Qt.black)
         super().__init__(name=series.name, pen=pen, antialias=True)
         self.render()
 
     def replace_data(self, newdata):
         newdata = self.sanitize_data(newdata)
         if newdata is None:
             # XXX report error
             return
         self.clear()
-        self.series = newdata.rename(self.opts['name'])
+        self.series = newdata.rename(self.opts["name"])
         self.samplerate = estimateSampleRate(self.series)
         self.render()
 
     def extend(self, newseries):
         merged = self.series.append(newseries)
         newdata = self.sanitize_data(merged)
         if newdata is None:
@@ -49,15 +50,15 @@
     def render(self):
         self.setData(x=self.series.index.to_numpy(), y=self.series.to_numpy())
 
     def set_samplerate(self, newsamplerate):
         self.samplerate = newsamplerate
 
     def rename(self, newname: str):
-        self.opts['name'] = newname
+        self.opts["name"] = newname
         self.series = self.series.rename(newname)
 
     def sanitize_data(self, series: pd.Series) -> Optional[pd.Series]:
         series = series.dropna()
         series = series.sort_index()
         # Less than 2 points are not visible
         if len(series) < 2:
@@ -65,21 +66,23 @@
         # Make timestamp unique and use mean of values on duplicates
         series = series.groupby(level=0).mean()
         return series
 
 
 class POIItem(pg.ScatterPlotItem):
     sym = {
-        'start': 'star',
-        'stop': 's',
-        'diastole': 't1',
-        'systole': 't',
-        'dicrotic': 'd',
-        'rwave': 'x',
-        'twave': 'o',
+        "start": "star",
+        "stop": "s",
+        "diastole": "t1",
+        "systole": "t",
+        "dicrotic": "d",
+        "qwave": "t1",
+        "rwave": "x",
+        "swave": "t",
+        "twave": "o",
     }
     # Symbols = OrderedDict([(name, QtGui.QPainterPath()) for name in
     # ['o', 's', 't', 't1', 't2', 't3','d', '+', 'x', 'p', 'h', 'star']])
 
     def __init__(self, parent, name, pen=None):
         super().__init__(pen=pen, name=name)
         self.parent = parent
@@ -96,68 +99,68 @@
         self.indices[key] = newidx.unique().sort_values()
         self.render()
 
     def removePointsByLocation(self, key, locations):
         if key not in self.indices:
             return
         oldidx = self.indices[key]
-        dellocs = oldidx.get_indexer(locations, method='nearest')
+        dellocs = oldidx.get_indexer(locations, method="nearest")
         newidx = oldidx.delete(dellocs)
         self.indices[key] = newidx
         self.render()
 
     def removePoints(self, points):
         for point in points:
             try:
                 sym = self.resym[point.symbol()]
                 idx = self.indices[sym]
             except KeyError as e:
-                raise KeyError('Point not found') from e
-            nidx = idx.get_indexer([point.pos().x()], method='nearest')
+                raise KeyError("Point not found") from e
+            nidx = idx.get_indexer([point.pos().x()], method="nearest")
             self.indices[sym] = idx.delete(nidx)
         self.render()
 
     def render(self):
         data = []
         for key, idx in self.indices.items():
             if len(idx) < 1:
                 continue
             idxnona = idx.dropna()
             points = self.parent.series.loc[idxnona]
-            tmp = pd.DataFrame({'points': points, 'sym': self.sym[key]}, index=idxnona)
+            tmp = pd.DataFrame({"points": points, "sym": self.sym[key]}, index=idxnona)
             data.append(tmp)
         if len(data) < 1:
             self.clear()
             return
         feet = pd.concat(data)
         self.setData(
-            x=feet.index.values, y=feet['points'].values, symbol=feet['sym'].values
+            x=feet.index.values, y=feet["points"].values, symbol=feet["sym"].values
         )
 
     def isPointSelected(self, point):
         return point in self.selected
 
     def selectPoint(self, point):
         if not self.isPointSelected(point):
             self.selected.append(point)
-        point.setPen('r')
-        point.setBrush('r')
+        point.setPen("r")
+        point.setBrush("r")
 
     def unselectPoint(self, point):
         if self.isPointSelected(point):
             self.selected.remove(point)
         point.resetPen()
         point.resetBrush()
 
     def removeSelection(self):
         self.removePoints(self.selected)
         self.selected = []
 
     def rename(self, newname: str):
-        self.opts['name'] = newname
+        self.opts["name"] = newname
 
 
 class CurveItemWithPOI(CurveItem):
     visible = QtCore.pyqtSignal()
     invisible = QtCore.pyqtSignal()
 
     @staticmethod
@@ -166,15 +169,15 @@
         if not feetitem.isPointSelected(point):
             feetitem.selectPoint(point)
         else:
             feetitem.unselectPoint(point)
 
     def __init__(self, series, parent, pen=None):
         super().__init__(series, parent, pen)
-        feetname = f'{series.name}-feet'
+        feetname = f"{series.name}-feet"
         self.feetitem = POIItem(self, name=feetname, pen=pen)
         parent.addItem(self.feetitem)
         self.feetitem.sigClicked.connect(self.sigPointClicked)
         self.visible.connect(self.__becameVisible)
         self.invisible.connect(self.__becameInvisible)
 
     def __becameVisible(self):
@@ -187,76 +190,78 @@
         self.parent.removeItem(self.feetitem)
 
     def addFeet(self, cycleid):
         if cycleid is CycleId.none:
             return
         elif cycleid is CycleId.velocity:
             starts, stops = waveform.findFlowCycles(self)
-            self.feetitem.indices['start'] = starts
-            self.feetitem.indices['stop'] = stops
+            self.feetitem.indices["start"] = starts
+            self.feetitem.indices["stop"] = stops
         elif cycleid is CycleId.foot:
             foot = waveform.findPressureFeet(self)
-            self.feetitem.indices['start'] = foot
+            self.feetitem.indices["start"] = foot
         elif cycleid is CycleId.pressure:
-            if 'start' not in self.feetitem.indices:
+            if "start" not in self.feetitem.indices:
                 self.addFeet(CycleId.foot)
             dia, sbp, dic = waveform.findPressureFull(self)
-            self.feetitem.indices['diastole'] = dia
-            self.feetitem.indices['systole'] = sbp
-            self.feetitem.indices['dicrotic'] = dic
+            self.feetitem.indices["diastole"] = dia
+            self.feetitem.indices["systole"] = sbp
+            self.feetitem.indices["dicrotic"] = dic
         elif cycleid is CycleId.rwave:
             ecg = ECG(self.series)
-            self.feetitem.indices['rwave'] = ecg.idxrwave
+            self.feetitem.indices["rwave"] = ecg.idxrwave
         elif cycleid is CycleId.ecg:
             ecg = ECG(self.series)
-            self.feetitem.indices['start'] = ecg.idxpwave
-            self.feetitem.indices['rwave'] = ecg.idxrwave
-            self.feetitem.indices['twave'] = ecg.idxtwave
+            self.feetitem.indices["start"] = ecg.idxpwave
+            self.feetitem.indices["qwave"] = ecg.idxqwave
+            self.feetitem.indices["rwave"] = ecg.idxrwave
+            self.feetitem.indices["swave"] = ecg.idxswave
+            self.feetitem.indices["twave"] = ecg.idxtwave
         elif cycleid is CycleId.foottan:
             p = Pressure(self.series)
-            self.feetitem.indices['start'] = p.idxtanfeet
+            self.feetitem.indices["start"] = p.idxtanfeet
         elif cycleid is CycleId.pressurebis:
             p = Pressure(self.series)
-            self.feetitem.indices['start'] = p.idxfeet
-            self.feetitem.indices['diastole'] = p.idxdia
-            self.feetitem.indices['systole'] = p.idxsys
-            self.feetitem.indices['dicrotic'] = p.idxdic
+            self.feetitem.indices["start"] = p.idxfeet
+            self.feetitem.indices["diastole"] = p.idxdia
+            self.feetitem.indices["systole"] = p.idxsys
+            self.feetitem.indices["dicrotic"] = p.idxdic
         else:
             raise ValueError(cycleid)
         self.feetitem.render()
 
     def getCycleIndices(self, vrange=None):
         s = self.series
         clip = partial(utils.clip, vrange=vrange)
-        hasstarts = ('start' in self.feetitem.indices) and self.feetitem.indices[
-            'start'
+        hasstarts = ("start" in self.feetitem.indices) and self.feetitem.indices[
+            "start"
         ].size > 0
-        hasstops = ('stop' in self.feetitem.indices) and self.feetitem.indices[
-            'stop'
+        hasstops = ("stop" in self.feetitem.indices) and self.feetitem.indices[
+            "stop"
         ].size > 0
         if vrange:
             xmin, xmax = vrange
         else:
             xmin = s.index[0]
             xmax = s.index[-1]
         if not hasstarts:
             # We have no feet, treat the whole signal as one cycle
-            locs = s.index.get_indexer([xmin, xmax], method='nearest')
+            locs = s.index.get_indexer([xmin, xmax], method="nearest")
             indices = s.index[locs]
             begins, ends = [np.array([i]) for i in indices]
         elif not hasstops:
             # We have no stops, starts serve as stops for previous cycle
-            begins = clip(self.feetitem.indices['start'].values)
-            endloc = s.index.get_indexer([xmax], method='nearest')
+            begins = clip(self.feetitem.indices["start"].values)
+            endloc = s.index.get_indexer([xmax], method="nearest")
             end = s.index[endloc]
             ends = np.append(begins[1:], end)
         else:
             # We have starts and stops, use them
-            begins = self.feetitem.indices['start'].values
-            ends = self.feetitem.indices['stop'].values
+            begins = self.feetitem.indices["start"].values
+            ends = self.feetitem.indices["stop"].values
             begins, ends = map(clip, [begins, ends])
 
         # Handle the case where we start in the middle of a cycle
         while ends[0] <= begins[0]:
             ends = ends[1:]
 
         begins, ends = utils.truncatevecs([begins, ends])
```

### Comparing `graphysio-2022.9.13/graphysio/plotwidgets/plotwidget.py` & `graphysio-2024.5.7/graphysio/plotwidgets/plotwidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from datetime import timedelta
 from functools import partial
 from typing import Optional
 
 import pyqtgraph as pg
+from pyqtgraph.Qt import QtCore, QtWidgets
+
 from graphysio.legend import LegendItem
 from graphysio.plotwidgets.curves import CurveItem, CurveItemWithPOI
 from graphysio.utils import Colors
-from pyqtgraph.Qt import QtCore, QtGui
 
 
 class TimeAxisItem(pg.AxisItem):
     @staticmethod
     def conv_absolute(value, mainwindow=False):
         value = int(value * 1e-6)  # convert from ns to ms
         date = QtCore.QDateTime.fromMSecsSinceEpoch(value)
-        date = date.toTimeSpec(QtCore.Qt.UTC)
+        date = date.toLocalTime()
         if mainwindow:
             timestr = date.toString("dd/MM/yyyy hh:mm:ss.zzz")
         else:
             timestr = date.toString("dd/MM/yyyy\nhh:mm:ss.zzz")
         return timestr
 
     @staticmethod
@@ -52,16 +53,16 @@
     def __init__(self, name, parent=None, properties=None):
         self.parent = parent
         self.name = name
         self.colors = Colors()
         self.hiddencurves = set()
         self.properties = properties if properties is not None else {}
 
-        axisItems = {'bottom': TimeAxisItem(orientation='bottom')}
-        super().__init__(parent=parent, axisItems=axisItems, background='w')
+        axisItems = {"bottom": TimeAxisItem(orientation="bottom")}
+        super().__init__(parent=parent, axisItems=axisItems, background="w")
 
         self.legend = LegendItem()
         self.legend.setParentItem(self.getPlotItem())
 
         self.vb = self.getViewBox()
         self.vb.setMouseMode(self.vb.RectMode)
 
@@ -134,30 +135,30 @@
                 self.legend.addItem(curve, curve.name())
 
     def validateNewCurveName(
         self, proposedname: str, alwaysShow: bool = False
     ) -> Optional[str]:
         if proposedname not in self.curves and not alwaysShow:
             return proposedname
-        newname, okPressed = QtGui.QInputDialog.getText(
+        newname, okPressed = QtWidgets.QInputDialog.getText(
             self,
             "Series name",
             "Series with identical names will be merged.",
             text=proposedname,
         )
         if not okPressed:
             return None
         return newname
 
     def applyCurveProperties(self, curve, properties: dict) -> None:
         # Setting Symbol and Connect does not work. TODO dig into pyqtgraph
         # curve.setData(symbol=properties['symbol'])
         # curve.setData(connect=properties['connect'], symbol=properties['symbol'])
-        curve.setPen(properties['color'], width=properties['width'])
-        curve.rename(properties['name'])
+        curve.setPen(properties["color"], width=properties["width"])
+        curve.rename(properties["name"])
 
     @property
     def vbrange(self):
         vbrange = self.vb.viewRange()
         xmin, xmax = map(int, vbrange[0])
         return (xmin, xmax)
```

### Comparing `graphysio-2022.9.13/graphysio/plotwidgets/poiselector.py` & `graphysio-2024.5.7/graphysio/plotwidgets/poiselector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from enum import Enum
 from functools import partial
 
 import pandas as pd
 import pyqtgraph as pg
+from pyqtgraph import QtWidgets
+
 from graphysio import ui
 from graphysio.algorithms.filters import savgol
 from graphysio.algorithms.waveform import findPOIGreedy
 from graphysio.plotwidgets import PlotWidget
 from graphysio.structures import PlotData
 from graphysio.writedata import exporter
-from pyqtgraph import QtGui, QtWidgets
 
 
 class FixIndex(Enum):
-    disabled = 'Disabled'
-    minimum = 'Local Minimum'
-    maximum = 'Local Maximum'
-    sndderiv = '2nd derivative peak'
+    disabled = "Disabled"
+    minimum = "Local Minimum"
+    maximum = "Local Maximum"
+    sndderiv = "2nd derivative peak"
 
 
 class POISelectorWidget(ui.Ui_POISelectorWidget, QtWidgets.QWidget):
     @staticmethod
     def buttonClicked(self, qbutton):
         fixval = FixIndex(qbutton.text())
         self.poiselectorwidget.fixvalue = fixval
@@ -37,50 +38,50 @@
         )
         self.horizontalLayout.addWidget(self.poiselectorplot)
 
         buttonClicked = partial(self.buttonClicked, self)
         self.buttonGroup.buttonClicked.connect(buttonClicked)
 
     def loadPOI(self, plotdata):
-        columnname, ok = QtGui.QInputDialog.getItem(
-            self, 'Select POI series', 'Load POI', plotdata.data.columns, editable=False
+        columnname, ok = QtWidgets.QInputDialog.getItem(
+            self, "Select POI series", "Load POI", plotdata.data.columns, editable=False
         )
         if not ok:
             return
         poiseries = plotdata.data[columnname].dropna().index
         self.poiselectorplot.curve.feetitem.addPointsByLocation(
             self.poiselectorplot.pointkey, poiseries
         )
 
     def launchNewPlotFromPOIs(self):
         srcseries = self.poiselectorplot.curve.series
         poiidx = self.poiselectorplot.curve.feetitem.indices[
             self.poiselectorplot.pointkey
         ]
-        pois = srcseries[poiidx.dropna()].rename('poi')
-        sname = f'{srcseries.name}-poi'
+        pois = srcseries[poiidx.dropna()].rename("poi")
+        sname = f"{srcseries.name}-poi"
         df = pd.DataFrame({sname: pois})
         plotdata = PlotData(data=df, name=sname)
         self.parent.createNewPlotWithData(plotdata)
 
     @property
     def menu(self):
         return {
-            'Plot': {
-                'Import POIs': partial(
+            "Plot": {
+                "Import POIs": partial(
                     self.parent.launchOpenFile, datahandler=self.loadPOI
                 ),
-                'POIs to New Plot': self.launchNewPlotFromPOIs,
+                "POIs to New Plot": self.launchNewPlotFromPOIs,
             },
-            'Export': {'POI to CSV': self.poiselectorplot.exporter.poi},
+            "Export": {"POI to CSV": self.poiselectorplot.exporter.poi},
         }
 
 
 class POISelectorPlot(PlotWidget):
-    pointkey = 'point'
+    pointkey = "point"
 
     @staticmethod
     def mouseMoved(self, evt):
         pos = evt[0]  # using signal proxy turns original arguments into a tuple
         if self.sceneBoundingRect().contains(pos):
             mousePoint = self.getViewBox().mapSceneToView(pos)
             self.vLine.setPos(mousePoint.x())
@@ -102,43 +103,43 @@
         self.properties = properties if properties is not None else {}
 
         self.__sndderiv = None
         self.fixvalue = FixIndex.disabled
 
         self.curve = self.addSeriesAsCurve(series)
         if self.curve is None:
-            raise ValueError('Not enough data')
+            raise ValueError("Not enough data")
         self.exporter = exporter.POIExporter(self, self.name)
 
-        pen = pg.mkPen('k', width=2)
+        pen = pg.mkPen("k", width=2)
         self.vLine = pg.InfiniteLine(angle=90, movable=False, pen=pen)
         self.addItem(self.vLine, ignoreBounds=True)
 
         clicked = partial(self.clicked, self)
         self.scene().sigMouseClicked.connect(clicked)
 
     def fixpos(self, pos):
         # Need to go through get_loc, otherwise strange things happen
         correctedpos = pos
         xmin, xmax = self.vbrange
         if self.fixvalue is FixIndex.minimum:
             s = self.curve.series.loc[xmin:xmax]
-            posprop = findPOIGreedy(s, pos, 'min')
-            fixedposloc = s.index.get_loc(posprop, method='nearest')
+            posprop = findPOIGreedy(s, pos, "min")
+            fixedposloc = s.index.get_loc(posprop, method="nearest")
         elif self.fixvalue is FixIndex.maximum:
             s = self.curve.series.loc[xmin:xmax]
-            posprop = findPOIGreedy(s, pos, 'max')
-            fixedposloc = s.index.get_loc(posprop, method='nearest')
+            posprop = findPOIGreedy(s, pos, "max")
+            fixedposloc = s.index.get_loc(posprop, method="nearest")
         elif self.fixvalue is FixIndex.sndderiv:
             s = self.sndderiv.loc[xmin:xmax]
-            posprop = findPOIGreedy(s, pos, 'max')
-            fixedposloc = s.index.get_loc(posprop, method='nearest')
+            posprop = findPOIGreedy(s, pos, "max")
+            fixedposloc = s.index.get_loc(posprop, method="nearest")
         else:
             s = self.curve.series.loc[xmin:xmax]
-            fixedposloc = s.index.get_loc(pos, method='nearest')
+            fixedposloc = s.index.get_loc(pos, method="nearest")
         correctedpos = s.index[fixedposloc]
         return correctedpos
 
     @property
     def sndderiv(self):
         if self.__sndderiv is None:
             sndderiv = self.curve.series.diff().diff().iloc[1:]
```

### Comparing `graphysio-2022.9.13/graphysio/plotwidgets/puplot.py` & `graphysio-2024.5.7/graphysio/plotwidgets/puplot.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import numpy as np
 import pandas as pd
 import pyqtgraph as pg
 from graphysio import ui
 from graphysio.writedata import exporter
 from pyqtgraph import QtWidgets
 
-Point = namedtuple('Point', ['x', 'y'])
-Cardinals = namedtuple('Cardinals', ['A', 'B', 'C'])
-Angles = namedtuple('Angles', ['alpha', 'beta', 'gala'])
+Point = namedtuple("Point", ["x", "y"])
+Cardinals = namedtuple("Cardinals", ["A", "B", "C"])
+Angles = namedtuple("Angles", ["alpha", "beta", "gala"])
 
 
 class LoopWidget(ui.Ui_LoopWidget, QtWidgets.QWidget):
     def __init__(self, u, p, subsetrange, parent):
         super().__init__(parent=parent)
         self.setupUi(self)
         self.properties = {}
@@ -25,16 +25,16 @@
 
         self.btnPrev.clicked.connect(self.prevloop)
         self.btnNext.clicked.connect(self.nextloop)
         self.btnDelete.clicked.connect(self.delloop)
 
         self.curidx = 0
         self.loops = []
-        self.pen = p.opts['pen']
-        self.graphicsView.setBackground('w')
+        self.pen = p.opts["pen"]
+        self.graphicsView.setBackground("w")
 
         plotitem = self.graphicsView.getPlotItem()
         vb = plotitem.getViewBox()
         vb.setAspectLocked(lock=True, ratio=1)
 
         self.curveitem = pg.PlotCurveItem()
         self.scatteritem = pg.ScatterPlotItem()
@@ -103,29 +103,29 @@
             # Handle the case where we deleted the last item
             self.curidx = len(self.loops) - 1
         self.lblTot.setText(str(len(self.loops)))
         self.renderloop()
 
     @property
     def menu(self):
-        return {'Export': {'&Loop Data to CSV directory': self.exporter.exportloops}}
+        return {"Export": {"&Loop Data to CSV directory": self.exporter.exportloops}}
 
 
 class PULoop(object):
     def __init__(self, u, p):
         self.__angles = None
         self.__cardpoints = None
 
         # Realign pressure and flow
         offset = p.index[0] - u.index[0]
         u.index += offset
         self.offset = abs(offset)
 
         df = pd.concat([u, p], axis=1)
-        self.df = df.interpolate(method='index')
+        self.df = df.interpolate(method="index")
 
         self.u = self.df[u.name]
         self.p = self.df[p.name]
 
     @property
     def cardpoints(self):
         if self.__cardpoints is None:
```

### Comparing `graphysio-2022.9.13/graphysio/plotwidgets/spectrogram.py` & `graphysio-2024.5.7/graphysio/plotwidgets/spectrogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,32 +11,32 @@
         super().__init__(parent=parent)
         self.spectro = SpectrogramPlotWidget(series, Fs, s_chunklen, parent)
         self.loslider = QtWidgets.QSlider()
         self.hislider = QtWidgets.QSlider()
         layout = QtWidgets.QHBoxLayout()
 
         lolayout = QtWidgets.QVBoxLayout()
-        lothres = QtWidgets.QLabel('Low')
+        lothres = QtWidgets.QLabel("Low")
         lolayout.addWidget(lothres)
         lolayout.addWidget(self.loslider)
 
         hilayout = QtWidgets.QVBoxLayout()
-        hithres = QtWidgets.QLabel('High')
+        hithres = QtWidgets.QLabel("High")
         hilayout.addWidget(hithres)
         hilayout.addWidget(self.hislider)
 
         layout.addWidget(self.spectro)
         layout.addLayout(lolayout)
         layout.addLayout(hilayout)
         self.setLayout(layout)
 
     @property
     def menu(self):
-        mplot = {'Extract SEF': self.spectro.launchSEFExtract}
-        return {'Plot': mplot}
+        mplot = {"Extract SEF": self.spectro.launchSEFExtract}
+        return {"Plot": mplot}
 
 
 class SpectroTimeAxisItem(pg.AxisItem):
     def __init__(self, initvalue, samplerate, chunksize, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.initvalue = initvalue / 1e6  # ns to ms
         self.samplerate = samplerate
@@ -70,22 +70,22 @@
         self.chunksize = int(s_chunklen * Fs)
         self.win = np.hanning(self.chunksize)
 
         axisItem = SpectroTimeAxisItem(
             initvalue=self.origidx[0],
             samplerate=self.fs,
             chunksize=self.chunksize,
-            orientation='bottom',
+            orientation="bottom",
         )
-        axisItems = {'bottom': axisItem}
+        axisItems = {"bottom": axisItem}
         super().__init__(parent=self.parent, axisItems=axisItems)
 
         self.img = pg.ImageItem()
         self.addItem(self.img)
-        self.setLabel('left', 'Frequency', units='Hz')
+        self.setLabel("left", "Frequency", units="Hz")
 
         # bipolar colormap
         pos = np.array([0.0, 0.25, 0.5, 0.75, 1.0])
         color = np.array(
             [
                 [0, 0, 0, 255],
                 [0, 0, 255, 255],
@@ -132,19 +132,19 @@
         windows = np.lib.stride_tricks.as_strided(
             self.origidx, shape=(nwindows, winsize)
         )
         result = np.apply_along_axis(np.mean, 1, windows)
         return result.astype(int)
 
     def launchSEFExtract(self):
-        q = Parameter('SEF percentage', int)
+        q = Parameter("SEF percentage", int)
         sefperc = dialogs.askUserValue(q)
         if not sefperc:
             return
-        curvename = f'{self.name}-sef{sefperc}'
+        curvename = f"{self.name}-sef{sefperc}"
         sef = self.calcsef(sefperc)
         sefseries = pd.Series(sef, index=self.genIndex(), name=curvename)
         data = {curvename: sefseries}
         plotdata = PlotData(data, name=curvename)
         self.parent.createNewPlotWithData(plotdata)
 
     def render(self):
```

### Comparing `graphysio-2022.9.13/graphysio/plotwidgets/tsplot.py` & `graphysio-2024.5.7/graphysio/plotwidgets/tsplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import string
 from functools import partial
 
 import numexpr as ne
 import pandas as pd
+from pyqtgraph.Qt import QtCore, QtWidgets
+
 from graphysio import dialogs, transformations
 from graphysio.algorithms import filters
 from graphysio.plotwidgets import (
     LoopWidget,
     PlotWidget,
     POISelectorWidget,
     SpectrogramWidget,
 )
 from graphysio.structures import CycleId, Parameter, PlotData
 from graphysio.writedata import exporter
-from pyqtgraph.Qt import QtCore, QtGui
 
 
 class TSWidget(PlotWidget):
     def __init__(self, plotdata, parent=None, properties=None):
         if properties is None:
             properties = {}
         super().__init__(plotdata.name, parent=parent, properties=properties)
@@ -38,22 +39,16 @@
         else:
             newseries = newseries.rename(oldcurve.series.name)
             oldcurve.replace_data(newseries)
             if newsamplerate:
                 oldcurve.set_samplerate(newsamplerate)
 
     def filterFeet(self, curve, filtername, asnew=False):
-        feetdict = curve.feetitem.indices
-        oldstarts = feetdict['start']
-        oldstops = feetdict['stop']
-        starts, stops = filters.filterFeet(
-            oldstarts, oldstops, filtername, dialogs.askUserValue
-        )
-        feetdict['start'] = starts
-        feetdict['stop'] = stops
+        new_feetdict = filters.filter_feet(curve, filtername, dialogs.askUserValue)
+        curve.feetitem.indices = new_feetdict
         curve.feetitem.render()
 
     def keyPressEvent(self, event):
         if event.key() == QtCore.Qt.Key_Delete:
             for curve in self.curves.values():
                 curve.feetitem.removeSelection()
 
@@ -101,15 +96,15 @@
     def launchFilter(self, filterfeet):
         dlgFilter = dialogs.DlgFilter(parent=self.parent, filterfeet=filterfeet)
 
         def cb(result):
             createnew, curvechoices = result
             filterfunc = self.filterFeet if filterfeet else self.filterCurve
             for curvename, choice in curvechoices.items():
-                if choice == 'None':
+                if choice == "None":
                     continue
                 curve = self.curves[curvename]
                 filterfunc(curve, choice, asnew=createnew)
 
         dlgFilter.dlgdata.connect(cb)
         dlgFilter.exec_()
 
@@ -136,35 +131,36 @@
             "Choose Transformation",
             list(transformations.Transformations.keys()),
         )
         qresult = dialogs.askUserValue(param)
         if qresult is None:
             return
         trans = transformations.Transformations[qresult]
-        for curve in trans(self):
-            self.addCurve(curve)
+        plotdatas = trans(self)
+        for plotdata in plotdatas:
+            self.parent.appendToPlotWithData(plotdata, do_timeshift=False)
 
     # Menu Plot
     def launchPOIWidget(self):
         curvenames = list(self.curves.keys())
-        q = Parameter('Select Curve', curvenames)
+        q = Parameter("Select Curve", curvenames)
         curvename = dialogs.askUserValue(q)
         if not curvename:
             return
         curve = self.curves[curvename]
         poiselector = POISelectorWidget(
             curve.series, parent=self.parent, properties=self.properties
         )
         self.parent.addTab(poiselector, curve.name())
 
     def launchSpectrogram(self):
         curvenames = list(self.curves.keys())
-        q = Parameter('Select Curve', curvenames)
+        q = Parameter("Select Curve", curvenames)
         curvename = dialogs.askUserValue(q)
-        q = Parameter('Enter time window', 'time')
+        q = Parameter("Enter time window", "time")
         window = dialogs.askUserValue(q)
         if not curvename:
             return
         curve = self.curves[curvename]
         spectro = SpectrogramWidget(
             curve.series, curve.samplerate, window, parent=self.parent
         )
@@ -179,100 +175,100 @@
             curvenames = [curvecorr[x] for x in symbols]
             sers = [self.curves[c].series for c in curvenames]
             if not len(sers):
                 return
 
             argsdf = pd.concat(sers, axis=1, keys=symbols)
             argsdf = argsdf.interpolate()
-            args = argsdf.to_dict(orient='series')
+            args = argsdf.to_dict(orient="series")
 
             newvals = ne.evaluate(formula, local_dict=args)
             newname = self.validateNewCurveName(formula, True)
             newseries = pd.Series(
-                newvals, index=argsdf.index, name=newname, dtype='float64'
+                newvals, index=argsdf.index, name=newname, dtype="float64"
             )
             self.addSeriesAsCurve(newseries)
 
         dlgCurveAlgebra.dlgdata.connect(cb)
         dlgCurveAlgebra.exec_()
 
     # Menu Selection
     def launchNewPlotFromSelection(self):
         xmin, xmax = self.vbrange
         sers = []
         for c in self.curves.values():
             series = c.series.loc[xmin:xmax]
             sers.append(series)
         df = pd.concat(sers, axis=1, keys=[s.name for s in sers])
-        newname = f'{self.name}-sub'
+        newname = f"{self.name}-sub"
         plotdata = PlotData(data=df, name=newname)
         self.parent.createNewPlotWithData(plotdata)
 
     def launchAppendToPlotFromSelection(self):
         tabWidget = self.parent.tabWidget
         ntabs = tabWidget.count()
         tabdict = {tabWidget.tabText(idx): idx for idx in range(ntabs)}
-        desttabname, ok = QtGui.QInputDialog.getItem(
+        desttabname, ok = QtWidgets.QInputDialog.getItem(
             self,
-            'Select destination',
-            'Destination plot',
+            "Select destination",
+            "Destination plot",
             list(tabdict.keys()),
             editable=False,
         )
         if not ok:
             return
         xmin, xmax = self.vbrange
         sers = []
         for c in self.curves.values():
             series = c.series.loc[xmin:xmax]
             sers.append(series)
         df = pd.concat(sers, axis=1, keys=[s.name for s in sers])
-        newname = f'{self.name}-sub'
+        newname = f"{self.name}-sub"
         plotdata = PlotData(data=df, name=newname)
         self.parent.appendToPlotWithData(plotdata, destidx=tabdict[desttabname])
 
     def launchLoop(self):
         dlgSetupPU = dialogs.DlgSetupPULoop(self, parent=self.parent)
 
         def cb(result):
             uname, pname = result
             u = self.curves[uname]
             p = self.curves[pname]
             loopwidget = LoopWidget(u, p, self.vbrange, parent=self.parent)
-            newname = f'{self.name}-{p.name()}-loops'
+            newname = f"{self.name}-{p.name()}-loops"
             self.parent.addTab(loopwidget, newname)
 
         dlgSetupPU.dlgdata.connect(cb)
         dlgSetupPU.exec_()
 
     @property
     def menu(self):
         mcurves = {
-            'Visible Curves': self.showCurveList,
-            'Cycle Detection': self.launchCycleDetection,
-            'Filter Curve': partial(self.launchFilter, filterfeet=False),
-            'Filter Feet': partial(self.launchFilter, filterfeet=True),
-            'Transformation': self.launchTransformation,
-            'Set Date / Time': self.setDateTime,
+            "Visible Curves": self.showCurveList,
+            "Cycle Detection": self.launchCycleDetection,
+            "Filter Curve": partial(self.launchFilter, filterfeet=False),
+            "Filter Feet": partial(self.launchFilter, filterfeet=True),
+            "Transformation": self.launchTransformation,
+            "Set Date / Time": self.setDateTime,
         }
         mselect = {
-            'As new plot': self.launchNewPlotFromSelection,
-            'Append to other plot': self.launchAppendToPlotFromSelection,
-            'Generate PU-Loops': self.launchLoop,
+            "As new plot": self.launchNewPlotFromSelection,
+            "Append to other plot": self.launchAppendToPlotFromSelection,
+            "Generate PU-Loops": self.launchLoop,
         }
         mplot = {
-            'POI Selector': self.launchPOIWidget,
-            'Spectrogram': self.launchSpectrogram,
-            'Curve Algebra': self.launchCurveAlgebra,
+            "POI Selector": self.launchPOIWidget,
+            "Spectrogram": self.launchSpectrogram,
+            "Curve Algebra": self.launchCurveAlgebra,
         }
         mexport = {
-            'Curves': self.exporter.curves,
-            'Time info': self.exporter.periods,
-            'Cycle info': self.exporter.cyclepoints,
-            'Cycles to directory': self.exporter.cycles,
+            "Curves": self.exporter.curves,
+            "Time info": self.exporter.periods,
+            "Cycle info": self.exporter.cyclepoints,
+            "Cycles to directory": self.exporter.cycles,
         }
         return {
-            'Curves': mcurves,
-            'Plot': mplot,
-            'Seletion': mselect,
-            'Export': mexport,
+            "Curves": mcurves,
+            "Plot": mplot,
+            "Seletion": mselect,
+            "Export": mexport,
         }
```

### Comparing `graphysio-2022.9.13/graphysio/readdata/__init__.py` & `graphysio-2024.5.7/graphysio/readdata/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 
 from graphysio.dialogs import askOpenFilePath
 
 from .csv import CsvReader
 from .edf import EdfReader
 from .parquet import ParquetReader
 
-file_readers = {'csv': CsvReader, 'parquet': ParquetReader, 'edf': EdfReader}
+file_readers = {"csv": CsvReader, "parquet": ParquetReader, "edf": EdfReader}
 file_readers = {k: mod for k, mod in file_readers.items() if mod.is_available}
 
 
 class FileReader:
     def __init__(self):
         super().__init__()
         self.reader = None
 
-        filters = ';;'.join(
-            [f'{ext.upper()} files (*.{ext})(*.{ext})' for ext in file_readers]
+        filters = ";;".join(
+            [f"{ext.upper()} files (*.{ext})(*.{ext})" for ext in file_readers]
         )
-        supported = ' '.join(f'*.{ext}' for ext in file_readers)
-        self.file_filters = f'All supported ({supported});;{filters}'
+        supported = " ".join(f"*.{ext}" for ext in file_readers)
+        self.file_filters = f"All supported ({supported});;{filters}"
 
-    def askFile(self, folder='') -> 'pathlib.PurePath':
+    def askFile(self, folder="") -> "pathlib.PurePath":
         filepath, ext = askOpenFilePath(
-            'Open File', folder=folder, filter=self.file_filters
+            "Open File", folder=folder, filter=self.file_filters
         )
         if not filepath:
             return folder
         self.reader = file_readers[ext]()
-        self.reader.set_data({'filepath': filepath})
+        self.reader.set_data({"filepath": filepath})
         self.reader.askUserInput()
         # Return the parent folder for caching
         return filepath.parent
 
     # Meant to be executed in seperate thread
     def get_plotdata(self):
         if self.reader:
```

### Comparing `graphysio-2022.9.13/graphysio/readdata/csv.py` & `graphysio-2024.5.7/graphysio/readdata/csv.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,91 +2,98 @@
 from dataclasses import dataclass
 from functools import partial
 from pathlib import Path
 from typing import List
 
 import numpy as np
 import pandas as pd
+from pyqtgraph.Qt import QtCore, QtGui, QtWidgets
+
 from graphysio import ui
 from graphysio.readdata.baseclass import BaseReader
 from graphysio.structures import PlotData
-from pyqtgraph.Qt import QtCore, QtGui, QtWidgets
 
 
 class CsvReader(BaseReader):
     is_available = True
 
     def askUserInput(self):
-        filepath = self.userdata['filepath']
+        filepath = self.userdata["filepath"]
         dlg = DlgNewPlotCsv(filepath)
         dlg.exec_()
         csvrequest = dlg.csvrequest
         if csvrequest:
-            self.userdata['csvrequest'] = dlg.csvrequest
+            self.userdata["csvrequest"] = dlg.csvrequest
 
     def __call__(self) -> List[PlotData]:
-        request = self.userdata['csvrequest']
+        request = self.userdata["csvrequest"]
         data = pd.read_csv(
             request.filepath,
             sep=request.seperator,
             usecols=request.fields,
             decimal=request.decimal,
             skiprows=request.droplines,
             encoding=request.encoding,
             index_col=False,
-            engine='c',
+            engine="c",
         )
-        pdtonum = partial(pd.to_numeric, errors='coerce')
+        pdtonum = partial(pd.to_numeric, errors="coerce")
         dtformat = request.datetime_format
         if request.generatex:
             data.index = (1e9 * data.index / request.samplerate).astype(np.int64)
             # Make all data numeric and remove empty rows
-            data = data.apply(pdtonum)
-            data = data.dropna(axis='rows', how='all')
+            datacols = data.columns.difference([request.clusterid])
+            data[datacols] = data[datacols].apply(pdtonum)
+            data = data.dropna(axis="rows", how="all", subset=datacols)
         else:
             timestamp = data[request.dtfield]
             data = data.drop(columns=request.dtfield)
             # Force all columns to numeric
-            data = data.apply(pdtonum)
+            datacols = data.columns.difference([request.clusterid])
+            data[datacols] = data[datacols].apply(pdtonum)
+            # data = data.dropna(axis="rows", how="all", subset=datacols)
+            nanrows = data[datacols].isna().all(axis=1)
+            data = data[~nanrows]
+            timestamp = timestamp[~nanrows]
 
-            if dtformat == '<seconds>':
+            if dtformat == "<seconds>":
                 timestamp = pdtonum(timestamp)
-                timestamp = pd.to_datetime(timestamp * 1e9, unit='ns')
-            elif dtformat == '<milliseconds>':
+                timestamp = pd.to_datetime(timestamp * 1e9, unit="ns")
+            elif dtformat == "<milliseconds>":
                 timestamp = pdtonum(timestamp)
-                timestamp = pd.to_datetime(timestamp * 1e6, unit='ns')
-            elif dtformat == '<microseconds>':
+                timestamp = pd.to_datetime(timestamp * 1e6, unit="ns")
+            elif dtformat == "<microseconds>":
                 timestamp = pdtonum(timestamp)
-                timestamp = pd.to_datetime(timestamp * 1e3, unit='ns')
-            elif dtformat == '<nanoseconds>':
+                timestamp = pd.to_datetime(timestamp * 1e3, unit="ns")
+            elif dtformat == "<nanoseconds>":
                 timestamp = pdtonum(timestamp)
-                timestamp = pd.to_datetime(timestamp, unit='ns')
-            elif dtformat == '<infer>':
+                timestamp = pd.to_datetime(timestamp, unit="ns")
+            elif dtformat == "<infer>":
                 timestamp = pd.to_datetime(timestamp, infer_datetime_format=True)
             else:
                 timestamp = pd.to_datetime(timestamp, format=dtformat)
                 timestamp = pd.Index(timestamp)
                 if timestamp.tz is None:
                     timestamp = timestamp.tz_localize(request.timezone)
-                timestamp = timestamp.tz_convert('UTC')
+                timestamp = timestamp.tz_convert("UTC")
 
-            timestamp = timestamp.view(np.int64)
+            timestamp = timestamp.astype(np.int64)
             data = data.set_index([timestamp])
 
-        data = data.dropna(axis='columns', how='all')
+        data = data.dropna(axis="columns", how="all")
         data = data.sort_index()
 
         fp = request.filepath
         if request.clusterid:
             g = data.groupby(request.clusterid)
             plotdata = (
                 PlotData(
                     data=df.drop(columns=request.clusterid),
                     filepath=fp,
-                    name=f'{fp.stem}-{i}',
+                    name=f"{fp.stem}-{i}",
                 )
                 for i, df in g
             )
         else:
             plotdata = [PlotData(data=data, filepath=fp)]
 
         return plotdata
@@ -116,15 +123,15 @@
         return dtfields + clusterfields + self.yfields
 
 
 class DlgNewPlotCsv(ui.Ui_NewPlot, QtWidgets.QDialog):
     def __init__(self, filepath, parent=None):
         super().__init__(parent=parent)
         self.setupUi(self)
-        self.setWindowTitle(f'Open {filepath.name}')
+        self.setWindowTitle(f"Open {filepath.name}")
 
         self.filepath = filepath
         self.csvrequest = None
 
         # Attach models to ListViews
         self.lstX = QtGui.QStandardItemModel()
         self.lstY = QtGui.QStandardItemModel()
@@ -134,16 +141,18 @@
         self.lstVX.setModel(self.lstX)
         self.lstVY.setModel(self.lstY)
         self.lstVCluster.setModel(self.lstCluster)
         self.lstVAll.setModel(self.lstAll)
 
         # Setup Field Table
         self.lstVAll.verticalHeader().hide()
-        self.lstVAll.horizontalHeader().setResizeMode(QtGui.QHeaderView.Stretch)
-        self.lstVAll.setSelectionBehavior(QtGui.QAbstractItemView.SelectRows)
+        self.lstVAll.horizontalHeader().setSectionResizeMode(
+            QtWidgets.QHeaderView.Stretch
+        )
+        self.lstVAll.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
 
         # Connect callbacks
         self.btnLoad.clicked.connect(self.loadCsvFields)
         self.btnOk.clicked.connect(self.loadPlot)
         self.btnCancel.clicked.connect(self.reject)
         self.btnToX.clicked.connect(self.moveToX)
         self.btnToY.clicked.connect(self.moveToY)
@@ -153,34 +162,34 @@
         self.btnRemoveCluster.clicked.connect(self.delFromCluster)
         self.lstVX.currentIndexChanged.connect(self.xChanged)
 
         # Guesstimate CSV field and decimal seperators
         delims = self.estimateDelimiters(filepath)
         self.txtSep.setEditText(delims[0])
         self.txtDecimal.setEditText(delims[1])
-        self.txtDateTime.setEditText(f'%Y-%m-%d %H:%M:%S{delims[1]}%f')
+        self.txtDateTime.setEditText(f"%Y-%m-%d %H:%M:%S{delims[1]}%f")
 
     # Methods / Callbacks
     def estimateDelimiters(self, filepath):
         encoding = self.txtEncoding.currentText()
-        with open(filepath, 'r', encoding=encoding) as csvfile:
-            seperator = ';' if ';' in next(csvfile) else ','
-            decimal = '.' if '.' in next(csvfile) else ','
+        with open(filepath, "r", encoding=encoding) as csvfile:
+            seperator = ";" if ";" in next(csvfile) else ","
+            decimal = "." if "." in next(csvfile) else ","
         return (seperator, decimal)
 
     def loadCsvFields(self):
         sep = self.txtSep.currentText()
-        if sep == '<tab>':
-            sep = '\t'
+        if sep == "<tab>":
+            sep = "\t"
         # Use the csv module to retrieve csv fields
         for lst in [self.lstAll, self.lstX, self.lstY]:
             lst.clear()
         self.lstAll.setHorizontalHeaderLabels(["Field", "1st Line"])
         encoding = self.txtEncoding.currentText()
-        with open(self.filepath, 'r', encoding=encoding) as csvfile:
+        with open(self.filepath, "r", encoding=encoding) as csvfile:
             # Artificially drop n first lines as requested
             for _ in range(self.spnLinedrop.value()):
                 next(csvfile)
             csvreader = csv.DictReader(csvfile, delimiter=sep)
             row = next(csvreader)
             for key, value in row.items():
                 if key is None:
@@ -246,15 +255,15 @@
         yRows = [i.text() for i in self.lstY.findItems("", QtCore.Qt.MatchContains)]
         xRows = [i.text() for i in self.lstX.findItems("", QtCore.Qt.MatchContains)]
         cRows = [
             i.text() for i in self.lstCluster.findItems("", QtCore.Qt.MatchContains)
         ]
 
         seperator = self.txtSep.currentText()
-        seperator = '\t' if seperator == '<tab>' else seperator
+        seperator = "\t" if seperator == "<tab>" else seperator
 
         generatex = self.chkGenX.checkState() > QtCore.Qt.Unchecked
         try:
             dtfield = xRows[0]
         except IndexError:
             dtfield = None
```

### Comparing `graphysio-2022.9.13/graphysio/readdata/edf.py` & `graphysio-2024.5.7/graphysio/readdata/edf.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,45 +12,45 @@
     is_available = True
 
 
 class EdfReader(BaseReader):
     is_available = is_available
 
     def askUserInput(self):
-        filepath = str(self.userdata['filepath'])
+        filepath = str(self.userdata["filepath"])
         edf = pyedflib.EdfReader(filepath)
 
         signals = {}
         for i in range(edf.signals_in_file):
             h = edf.getSignalHeader(i)
-            signals[h['label']] = i
+            signals[h["label"]] = i
         edf.close()
 
         def cb(colnames):
-            self.userdata['columns'] = [signals[lbl] for lbl in colnames]
+            self.userdata["columns"] = [signals[lbl] for lbl in colnames]
 
         colnames = list(signals.keys())
-        dlgchoice = DlgListChoice(colnames, 'Open EDF', 'Choose curves to load')
+        dlgchoice = DlgListChoice(colnames, "Open EDF", "Choose curves to load")
         dlgchoice.dlgdata.connect(cb)
         dlgchoice.exec_()
 
     def __call__(self) -> PlotData:
-        filepath = str(self.userdata['filepath'])
+        filepath = str(self.userdata["filepath"])
         edf = pyedflib.EdfReader(filepath)
         beginns = edf.getStartdatetime().timestamp() * 1e9
         nsamplesPerChannel = edf.getNSamples()
 
         signals = []
-        for i in self.userdata['columns']:
+        for i in self.userdata["columns"]:
             h = edf.getSignalHeader(i)
-            fs = h['sample_rate']
+            fs = h["sample_rate"]
             n = nsamplesPerChannel[i]
             endns = beginns + n * 1e9 / fs
             idx = np.linspace(beginns, endns, num=n, dtype=np.int64)
-            s = pd.Series(edf.readSignal(i), index=idx, name=h['label'])
+            s = pd.Series(edf.readSignal(i), index=idx, name=h["label"])
             signals.append(s)
         edf.close()
 
         if not signals:
             return None
 
         df = pd.concat(signals, axis=1)
```

### Comparing `graphysio-2022.9.13/graphysio/readdata/parquet.py` & `graphysio-2024.5.7/graphysio/readdata/parquet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import pandas as pd
+
 from graphysio.dialogs import DlgListChoice
 from graphysio.readdata.baseclass import BaseReader
 from graphysio.structures import PlotData
 
 try:
     import pyarrow.parquet as pa
 except ImportError:
@@ -12,27 +13,27 @@
     is_available = True
 
 
 class ParquetReader(BaseReader):
     is_available = is_available
 
     def askUserInput(self):
-        filepath = self.userdata['filepath']
+        filepath = self.userdata["filepath"]
         s = pa.read_schema(filepath)
         colnames = s.names
 
         def cb(columns):
-            self.userdata['columns'] = columns
+            self.userdata["columns"] = columns
 
-        dlgchoice = DlgListChoice(colnames, 'Open Parquet', 'Choose curves to load')
+        dlgchoice = DlgListChoice(colnames, "Open Parquet", "Choose curves to load")
         dlgchoice.dlgdata.connect(cb)
         dlgchoice.exec_()
 
     def __call__(self) -> PlotData:
-        filepath = self.userdata['filepath']
-        data = pd.read_parquet(filepath, columns=self.userdata['columns'])
+        filepath = self.userdata["filepath"]
+        data = pd.read_parquet(filepath, columns=self.userdata["columns"])
 
-        data = data.dropna(axis='columns', how='all')
+        data = data.dropna(axis="columns", how="all")
         data = data.sort_index()
-        data.index = data.index.view(np.int64)
+        data.index = data.index.astype(np.int64)
 
         return PlotData(data=data, filepath=filepath)
```

### Comparing `graphysio-2022.9.13/graphysio/structures.py` & `graphysio-2024.5.7/graphysio/structures.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 from collections import namedtuple
 from enum import Enum
 from pathlib import Path
 from typing import Optional
 
-Filter = namedtuple('Filter', ['name', 'parameters'])
-Parameter = namedtuple('Parameter', ['description', 'request'])
+import pandas as pd
+
+Filter = namedtuple("Filter", ["name", "parameters"])
+Parameter = namedtuple("Parameter", ["description", "request"])
 
 
 class CycleId(Enum):
-    none = 'None'
-    foot = 'Pressure foot'
-    pressure = 'Pressure Full'
-    velocity = 'Velocity'
-    rwave = 'ECG R Wave'
-    foottan = 'Pressure foot (tangents)'
-    pressurebis = 'Pressure full (physiocurve)'
-    ecg = 'ECG full'
+    none = "None"
+    foot = "Pressure foot"
+    pressure = "Pressure Full"
+    velocity = "Velocity"
+    rwave = "ECG R Wave"
+    foottan = "Pressure foot (tangents)"
+    pressurebis = "Pressure full (physiocurve)"
+    ecg = "ECG full"
 
 
 class PlotData:
     def __init__(
         self, data, filepath: Optional[Path] = None, name: Optional[str] = None
     ):
         if filepath is None and name is None:
-            raise ValueError('At least one of filepath or name needs to be specified.')
+            raise ValueError("At least one of filepath or name needs to be specified.")
         if filepath is not None:
             self.filepath = Path(filepath)
         self._name = name
-        self.data = data
+        if isinstance(data, pd.Series):
+            self.data = data.to_frame(name=self.name)
+        else:
+            self.data = data
 
     @property
     def name(self):
         if self._name is not None:
             name = self._name
         else:
             name = self.filepath.stem
```

### Comparing `graphysio-2022.9.13/graphysio/transformations/feet_to_curve.py` & `graphysio-2024.5.7/graphysio/transformations/feet_time_interval.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from typing import List
 
 from graphysio.dialogs import askUserValue
 from graphysio.plotwidgets import PlotWidget
 from graphysio.plotwidgets.curves import CurveItemWithPOI
-from graphysio.structures import Parameter
+from graphysio.structures import Parameter, PlotData
 
 
-def get_feet_to_curve(plotwidget: PlotWidget) -> List[CurveItemWithPOI]:
+def get_feet_time_interval(plotwidget: PlotWidget) -> List[CurveItemWithPOI]:
     feetitemhash = {}
     for curve in plotwidget.curves.values():
         feetitemhash.update(
             {
-                f'{curve.name()}-{feetname}': (curve, feetname)
+                f"{curve.name()}-{feetname}": (curve, feetname)
                 for feetname in curve.feetitem.indices.keys()
             }
         )
     param = Parameter("Choose points to create curve", list(feetitemhash.keys()))
     qresult = askUserValue(param)
     curve, feetname = feetitemhash[qresult]
 
-    newseries = curve.getFeetPoints(feetname)
-    newseries.name = qresult
+    points = curve.getFeetPoints(feetname)
+    time_intervals = points.index.to_series().diff()  # ns
+    time_intervals /= 1e6  # ms
 
-    newcurve = CurveItemWithPOI(
-        parent=plotwidget, series=newseries, pen=plotwidget.getPen()
-    )
-    return [newcurve]
+    sname = f"{qresult}(ms)"
+
+    plotdata = PlotData(data=time_intervals, name=sname)
+    return [plotdata]
```

### Comparing `graphysio-2022.9.13/graphysio/transformations/perfusion_index.py` & `graphysio-2024.5.7/graphysio/transformations/perfusion_index.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 from typing import List
 
 import pandas as pd
 from graphysio.dialogs import askUserValue
 from graphysio.plotwidgets import PlotWidget
 from graphysio.plotwidgets.curves import CurveItemWithPOI
-from graphysio.structures import Parameter
+from graphysio.structures import Parameter, PlotData
 
 
 def get_perfusion_index(plotwidget: PlotWidget) -> List[CurveItemWithPOI]:
     curvenames = list(plotwidget.curves.keys())
     curvenames = list(plotwidget.curves.keys())
     if len(curvenames) < 1:
-        raise ValueError('No curve')
+        raise ValueError("No curve")
     elif len(curvenames) > 1:
-        q = Parameter('Select Curve', curvenames)
+        q = Parameter("Select Curve", curvenames)
         curvename = askUserValue(q)
     else:
         curvename = curvenames[0]
 
     curve = plotwidget.curves[curvename]
     if (
-        'start' not in curve.feetitem.indices
-        or curve.feetitem.indices['start'].size < 1
+        "start" not in curve.feetitem.indices
+        or curve.feetitem.indices["start"].size < 1
     ):
-        raise ValueError('No start information for curve')
+        raise ValueError("No start information for curve")
 
     wave = curve.series
-    starts = curve.getFeetPoints('start')
+    starts = curve.getFeetPoints("start")
     df = pd.concat([wave, starts], axis=1)
-    df = df.interpolate(method='index')
+    df = df.interpolate(method="index")
 
     begins, durations = curve.getCycleIndices()
     pivalues = []
     for begin, duration in zip(begins, durations):
         cycle = df.loc[begin : begin + duration]
         auctot = cycle[wave.name].sum()
         aucbase = cycle[starts.name].sum()
         aucpulse = auctot - aucbase
         pi = aucpulse / auctot
         pivalues.append(pi)
 
-    piseries = pd.Series(pivalues, index=begins)
-    piseries.name = f'{wave.name}-perf'
+    out_series = pd.Series(pivalues, index=begins)
+    sname = f"{wave.name}-perf"
 
-    newcurve = CurveItemWithPOI(
-        parent=plotwidget, series=piseries, pen=plotwidget.getPen()
-    )
-    return [newcurve]
+    plotdata = PlotData(data=out_series, name=sname)
+    return [plotdata]
```

### Comparing `graphysio-2022.9.13/graphysio/transformations/precise_feet.py` & `graphysio-2024.5.7/graphysio/transformations/precise_feet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 from typing import List
 
 import numpy as np
 import pandas as pd
 from graphysio.dialogs import askUserValue
 from graphysio.plotwidgets import PlotWidget
 from graphysio.plotwidgets.curves import CurveItemWithPOI
-from graphysio.structures import Parameter
+from graphysio.structures import Parameter, PlotData
 from physiocurve.pressure.foot import find_tangent_intersections
 
 
 def get_precise_feet(plotwidget: PlotWidget) -> List[CurveItemWithPOI]:
     curvenames = list(plotwidget.curves.keys())
     if len(curvenames) < 1:
-        raise ValueError('No curve')
+        raise ValueError("No curve")
     elif len(curvenames) > 1:
-        q = Parameter('Select Curve', curvenames)
+        q = Parameter("Select Curve", curvenames)
         curvename = askUserValue(q)
     else:
         curvename = curvenames[0]
 
     curve = plotwidget.curves[curvename]
     wave = curve.series
 
     try:
-        idxdia = curve.feetitem.indices['diastole']
-        idxsys = curve.feetitem.indices['systole']
+        idxdia = curve.feetitem.indices["diastole"]
+        idxsys = curve.feetitem.indices["systole"]
     except KeyError as e:
-        raise ValueError('No systole or diastole') from e
+        raise ValueError("No systole or diastole") from e
 
     argdia = wave.index.get_indexer(idxdia)
     argsys = wave.index.get_indexer(idxsys)
 
     intersections = find_tangent_intersections(wave.to_numpy(), argdia, argsys)
 
     scale = (wave.index[-1] - wave.index[0]) / len(wave)
     intersections = intersections * scale + wave.index[0]
     intersections = np.rint(intersections).astype(np.int64)
 
-    y_value_index = wave.index.get_indexer(intersections, method='nearest')
+    y_value_index = wave.index.get_indexer(intersections, method="nearest")
     y_values = wave.iloc[y_value_index]
 
     out_series = pd.Series(y_values.to_numpy(), index=intersections)
-    out_series.name = f'{wave.name}-precise_feet'
+    sname = f"{wave.name}-precise_feet"
 
-    newcurve = CurveItemWithPOI(
-        parent=plotwidget, series=out_series, pen=plotwidget.getPen()
-    )
-
-    return [newcurve]
+    plotdata = PlotData(data=out_series, name=sname)
+    return [plotdata]
```

### Comparing `graphysio-2022.9.13/graphysio/ui/csvrequest.py` & `graphysio-2024.5.7/graphysio/ui/csvrequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,24 +76,28 @@
         self.line = QtWidgets.QFrame(NewPlot)
         self.line.setFrameShape(QtWidgets.QFrame.HLine)
         self.line.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line.setObjectName("line")
         self.verticalLayout_3.addWidget(self.line)
         self.horizontalLayout_4.addLayout(self.verticalLayout_3)
         self.groupBox_2 = QtWidgets.QGroupBox(NewPlot)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.groupBox_2.sizePolicy().hasHeightForWidth())
         self.groupBox_2.setSizePolicy(sizePolicy)
         self.groupBox_2.setObjectName("groupBox_2")
         self.verticalLayout = QtWidgets.QVBoxLayout(self.groupBox_2)
         self.verticalLayout.setObjectName("verticalLayout")
         self.lstVAll = QtWidgets.QTableView(self.groupBox_2)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.lstVAll.sizePolicy().hasHeightForWidth())
         self.lstVAll.setSizePolicy(sizePolicy)
         self.lstVAll.setSelectionMode(QtWidgets.QAbstractItemView.MultiSelection)
         self.lstVAll.setObjectName("lstVAll")
         self.verticalLayout.addWidget(self.lstVAll)
@@ -132,26 +136,32 @@
         self.txtDateTime.addItem("")
         self.txtDateTime.addItem("")
         self.txtDateTime.addItem("")
         self.txtDateTime.addItem("")
         self.txtDateTime.addItem("")
         self.txtDateTime.addItem("")
         self.txtDateTime.addItem("")
-        self.formLayout_2.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.txtDateTime)
+        self.formLayout_2.setWidget(
+            2, QtWidgets.QFormLayout.FieldRole, self.txtDateTime
+        )
         self.lstVX = QtWidgets.QComboBox(self.groupBox_6)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.lstVX.sizePolicy().hasHeightForWidth())
         self.lstVX.setSizePolicy(sizePolicy)
         self.lstVX.setMaxCount(4)
         self.lstVX.setObjectName("lstVX")
         self.formLayout_2.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.lstVX)
         self.btnRemoveX = QtWidgets.QPushButton(self.groupBox_6)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.btnRemoveX.sizePolicy().hasHeightForWidth())
         self.btnRemoveX.setSizePolicy(sizePolicy)
         self.btnRemoveX.setObjectName("btnRemoveX")
         self.formLayout_2.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.btnRemoveX)
         self.verticalLayout_2.addLayout(self.formLayout_2)
@@ -173,24 +183,28 @@
         self.groupBox_5 = QtWidgets.QGroupBox(NewPlot)
         self.groupBox_5.setObjectName("groupBox_5")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.groupBox_5)
         self.verticalLayout_7.setObjectName("verticalLayout_7")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout()
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.lstVY = QtWidgets.QListView(self.groupBox_5)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Expanding)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Expanding
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.lstVY.sizePolicy().hasHeightForWidth())
         self.lstVY.setSizePolicy(sizePolicy)
         self.lstVY.setSelectionMode(QtWidgets.QAbstractItemView.MultiSelection)
         self.lstVY.setObjectName("lstVY")
         self.verticalLayout_6.addWidget(self.lstVY)
         self.btnRemoveY = QtWidgets.QPushButton(self.groupBox_5)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.btnRemoveY.sizePolicy().hasHeightForWidth())
         self.btnRemoveY.setSizePolicy(sizePolicy)
         self.btnRemoveY.setObjectName("btnRemoveY")
         self.verticalLayout_6.addWidget(self.btnRemoveY)
         self.verticalLayout_7.addLayout(self.verticalLayout_6)
@@ -216,33 +230,37 @@
         self.line_2.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_2.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_2.setObjectName("line_2")
         self.verticalLayout_4.addWidget(self.line_2)
         self.horizontalLayout_3 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_3.setObjectName("horizontalLayout_3")
         self.btnOk = QtWidgets.QPushButton(NewPlot)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.btnOk.sizePolicy().hasHeightForWidth())
         self.btnOk.setSizePolicy(sizePolicy)
         self.btnOk.setObjectName("btnOk")
         self.horizontalLayout_3.addWidget(self.btnOk)
         self.btnCancel = QtWidgets.QPushButton(NewPlot)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.btnCancel.sizePolicy().hasHeightForWidth())
         self.btnCancel.setSizePolicy(sizePolicy)
         self.btnCancel.setObjectName("btnCancel")
         self.horizontalLayout_3.addWidget(self.btnCancel)
         self.verticalLayout_4.addLayout(self.horizontalLayout_3)
 
         self.retranslateUi(NewPlot)
-        self.chkGenX.clicked['bool'].connect(self.lstVX.setDisabled)
+        self.chkGenX.clicked["bool"].connect(self.lstVX.setDisabled)
         QtCore.QMetaObject.connectSlotsByName(NewPlot)
 
     def retranslateUi(self, NewPlot):
         _translate = QtCore.QCoreApplication.translate
         NewPlot.setWindowTitle(_translate("NewPlot", "New Plot"))
         self.label.setText(_translate("NewPlot", "Field Seperator"))
         self.txtSep.setItemText(0, _translate("NewPlot", ";"))
```

### Comparing `graphysio-2022.9.13/graphysio/ui/csvrequest.ui` & `graphysio-2024.5.7/graphysio/ui/csvrequest.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2022.9.13/graphysio/ui/curveproperties.py` & `graphysio-2024.5.7/graphysio/ui/curveproperties.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,17 @@
         self.btnColor.setObjectName("btnColor")
         self.formLayout.setWidget(6, QtWidgets.QFormLayout.FieldRole, self.btnColor)
         self.label_4 = QtWidgets.QLabel(self.grpName)
         self.label_4.setObjectName("label_4")
         self.formLayout.setWidget(7, QtWidgets.QFormLayout.LabelRole, self.label_4)
         self.lblSamplerate = QtWidgets.QLabel(self.grpName)
         self.lblSamplerate.setObjectName("lblSamplerate")
-        self.formLayout.setWidget(7, QtWidgets.QFormLayout.FieldRole, self.lblSamplerate)
+        self.formLayout.setWidget(
+            7, QtWidgets.QFormLayout.FieldRole, self.lblSamplerate
+        )
         self.cmbSymbol = QtWidgets.QComboBox(self.grpName)
         self.cmbSymbol.setObjectName("cmbSymbol")
         self.cmbSymbol.addItem("")
         self.cmbSymbol.addItem("")
         self.cmbSymbol.addItem("")
         self.cmbSymbol.addItem("")
         self.cmbSymbol.addItem("")
@@ -67,15 +69,17 @@
         self.cmbConnect.addItem("")
         self.cmbConnect.addItem("")
         self.formLayout.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.cmbConnect)
         self.verticalLayout.addWidget(self.grpName)
         self.horizontalLayout = QtWidgets.QHBoxLayout()
         self.horizontalLayout.setObjectName("horizontalLayout")
         self.okButton = QtWidgets.QPushButton(CurveProperties)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Fixed
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.okButton.sizePolicy().hasHeightForWidth())
         self.okButton.setSizePolicy(sizePolicy)
         self.okButton.setObjectName("okButton")
         self.horizontalLayout.addWidget(self.okButton)
         self.cancelButton = QtWidgets.QPushButton(CurveProperties)
```

### Comparing `graphysio-2022.9.13/graphysio/ui/curveproperties.ui` & `graphysio-2024.5.7/graphysio/ui/curveproperties.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2022.9.13/graphysio/ui/curveselect.py` & `graphysio-2024.5.7/graphysio/ui/curveselect.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,34 +22,40 @@
         self.verticalLayout.addWidget(self.lstCurves)
         self.btnProperties = QtWidgets.QPushButton(CurveSelection)
         self.btnProperties.setObjectName("btnProperties")
         self.verticalLayout.addWidget(self.btnProperties)
         self.horizontalLayout = QtWidgets.QHBoxLayout()
         self.horizontalLayout.setObjectName("horizontalLayout")
         self.okButton = QtWidgets.QPushButton(CurveSelection)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.okButton.sizePolicy().hasHeightForWidth())
         self.okButton.setSizePolicy(sizePolicy)
         self.okButton.setChecked(False)
         self.okButton.setObjectName("okButton")
         self.horizontalLayout.addWidget(self.okButton)
         self.cancelButton = QtWidgets.QPushButton(CurveSelection)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.cancelButton.sizePolicy().hasHeightForWidth())
         self.cancelButton.setSizePolicy(sizePolicy)
         self.cancelButton.setObjectName("cancelButton")
         self.horizontalLayout.addWidget(self.cancelButton)
         self.verticalLayout.addLayout(self.horizontalLayout)
 
         self.retranslateUi(CurveSelection)
         QtCore.QMetaObject.connectSlotsByName(CurveSelection)
 
     def retranslateUi(self, CurveSelection):
         _translate = QtCore.QCoreApplication.translate
-        CurveSelection.setWindowTitle(_translate("CurveSelection", "Select visible curves"))
+        CurveSelection.setWindowTitle(
+            _translate("CurveSelection", "Select visible curves")
+        )
         self.btnProperties.setText(_translate("CurveSelection", "Curve Properties"))
         self.okButton.setText(_translate("CurveSelection", "Ok"))
         self.cancelButton.setText(_translate("CurveSelection", "Cancel"))
```

### Comparing `graphysio-2022.9.13/graphysio/ui/curveselect.ui` & `graphysio-2024.5.7/graphysio/ui/curveselect.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2022.9.13/graphysio/ui/cycledetect.py` & `graphysio-2024.5.7/graphysio/ui/cycledetect.py`

 * *Files identical despite different names*

### Comparing `graphysio-2022.9.13/graphysio/ui/cycledetect.ui` & `graphysio-2024.5.7/graphysio/ui/cycledetect.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2022.9.13/graphysio/ui/datetime.py` & `graphysio-2024.5.7/graphysio/ui/datetime.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,17 @@
         self.gridLayout = QtWidgets.QGridLayout(SetDateTime)
         self.gridLayout.setObjectName("gridLayout")
         self.widgetCalendar = QtWidgets.QCalendarWidget(SetDateTime)
         self.widgetCalendar.setFirstDayOfWeek(QtCore.Qt.Monday)
         self.widgetCalendar.setGridVisible(True)
         self.widgetCalendar.setObjectName("widgetCalendar")
         self.gridLayout.addWidget(self.widgetCalendar, 0, 2, 1, 1)
-        spacerItem = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        spacerItem = QtWidgets.QSpacerItem(
+            40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum
+        )
         self.gridLayout.addItem(spacerItem, 0, 0, 1, 1)
         self.edDate = QtWidgets.QDateEdit(SetDateTime)
         self.edDate.setObjectName("edDate")
         self.gridLayout.addWidget(self.edDate, 1, 2, 1, 1)
         self.edTime = QtWidgets.QTimeEdit(SetDateTime)
         self.edTime.setObjectName("edTime")
         self.gridLayout.addWidget(self.edTime, 2, 2, 1, 1)
@@ -34,40 +36,48 @@
         self.label_2.setObjectName("label_2")
         self.gridLayout.addWidget(self.label_2, 2, 0, 1, 1)
         self.label = QtWidgets.QLabel(SetDateTime)
         self.label.setObjectName("label")
         self.gridLayout.addWidget(self.label, 1, 0, 1, 1)
         self.horizontalLayout = QtWidgets.QHBoxLayout()
         self.horizontalLayout.setObjectName("horizontalLayout")
-        spacerItem1 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        spacerItem1 = QtWidgets.QSpacerItem(
+            40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum
+        )
         self.horizontalLayout.addItem(spacerItem1)
         self.btnOk = QtWidgets.QPushButton(SetDateTime)
         self.btnOk.setObjectName("btnOk")
         self.horizontalLayout.addWidget(self.btnOk)
-        spacerItem2 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        spacerItem2 = QtWidgets.QSpacerItem(
+            40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum
+        )
         self.horizontalLayout.addItem(spacerItem2)
         self.gridLayout.addLayout(self.horizontalLayout, 3, 0, 1, 1)
         self.horizontalLayout_2 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_2.setObjectName("horizontalLayout_2")
-        spacerItem3 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        spacerItem3 = QtWidgets.QSpacerItem(
+            40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum
+        )
         self.horizontalLayout_2.addItem(spacerItem3)
         self.btnCancel = QtWidgets.QPushButton(SetDateTime)
         self.btnCancel.setObjectName("btnCancel")
         self.horizontalLayout_2.addWidget(self.btnCancel)
-        spacerItem4 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        spacerItem4 = QtWidgets.QSpacerItem(
+            40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum
+        )
         self.horizontalLayout_2.addItem(spacerItem4)
         self.gridLayout.addLayout(self.horizontalLayout_2, 3, 2, 1, 1)
         self.widgetCalendar.raise_()
         self.edTime.raise_()
         self.label_2.raise_()
         self.label.raise_()
         self.edDate.raise_()
 
         self.retranslateUi(SetDateTime)
-        self.widgetCalendar.clicked['QDate'].connect(self.edDate.setDate)
+        self.widgetCalendar.clicked["QDate"].connect(self.edDate.setDate)
         QtCore.QMetaObject.connectSlotsByName(SetDateTime)
 
     def retranslateUi(self, SetDateTime):
         _translate = QtCore.QCoreApplication.translate
         SetDateTime.setWindowTitle(_translate("SetDateTime", "Set Date and Time"))
         self.edDate.setDisplayFormat(_translate("SetDateTime", "dd/MM/yyyy"))
         self.edTime.setDisplayFormat(_translate("SetDateTime", "hh:mm:ss.zzz"))
```

### Comparing `graphysio-2022.9.13/graphysio/ui/datetime.ui` & `graphysio-2024.5.7/graphysio/ui/datetime.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2022.9.13/graphysio/ui/filter.py` & `graphysio-2024.5.7/graphysio/ui/filter.py`

 * *Files identical despite different names*

### Comparing `graphysio-2022.9.13/graphysio/ui/filter.ui` & `graphysio-2024.5.7/graphysio/ui/filter.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2022.9.13/graphysio/ui/loopwidget.py` & `graphysio-2024.5.7/graphysio/ui/loopwidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         self.lblDelay = QtWidgets.QLabel(LoopWidget)
         self.lblDelay.setText("")
         self.lblDelay.setObjectName("lblDelay")
         self.gridLayout.addWidget(self.lblDelay, 5, 1, 1, 1)
         self.btnPrev = QtWidgets.QPushButton(LoopWidget)
         self.btnPrev.setObjectName("btnPrev")
         self.gridLayout.addWidget(self.btnPrev, 1, 0, 1, 1)
-        spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem = QtWidgets.QSpacerItem(
+            20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding
+        )
         self.gridLayout.addItem(spacerItem, 4, 0, 1, 1)
         self.label_2 = QtWidgets.QLabel(LoopWidget)
         self.label_2.setObjectName("label_2")
         self.gridLayout.addWidget(self.label_2, 2, 1, 1, 1)
         self.label = QtWidgets.QLabel(LoopWidget)
         self.label.setObjectName("label")
         self.gridLayout.addWidget(self.label, 2, 0, 1, 1)
@@ -46,48 +48,56 @@
         self.label_4 = QtWidgets.QLabel(LoopWidget)
         self.label_4.setObjectName("label_4")
         self.gridLayout.addWidget(self.label_4, 5, 0, 1, 1)
         self.lblIdx = QtWidgets.QLabel(LoopWidget)
         self.lblIdx.setAlignment(QtCore.Qt.AlignCenter)
         self.lblIdx.setObjectName("lblIdx")
         self.gridLayout.addWidget(self.lblIdx, 3, 0, 1, 1)
-        spacerItem1 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem1 = QtWidgets.QSpacerItem(
+            20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding
+        )
         self.gridLayout.addItem(spacerItem1, 0, 0, 1, 1)
         self.label_3 = QtWidgets.QLabel(LoopWidget)
         self.label_3.setObjectName("label_3")
         self.gridLayout.addWidget(self.label_3, 6, 0, 1, 1)
         self.label_5 = QtWidgets.QLabel(LoopWidget)
         self.label_5.setObjectName("label_5")
         self.gridLayout.addWidget(self.label_5, 7, 0, 1, 1)
         self.lblBeta = QtWidgets.QLabel(LoopWidget)
         self.lblBeta.setText("")
         self.lblBeta.setObjectName("lblBeta")
         self.gridLayout.addWidget(self.lblBeta, 7, 1, 1, 1)
         self.label_7 = QtWidgets.QLabel(LoopWidget)
         self.label_7.setObjectName("label_7")
         self.gridLayout.addWidget(self.label_7, 8, 0, 1, 1)
-        spacerItem2 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem2 = QtWidgets.QSpacerItem(
+            20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding
+        )
         self.gridLayout.addItem(spacerItem2, 0, 1, 1, 1)
         self.btnNext = QtWidgets.QPushButton(LoopWidget)
         self.btnNext.setObjectName("btnNext")
         self.gridLayout.addWidget(self.btnNext, 1, 1, 1, 1)
         self.lblAlpha = QtWidgets.QLabel(LoopWidget)
         self.lblAlpha.setText("")
         self.lblAlpha.setObjectName("lblAlpha")
         self.gridLayout.addWidget(self.lblAlpha, 6, 1, 1, 1)
         self.lblTot = QtWidgets.QLabel(LoopWidget)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.lblTot.sizePolicy().hasHeightForWidth())
         self.lblTot.setSizePolicy(sizePolicy)
         self.lblTot.setAlignment(QtCore.Qt.AlignCenter)
         self.lblTot.setObjectName("lblTot")
         self.gridLayout.addWidget(self.lblTot, 3, 1, 1, 1)
-        spacerItem3 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem3 = QtWidgets.QSpacerItem(
+            20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding
+        )
         self.gridLayout.addItem(spacerItem3, 4, 1, 1, 1)
         self.verticalLayout_2.addLayout(self.gridLayout)
         self.comboSeries = QtWidgets.QComboBox(LoopWidget)
         self.comboSeries.setObjectName("comboSeries")
         self.verticalLayout_2.addWidget(self.comboSeries)
         self.btnDelete = QtWidgets.QPushButton(LoopWidget)
         self.btnDelete.setObjectName("btnDelete")
@@ -107,8 +117,10 @@
         self.lblIdx.setText(_translate("LoopWidget", "0"))
         self.label_3.setText(_translate("LoopWidget", "α"))
         self.label_5.setText(_translate("LoopWidget", "β"))
         self.label_7.setText(_translate("LoopWidget", "GALA"))
         self.btnNext.setText(_translate("LoopWidget", ">"))
         self.lblTot.setText(_translate("LoopWidget", "0"))
         self.btnDelete.setText(_translate("LoopWidget", "Delete current Loop"))
+
+
 from pyqtgraph import PlotWidget
```

### Comparing `graphysio-2022.9.13/graphysio/ui/loopwidget.ui` & `graphysio-2024.5.7/graphysio/ui/loopwidget.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2022.9.13/graphysio/ui/mainwindow.py` & `graphysio-2024.5.7/graphysio/ui/mainwindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,22 @@
         self.horizontalLayout = QtWidgets.QHBoxLayout()
         self.horizontalLayout.setObjectName("horizontalLayout")
         self.lblStatus = QtWidgets.QLabel(self.centralwidget)
         self.lblStatus.setMinimumSize(QtCore.QSize(150, 0))
         self.lblStatus.setText("")
         self.lblStatus.setObjectName("lblStatus")
         self.horizontalLayout.addWidget(self.lblStatus)
-        spacerItem = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        spacerItem = QtWidgets.QSpacerItem(
+            40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum
+        )
         self.horizontalLayout.addItem(spacerItem)
         self.lblCoords = QtWidgets.QLabel(self.centralwidget)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.lblCoords.sizePolicy().hasHeightForWidth())
         self.lblCoords.setSizePolicy(sizePolicy)
         self.lblCoords.setMinimumSize(QtCore.QSize(150, 0))
         self.lblCoords.setText("")
         self.lblCoords.setObjectName("lblCoords")
```

### Comparing `graphysio-2022.9.13/graphysio/ui/mainwindow.ui` & `graphysio-2024.5.7/graphysio/ui/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2022.9.13/graphysio/ui/periodexport.py` & `graphysio-2024.5.7/graphysio/ui/periodexport.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,47 +29,59 @@
         self.formLayout_3.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.txtFile)
         self.verticalLayout.addWidget(self.groupBox)
         self.groupBox_2 = QtWidgets.QGroupBox(PeriodExport)
         self.groupBox_2.setObjectName("groupBox_2")
         self.horizontalLayout_2 = QtWidgets.QHBoxLayout(self.groupBox_2)
         self.horizontalLayout_2.setObjectName("horizontalLayout_2")
         self.lblPeriodStart = QtWidgets.QLabel(self.groupBox_2)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.lblPeriodStart.sizePolicy().hasHeightForWidth())
+        sizePolicy.setHeightForWidth(
+            self.lblPeriodStart.sizePolicy().hasHeightForWidth()
+        )
         self.lblPeriodStart.setSizePolicy(sizePolicy)
         self.lblPeriodStart.setAlignment(QtCore.Qt.AlignCenter)
         self.lblPeriodStart.setObjectName("lblPeriodStart")
         self.horizontalLayout_2.addWidget(self.lblPeriodStart)
         self.label_3 = QtWidgets.QLabel(self.groupBox_2)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Preferred
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_3.sizePolicy().hasHeightForWidth())
         self.label_3.setSizePolicy(sizePolicy)
         self.label_3.setObjectName("label_3")
         self.horizontalLayout_2.addWidget(self.label_3)
         self.lblPeriodStop = QtWidgets.QLabel(self.groupBox_2)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.lblPeriodStop.sizePolicy().hasHeightForWidth())
+        sizePolicy.setHeightForWidth(
+            self.lblPeriodStop.sizePolicy().hasHeightForWidth()
+        )
         self.lblPeriodStop.setSizePolicy(sizePolicy)
         self.lblPeriodStop.setAlignment(QtCore.Qt.AlignCenter)
         self.lblPeriodStop.setObjectName("lblPeriodStop")
         self.horizontalLayout_2.addWidget(self.lblPeriodStop)
         self.verticalLayout.addWidget(self.groupBox_2)
         self.formLayout = QtWidgets.QFormLayout()
         self.formLayout.setObjectName("formLayout")
         self.label = QtWidgets.QLabel(PeriodExport)
         self.label.setObjectName("label")
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label)
         self.txtPatient = QtWidgets.QLineEdit(PeriodExport)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed
+        )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.txtPatient.sizePolicy().hasHeightForWidth())
         self.txtPatient.setSizePolicy(sizePolicy)
         self.txtPatient.setObjectName("txtPatient")
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.txtPatient)
         self.label_7 = QtWidgets.QLabel(PeriodExport)
@@ -103,15 +115,17 @@
         self.verticalLayout.addLayout(self.horizontalLayout_3)
 
         self.retranslateUi(PeriodExport)
         QtCore.QMetaObject.connectSlotsByName(PeriodExport)
 
     def retranslateUi(self, PeriodExport):
         _translate = QtCore.QCoreApplication.translate
-        PeriodExport.setWindowTitle(_translate("PeriodExport", "Export period information"))
+        PeriodExport.setWindowTitle(
+            _translate("PeriodExport", "Export period information")
+        )
         self.groupBox.setTitle(_translate("PeriodExport", "Destination file"))
         self.btnBrowse.setText(_translate("PeriodExport", "Browse"))
         self.groupBox_2.setTitle(_translate("PeriodExport", "Period"))
         self.lblPeriodStart.setText(_translate("PeriodExport", "Beginning"))
         self.label_3.setText(_translate("PeriodExport", "-"))
         self.lblPeriodStop.setText(_translate("PeriodExport", "End"))
         self.label.setText(_translate("PeriodExport", "Patient"))
```

### Comparing `graphysio-2022.9.13/graphysio/ui/periodexport.ui` & `graphysio-2024.5.7/graphysio/ui/periodexport.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2022.9.13/graphysio/ui/poiwidget.py` & `graphysio-2024.5.7/graphysio/ui/poiwidget.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     def setupUi(self, POISelectorWidget):
         POISelectorWidget.setObjectName("POISelectorWidget")
         POISelectorWidget.resize(763, 601)
         self.horizontalLayout = QtWidgets.QHBoxLayout(POISelectorWidget)
         self.horizontalLayout.setObjectName("horizontalLayout")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout()
         self.verticalLayout_2.setObjectName("verticalLayout_2")
-        spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem = QtWidgets.QSpacerItem(
+            20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding
+        )
         self.verticalLayout_2.addItem(spacerItem)
         self.groupBox = QtWidgets.QGroupBox(POISelectorWidget)
         self.groupBox.setCheckable(False)
         self.groupBox.setObjectName("groupBox")
         self.verticalLayout = QtWidgets.QVBoxLayout(self.groupBox)
         self.verticalLayout.setObjectName("verticalLayout")
         self.radioFixDisabled = QtWidgets.QRadioButton(self.groupBox)
@@ -42,22 +44,26 @@
         self.buttonGroup.addButton(self.radioFixMaximum)
         self.verticalLayout.addWidget(self.radioFixMaximum)
         self.radioFixSecondDerivative = QtWidgets.QRadioButton(self.groupBox)
         self.radioFixSecondDerivative.setObjectName("radioFixSecondDerivative")
         self.buttonGroup.addButton(self.radioFixSecondDerivative)
         self.verticalLayout.addWidget(self.radioFixSecondDerivative)
         self.verticalLayout_2.addWidget(self.groupBox)
-        spacerItem1 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem1 = QtWidgets.QSpacerItem(
+            20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding
+        )
         self.verticalLayout_2.addItem(spacerItem1)
         self.horizontalLayout.addLayout(self.verticalLayout_2)
 
         self.retranslateUi(POISelectorWidget)
         QtCore.QMetaObject.connectSlotsByName(POISelectorWidget)
 
     def retranslateUi(self, POISelectorWidget):
         _translate = QtCore.QCoreApplication.translate
         POISelectorWidget.setWindowTitle(_translate("POISelectorWidget", "Form"))
         self.groupBox.setTitle(_translate("POISelectorWidget", "Fix Position"))
         self.radioFixDisabled.setText(_translate("POISelectorWidget", "Disabled"))
         self.radioFixMinimum.setText(_translate("POISelectorWidget", "Local Minimum"))
         self.radioFixMaximum.setText(_translate("POISelectorWidget", "Local Maximum"))
-        self.radioFixSecondDerivative.setText(_translate("POISelectorWidget", "2nd derivative peak"))
+        self.radioFixSecondDerivative.setText(
+            _translate("POISelectorWidget", "2nd derivative peak")
+        )
```

### Comparing `graphysio-2022.9.13/graphysio/ui/poiwidget.ui` & `graphysio-2024.5.7/graphysio/ui/poiwidget.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2022.9.13/graphysio/ui/setuppuloop.py` & `graphysio-2024.5.7/graphysio/ui/setuppuloop.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     def setupUi(self, SetupPULoop):
         SetupPULoop.setObjectName("SetupPULoop")
         SetupPULoop.resize(387, 371)
         self.verticalLayout = QtWidgets.QVBoxLayout(SetupPULoop)
         self.verticalLayout.setObjectName("verticalLayout")
         self.formLayout_2 = QtWidgets.QFormLayout()
         self.formLayout_2.setSizeConstraint(QtWidgets.QLayout.SetMaximumSize)
-        self.formLayout_2.setFieldGrowthPolicy(QtWidgets.QFormLayout.AllNonFixedFieldsGrow)
+        self.formLayout_2.setFieldGrowthPolicy(
+            QtWidgets.QFormLayout.AllNonFixedFieldsGrow
+        )
         self.formLayout_2.setObjectName("formLayout_2")
         self.label = QtWidgets.QLabel(SetupPULoop)
         self.label.setObjectName("label")
         self.formLayout_2.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label)
         self.comboU = QtWidgets.QComboBox(SetupPULoop)
         self.comboU.setObjectName("comboU")
         self.formLayout_2.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.comboU)
```

### Comparing `graphysio-2022.9.13/graphysio/ui/setuppuloop.ui` & `graphysio-2024.5.7/graphysio/ui/setuppuloop.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2022.9.13/graphysio/utils.py` & `graphysio-2024.5.7/graphysio/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import os
 import sys
 from functools import partial
 from itertools import cycle
 
 import numpy as np
 import pathvalidate
-from pyqtgraph.Qt import QtGui
+from pyqtgraph.Qt import QtGui, QtWidgets
 
-sanitize_filename = partial(pathvalidate.sanitize_filename, platform='auto')
-sanitize_filepath = partial(pathvalidate.sanitize_filepath, platform='auto')
+sanitize_filename = partial(pathvalidate.sanitize_filename, platform="auto")
+sanitize_filepath = partial(pathvalidate.sanitize_filepath, platform="auto")
 
 
 def Colors():
     qtcolors = [
         QtGui.QColor(0, 114, 189),
         QtGui.QColor(217, 83, 25),
         QtGui.QColor(237, 177, 32),
@@ -33,33 +33,33 @@
         fs = 0
     if fs > 1:
         fs = int(round(fs))
     return fs
 
 
 def loadmodule():
-    defaultdir = os.path.expanduser('~')
-    filepath = QtGui.QFileDialog.getOpenFileName(
+    defaultdir = os.path.expanduser("~")
+    filepath = QtWidgets.QFileDialog.getOpenFileName(
         caption="Import module", filter="Python files (*.py)", directory=defaultdir
     )
-    if type(filepath) is not str:
+    if not isinstance(filepath, str):
         # PyQt5 API change
         filepath = filepath[0]
     if not filepath:
         # Cancel pressed
         return
 
     folder, filename = os.path.split(filepath)
     modulename, _ = os.path.splitext(filename)
     f, filename, description = imp.find_module(modulename, [folder])
 
     bcbak = sys.dont_write_bytecode
     try:
         sys.dont_write_bytecode = True
-        imp.load_module('graphysio.plugin', f, filename, description)
+        imp.load_module("graphysio.plugin", f, filename, description)
     finally:
         sys.dont_write_bytecode = bcbak
         f.close()
 
 
 def clip(vec, vrange):
     if vrange is None:
@@ -78,13 +78,13 @@
 def getshell(ui=None):
     import IPython
 
     IPython.embed(ui=ui)
 
 
 def displayError(errmsg):
-    msgbox = QtGui.QMessageBox()
+    msgbox = QtWidgets.QMessageBox()
     msgbox.setWindowTitle("Error")
     msgbox.setText(str(errmsg))
-    msgbox.setStandardButtons(QtGui.QMessageBox.Ok)
-    msgbox.setIcon(QtGui.QMessageBox.Critical)
+    msgbox.setStandardButtons(QtWidgets.QMessageBox.Ok)
+    msgbox.setIcon(QtWidgets.QMessageBox.Critical)
     msgbox.exec_()
```

### Comparing `graphysio-2022.9.13/graphysio/writedata/edf.py` & `graphysio-2024.5.7/graphysio/writedata/edf.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,52 +13,52 @@
     is_available = False
 else:
     is_available = True
 
 
 def interp_series(s, samplerate, start, stop):
     f = interpolate.interp1d(
-        s.index, s.values, assume_sorted=True, copy=False, fill_value='extrapolate'
+        s.index, s.values, assume_sorted=True, copy=False, fill_value="extrapolate"
     )
     # Account for periods of missing data.
     duration_s = (stop - start) * 1e-9
     npoints = int(duration_s * samplerate)
     newidx = np.linspace(start, stop, num=npoints)
     return f(newidx)
 
 
 def curves_to_edf(
-    curves: List[CurveItem], filepath: str, index_label: str = 'timens'
+    curves: List[CurveItem], filepath: str, index_label: str = "timens"
 ) -> None:
     headers = []
     signals = []
 
     beginns = min(c.series.index[0] for c in curves)
     endns = max(c.series.index[-1] for c in curves)
     begindt = datetime.fromtimestamp(beginns * 1e-9)
 
     # Use global min / max of values since some viewers need this (edfbrowser)
     physmax = max(c.series.max() for c in curves)
     physmin = min(c.series.min() for c in curves)
 
     # Ask the user for the physical dimension shared by all curves
-    dim = askUserValue(Parameter('Enter physical dimension', str))
+    dim = askUserValue(Parameter("Enter physical dimension", str))
 
     for c in curves:
         s = c.series
         header = {
-            'label': c.name(),
-            'sample_rate': c.samplerate,
-            'physical_max': physmax,
-            'physical_min': physmin,
-            'digital_max': 32767,
-            'digital_min': -32768,
-            'transducer': '',
-            'prefilter': '',
-            'dimension': dim,
+            "label": c.name(),
+            "sample_rate": c.samplerate,
+            "physical_max": physmax,
+            "physical_min": physmin,
+            "digital_max": 32767,
+            "digital_min": -32768,
+            "transducer": "",
+            "prefilter": "",
+            "dimension": dim,
         }
         headers.append(header)
         resampled = interp_series(s, c.samplerate, beginns, endns)
         signals.append(resampled)
 
     edf = pyedflib.EdfWriter(
         str(filepath), len(signals), file_type=pyedflib.FILETYPE_EDFPLUS
```

### Comparing `graphysio-2022.9.13/graphysio/writedata/exporter.py` & `graphysio-2024.5.7/graphysio/writedata/exporter.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 
 import pandas as pd
 
 from graphysio import writedata
 from graphysio.dialogs import DlgPeriodExport, askDirPath, askSaveFilePath
 from graphysio.utils import sanitize_filename
 
-file_filters = ';;'.join(
-    [f'{ext.upper()} files (*.{ext})' for ext in writedata.curve_writers]
+file_filters = ";;".join(
+    [f"{ext.upper()} files (*.{ext})" for ext in writedata.curve_writers]
 )
 
 
 class TsExporter:
-    periodfields = ['patient', 'begin', 'end', 'periodid', 'comment']
+    periodfields = ["patient", "begin", "end", "periodid", "comment"]
 
     def __init__(self, parent, name):
         self.parent = parent
         self.name = name
         try:
-            self.outdir = parent.properties['dircache']
+            self.outdir = parent.properties["dircache"]
         except KeyError:
-            self.outdir = os.path.expanduser('~')
+            self.outdir = os.path.expanduser("~")
 
     def curves(self) -> None:
         filepath, ext = askSaveFilePath(
-            'Export to', f'{self.name}.csv', self.outdir, filter=file_filters
+            "Export to", f"{self.name}.csv", self.outdir, filter=file_filters
         )
         if filepath is None:
             return
         self.outdir = os.path.dirname(filepath)
         curves = list(self.parent.curves.values())
         export_func = writedata.curve_writers[ext]
         export_func(curves, filepath)
@@ -42,27 +42,27 @@
         )
 
         def cb(result):
             patient, comment, periodname, filepath = result
             self.name = patient
             self.outdir = os.path.dirname(filepath)
 
-            with open(filepath, 'a', newline='') as csvfile:
+            with open(filepath, "a", newline="") as csvfile:
                 writer = csv.DictWriter(
                     csvfile, fieldnames=self.periodfields, quoting=csv.QUOTE_MINIMAL
                 )
                 if not os.path.exists(filepath):
                     writer.writeheader()
                 writer.writerow(
                     {
-                        'patient': patient,
-                        'begin': xmin,
-                        'end': xmax,
-                        'periodid': periodname,
-                        'comment': comment,
+                        "patient": patient,
+                        "begin": xmin,
+                        "end": xmax,
+                        "periodid": periodname,
+                        "comment": comment,
                     }
                 )
 
         dlg.dlgdata.connect(cb)
         dlg.exec_()
 
     def cycles(self) -> None:
@@ -89,95 +89,95 @@
                 if s is None or len(s) < 1:
                     continue
                 if idxstart is None:
                     idxstart = s.index[0]
                 idxdelta = s.index[0] - idxstart
                 s.index -= idxdelta
             df = pd.concat(cycle, axis=1)
-            df['datetime'] = pd.to_datetime(df.index, unit='ns')
+            df["datetime"] = pd.to_datetime(df.index, unit="ns")
 
-            filename = sanitize_filename(f'{self.name}-{n+1}.csv')
+            filename = sanitize_filename(f"{self.name}-{n+1}.csv")
             filepath = os.path.join(self.outdir, filename)
             df.to_csv(
-                filepath, date_format="%Y-%m-%d %H:%M:%S.%f", index_label='timens'
+                filepath, date_format="%Y-%m-%d %H:%M:%S.%f", index_label="timens"
             )
 
     def cyclepoints(self) -> None:
-        filepath, _ = askSaveFilePath('Export to', f'{self.name}-feet.csv', self.outdir)
+        filepath, _ = askSaveFilePath("Export to", f"{self.name}-feet.csv", self.outdir)
         if filepath is None:
             # Cancel pressed
             return
         self.outdir = os.path.dirname(filepath)
 
         feetseries = []
         for c in self.parent.curves.values():
             for k, v in c.feetitem.indices.items():
-                feetseries.append(pd.Series(v, name=f'{c.name()}-{k}'))
+                feetseries.append(pd.Series(v, name=f"{c.name()}-{k}"))
         df = pd.concat(feetseries, axis=1)
-        df.to_csv(filepath, index_label='idx')
+        df.to_csv(filepath, index_label="idx")
 
 
 class PuExporter:
     def __init__(self, parent, name):
         self.parent = parent
         self.name = name
         try:
-            self.outdir = parent.properties['dircache']
+            self.outdir = parent.properties["dircache"]
         except KeyError:
-            self.outdir = os.path.expanduser('~')
+            self.outdir = os.path.expanduser("~")
 
     def exportloops(self):
-        outdir = askDirPath('Export to', self.outdir)
+        outdir = askDirPath("Export to", self.outdir)
         if outdir is None:
             # Cancel pressed
             return
         self.outdir = outdir
         self.writetable()
         self.writeloops()
 
     def writetable(self):
         data = []
         for loop in self.parent.loops:
             alpha, beta, gala = loop.angles
             delay = loop.offset / 1e6
-            tmpdict = {'alpha': alpha, 'beta': beta, 'gala': gala, 'delay': delay}
+            tmpdict = {"alpha": alpha, "beta": beta, "gala": gala, "delay": delay}
             data.append(tmpdict)
         df = pd.DataFrame(data)
         df.index += 1
-        filename = sanitize_filename(f'{self.name}-loopdata.csv')
+        filename = sanitize_filename(f"{self.name}-loopdata.csv")
         filepath = os.path.join(self.outdir, filename)
-        df.to_csv(filepath, index_label='idx')
+        df.to_csv(filepath, index_label="idx")
 
     def writeloops(self):
         for n, loop in enumerate(self.parent.loops):
             df = loop.df
-            filename = sanitize_filename(f'{self.name}-{n+1}.csv')
+            filename = sanitize_filename(f"{self.name}-{n+1}.csv")
             filepath = os.path.join(self.outdir, filename)
-            df['datetime'] = pd.to_datetime(df.index, unit='ns')
+            df["datetime"] = pd.to_datetime(df.index, unit="ns")
             df.to_csv(
-                filepath, date_format="%Y-%m-%d %H:%M:%S.%f", index_label='timens'
+                filepath, date_format="%Y-%m-%d %H:%M:%S.%f", index_label="timens"
             )
 
 
 class POIExporter:
     def __init__(self, parent, name):
         self.parent = parent
         self.name = name
         try:
-            self.outdir = parent.properties['dircache']
+            self.outdir = parent.properties["dircache"]
         except KeyError:
-            self.outdir = os.path.expanduser('~')
+            self.outdir = os.path.expanduser("~")
 
     def poi(self):
-        filepath, _ = askSaveFilePath('Export to', f'{self.name}-poi.csv', self.outdir)
+        filepath, _ = askSaveFilePath("Export to", f"{self.name}-poi.csv", self.outdir)
         if filepath is None:
             # Cancel pressed
             return
         self.outdir = os.path.dirname(filepath)
 
         srcseries = self.parent.curve.series
         poiidx = self.parent.curve.feetitem.indices[self.parent.pointkey]
-        pois = srcseries[poiidx.dropna()].rename('poi')
+        pois = srcseries[poiidx.dropna()].rename("poi")
         sers = [srcseries, pois]
         df = pd.concat(sers, axis=1, keys=[s.name for s in sers])
-        df['datetime'] = pd.to_datetime(df.index, unit='ns')
-        df.to_csv(filepath, date_format="%Y-%m-%d %H:%M:%S.%f", index_label='timens')
+        df["datetime"] = pd.to_datetime(df.index, unit="ns")
+        df.to_csv(filepath, date_format="%Y-%m-%d %H:%M:%S.%f", index_label="timens")
```

### Comparing `graphysio-2022.9.13/graphysio/writedata/parquet.py` & `graphysio-2024.5.7/graphysio/writedata/parquet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import List
 
 import pandas as pd
 from graphysio.plotwidgets.curves import CurveItem
 
 try:
-    import pyarrow.parquet
+    import pyarrow.parquet  # noqa: F401
 except ImportError:
     is_available = False
 else:
     is_available = True
 
 
 def export_curves(
-    curves: List[CurveItem], filepath: str, index_label: str = 'timens'
+    curves: List[CurveItem], filepath: str, index_label: str = "timens"
 ) -> None:
     sers = [c.series for c in curves]
     data = pd.concat(sers, axis=1).sort_index()
     data.to_parquet(
         filepath,
-        engine='pyarrow',
-        compression='gzip',
-        coerce_timestamps='us',
+        engine="pyarrow",
+        compression="gzip",
+        coerce_timestamps="us",
         allow_truncated_timestamps=True,
     )
 
 
 export_curves.is_available = is_available
```

### Comparing `graphysio-2022.9.13/pyproject.toml` & `graphysio-2024.5.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "graphysio"
-version = "2022.9.13"
+version = "2024.5.7"
 description = "Visualizer and analyser for biometric signals"
 authors = ["Jona Joachim <jona@joachim.cc>"]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/jaj42/GraPhysio"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-pandas = "^1.4.3"
-pathvalidate = "^2.5.0"
-Pint = "^0.19.2"
-pyqtgraph = "^0.12.4"
-scipy = "^1.8.1"
-numexpr = "2.8.3"
-pyarrow = {version = "^8.0.0", optional = true}
-pyEDFlib = {version = "^0.1.29", optional = true}
-physiocurve = "^2022.7.14"
+python = ">=3.9,<3.13"
+pandas = "^2"
+pathvalidate = "^3"
+Pint = "^0.23"
+pyqtgraph = "^0.13"
+scipy = "^1.13"
+numexpr = "^2.9"
+physiocurve = "^2024"
+pyshortcuts = "^1.9.0"
+pyarrow = {version = ">=14", optional = true}
+pyEDFlib = {version = "^0.1.37", optional = true}
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 flake8 = "^4.0.1"
 flake8-bandit = "^3.0.0"
-safety = "^1.10.3"
 flake8-bugbear = "^22.4.25"
 vulture = "^2.5"
 vermin = "^1.4.0"
+safety = "^2"
 
 [tool.poetry.scripts]
 graphysio = "graphysio.main:main"
 
-[tool.black]
-line-length = 88
+[tool.ruff.lint]
+select = ["ALL"]
 extend-exclude = 'ui'
-target-version = ['py38', 'py39', 'py310']
-skip-string-normalization = true
-
+line-length = 88
```

### Comparing `graphysio-2022.9.13/PKG-INFO` & `graphysio-2024.5.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: graphysio
-Version: 2022.9.13
+Version: 2024.5.7
 Summary: Visualizer and analyser for biometric signals
 Home-page: https://github.com/jaj42/GraPhysio
 License: ISC
 Author: Jona Joachim
 Author-email: jona@joachim.cc
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Pint (>=0.19.2,<0.20.0)
-Requires-Dist: numexpr (==2.8.3)
-Requires-Dist: pandas (>=1.4.3,<2.0.0)
-Requires-Dist: pathvalidate (>=2.5.0,<3.0.0)
-Requires-Dist: physiocurve (>=2022.7.14,<2023.0.0)
-Requires-Dist: pyEDFlib (>=0.1.29,<0.2.0)
-Requires-Dist: pyarrow (>=8.0.0,<9.0.0)
-Requires-Dist: pyqtgraph (>=0.12.4,<0.13.0)
-Requires-Dist: scipy (>=1.8.1,<2.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Pint (>=0.23,<0.24)
+Requires-Dist: numexpr (>=2.9,<3.0)
+Requires-Dist: pandas (>=2,<3)
+Requires-Dist: pathvalidate (>=3,<4)
+Requires-Dist: physiocurve (>=2024,<2025)
+Requires-Dist: pyEDFlib (>=0.1.37,<0.2.0)
+Requires-Dist: pyarrow (>=14)
+Requires-Dist: pyqtgraph (>=0.13,<0.14)
+Requires-Dist: pyshortcuts (>=1.9.0,<2.0.0)
+Requires-Dist: scipy (>=1.13,<2.0)
 Project-URL: Repository, https://github.com/jaj42/GraPhysio
 Description-Content-Type: text/markdown
 
 # GraPhysio
 GraPhysio is a graphical time series visualizer created for biometric data
 signals from ICU patient monitors. It is however not limited to this. It can
 handle low frequency and high frequency data as well as aggregating and
```

