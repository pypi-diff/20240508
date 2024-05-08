# Comparing `tmp/ipsvm-1.1.0.tar.gz` & `tmp/ipsvm-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ipsvm-1.1.0.tar", last modified: Tue Nov  5 18:26:23 2019, max compression
+gzip compressed data, was "ipsvm-1.2.0.tar", last modified: Wed May  8 12:52:20 2024, max compression
```

## Comparing `ipsvm-1.1.0.tar` & `ipsvm-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2019-11-05 18:26:23.000000 ipsvm-1.1.0/
--rw-rw-r--   0 rof       (1001) rof       (1001)       38 2019-11-05 18:26:23.000000 ipsvm-1.1.0/setup.cfg
--rw-rw-r--   0 rof       (1001) rof       (1001)      300 2019-11-05 18:26:23.000000 ipsvm-1.1.0/PKG-INFO
--rw-rw-r--   0 rof       (1001) rof       (1001)       20 2019-11-05 18:25:56.000000 ipsvm-1.1.0/version.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      811 2019-11-05 18:25:56.000000 ipsvm-1.1.0/setup.py
--rw-rw-r--   0 rof       (1001) rof       (1001)       82 2019-11-05 18:25:56.000000 ipsvm-1.1.0/MANIFEST.in
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2019-11-05 18:26:23.000000 ipsvm-1.1.0/src/
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2019-11-05 18:26:23.000000 ipsvm-1.1.0/src/ipsvm.egg-info/
--rw-rw-r--   0 rof       (1001) rof       (1001)        6 2019-11-05 18:26:23.000000 ipsvm-1.1.0/src/ipsvm.egg-info/top_level.txt
--rw-rw-r--   0 rof       (1001) rof       (1001)       79 2019-11-05 18:26:23.000000 ipsvm-1.1.0/src/ipsvm.egg-info/requires.txt
--rw-rw-r--   0 rof       (1001) rof       (1001)        1 2019-11-05 18:26:23.000000 ipsvm-1.1.0/src/ipsvm.egg-info/dependency_links.txt
--rw-rw-r--   0 rof       (1001) rof       (1001)      340 2019-11-05 18:26:23.000000 ipsvm-1.1.0/src/ipsvm.egg-info/SOURCES.txt
--rw-rw-r--   0 rof       (1001) rof       (1001)      300 2019-11-05 18:26:23.000000 ipsvm-1.1.0/src/ipsvm.egg-info/PKG-INFO
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2019-11-05 18:26:23.000000 ipsvm-1.1.0/src/ipsvm/
--rw-rw-r--   0 rof       (1001) rof       (1001)     6414 2019-11-05 18:25:56.000000 ipsvm-1.1.0/src/ipsvm/shock.py
--rw-rw-r--   0 rof       (1001) rof       (1001)   241414 2019-11-05 18:25:56.000000 ipsvm-1.1.0/src/ipsvm/predictor.pkl
--rw-rw-r--   0 rof       (1001) rof       (1001)    19783 2019-11-05 18:25:56.000000 ipsvm-1.1.0/src/ipsvm/ipsvm.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     5262 2019-11-05 18:25:56.000000 ipsvm-1.1.0/src/ipsvm/default.json
--rw-rw-r--   0 rof       (1001) rof       (1001)    31004 2019-11-05 18:25:56.000000 ipsvm-1.1.0/src/ipsvm/data.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1002 2019-11-05 18:25:56.000000 ipsvm-1.1.0/src/ipsvm/config.py
--rw-rw-r--   0 rof       (1001) rof       (1001)       25 2019-11-05 18:25:56.000000 ipsvm-1.1.0/src/ipsvm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:52:20.065726 ipsvm-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       82 2024-05-08 12:51:59.000000 ipsvm-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      253 2024-05-08 12:52:20.065726 ipsvm-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 12:52:20.065726 ipsvm-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      708 2024-05-08 12:51:59.000000 ipsvm-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:52:20.065726 ipsvm-1.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:52:20.065726 ipsvm-1.2.0/src/ipsvm/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-08 12:51:59.000000 ipsvm-1.2.0/src/ipsvm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-05-08 12:51:59.000000 ipsvm-1.2.0/src/ipsvm/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    39002 2024-05-08 12:51:59.000000 ipsvm-1.2.0/src/ipsvm/data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5369 2024-05-08 12:51:59.000000 ipsvm-1.2.0/src/ipsvm/default.json
+-rw-rw-rw-   0 root         (0) root         (0)    21654 2024-05-08 12:51:59.000000 ipsvm-1.2.0/src/ipsvm/ipsvm.py
+-rw-rw-rw-   0 root         (0) root         (0)   145841 2024-05-08 12:51:59.000000 ipsvm-1.2.0/src/ipsvm/predictor.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     6612 2024-05-08 12:51:59.000000 ipsvm-1.2.0/src/ipsvm/shock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:52:20.065726 ipsvm-1.2.0/src/ipsvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      253 2024-05-08 12:52:20.000000 ipsvm-1.2.0/src/ipsvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      340 2024-05-08 12:52:20.000000 ipsvm-1.2.0/src/ipsvm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 12:52:20.000000 ipsvm-1.2.0/src/ipsvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2024-05-08 12:52:20.000000 ipsvm-1.2.0/src/ipsvm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-08 12:52:20.000000 ipsvm-1.2.0/src/ipsvm.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-08 12:51:59.000000 ipsvm-1.2.0/version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ipsvm-1.1.0/src/ipsvm/shock.py` & `ipsvm-1.2.0/src/ipsvm/shock.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 import numpy as np
 from sklearn.linear_model import RANSACRegressor
 from sklearn.tree import DecisionTreeRegressor
 
 
 class Jump:
     def __init__(self, data, config):
