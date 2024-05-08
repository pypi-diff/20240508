# Comparing `tmp/miautawn_auto_validate_by_history-0.1.0.tar.gz` & `tmp/miautawn_auto_validate_by_history-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miautawn_auto_validate_by_history-0.1.0.tar", max compression
+gzip compressed data, was "miautawn_auto_validate_by_history-0.1.1.tar", max compression
```

## Comparing `miautawn_auto_validate_by_history-0.1.0.tar` & `miautawn_auto_validate_by_history-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1076 2024-04-01 09:38:57.072679 miautawn_auto_validate_by_history-0.1.0/LICENSE
--rw-r--r--   0        0        0     4244 2024-05-07 06:09:37.192441 miautawn_auto_validate_by_history-0.1.0/README.md
--rw-r--r--   0        0        0     1195 2024-05-07 05:50:36.976350 miautawn_auto_validate_by_history-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      840 2024-05-06 16:05:34.417573 miautawn_auto_validate_by_history-0.1.0/src/avh/__init__.py
--rw-r--r--   0        0        0      228 2024-05-06 16:05:34.418012 miautawn_auto_validate_by_history-0.1.0/src/avh/aliases.py
--rw-r--r--   0        0        0    14563 2024-05-07 05:50:36.977225 miautawn_auto_validate_by_history-0.1.0/src/avh/auto_validate_by_history.py
--rw-r--r--   0        0        0      514 2024-05-06 16:05:34.419437 miautawn_auto_validate_by_history-0.1.0/src/avh/constraints/__init__.py
--rw-r--r--   0        0        0     3027 2024-05-06 16:05:34.419775 miautawn_auto_validate_by_history-0.1.0/src/avh/constraints/_base.py
--rw-r--r--   0        0        0     4060 2024-05-06 16:05:34.420212 miautawn_auto_validate_by_history-0.1.0/src/avh/constraints/_constraints.py
--rw-r--r--   0        0        0     1047 2024-05-06 16:05:34.420682 miautawn_auto_validate_by_history-0.1.0/src/avh/constraints/_data_quality_program.py
--rw-r--r--   0        0        0      612 2024-05-06 16:05:34.421116 miautawn_auto_validate_by_history-0.1.0/src/avh/data_generation/__init__.py
--rw-r--r--   0        0        0     5111 2024-05-06 16:05:34.421486 miautawn_auto_validate_by_history-0.1.0/src/avh/data_generation/_base.py
--rw-r--r--   0        0        0     1827 2024-05-07 05:50:36.977856 miautawn_auto_validate_by_history-0.1.0/src/avh/data_generation/_categorical.py
--rw-r--r--   0        0        0     3255 2024-05-06 16:05:34.422365 miautawn_auto_validate_by_history-0.1.0/src/avh/data_generation/_numeric.py
--rw-r--r--   0        0        0     4960 2024-05-06 16:05:34.422769 miautawn_auto_validate_by_history-0.1.0/src/avh/data_generation/_pipeline.py
--rw-r--r--   0        0        0     2008 2024-05-06 16:05:34.423121 miautawn_auto_validate_by_history-0.1.0/src/avh/data_issues/__init__.py
--rw-r--r--   0        0        0     1381 2024-05-06 16:05:34.423448 miautawn_auto_validate_by_history-0.1.0/src/avh/data_issues/_base.py
--rw-r--r--   0        0        0     1214 2024-05-06 16:05:34.423778 miautawn_auto_validate_by_history-0.1.0/src/avh/data_issues/_categorical.py
--rw-r--r--   0        0        0     4392 2024-05-06 16:05:34.424186 miautawn_auto_validate_by_history-0.1.0/src/avh/data_issues/_dataset.py
--rw-r--r--   0        0        0     6457 2024-05-06 16:05:34.424677 miautawn_auto_validate_by_history-0.1.0/src/avh/data_issues/_issues.py
--rw-r--r--   0        0        0     6265 2024-05-06 16:05:34.425108 miautawn_auto_validate_by_history-0.1.0/src/avh/data_issues/_numeric.py
--rw-r--r--   0        0        0     1067 2024-05-06 16:05:34.425440 miautawn_auto_validate_by_history-0.1.0/src/avh/metrics/__init__.py
--rw-r--r--   0        0        0     2199 2024-05-06 16:05:34.425758 miautawn_auto_validate_by_history-0.1.0/src/avh/metrics/_base.py
--rw-r--r--   0        0        0     1139 2024-05-06 16:05:34.426142 miautawn_auto_validate_by_history-0.1.0/src/avh/metrics/_categorical.py
--rw-r--r--   0        0        0      887 2024-05-06 16:05:34.426596 miautawn_auto_validate_by_history-0.1.0/src/avh/metrics/_metrics.py
--rw-r--r--   0        0        0     4959 2024-05-06 16:05:34.427162 miautawn_auto_validate_by_history-0.1.0/src/avh/metrics/_numeric.py
--rw-r--r--   0        0        0     1774 2024-05-06 16:05:34.428067 miautawn_auto_validate_by_history-0.1.0/src/avh/utility_functions.py
--rw-r--r--   0        0        0     5223 1970-01-01 00:00:00.000000 miautawn_auto_validate_by_history-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-01 09:38:57.072679 miautawn_auto_validate_by_history-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4244 2024-05-07 06:09:37.192441 miautawn_auto_validate_by_history-0.1.1/README.md
+-rw-r--r--   0        0        0     1195 2024-05-07 10:45:00.249285 miautawn_auto_validate_by_history-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      840 2024-05-06 16:05:34.417573 miautawn_auto_validate_by_history-0.1.1/src/avh/__init__.py
+-rw-r--r--   0        0        0      228 2024-05-06 16:05:34.418012 miautawn_auto_validate_by_history-0.1.1/src/avh/aliases.py
+-rw-r--r--   0        0        0    14563 2024-05-07 10:45:00.250246 miautawn_auto_validate_by_history-0.1.1/src/avh/auto_validate_by_history.py
+-rw-r--r--   0        0        0      514 2024-05-06 16:05:34.419437 miautawn_auto_validate_by_history-0.1.1/src/avh/constraints/__init__.py
+-rw-r--r--   0        0        0     3027 2024-05-06 16:05:34.419775 miautawn_auto_validate_by_history-0.1.1/src/avh/constraints/_base.py
+-rw-r--r--   0        0        0     4060 2024-05-06 16:05:34.420212 miautawn_auto_validate_by_history-0.1.1/src/avh/constraints/_constraints.py
+-rw-r--r--   0        0        0     1047 2024-05-06 16:05:34.420682 miautawn_auto_validate_by_history-0.1.1/src/avh/constraints/_data_quality_program.py
+-rw-r--r--   0        0        0      612 2024-05-06 16:05:34.421116 miautawn_auto_validate_by_history-0.1.1/src/avh/data_generation/__init__.py
+-rw-r--r--   0        0        0     5111 2024-05-06 16:05:34.421486 miautawn_auto_validate_by_history-0.1.1/src/avh/data_generation/_base.py
+-rw-r--r--   0        0        0     1827 2024-05-07 05:50:36.977856 miautawn_auto_validate_by_history-0.1.1/src/avh/data_generation/_categorical.py
+-rw-r--r--   0        0        0     3255 2024-05-06 16:05:34.422365 miautawn_auto_validate_by_history-0.1.1/src/avh/data_generation/_numeric.py
+-rw-r--r--   0        0        0     4960 2024-05-06 16:05:34.422769 miautawn_auto_validate_by_history-0.1.1/src/avh/data_generation/_pipeline.py
+-rw-r--r--   0        0        0     2008 2024-05-06 16:05:34.423121 miautawn_auto_validate_by_history-0.1.1/src/avh/data_issues/__init__.py
+-rw-r--r--   0        0        0     1381 2024-05-06 16:05:34.423448 miautawn_auto_validate_by_history-0.1.1/src/avh/data_issues/_base.py
+-rw-r--r--   0        0        0     1214 2024-05-06 16:05:34.423778 miautawn_auto_validate_by_history-0.1.1/src/avh/data_issues/_categorical.py
+-rw-r--r--   0        0        0     4392 2024-05-06 16:05:34.424186 miautawn_auto_validate_by_history-0.1.1/src/avh/data_issues/_dataset.py
+-rw-r--r--   0        0        0     6457 2024-05-06 16:05:34.424677 miautawn_auto_validate_by_history-0.1.1/src/avh/data_issues/_issues.py
+-rw-r--r--   0        0        0     6265 2024-05-06 16:05:34.425108 miautawn_auto_validate_by_history-0.1.1/src/avh/data_issues/_numeric.py
+-rw-r--r--   0        0        0     1067 2024-05-06 16:05:34.425440 miautawn_auto_validate_by_history-0.1.1/src/avh/metrics/__init__.py
+-rw-r--r--   0        0        0     2199 2024-05-06 16:05:34.425758 miautawn_auto_validate_by_history-0.1.1/src/avh/metrics/_base.py
+-rw-r--r--   0        0        0     1139 2024-05-06 16:05:34.426142 miautawn_auto_validate_by_history-0.1.1/src/avh/metrics/_categorical.py
+-rw-r--r--   0        0        0      887 2024-05-06 16:05:34.426596 miautawn_auto_validate_by_history-0.1.1/src/avh/metrics/_metrics.py
+-rw-r--r--   0        0        0     4975 2024-05-07 10:45:00.251282 miautawn_auto_validate_by_history-0.1.1/src/avh/metrics/_numeric.py
+-rw-r--r--   0        0        0     1774 2024-05-06 16:05:34.428067 miautawn_auto_validate_by_history-0.1.1/src/avh/utility_functions.py
+-rw-r--r--   0        0        0     5223 1970-01-01 00:00:00.000000 miautawn_auto_validate_by_history-0.1.1/PKG-INFO
```

### Comparing `miautawn_auto_validate_by_history-0.1.0/LICENSE` & `miautawn_auto_validate_by_history-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/README.md` & `miautawn_auto_validate_by_history-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/pyproject.toml` & `miautawn_auto_validate_by_history-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "miautawn-auto-validate-by-history"
-version = "0.1.0"
+version = "0.1.1"
 description = "Automatic data quality validation for data pipelines"
 authors = ["miautawn <miautawn@gmail.com>"]
 packages = [
   {include = "avh", from = "src"},
 ]
 readme = "README.md"
 repository = "https://github.com/Miautawn/Auto-Validate-By-History-Clone"
