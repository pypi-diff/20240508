# Comparing `tmp/pytest-ranking-0.2.7.tar.gz` & `tmp/pytest_ranking-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-ranking-0.2.7.tar", last modified: Mon Mar 18 19:06:47 2024, max compression
+gzip compressed data, was "pytest_ranking-0.2.8.tar", last modified: Wed May  8 19:57:30 2024, max compression
```

## Comparing `pytest-ranking-0.2.7.tar` & `pytest_ranking-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-03-18 19:06:47.225151 pytest-ranking-0.2.7/
--rw-r--r--   0 samcheng   (501) staff       (20)     1091 2023-12-04 16:30:45.000000 pytest-ranking-0.2.7/LICENSE
--rw-r--r--   0 samcheng   (501) staff       (20)       96 2024-02-17 03:47:33.000000 pytest-ranking-0.2.7/MANIFEST.in
--rw-r--r--   0 samcheng   (501) staff       (20)     6000 2024-03-18 19:06:47.224940 pytest-ranking-0.2.7/PKG-INFO
--rw-r--r--   0 samcheng   (501) staff       (20)     4519 2024-03-18 19:06:13.000000 pytest-ranking-0.2.7/README.md
--rw-r--r--   0 samcheng   (501) staff       (20)       38 2024-03-18 19:06:47.225198 pytest-ranking-0.2.7/setup.cfg
--rw-r--r--   0 samcheng   (501) staff       (20)     2211 2024-03-18 18:59:05.000000 pytest-ranking-0.2.7/setup.py
-drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-03-18 19:06:47.222793 pytest-ranking-0.2.7/src/
-drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-03-18 19:06:47.223783 pytest-ranking-0.2.7/src/pytest_ranking/
--rw-r--r--   0 samcheng   (501) staff       (20)       22 2024-02-17 03:49:46.000000 pytest-ranking-0.2.7/src/pytest_ranking/__init__.py
--rw-r--r--   0 samcheng   (501) staff       (20)    10244 2024-03-18 19:03:30.000000 pytest-ranking-0.2.7/src/pytest_ranking/plugin.py
--rw-r--r--   0 samcheng   (501) staff       (20)      191 2024-03-18 19:00:42.000000 pytest-ranking-0.2.7/src/pytest_ranking/plugin_utils.py
--rw-r--r--   0 samcheng   (501) staff       (20)     2658 2024-02-17 03:50:57.000000 pytest-ranking-0.2.7/src/pytest_ranking/relate.py
-drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-03-18 19:06:47.224739 pytest-ranking-0.2.7/src/pytest_ranking.egg-info/
--rw-r--r--   0 samcheng   (501) staff       (20)     6000 2024-03-18 19:06:47.000000 pytest-ranking-0.2.7/src/pytest_ranking.egg-info/PKG-INFO
--rw-r--r--   0 samcheng   (501) staff       (20)      445 2024-03-18 19:06:47.000000 pytest-ranking-0.2.7/src/pytest_ranking.egg-info/SOURCES.txt
--rw-r--r--   0 samcheng   (501) staff       (20)        1 2024-03-18 19:06:47.000000 pytest-ranking-0.2.7/src/pytest_ranking.egg-info/dependency_links.txt
--rw-r--r--   0 samcheng   (501) staff       (20)       50 2024-03-18 19:06:47.000000 pytest-ranking-0.2.7/src/pytest_ranking.egg-info/entry_points.txt
--rw-r--r--   0 samcheng   (501) staff       (20)       20 2024-03-18 19:06:47.000000 pytest-ranking-0.2.7/src/pytest_ranking.egg-info/requires.txt
--rw-r--r--   0 samcheng   (501) staff       (20)       15 2024-03-18 19:06:47.000000 pytest-ranking-0.2.7/src/pytest_ranking.egg-info/top_level.txt
-drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-03-18 19:06:47.224572 pytest-ranking-0.2.7/tests/
--rw-r--r--   0 samcheng   (501) staff       (20)    14006 2024-03-18 19:03:40.000000 pytest-ranking-0.2.7/tests/test_pytest_ranking.py
+drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-05-08 19:57:30.445850 pytest_ranking-0.2.8/
+-rw-r--r--   0 samcheng   (501) staff       (20)     1091 2023-12-04 16:30:45.000000 pytest_ranking-0.2.8/LICENSE
+-rw-r--r--   0 samcheng   (501) staff       (20)       96 2024-02-17 03:47:33.000000 pytest_ranking-0.2.8/MANIFEST.in
+-rw-r--r--   0 samcheng   (501) staff       (20)     6257 2024-05-08 19:57:30.445495 pytest_ranking-0.2.8/PKG-INFO
+-rw-r--r--   0 samcheng   (501) staff       (20)     4776 2024-05-07 18:44:25.000000 pytest_ranking-0.2.8/README.md
+-rw-r--r--   0 samcheng   (501) staff       (20)       38 2024-05-08 19:57:30.445915 pytest_ranking-0.2.8/setup.cfg
+-rw-r--r--   0 samcheng   (501) staff       (20)     2211 2024-05-08 19:55:39.000000 pytest_ranking-0.2.8/setup.py
+drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-05-08 19:57:30.441677 pytest_ranking-0.2.8/src/
+drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-05-08 19:57:30.443455 pytest_ranking-0.2.8/src/pytest_ranking/
+-rw-r--r--   0 samcheng   (501) staff       (20)       22 2024-02-17 03:49:46.000000 pytest_ranking-0.2.8/src/pytest_ranking/__init__.py
+-rw-r--r--   0 samcheng   (501) staff       (20)     2739 2024-05-08 16:51:24.000000 pytest_ranking-0.2.8/src/pytest_ranking/change_tracker.py
+-rw-r--r--   0 samcheng   (501) staff       (20)    10555 2024-05-08 19:54:23.000000 pytest_ranking-0.2.8/src/pytest_ranking/plugin.py
+-rw-r--r--   0 samcheng   (501) staff       (20)      191 2024-05-08 19:54:27.000000 pytest_ranking-0.2.8/src/pytest_ranking/plugin_utils.py
+drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-05-08 19:57:30.445155 pytest_ranking-0.2.8/src/pytest_ranking.egg-info/
+-rw-r--r--   0 samcheng   (501) staff       (20)     6257 2024-05-08 19:57:30.000000 pytest_ranking-0.2.8/src/pytest_ranking.egg-info/PKG-INFO
+-rw-r--r--   0 samcheng   (501) staff       (20)      453 2024-05-08 19:57:30.000000 pytest_ranking-0.2.8/src/pytest_ranking.egg-info/SOURCES.txt
+-rw-r--r--   0 samcheng   (501) staff       (20)        1 2024-05-08 19:57:30.000000 pytest_ranking-0.2.8/src/pytest_ranking.egg-info/dependency_links.txt
+-rw-r--r--   0 samcheng   (501) staff       (20)       50 2024-05-08 19:57:30.000000 pytest_ranking-0.2.8/src/pytest_ranking.egg-info/entry_points.txt
+-rw-r--r--   0 samcheng   (501) staff       (20)       20 2024-05-08 19:57:30.000000 pytest_ranking-0.2.8/src/pytest_ranking.egg-info/requires.txt
+-rw-r--r--   0 samcheng   (501) staff       (20)       15 2024-05-08 19:57:30.000000 pytest_ranking-0.2.8/src/pytest_ranking.egg-info/top_level.txt
+drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-05-08 19:57:30.444614 pytest_ranking-0.2.8/tests/
+-rw-r--r--   0 samcheng   (501) staff       (20)    14016 2024-05-07 21:07:06.000000 pytest_ranking-0.2.8/tests/test_pytest_ranking.py
```

### Comparing `pytest-ranking-0.2.7/LICENSE` & `pytest_ranking-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-ranking-0.2.7/PKG-INFO` & `pytest_ranking-0.2.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ranking
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Pytest plugin for automatically prioritizing/ranking tests to speed up failure detection
 Home-page: https://github.com/softwareTestingResearch/pytest-ranking
 Author: softwareTestingResearch
 Author-email: testingresearch4all@gmail.com
 Maintainer: softwareTestingResearch
 Maintainer-email: testingresearch4all@gmail.com
 License: MIT
