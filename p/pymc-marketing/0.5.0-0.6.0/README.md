# Comparing `tmp/pymc_marketing-0.5.0.tar.gz` & `tmp/pymc_marketing-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymc_marketing-0.5.0.tar", last modified: Fri Apr 19 07:39:45 2024, max compression
+gzip compressed data, was "pymc_marketing-0.6.0.tar", last modified: Wed May  8 18:58:47 2024, max compression
```

## Comparing `pymc_marketing-0.5.0.tar` & `pymc_marketing-0.6.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:39:45.511607 pymc_marketing-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-04-19 07:39:45.511607 pymc_marketing-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:39:45.507607 pymc_marketing-0.5.0/pymc_marketing/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:39:45.507607 pymc_marketing-0.5.0/pymc_marketing/clv/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:39:45.507607 pymc_marketing-0.5.0/pymc_marketing/clv/models/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/models/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/models/beta_geo.py
--rw-r--r--   0 runner    (1001) docker     (127)    17844 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/models/gamma_gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)    40713 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/models/pareto_nbd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/models/shifted_beta_geo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10752 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    22801 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:39:45.511607 pymc_marketing-0.5.0/pymc_marketing/mmm/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47999 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/budget_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    52249 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/delayed_saturated_mmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16868 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/lift_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    26172 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/validating.py
--rw-r--r--   0 runner    (1001) docker     (127)    25723 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/version.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:39:45.511607 pymc_marketing-0.5.0/pymc_marketing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-04-19 07:39:45.000000 pymc_marketing-0.5.0/pymc_marketing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-19 07:39:45.000000 pymc_marketing-0.5.0/pymc_marketing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:39:45.000000 pymc_marketing-0.5.0/pymc_marketing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-19 07:39:45.000000 pymc_marketing-0.5.0/pymc_marketing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 07:39:45.000000 pymc_marketing-0.5.0/pymc_marketing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 07:39:45.511607 pymc_marketing-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:58:47.221387 pymc_marketing-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24424 2024-05-08 18:58:47.221387 pymc_marketing-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9990 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:58:47.213387 pymc_marketing-0.6.0/pymc_marketing/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:58:47.217387 pymc_marketing-0.6.0/pymc_marketing/clv/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/clv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/clv/distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:58:47.217387 pymc_marketing-0.6.0/pymc_marketing/clv/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/clv/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/clv/models/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/clv/models/beta_geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18452 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/clv/models/gamma_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41321 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/clv/models/pareto_nbd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/clv/models/shifted_beta_geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/clv/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23409 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/clv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:58:47.217387 pymc_marketing-0.6.0/pymc_marketing/mmm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/mmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57258 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/mmm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/mmm/budget_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55521 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/mmm/delayed_saturated_mmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/mmm/lift_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/mmm/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29709 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/mmm/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/mmm/tvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13077 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/mmm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/mmm/validating.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25386 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pymc_marketing/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:58:47.217387 pymc_marketing-0.6.0/pymc_marketing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24424 2024-05-08 18:58:47.000000 pymc_marketing-0.6.0/pymc_marketing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-08 18:58:47.000000 pymc_marketing-0.6.0/pymc_marketing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:58:47.000000 pymc_marketing-0.6.0/pymc_marketing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-08 18:58:47.000000 pymc_marketing-0.6.0/pymc_marketing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 18:58:47.000000 pymc_marketing-0.6.0/pymc_marketing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-08 18:58:43.000000 pymc_marketing-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:58:47.221387 pymc_marketing-0.6.0/setup.cfg
```

### Comparing `pymc_marketing-0.5.0/LICENSE` & `pymc_marketing-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc_marketing-0.5.0/PKG-INFO` & `pymc_marketing-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-marketing
-Version: 0.5.0
+Version: 0.6.0
 Summary: Marketing Statistical Models in PyMC
 Maintainer-email: PyMC Labs <info@pymc-labs.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,24 +209,24 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: arviz>=0.13.0
 Requires-Dist: matplotlib>=3.5.1
 Requires-Dist: numpy>=1.17
 Requires-Dist: pandas
-Requires-Dist: pymc>=5.10.4
+Requires-Dist: pymc>=5.12.0
 Requires-Dist: scikit-learn>=1.1.1
 Requires-Dist: seaborn>=0.12.2
 Requires-Dist: xarray
 Requires-Dist: xarray-einstats>=0.5.1
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: ipython!=8.7.0; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
-Requires-Dist: myst-nb; extra == "docs"
+Requires-Dist: myst-nb<=1.0.0; extra == "docs"
 Requires-Dist: pydata-sphinx-theme>=0.12.0.dev0; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinxext-opengraph; extra == "docs"
 Requires-Dist: sphinx-notfound-page; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
 Provides-Extra: lint
@@ -243,27 +243,45 @@
 
 ![PyMC-Marketing Logo](docs/source/_static/marketing-logo-light.jpg)
 
 </div>
 
 ----
 
