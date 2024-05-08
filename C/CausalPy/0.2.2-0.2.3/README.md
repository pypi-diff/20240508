# Comparing `tmp/CausalPy-0.2.2.tar.gz` & `tmp/CausalPy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CausalPy-0.2.2.tar", last modified: Mon Mar  4 11:32:16 2024, max compression
+gzip compressed data, was "CausalPy-0.2.3.tar", last modified: Tue Apr  9 08:46:41 2024, max compression
```

## Comparing `CausalPy-0.2.2.tar` & `CausalPy-0.2.3.tar`

### file list

```diff
@@ -1,39 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 11:32:16.710038 CausalPy-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 11:32:16.706037 CausalPy-0.2.2/CausalPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26363 2024-03-04 11:32:16.000000 CausalPy-0.2.2/CausalPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-04 11:32:16.000000 CausalPy-0.2.2/CausalPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 11:32:16.000000 CausalPy-0.2.2/CausalPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-04 11:32:16.000000 CausalPy-0.2.2/CausalPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-04 11:32:16.000000 CausalPy-0.2.2/CausalPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-04 11:32:12.000000 CausalPy-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    26363 2024-03-04 11:32:16.710038 CausalPy-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-03-04 11:32:12.000000 CausalPy-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 11:32:16.702037 CausalPy-0.2.2/causalpy/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/custom_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 11:32:16.706037 CausalPy-0.2.2/causalpy/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data/AJR2001.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data/GDP_in_dollars_billions.csv
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data/ancova_generated.csv
--rw-r--r--   0 runner    (1001) docker     (127)    77216 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data/banks.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data/deaths_and_temps_england_wales.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data/did.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data/drinking.csv
--rw-r--r--   0 runner    (1001) docker     (127)    29149 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data/geolift1.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data/its.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data/its_simple.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data/regression_discontinuity.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data/simulate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17645 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data/synthetic_control.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/data_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    52950 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/pymc_experiments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/pymc_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    22937 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/skl_experiments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/skl_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-04 11:32:12.000000 CausalPy-0.2.2/causalpy/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-04 11:32:12.000000 CausalPy-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 11:32:16.710038 CausalPy-0.2.2/setup.cfg
+drwxr-xr-x   0 benjamv    (501) staff       (20)        0 2024-04-09 08:46:41.974318 CausalPy-0.2.3/
+-rw-r--r--   0 benjamv    (501) staff       (20)     8159 2024-04-05 11:25:03.000000 CausalPy-0.2.3/CONTRIBUTING.md
+drwxr-xr-x   0 benjamv    (501) staff       (20)        0 2024-04-09 08:46:41.973011 CausalPy-0.2.3/CausalPy.egg-info/
+-rw-r--r--   0 benjamv    (501) staff       (20)    26467 2024-04-09 08:46:41.000000 CausalPy-0.2.3/CausalPy.egg-info/PKG-INFO
+-rw-r--r--   0 benjamv    (501) staff       (20)     1138 2024-04-09 08:46:41.000000 CausalPy-0.2.3/CausalPy.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamv    (501) staff       (20)        1 2024-04-09 08:46:41.000000 CausalPy-0.2.3/CausalPy.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamv    (501) staff       (20)      445 2024-04-09 08:46:41.000000 CausalPy-0.2.3/CausalPy.egg-info/requires.txt
+-rw-r--r--   0 benjamv    (501) staff       (20)       14 2024-04-09 08:46:41.000000 CausalPy-0.2.3/CausalPy.egg-info/top_level.txt
+-rw-r--r--   0 benjamv    (501) staff       (20)    11357 2022-10-28 10:08:58.000000 CausalPy-0.2.3/LICENSE
+-rw-r--r--   0 benjamv    (501) staff       (20)    26467 2024-04-09 08:46:41.974047 CausalPy-0.2.3/PKG-INFO
+-rw-r--r--   0 benjamv    (501) staff       (20)    11690 2024-04-02 11:20:58.000000 CausalPy-0.2.3/README.md
+drwxr-xr-x   0 benjamv    (501) staff       (20)        0 2024-04-09 08:46:41.966339 CausalPy-0.2.3/causalpy/
+-rw-r--r--   0 benjamv    (501) staff       (20)      337 2023-12-22 13:16:13.000000 CausalPy-0.2.3/causalpy/__init__.py
+-rw-r--r--   0 benjamv    (501) staff       (20)      689 2023-09-28 10:19:48.000000 CausalPy-0.2.3/causalpy/custom_exceptions.py
+drwxr-xr-x   0 benjamv    (501) staff       (20)        0 2024-04-09 08:46:41.971076 CausalPy-0.2.3/causalpy/data/
+-rw-r--r--   0 benjamv    (501) staff       (20)    11868 2023-09-13 14:56:26.000000 CausalPy-0.2.3/causalpy/data/AJR2001.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)    11574 2022-11-30 15:35:27.000000 CausalPy-0.2.3/causalpy/data/GDP_in_dollars_billions.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)       90 2022-11-23 17:12:53.000000 CausalPy-0.2.3/causalpy/data/__init__.py
+-rw-r--r--   0 benjamv    (501) staff       (20)     7852 2023-01-04 11:05:40.000000 CausalPy-0.2.3/causalpy/data/ancova_generated.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)    77216 2022-11-23 10:37:32.000000 CausalPy-0.2.3/causalpy/data/banks.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)     1295 2023-09-28 10:19:48.000000 CausalPy-0.2.3/causalpy/data/datasets.py
+-rw-r--r--   0 benjamv    (501) staff       (20)     7379 2022-12-02 14:17:13.000000 CausalPy-0.2.3/causalpy/data/deaths_and_temps_england_wales.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)     1339 2023-01-04 11:05:40.000000 CausalPy-0.2.3/causalpy/data/did.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)     9109 2023-01-04 11:05:40.000000 CausalPy-0.2.3/causalpy/data/drinking.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)    29149 2023-01-04 11:05:40.000000 CausalPy-0.2.3/causalpy/data/geolift1.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)     4778 2022-10-28 10:08:58.000000 CausalPy-0.2.3/causalpy/data/its.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)     4830 2022-10-28 10:08:58.000000 CausalPy-0.2.3/causalpy/data/its_simple.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)     4520 2022-10-28 10:08:58.000000 CausalPy-0.2.3/causalpy/data/regression_discontinuity.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)    11712 2023-09-28 10:19:48.000000 CausalPy-0.2.3/causalpy/data/simulate_data.py
+-rw-r--r--   0 benjamv    (501) staff       (20)    17645 2022-10-28 17:54:16.000000 CausalPy-0.2.3/causalpy/data/synthetic_control.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)     5282 2024-03-01 16:19:42.000000 CausalPy-0.2.3/causalpy/data_validation.py
+-rw-r--r--   0 benjamv    (501) staff       (20)     1691 2023-09-28 10:19:48.000000 CausalPy-0.2.3/causalpy/plot_utils.py
+-rw-r--r--   0 benjamv    (501) staff       (20)    52936 2024-04-02 11:20:53.000000 CausalPy-0.2.3/causalpy/pymc_experiments.py
+-rw-r--r--   0 benjamv    (501) staff       (20)    12395 2024-04-02 11:20:53.000000 CausalPy-0.2.3/causalpy/pymc_models.py
+-rw-r--r--   0 benjamv    (501) staff       (20)    22987 2024-04-02 11:20:53.000000 CausalPy-0.2.3/causalpy/skl_experiments.py
+-rw-r--r--   0 benjamv    (501) staff       (20)     1825 2023-09-28 10:19:48.000000 CausalPy-0.2.3/causalpy/skl_models.py
+drwxr-xr-x   0 benjamv    (501) staff       (20)        0 2024-04-09 08:46:41.972669 CausalPy-0.2.3/causalpy/tests/
+-rw-r--r--   0 benjamv    (501) staff       (20)        0 2022-11-25 13:01:06.000000 CausalPy-0.2.3/causalpy/tests/__init__.py
+-rw-r--r--   0 benjamv    (501) staff       (20)      368 2023-09-28 10:19:48.000000 CausalPy-0.2.3/causalpy/tests/conftest.py
+-rw-r--r--   0 benjamv    (501) staff       (20)      655 2023-09-28 10:19:48.000000 CausalPy-0.2.3/causalpy/tests/test_data_loading.py
+-rw-r--r--   0 benjamv    (501) staff       (20)    18462 2023-11-09 10:26:25.000000 CausalPy-0.2.3/causalpy/tests/test_integration_pymc_examples.py
+-rw-r--r--   0 benjamv    (501) staff       (20)     5658 2023-09-28 10:19:48.000000 CausalPy-0.2.3/causalpy/tests/test_integration_skl_examples.py
+-rw-r--r--   0 benjamv    (501) staff       (20)     5957 2024-02-05 13:10:54.000000 CausalPy-0.2.3/causalpy/tests/test_pymc_models.py
+-rw-r--r--   0 benjamv    (501) staff       (20)     1192 2024-04-02 11:20:53.000000 CausalPy-0.2.3/causalpy/utils.py
+-rw-r--r--   0 benjamv    (501) staff       (20)       46 2024-04-05 11:37:56.000000 CausalPy-0.2.3/causalpy/version.py
+-rw-r--r--   0 benjamv    (501) staff       (20)     3204 2024-04-05 11:37:56.000000 CausalPy-0.2.3/pyproject.toml
+-rw-r--r--   0 benjamv    (501) staff       (20)       38 2024-04-09 08:46:41.974362 CausalPy-0.2.3/setup.cfg
```

### Comparing `CausalPy-0.2.2/CausalPy.egg-info/PKG-INFO` & `CausalPy-0.2.3/CausalPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CausalPy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Causal inference for quasi-experiments in Python
 Author-email: Ben Vincent <ben.vincent@pymc-labs.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,15 +204,15 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/pymc-labs/CausalPy
 Project-URL: Bug Reports, https://github.com/pymc-labs/CausalPy/issues
 Project-URL: Source, https://github.com/pymc-labs/CausalPy
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: arviz>=0.14.0
 Requires-Dist: graphviz
 Requires-Dist: ipython!=8.7.0
 Requires-Dist: matplotlib>=3.5.3
 Requires-Dist: numpy<1.26.0
