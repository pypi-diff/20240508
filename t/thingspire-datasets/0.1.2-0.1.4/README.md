# Comparing `tmp/thingspire-datasets-0.1.2.tar.gz` & `tmp/thingspire-datasets-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingspire-datasets-0.1.2.tar", last modified: Tue May  7 05:59:41 2024, max compression
+gzip compressed data, was "thingspire-datasets-0.1.4.tar", last modified: Wed May  8 05:54:57 2024, max compression
```

## Comparing `thingspire-datasets-0.1.2.tar` & `thingspire-datasets-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 05:59:41.169576 thingspire-datasets-0.1.2/
--rw-rw-rw-   0        0        0      594 2024-05-07 05:59:41.169576 thingspire-datasets-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-07 05:59:41.171619 thingspire-datasets-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      821 2024-05-07 05:59:09.000000 thingspire-datasets-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 05:59:41.154020 thingspire-datasets-0.1.2/thingspire_datasets.egg-info/
--rw-rw-rw-   0        0        0      594 2024-05-07 05:59:41.000000 thingspire-datasets-0.1.2/thingspire_datasets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2024-05-07 05:59:41.000000 thingspire-datasets-0.1.2/thingspire_datasets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 05:59:41.000000 thingspire-datasets-0.1.2/thingspire_datasets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-07 05:59:41.000000 thingspire-datasets-0.1.2/thingspire_datasets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-07 05:59:41.000000 thingspire-datasets-0.1.2/thingspire_datasets.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 05:59:41.166576 thingspire-datasets-0.1.2/ts_feature/
--rw-rw-rw-   0        0        0      133 2024-05-07 05:13:41.000000 thingspire-datasets-0.1.2/ts_feature/__init__.py
--rw-rw-rw-   0        0        0     4472 2024-05-03 02:26:58.000000 thingspire-datasets-0.1.2/ts_feature/get_calendar.py
--rw-rw-rw-   0        0        0     7430 2024-05-07 05:58:35.000000 thingspire-datasets-0.1.2/ts_feature/get_weather.py
--rw-rw-rw-   0        0        0     1879 2024-05-02 01:55:42.000000 thingspire-datasets-0.1.2/ts_feature/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:54:57.313547 thingspire-datasets-0.1.4/
+-rw-rw-rw-   0        0        0      594 2024-05-08 05:54:57.313547 thingspire-datasets-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-08 05:54:57.314550 thingspire-datasets-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      821 2024-05-08 05:54:51.000000 thingspire-datasets-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:54:57.285359 thingspire-datasets-0.1.4/thingspire/
+-rw-rw-rw-   0        0        0      149 2024-05-08 05:46:46.000000 thingspire-datasets-0.1.4/thingspire/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:54:57.298976 thingspire-datasets-0.1.4/thingspire/dataset/
+-rw-rw-rw-   0        0        0      133 2024-05-08 05:46:46.000000 thingspire-datasets-0.1.4/thingspire/dataset/__init__.py
+-rw-rw-rw-   0        0        0     5190 2024-05-07 08:50:18.000000 thingspire-datasets-0.1.4/thingspire/dataset/get_calendar.py
+-rw-rw-rw-   0        0        0     7520 2024-05-07 06:40:21.000000 thingspire-datasets-0.1.4/thingspire/dataset/get_weather.py
+-rw-rw-rw-   0        0        0    15557 2024-05-02 01:56:43.000000 thingspire-datasets-0.1.4/thingspire/dataset/resource-id-name.py
+-rw-rw-rw-   0        0        0     1879 2024-05-02 01:55:42.000000 thingspire-datasets-0.1.4/thingspire/dataset/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:54:57.310541 thingspire-datasets-0.1.4/thingspire_datasets.egg-info/
+-rw-rw-rw-   0        0        0      594 2024-05-08 05:54:57.000000 thingspire-datasets-0.1.4/thingspire_datasets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2024-05-08 05:54:57.000000 thingspire-datasets-0.1.4/thingspire_datasets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 05:54:57.000000 thingspire-datasets-0.1.4/thingspire_datasets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-08 05:54:57.000000 thingspire-datasets-0.1.4/thingspire_datasets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 05:54:57.000000 thingspire-datasets-0.1.4/thingspire_datasets.egg-info/top_level.txt
```

### Comparing `thingspire-datasets-0.1.2/PKG-INFO` & `thingspire-datasets-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thingspire-datasets
-Version: 0.1.2
+Version: 0.1.4
 Summary: thingspire feature package
 Home-page: UNKNOWN
 Author: Inho Kim
 Author-email: inho@thingspire.com
 License: UNKNOWN
