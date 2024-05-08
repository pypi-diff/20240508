# Comparing `tmp/stepcount-3.7.1.tar.gz` & `tmp/stepcount-3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepcount-3.7.1.tar", last modified: Sat May  4 06:55:13 2024, max compression
+gzip compressed data, was "stepcount-3.7.2.tar", last modified: Wed May  8 17:19:35 2024, max compression
```

## Comparing `stepcount-3.7.1.tar` & `stepcount-3.7.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:55:13.390142 stepcount-3.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-04 06:55:05.000000 stepcount-3.7.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-04 06:55:13.382142 stepcount-3.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-04 06:55:05.000000 stepcount-3.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-04 06:55:05.000000 stepcount-3.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 06:55:13.390142 stepcount-3.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-04 06:55:05.000000 stepcount-3.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:55:13.378142 stepcount-3.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:55:13.390142 stepcount-3.7.1/src/stepcount/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-04 06:55:05.000000 stepcount-3.7.1/src/stepcount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-04 06:55:13.390142 stepcount-3.7.1/src/stepcount/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-04 06:55:05.000000 stepcount-3.7.1/src/stepcount/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-05-04 06:55:05.000000 stepcount-3.7.1/src/stepcount/hmm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23839 2024-05-04 06:55:05.000000 stepcount-3.7.1/src/stepcount/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-05-04 06:55:05.000000 stepcount-3.7.1/src/stepcount/sslmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    30189 2024-05-04 06:55:05.000000 stepcount-3.7.1/src/stepcount/stepcount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:55:13.382142 stepcount-3.7.1/src/stepcount/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-04 06:55:05.000000 stepcount-3.7.1/src/stepcount/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-04 06:55:05.000000 stepcount-3.7.1/src/stepcount/utils/collate_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-04 06:55:05.000000 stepcount-3.7.1/src/stepcount/utils/generate_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:55:13.378142 stepcount-3.7.1/src/stepcount.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-04 06:55:13.000000 stepcount-3.7.1/src/stepcount.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-04 06:55:13.000000 stepcount-3.7.1/src/stepcount.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 06:55:13.000000 stepcount-3.7.1/src/stepcount.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-04 06:55:13.000000 stepcount-3.7.1/src/stepcount.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-04 06:55:13.000000 stepcount-3.7.1/src/stepcount.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-04 06:55:13.000000 stepcount-3.7.1/src/stepcount.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-05-04 06:55:05.000000 stepcount-3.7.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:19:35.095379 stepcount-3.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-08 17:19:26.000000 stepcount-3.7.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-08 17:19:35.087379 stepcount-3.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-08 17:19:26.000000 stepcount-3.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-08 17:19:26.000000 stepcount-3.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:19:35.095379 stepcount-3.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-08 17:19:26.000000 stepcount-3.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:19:35.083379 stepcount-3.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:19:35.095379 stepcount-3.7.2/src/stepcount/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-08 17:19:26.000000 stepcount-3.7.2/src/stepcount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-08 17:19:35.095379 stepcount-3.7.2/src/stepcount/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-08 17:19:26.000000 stepcount-3.7.2/src/stepcount/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-05-08 17:19:26.000000 stepcount-3.7.2/src/stepcount/hmm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23839 2024-05-08 17:19:26.000000 stepcount-3.7.2/src/stepcount/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-05-08 17:19:26.000000 stepcount-3.7.2/src/stepcount/sslmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31341 2024-05-08 17:19:26.000000 stepcount-3.7.2/src/stepcount/stepcount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:19:35.083379 stepcount-3.7.2/src/stepcount/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 17:19:26.000000 stepcount-3.7.2/src/stepcount/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-08 17:19:26.000000 stepcount-3.7.2/src/stepcount/utils/collate_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-08 17:19:26.000000 stepcount-3.7.2/src/stepcount/utils/generate_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:19:35.083379 stepcount-3.7.2/src/stepcount.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-08 17:19:35.000000 stepcount-3.7.2/src/stepcount.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-08 17:19:35.000000 stepcount-3.7.2/src/stepcount.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:19:35.000000 stepcount-3.7.2/src/stepcount.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-08 17:19:35.000000 stepcount-3.7.2/src/stepcount.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-08 17:19:35.000000 stepcount-3.7.2/src/stepcount.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 17:19:35.000000 stepcount-3.7.2/src/stepcount.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-05-08 17:19:26.000000 stepcount-3.7.2/versioneer.py
```

### Comparing `stepcount-3.7.1/LICENSE.md` & `stepcount-3.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stepcount-3.7.1/PKG-INFO` & `stepcount-3.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 3.7.1
+Version: 3.7.2
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
```

### Comparing `stepcount-3.7.1/README.md` & `stepcount-3.7.2/README.md`

 * *Files identical despite different names*

### Comparing `stepcount-3.7.1/pyproject.toml` & `stepcount-3.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stepcount-3.7.1/setup.py` & `stepcount-3.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.7.1/src/stepcount/__init__.py` & `stepcount-3.7.2/src/stepcount/__init__.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.7.1/src/stepcount/features.py` & `stepcount-3.7.2/src/stepcount/features.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.7.1/src/stepcount/hmm_utils.py` & `stepcount-3.7.2/src/stepcount/hmm_utils.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.7.1/src/stepcount/models.py` & `stepcount-3.7.2/src/stepcount/models.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.7.1/src/stepcount/sslmodel.py` & `stepcount-3.7.2/src/stepcount/sslmodel.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.7.1/src/stepcount/stepcount.py` & `stepcount-3.7.2/src/stepcount/stepcount.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,66 +161,84 @@
         json.dump(info, f, indent=4, cls=NpEncoder)
 
     # Save hourly data
     hourly = pd.concat([
         steps_summary['hourly'],
         enmo_summary['hourly'],
     ], axis=1)