@@ -92,15 +93,15 @@
     @property
     def dtr(self):
         if self._dtr is None and self.data.size >= self._config["MIN_POINTS"]:
             try:
                 self._dtr = RANSACRegressor(DecisionTreeRegressor(max_depth=1), min_samples=self.data.size - 1)
                 self._dtr.fit(np.transpose([self.data.index]), self.data)
             except:
-               self._dtr = None
+                self._dtr = None
         return self._dtr
 
     @property
     def timestamp(self):
         if self._timestamp is None and self.dtr is not None:
             self._timestamp = self.dtr.estimator_.tree_.threshold[0]
         return self._timestamp
@@ -119,14 +120,16 @@
                     / np.mean(self.data[self.after].diff()[1:].abs() / np.diff(self.data.index[self.after]))
                 )
             else:
                 self._jitter = 1 - (
                     np.median(self.data[self.after].diff()[1:].abs() / np.diff(self.data.index[self.after]))
                     / np.mean(self.data[self.before].diff()[1:].abs() / np.diff(self.data.index[self.before]))
                 )
+            if math.isinf(self._jitter) or math.isnan(self._jitter):
+                self._jitter = None
         return self._jitter
 
 
 class DensityJump(Jump):
     pass
 
 
@@ -166,14 +169,18 @@
             self.field_jump.sharpness,
             self.field_jump.jitter,
             (self._timestamp - self.field_jump.timestamp) / 60 if self.field_jump.timestamp is not None else None,
             self.density_jump.jump,
             self.density_jump.sharpness,
             self.speed_jump.jump,
             self.speed_jump.sharpness,
-            (self.field_jump.timestamp - self.density_jump.timestamp) / 60
-            if self.field_jump.timestamp is not None and self.density_jump.timestamp is not None
-            else None,
-            (self.field_jump.timestamp - self.speed_jump.timestamp) / 60
-            if self.field_jump.timestamp is not None and self.speed_jump.timestamp is not None
-            else None,
+            (
+                (self.field_jump.timestamp - self.density_jump.timestamp) / 60
+                if self.field_jump.timestamp is not None and self.density_jump.timestamp is not None
+                else None
+            ),
+            (
+                (self.field_jump.timestamp - self.speed_jump.timestamp) / 60
+                if self.field_jump.timestamp is not None and self.speed_jump.timestamp is not None
+                else None
+            ),
         )
```

### Comparing `ipsvm-1.1.0/src/ipsvm/ipsvm.py` & `ipsvm-1.2.0/src/ipsvm/ipsvm.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 from .config import Config
 from .data import Data
 from .shock import Shock
 
 
 DEFAULT_PREDICTOR_PATH = os.path.join(os.path.dirname(os.path.realpath(__file__)), "predictor.pkl")
 