```

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/__init__.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/__init__.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/auto_validate_by_history.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/auto_validate_by_history.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -102,17 +102,17 @@
             metrics.KsDist,
             metrics.CohenD,
         ]
 
     @property
     def default_constraint_estimators(self) -> List[constraints.ConstraintType]:
         return [
-            constraints.CLTConstraint,
             constraints.ChebyshevConstraint,
             constraints.CantelliConstraint,
+            constraints.CLTConstraint,
         ]
 
     @property
     def default_beta_ranges(self) -> Dict[constraints.ConstraintType, Tuple[float, float, float]]:
         """
         Returns default beta ranges (in terms fo standard deviations)
             for the default constraint estimators.
```

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/constraints/__init__.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/constraints/_base.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/constraints/_base.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/constraints/_constraints.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/constraints/_constraints.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/constraints/_data_quality_program.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/constraints/_data_quality_program.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/data_generation/__init__.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/data_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/data_generation/_base.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/data_generation/_base.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/data_generation/_categorical.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/data_generation/_categorical.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/data_generation/_numeric.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/data_generation/_numeric.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/data_generation/_pipeline.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/data_generation/_pipeline.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/data_issues/__init__.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/data_issues/__init__.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/data_issues/_base.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/data_issues/_base.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/data_issues/_categorical.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/data_issues/_categorical.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/data_issues/_dataset.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/data_issues/_dataset.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/data_issues/_issues.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/data_issues/_issues.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/data_issues/_numeric.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/data_issues/_numeric.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/metrics/__init__.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/metrics/_base.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/metrics/_base.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/metrics/_categorical.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/metrics/_categorical.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/metrics/_metrics.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/metrics/_metrics.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/metrics/_numeric.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/metrics/_numeric.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 class KsDist(NumericMetricMixin, TwoDistributionMetric):
     @classmethod
     def _calculate(self, new_sample: pd.Series, old_sample: pd.Series) -> float:
         if self._is_empty(new_sample, old_sample):
             return np.inf
 
-        _, ks_p_val = ks_2samp(new_sample, old_sample, nan_policy="omit")
+        _, ks_p_val = ks_2samp(new_sample, old_sample, nan_policy="omit", method="asymp")
         return 1 - ks_p_val
 
 
 class CohenD(NumericMetricMixin, TwoDistributionMetric):
     @classmethod
     def _calculate(self, new_sample: pd.Series, old_sample: pd.Series) -> float:
         """
```

### Comparing `miautawn_auto_validate_by_history-0.1.0/src/avh/utility_functions.py` & `miautawn_auto_validate_by_history-0.1.1/src/avh/utility_functions.py`

 * *Files identical despite different names*

### Comparing `miautawn_auto_validate_by_history-0.1.0/PKG-INFO` & `miautawn_auto_validate_by_history-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miautawn-auto-validate-by-history
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automatic data quality validation for data pipelines
 Home-page: https://github.com/Miautawn/Auto-Validate-By-History-Clone
 Keywords: data,quality,pipeline
 Author: miautawn
 Author-email: miautawn@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
```