-    hourly.to_csv(f"{outdir}/{basename}-Hourly.csv.gz")
+    hourly.index.name = 'Time'
+    hourly.reset_index(inplace=True)
+    hourly.insert(0, 'Filename', info['Filename'])  # add filename for reference
+    hourly.to_csv(f"{outdir}/{basename}-Hourly.csv.gz", index=False)
     del hourly  # free memory
 
     # Save hourly data, adjusted
     hourly_adj = pd.concat([
         steps_summary_adj['hourly'],
         enmo_summary_adj['hourly'],
     ], axis=1)
-    hourly_adj.to_csv(f"{outdir}/{basename}-HourlyAdjusted.csv.gz")
+    hourly_adj.index.name = 'Time'
+    hourly_adj.reset_index(inplace=True)
+    hourly_adj.insert(0, 'Filename', info['Filename'])  # add filename for reference
+    hourly_adj.to_csv(f"{outdir}/{basename}-HourlyAdjusted.csv.gz", index=False)
     del hourly_adj  # free memory
 
     # Save minutely data
     minutely = pd.concat([
         steps_summary['minutely'],
         enmo_summary['minutely'],
     ], axis=1)
-    minutely.to_csv(f"{outdir}/{basename}-Minutely.csv.gz")
+    minutely.index.name = 'Time'
+    minutely.reset_index(inplace=True)
+    minutely.insert(0, 'Filename', info['Filename'])  # add filename for reference
+    minutely.to_csv(f"{outdir}/{basename}-Minutely.csv.gz", index=False)
     del minutely  # free memory
 
     # Save minutely data, adjusted
     minutely_adj = pd.concat([
         steps_summary_adj['minutely'],
         enmo_summary_adj['minutely'],
     ], axis=1)
-    minutely_adj.to_csv(f"{outdir}/{basename}-MinutelyAdjusted.csv.gz")
+    minutely_adj.index.name = 'Time'
+    minutely_adj.reset_index(inplace=True)
+    minutely_adj.insert(0, 'Filename', info['Filename'])  # add filename for reference
+    minutely_adj.to_csv(f"{outdir}/{basename}-MinutelyAdjusted.csv.gz", index=False)
     del minutely_adj  # free memory
 
     # Save daily data
     daily = pd.concat([
         steps_summary['daily'],
         cadence_summary['daily'],
         enmo_summary['daily'],
     ], axis=1)
-    daily.to_csv(f"{outdir}/{basename}-Daily.csv.gz")
+    daily.index.name = 'Date'
+    daily.reset_index(inplace=True)
+    daily.insert(0, 'Filename', info['Filename'])  # add filename for reference
+    daily.to_csv(f"{outdir}/{basename}-Daily.csv.gz", index=False)
     # del daily  # still needed for printing
 
     # Save daily data, adjusted
     daily_adj = pd.concat([
         steps_summary_adj['daily'],
         cadence_summary_adj['daily'],
         enmo_summary_adj['daily'],
     ], axis=1)