+if not os.path.exists(DEFAULT_PREDICTOR_PATH):
+    print("Predictor file does not exist at the specified path:", DEFAULT_PREDICTOR_PATH)
+
 
 def get_random_datetime(start, end):
     start_ts = calendar.timegm(start.timetuple())
     end_ts = calendar.timegm(end.timetuple())
     return datetime.fromtimestamp(random.random() * (end_ts - start_ts) + start_ts)
 
 
@@ -59,32 +62,47 @@
         precise_shock_datetime = shock_datetime
         for step in range(
             self.config["MIN_SCAN_WINDOW"],
             self.config["MAX_SCAN_WINDOW"] + self.config["SCAN_STEP"],
             self.config["SCAN_STEP"],
         ):
             shock = Shock(
-                shock_timestamp, data.range(shock_timestamp - step * 60, shock_timestamp + step * 60), self.config
+                shock_timestamp,
+                data.range(shock_timestamp - step * 60, shock_timestamp + step * 60),
+                self.config,
             )
             features = shock.features
             if None not in features:
                 precise_shock_datetime = datetime.utcfromtimestamp(shock.field_jump.timestamp)
                 break
         return features, precise_shock_datetime
 
     def collect_true_positives(self, spacecraft, monthly=True):
         spacecraft = self.config.spacecraft_from_alias(spacecraft)
         shocks = ascii.read(self.config["SPACECRAFT"][spacecraft]["TRUE_POSITIVES_LIST"])
         shock_datetimes = np.array(
-            [datetime(row["col1"], row["col2"], row["col3"], row["col4"], row["col5"], row["col6"]) for row in shocks]
+            [
+                datetime(
+                    row["col1"],
+                    row["col2"],
+                    row["col3"],
+                    row["col4"],
+                    row["col5"],
+                    row["col6"],
+                )
+                for row in shocks
+            ]
         )
         shock_datetimes.sort()
         features_set = []
         classes_set = []
-        bar = pyprind.ProgPercent(shock_datetimes.size * self.config["TRUE_POSITIVES_SHIFT_NUMBER"], track_time=True)
+        bar = pyprind.ProgPercent(
+            shock_datetimes.size * self.config["TRUE_POSITIVES_SHIFT_NUMBER"],
+            track_time=True,
+        )
         prev_year = 0
         prev_month = 0
         data = None
         for shock_datetime in shock_datetimes:
             if monthly:
                 if shock_datetime.year != prev_year or shock_datetime.month != prev_month:
                     start = datetime(shock_datetime.year, shock_datetime.month, 1)
@@ -98,15 +116,16 @@
                     data.filter(self.config)
                     prev_year = shock_datetime.year
                     prev_month = shock_datetime.month
 
             count_shifts = 0
             while count_shifts < self.config["TRUE_POSITIVES_SHIFT_NUMBER"]:
                 shift = random.uniform(
-                    -self.config["TRUE_POSITIVES_SHIFT_RANGE"], self.config["TRUE_POSITIVES_SHIFT_RANGE"]
+                    -self.config["TRUE_POSITIVES_SHIFT_RANGE"],
+                    self.config["TRUE_POSITIVES_SHIFT_RANGE"],
                 )
                 if monthly:
                     range_data = data.range(
                         dt2ts(
                             shock_datetime
                             + timedelta(minutes=shift)
                             - timedelta(minutes=self.config["MAX_SCAN_WINDOW"])
@@ -136,15 +155,25 @@
             self.config["SPACECRAFT"][spacecraft]["TRUE_POSITIVES_FEATURES_SET"],
         )
 
     def collect_false_positives(self, spacecraft, start=None, step=timedelta(minutes=5)):
         spacecraft = self.config.spacecraft_from_alias(spacecraft)
         shocks = ascii.read(self.config["SPACECRAFT"][spacecraft]["TRUE_POSITIVES_LIST"])
         shock_datetimes = np.array(
-            [datetime(row["col1"], row["col2"], row["col3"], row["col4"], row["col5"], row["col6"]) for row in shocks]
+            [
+                datetime(
+                    row["col1"],
+                    row["col2"],
+                    row["col3"],
+                    row["col4"],
+                    row["col5"],
+                    row["col6"],
+                )
+                for row in shocks
+            ]
         )
         shock_datetimes.sort()
         first_shock_datetime = np.amin(shock_datetimes)
         last_shock_datetime = np.amax(shock_datetimes)
 
         if start is None:
             start = datetime(first_shock_datetime.year, first_shock_datetime.month, 1)
@@ -201,15 +230,25 @@
                 self.config["SPACECRAFT"][spacecraft]["FALSE_POSITIVES_FEATURES_SET"],
             )
 
     def collect_true_negatives(self, spacecraft, monthly=True):
         spacecraft = self.config.spacecraft_from_alias(spacecraft)
         shocks = ascii.read(self.config["SPACECRAFT"][spacecraft]["TRUE_POSITIVES_LIST"])
         shock_datetimes = np.array(
-            [datetime(row["col1"], row["col2"], row["col3"], row["col4"], row["col5"], row["col6"]) for row in shocks]
+            [
+                datetime(
+                    row["col1"],
+                    row["col2"],
+                    row["col3"],
+                    row["col4"],
+                    row["col5"],
+                    row["col6"],
+                )
+                for row in shocks
+            ]
         )
         shock_datetimes.sort()
         first_shock_datetime = np.amin(shock_datetimes)
 
         features_set = []
         classes_set = []
 