@@ -426,15 +426,15 @@
 | $\ldots$  | $\ldots$  | $\ldots$ | $\ldots$  |
 | $t_{N-1}$ | $y_{N-1}$ | True     | $x_{N-1}$ |
 | $t_N$     | $y_N$     | True     | $x_N$     |
 
 
 | Frequentist | Bayesian |
 |--|--|
-| coming soon | ![](https://raw.githubusercontent.com/pymc-labs/CausalPy/main/docs/source/_static/interrupted_time_series_pymc.svg) |
+| ![](https://raw.githubusercontent.com/pymc-labs/CausalPy/main/docs/source/_static/interrupted_time_series_skl.svg) | ![](https://raw.githubusercontent.com/pymc-labs/CausalPy/main/docs/source/_static/interrupted_time_series_pymc.svg) |
 
 > The data, pre-treatment model fit, and counterfactual are plotted (top). The causal impact is shown as a blue shaded region. The Bayesian analysis shows shaded Bayesian credible regions of the model fit and counterfactual. Also shown is the causal impact (middle) and cumulative causal impact (bottom).
 
 ### Instrumental Variable Regression
 
 Instrumental Variable regression is an appropriate technique when you wish to estimate the treatment effect of some variable on another, but are concerned that the treatment variable is endogenous in the system of interest i.e. correlated with the errors. In this case an “instrument” variable can be used in a regression context to disentangle treatment effect due to the threat of confounding due to endogeneity.
```

### Comparing `CausalPy-0.2.2/LICENSE` & `CausalPy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/PKG-INFO` & `CausalPy-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CausalPy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Causal inference for quasi-experiments in Python
 Author-email: Ben Vincent <ben.vincent@pymc-labs.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,15 +204,15 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/pymc-labs/CausalPy
 Project-URL: Bug Reports, https://github.com/pymc-labs/CausalPy/issues
 Project-URL: Source, https://github.com/pymc-labs/CausalPy
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: arviz>=0.14.0
 Requires-Dist: graphviz
 Requires-Dist: ipython!=8.7.0
 Requires-Dist: matplotlib>=3.5.3
 Requires-Dist: numpy<1.26.0
@@ -426,15 +426,15 @@
 | $\ldots$  | $\ldots$  | $\ldots$ | $\ldots$  |
 | $t_{N-1}$ | $y_{N-1}$ | True     | $x_{N-1}$ |
 | $t_N$     | $y_N$     | True     | $x_N$     |
 
 
 | Frequentist | Bayesian |
 |--|--|
-| coming soon | ![](https://raw.githubusercontent.com/pymc-labs/CausalPy/main/docs/source/_static/interrupted_time_series_pymc.svg) |
+| ![](https://raw.githubusercontent.com/pymc-labs/CausalPy/main/docs/source/_static/interrupted_time_series_skl.svg) | ![](https://raw.githubusercontent.com/pymc-labs/CausalPy/main/docs/source/_static/interrupted_time_series_pymc.svg) |
 
 > The data, pre-treatment model fit, and counterfactual are plotted (top). The causal impact is shown as a blue shaded region. The Bayesian analysis shows shaded Bayesian credible regions of the model fit and counterfactual. Also shown is the causal impact (middle) and cumulative causal impact (bottom).
 
 ### Instrumental Variable Regression
 
 Instrumental Variable regression is an appropriate technique when you wish to estimate the treatment effect of some variable on another, but are concerned that the treatment variable is endogenous in the system of interest i.e. correlated with the errors. In this case an “instrument” variable can be used in a regression context to disentangle treatment effect due to the threat of confounding due to endogeneity.
```

### Comparing `CausalPy-0.2.2/README.md` & `CausalPy-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 | $\ldots$  | $\ldots$  | $\ldots$ | $\ldots$  |
 | $t_{N-1}$ | $y_{N-1}$ | True     | $x_{N-1}$ |
 | $t_N$     | $y_N$     | True     | $x_N$     |
 
 
 | Frequentist | Bayesian |
 |--|--|
-| coming soon | ![](https://raw.githubusercontent.com/pymc-labs/CausalPy/main/docs/source/_static/interrupted_time_series_pymc.svg) |
+| ![](https://raw.githubusercontent.com/pymc-labs/CausalPy/main/docs/source/_static/interrupted_time_series_skl.svg) | ![](https://raw.githubusercontent.com/pymc-labs/CausalPy/main/docs/source/_static/interrupted_time_series_pymc.svg) |
 
 > The data, pre-treatment model fit, and counterfactual are plotted (top). The causal impact is shown as a blue shaded region. The Bayesian analysis shows shaded Bayesian credible regions of the model fit and counterfactual. Also shown is the causal impact (middle) and cumulative causal impact (bottom).
 
 ### Instrumental Variable Regression
 
 Instrumental Variable regression is an appropriate technique when you wish to estimate the treatment effect of some variable on another, but are concerned that the treatment variable is endogenous in the system of interest i.e. correlated with the errors. In this case an “instrument” variable can be used in a regression context to disentangle treatment effect due to the threat of confounding due to endogeneity.
```

#### html2text {}

```diff
@@ -109,40 +109,42 @@
 appropriate when you have a time series of observations which undergo treatment
 at a particular point in time. This kind of analysis has no control group and
 looks for the presence of a change in the outcome measure at or soon after the
 treatment time. Multiple predictors can be included. | Time | Outcome | Treated
 | Predictor | |-----------|-----------|----------|----------| | $t_0$ | $y_0$ |
 False | $x_0$ | | $t_1$ | $y_0$ | False | $x_1$ | | $\ldots$ | $\ldots$ |
 $\ldots$ | $\ldots$ | | $t_{N-1}$ | $y_{N-1}$ | True | $x_{N-1}$ | | $t_N$ |
-$y_N$ | True | $x_N$ | | Frequentist | Bayesian | |--|--| | coming soon | ![]
-(https://raw.githubusercontent.com/pymc-labs/CausalPy/main/docs/source/_static/
-interrupted_time_series_pymc.svg) | > The data, pre-treatment model fit, and
-counterfactual are plotted (top). The causal impact is shown as a blue shaded
-region. The Bayesian analysis shows shaded Bayesian credible regions of the
-model fit and counterfactual. Also shown is the causal impact (middle) and
-cumulative causal impact (bottom). ### Instrumental Variable Regression
-Instrumental Variable regression is an appropriate technique when you wish to
-estimate the treatment effect of some variable on another, but are concerned
-that the treatment variable is endogenous in the system of interest i.e.
-correlated with the errors. In this case an âinstrumentâ variable can be
-used in a regression context to disentangle treatment effect due to the threat
-of confounding due to endogeneity. ![](https://raw.githubusercontent.com/pymc-
-labs/CausalPy/main/docs/source/_static/iv_reg1.png) ## Learning resources Here
-are some general resources about causal inference: * The official [PyMC
-examples gallery](https://www.pymc.io/projects/examples/en/latest/gallery.html)
-has a set of examples specifically relating to causal inference. * Angrist, J.
-D., & Pischke, J. S. (2009). Mostly harmless econometrics: An empiricist's
-companion. Princeton university press. * Angrist, J. D., & Pischke, J. S.
-(2014). Mastering'metrics: The path from cause to effect. Princeton university
-press. * Cunningham, S. (2021). [Causal inference: The Mixtape](https://
-mixtape.scunning.com). Yale University Press. * Huntington-Klein, N. (2021).
-[The effect: An introduction to research design and causality](https://
-theeffectbook.net). Chapman and Hall/CRC. * Reichardt, C. S. (2019). Quasi-
-experimentation: A guide to design and analysis. Guilford Publications. ##
-License [Apache License 2.0](LICENSE) --- ## Support [https://
-raw.githubusercontent.com/pymc-labs/CausalPy/main/docs/source/_static/pymc-
-labs-log.png]This repository is supported by [PyMC Labs](https://www.pymc-
-labs.com). If you are interested in seeing what PyMC Labs can do for you, then
-please email [ben.vincent@pymc-labs.com](mailto:ben.vincent@pymc-labs.com). We
-work with companies at a variety of scales and with varying levels of existing
-modeling capacity. We also run corporate workshop training events and can
-provide sessions ranging from introduction to Bayes to more advanced topics.
+$y_N$ | True | $x_N$ | | Frequentist | Bayesian | |--|--| | ![](https://
+raw.githubusercontent.com/pymc-labs/CausalPy/main/docs/source/_static/
+interrupted_time_series_skl.svg) | ![](https://raw.githubusercontent.com/pymc-
+labs/CausalPy/main/docs/source/_static/interrupted_time_series_pymc.svg) | >
+The data, pre-treatment model fit, and counterfactual are plotted (top). The
+causal impact is shown as a blue shaded region. The Bayesian analysis shows
+shaded Bayesian credible regions of the model fit and counterfactual. Also
+shown is the causal impact (middle) and cumulative causal impact (bottom). ###
+Instrumental Variable Regression Instrumental Variable regression is an
+appropriate technique when you wish to estimate the treatment effect of some
+variable on another, but are concerned that the treatment variable is
+endogenous in the system of interest i.e. correlated with the errors. In this
+case an âinstrumentâ variable can be used in a regression context to
+disentangle treatment effect due to the threat of confounding due to
+endogeneity. ![](https://raw.githubusercontent.com/pymc-labs/CausalPy/main/
+docs/source/_static/iv_reg1.png) ## Learning resources Here are some general
+resources about causal inference: * The official [PyMC examples gallery](https:
+//www.pymc.io/projects/examples/en/latest/gallery.html) has a set of examples
+specifically relating to causal inference. * Angrist, J. D., & Pischke, J. S.
+(2009). Mostly harmless econometrics: An empiricist's companion. Princeton
+university press. * Angrist, J. D., & Pischke, J. S. (2014). Mastering'metrics:
+The path from cause to effect. Princeton university press. * Cunningham, S.
+(2021). [Causal inference: The Mixtape](https://mixtape.scunning.com). Yale
+University Press. * Huntington-Klein, N. (2021). [The effect: An introduction
+to research design and causality](https://theeffectbook.net). Chapman and Hall/
+CRC. * Reichardt, C. S. (2019). Quasi-experimentation: A guide to design and
+analysis. Guilford Publications. ## License [Apache License 2.0](LICENSE) --
+- ## Support [https://raw.githubusercontent.com/pymc-labs/CausalPy/main/docs/
+source/_static/pymc-labs-log.png]This repository is supported by [PyMC Labs]
+(https://www.pymc-labs.com). If you are interested in seeing what PyMC Labs can
+do for you, then please email [ben.vincent@pymc-labs.com](mailto:
+ben.vincent@pymc-labs.com). We work with companies at a variety of scales and
+with varying levels of existing modeling capacity. We also run corporate
+workshop training events and can provide sessions ranging from introduction to
+Bayes to more advanced topics.
```

### Comparing `CausalPy-0.2.2/causalpy/custom_exceptions.py` & `CausalPy-0.2.3/causalpy/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/data/AJR2001.csv` & `CausalPy-0.2.3/causalpy/data/AJR2001.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/data/GDP_in_dollars_billions.csv` & `CausalPy-0.2.3/causalpy/data/GDP_in_dollars_billions.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/data/ancova_generated.csv` & `CausalPy-0.2.3/causalpy/data/ancova_generated.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/data/banks.csv` & `CausalPy-0.2.3/causalpy/data/banks.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/data/datasets.py` & `CausalPy-0.2.3/causalpy/data/datasets.py`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/data/deaths_and_temps_england_wales.csv` & `CausalPy-0.2.3/causalpy/data/deaths_and_temps_england_wales.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/data/did.csv` & `CausalPy-0.2.3/causalpy/data/did.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/data/drinking.csv` & `CausalPy-0.2.3/causalpy/data/drinking.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/data/geolift1.csv` & `CausalPy-0.2.3/causalpy/data/geolift1.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/data/its.csv` & `CausalPy-0.2.3/causalpy/data/its.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/data/its_simple.csv` & `CausalPy-0.2.3/causalpy/data/its_simple.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/data/regression_discontinuity.csv` & `CausalPy-0.2.3/causalpy/data/regression_discontinuity.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/data/simulate_data.py` & `CausalPy-0.2.3/causalpy/data/simulate_data.py`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/data/synthetic_control.csv` & `CausalPy-0.2.3/causalpy/data/synthetic_control.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/data_validation.py` & `CausalPy-0.2.3/causalpy/data_validation.py`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/plot_utils.py` & `CausalPy-0.2.3/causalpy/plot_utils.py`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/pymc_experiments.py` & `CausalPy-0.2.3/causalpy/pymc_experiments.py`

 * *Files 0% similar despite different names*

```diff
@@ -705,15 +705,15 @@
         :param round_to:
             Number of decimals used to round results. Defaults to 2. Use "None" to return raw numbers.
         """
 
         print(f"{self.expt_type:=^80}")
         print(f"Formula: {self.formula}")
         print("\nResults:")
-        print(round_num(self._causal_impact_summary_stat(), round_to))
+        print(self._causal_impact_summary_stat(round_to))
         self.print_coefficients(round_to)
 
 
 class RegressionDiscontinuity(ExperimentalDesign, RDDataValidator):
     """
     A class to analyse sharp regression discontinuity experiments.
 
@@ -899,15 +899,15 @@
         ax.legend(
             handles=(h_tuple for h_tuple in handles),
             labels=labels,
             fontsize=LEGEND_FONT_SIZE,
         )
         return fig, ax
 
-    def summary(self, round_to: None) -> None:
+    def summary(self, round_to=None) -> None:
         """
         Print text output summarising the results
 
         :param round_to:
             Number of decimals used to round results. Defaults to 2. Use "None" to return raw numbers.
         """
```

### Comparing `CausalPy-0.2.2/causalpy/pymc_models.py` & `CausalPy-0.2.3/causalpy/pymc_models.py`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/skl_experiments.py` & `CausalPy-0.2.3/causalpy/skl_experiments.py`

 * *Files 1% similar despite different names*

```diff
@@ -471,15 +471,18 @@
             xycoords="data",
             xytext=(1.05, self.y_pred_treatment[1]),
             textcoords="data",
             arrowprops={"arrowstyle": "<->", "color": "green", "lw": 3},
         )
         ax.annotate(
             "causal\nimpact",
-            xy=(1.05, np.mean([self.y_pred_counterfactual, self.y_pred_treatment[1]])),
+            xy=(
+                1.05,
+                np.mean([self.y_pred_counterfactual[0], self.y_pred_treatment[1]]),
+            ),
             xycoords="data",
             xytext=(5, 0),
             textcoords="offset points",
             color="green",
             va="center",
         )
         # formatting
```

### Comparing `CausalPy-0.2.2/causalpy/skl_models.py` & `CausalPy-0.2.3/causalpy/skl_models.py`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/causalpy/utils.py` & `CausalPy-0.2.3/causalpy/utils.py`

 * *Files identical despite different names*

### Comparing `CausalPy-0.2.2/pyproject.toml` & `CausalPy-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 exclude = ["causalpy.test*", "docs*"]
 
 [tool.setuptools.package-data]
 "causalpy.data" = ["*.csv"]
 
 [project]
 name = "CausalPy"
-version = "0.2.2"
+version = "0.2.3"
 description = "Causal inference for quasi-experiments in Python"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Ben Vincent", email = "ben.vincent@pymc-labs.com" }]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 
 # This field lists other packages that your project depends on to run.
 # Any package you put here will be installed by pip when your project is
 # installed, so they must be valid existing projects.
 #
 # For an analysis of this field vs pip's requirements files see:
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
@@ -111,9 +111,9 @@
 color = true
 omit-covered-files = false
 generate-badge = "docs/source/_static/"
 badge-format = "svg"
 
 [tool.ruff.lint]
 extend-select = [
-  "I",  # isort
+    "I", # isort
 ]
```

