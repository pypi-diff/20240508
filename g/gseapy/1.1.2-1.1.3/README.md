# Comparing `tmp/gseapy-1.1.2.tar.gz` & `tmp/gseapy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gseapy-1.1.2.tar", last modified: Thu Feb 29 20:26:18 2024, max compression
+gzip compressed data, was "gseapy-1.1.3.tar", last modified: Wed May  8 18:06:28 2024, max compression
```

## Comparing `gseapy-1.1.2.tar` & `gseapy-1.1.3.tar`

### file list

```diff
@@ -1,45 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 20:26:18.114448 gseapy-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-29 20:26:01.000000 gseapy-1.1.2/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-02-29 20:26:01.000000 gseapy-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-29 20:26:01.000000 gseapy-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-02-29 20:26:18.114448 gseapy-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-02-29 20:26:01.000000 gseapy-1.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 20:26:18.110448 gseapy-1.1.2/gseapy/
--rw-r--r--   0 runner    (1001) docker     (127)    29501 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28866 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27980 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)    32042 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/biomart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 20:26:18.110448 gseapy-1.1.2/gseapy/data/
--rw-r--r--   0 runner    (1001) docker     (127)    30869 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/data/palette.json
--rw-r--r--   0 runner    (1001) docker     (127)    23542 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/enrichr.py
--rw-r--r--   0 runner    (1001) docker     (127)    23254 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/gsea.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/gsva.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/msigdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    57322 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/scipalette.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/ssgsea.py
--rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-02-29 20:26:01.000000 gseapy-1.1.2/gseapy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 20:26:18.114448 gseapy-1.1.2/gseapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-02-29 20:26:18.000000 gseapy-1.1.2/gseapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-29 20:26:18.000000 gseapy-1.1.2/gseapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 20:26:18.000000 gseapy-1.1.2/gseapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-29 20:26:18.000000 gseapy-1.1.2/gseapy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 20:26:18.000000 gseapy-1.1.2/gseapy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-29 20:26:18.000000 gseapy-1.1.2/gseapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-29 20:26:18.000000 gseapy-1.1.2/gseapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-29 20:26:01.000000 gseapy-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-29 20:26:01.000000 gseapy-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 20:26:18.114448 gseapy-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-02-29 20:26:01.000000 gseapy-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 20:26:18.114448 gseapy-1.1.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-02-29 20:26:01.000000 gseapy-1.1.2/src/algorithm.rs
--rw-r--r--   0 runner    (1001) docker     (127)    13423 2024-02-29 20:26:01.000000 gseapy-1.1.2/src/gsva.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-02-29 20:26:01.000000 gseapy-1.1.2/src/help.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-02-29 20:26:01.000000 gseapy-1.1.2/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)    42194 2024-02-29 20:26:01.000000 gseapy-1.1.2/src/stats.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-02-29 20:26:01.000000 gseapy-1.1.2/src/utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 20:26:18.114448 gseapy-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-02-29 20:26:01.000000 gseapy-1.1.2/tests/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:06:28.526145 gseapy-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-08 18:06:13.000000 gseapy-1.1.3/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-08 18:06:13.000000 gseapy-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 18:06:13.000000 gseapy-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11493 2024-05-08 18:06:28.526145 gseapy-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-05-08 18:06:13.000000 gseapy-1.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:06:28.526145 gseapy-1.1.3/gseapy/
+-rw-r--r--   0 runner    (1001) docker     (127)    29495 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28866 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27980 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32042 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/biomart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:06:28.526145 gseapy-1.1.3/gseapy/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    30869 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/data/palette.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23542 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/enrichr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24362 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/gsea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/gsva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/msigdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57946 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/scipalette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/ssgsea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-08 18:06:13.000000 gseapy-1.1.3/gseapy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:06:28.526145 gseapy-1.1.3/gseapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11493 2024-05-08 18:06:28.000000 gseapy-1.1.3/gseapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-08 18:06:28.000000 gseapy-1.1.3/gseapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:06:28.000000 gseapy-1.1.3/gseapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 18:06:28.000000 gseapy-1.1.3/gseapy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:06:28.000000 gseapy-1.1.3/gseapy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 18:06:28.000000 gseapy-1.1.3/gseapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 18:06:28.000000 gseapy-1.1.3/gseapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-08 18:06:13.000000 gseapy-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-08 18:06:13.000000 gseapy-1.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:06:28.526145 gseapy-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-08 18:06:13.000000 gseapy-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:06:28.526145 gseapy-1.1.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-05-08 18:06:13.000000 gseapy-1.1.3/src/algorithm.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    13423 2024-05-08 18:06:13.000000 gseapy-1.1.3/src/gsva.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-08 18:06:13.000000 gseapy-1.1.3/src/help.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-08 18:06:13.000000 gseapy-1.1.3/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    42194 2024-05-08 18:06:13.000000 gseapy-1.1.3/src/stats.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-08 18:06:13.000000 gseapy-1.1.3/src/utils.rs
```

### Comparing `gseapy-1.1.2/Cargo.toml` & `gseapy-1.1.3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/LICENSE` & `gseapy-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/PKG-INFO` & `gseapy-1.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gseapy
-Version: 1.1.2
+Version: 1.1.3
 Summary: Gene Set Enrichment Analysis in Python
 Home-page: https://github.com/zqfang/gseapy
 Download-URL: https://github.com/zqfang/gseapy
 Author: Zhuoqing Fang
 Author-email: fzq518@gmail.com
 License: MIT
 Project-URL: Documentation, https://gseapy.readthedocs.io/en/latest/