@@ -218,15 +257,16 @@
         prev_year = 0
         prev_month = 0
 
         start = datetime(first_shock_datetime.year, first_shock_datetime.month, 1)
         end = start + relativedelta(months=1)
 
         bar = pyprind.ProgPercent(
-            self.config["TRUE_NEGATIVES_PER_TRUE_POSITIVES"] * shock_datetimes.size, track_time=True
+            self.config["TRUE_NEGATIVES_PER_TRUE_POSITIVES"] * shock_datetimes.size,
+            track_time=True,
         )
         for shock_datetime in shock_datetimes:
             if monthly:
                 if shock_datetime.year != prev_year or shock_datetime.month != prev_month:
                     start = datetime(shock_datetime.year, shock_datetime.month, 1)
                     end = start + relativedelta(months=1)
                     data = Data.get_spacecraft_data(
@@ -268,15 +308,21 @@
                     bar.update()
 
         joblib.dump(
             {"features": features_set, "classes": classes_set},
             self.config["SPACECRAFT"][spacecraft]["TRUE_NEGATIVES_FEATURES_SET"],
         )
 
-    def fit(self, true_positives=["ACE"], false_positives=[], true_negatives=["ACE"], save=False):
+    def fit(
+        self,
+        true_positives=["ACE"],
+        false_positives=[],
+        true_negatives=["ACE"],
+        save=False,
+    ):
         train_features_set = []
         train_classes_set = []
         test_features_set = []
         test_classes_set = []
 
         if true_positives is not None:
             true_positives_features_set = []
@@ -284,15 +330,17 @@
             for spacecraft in true_positives:
                 spacecraft = self.config.spacecraft_from_alias(spacecraft)
                 data = joblib.load(self.config["SPACECRAFT"][spacecraft]["TRUE_POSITIVES_FEATURES_SET"])
                 true_positives_features_set += data["features"]
                 true_positives_classes_set += data["classes"]
             n_true_positives = len(true_positives_features_set)
             i_train_true_positives = np.random.choice(
-                np.arange(n_true_positives), int(self.config["TRAIN_RATIO"] * n_true_positives), replace=False
+                np.arange(n_true_positives),
+                int(self.config["TRAIN_RATIO"] * n_true_positives),
+                replace=False,
             )
             i_test_true_positives = np.random.choice(
                 np.delete(np.arange(n_true_positives), i_train_true_positives),
                 int(self.config["TEST_RATIO"] * n_true_positives),
                 replace=False,
             )
             for i in i_train_true_positives:
@@ -308,15 +356,17 @@
             for spacecraft in false_positives:
                 spacecraft = self.config.spacecraft_from_alias(spacecraft)
                 data = joblib.load(self.config["SPACECRAFT"][spacecraft]["FALSE_POSITIVES_FEATURES_SET"])
                 false_positives_features_set += data["features"]
                 false_positives_classes_set += data["classes"]
             n_false_positives = len(false_positives_features_set)
             i_train_false_positives = np.random.choice(
-                np.arange(n_false_positives), int(self.config["TRAIN_RATIO"] * n_false_positives), replace=False
+                np.arange(n_false_positives),
+                int(self.config["TRAIN_RATIO"] * n_false_positives),
+                replace=False,
             )
             i_test_false_positives = np.random.choice(
                 np.delete(np.arange(n_false_positives), i_train_false_positives),
                 int(self.config["TEST_RATIO"] * n_false_positives),
                 replace=False,
             )
             for i in i_train_false_positives:
@@ -332,15 +382,17 @@
             for spacecraft in true_negatives:
                 spacecraft = self.config.spacecraft_from_alias(spacecraft)
                 data = joblib.load(self.config["SPACECRAFT"][spacecraft]["TRUE_NEGATIVES_FEATURES_SET"])
                 true_negatives_features_set += data["features"]
                 true_negatives_classes_set += data["classes"]
             n_true_negatives = len(true_negatives_features_set)
             i_train_true_negatives = np.random.choice(
-                np.arange(n_true_negatives), int(self.config["TRAIN_RATIO"] * n_true_negatives), replace=False
+                np.arange(n_true_negatives),
+                int(self.config["TRAIN_RATIO"] * n_true_negatives),
+                replace=False,
             )
             i_test_true_negatives = np.random.choice(
                 np.delete(np.arange(n_true_negatives), i_train_true_negatives),
                 int(self.config["TEST_RATIO"] * n_true_negatives),
                 replace=False,
             )
             for i in i_train_true_negatives:
@@ -354,31 +406,38 @@
         train_classes_set = np.hstack(train_classes_set)
         test_features_set = np.vstack(test_features_set)
         test_classes_set = np.hstack(test_classes_set)
 
         param_grid = [{"svc__C": np.logspace(0, 2, 10), "svc__gamma": np.logspace(-2, 0, 10)}]
 
         self._predictor = GridSearchCV(
-            make_pipeline(StandardScaler().fit(train_features_set), SVC(class_weight="balanced", probability=True)),
+            make_pipeline(
+                StandardScaler().fit(train_features_set),
+                SVC(class_weight="balanced", probability=True),
+            ),
             param_grid=param_grid,
             scoring=self.config["SCORING"],
             n_jobs=-1,
             cv=self.config["CROSS_VALIDATION"],
         )
         self.predictor.fit(train_features_set, train_classes_set)
 
         if save:
             joblib.dump(self.predictor, self.config["PREDICTOR"])
 
         if self.config["TEST_RATIO"] > 0.0:
-            print("All test set score: ", self.predictor.score(test_features_set, test_classes_set))
+            print(
+                "All test set score: ",
+                self.predictor.score(test_features_set, test_classes_set),
+            )
             print(
                 "Only shocks score: ",
                 self.predictor.score(
-                    test_features_set[test_classes_set == True], test_classes_set[test_classes_set == True]
+                    test_features_set[test_classes_set == True],
+                    test_classes_set[test_classes_set == True],
                 ),
             )
         precision, recall, _ = precision_recall_curve(
             test_classes_set, self.predictor.decision_function(test_features_set)
         )
         plt.plot(recall, precision, label="Precision-Recall curve")
         plt.xlabel("Recall")
@@ -420,16 +479,35 @@
             range_data = data.range(
                 dt2ts(test_datetime - timedelta(minutes=self.config["MAX_SCAN_WINDOW"])),
                 dt2ts(test_datetime + timedelta(minutes=self.config["MAX_SCAN_WINDOW"])),
             )
             features, shock_datetime = self.get_adaptive_features(test_datetime, range_data)
 
             if None not in features:
-                predicted_class = self.predictor.predict(np.array([np.hstack(features)]))[0]
-                if predicted_class == True:
-                    predicted_prob = self.predictor.predict_proba(np.array([np.hstack(features)]))[0][
-                        int(predicted_class)
-                    ]
-                    shocks.append([shock_datetime, predicted_prob])
-                    print(shock_datetime, predicted_prob)
+                try:
+                    predicted_class = self.predictor.predict(np.array([np.hstack(features)]))[0]
+                    if predicted_class == True:
+                        predicted_prob = self.predictor.predict_proba(np.array([np.hstack(features)]))[0][
+                            int(predicted_class)
+                        ]
+                        shocks.append([shock_datetime, predicted_prob])
+                        print(shock_datetime, predicted_prob)
+                except:
+                    print(features)
             test_datetime += step
         return np.array(shocks)
+
+    def bigscan(self, spacecraft, start_date, end_date):
+        shocks = []
+        spacecraft = self.config.spacecraft_from_alias(spacecraft)
+        start = datetime(start_date.year, start_date.month, 1)
+        end = start + relativedelta(months=1)
+        total_months = (end_date.year - start_date.year - 1) * 12 + end_date.month + (12 - start_date.month + 1)
+        bar = pyprind.ProgPercent(total_months, track_time=True)
+
+        while start <= end_date:
+            monthly_shocks = self.scan(spacecraft, start, end)
+            shocks.extend(monthly_shocks)
+            start += relativedelta(months=1)
+            end += relativedelta(months=1)
+            bar.update()
+        return shocks
```

### Comparing `ipsvm-1.1.0/src/ipsvm/default.json` & `ipsvm-1.2.0/src/ipsvm/default.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967948717948718%*

 * *Differences: {"'SPACECRAFT'": "{'PSP': OrderedDict([('ALIASES', ['PSP', 'psp'])]), 'SOLO': "*

 * *                 "OrderedDict([('ALIASES', ['SOLO', 'solo'])])}"}*

```diff
@@ -69,14 +69,26 @@
                 "omni"
             ],
             "FALSE_POSITIVES_FEATURES_SET": "./resources/false_positives_features_set_omni.pkl",
             "TRUE_NEGATIVES_FEATURES_SET": "./resources/true_negatives_features_set_omni.pkl",
             "TRUE_POSITIVES_FEATURES_SET": "./resources/true_positives_features_set_omni.pkl",
             "TRUE_POSITIVES_LIST": "./resources/true_positives_list_omni.dat"
         },
+        "PSP": {
+            "ALIASES": [
+                "PSP",
+                "psp"
+            ]
+        },
+        "SOLO": {
+            "ALIASES": [
+                "SOLO",
+                "solo"
+            ]
+        },
         "STEREOA": {
             "ALIASES": [
                 "stereo-a",
                 "stereoa",
                 "stereo a",
                 "sta"
             ],
```

### Comparing `ipsvm-1.1.0/src/ipsvm/data.py` & `ipsvm-1.2.0/src/ipsvm/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,17 +72,205 @@
             data = Data.get_ulysses_data(start, end, config)
         elif spacecraft == "VOYAGER1":
             data = Data.get_voyager1_data(start, end, config)
         elif spacecraft == "VOYAGER2":
             data = Data.get_voyager2_data(start, end, config)
         elif spacecraft == "WIND":
             data = Data.get_wind_data(start, end, config)
+        elif spacecraft == "PSP":
+            data = Data.get_psp_data(start, end, config)
+        elif spacecraft == "SOLO":
+            data = Data.get_solo_data(start, end, config)
         return data
 
     @staticmethod
+    def get_psp_data(start, end, config):
+        if config["CACHE"] is not None and os.path.isdir(config["CACHE"]):
+            cdas.set_cache(True, config["CACHE"])
+        else:
+            cdas.set_cache(False)
+        try:
+            field_data = cdas.get_data(
+                "sp_phys",
+                "PSP_FLD_L2_MAG_RTN_1MIN",
+                start,
+                end,
+                ["psp_fld_l2_mag_RTN_1min"],
+                cdf=config["DOWNLOAD_CDF"],
+                progress=config["DOWNLOAD_PROGRESS"],
+            )
+            if config["DOWNLOAD_CDF"]:
+                epoch_key = "epoch_mag_RTN_1min"
+                field_key = "psp_fld_l2_mag_RTN_1min"
+                mask = (
+                    (field_data[field_key][:, 0] != GAP)
+                    & (field_data[field_key][:, 1] != GAP)
+                    & (field_data[field_key][:, 2] != GAP)
+                )
+                field = pd.Series(
+                    np.sqrt(
+                        field_data[field_key][mask, 0] ** 2
+                        + field_data[field_key][mask, 1] ** 2
+                        + field_data[field_key][mask, 2] ** 2
+                    ),
+                    index=[calendar.timegm(dt.timetuple()) for dt in field_data[epoch_key][mask]],
+                )
+            else:
+                epoch_key = "EPOCH"
+                mask = (field_data["B_R"] != GAP) & (field_data["B_T"] != GAP) & (field_data["B_N"] != GAP)
+                field = pd.Series(
+                    np.sqrt(field_data["B_R"][mask] ** 2 + field_data["B_T"][mask] ** 2 + field_data["B_N"][mask] ** 2),
+                    index=[calendar.timegm(dt.timetuple()) for dt in field_data[epoch_key][mask]],
+                )
+        except cdas.NoDataError:
+            field = pd.Series()
+        try:
+            plasma_data = cdas.get_data(
+                "sp_phys",
+                "PSP_SWP_SPC_L3I",
+                start,
+                end,
+                ["np_moment_gd", "vp_moment_RTN_gd"],
+                cdf=config["DOWNLOAD_CDF"],
+                progress=config["DOWNLOAD_PROGRESS"],
+            )
+
+            epoch_key = "Epoch" if config["DOWNLOAD_CDF"] else "EPOCH"
+            density_key = "np_moment_gd" if config["DOWNLOAD_CDF"] else "NP_MOMENT"
+            mask = plasma_data[density_key] != GAP
+            density = pd.Series(
+                plasma_data[density_key][mask],
+                index=[calendar.timegm(dt.timetuple()) for dt in plasma_data[epoch_key][mask]],
+            )
+
+            if config["DOWNLOAD_CDF"]:
+                speed_key = "vp_moment_RTN_gd"
+                mask = (
+                    (plasma_data[speed_key][:, 0] != GAP)
+                    & (plasma_data[speed_key][:, 1] != GAP)
+                    & (plasma_data[speed_key][:, 2] != GAP)
+                )
+                speed = pd.Series(
+                    np.sqrt(
+                        plasma_data[speed_key][mask, 0] ** 2
+                        + plasma_data[speed_key][mask, 1] ** 2
+                        + plasma_data[speed_key][mask, 2] ** 2
+                    ),
+                    index=[calendar.timegm(dt.timetuple()) for dt in plasma_data[epoch_key][mask]],
+                )
+            else:
+                mask = (
+                    (plasma_data["VP_MOMENT_R"] != GAP)
+                    & (plasma_data["VP_MOMENT_T"] != GAP)
+                    & (plasma_data["VP_MOMENT_N"] != GAP)
+                )
+                speed = pd.Series(
+                    np.sqrt(
+                        plasma_data["VP_MOMENT_R"][mask] ** 2
+                        + plasma_data["VP_MOMENT_T"][mask] ** 2
+                        + plasma_data["VP_MOMENT_N"][mask] ** 2
+                    ),
+                    index=[calendar.timegm(dt.timetuple()) for dt in plasma_data[epoch_key][mask]],
+                )
+
+        except cdas.NoDataError:
+            density = pd.Series()
+            speed = pd.Series()
+
+        return Data(field, density, speed)
+
+    @staticmethod
+    def get_solo_data(start, end, config):
+        if config["CACHE"] is not None and os.path.isdir(config["CACHE"]):
+            cdas.set_cache(True, config["CACHE"])
+        else:
+            cdas.set_cache(False)
+        try:
+            field_data = cdas.get_data(
+                "sp_phys",
+                "SOLO_L2_MAG-RTN-NORMAL",
+                start,
+                end,
+                ["B_RTN"],
+                cdf=config["DOWNLOAD_CDF"],
+                progress=config["DOWNLOAD_PROGRESS"],
+            )
+            epoch_key = "EPOCH"
+            if config["DOWNLOAD_CDF"]:
+                field_key = "B_RTN"
+                mask = (
+                    (field_data[field_key][:, 0] != GAP)
+                    & (field_data[field_key][:, 1] != GAP)
+                    & (field_data[field_key][:, 2] != GAP)
+                )
+                field = pd.Series(
+                    np.sqrt(
+                        field_data[field_key][mask, 0] ** 2
+                        + field_data[field_key][mask, 1] ** 2
+                        + field_data[field_key][mask, 2] ** 2
+                    ),
+                    index=[calendar.timegm(dt.timetuple()) for dt in field_data[epoch_key][mask]],
+                )
+            else:
+                mask = mask = (field_data["B_R"] != GAP) & (field_data["B_T"] != GAP) & (field_data["B_N"] != GAP)
+                field = pd.Series(
+                    np.sqrt(field_data["B_R"][mask] ** 2 + field_data["B_T"][mask] ** 2 + field_data["B_N"][mask] ** 2),
+                    index=[calendar.timegm(dt.timetuple()) for dt in field_data[epoch_key][mask]],
+                )
+
+        except cdas.NoDataError:
+            field = pd.Series()
+        try:
+            plasma_data = cdas.get_data(
+                "sp_phys",
+                "SOLO_L2_SWA-PAS-GRND-MOM",
+                start,
+                end,
+                ["N", "V_RTN"],
+                cdf=config["DOWNLOAD_CDF"],
+                progress=config["DOWNLOAD_PROGRESS"],
+            )
+            epoch_key = "Epoch" if config["DOWNLOAD_CDF"] else "EPOCH"
+            density_key = "N" if config["DOWNLOAD_CDF"] else "DENSITY"
+            mask = plasma_data[density_key] != GAP
+            density = pd.Series(
+                plasma_data[density_key][mask],
+                index=[calendar.timegm(dt.timetuple()) for dt in plasma_data[epoch_key][mask]],
+            )
+            if config["DOWNLOAD_CDF"]:
+                speed_key = "V_RTN"
+                mask = (
+                    (plasma_data[speed_key][:, 0] != GAP)
+                    & (plasma_data[speed_key][:, 1] != GAP)
+                    & (plasma_data[speed_key][:, 2] != GAP)
+                )
+                speed = pd.Series(
+                    np.sqrt(
+                        plasma_data[speed_key][mask, 0] ** 2
+                        + plasma_data[speed_key][mask, 1] ** 2
+                        + plasma_data[speed_key][mask, 2] ** 2
+                    ),
+                    index=[calendar.timegm(dt.timetuple()) for dt in plasma_data[epoch_key][mask]],
+                )
+            else:
+                mask = (plasma_data["VR_RTN"] != GAP) & (plasma_data["VT_RTN"] != GAP) & (plasma_data["VN_RTN"] != GAP)
+                speed = pd.Series(
+                    np.sqrt(
+                        plasma_data["VR_RTN"][mask] ** 2
+                        + plasma_data["VT_RTN"][mask] ** 2
+                        + plasma_data["VN_RTN"][mask] ** 2
+                    ),
+                    index=[calendar.timegm(dt.timetuple()) for dt in plasma_data[epoch_key][mask]],
+                )
+        except cdas.NoDataError:
+            density = pd.Series()
+            speed = pd.Series()
+        return Data(field, density, speed)
+
+    @staticmethod
     def get_ace_data(start, end, config):
         if config["CACHE"] is not None and os.path.isdir(config["CACHE"]):
             cdas.set_cache(True, config["CACHE"])
         else:
             cdas.set_cache(False)
         try:
             field_data = cdas.get_data(
@@ -701,27 +889,29 @@
                 ["V_GSE_plog", "Np"],
                 cdf=config["DOWNLOAD_CDF"],
                 progress=config["DOWNLOAD_PROGRESS"],
             )
             if config["DOWNLOAD_CDF"]:
                 mask = plasma_data["Np"] != GAP
                 density = pd.Series(
-                    plasma_data["Np"][mask], index=[calendar.timegm(dt.timetuple()) for dt in plasma_data["Epoch"][mask]]
+                    plasma_data["Np"][mask],
+                    index=[calendar.timegm(dt.timetuple()) for dt in plasma_data["Epoch"][mask]],
                 )
                 if plasma_data["Epoch"].size == 1:
                     plasma_data["V_GSE_p"] = np.array([plasma_data["V_GSE_p"]])
                 mask = plasma_data["V_GSE_p"][:, 0] != GAP
                 speed = pd.Series(
                     plasma_data["V_GSE_p"][mask, 0],
                     index=[calendar.timegm(dt.timetuple()) for dt in plasma_data["Epoch"][mask]],
                 )
             else:
                 mask = plasma_data["ION_NP"] != GAP
                 density = pd.Series(
-                    plasma_data["ION_NP"][mask], index=[calendar.timegm(dt.timetuple()) for dt in plasma_data["EPOCH"][mask]]
+                    plasma_data["ION_NP"][mask],
+                    index=[calendar.timegm(dt.timetuple()) for dt in plasma_data["EPOCH"][mask]],
                 )
                 mask = plasma_data["FLOW_SPEED"] != GAP
                 speed = pd.Series(
                     plasma_data["FLOW_SPEED"][mask],
                     index=[calendar.timegm(dt.timetuple()) for dt in plasma_data["EPOCH"][mask]],
                 )
         except:
```

### Comparing `ipsvm-1.1.0/src/ipsvm/config.py` & `ipsvm-1.2.0/src/ipsvm/config.py`

 * *Files identical despite different names*