-![Build](https://github.com/pymc-labs/pymc-marketing/workflows/ci/badge.svg)
+![Build](https://github.com/pymc-labs/pymc-marketing/actions/workflows/ci.yml/badge.svg)
 [![codecov](https://codecov.io/gh/pymc-labs/pymc-marketing/branch/main/graph/badge.svg?token=OBV3BS5TYE)](https://codecov.io/gh/pymc-labs/pymc-marketing)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![docs](https://readthedocs.org/projects/pymc-marketing/badge/?version=latest)](https://docs.readthedocs.io/en/latest/)
 [![PyPI Version](https://img.shields.io/pypi/v/pymc-marketing.svg)](https://pypi.python.org/pypi/pymc-marketing)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pymc-marketing.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 # <span style="color:limegreen">PyMC-Marketing</span>: Bayesian Marketing Mix Modeling (MMM) & Customer Lifetime Value (CLV)
 
 ## Marketing Analytics Tools from [PyMC Labs](https://www.pymc-labs.com)
 
 Unlock the power of **Marketing Mix Modeling (MMM)** and **Customer Lifetime Value (CLV)** analytics with PyMC-Marketing. This open-source marketing analytics tool empowers businesses to make smarter, data-driven decisions for maximizing ROI in marketing campaigns.
 
+----
+
+This repository is supported by [PyMC Labs](https://www.pymc-labs.com).
+
+<center>
+    <img src="docs/source/_static/labs-logo-light.png" width="50%" />
+</center>
+
+For businesses looking to integrate PyMC-Marketing into their operational framework, [PyMC Labs](https://www.pymc-labs.com) offers expert consulting and training. Our team is proficient in state-of-the-art Bayesian modeling techniques, with a focus on Marketing Mix Models (MMMs) and Customer Lifetime Value (CLV). For more information see [here](#-schedule-a-free-consultation-for-mmm--clv-strategy).
+
+Explore these topics further by watching our video on [Bayesian Marketing Mix Models: State of the Art](https://www.youtube.com/watch?v=xVx91prC81g).
+
+### Community Resources
+
+- [Bayesian discord server](https://discord.gg/swztKRaVKe)
+- [PyMC discourse](https://discourse.pymc.io/)
+
 ## Quick Installation Guide for Marketing Mix Modeling (MMM) & CLV
 
 To dive into MMM and CLV analytics, set up a specialized environment, `marketing_env`, via conda-forge:
 
 ```bash
 conda create -c conda-forge -n marketing_env pymc-marketing
 conda activate marketing_env
@@ -275,67 +293,133 @@
 
 We provide a `Dockerfile` to build a Docker image for PyMC-Marketing so that is accessible from a Jupyter Notebook. See [here](/scripts/docker/README.md) for more details.
 
 ## In-depth Bayesian Marketing Mix Modeling (MMM) in PyMC
 
 Leverage our Bayesian MMM API to tailor your marketing strategies effectively. Based on the research [Jin, Yuxue, et al. “Bayesian methods for media mix modeling with carryover and shape effects.” (2017)](https://research.google/pubs/pub46001/),  and integrating the expertise from core PyMC developers, our API provides:
 
+- **Custom Priors and Likelihoods**: Tailor your model to your specific business needs by including domain knowledge via prior distributions.
 - **Adstock Transformation**: Optimize the carry-over effects in your marketing channels.
 - **Saturation Effects**: Understand the diminishing returns in media investments.
+- **Time-varying Intercept:** Capture time-varying baseline contributions in your model (using modern and efficient Gaussian processes approximation methods).
+- **Visualization and Model Diagnostics**: Get a comprehensive view of your model's performance and insights.
+- **Out-of-sample Predictions**: Forecast future marketing performance with credible intervals. Use this for simulations and scenario planning.
 - **Budget Optimization**: Allocate your marketing spend efficiently across various channels for maximum ROI.
 - **Experiment Calibration**: Fine-tune your model based on empirical experiments for a more unified view of marketing.
 
+### MMM Quickstart
+
+```python
+import pandas as pd
+from pymc_marketing.mmm import DelayedSaturatedMMM
+
+data_url = "https://raw.githubusercontent.com/pymc-labs/pymc-marketing/main/data/mmm_example.csv"
+data = pd.read_csv(data_url, parse_dates=['date_week'])
+
+mmm = DelayedSaturatedMMM(
+    date_column="date_week",
+    channel_columns=["x1", "x2"],
+    control_columns=[
+        "event_1",
+        "event_2",
+        "t",
+    ],
+    adstock_max_lag=8,
+    yearly_seasonality=2,
+)
+```
+
+Initiate fitting and get a visualization of some of the outputs with:
+
+```python
+X = data.drop("y",axis=1)
+y = data["y"]
+mmm.fit(X,y)
+mmm.plot_components_contributions();
+```
+
+![](/docs/source/_static/mmm_plot_components_contributions.png)
+
+Once the model is fitted, we can further optimize our budget allocation as we are including diminishing returns and carry-over effects in our model.
+
+<center>
+    <img src="/docs/source/_static/mmm_plot_plot_channel_contributions_grid.png" width="80%" />
+</center>
+
 Explore a hands-on [simulated example](https://pymc-marketing.readthedocs.io/en/stable/notebooks/mmm/mmm_example.html) for more insights into MMM with PyMC-Marketing.
 
 ### Essential Reading for Marketing Mix Modeling (MMM)
 
 - [Bayesian Media Mix Modeling for Marketing Optimization](https://www.pymc-labs.com/blog-posts/bayesian-media-mix-modeling-for-marketing-optimization/)
 - [Improving the Speed and Accuracy of Bayesian Marketing Mix Models](https://www.pymc-labs.com/blog-posts/reducing-customer-acquisition-costs-how-we-helped-optimizing-hellofreshs-marketing-budget/)
 - [Johns, Michael and Wang,  Zhenyu. "A Bayesian Approach to Media Mix Modeling"](https://www.youtube.com/watch?v=UznM_-_760Y)
 - [Orduz, Juan. "Media Effect Estimation with PyMC: Adstock, Saturation & Diminishing Returns"](https://juanitorduz.github.io/pymc_mmm/)
-- [A Comprehensive Guide to Bayesian Marketing Mix Modeling](https://1749.io/resource-center/f/a-comprehensive-guide-to-bayesian-marketing-mix-modeling)
+- [A Comprehensive Guide to Bayesian Marketing Mix Modeling](https://1749.io/learn/f/a-comprehensive-guide-to-bayesian-marketing-mix-modeling)
 
 ## Unlock Customer Lifetime Value (CLV) with PyMC
 
 Understand and optimize your customer's value with our **CLV models**. Our API supports various types of CLV models, catering to both contractual and non-contractual settings, as well as continuous and discrete transaction modes.
 
 Explore our detailed CLV examples using data from the [`lifetimes`](https://github.com/CamDavidsonPilon/lifetimes) package:
 
 - [CLV Quickstart](https://pymc-marketing.readthedocs.io/en/stable/notebooks/clv/clv_quickstart.html)
 - [BG/NBD model](https://pymc-marketing.readthedocs.io/en/stable/notebooks/clv/bg_nbd.html)
+- [Pareto/NBD model](https://pymc-marketing.readthedocs.io/en/stable/notebooks/clv/pareto_nbd.html)
 - [Gamma-Gamma model](https://pymc-marketing.readthedocs.io/en/stable/notebooks/clv/gamma_gamma.html)
 
 ### Examples
 
 |                | **Non-contractual** | **Contractual**                 |
 |----------------|---------------------|---------------------------------|
 | **Continuous** | Buying groceries    | Audible                         |
 | **Discrete**   | Cinema ticket       | Monthly or yearly subscriptions |
 
----
+### CLV Quickstart
+
+```python
+import matplotlib.pyplot as plt
+import pandas as pd
+import seaborn as sns
+from pymc_marketing import clv
+
+data_url = "https://raw.githubusercontent.com/pymc-labs/pymc-marketing/main/data/clv_quickstart.csv"
+data = pd.read_csv(data_url)
+data["customer_id"] = data.index
+
+beta_geo_model = clv.BetaGeoModel(data=data)
+
+beta_geo_model.fit()
+```
+
+Once fitted, we can use the model to predict the number of future purchases for known customers, the probability that they are still alive, and get various visualizations plotted.
+
+![](/docs/source/_static/expected_purchases.png)
+
+See the Examples section for more on this.
 
 ## Why PyMC-Marketing vs other solutions?
 
 PyMC-Marketing is and will always be free for commercial use, licensed under [Apache 2.0](LICENSE). Developed by core developers behind the popular PyMC package and marketing experts, it provides state-of-the-art measurements and analytics for marketing teams.
 
-Due to its open-source nature and active contributor base, new features are added constantly. Missing a feature or want to contribute? Fork our repository and submit a pull request. For any questions, feel free to [open an issue](https://github.com/your-repo/issues).
+Due to its open-source nature and active contributor base, new features are constantly added. Are you missing a feature or want to contribute? Fork our repository and submit a pull request. If you have any questions, feel free to [open an issue](https://github.com/your-repo/issues).
+
+### Thanks to our contributors!
+
+[![https://github.com/pymc-devs/pymc/graphs/contributors](https://contrib.rocks/image?repo=pymc-labs/pymc-marketing)](https://github.com/pymc-labs/pymc-marketing/graphs/contributors)
+
 
 ## Marketing AI Assistant: MMM-GPT with PyMC-Marketing
 
 Not sure how to start or have questions? MMM-GPT is an AI that answers questions and provides expert advice on marketing analytics using PyMC-Marketing.
 
 **[Try MMM-GPT here.](https://mmm-gpt.com/)**
 
-
-
 ## 📞 Schedule a Free Consultation for MMM & CLV Strategy
 
 Maximize your marketing ROI with a [free 30-minute strategy session](https://calendly.com/niall-oulton) with our PyMC-Marketing experts. Learn how Bayesian Marketing Mix Modeling and Customer Lifetime Value analytics can boost your organization by making smarter, data-driven decisions.
 
-For businesses looking to integrate PyMC-Marketing into their operational framework, [PyMC Labs](https://www.pymc-labs.com) offers expert consulting and training. Our team is proficient in state-of-the-art Bayesian modeling techniques, with a focus on Marketing Mix Models (MMMs) and Customer Lifetime Value (CLV). Explore these topics further by watching our video on [Bayesian Marketing Mix Models: State of the Art](https://www.youtube.com/watch?v=xVx91prC81g).
-
 We provide the following professional services:
 
 - **Custom Models**: We tailor niche marketing analytics models to fit your organization's unique needs.
 - **Build Within PyMC-Marketing**: Our team members are experts leveraging the capabilities of PyMC-Marketing to create robust marketing models for precise insights.
 - **SLA & Coaching**: Get guaranteed support levels and personalized coaching to ensure your team is well-equipped and confident in using our tools and approaches.
 - **SaaS Solutions**: Harness the power of our state-of-the-art software solutions to streamline your data-driven marketing initiatives.
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/clv/distributions.py` & `pymc_marketing-0.6.0/pymc_marketing/clv/distributions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#   Copyright 2024 The PyMC Labs Developers
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 import numpy as np
 import pymc as pm
 import pytensor.tensor as pt
 from pymc.distributions.continuous import PositiveContinuous
 from pymc.distributions.dist_math import check_parameters
 from pytensor.tensor.random.op import RandomVariable
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/clv/models/basic.py` & `pymc_marketing-0.6.0/pymc_marketing/clv/models/basic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#   Copyright 2024 The PyMC Labs Developers
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 import json
 import warnings
 from collections.abc import Sequence
 from pathlib import Path
 from typing import cast
 
 import arviz as az
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/clv/models/beta_geo.py` & `pymc_marketing-0.6.0/pymc_marketing/clv/models/beta_geo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#   Copyright 2024 The PyMC Labs Developers
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 from collections.abc import Sequence
 
 import numpy as np
 import pandas as pd
 import pymc as pm
 import pytensor.tensor as pt
 import xarray as xr
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/clv/models/gamma_gamma.py` & `pymc_marketing-0.6.0/pymc_marketing/clv/models/gamma_gamma.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#   Copyright 2024 The PyMC Labs Developers
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 import numpy as np
 import pandas as pd
 import pymc as pm
 import pytensor.tensor as pt
 import xarray
 from pymc.util import RandomState
 from pytensor.tensor import TensorVariable
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/clv/models/pareto_nbd.py` & `pymc_marketing-0.6.0/pymc_marketing/clv/models/pareto_nbd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#   Copyright 2024 The PyMC Labs Developers
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 import warnings
 from collections.abc import Sequence
 from typing import Any, Literal, cast
 
 import numpy as np
 import pandas as pd
 import pymc as pm
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/clv/models/shifted_beta_geo.py` & `pymc_marketing-0.6.0/pymc_marketing/clv/models/shifted_beta_geo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#   Copyright 2024 The PyMC Labs Developers
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 from collections.abc import Sequence
 
 import numpy as np
 import pandas as pd
 import pymc as pm
 from pymc.util import RandomState
 from xarray import DataArray, Dataset
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/clv/plotting.py` & `pymc_marketing-0.6.0/pymc_marketing/clv/plotting.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#   Copyright 2024 The PyMC Labs Developers
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 from collections.abc import Sequence
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from matplotlib.lines import Line2D
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/clv/utils.py` & `pymc_marketing-0.6.0/pymc_marketing/clv/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#   Copyright 2024 The PyMC Labs Developers
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 import warnings
 from datetime import date, datetime
 
 import numpy as np
 import pandas as pd
 import xarray
 from numpy import datetime64
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/mmm/base.py` & `pymc_marketing-0.6.0/pymc_marketing/mmm/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#   Copyright 2024 The PyMC Labs Developers
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 """Base class for Marketing Mix Models (MMM)."""
 
 import warnings
 from collections.abc import Callable
 from inspect import (
     getattr_static,
     isdatadescriptor,
@@ -15,26 +28,29 @@
 import arviz as az
 import matplotlib.pyplot as plt
 import matplotlib.ticker as mtick
 import numpy as np
 import pandas as pd
 import pymc as pm
 import seaborn as sns
+from numpy.typing import NDArray
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import FunctionTransformer
 from xarray import DataArray, Dataset
 
 from pymc_marketing.mmm.budget_optimizer import budget_allocator
 from pymc_marketing.mmm.transformers import michaelis_menten
 from pymc_marketing.mmm.utils import (
+    apply_sklearn_transformer_across_dim,
     estimate_menten_parameters,
     estimate_sigmoid_parameters,
     find_sigmoid_inflection_point,
     sigmoid_saturation,
     standardize_scenarios_dict_keys,
+    transform_1d_array,
 )
 from pymc_marketing.mmm.validating import (
     ValidateChannelColumns,
     ValidateDateColumn,
     ValidateTargetColumn,
 )
 from pymc_marketing.model_builder import ModelBuilder
@@ -51,21 +67,27 @@
         self,
         date_column: str,
         channel_columns: list[str] | tuple[str],
         model_config: dict | None = None,
         sampler_config: dict | None = None,
         **kwargs,
     ) -> None:
-        self.X: pd.DataFrame | None = None
-        self.y: pd.Series | np.ndarray | None = None
         self.date_column: str = date_column
         self.channel_columns: list[str] | tuple[str] = channel_columns
+
         self.n_channel: int = len(channel_columns)
-        self._fit_result: az.InferenceData | None = None
-        self._posterior_predictive: az.InferenceData | None = None
+
+        self.X: pd.DataFrame
+        self.y: pd.Series | np.ndarray
+
+        self._time_resolution: int
+        self._time_index: NDArray[np.int_]
+        self._time_index_mid: int
+        self._fit_result: az.InferenceData
+        self._posterior_predictive: az.InferenceData
         super().__init__(model_config=model_config, sampler_config=sampler_config)
 
     @property
     def methods(self) -> list[Any]:
         maybe_methods = [getattr_static(self, attr) for attr in dir(self)]
         return [
             method
@@ -310,67 +332,198 @@
         else:
             raise RuntimeError(
                 "The model hasn't been fit yet, call .fit() first with X and y data."
             )
         return fig
 
     def plot_posterior_predictive(
-        self, original_scale: bool = False, **plt_kwargs: Any
+        self, original_scale: bool = False, ax: plt.Axes = None, **plt_kwargs: Any
     ) -> plt.Figure:
-        posterior_predictive_data: Dataset = self.posterior_predictive
-        likelihood_hdi_94: DataArray = az.hdi(
-            ary=posterior_predictive_data, hdi_prob=0.94
-        )[self.output_var]
-        likelihood_hdi_50: DataArray = az.hdi(
-            ary=posterior_predictive_data, hdi_prob=0.50
-        )[self.output_var]
+        """Plot posterior distribution from the model fit.
 
-        if original_scale:
-            likelihood_hdi_94 = self.get_target_transformer().inverse_transform(
-                Xt=likelihood_hdi_94
-            )
-            likelihood_hdi_50 = self.get_target_transformer().inverse_transform(
-                Xt=likelihood_hdi_50
-            )
+        Parameters
+        ----------
+        original_scale : bool, optional
+            Whether to plot in the original scale.
+        ax : plt.Axes, optional
+            Matplotlib axis object.
+        **plt_kwargs
+            Keyword arguments passed to `plt.subplots`.
 
-        fig, ax = plt.subplots(**plt_kwargs)
-        if self.X is not None and self.y is not None:
-            ax.fill_between(
-                x=self.X[self.date_column],
-                y1=likelihood_hdi_94[:, 0],
-                y2=likelihood_hdi_94[:, 1],
-                color="C0",
-                alpha=0.2,
-                label="$94\%$ HDI",  # noqa: W605
+        Returns
+        -------
+        plt.Figure
+        """
+        try:
+            posterior_predictive_data: Dataset = self.posterior_predictive
+
+        except Exception as e:
+            raise RuntimeError(
+                "Make sure the model has bin fitted and the posterior predictive has been sampled!"
+            ) from e
+
+        target_to_plot = np.asarray(
+            self.y
+            if original_scale
+            else transform_1d_array(self.get_target_transformer().transform, self.y)
+        )
+
+        if len(target_to_plot) != len(posterior_predictive_data.date):
+            raise ValueError(
+                "The length of the target variable doesn't match the length of the date column. "
+                "If you are predicting out-of-sample, please overwrite `self.y` with the "
+                "corresponding (non-transformed) target variable."
             )
 
+        if ax is None:
+            fig, ax = plt.subplots(**plt_kwargs)
+        else:
+            fig = ax.figure
+
+        for hdi_prob, alpha in zip((0.94, 0.50), (0.2, 0.4), strict=True):
+            likelihood_hdi: DataArray = az.hdi(
+                ary=posterior_predictive_data, hdi_prob=hdi_prob
+            )[self.output_var]
+
+            if original_scale:
+                likelihood_hdi = self.get_target_transformer().inverse_transform(
+                    Xt=likelihood_hdi
+                )
+
             ax.fill_between(
-                x=self.X[self.date_column],
-                y1=likelihood_hdi_50[:, 0],
-                y2=likelihood_hdi_50[:, 1],
+                x=posterior_predictive_data.date,
+                y1=likelihood_hdi[:, 0],
+                y2=likelihood_hdi[:, 1],
                 color="C0",
-                alpha=0.3,
-                label="$50\%$ HDI",  # noqa: W605
+                alpha=alpha,
+                label=f"${100 * hdi_prob}\%$ HDI",  # noqa: W605
             )
 
-            target_to_plot: np.ndarray = np.asarray(
-                self.y if original_scale else self.preprocessed_data["y"]  # type: ignore
-            )
-            ax.plot(
-                np.asarray(self.X[self.date_column]),
-                target_to_plot,
-                color="black",
+        ax.plot(
+            np.asarray(posterior_predictive_data.date),
+            target_to_plot,
+            color="black",
+            label="Observed",
+        )
+        ax.legend()
+        ax.set(
+            title="Posterior Predictive Check",
+            xlabel="date",
+            ylabel=self.output_var,
+        )
+
+        return fig
+
+    def get_errors(self, original_scale: bool = False) -> DataArray:
+        """Get model errors posterior distribution.
+
+        errors = true values - predicted
+
+        Parameters
+        ----------
+        original_scale : bool, optional
+            Whether to plot in the original scale.
+
+        Returns
+        -------
+        DataArray
+        """
+        try:
+            posterior_predictive_data: Dataset = self.posterior_predictive
+
+        except Exception as e:
+            raise RuntimeError(
+                "Make sure the model has bin fitted and the posterior predictive has been sampled!"
+            ) from e
+
+        target_array = np.asarray(
+            transform_1d_array(self.get_target_transformer().transform, self.y)
+        )
+
+        if len(target_array) != len(posterior_predictive_data.date):
+            raise ValueError(
+                "The length of the target variable doesn't match the length of the date column. "
+                "If you are computing out-of-sample errors, please overwrite `self.y` with the "
+                "corresponding (non-transformed) target variable."
             )
-            ax.set(
-                title="Posterior Predictive Check",
-                xlabel="date",
-                ylabel=self.output_var,
+
+        target = (
+            pd.Series(target_array, index=self.posterior_predictive.date)
+            .rename_axis("date")
+            .to_xarray()
+        )
+
+        errors = (
+            (target - posterior_predictive_data)[self.output_var]
+            .rename("errors")
+            .transpose(..., "date")
+        )
+
+        if original_scale:
+            return apply_sklearn_transformer_across_dim(
+                data=errors,
+                func=self.get_target_transformer().inverse_transform,
+                dim_name="date",
             )
+
+        return errors
+
+    def plot_errors(
+        self, original_scale: bool = False, ax: plt.Axes = None, **plt_kwargs: Any
+    ) -> plt.Figure:
+        """Plot model errors by taking the difference between true values and predicted.
+
+        errors = true values - predicted
+
+        Parameters
+        ----------
+        original_scale : bool, optional
+            Whether to plot in the original scale.
+        ax : plt.Axes, optional
+            Matplotlib axis object.
+        **plt_kwargs
+            Keyword arguments passed to `plt.subplots`.
+
+        Returns
+        -------
+        plt.Figure
+        """
+        errors = self.get_errors(original_scale=original_scale)
+
+        if ax is None:
+            fig, ax = plt.subplots(**plt_kwargs)
         else:
-            raise RuntimeError("The model hasn't been fit yet, call .fit() first")
+            fig = ax.figure
+
+        for hdi_prob, alpha in zip((0.94, 0.50), (0.2, 0.4), strict=True):
+            errors_hdi = az.hdi(ary=errors, hdi_prob=hdi_prob)
+
+            ax.fill_between(
+                x=self.posterior_predictive.date,
+                y1=errors_hdi["errors"].sel(hdi="lower"),
+                y2=errors_hdi["errors"].sel(hdi="higher"),
+                color="C3",
+                alpha=alpha,
+                label=f"${100 * hdi_prob}\%$ HDI",  # noqa: W605
+            )
+
+        ax.plot(
+            self.posterior_predictive.date,
+            errors.mean(dim=("chain", "draw")).to_numpy(),
+            color="C3",
+            label="Errors Mean",
+        )
+
+        ax.axhline(y=0.0, linestyle="--", color="black", label="zero")
+        ax.legend()
+        ax.set(
+            title="Errors Posterior Distribution",
+            xlabel="date",
+            ylabel="true - predictions",
+        )
         return fig
 
     def _format_model_contributions(self, var_contribution: str) -> DataArray:
         contributions = az.extract(
             self.fit_result,
             var_names=[var_contribution],
             combined=False,
@@ -431,19 +584,26 @@
                     np.asarray(mean),
                     color=f"C{i}",
                 )
         if self.X is not None:
             intercept = az.extract(
                 self.fit_result, var_names=["intercept"], combined=False
             )
-            intercept_hdi = np.repeat(
-                a=az.hdi(intercept).intercept.data[None, ...],
-                repeats=self.X[self.date_column].shape[0],
-                axis=0,
-            )
+
+            if intercept.ndim == 2:
+                # Intercept has a stationary prior
+                intercept_hdi = np.repeat(
+                    a=az.hdi(intercept).intercept.data[None, ...],
+                    repeats=self.X[self.date_column].shape[0],
+                    axis=0,
+                )
+            elif intercept.ndim == 3:
+                # Intercept has a time-varying prior
+                intercept_hdi = az.hdi(intercept).intercept.data
+
             ax.plot(
                 np.asarray(self.X[self.date_column]),
                 np.full(len(self.X[self.date_column]), intercept.mean().data),
                 color=f"C{i + 1}",
             )
             ax.fill_between(
                 x=self.X[self.date_column],
@@ -1024,14 +1184,15 @@
             figsize = (12, 4)
 
             def label_func(channel):
                 return f"{channel} Data Points"
 
             def legend_title_func(channel):
                 return "Legend"
+
         else:
             nrows = len(channels_to_plot)
             figsize = (12, 4 * len(channels_to_plot))
 
             def label_func(channel):
                 return "Data Points"
 
@@ -1158,24 +1319,26 @@
             )
         else:
             contributions_control_over_time = pd.DataFrame(
                 index=contributions_channel_over_time.index
             )
 
         if getattr(self, "yearly_seasonality", None):
-            contributions_fourier_over_time = (
+            contributions_fourier_over_time = pd.DataFrame(
                 az.extract(
                     self.fit_result,
                     var_names=["fourier_contributions"],
                     combined=True,
                 )
                 .mean("sample")
                 .to_dataframe()
                 .squeeze()
                 .unstack()
+                .sum(axis=1),
+                columns=["yearly_seasonality"],
             )
         else:
             contributions_fourier_over_time = pd.DataFrame(
                 index=contributions_channel_over_time.index
             )
 
         contributions_intercept_over_time = (
@@ -1296,10 +1459,127 @@
         fig: plt.Figure = plt.gcf()
         fig.suptitle("channel Contribution Share", fontsize=16, y=1.05)
         return fig
 
     def graphviz(self, **kwargs):
         return pm.model_to_graphviz(self.model, **kwargs)
 
+    def _process_decomposition_components(self, data: pd.DataFrame) -> pd.DataFrame:
+        """
+        Process data to compute the sum of contributions by component and calculate their percentages.
+        The output dataframe will have columns for "component", "contribution", and "percentage".
+
+        Parameters
+        ----------
+        data : pd.DataFrame
+            Dataframe containing the contribution by component from the function "compute_mean_contributions_over_time".
+
+        Returns
+        -------
+        pd.DataFrame
+            A dataframe with contributions summed up by component, sorted by contribution in ascending order.
+            With an additional column showing the percentage contribution of each component.
+        """
+
+        dataframe = data.copy()
+        stack_dataframe = dataframe.stack().reset_index()
+        stack_dataframe.columns = pd.Index(["date", "component", "contribution"])
+        stack_dataframe.set_index(["date", "component"], inplace=True)
+        dataframe = stack_dataframe.groupby("component").sum()
+        dataframe.sort_values(by="contribution", ascending=True, inplace=True)
+        dataframe.reset_index(inplace=True)
+
+        total_contribution = dataframe["contribution"].sum()
+        dataframe["percentage"] = (dataframe["contribution"] / total_contribution) * 100
+
+        return dataframe
+
+    def plot_waterfall_components_decomposition(
+        self,
+        original_scale: bool = True,
+        figsize: tuple[int, int] = (14, 7),
+        **kwargs,
+    ) -> plt.Figure:
+        """
+        This function creates a waterfall plot. The plot shows the decomposition of the target into its components.
+
+        Parameters
+        ----------
+        original_scale : bool, optional
+            If True, the contributions are plotted in the original scale of the target.
+        figsize : Tuple, optional
+            The size of the figure. The default is (14, 7).
+        **kwargs
+            Additional keyword arguments to pass to the matplotlib `subplots` function.
+
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The matplotlib figure object.
+        """
+
+        dataframe = self.compute_mean_contributions_over_time(
+            original_scale=original_scale
+        )
+
+        dataframe = self._process_decomposition_components(data=dataframe)
+        total_contribution = dataframe["contribution"].sum()
+
+        fig, ax = plt.subplots(figsize=figsize, layout="constrained", **kwargs)
+
+        cumulative_contribution = 0
+
+        for index, row in dataframe.iterrows():
+            color = "C0" if row["contribution"] >= 0 else "C3"
+
+            bar_start = (
+                cumulative_contribution + row["contribution"]
+                if row["contribution"] < 0
+                else cumulative_contribution
+            )
+            ax.barh(
+                row["component"],
+                row["contribution"],
+                left=bar_start,
+                color=color,
+                alpha=0.5,
+            )
+
+            if row["contribution"] > 0:
+                cumulative_contribution += row["contribution"]
+
+            label_pos = bar_start + (row["contribution"] / 2)
+
+            if row["contribution"] < 0:
+                label_pos = bar_start - (row["contribution"] / 2)
+
+            ax.text(
+                label_pos,
+                index,
+                f"{row['contribution']:,.0f}\n({row['percentage']:.1f}%)",
+                ha="center",
+                va="center",
+                color="black",
+                fontsize=10,
+            )
+
+        ax.set_title("Response Decomposition Waterfall by Components")
+        ax.set_xlabel("Cumulative Contribution")
+        ax.set_ylabel("Components")
+
+        xticks = np.linspace(0, total_contribution, num=11)
+        xticklabels = [f"{(x/total_contribution)*100:.0f}%" for x in xticks]
+        ax.set_xticks(xticks)
+        ax.set_xticklabels(xticklabels)
+
+        ax.spines["right"].set_visible(False)
+        ax.spines["top"].set_visible(False)
+        ax.spines["left"].set_visible(False)
+
+        ax.set_yticks(np.arange(len(dataframe)))
+        ax.set_yticklabels(dataframe["component"])
+
+        return fig
+
 
 class MMM(BaseMMM, ValidateTargetColumn, ValidateDateColumn, ValidateChannelColumns):
     pass
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/mmm/budget_optimizer.py` & `pymc_marketing-0.6.0/pymc_marketing/mmm/budget_optimizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#   Copyright 2024 The PyMC Labs Developers
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 """Budget optimization module."""
 
 import numpy as np
 from pandas import DataFrame
 from scipy.optimize import minimize
 
 from pymc_marketing.mmm.transformers import michaelis_menten
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/mmm/delayed_saturated_mmm.py` & `pymc_marketing-0.6.0/pymc_marketing/mmm/delayed_saturated_mmm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#   Copyright 2024 The PyMC Labs Developers
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 """Media Mix Model with delayed adstock and logistic saturation class."""
 
 import json
 from pathlib import Path
 from typing import Any
 
 import arviz as az
@@ -10,21 +23,23 @@
 import numpy.typing as npt
 import pandas as pd
 import pymc as pm
 import seaborn as sns
 from pytensor.tensor import TensorVariable
 from xarray import DataArray, Dataset
 
+from pymc_marketing.constants import DAYS_IN_YEAR
 from pymc_marketing.mmm.base import MMM
 from pymc_marketing.mmm.lift_test import (
     add_logistic_empirical_lift_measurements_to_likelihood,
     scale_lift_measurements,
 )
 from pymc_marketing.mmm.preprocessing import MaxAbsScaleChannels, MaxAbsScaleTarget
 from pymc_marketing.mmm.transformers import geometric_adstock, logistic_saturation
+from pymc_marketing.mmm.tvp import create_time_varying_intercept, infer_time_index
 from pymc_marketing.mmm.utils import (
     apply_sklearn_transformer_across_dim,
     create_new_spend_data,
     generate_fourier_modes,
 )
 from pymc_marketing.mmm.validating import ValidateControlColumns
 
@@ -43,14 +58,15 @@
     version = "0.0.2"
 
     def __init__(
         self,
         date_column: str,
         channel_columns: list[str],
         adstock_max_lag: int,
+        time_varying_intercept: bool = False,
         model_config: dict | None = None,
         sampler_config: dict | None = None,
         validate_data: bool = True,
         control_columns: list[str] | None = None,
         yearly_seasonality: int | None = None,
         **kwargs,
     ) -> None:
@@ -58,14 +74,18 @@
 
         Parameters
         ----------
         date_column : str
             Column name of the date variable.
         channel_columns : List[str]
             Column names of the media channel variables.
+        adstock_max_lag : int
+            Number of lags to consider in the adstock transformation.
+        time_varying_intercept : bool, optional
+            Whether to consider time-varying intercept, by default False.
         model_config : Dictionary, optional
             dictionary of parameters that initialise model configuration.
             Class-default defined by the user default_model_config method.
         sampler_config : Dictionary, optional
             dictionary of parameters that initialise sampler configuration.
             Class-default defined by the user default_sampler_config method.
         validate_data : bool, optional
@@ -75,14 +95,15 @@
         adstock_max_lag : int, optional
             Number of lags to consider in the adstock transformation, by default 4
         yearly_seasonality : Optional[int], optional
             Number of Fourier modes to model yearly seasonality, by default None.
         """
         self.control_columns = control_columns
         self.adstock_max_lag = adstock_max_lag
+        self.time_varying_intercept = time_varying_intercept
         self.yearly_seasonality = yearly_seasonality
         self.date_column = date_column
         self.validate_data = validate_data
 
         super().__init__(
             date_column=date_column,
             channel_columns=channel_columns,
@@ -108,14 +129,32 @@
         If validate is True, it will check if the data is valid for the model.
         sets self.model_coords based on provided dataset
 
         Parameters
         ----------
         X : Union[pd.DataFrame, pd.Series], shape (n_obs, n_features)
         y : Union[pd.Series, np.ndarray], shape (n_obs,)
+
+        Sets
+        ----
+        preprocessed_data : Dict[str, Union[pd.DataFrame, pd.Series]]
+            Preprocessed data for the model.
+        X : pd.DataFrame
+            A filtered version of the input `X`, such that it is guaranteed that
+            it contains only the `date_column`, the columns that are specified
+            in the `channel_columns` and `control_columns`, and fourier features
+            if `yearly_seasonality=True`.
+        y : Union[pd.Series, np.ndarray]
+            The target variable for the model (as provided).
+        _time_index : np.ndarray
+            The index of the date column. Used by TVP
+        _time_index_mid : int
+            The middle index of the date index. Used by TVP.
+        _time_resolution: int
+            The time resolution of the date index. Used by TVP.
         """
         date_data = X[self.date_column]
         channel_data = X[self.channel_columns]
 
         self.coords_mutable: dict[str, Any] = {
             "date": date_data,
         }
@@ -148,14 +187,21 @@
         self.preprocessed_data: dict[str, pd.DataFrame | pd.Series] = {
             "X": self.preprocess("X", X_data),  # type: ignore
             "y": self.preprocess("y", y),  # type: ignore
         }
         self.X: pd.DataFrame = X_data
         self.y: pd.Series | np.ndarray = y
 
+        if self.time_varying_intercept:
+            self._time_index = np.arange(0, X.shape[0])
+            self._time_index_mid = X.shape[0] // 2
+            self._time_resolution = (
+                self.X[self.date_column].iloc[1] - self.X[self.date_column].iloc[0]
+            ).days
+
     def _save_input_params(self, idata) -> None:
         """Saves input parameters to the attrs of idata."""
         idata.attrs["date_column"] = json.dumps(self.date_column)
         idata.attrs["control_columns"] = json.dumps(self.control_columns)
         idata.attrs["channel_columns"] = json.dumps(self.channel_columns)
         idata.attrs["adstock_max_lag"] = json.dumps(self.adstock_max_lag)
         idata.attrs["validate_data"] = json.dumps(self.validate_data)
@@ -351,17 +397,31 @@
 
             target_ = pm.MutableData(
                 name="target",
                 value=self.preprocessed_data["y"],
                 dims="date",
             )
 
-            intercept = self.intercept_dist(
-                name="intercept", **self.model_config["intercept"]["kwargs"]
-            )
+            if self.time_varying_intercept:
+                time_index = pm.Data(
+                    "time_index",
+                    self._time_index,
+                    dims="date",
+                )
+                intercept = create_time_varying_intercept(
+                    time_index,
+                    self._time_index_mid,
+                    self._time_resolution,
+                    self.intercept_dist,
+                    self.model_config,
+                )
+            else:
+                intercept = self.intercept_dist(
+                    name="intercept", **self.model_config["intercept"]["kwargs"]
+                )
 
             beta_channel = self.beta_channel_dist(
                 name="beta_channel",
                 **self.model_config["beta_channel"]["kwargs"],
                 dims=("channel",),
             )
             alpha = self.alpha_dist(
@@ -387,17 +447,19 @@
                 dims=("date", "channel"),
             )
             channel_adstock_saturated = pm.Deterministic(
                 name="channel_adstock_saturated",
                 var=logistic_saturation(x=channel_adstock, lam=lam),
                 dims=("date", "channel"),
             )
+
+            channel_contributions_var = channel_adstock_saturated * beta_channel
             channel_contributions = pm.Deterministic(
                 name="channel_contributions",
-                var=channel_adstock_saturated * beta_channel,
+                var=channel_contributions_var,
                 dims=("date", "channel"),
             )
 
             mu_var = intercept + channel_contributions.sum(axis=-1)
 
             if (
                 self.control_columns is not None
@@ -464,41 +526,54 @@
                 observed=target_,
                 dims="date",
             )
 
     @property
     def default_model_config(self) -> dict:
         return {
-            "intercept": {"dist": "Normal", "kwargs": {"mu": 0, "sigma": 2}},
+            "intercept": {
+                "dist": "Normal",
+                "kwargs": {"mu": 0, "sigma": 2},
+            },
             "beta_channel": {"dist": "HalfNormal", "kwargs": {"sigma": 2}},
             "alpha": {"dist": "Beta", "kwargs": {"alpha": 1, "beta": 3}},
             "lam": {"dist": "Gamma", "kwargs": {"alpha": 3, "beta": 1}},
             "likelihood": {
                 "dist": "Normal",
                 "kwargs": {
                     "sigma": {"dist": "HalfNormal", "kwargs": {"sigma": 2}},
                 },
             },
             "gamma_control": {"dist": "Normal", "kwargs": {"mu": 0, "sigma": 2}},
             "gamma_fourier": {"dist": "Laplace", "kwargs": {"mu": 0, "b": 1}},
+            "intercept_tvp_kwargs": {
+                "m": 200,
+                "L": None,
+                "eta_lam": 1,
+                "ls_mu": None,
+                "ls_sigma": 10,
+                "cov_func": None,
+            },
         }
 
     def _get_fourier_models_data(self, X) -> pd.DataFrame:
         """Generates fourier modes to model seasonality.
 
         References
         ----------
         https://www.pymc.io/projects/examples/en/latest/time_series/Air_passengers-Prophet_with_Bayesian_workflow.html
         """
         if self.yearly_seasonality is None:
             raise ValueError("yearly_seasonality must be specified.")
         date_data: pd.Series = pd.to_datetime(
             arg=X[self.date_column], format="%Y-%m-%d"
         )
-        periods: npt.NDArray[np.float_] = date_data.dt.dayofyear.to_numpy() / 365.25
+        periods: npt.NDArray[np.float_] = (
+            date_data.dt.dayofyear.to_numpy() / DAYS_IN_YEAR
+        )
         return generate_fourier_modes(
             periods=periods,
             n_order=self.yearly_seasonality,
         )
 
     def channel_contributions_forward_pass(
         self, channel_data: npt.NDArray[np.float_]
@@ -674,14 +749,19 @@
                 else self.control_transformer.transform
             )
             data["control_data"] = control_transformation(control_data)
 
         if hasattr(self, "fourier_columns"):
             data["fourier_data"] = self._get_fourier_models_data(X)
 
+        if self.time_varying_intercept:
+            data["time_index"] = infer_time_index(
+                X[self.date_column], self.X[self.date_column], self._time_resolution
+            )
+
         if y is not None:
             if isinstance(y, pd.Series):
                 data["target"] = (
                     y.to_numpy()
                 )  # convert Series to numpy array explicitly
             elif isinstance(y, np.ndarray):
                 data["target"] = y
@@ -1299,24 +1379,24 @@
         """Add lift tests to the model.
 
         The model difference of a channel's saturation curve is created
         from `x` and `x + delta_x` for each channel. This random variable is
         then conditioned using the empirical lift, `delta_y`, and `sigma` of the lift test
         with the specified distribution `dist`.
 
-        The sudo code for the lift test is as follows:
+        The pseudo-code for the lift test is as follows:
 
         .. code-block:: python
 
             model_estimated_lift = (
                 saturation_curve(x + delta_x)
                 - saturation_curve(x)
             )
             empirical_lift = delta_y
-            dist(model_estimated_lift, sigma=sigma, observed=empirical_lift)
+            dist(abs(model_estimated_lift), sigma=sigma, observed=abs(empirical_lift))
 
 
         The model has to be built before adding the lift tests.
 
         Parameters
         ----------
         df_lift_test : pd.DataFrame
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/mmm/lift_test.py` & `pymc_marketing-0.6.0/pymc_marketing/mmm/lift_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#   Copyright 2024 The PyMC Labs Developers
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 """Lift test functions for the MMM."""
 
 from collections.abc import Callable
 from functools import partial
 from typing import Union
 
 import numpy as np
@@ -24,15 +37,14 @@
 
 Index = npt.NDArray[np.int_]
 Indices = dict[str, Index]
 Values = Union[npt.NDArray[np.int_], npt.NDArray[np.float_], npt.NDArray[np.str_]]  # noqa: UP007
 
 
 def _lift_test_index(lift_values: Values, model_values: Values) -> Index:
-    # TODO: better support for datetime64 required for date coordinates
     same_value = lift_values[:, None] == model_values
     if not (same_value.sum(axis=1) == 1).all():
         missing_values = np.argwhere(same_value.sum(axis=1) == 0).flatten()
         raise MissingLiftTestError(missing_values)
 
     return np.argmax(same_value, axis=1)
 
@@ -59,16 +71,24 @@
     ------
     MissingLiftTestError
         If some lift test values are not in the model.
 
     """
 
     columns = df_lift_test.columns.tolist()
+
     return {
-        col: _lift_test_index(df_lift_test[col].to_numpy(), np.array(model.coords[col]))
+        col: _lift_test_index(
+            df_lift_test[col].to_numpy(),
+            # Coords in the model become tuples
+            # Reference: https://github.com/pymc-devs/pymc/blob/04b6881efa9f69711d604d2234c5645304f63d28/pymc/model/core.py#L998
+            # which become pd.Timestamp if from pandas objects
+            # Convert to Series stores them as np.datetime64
+            pd.Series(model.coords[col]).to_numpy(),
+        )
         for col in columns
     }
 
 
 def calculate_lift_measurements_from_curve(
     x_before: npt.NDArray[np.float_],
     x_after: npt.NDArray[np.float_],
@@ -174,14 +194,31 @@
     indices: Indices,
 ) -> pt.TensorVariable:
     """Index the TensorVariable based on the required lift test indices."""
     idx = tuple([indices[dim] for dim in var_dims])
     return var.__getitem__(idx)
 
 
+class NonMonotonicLiftError(Exception):
+    """Raised when the lift test results do not satisfy the increasing assumption."""
+
+
+def check_increasing_assumption(df_lift_tests: pd.DataFrame) -> None:
+    """Checks if the lift test results satisfy the increasing assumption.
+
+    If delta_x is positive, delta_y must be positive, and vice versa.
+    """
+    increasing = df_lift_tests["delta_x"] * df_lift_tests["delta_y"] >= 0
+
+    if not increasing.all():
+        raise NonMonotonicLiftError(
+            "The lift test results do not satisfy the increasing assumption."
+        )
+
+
 def add_lift_measurements_to_likelihood(
     df_lift_test: pd.DataFrame,
     variable_mapping,
     saturation_function,
     model: pm.Model | None = None,
     dist=pm.Gamma,
     name: str = "lift_measurements",
@@ -253,14 +290,16 @@
     """
     required_columns = ["x", "delta_x", "delta_y", "sigma"]
 
     missing_cols = set(required_columns).difference(df_lift_test.columns)
     if missing_cols:
         raise KeyError(f"Missing from DataFrame: {list(missing_cols)}")
 
+    check_increasing_assumption(df_lift_test)
+
     model = pm.modelcontext(model)
 
     var_names = list(variable_mapping.values())
     indices = indices_from_lift_tests(df_lift_test, model, var_names)
 
     x_before = df_lift_test["x"].to_numpy()
     x_after = x_before + df_lift_test["delta_x"].to_numpy()
@@ -277,17 +316,17 @@
     partial_saturation_function = partial(saturation_function, **kwargs)
     model_estimated_lift = calculate_lift_measurements_from_curve(
         x_before, x_after, partial_saturation_function
     )
 
     dist(
         name=name,
-        mu=model_estimated_lift,
+        mu=pt.abs(model_estimated_lift),
         sigma=df_lift_test["sigma"].to_numpy(),
-        observed=df_lift_test["delta_y"].to_numpy(),
+        observed=np.abs(df_lift_test["delta_y"].to_numpy()),
     )
 
 
 def add_menten_empirical_lift_measurements_to_likelihood(
     df_lift_test: pd.DataFrame,
     alpha_name: str,
     lam_name: str,
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/mmm/preprocessing.py` & `pymc_marketing-0.6.0/pymc_marketing/mmm/preprocessing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#   Copyright 2024 The PyMC Labs Developers
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 """Preprocessing methods for the Marketing Mix Model."""
 
 from collections.abc import Callable
 from typing import Any
 
 import numpy as np
 import pandas as pd
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/mmm/transformers.py` & `pymc_marketing-0.6.0/pymc_marketing/mmm/transformers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#   Copyright 2024 The PyMC Labs Developers
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 """Media transformation functions for Marketing Mix Models."""
 
 from enum import Enum
 from typing import Any, NamedTuple
 
 import numpy as np
 import numpy.typing as npt
@@ -135,15 +148,20 @@
     # along the dimension that represents the convolution time lags
     conv = pt.sum(padded_x * w[..., None, :], axis=-1)
     # Move the "time" axis back to where it was in the original x array
     return pt.moveaxis(conv, -1, axis + conv.ndim - orig_ndim)
 
 
 def geometric_adstock(
-    x, alpha: float = 0.0, l_max: int = 12, normalize: bool = False, axis: int = 0
+    x,
+    alpha: float = 0.0,
+    l_max: int = 12,
+    normalize: bool = False,
+    axis: int = 0,
+    mode: ConvMode = ConvMode.After,
 ):
     R"""Geometric adstock transformation.
 
     Adstock with geometric decay assumes advertising effect peaks at the same
     time period as ad exposure. The cumulative media effect is a weighted average
     of media spend in the current time-period (e.g. week) and previous `l_max` - 1
     periods (e.g. weeks). `l_max` is the maximum duration of carryover effect.
@@ -185,38 +203,50 @@
         Input tensor.
     alpha : float, by default 0.0
         Retention rate of ad effect. Must be between 0 and 1.
     l_max : int, by default 12
         Maximum duration of carryover effect.
     normalize : bool, by default False
         Whether to normalize the weights.
+    axis : int
+        The axis of ``x`` along witch to apply the convolution
+    mode : ConvMode, optional
+        The convolution mode determines how the convolution is applied at the boundaries
+        of the input signal, denoted as "x." The default mode is ConvMode.Before.
+
+        - ConvMode.After: Applies the convolution with the "Adstock" effect, resulting in a trailing decay effect.
+        - ConvMode.Before: Applies the convolution with the "Excitement" effect, creating a leading effect
+            similar to the wow factor.
+        - ConvMode.Overlap: Applies the convolution with both "Pull-Forward" and "Pull-Backward" effects,
+            where the effect overlaps with both preceding and succeeding elements.
 
     Returns
     -------
     tensor
         Transformed tensor.
 
     References
     ----------
     .. [1] Jin, Yuxue, et al. "Bayesian methods for media mix modeling
        with carryover and shape effects." (2017).
     """
 
     w = pt.power(pt.as_tensor(alpha)[..., None], pt.arange(l_max, dtype=x.dtype))
     w = w / pt.sum(w, axis=-1, keepdims=True) if normalize else w
-    return batched_convolution(x, w, axis=axis, mode=ConvMode.After)
+    return batched_convolution(x, w, axis=axis, mode=mode)
 
 
 def delayed_adstock(
     x,
     alpha: float = 0.0,
     theta: int = 0,
     l_max: int = 12,
     normalize: bool = False,
     axis: int = 0,
+    mode: ConvMode = ConvMode.After,
 ):
     R"""Delayed adstock transformation.
 
     This transformation is similar to geometric adstock transformation, but it
     allows for a delayed peak of the effect. The peak is assumed to occur at `theta`.
 
     .. plot::
@@ -255,14 +285,25 @@
         Retention rate of ad effect. Must be between 0 and 1.
     theta : float, by default 0
         Delay of the peak effect. Must be between 0 and `l_max` - 1.
     l_max : int, by default 12
         Maximum duration of carryover effect.
     normalize : bool, by default False
         Whether to normalize the weights.
+    axis : int
+        The axis of ``x`` along witch to apply the convolution
+    mode : ConvMode, optional
+        The convolution mode determines how the convolution is applied at the boundaries
+        of the input signal, denoted as "x." The default mode is ConvMode.Before.
+
+        - ConvMode.After: Applies the convolution with the "Adstock" effect, resulting in a trailing decay effect.
+        - ConvMode.Before: Applies the convolution with the "Excitement" effect, creating a leading effect
+            similar to the wow factor.
+        - ConvMode.Overlap: Applies the convolution with both "Pull-Forward" and "Pull-Backward" effects,
+            where the effect overlaps with both preceding and succeeding elements.
 
     Returns
     -------
     tensor
         Transformed tensor.
 
     References
@@ -271,23 +312,24 @@
        with carryover and shape effects." (2017).
     """
     w = pt.power(
         pt.as_tensor(alpha)[..., None],
         (pt.arange(l_max, dtype=x.dtype) - pt.as_tensor(theta)[..., None]) ** 2,
     )
     w = w / pt.sum(w, axis=-1, keepdims=True) if normalize else w
-    return batched_convolution(x, w, axis=axis, mode=ConvMode.After)
+    return batched_convolution(x, w, axis=axis, mode=mode)
 
 
 def weibull_adstock(
     x,
     lam=1,
     k=1,
     l_max: int = 12,
     axis: int = 0,
+    mode: ConvMode = ConvMode.After,
     type: WeibullType | str = WeibullType.PDF,
 ):
     R"""Weibull Adstocking Transformation.
 
     This transformation is similar to geometric adstock transformation but has more
     degrees of freedom, adding more flexibility.
 
@@ -345,14 +387,25 @@
         Input tensor.
     lam : float, by default 1.
         Scale parameter of the Weibull distribution. Must be positive.
     k : float, by default 1.
         Shape parameter of the Weibull distribution. Must be positive.
     l_max : int, by default 12
         Maximum duration of carryover effect.
+    axis : int
+        The axis of ``x`` along witch to apply the convolution
+    mode : ConvMode, optional
+        The convolution mode determines how the convolution is applied at the boundaries
+        of the input signal, denoted as "x." The default mode is ConvMode.Before.
+
+        - ConvMode.After: Applies the convolution with the "Adstock" effect, resulting in a trailing decay effect.
+        - ConvMode.Before: Applies the convolution with the "Excitement" effect, creating a leading effect
+            similar to the wow factor.
+        - ConvMode.Overlap: Applies the convolution with both "Pull-Forward" and "Pull-Backward" effects,
+            where the effect overlaps with both preceding and succeeding elements.
     type : WeibullType or str, by default WeibullType.PDF
         Type of Weibull adstock transformation to be applied (PDF or CDF).
 
     Returns
     -------
     tensor
         Transformed tensor based on Weibull adstock transformation.
@@ -370,15 +423,15 @@
         w = 1 - pt.exp(pm.Weibull.logcdf(t, k, lam))
         shape = (*w.shape[:-1], w.shape[-1] + 1)
         padded_w = pt.ones(shape, dtype=w.dtype)
         padded_w = pt.set_subtensor(padded_w[..., 1:], w)
         w = pt.cumprod(padded_w, axis=-1)
     else:
         raise ValueError(f"Wrong WeibullType: {type}, expected of WeibullType")
-    return batched_convolution(x, w, axis=axis)
+    return batched_convolution(x, w, axis=axis, mode=mode)
 
 
 def logistic_saturation(x, lam: npt.NDArray[np.float_] | float = 0.5):
     """Logistic saturation transformation.
 
     .. math::
         f(x) = \\frac{1 - e^{-\lambda x}}{1 + e^{-\lambda x}}
@@ -416,42 +469,75 @@
     tensor
         Transformed tensor.
     """  # noqa: W605
     return (1 - pt.exp(-lam * x)) / (1 + pt.exp(-lam * x))
 
 
 class TanhSaturationParameters(NamedTuple):
-    b: pt.TensorLike
-    """Saturation.
+    """Container for tanh saturation parameters.
+
+    Parameters
+    ----------
+    b : pt.TensorLike
+        Saturation
+    c : pt.TensorLike
+        Customer Aquisition Cost at 0.
+
     """
+
+    b: pt.TensorLike
     c: pt.TensorLike
-    """Customer Aquisition Cost at 0.
-    """
 
     def baseline(self, x0: pt.TensorLike) -> "TanhSaturationBaselinedParameters":
-        """Change the parameterization to baselined at :math:`x_0`."""
+        """Change the parameterization to baselined at :math:`x_0`.
+
+        Parameters
+        ----------
+        x0 : pt.TensorLike
+            Baseline spend.
+
+        Returns
+        -------
+        TanhSaturationBaselinedParameters
+            Baselined parameters.
+
+        """
         y_ref = tanh_saturation(x0, self.b, self.c)
         gain_ref = y_ref / x0
         r_ref = y_ref / self.b
         return TanhSaturationBaselinedParameters(x0, gain_ref, r_ref)
 
 
 class TanhSaturationBaselinedParameters(NamedTuple):
-    x0: pt.TensorLike
-    """Baseline spend.
+    """Representation of tanh saturation parameters in baselined form.
+
+    Parameters
+    ----------
+    x0 : pt.TensorLike
+        Baseline spend.
+    gain : pt.TensorLike
+        ROAS at :math:`x_0`.
+    r : pt.TensorLike
+        Overspend Fraction.
+
     """
+
+    x0: pt.TensorLike
     gain: pt.TensorLike
-    """ROAS at :math:`x_0`.
-    """
     r: pt.TensorLike
-    """Overspend Fraction.
-    """
 
     def debaseline(self) -> TanhSaturationParameters:
-        """Change the parameterization to baselined to be classic saturation and cac."""
+        """Change the parameterization to baselined to be classic saturation and cac.
+
+        Returns
+        -------
+        TanhSaturationParameters
+            Classic saturation and cac parameters.
+
+        """
         saturation = (self.gain * self.x0) / self.r
         cac = self.r / (self.gain * pt.arctanh(self.r))
         return TanhSaturationParameters(saturation, cac)
 
     def rebaseline(self, x1: pt.TensorLike) -> "TanhSaturationBaselinedParameters":
         """Change the parameterization to baselined at :math:`x_1`."""
         params = self.debaseline()
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/mmm/utils.py` & `pymc_marketing-0.6.0/pymc_marketing/mmm/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#   Copyright 2024 The PyMC Labs Developers
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 """Utility functions for the Marketing Mix Modeling module."""
 
 import re
 from collections.abc import Callable
 from typing import Any
 
 import numpy as np
@@ -276,14 +289,34 @@
         ).squeeze(dim="_")
 
     data.attrs = attrs
 
     return data
 
 
+def transform_1d_array(
+    transform: Callable[[pd.Series | np.ndarray], np.ndarray], y: pd.Series | np.ndarray
+) -> np.ndarray:
+    """Transform a 1D array using a scikit-learn transformer.
+
+    Parameters
+    ----------
+    transform : scikit-learn transformer
+        The transformer to apply to the data.
+    y : np.ndarray
+        The data to transform.
+
+    Returns
+    -------
+    np.ndarray
+        The transformed data.
+    """
+    return transform(np.array(y)[:, None]).flatten()
+
+
 def sigmoid_saturation(
     x: float | np.ndarray | npt.NDArray[np.float64],
     alpha: float | np.ndarray | npt.NDArray[np.float64],
     lam: float | np.ndarray | npt.NDArray[np.float64],
 ) -> float | Any:
     """
     Parameters
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing/model_builder.py` & `pymc_marketing-0.6.0/pymc_marketing/model_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright 2023 The PyMC Developers
+#   Copyright 2024 The PyMC Labs Developers
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -126,28 +126,25 @@
         >>>         try: # if y values in new data
         >>>             pm.set_data({'y_data': y.values})
         >>>         except: # dummies otherwise
         >>>             pm.set_data({'y_data': np.zeros(len(data))})
 
         """
 
-        raise NotImplementedError
-
     @property
     @abstractmethod
     def output_var(self):
         """
         Returns the name of the output variable of the model.
 
         Returns
         -------
         output_var : str
             Name of the output variable of the model.
         """
-        raise NotImplementedError
 
     @property
     @abstractmethod
     def default_model_config(self) -> dict:
         """
         Returns a class default config dict for model builder if no model_config is provided on class initialization
         Useful for understanding structure of required model_config to allow its customization by users
@@ -168,15 +165,14 @@
         >>>         }
 
         Returns
         -------
         model_config : dict
             A set of default parameters for predictor distributions that allow to save and recreate the model.
         """
-        raise NotImplementedError
 
     @property
     @abstractmethod
     def default_sampler_config(self) -> dict:
         """
         Returns a class default sampler dict for model builder if no sampler_config is provided on class initialization
         Useful for understanding structure of required sampler_config to allow its customization by users
@@ -192,15 +188,14 @@
         >>>         }
 
         Returns
         -------
         sampler_config : dict
             A set of default settings for used by model in fit process.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def _generate_and_preprocess_model_data(
         self, X: pd.DataFrame | pd.Series, y: np.ndarray
     ) -> None:
         """
         Applies preprocessing to the data before fitting the model.
@@ -225,15 +220,14 @@
         >>>         self.y = y
 
         Returns
         -------
         None
 
         """
-        raise NotImplementedError
 
     @abstractmethod
     def build_model(
         self,
         X: pd.DataFrame,
         y: pd.Series | np.ndarray,
         **kwargs,
@@ -260,21 +254,15 @@
         See Also
         --------
         default_model_config : returns default model config
 
         Returns
         -------
         None
-
-        Raises
-        ------
-        NotImplementedError
-            This is an abstract method and must be implemented in a subclass.
         """
-        raise NotImplementedError
 
     def set_idata_attrs(self, idata=None):
         """
         Set attributes on an InferenceData object.
 
         Parameters
         ----------
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing.egg-info/PKG-INFO` & `pymc_marketing-0.6.0/pymc_marketing.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-marketing
-Version: 0.5.0
+Version: 0.6.0
 Summary: Marketing Statistical Models in PyMC
 Maintainer-email: PyMC Labs <info@pymc-labs.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,24 +209,24 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: arviz>=0.13.0
 Requires-Dist: matplotlib>=3.5.1
 Requires-Dist: numpy>=1.17
 Requires-Dist: pandas
-Requires-Dist: pymc>=5.10.4
+Requires-Dist: pymc>=5.12.0
 Requires-Dist: scikit-learn>=1.1.1
 Requires-Dist: seaborn>=0.12.2
 Requires-Dist: xarray
 Requires-Dist: xarray-einstats>=0.5.1
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: ipython!=8.7.0; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
-Requires-Dist: myst-nb; extra == "docs"
+Requires-Dist: myst-nb<=1.0.0; extra == "docs"
 Requires-Dist: pydata-sphinx-theme>=0.12.0.dev0; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinxext-opengraph; extra == "docs"
 Requires-Dist: sphinx-notfound-page; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
 Provides-Extra: lint
@@ -243,27 +243,45 @@
 
 ![PyMC-Marketing Logo](docs/source/_static/marketing-logo-light.jpg)
 
 </div>
 
 ----
 
-![Build](https://github.com/pymc-labs/pymc-marketing/workflows/ci/badge.svg)
+![Build](https://github.com/pymc-labs/pymc-marketing/actions/workflows/ci.yml/badge.svg)
 [![codecov](https://codecov.io/gh/pymc-labs/pymc-marketing/branch/main/graph/badge.svg?token=OBV3BS5TYE)](https://codecov.io/gh/pymc-labs/pymc-marketing)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![docs](https://readthedocs.org/projects/pymc-marketing/badge/?version=latest)](https://docs.readthedocs.io/en/latest/)
 [![PyPI Version](https://img.shields.io/pypi/v/pymc-marketing.svg)](https://pypi.python.org/pypi/pymc-marketing)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pymc-marketing.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 # <span style="color:limegreen">PyMC-Marketing</span>: Bayesian Marketing Mix Modeling (MMM) & Customer Lifetime Value (CLV)
 
 ## Marketing Analytics Tools from [PyMC Labs](https://www.pymc-labs.com)
 
 Unlock the power of **Marketing Mix Modeling (MMM)** and **Customer Lifetime Value (CLV)** analytics with PyMC-Marketing. This open-source marketing analytics tool empowers businesses to make smarter, data-driven decisions for maximizing ROI in marketing campaigns.
 
+----
+
+This repository is supported by [PyMC Labs](https://www.pymc-labs.com).
+
+<center>
+    <img src="docs/source/_static/labs-logo-light.png" width="50%" />
+</center>
+
+For businesses looking to integrate PyMC-Marketing into their operational framework, [PyMC Labs](https://www.pymc-labs.com) offers expert consulting and training. Our team is proficient in state-of-the-art Bayesian modeling techniques, with a focus on Marketing Mix Models (MMMs) and Customer Lifetime Value (CLV). For more information see [here](#-schedule-a-free-consultation-for-mmm--clv-strategy).
+
+Explore these topics further by watching our video on [Bayesian Marketing Mix Models: State of the Art](https://www.youtube.com/watch?v=xVx91prC81g).
+
+### Community Resources
+
+- [Bayesian discord server](https://discord.gg/swztKRaVKe)
+- [PyMC discourse](https://discourse.pymc.io/)
+
 ## Quick Installation Guide for Marketing Mix Modeling (MMM) & CLV
 
 To dive into MMM and CLV analytics, set up a specialized environment, `marketing_env`, via conda-forge:
 
 ```bash
 conda create -c conda-forge -n marketing_env pymc-marketing
 conda activate marketing_env
@@ -275,67 +293,133 @@
 
 We provide a `Dockerfile` to build a Docker image for PyMC-Marketing so that is accessible from a Jupyter Notebook. See [here](/scripts/docker/README.md) for more details.
 
 ## In-depth Bayesian Marketing Mix Modeling (MMM) in PyMC
 
 Leverage our Bayesian MMM API to tailor your marketing strategies effectively. Based on the research [Jin, Yuxue, et al. “Bayesian methods for media mix modeling with carryover and shape effects.” (2017)](https://research.google/pubs/pub46001/),  and integrating the expertise from core PyMC developers, our API provides:
 
+- **Custom Priors and Likelihoods**: Tailor your model to your specific business needs by including domain knowledge via prior distributions.
 - **Adstock Transformation**: Optimize the carry-over effects in your marketing channels.
 - **Saturation Effects**: Understand the diminishing returns in media investments.
+- **Time-varying Intercept:** Capture time-varying baseline contributions in your model (using modern and efficient Gaussian processes approximation methods).
+- **Visualization and Model Diagnostics**: Get a comprehensive view of your model's performance and insights.
+- **Out-of-sample Predictions**: Forecast future marketing performance with credible intervals. Use this for simulations and scenario planning.
 - **Budget Optimization**: Allocate your marketing spend efficiently across various channels for maximum ROI.
 - **Experiment Calibration**: Fine-tune your model based on empirical experiments for a more unified view of marketing.
 
+### MMM Quickstart
+
+```python
+import pandas as pd
+from pymc_marketing.mmm import DelayedSaturatedMMM
+
+data_url = "https://raw.githubusercontent.com/pymc-labs/pymc-marketing/main/data/mmm_example.csv"
+data = pd.read_csv(data_url, parse_dates=['date_week'])
+
+mmm = DelayedSaturatedMMM(
+    date_column="date_week",
+    channel_columns=["x1", "x2"],
+    control_columns=[
+        "event_1",
+        "event_2",
+        "t",
+    ],
+    adstock_max_lag=8,
+    yearly_seasonality=2,
+)
+```
+
+Initiate fitting and get a visualization of some of the outputs with:
+
+```python
+X = data.drop("y",axis=1)
+y = data["y"]
+mmm.fit(X,y)
+mmm.plot_components_contributions();
+```
+
+![](/docs/source/_static/mmm_plot_components_contributions.png)
+
+Once the model is fitted, we can further optimize our budget allocation as we are including diminishing returns and carry-over effects in our model.
+
+<center>
+    <img src="/docs/source/_static/mmm_plot_plot_channel_contributions_grid.png" width="80%" />
+</center>
+
 Explore a hands-on [simulated example](https://pymc-marketing.readthedocs.io/en/stable/notebooks/mmm/mmm_example.html) for more insights into MMM with PyMC-Marketing.
 
 ### Essential Reading for Marketing Mix Modeling (MMM)
 
 - [Bayesian Media Mix Modeling for Marketing Optimization](https://www.pymc-labs.com/blog-posts/bayesian-media-mix-modeling-for-marketing-optimization/)
 - [Improving the Speed and Accuracy of Bayesian Marketing Mix Models](https://www.pymc-labs.com/blog-posts/reducing-customer-acquisition-costs-how-we-helped-optimizing-hellofreshs-marketing-budget/)
 - [Johns, Michael and Wang,  Zhenyu. "A Bayesian Approach to Media Mix Modeling"](https://www.youtube.com/watch?v=UznM_-_760Y)
 - [Orduz, Juan. "Media Effect Estimation with PyMC: Adstock, Saturation & Diminishing Returns"](https://juanitorduz.github.io/pymc_mmm/)
-- [A Comprehensive Guide to Bayesian Marketing Mix Modeling](https://1749.io/resource-center/f/a-comprehensive-guide-to-bayesian-marketing-mix-modeling)
+- [A Comprehensive Guide to Bayesian Marketing Mix Modeling](https://1749.io/learn/f/a-comprehensive-guide-to-bayesian-marketing-mix-modeling)
 
 ## Unlock Customer Lifetime Value (CLV) with PyMC
 
 Understand and optimize your customer's value with our **CLV models**. Our API supports various types of CLV models, catering to both contractual and non-contractual settings, as well as continuous and discrete transaction modes.
 
 Explore our detailed CLV examples using data from the [`lifetimes`](https://github.com/CamDavidsonPilon/lifetimes) package:
 
 - [CLV Quickstart](https://pymc-marketing.readthedocs.io/en/stable/notebooks/clv/clv_quickstart.html)
 - [BG/NBD model](https://pymc-marketing.readthedocs.io/en/stable/notebooks/clv/bg_nbd.html)
+- [Pareto/NBD model](https://pymc-marketing.readthedocs.io/en/stable/notebooks/clv/pareto_nbd.html)
 - [Gamma-Gamma model](https://pymc-marketing.readthedocs.io/en/stable/notebooks/clv/gamma_gamma.html)
 
 ### Examples
 
 |                | **Non-contractual** | **Contractual**                 |
 |----------------|---------------------|---------------------------------|
 | **Continuous** | Buying groceries    | Audible                         |
 | **Discrete**   | Cinema ticket       | Monthly or yearly subscriptions |
 
----
+### CLV Quickstart
+
+```python
+import matplotlib.pyplot as plt
+import pandas as pd
+import seaborn as sns
+from pymc_marketing import clv
+
+data_url = "https://raw.githubusercontent.com/pymc-labs/pymc-marketing/main/data/clv_quickstart.csv"
+data = pd.read_csv(data_url)
+data["customer_id"] = data.index
+
+beta_geo_model = clv.BetaGeoModel(data=data)
+
+beta_geo_model.fit()
+```
+
+Once fitted, we can use the model to predict the number of future purchases for known customers, the probability that they are still alive, and get various visualizations plotted.
+
+![](/docs/source/_static/expected_purchases.png)
+
+See the Examples section for more on this.
 
 ## Why PyMC-Marketing vs other solutions?
 
 PyMC-Marketing is and will always be free for commercial use, licensed under [Apache 2.0](LICENSE). Developed by core developers behind the popular PyMC package and marketing experts, it provides state-of-the-art measurements and analytics for marketing teams.
 
-Due to its open-source nature and active contributor base, new features are added constantly. Missing a feature or want to contribute? Fork our repository and submit a pull request. For any questions, feel free to [open an issue](https://github.com/your-repo/issues).
+Due to its open-source nature and active contributor base, new features are constantly added. Are you missing a feature or want to contribute? Fork our repository and submit a pull request. If you have any questions, feel free to [open an issue](https://github.com/your-repo/issues).
+
+### Thanks to our contributors!
+
+[![https://github.com/pymc-devs/pymc/graphs/contributors](https://contrib.rocks/image?repo=pymc-labs/pymc-marketing)](https://github.com/pymc-labs/pymc-marketing/graphs/contributors)
+
 
 ## Marketing AI Assistant: MMM-GPT with PyMC-Marketing
 
 Not sure how to start or have questions? MMM-GPT is an AI that answers questions and provides expert advice on marketing analytics using PyMC-Marketing.
 
 **[Try MMM-GPT here.](https://mmm-gpt.com/)**
 
-
-
 ## 📞 Schedule a Free Consultation for MMM & CLV Strategy
 
 Maximize your marketing ROI with a [free 30-minute strategy session](https://calendly.com/niall-oulton) with our PyMC-Marketing experts. Learn how Bayesian Marketing Mix Modeling and Customer Lifetime Value analytics can boost your organization by making smarter, data-driven decisions.
 
-For businesses looking to integrate PyMC-Marketing into their operational framework, [PyMC Labs](https://www.pymc-labs.com) offers expert consulting and training. Our team is proficient in state-of-the-art Bayesian modeling techniques, with a focus on Marketing Mix Models (MMMs) and Customer Lifetime Value (CLV). Explore these topics further by watching our video on [Bayesian Marketing Mix Models: State of the Art](https://www.youtube.com/watch?v=xVx91prC81g).
-
 We provide the following professional services:
 
 - **Custom Models**: We tailor niche marketing analytics models to fit your organization's unique needs.
 - **Build Within PyMC-Marketing**: Our team members are experts leveraging the capabilities of PyMC-Marketing to create robust marketing models for precise insights.
 - **SLA & Coaching**: Get guaranteed support levels and personalized coaching to ensure your team is well-equipped and confident in using our tools and approaches.
 - **SaaS Solutions**: Harness the power of our state-of-the-art software solutions to streamline your data-driven marketing initiatives.
```

### Comparing `pymc_marketing-0.5.0/pymc_marketing.egg-info/SOURCES.txt` & `pymc_marketing-0.6.0/pymc_marketing.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 pymc_marketing/__init__.py
+pymc_marketing/constants.py
 pymc_marketing/model_builder.py
 pymc_marketing/version.py
 pymc_marketing/version.txt
 pymc_marketing.egg-info/PKG-INFO
 pymc_marketing.egg-info/SOURCES.txt
 pymc_marketing.egg-info/dependency_links.txt
 pymc_marketing.egg-info/requires.txt
@@ -23,9 +24,10 @@
 pymc_marketing/mmm/__init__.py
 pymc_marketing/mmm/base.py
 pymc_marketing/mmm/budget_optimizer.py
 pymc_marketing/mmm/delayed_saturated_mmm.py
 pymc_marketing/mmm/lift_test.py
 pymc_marketing/mmm/preprocessing.py
 pymc_marketing/mmm/transformers.py
+pymc_marketing/mmm/tvp.py
 pymc_marketing/mmm/utils.py
 pymc_marketing/mmm/validating.py
```

### Comparing `pymc_marketing-0.5.0/pyproject.toml` & `pymc_marketing-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 maintainers = [{ name = "PyMC Labs", email = "info@pymc-labs.io" }]
 
 dependencies = [
     "arviz>=0.13.0",
     "matplotlib>=3.5.1",
     "numpy>=1.17",
     "pandas",
-    # NOTE: Keep minimum pymc version in sync with ci.yml `OLDEST_PYMC_VERSION`
-    "pymc>=5.10.4",
+    # NOTE: Used as minimum pymc version with ci.yml `OLDEST_PYMC_VERSION`
+    "pymc>=5.12.0",
     "scikit-learn>=1.1.1",
     "seaborn>=0.12.2",
     "xarray",
     "xarray-einstats>=0.5.1",
 ]
 
 [project.optional-dependencies]
 docs = [
     "sphinx",
     "ipython!=8.7.0",
     "myst-parser",
-    "myst-nb",
+    "myst-nb<=1.0.0",
     "pydata-sphinx-theme>=0.12.0.dev0",
     "sphinx-copybutton",
     "sphinx-autodoc-typehints",
     "sphinxext-opengraph",
     "sphinx-notfound-page",
     "sphinx-design",
 ]
```