@@ -69,33 +69,51 @@
 [pytest-ranking] Weights: 1-1-0
 [pytest-ranking] History length: 30
 [pytest-ranking] Number of files with new hashes: 0
 [pytest-ranking] Change relatedness computation time (s): 0.0007872581481933594
 [pytest-ranking] Test order computation time(s): 0.00020933151245117188
 ```
 
+
+### Weighting ranking heuristics
+
 You can configure the weights of different prioritization heuristics by passing the optional `--rank-weight` flag with formatted values:
 
 ```bash
 pytest --rank --rank-weight=0-1-0
 ```
 
 Weights are separated by ``-``. The 1st weight is for running faster tests, the 2nd weight is for running recently failed tests, and the 3rd weight is for running tests related to the changed `*.py` files in the codebase since the last run.
 All weights must be integers or floats, and their sum will be normalized to 1.
 A higher weight means that a corresponding heuristic is favored. The default value is ``1-0-0``, only prioritizes faster tests.
 
 
+### Tracking heuristics from historical runs
+
 You can also configure the maximum window size for looking into previous test runs, which is used to compute the number of runs since a test had failed, by passing the optional `--rank-hist-len` flag (the default value is 50):
 
 ```bash
 pytest --rank --rank-hist-len=30
 ```
 
+Note that the plugin does not store any historical run logs, it merely resets cached ranking heuristics after every `rank-hist-len` number of runs.
+
+### Running tests in random order
+
+You can prompt `pytest-ranking` to run tests in random order, via setting the sum of `--rank-weight` option to 0, e.g., `--rank-weight=0-0-0`.
+You can also configure the seed used when running tests in random order, via setting an integer to the option `--rank-seed`.
+For example, the command below runs tests randomly with seed `1234`:
+
+```bash
+pytest --rank --rank-weight=0-0-0 --rank-seed=1234
+```
 
-You can always apply these options by adding them to the ``addopts`` setting in your [pytest.ini](https://docs.pytest.org/en/latest/reference/customize.html#configuration).
+### Passing plugin options via config file
+
+You can always apply available options by adding them to the ``addopts`` setting in your [pytest.ini](https://docs.pytest.org/en/latest/reference/customize.html#configuration).
 
 For example, create `pytest.ini` in your codebase root folder as such:
 ```ini
 [pytest]
 addopts = --rank --rank-weight=0-1-0 --rank-hist-len=30
 ```
 and run `pytest` on command line.
@@ -106,29 +124,18 @@
 rank_weight=0-1-0
 rank_hist_len=30
 ```
 
 and run `pytest --rank` on command line.
 
 