@@ -19,19 +19,14 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: numpy>=1.13.0
-Requires-Dist: scipy
-Requires-Dist: pandas
-Requires-Dist: matplotlib>=2.2
-Requires-Dist: requests
 
 
 GSEApy
 ========
 
 GSEApy: Gene Set Enrichment Analysis in Python.
 ------------------------------------------------
```

### Comparing `gseapy-1.1.2/README.rst` & `gseapy-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/gseapy/__init__.py` & `gseapy-1.1.3/gseapy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     :param int min_size: Minimum allowed number of genes from gene set also the data set. Default: 15.
 
     :param int max_size: Maximum allowed number of genes from gene set also the data set. Default: 500.
 
     :param float weight: Refer to :func:`algorithm.enrichment_score`. Default:1.
 
-    :param method:  The method used to calculate a correlation or ranking. Default: 'log2_ratio_of_classes'.
+    :param method:  The method used to calculate a correlation or ranking. Default: 'signal_to_noise'.
                    Others methods are:
 
                    1. 'signal_to_noise'
 
                       You must have at least three samples for each phenotype to use this metric.
                       The larger the signal-to-noise ratio, the larger the differences of the means
                       (scaled by the standard deviations); that is, the more distinct
```

### Comparing `gseapy-1.1.2/gseapy/__main__.py` & `gseapy-1.1.3/gseapy/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Main function
 # ------------------------------------
 
 # there is a bug in add_argument(required=True), for hacking, don't set metavar='' when required=True,
 # or args = argparser.parse_args() will throw bugs!!!
 
 
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 
 
 def main():
     """The Main function/pipeline for GSEApy."""
 
     # Parse options...
     argparser = prepare_argparser()