-Keywords: thingspire,ts_feature
+Keywords: thingspire,thingspire
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `thingspire-datasets-0.1.2/setup.py` & `thingspire-datasets-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 setuptools.setup(
     name="thingspire-datasets",
-    version="0.1.2",
+    version="0.1.4",
     author="Inho Kim",
     author_email="inho@thingspire.com",
     description="thingspire feature package",
     long_description="A package that collects and processes weather and "
                      "special day information by local government and "
                      "applies it to various projects",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=['Bottleneck', 'numpy', 'pandas', 'requests'],
-    keywords=['thingspire', 'ts_feature'],
+    keywords=['thingspire', 'thingspire'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6'
 )
```

### Comparing `thingspire-datasets-0.1.2/thingspire_datasets.egg-info/PKG-INFO` & `thingspire-datasets-0.1.4/thingspire_datasets.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thingspire-datasets
-Version: 0.1.2
+Version: 0.1.4
 Summary: thingspire feature package
 Home-page: UNKNOWN
 Author: Inho Kim
 Author-email: inho@thingspire.com
 License: UNKNOWN
-Keywords: thingspire,ts_feature
+Keywords: thingspire,thingspire
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `thingspire-datasets-0.1.2/ts_feature/get_calendar.py` & `thingspire-datasets-0.1.4/thingspire/dataset/get_calendar.py`

 * *Files 16% similar despite different names*

```diff
@@ -112,8 +112,22 @@
     calendar_df = date_merge(calendar_pd, holiday_pd)
     calendar_df = weekend_collect(calendar_df)
     calendar_df = between_collect(calendar_df)
     calendar_df = date_merge(calendar_df, vacation_pd)
     calendar_df = calendar_df[(calendar_df['date'] >= pd.to_datetime(start)) & (calendar_df['date'] <= pd.to_datetime(end))]
     calendar_df['vacation'] = calendar_df['vacation'].fillna(0)
 
-    return calendar_df
+    calendar_df = calendar_df.astype({"holiday": int,
+                                      "day_of_week": int,
+                                      "prev_day": int,
+                                      "next_day": int})
+    calendar_df['year'] = calendar_df['date'].dt.year
+    calendar_df['month'] = calendar_df['date'].dt.month
+    calendar_df['day'] = calendar_df['date'].dt.day
+    calendar_df['date'] = calendar_df['date'].dt.strftime('%Y-%m-%d')
+
+    return calendar_df
+
+
+calendar_data = select_calender(calender_key= 'VIWgm1LPd%2FwyqU9Ui7ANmaTjE58HGicrTNSSY8ZMNxhbpzEyRIVzd6OvDDnh63UUNKdcJkyaRlVx5SjWeFi%2FSA%3D%3D',
+                                start= "20240501",
+                                end= "20240520")
```

### Comparing `thingspire-datasets-0.1.2/ts_feature/get_weather.py` & `thingspire-datasets-0.1.4/thingspire/dataset/get_weather.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from datetime import datetime, timedelta
 import json
 import time
 import pandas as pd
 import requests
 from io import StringIO
 import numpy as np
+import os
 
 from .utils import flomon_url, api_payload, region_name
 
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 
 current_dir = os.path.dirname(__file__)
-json_path = os.path.join(current_dir, 'resource-id-name.json')
+json_path = os.path.join(current_dir, 'resource-id-name.py')
 
 
 def find_sido(input_name, region_dict):
     for key, names in region_dict.items():
         if input_name in names:
             return key
     return "해당 지역을 찾을 수 없습니다."
@@ -134,14 +135,17 @@
 
     df = df[['region', 'datetime', 'time',
              'sunrise', 'sunset', 'temp', 'sensibleTemp',
              'humidity', 'pressure', 'clouds', 'visibility',
              'precipitationIntensity', 'snowfall', 'windGust',
              'windDirection', 'windSpeed', 'weatherCode']]
 
+    df['datetime'] = df['datetime'].dt.tz_localize(None)
+    df = df.fillna(0)
+
     return df
 
 
 def adjust_column_names(cols):
     new_cols = []
     for col in cols:
         if isinstance(col, tuple):
@@ -210,8 +214,8 @@
     processed_data = round_time_and_aggregate(response.json())
     named_data = ids_to_names(processed_data, id_names)
     output = js_to_dataframe(named_data, start, end)
 
     if period == "daily":
         output = hourly_to_daily(output)
 
-    return output
+    return output
```

### Comparing `thingspire-datasets-0.1.2/ts_feature/utils.py` & `thingspire-datasets-0.1.4/thingspire/dataset/utils.py`

 * *Files identical despite different names*