-### Running tests in random order
-
-You can prompt `pytest-ranking` to run tests in random order, via setting the sum of `--rank-weight` option to 0, e.g., `--rank-weight=0-0-0`.
-You can also configure the seed used when running tests in random order, via setting an integer to the option `--rank-seed`.
-For example, the command below runs tests randomly with seed `1234`:
-
-```bash
-pytest --rank --rank-weight=0-0-0 --rank-seed=1234
-```
-
-
-### Warning
 
-Because `pytest-ranking` re-orders tests to speed up failure detection time, please disable other pytest plugins that enforeces other test orders, e.g., [pytest-randomly](https://github.com/pytest-dev/pytest-randomly), [pytest-random-order](https://github.com/pytest-dev/pytest-random-order), [pytest-reverse](https://github.com/adamchainz/pytest-reverse).
+### Compatibility
 
+Because `pytest-ranking` re-orders tests, it is not compatible with other pytest plugins that enforece other test orders, e.g., [pytest-randomly](https://github.com/pytest-dev/pytest-randomly), [pytest-random-order](https://github.com/pytest-dev/pytest-random-order), [pytest-reverse](https://github.com/adamchainz/pytest-reverse).
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox](https://tox.readthedocs.io/en/latest/).
```

### Comparing `pytest-ranking-0.2.7/README.md` & `pytest_ranking-0.2.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -35,33 +35,51 @@
 [pytest-ranking] Weights: 1-1-0
 [pytest-ranking] History length: 30
 [pytest-ranking] Number of files with new hashes: 0
 [pytest-ranking] Change relatedness computation time (s): 0.0007872581481933594
 [pytest-ranking] Test order computation time(s): 0.00020933151245117188
 ```
 
+
+### Weighting ranking heuristics
+
 You can configure the weights of different prioritization heuristics by passing the optional `--rank-weight` flag with formatted values:
 
 ```bash
 pytest --rank --rank-weight=0-1-0
 ```
 
 Weights are separated by ``-``. The 1st weight is for running faster tests, the 2nd weight is for running recently failed tests, and the 3rd weight is for running tests related to the changed `*.py` files in the codebase since the last run.
 All weights must be integers or floats, and their sum will be normalized to 1.
 A higher weight means that a corresponding heuristic is favored. The default value is ``1-0-0``, only prioritizes faster tests.
 
 
+### Tracking heuristics from historical runs
+
 You can also configure the maximum window size for looking into previous test runs, which is used to compute the number of runs since a test had failed, by passing the optional `--rank-hist-len` flag (the default value is 50):
 
 ```bash
 pytest --rank --rank-hist-len=30
 ```
 
+Note that the plugin does not store any historical run logs, it merely resets cached ranking heuristics after every `rank-hist-len` number of runs.
+
+### Running tests in random order
+
+You can prompt `pytest-ranking` to run tests in random order, via setting the sum of `--rank-weight` option to 0, e.g., `--rank-weight=0-0-0`.
+You can also configure the seed used when running tests in random order, via setting an integer to the option `--rank-seed`.
+For example, the command below runs tests randomly with seed `1234`:
+
+```bash
+pytest --rank --rank-weight=0-0-0 --rank-seed=1234
+```
 
-You can always apply these options by adding them to the ``addopts`` setting in your [pytest.ini](https://docs.pytest.org/en/latest/reference/customize.html#configuration).
+### Passing plugin options via config file
+
+You can always apply available options by adding them to the ``addopts`` setting in your [pytest.ini](https://docs.pytest.org/en/latest/reference/customize.html#configuration).
 
 For example, create `pytest.ini` in your codebase root folder as such:
 ```ini
 [pytest]
 addopts = --rank --rank-weight=0-1-0 --rank-hist-len=30
 ```
 and run `pytest` on command line.
@@ -72,29 +90,18 @@
 rank_weight=0-1-0
 rank_hist_len=30
 ```
 
 and run `pytest --rank` on command line.
 
 
-### Running tests in random order
-
-You can prompt `pytest-ranking` to run tests in random order, via setting the sum of `--rank-weight` option to 0, e.g., `--rank-weight=0-0-0`.
-You can also configure the seed used when running tests in random order, via setting an integer to the option `--rank-seed`.
-For example, the command below runs tests randomly with seed `1234`:
-
-```bash
-pytest --rank --rank-weight=0-0-0 --rank-seed=1234
-```
-
-
-### Warning
 
-Because `pytest-ranking` re-orders tests to speed up failure detection time, please disable other pytest plugins that enforeces other test orders, e.g., [pytest-randomly](https://github.com/pytest-dev/pytest-randomly), [pytest-random-order](https://github.com/pytest-dev/pytest-random-order), [pytest-reverse](https://github.com/adamchainz/pytest-reverse).
+### Compatibility
 
+Because `pytest-ranking` re-orders tests, it is not compatible with other pytest plugins that enforece other test orders, e.g., [pytest-randomly](https://github.com/pytest-dev/pytest-randomly), [pytest-random-order](https://github.com/pytest-dev/pytest-random-order), [pytest-reverse](https://github.com/adamchainz/pytest-reverse).
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox](https://tox.readthedocs.io/en/latest/).
```

### Comparing `pytest-ranking-0.2.7/setup.py` & `pytest_ranking-0.2.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pytest-ranking',
-    version='0.2.7',
+    version='0.2.8',
     author='softwareTestingResearch',
     author_email='testingresearch4all@gmail.com',
     maintainer='softwareTestingResearch',
     maintainer_email='testingresearch4all@gmail.com',
     license='MIT',
     url='https://github.com/softwareTestingResearch/pytest-ranking',
     description='A Pytest plugin for automatically'
```

### Comparing `pytest-ranking-0.2.7/src/pytest_ranking/plugin.py` & `pytest_ranking-0.2.8/src/pytest_ranking/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 import pytest
 from _pytest.config import Config
 from _pytest.config.argparsing import Parser
 from _pytest.main import Session
 from _pytest.nodes import Item
 from _pytest.reports import TestReport
 
+from .change_tracker import changeTracker
 from .plugin_utils import (DATA_DIR, DEFAULT_HIST_LEN, DEFAULT_SEED,
                            DEFAULT_WEIGHT)
-from .relate import changeRelatedness
 
 PLUGIN_HELP = "Run test-case prioritization algorithm for pytest test suite. "\
     "It re-orders execution of tests to expose test failure sooner. "\
     "Default behavior: runs faster tests first, "\
     "so that more tests are executed per unit time. "\
     "See more customization in the `--rank-weight` option."
 
@@ -112,18 +112,18 @@
 class TCPRunner:
     """Plugin class"""
     def __init__(self, config: Config) -> None:
         self.config = config
         self.test_reports = []
         # for logging runtime overhead, etc
         self.log = {}
-        self.change_rel = changeRelatedness(config)
         self.weights = self.parse_tcp_weights()
         self.hist_len = self.parse_hist_len()
         self.seed = self.parse_seed()
+        self.chgtracker = changeTracker(config)
 
     def parse_tcp_weights(self) -> list[float]:
         """Get weights, non-default CLI overrides ini file input"""
         weights = self.config.getoption("--rank-weight")
         if weights == DEFAULT_WEIGHT:
             ini_val = self.config.getini("rank_weight")
             weights = ini_val if ini_val else weights
@@ -175,51 +175,56 @@
         if transform:
             values = 1 - values
         return values.tolist()
 
     def run_tcp(self, items: list[Item]) -> None:
         """Run test prioritization algorithm"""
         # load code change features
-        num_delta_file, compute_time = self.change_rel.run(items)
-        self.log['Number of files with new hashes'] = num_delta_file
+        self.chgtracker.compute_test_suite_relatedness(items)
+        num_delta_file = self.chgtracker.num_delta_files
+        compute_time = self.chgtracker.overhead
+        self.log['Number of *.py files with new hashes'] = num_delta_file
         self.log['Relatedness computation time (s)'] = compute_time
 
         # start ordering tests
         start_time = time.time()
 
         if self.weights == [0, 0, 0]:
+            # fix input test list order for different workers in pytest-xdist
+            items.sort(key=lambda item: item.nodeid, reverse=True)
+            # randomly order with seed so that all workers have the same order
             random.seed(self.seed)
             random.shuffle(items)
             self.log["Test order is set to random with seed"] = self.seed
         else:
             w_time, w_fail, w_rel = self.weights
             h_time = self.load_feature_data("last_durations", items, True)
             h_fail = self.load_feature_data("num_runs_since_fail", items, True)
             h_rel = self.load_feature_data("change_relatedness", items, False)
 
             def rank(i):
                 s = h_time[i] * w_time + h_fail[i] * w_fail + h_rel[i] * w_rel
                 return s
 
             # assign priority score to each test by weighted sum
-            # tests with higher priority score are run first: descending sort
+            # tests with higher priority score are run first
             # ties are broken by alphabetical order (pytest default)
             scores = {item.nodeid: rank(i) for i, item in enumerate(items)}
             items.sort(
                 key=lambda item: (scores.get(item.nodeid, 0), item.nodeid),
                 reverse=True)
 
         # log time to compute test order
         self.log["Test order computation time (s)"] = time.time() - start_time
 
     def pytest_runtest_logreport(self, report: TestReport) -> None:
         """Record test result of each executed test case"""
         if not report.skipped and report.when == "call":
             # no skipped: only look at the executed test
-            # called: only look at called duration (ignore setup/teardown)
+            # call: only look at called duration (ignore setup/teardown)
             self.test_reports.append(report)
 
     @pytest.hookimpl(trylast=True)
     def pytest_collection_modifyitems(self, items: list[Item]) -> None:
         if self.config.getoption("--rank"):
             self.run_tcp(items)
```

### Comparing `pytest-ranking-0.2.7/src/pytest_ranking/relate.py` & `pytest_ranking-0.2.8/src/pytest_ranking/change_tracker.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,66 +12,68 @@
 from .plugin_utils import DATA_DIR
 
 
 def tokenize(string: str) -> list[str]:
     return re.findall(r'[a-zA-Z0-9]+', string.lower())
 
 
-class changeRelatedness:
+class changeTracker:
     def __init__(self, pytest_config: Config) -> None:
         self.pytest_config = pytest_config
-        self.delta = set()
+        # record overhead
+        self.overhead = 0
+        # get the set of changed files
+        self.get_delta()
 
     def get_all_file_paths(self):
         """Get all file paths in the codebase"""
         pattern = os.path.join(self.pytest_config.rootpath, "**/*.py")
         file_paths = glob.glob(pattern, recursive=True)
         return file_paths
 
     def get_hash(self, file_path):
         """Compute hash for the file"""
         with open(file_path, "rb") as f:
             return hashlib.sha1(f.read()).hexdigest()
 
-    def get_delta(self) -> int:
+    def get_delta(self) -> None:
         """
         Compute hashes for all files,
         get token set for files whose hashes differ or have not been seen,
         those are the changed or new files since last run (delta).
         Save the newest hashes for all files.
-        *Return the number of files to compute hashes
+        *Update the number of files that were re-computed hashes
         """
+        start_time = time.time()
         file_paths = self.get_all_file_paths()
         hashes = {path: self.get_hash(path) for path in file_paths}
 
         key = os.path.join(DATA_DIR, "file_hashes")
         # load file hashes since last run
         old_hashes = self.pytest_config.cache.get(key, {})
         # save newest hashes anyway
         self.pytest_config.cache.set(key, hashes)
 
         # if hashes are computed for the first time
         if old_hashes == {}:
+            self.overhead += time.time() - start_time
             return len(file_paths)
 
         # get files with a different/new hash since last run
-        num_delta_files = 0
+        self.delta = set()
+        self.num_delta_files = 0
         for path, hash in hashes.items():
             if path not in old_hashes or old_hashes[path] != hash:
                 self.delta = self.delta.union(tokenize(path))
-                num_delta_files += 1
-        return num_delta_files
+                self.num_delta_files += 1
+        self.overhead += time.time() - start_time
 
     def compute_test_suite_relatedness(self, items: list[Item]) -> None:
         """Compute and save relatedness to changed files per test"""
+        start_time = time.time()
         ret = {}
         for item in items:
             test_tokens = set(tokenize(item.nodeid))
             ret[item.nodeid] = len(self.delta.intersection(set(test_tokens)))
         key = os.path.join(DATA_DIR, "change_relatedness")
         self.pytest_config.cache.set(key, ret)
-
-    def run(self, items: list[Item]) -> tuple[int, float]:
-        start_time = time.time()
-        num_delta_file = self.get_delta()
-        self.compute_test_suite_relatedness(items)
-        return num_delta_file, time.time() - start_time
+        self.overhead += time.time() - start_time
```

### Comparing `pytest-ranking-0.2.7/src/pytest_ranking.egg-info/PKG-INFO` & `pytest_ranking-0.2.8/src/pytest_ranking.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ranking
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Pytest plugin for automatically prioritizing/ranking tests to speed up failure detection
 Home-page: https://github.com/softwareTestingResearch/pytest-ranking
 Author: softwareTestingResearch
 Author-email: testingresearch4all@gmail.com
 Maintainer: softwareTestingResearch
 Maintainer-email: testingresearch4all@gmail.com
 License: MIT
@@ -69,33 +69,51 @@
 [pytest-ranking] Weights: 1-1-0
 [pytest-ranking] History length: 30
 [pytest-ranking] Number of files with new hashes: 0
 [pytest-ranking] Change relatedness computation time (s): 0.0007872581481933594
 [pytest-ranking] Test order computation time(s): 0.00020933151245117188
 ```
 
+
+### Weighting ranking heuristics
+
 You can configure the weights of different prioritization heuristics by passing the optional `--rank-weight` flag with formatted values:
 
 ```bash
 pytest --rank --rank-weight=0-1-0
 ```
 
 Weights are separated by ``-``. The 1st weight is for running faster tests, the 2nd weight is for running recently failed tests, and the 3rd weight is for running tests related to the changed `*.py` files in the codebase since the last run.
 All weights must be integers or floats, and their sum will be normalized to 1.
 A higher weight means that a corresponding heuristic is favored. The default value is ``1-0-0``, only prioritizes faster tests.
 
 
+### Tracking heuristics from historical runs
+
 You can also configure the maximum window size for looking into previous test runs, which is used to compute the number of runs since a test had failed, by passing the optional `--rank-hist-len` flag (the default value is 50):
 
 ```bash
 pytest --rank --rank-hist-len=30
 ```
 
+Note that the plugin does not store any historical run logs, it merely resets cached ranking heuristics after every `rank-hist-len` number of runs.
+
+### Running tests in random order
+
+You can prompt `pytest-ranking` to run tests in random order, via setting the sum of `--rank-weight` option to 0, e.g., `--rank-weight=0-0-0`.
+You can also configure the seed used when running tests in random order, via setting an integer to the option `--rank-seed`.
+For example, the command below runs tests randomly with seed `1234`:
+
+```bash
+pytest --rank --rank-weight=0-0-0 --rank-seed=1234
+```
 
-You can always apply these options by adding them to the ``addopts`` setting in your [pytest.ini](https://docs.pytest.org/en/latest/reference/customize.html#configuration).
+### Passing plugin options via config file
+
+You can always apply available options by adding them to the ``addopts`` setting in your [pytest.ini](https://docs.pytest.org/en/latest/reference/customize.html#configuration).
 
 For example, create `pytest.ini` in your codebase root folder as such:
 ```ini
 [pytest]
 addopts = --rank --rank-weight=0-1-0 --rank-hist-len=30
 ```
 and run `pytest` on command line.
@@ -106,29 +124,18 @@
 rank_weight=0-1-0
 rank_hist_len=30
 ```
 
 and run `pytest --rank` on command line.
 
 
-### Running tests in random order
-
-You can prompt `pytest-ranking` to run tests in random order, via setting the sum of `--rank-weight` option to 0, e.g., `--rank-weight=0-0-0`.
-You can also configure the seed used when running tests in random order, via setting an integer to the option `--rank-seed`.
-For example, the command below runs tests randomly with seed `1234`:
-
-```bash
-pytest --rank --rank-weight=0-0-0 --rank-seed=1234
-```
-
-
-### Warning
 
-Because `pytest-ranking` re-orders tests to speed up failure detection time, please disable other pytest plugins that enforeces other test orders, e.g., [pytest-randomly](https://github.com/pytest-dev/pytest-randomly), [pytest-random-order](https://github.com/pytest-dev/pytest-random-order), [pytest-reverse](https://github.com/adamchainz/pytest-reverse).
+### Compatibility
 
+Because `pytest-ranking` re-orders tests, it is not compatible with other pytest plugins that enforece other test orders, e.g., [pytest-randomly](https://github.com/pytest-dev/pytest-randomly), [pytest-random-order](https://github.com/pytest-dev/pytest-random-order), [pytest-reverse](https://github.com/adamchainz/pytest-reverse).
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox](https://tox.readthedocs.io/en/latest/).
```

### Comparing `pytest-ranking-0.2.7/tests/test_pytest_ranking.py` & `pytest_ranking-0.2.8/tests/test_pytest_ranking.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 
     # run without tcp
     args = ["-v"]
     out = mytester.runpytest(*args)
     out.assert_outcomes(passed=2, failed=1)
     # should only log feature computation time
     logging_strings = (
-        "[pytest-ranking] Number of files with new hashes",
+        "[pytest-ranking] Number of *.py files with new hashes",
         "[pytest-ranking] Relatedness computation time (s)",
         "[pytest-ranking] Test prioritization weights",
         "[pytest-ranking] Test order computation time (s)",
         "[pytest-ranking] Test prioritization history length"
     )
 
     assert len([x for x in out.outlines if x.startswith(logging_strings)]) == 0
@@ -396,15 +396,15 @@
 
     # run without tcp
     args = ["-v"]
     out = mytester.runpytest(*args)
     out.assert_outcomes(passed=2, failed=1)
     # should only log feature computation time
     logging_strings = (
-        "[pytest-ranking] Number of files with new hashes",
+        "[pytest-ranking] Number of *.py files with new hashes",
         "[pytest-ranking] Relatedness computation time (s)",
         "[pytest-ranking] Test prioritization weights",
         "[pytest-ranking] Test order computation time (s)",
         "[pytest-ranking] Test prioritization history length"
     )
     assert len([x for x in out.outlines if x.startswith(logging_strings)]) == 0
```