```

### Comparing `gseapy-1.1.2/gseapy/algorithm.py` & `gseapy-1.1.3/gseapy/algorithm.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/gseapy/base.py` & `gseapy-1.1.3/gseapy/base.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/gseapy/biomart.py` & `gseapy-1.1.3/gseapy/biomart.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/gseapy/data/palette.json` & `gseapy-1.1.3/gseapy/data/palette.json`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/gseapy/enrichr.py` & `gseapy-1.1.3/gseapy/enrichr.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/gseapy/gsea.py` & `gseapy-1.1.3/gseapy/gsea.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,22 +61,26 @@
         self.ascending = ascending
         self.figsize = figsize
         self.format = format
         self.graph_num = int(graph_num)
         self.seed = seed
         self.ranking = None
         self._noplot = no_plot
+        # some preprocessing
+        assert self.permutation_type in ["phenotype", "gene_set"]
+        assert self.min_size <= self.max_size
         # phenotype labels parsing
         self.load_classes(classes)
 
     def load_data(self) -> Tuple[pd.DataFrame, Dict]:
         """pre-processed the data frame.new filtering methods will be implement here."""
         exprs = self._load_data(self.data)
         exprs = self._check_data(exprs)
         exprs, cls_dict = self._filter_data(exprs)
+
         return exprs, cls_dict
 
     def _map_classes(self, sample_names: List[str]) -> Dict[str, Any]:
         """
         update
         """
         cls_dict = self.groups
@@ -94,21 +98,29 @@
         # in case the description column is numeric
         if len(self.groups) == (df.shape[1] - 1):
             df = df.iloc[:, 1:]
         cls_dict = self._map_classes(df.columns)
         # drop gene which std == 0 in all samples
         # compatible to py3.7
         major, minor, _ = [int(i) for i in pd.__version__.split(".")]
+        # handle cases for samples < 3, use mean
         if (major == 1 and minor < 5) or (major < 1):
             # fix numeric_only error
-            df_std = df.groupby(by=cls_dict, axis=1).std()
+            df_std = df.groupby(by=cls_dict, axis=1).std(ddof=0)
         else:
-            df_std = df.groupby(by=cls_dict, axis=1).std(numeric_only=True)
-        df = df[df_std.sum(axis=1) > 0]
-        df = df + 1e-08  # we don't like zeros!!!
+            df_std = df.groupby(by=cls_dict, axis=1).std(numeric_only=True, ddof=0)
+
+        # remove rows that are all zeros !
+        df = df.loc[df.abs().sum(axis=1) > 0, :]
+        # remove rows that std are zeros for sample size >= 3 in each group
+        if all(map(lambda a: a[1] >= 3, Counter(cls_dict.values()).items())):
+            df = df[df_std.abs().sum(axis=1) > 0]
+        df = df + 1e-08  # we don't like zeros in denominator !!!
+        # data frame must have length > 1
+        assert df.shape[0] > 1
 
         return df, cls_dict
 
     def calc_metric(
         self,
         df: pd.DataFrame,
         method: str,
@@ -184,73 +196,85 @@
             )
         elif method == "ratio_of_classes":
             ser = df_mean[pos] / df_mean[neg]
         elif method == "diff_of_classes":
             ser = df_mean[pos] - df_mean[neg]
         elif method == "log2_ratio_of_classes":
             ser = np.log2(df_mean[pos] / df_mean[neg])
+            if ser.isna().sum() > 0:
+                self._logger.warning("Invalid value encountered in log2, and dumped.")
+                ser = ser.dropna()
+                assert len(ser) > 1
         else:
             logging.error("Please provide correct method name!!!")
             raise LookupError("Input method: %s is not supported" % method)
         ser_ind = ser.values.argsort().tolist()
         ser = ser.iloc[ser_ind]
         if ascending:
             return ser_ind, ser
         # descending order
         return ser_ind[::-1], ser[::-1]
 
+    def _check_classes(self, counter: Counter) -> List[str]:
+        """
+        check each cls group length
+        """
+        metrics = ["signal_to_noise", "s2n", "abs_signal_to_noise", "abs_s2n", "t_test"]
+        s = []
+        for c, v in sorted(counter.items(), key=lambda item: item[1]):
+            if v < 3:
+                if self.permutation_type == "phenotype":
+                    self._logger.warning(
+                        f"Number of {c}: {v}, it must be >= 3 for permutation type: phenotype !"
+                    )
+                    self._logger.warning("Permutation type change to gene_set.")
+                    self.permutation_type == "gene_set"
+            s.append(c)
+        return s
+
     def load_classes(self, classes: Union[str, List[str], Dict[str, Any]]):
         """Parse group (classes)"""
         if isinstance(classes, dict):
             # check number of samples
-            class_values = Counter(classes.values())
-            s = []
-            for c, v in sorted(class_values.items(), key=lambda item: item[1]):
-                if v < 3:
-                    raise Exception(f"Number of {c}: {v}, it must be >= 3!")
-                s.append(c)
+            s = self._check_classes(Counter(classes.values()))
             self.pheno_pos = s[0]
             self.pheno_neg = s[1]
             # n_pos = class_values[pos]
             # n_neg = class_values[neg]
             self.groups = classes
         else:
             pos, neg, cls_vector = gsea_cls_parser(classes)
+            s = self._check_classes(Counter(cls_vector))
             self.pheno_pos = pos
             self.pheno_neg = neg
             self.groups = cls_vector
 
     # @profile
     def run(self):
         """GSEA main procedure"""
         m = self.method.lower()
         if m in ["signal_to_noise", "s2n"]:
             method = Metric.Signal2Noise
-        elif m in ["s2n", "abs_signal_to_noise", "abs_s2n"]:
+        elif m in ["abs_signal_to_noise", "abs_s2n"]:
             method = Metric.AbsSignal2Noise
         elif m == "t_test":
             method = Metric.Ttest
         elif m == "ratio_of_classes":
             method = Metric.RatioOfClasses
         elif m == "diff_of_classes":
             method = Metric.DiffOfClasses
         elif m == "log2_ratio_of_classes":
             method = Metric.Log2RatioOfClasses
         else:
             raise Exception("Sorry, input method %s is not supported" % m)
 
-        assert self.permutation_type in ["phenotype", "gene_set"]
-        assert self.min_size <= self.max_size
-
         # Start Analysis
         self._logger.info("Parsing data files for GSEA.............................")
         # select correct expression genes and values.
         dat, cls_dict = self.load_data()
-        # data frame must have length > 1
-        assert len(dat) > 1
         # filtering out gene sets and build gene sets dictionary
         gmt = self.load_gmt(gene_list=dat.index.values, gmt=self.gene_sets)
         self.gmt = gmt
         self._logger.info(
             "%04d gene_sets used for further statistical testing....." % len(gmt)
         )
         self._logger.info("Start to run GSEA...Might take a while..................")
```