-    daily_adj.to_csv(f"{outdir}/{basename}-DailyAdjusted.csv.gz")
+    daily_adj.index.name = 'Date'
+    daily_adj.reset_index(inplace=True)
+    daily_adj.insert(0, 'Filename', info['Filename'])  # add filename for reference
+    daily_adj.to_csv(f"{outdir}/{basename}-DailyAdjusted.csv.gz", index=False)
     # del daily_adj  # still needed for printing
 
     # Print
     print("\nSummary\n-------")
     print(json.dumps(info, indent=4, cls=NpEncoder))
     print("\nEstimated Daily Stats\n---------------------")
-    print(daily)
+    print(daily.set_index('Date').drop(columns='Filename'))
     print("\nEstimated Daily Stats (Adjusted)\n---------------------")
-    print(daily_adj)
+    print(daily_adj.set_index('Date').drop(columns='Filename'))
     print("\nOutput files saved in:", outdir)
 
     after = time.time()
     print(f"Done! ({round(after - before,2)}s)")
 
 
 def summarize_enmo(data: pd.DataFrame, exclude_wear_below=None, exclude_first_last=None, adjust_estimates=False):
@@ -265,15 +283,15 @@
         # TODO: 7-day padding for shorter recordings
         day_of_week = impute_days(daily).groupby(daily.index.weekday).agg(_mean)
         avg = day_of_week.agg(_mean)
     else:
         # crude (unadjusted) estimates ignore NAs
         minutely = v.resample('T').agg(_mean).rename('ENMO(mg)')
         hourly = v.resample('H').agg(_mean).rename('ENMO(mg)')
-        daily = v.resample('D').agg(_mean).rename('ENMO(mg')
+        daily = v.resample('D').agg(_mean).rename('ENMO(mg)')
         avg = daily.agg(_mean)
 
     return {
         'avg': avg,
         'hourly': hourly,
         'daily': daily,
         'minutely': minutely,
@@ -497,17 +515,17 @@
     with warnings.catch_warnings():
         warnings.filterwarnings('ignore', message='Mean of empty slice')
 
         if adjust_estimates:
             # adjusted estimates first form a 7-day representative week before final aggregation
             # TODO: 7-day padding for shorter recordings
             # TODO: maybe impute output daily_cadence? but skip user-excluded days
-            day_of_week_cadence_peak1 = impute_days(daily_cadence_peak1).groupby(daily_cadence_peak1.index.weekday).median()
-            day_of_week_cadence_peak30 = impute_days(daily_cadence_peak30).groupby(daily_cadence_peak30.index.weekday).median()
-            day_of_week_cadence_p95 = impute_days(daily_cadence_p95).groupby(daily_cadence_p95.index.weekday).median()
+            day_of_week_cadence_peak1 = impute_days(daily_cadence_peak1, method='median').groupby(daily_cadence_peak1.index.weekday).median()
+            day_of_week_cadence_peak30 = impute_days(daily_cadence_peak30, method='median').groupby(daily_cadence_peak30.index.weekday).median()
+            day_of_week_cadence_p95 = impute_days(daily_cadence_p95, method='median').groupby(daily_cadence_p95.index.weekday).median()
 
             cadence_peak1 = day_of_week_cadence_peak1.median()
             cadence_peak30 = day_of_week_cadence_peak30.median()
             cadence_p95 = day_of_week_cadence_p95.median()
 
         else:
             cadence_peak1 = daily_cadence_peak1.median()
```

### Comparing `stepcount-3.7.1/src/stepcount/utils/collate_outputs.py` & `stepcount-3.7.2/src/stepcount/utils/collate_outputs.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.7.1/src/stepcount/utils/generate_commands.py` & `stepcount-3.7.2/src/stepcount/utils/generate_commands.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.7.1/src/stepcount.egg-info/PKG-INFO` & `stepcount-3.7.2/src/stepcount.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 3.7.1
+Version: 3.7.2
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
```

### Comparing `stepcount-3.7.1/src/stepcount.egg-info/SOURCES.txt` & `stepcount-3.7.2/src/stepcount.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stepcount-3.7.1/versioneer.py` & `stepcount-3.7.2/versioneer.py`

 * *Files identical despite different names*