### Comparing `gseapy-1.1.2/gseapy/gsva.py` & `gseapy-1.1.3/gseapy/gsva.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/gseapy/msigdb.py` & `gseapy-1.1.3/gseapy/msigdb.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/gseapy/parser.py` & `gseapy-1.1.3/gseapy/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 import json
 import logging
 import os
 import xml.etree.ElementTree as ET
-from collections import Counter
 from collections.abc import Iterable
 from typing import Dict, List, Optional, Tuple, Union
 
 import requests
 
 from gseapy.utils import DEFAULT_CACHE_PATH, unique
 
@@ -38,18 +37,14 @@
                     classes[i] = sample_name[1]
     else:
         raise Exception("Error parsing sample name!")
 
     if len(sample_name) != 2:
         raise Exception("Input groups have to be 2!")
 
-    for c, v in Counter(classes).items():
-        if v < 3:
-            raise Exception(f"Number of {c}: {v}, it must be >= 3!")
-
     return sample_name[0], sample_name[1], classes
 
 
 def gsea_edb_parser(results_path: str) -> Dict[str, List[str]]:
     """Parse results.edb file stored under **edb** file folder.
 
     :param results_path: the path of results.edb file.
```

### Comparing `gseapy-1.1.2/gseapy/plot.py` & `gseapy-1.1.3/gseapy/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -656,50 +656,60 @@
             return False
         else:
             return True
 
     def process(self, df: pd.DataFrame):
         # check if any values in `df[colname]` can't be coerced to floats
         can_be_coerced = df[self.colname].map(self.isfloat).sum()
-        if can_be_coerced < len(df):
+        if can_be_coerced < df.shape[0]:
             msg = "some value in %s could not be typecast to `float`" % self.colname
             raise ValueError(msg)
         # subset
         mask = df[self.colname] <= self.thresh
         if self.colname in ["Combined Score", "NES", "ES", "Odds Ratio"]:
             mask.loc[:] = True
 
         df = df.loc[mask]
-        if len(df) < 1:
+        if df.shape[0] < 1:
             msg = "Warning: No enrich terms when cutoff = %s" % self.thresh
             raise ValueError(msg)
         self.cbar_title = self.colname
         # clip GSEA lower bounds
         # if self.colname in ["NOM p-val", "FDR q-val"]:
         #     df[self.colname].clip(1e-5, 1.0, inplace=True)
         # sorting the dataframe for better visualization
         colnd = {
             "Adjusted P-value": "FDR",
             "P-value": "Pval",
             "NOM p-val": "Pval",
             "FDR q-val": "FDR",
         }
+        ## impute the 0s in pval, fdr for visualization purpose
         if self.colname in ["Adjusted P-value", "P-value", "NOM p-val", "FDR q-val"]:
-            # get top_terms
+            # if all values are zeros, raise error
+            if not any(df[self.colname].abs() > 0):
+                raise ValueError(
+                    f"Can not detetermine colormap. All values in {self.colname} are 0s"
+                )
             df = df.sort_values(by=self.colname)
             df[self.colname].replace(
                 0, method="bfill", inplace=True
             )  ## asending order, use bfill
             df = df.assign(p_inv=np.log10(1 / df[self.colname].astype(float)))
             _t = colnd[self.colname]
             self.colname = "p_inv"
             self.cbar_title = r"$\log_{10} \frac{1}{ " + _t + " }$"
 
         # get top terms; sort ascending
-        if (self.x is not None) and (self.x in df.columns):
+        if (
+            (self.x is not None)
+            and (self.x in df.columns)
+            and (not all(df[self.x].map(self.isfloat)))
+        ):
+            # if x is numeric column
             # get top term of each group
             df = (
                 df.groupby(self.x)
                 .apply(lambda _x: _x.sort_values(by=self.colname).tail(self.n_terms))
                 .reset_index(drop=True)
             )
         else:
@@ -824,15 +834,18 @@
         vmax = np.percentile(colmap.max(), 98)
         # vmin = np.percentile(df.colmap.min(), 2)
         # vmax = np.percentile(df.colmap.max(), 98)
         ax = self.get_ax()
         # if self.x is None:
         x, xlabel = self.set_x()
         y = self.y
-        # set x, y order
+        # if x axis is numberic, prettifiy the plot with the numberic order
+        if all(df[x].map(self.isfloat)):
+            df = df.sort_values(by=x)
+        # set x, y order if set
         xunits = UnitData(self.get_x_order()) if self.x_order else None
         yunits = UnitData(self.get_y_order()) if self.y_order else None
 
         # outer ring
         if outer_ring:
             smax = df["area"].max()
             # TODO:
@@ -1128,15 +1141,15 @@
     :param x_order: bool, array-like list. Default: False.
                     If True, peformed hierarchical_clustering on Y-axis.
                     or input a array-like list of `y` categorical levels.
 
     :param title: Figure title.
     :param cutoff: Terms with `column` value < cut-off are shown. Work only for
                    ("Adjusted P-value", "P-value", "NOM p-val", "FDR q-val")
-    :param top_term: Number of enriched terms to show.
+    :param top_term: Number of enriched terms to show (based on values in the `column` (colormap)).
     :param size: float, scale the dot size to get proper visualization.
     :param figsize: tuple, matplotlib figure size.
     :param cmap: Matplotlib colormap for mapping the `column` semantic.
     :param ofname: Output file name. If None, don't save figure
     :param marker: The matplotlib.markers. See https://matplotlib.org/stable/api/markers_api.html
     :param show_ring bool: Whether to draw outer ring.
```

### Comparing `gseapy-1.1.2/gseapy/scipalette.py` & `gseapy-1.1.3/gseapy/scipalette.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/gseapy/ssgsea.py` & `gseapy-1.1.3/gseapy/ssgsea.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/gseapy/stats.py` & `gseapy-1.1.3/gseapy/stats.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/gseapy/utils.py` & `gseapy-1.1.3/gseapy/utils.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/gseapy.egg-info/PKG-INFO` & `gseapy-1.1.3/gseapy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gseapy
-Version: 1.1.2
+Version: 1.1.3
 Summary: Gene Set Enrichment Analysis in Python
 Home-page: https://github.com/zqfang/gseapy
 Download-URL: https://github.com/zqfang/gseapy
 Author: Zhuoqing Fang
 Author-email: fzq518@gmail.com
 License: MIT
 Project-URL: Documentation, https://gseapy.readthedocs.io/en/latest/
@@ -19,19 +19,14 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: numpy>=1.13.0
-Requires-Dist: scipy
-Requires-Dist: pandas
-Requires-Dist: matplotlib>=2.2
-Requires-Dist: requests
 
 
 GSEApy
 ========
 
 GSEApy: Gene Set Enrichment Analysis in Python.
 ------------------------------------------------
```

### Comparing `gseapy-1.1.2/gseapy.egg-info/SOURCES.txt` & `gseapy-1.1.3/gseapy.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -29,9 +29,8 @@
 gseapy.egg-info/top_level.txt
 gseapy/data/palette.json
 src/algorithm.rs
 src/gsva.rs
 src/help.rs
 src/lib.rs
 src/stats.rs
-src/utils.rs
-tests/test_commands.py
+src/utils.rs
```

### Comparing `gseapy-1.1.2/setup.py` & `gseapy-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/src/algorithm.rs` & `gseapy-1.1.3/src/algorithm.rs`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/src/gsva.rs` & `gseapy-1.1.3/src/gsva.rs`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/src/help.rs` & `gseapy-1.1.3/src/help.rs`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/src/lib.rs` & `gseapy-1.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/src/stats.rs` & `gseapy-1.1.3/src/stats.rs`

 * *Files identical despite different names*

### Comparing `gseapy-1.1.2/src/utils.rs` & `gseapy-1.1.3/src/utils.rs`

 * *Files identical despite different names*

