# Comparing `tmp/treat_sim-1.1.1.tar.gz` & `tmp/treat_sim-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treat_sim-1.1.1.tar", last modified: Wed May  1 16:04:26 2024, max compression
+gzip compressed data, was "treat_sim-1.2.0.tar", last modified: Wed May  8 10:57:28 2024, max compression
```

## Comparing `treat_sim-1.1.1.tar` & `treat_sim-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:04:26.666568 treat_sim-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-01 16:04:22.000000 treat_sim-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 16:04:22.000000 treat_sim-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-01 16:04:26.666568 treat_sim-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-05-01 16:04:22.000000 treat_sim-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-01 16:04:22.000000 treat_sim-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:04:26.666568 treat_sim-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-01 16:04:22.000000 treat_sim-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:04:26.666568 treat_sim-1.1.1/treat_sim/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 16:04:22.000000 treat_sim-1.1.1/treat_sim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:04:26.666568 treat_sim-1.1.1/treat_sim/data/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-01 16:04:22.000000 treat_sim-1.1.1/treat_sim/data/ed_arrivals.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-01 16:04:22.000000 treat_sim-1.1.1/treat_sim/distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    38338 2024-05-01 16:04:22.000000 treat_sim-1.1.1/treat_sim/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:04:26.666568 treat_sim-1.1.1/treat_sim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-01 16:04:26.000000 treat_sim-1.1.1/treat_sim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 16:04:26.000000 treat_sim-1.1.1/treat_sim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:04:26.000000 treat_sim-1.1.1/treat_sim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-01 16:04:26.000000 treat_sim-1.1.1/treat_sim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 16:04:26.000000 treat_sim-1.1.1/treat_sim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:57:28.296830 treat_sim-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-08 10:57:24.000000 treat_sim-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 10:57:24.000000 treat_sim-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-08 10:57:28.296830 treat_sim-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-08 10:57:24.000000 treat_sim-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 10:57:24.000000 treat_sim-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 10:57:28.296830 treat_sim-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-08 10:57:24.000000 treat_sim-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:57:28.296830 treat_sim-1.2.0/treat_sim/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 10:57:24.000000 treat_sim-1.2.0/treat_sim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:57:28.296830 treat_sim-1.2.0/treat_sim/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-08 10:57:24.000000 treat_sim-1.2.0/treat_sim/data/ed_arrivals.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-08 10:57:24.000000 treat_sim-1.2.0/treat_sim/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38343 2024-05-08 10:57:24.000000 treat_sim-1.2.0/treat_sim/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:57:28.296830 treat_sim-1.2.0/treat_sim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-08 10:57:28.000000 treat_sim-1.2.0/treat_sim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-08 10:57:28.000000 treat_sim-1.2.0/treat_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:57:28.000000 treat_sim-1.2.0/treat_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 10:57:28.000000 treat_sim-1.2.0/treat_sim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 10:57:28.000000 treat_sim-1.2.0/treat_sim.egg-info/top_level.txt
```

### Comparing `treat_sim-1.1.1/LICENSE` & `treat_sim-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `treat_sim-1.1.1/PKG-INFO` & `treat_sim-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treat-sim
-Version: 1.1.1
+Version: 1.2.0
 Summary: A free and open implementation of the Treatment Centre Model from Nelson (2013)
 Home-page: https://github.com/pythonhealthdatascience/stars-treat-sim
 Author: Thomas Monks
 Author-email: forecast-tools@gmail.com
 License: The MIT License (MIT)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,33 +18,33 @@
 Requires-Dist: numpy>=1.19.2
 Requires-Dist: pandas>=1.2.3
 Requires-Dist: scipy>=1.6.1
 Requires-Dist: simpy>=4.0.1
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pythonhealthdatascience/stars-treat-sim/HEAD)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-360+/)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10026327.svg)](https://doi.org/10.5281/zenodo.10026327)
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380+/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10026326.svg)](https://doi.org/10.5281/zenodo.10026326)
 [![PyPI version fury.io](https://badge.fury.io/py/treat-sim.svg)](https://pypi.org/project/treat-sim/)
 
 [<img src="https://img.shields.io/static/v1?label=dockerhub&message=images&color=important?style=for-the-badge&logo=docker">](https://hub.docker.com/r/tommonks01/treat_sim)
 
 
 # Towards Sharing Tools, and Artifacts, for Reusable Simulation: a minimal model example
 
 ## Overview
 
-The materials and methods in this repository support work towards developing the S.T.A.R.S healthcare framework (**S**haring **T**ools and **A**rtifacts for **R**euable **S**imulations in healthcare).  The code and written materials here demonstrate the application of S.T.A.R.S' version 1 to sharing a `simpy` discrete-event simuilation model and associated research artifacts.  
+The materials and methods in this repository support work towards developing the S.T.A.R.S healthcare framework (**S**haring **T**ools and **A**rtifacts for **R**eusable **S**imulations in healthcare).  The code and written materials here demonstrate the application of S.T.A.R.S' version 1 to sharing a `SimPy` discrete-event simulation model and associated research artifacts.  
 
 * All artifacts in this repository are linked to study researchers via ORCIDs;
 * Model code is made available under an MIT license;
-* Python dependencies are managed through `conda`;`
+* Python dependencies are managed through `conda`;
 * Documentation of the model is enhanced using a Jupyter notebook.
 * The python code itself can be viewed and executed in Jupyter notebooks via [Binder](https://mybinder.org); 
-* The materials are deposited and made citatable using Zenodo;
+* The materials are deposited and made citable using Zenodo;
 * The model is sharable with other researchers and the NHS without the need to install software.
 
 ## Author ORCIDs
 
 [![ORCID: Harper](https://img.shields.io/badge/ORCID-0000--0001--5274--5037-brightgreen)](https://orcid.org/0000-0001-5274-5037)
 [![ORCID: Monks](https://img.shields.io/badge/ORCID-0000--0003--2631--4481-brightgreen)](https://orcid.org/0000-0003-2631-4481)
 
@@ -54,46 +54,45 @@
 
 ## Instructions to run the model
 
 ### Online Notebooks via Binder
 
 The python code for the model has been setup to run online in Jupyter notebooks via binder [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pythonhealthdatascience/stars-treat-sim/HEAD)
 
-> mybinder.org is a free tier service.  If it has not been used in a while Binder will need to re-containerise the code repository, and push to binderhub. This will take several minutes. After that the online environment will be quick to load.
+> mybinder.org is a free tier service.  If it has not been used in a while Binder will need to re-containerise the code repository, and push to BinderHub. This will take several minutes. After that the online environment will be quick to load.
 
 ### To download code and run locally
 
 #### Downloading the code
 
 Either clone the repository using git or click on the green "code" button and select "Download Zip".
 
 ```bash
 git clone https://github.com/pythonhealthdatascience/stars-treat-sim
 ```
 
 #### Installing dependencies
 
-[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
 All dependencies can be found in [`binder/environment.yml`]() and are pulled from conda-forge.  To run the code locally, we recommend install [mini-conda](https://docs.conda.io/en/latest/miniconda.html); navigating your terminal (or cmd prompt) to the directory containing the repo and issuing the following command:
 
 ```
 conda env create -f binder/environment.yml
 ```
 
-Activate the conda environment using the following command
+Activate the conda environment using the following command:
 
 ```
 conda activate stars_treat_sim
 ```
 
 #### Running the model
 
-To run 50 multiple replications of across a number of example experiments use the following code
-
+To run 50 multiple replications across a number of example experiments, use the following code:
 
 ```python
 from treat_sim.model import (get_scenarios, run_scenario_analysis,
                              scenario_summary_frame, 
                              DEFAULT_RESULTS_COLLECTION_PERIOD)
 
 if __name__ == '__main__':
@@ -103,36 +102,37 @@
                                     n_reps=50)
 
     results_summary = scenario_summary_frame(results)
     print(results_summary)
 
 ```
 
-Alternative you can design and execute individual experiments by creating a `Scenario` object
+Alternative you can design and execute individual experiments by creating a `Scenario` object:
 
 ```python
 from treat_sim.model import Scenario, multiple_replications
 
 if __name__ == '__main__':
 
     # use all default parameter values
     base_case = Scenario()
 
     results = multiple_replications(base_case).describe().round(2).T
     print(results)
 
 ```
 
-
 ## Repo overview
 
 ```
 .
 ├── binder
 │   └── environment.yml
+├── CHANGES.md
+├── CITATION.cff
 ├── LICENSE
 ├── MANIFEST.in
 ├── notebooks
 │   └── test_package.ipynb
 ├── README.md
 ├── requirements.txt
 ├── setup.py
@@ -140,34 +140,43 @@
     ├── data
     │   └── ed_arrivals.csv
     ├── distributions.py
     ├── __init__.py
     └── model.py
 ```
 
-* `binder` - contains the environment.yml file (sim) and all dependencies managed via conda
-* `data` - directory containing data files used by analysis notebooks. 
+* `binder/` - contains the environment.yml file (sim) and all dependencies managed via conda, used to set-up the notebooks on Binder.
+* `CHANGES.md` - changelog with record of notable changes to project between versions.
+* `CITATION.cff` - citation information for the package.
 * `LICENSE` - details of the MIT permissive license of this work.
-* `notebooks` - contains a notebook to run the model and provides basic enhanced model documentation.
-* `main.py` - an example simpy model to use to test the virtual environment 
-* `README` - what you are reading now!
-* `treat_sim` - contains a packaged version of the model.
-
+* `MANIFEST.in` - files to include in the package.
+* `notebooks/` - contains a notebook to run the model and provides basic enhanced model documentation.
+* `README.md` - what you are reading now!
+* `requirements.txt` - list of packages and minimum versions required.
+* `setup.py` - used to build and distribute package.
+* `treat_sim/` - contains packaged version of the model.
+    * `data/` - directory containing data file used by package.
+    * `distributions.py` - distribution classes.
+    * `__init__.py` - required as part of package - contains author and version.
+    * `model.py` - example SimPy model.
 
 ## Citation
 
 If you use the materials within this repository we would appreciate a citation.
 
+```
+Monks, T., Harper, A., & Heather, A. (2024). Towards Sharing Tools, and Artifacts, for Reusable Simulation: a minimal model example (v1.2.0). Zenodo. https://doi.org/10.5281//zenodo.10026326
+```
+
 ```bibtex
-@software{monks_2023_10026327,
-  author       = {Monks, Thomas and
-                  Harper, Alison},
+@software{stars_treat_sim,
+  author       = {Thomas Monks, Alison Harper and Amy Heather},
   title        = {{Towards Sharing Tools, and Artifacts, for Reusable 
-                   Simulation: a minimal model examplar}},
-  month        = oct,
-  year         = 2023,
+                   Simulation: a minimal model example}},
+  month        = May,
+  year         = 2024,
   publisher    = {Zenodo},
-  version      = {v1.0.0},
-  url 	       = {https://zenodo.org/records/10026327}
+  version      = {v1.2.0},
+  doi          = {10.5281//zenodo.10026326.},
+  url          = {https://doi.org/10.5281//zenodo.10026326}
 }
 ```
-
```

### Comparing `treat_sim-1.1.1/README.md` & `treat_sim-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pythonhealthdatascience/stars-treat-sim/HEAD)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-360+/)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10026327.svg)](https://doi.org/10.5281/zenodo.10026327)
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380+/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10026326.svg)](https://doi.org/10.5281/zenodo.10026326)
 [![PyPI version fury.io](https://badge.fury.io/py/treat-sim.svg)](https://pypi.org/project/treat-sim/)
 
 [<img src="https://img.shields.io/static/v1?label=dockerhub&message=images&color=important?style=for-the-badge&logo=docker">](https://hub.docker.com/r/tommonks01/treat_sim)
 
 
 # Towards Sharing Tools, and Artifacts, for Reusable Simulation: a minimal model example
 
 ## Overview
 
-The materials and methods in this repository support work towards developing the S.T.A.R.S healthcare framework (**S**haring **T**ools and **A**rtifacts for **R**euable **S**imulations in healthcare).  The code and written materials here demonstrate the application of S.T.A.R.S' version 1 to sharing a `simpy` discrete-event simuilation model and associated research artifacts.  
+The materials and methods in this repository support work towards developing the S.T.A.R.S healthcare framework (**S**haring **T**ools and **A**rtifacts for **R**eusable **S**imulations in healthcare).  The code and written materials here demonstrate the application of S.T.A.R.S' version 1 to sharing a `SimPy` discrete-event simulation model and associated research artifacts.  
 
 * All artifacts in this repository are linked to study researchers via ORCIDs;
 * Model code is made available under an MIT license;
-* Python dependencies are managed through `conda`;`
+* Python dependencies are managed through `conda`;
 * Documentation of the model is enhanced using a Jupyter notebook.
 * The python code itself can be viewed and executed in Jupyter notebooks via [Binder](https://mybinder.org); 
-* The materials are deposited and made citatable using Zenodo;
+* The materials are deposited and made citable using Zenodo;
 * The model is sharable with other researchers and the NHS without the need to install software.
 
 ## Author ORCIDs
 
 [![ORCID: Harper](https://img.shields.io/badge/ORCID-0000--0001--5274--5037-brightgreen)](https://orcid.org/0000-0001-5274-5037)
 [![ORCID: Monks](https://img.shields.io/badge/ORCID-0000--0003--2631--4481-brightgreen)](https://orcid.org/0000-0003-2631-4481)
 
@@ -32,46 +32,45 @@
 
 ## Instructions to run the model
 
 ### Online Notebooks via Binder
 
 The python code for the model has been setup to run online in Jupyter notebooks via binder [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pythonhealthdatascience/stars-treat-sim/HEAD)
 
-> mybinder.org is a free tier service.  If it has not been used in a while Binder will need to re-containerise the code repository, and push to binderhub. This will take several minutes. After that the online environment will be quick to load.
+> mybinder.org is a free tier service.  If it has not been used in a while Binder will need to re-containerise the code repository, and push to BinderHub. This will take several minutes. After that the online environment will be quick to load.
 
 ### To download code and run locally
 
 #### Downloading the code
 
 Either clone the repository using git or click on the green "code" button and select "Download Zip".
 
 ```bash
 git clone https://github.com/pythonhealthdatascience/stars-treat-sim
 ```
 
 #### Installing dependencies
 
-[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
 All dependencies can be found in [`binder/environment.yml`]() and are pulled from conda-forge.  To run the code locally, we recommend install [mini-conda](https://docs.conda.io/en/latest/miniconda.html); navigating your terminal (or cmd prompt) to the directory containing the repo and issuing the following command:
 
 ```
 conda env create -f binder/environment.yml
 ```
 
-Activate the conda environment using the following command
+Activate the conda environment using the following command:
 
 ```
 conda activate stars_treat_sim
 ```
 
 #### Running the model
 
-To run 50 multiple replications of across a number of example experiments use the following code
-
+To run 50 multiple replications across a number of example experiments, use the following code:
 
 ```python
 from treat_sim.model import (get_scenarios, run_scenario_analysis,
                              scenario_summary_frame, 
                              DEFAULT_RESULTS_COLLECTION_PERIOD)
 
 if __name__ == '__main__':
@@ -81,36 +80,37 @@
                                     n_reps=50)
 
     results_summary = scenario_summary_frame(results)
     print(results_summary)
 
 ```
 
-Alternative you can design and execute individual experiments by creating a `Scenario` object
+Alternative you can design and execute individual experiments by creating a `Scenario` object:
 
 ```python
 from treat_sim.model import Scenario, multiple_replications
 
 if __name__ == '__main__':
 
     # use all default parameter values
     base_case = Scenario()
 
     results = multiple_replications(base_case).describe().round(2).T
     print(results)
 
 ```
 
-
 ## Repo overview
 
 ```
 .
 ├── binder
 │   └── environment.yml
+├── CHANGES.md
+├── CITATION.cff
 ├── LICENSE
 ├── MANIFEST.in
 ├── notebooks
 │   └── test_package.ipynb
 ├── README.md
 ├── requirements.txt
 ├── setup.py
@@ -118,34 +118,43 @@
     ├── data
     │   └── ed_arrivals.csv
     ├── distributions.py
     ├── __init__.py
     └── model.py
 ```
 
-* `binder` - contains the environment.yml file (sim) and all dependencies managed via conda
-* `data` - directory containing data files used by analysis notebooks. 
+* `binder/` - contains the environment.yml file (sim) and all dependencies managed via conda, used to set-up the notebooks on Binder.
+* `CHANGES.md` - changelog with record of notable changes to project between versions.
+* `CITATION.cff` - citation information for the package.
 * `LICENSE` - details of the MIT permissive license of this work.
-* `notebooks` - contains a notebook to run the model and provides basic enhanced model documentation.
-* `main.py` - an example simpy model to use to test the virtual environment 
-* `README` - what you are reading now!
-* `treat_sim` - contains a packaged version of the model.
-
+* `MANIFEST.in` - files to include in the package.
+* `notebooks/` - contains a notebook to run the model and provides basic enhanced model documentation.
+* `README.md` - what you are reading now!
+* `requirements.txt` - list of packages and minimum versions required.
+* `setup.py` - used to build and distribute package.
+* `treat_sim/` - contains packaged version of the model.
+    * `data/` - directory containing data file used by package.
+    * `distributions.py` - distribution classes.
+    * `__init__.py` - required as part of package - contains author and version.
+    * `model.py` - example SimPy model.
 
 ## Citation
 
 If you use the materials within this repository we would appreciate a citation.
 
+```
+Monks, T., Harper, A., & Heather, A. (2024). Towards Sharing Tools, and Artifacts, for Reusable Simulation: a minimal model example (v1.2.0). Zenodo. https://doi.org/10.5281//zenodo.10026326
+```
+
 ```bibtex
-@software{monks_2023_10026327,
-  author       = {Monks, Thomas and
-                  Harper, Alison},
+@software{stars_treat_sim,
+  author       = {Thomas Monks, Alison Harper and Amy Heather},
   title        = {{Towards Sharing Tools, and Artifacts, for Reusable 
-                   Simulation: a minimal model examplar}},
-  month        = oct,
-  year         = 2023,
+                   Simulation: a minimal model example}},
+  month        = May,
+  year         = 2024,
   publisher    = {Zenodo},
-  version      = {v1.0.0},
-  url 	       = {https://zenodo.org/records/10026327}
+  version      = {v1.2.0},
+  doi          = {10.5281//zenodo.10026326.},
+  url          = {https://doi.org/10.5281//zenodo.10026326}
 }
 ```
-
```

### Comparing `treat_sim-1.1.1/setup.py` & `treat_sim-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `treat_sim-1.1.1/treat_sim/distributions.py` & `treat_sim-1.2.0/treat_sim/distributions.py`

 * *Files identical despite different names*

### Comparing `treat_sim-1.1.1/treat_sim/model.py` & `treat_sim-1.2.0/treat_sim/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,32 +11,33 @@
 non-stationary poisson process. After 12am arriving patients are diverted 
 elsewhere and remaining WIP is completed.  
 On arrival, all patients quickly sign-in and are triaged.   
 
 The health clinic expects two types of patient arrivals: 
 
 **Trauma arrivals:**
-patients with severe illness and trauma that must first be stablised in a 
+patients with severe illness and trauma that must first be stabilised in a 
 trauma room. These patients then undergo treatment in a cubicle before being 
 discharged.
 
 **Non-trauma arrivals**
 patients with minor illness and no trauma go through registration and 
 examination activities. A proportion of non-trauma patients require treatment
-in a cubicle before being dicharged. 
+in a cubicle before being discharged. 
 
 In this model treatment of trauma and non-trauma patients is modelled seperately 
 '''
 
 import numpy as np
 import pandas as pd
 import itertools
 import simpy
 
-from treat_sim.distributions import (Exponential, Normal, Uniform, Bernoulli, Lognormal)
+from treat_sim.distributions import (
+    Exponential, Normal, Uniform, Bernoulli, Lognormal)
 
 # Constants and defaults for modelling **as-is**
 
 # Distribution parameters
 
 # sign-in/triage parameters
 DEFAULT_TRIAGE_MEAN = 3.0
@@ -67,16 +68,16 @@
 DEFAULT_PROB_TRAUMA = 0.12
 
 
 # Time dependent arrival rates data
 # The data for arrival rates varies between clinic opening at 6am and closure at
 # 12am.
 
-NSPP_PATH = 'https://raw.githubusercontent.com/TomMonks/' \
- + 'open-science-for-sim/main/src/notebooks/01_foss_sim/data/ed_arrivals.csv'
+NSPP_PATH = 'https://raw.githubusercontent.com/pythonhealthdatascience/' \
+ + 'stars-treat-sim/main/treat_sim/data/ed_arrivals.csv'
 
 # Resource counts
 
 DEFAULT_N_TRIAGE = 1
 DEFAULT_N_REG = 1
 DEFAULT_N_EXAM = 3
 DEFAULT_N_TRAUMA = 2
@@ -199,15 +200,15 @@
         n_reg: int
             The number of registration clerks
             
         n_exam: int
             The number of examination rooms
             
         n_trauma: int
-            The number of trauma bays for stablisation
+            The number of trauma bays for stabilisation
             
         n_cubicles_1: int
             The number of non-trauma treatment cubicles
             
         n_cubicles_2: int
             The number of trauma treatment cubicles
             
@@ -272,15 +273,15 @@
     
     def set_random_no_set(self, random_number_set):
         '''
         Controls the random sampling 
         Parameters:
         ----------
         random_number_set: int
-            Used to control the set of psuedo random numbers
+            Used to control the set of pseudo random numbers
             used by the distributions in the simulation.
         '''
         self.random_number_set = random_number_set
         self.init_sampling()
 
     def init_resourse_counts(self, n_triage, n_reg, n_exam, n_trauma,
                              n_cubicles_1, n_cubicles_2):
@@ -510,15 +511,15 @@
         Constructor method
         
         Params:
         -----
         identifier: int
             a numeric identifier for the patient.
             
-        env: simpy.Environment
+        env: SimPy.Environment
             the simulation environment
             
         args: Scenario
             Container class for the simulation parameters
             
         '''
         self.identifier = identifier
@@ -645,15 +646,15 @@
     The treatment centre model
     
     Patients arrive at random to a treatment centre, are triaged
     and then processed in either a trauma or non-trauma pathway.
 
     The main class that a user interacts with to run the model is 
     `TreatmentCentreModel`.  This implements a `.run()` method, contains a simple
-    algorithm for the non-stationary poission process for patients arrivals and 
+    algorithm for the non-stationary Poisson process for patients arrivals and 
     inits instances of `TraumaPathway` or `NonTraumaPathway` depending on the 
     arrival type.    
 
     '''
     def __init__(self, args):
         self.env = simpy.Environment()
         self.args = args
@@ -725,15 +726,15 @@
         Returns:
         --------
             None
         '''
         # setup the arrival generator process
         self.env.process(self.arrivals_generator())
         
-        # store rc perio
+        # store rc period
         self.rc_period = results_collection_period
         
         # run
         self.env.run(until=results_collection_period)
         
     
     def arrivals_generator(self):  
@@ -748,15 +749,15 @@
         '''
         for patient_count in itertools.count():
 
             # this give us the index of dataframe to use
             t = int(self.env.now // 60) % self.args.arrivals.shape[0]
             lambda_t = self.args.arrivals['arrival_rate'].iloc[t]
 
-            #set to a large number so that at least 1 sample taken!
+            # set to a large number so that at least 1 sample taken!
             u = np.Inf
             
             interarrival_time = 0.0
 
             # reject samples if u >= lambda_t / lambda_max
             while u >= (lambda_t / self.args.lambda_max):
                 interarrival_time += self.args.arrival_dist.sample()
@@ -852,15 +853,15 @@
                                                 self.model.trauma_patients)
         
         # trauma utilisation (trauma)
         trauma_util = self.get_resource_util('trauma_duration', 
                                              self.args.n_trauma, 
                                              self.model.trauma_patients)
         
-        # mean waiting time for treatment (rauma) 
+        # mean waiting time for treatment (trauma) 
         mean_treat_wait2 = self.get_mean_metric('wait_treat', 
                                                 self.model.trauma_patients)
         
         # treatment utilisation (trauma)
         treat_util2 = self.get_resource_util('treat_duration', 
                                              self.args.n_cubicles_2, 
                                              self.model.trauma_patients)
@@ -975,15 +976,15 @@
     '''
     Perform a single run of the model and return the results
     
     Parameters:
     -----------
     
     scenario: Scenario object
-        The scenario/paramaters to run
+        The scenario/parameters to run
         
     rc_period: int
         The length of the simulation run that collects results
         
     random_no_set: int or None, optional (default=DEFAULT_RNG_SET)
         Controls the set of random seeds used by the stochastic parts of the 
         model.  Set to different ints to get different results.  Set to None
@@ -1015,15 +1016,15 @@
                           n_reps=5):
     '''
     Perform multiple replications of the model.
     
     Params:
     ------
     scenario: Scenario
-        Parameters/arguments to configurethe model
+        Parameters/arguments to configure the model
     
     rc_period: float, optional (default=DEFAULT_RESULTS_COLLECTION_PERIOD)
         results collection period.  
         the number of minutes to run the model to collect results
 
     n_reps: int, optional (default=DEFAULT_N_REPS)
         Number of independent replications to run.
```

### Comparing `treat_sim-1.1.1/treat_sim.egg-info/PKG-INFO` & `treat_sim-1.2.0/treat_sim.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treat-sim
-Version: 1.1.1
+Version: 1.2.0
 Summary: A free and open implementation of the Treatment Centre Model from Nelson (2013)
 Home-page: https://github.com/pythonhealthdatascience/stars-treat-sim
 Author: Thomas Monks
 Author-email: forecast-tools@gmail.com
 License: The MIT License (MIT)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,33 +18,33 @@
 Requires-Dist: numpy>=1.19.2
 Requires-Dist: pandas>=1.2.3
 Requires-Dist: scipy>=1.6.1
 Requires-Dist: simpy>=4.0.1
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pythonhealthdatascience/stars-treat-sim/HEAD)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-360+/)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10026327.svg)](https://doi.org/10.5281/zenodo.10026327)
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380+/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10026326.svg)](https://doi.org/10.5281/zenodo.10026326)
 [![PyPI version fury.io](https://badge.fury.io/py/treat-sim.svg)](https://pypi.org/project/treat-sim/)
 
 [<img src="https://img.shields.io/static/v1?label=dockerhub&message=images&color=important?style=for-the-badge&logo=docker">](https://hub.docker.com/r/tommonks01/treat_sim)
 
 
 # Towards Sharing Tools, and Artifacts, for Reusable Simulation: a minimal model example
 
 ## Overview
 
-The materials and methods in this repository support work towards developing the S.T.A.R.S healthcare framework (**S**haring **T**ools and **A**rtifacts for **R**euable **S**imulations in healthcare).  The code and written materials here demonstrate the application of S.T.A.R.S' version 1 to sharing a `simpy` discrete-event simuilation model and associated research artifacts.  
+The materials and methods in this repository support work towards developing the S.T.A.R.S healthcare framework (**S**haring **T**ools and **A**rtifacts for **R**eusable **S**imulations in healthcare).  The code and written materials here demonstrate the application of S.T.A.R.S' version 1 to sharing a `SimPy` discrete-event simulation model and associated research artifacts.  
 
 * All artifacts in this repository are linked to study researchers via ORCIDs;
 * Model code is made available under an MIT license;
-* Python dependencies are managed through `conda`;`
+* Python dependencies are managed through `conda`;
 * Documentation of the model is enhanced using a Jupyter notebook.
 * The python code itself can be viewed and executed in Jupyter notebooks via [Binder](https://mybinder.org); 
-* The materials are deposited and made citatable using Zenodo;
+* The materials are deposited and made citable using Zenodo;
 * The model is sharable with other researchers and the NHS without the need to install software.
 
 ## Author ORCIDs
 
 [![ORCID: Harper](https://img.shields.io/badge/ORCID-0000--0001--5274--5037-brightgreen)](https://orcid.org/0000-0001-5274-5037)
 [![ORCID: Monks](https://img.shields.io/badge/ORCID-0000--0003--2631--4481-brightgreen)](https://orcid.org/0000-0003-2631-4481)
 
@@ -54,46 +54,45 @@
 
 ## Instructions to run the model
 
 ### Online Notebooks via Binder
 
 The python code for the model has been setup to run online in Jupyter notebooks via binder [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pythonhealthdatascience/stars-treat-sim/HEAD)
 
-> mybinder.org is a free tier service.  If it has not been used in a while Binder will need to re-containerise the code repository, and push to binderhub. This will take several minutes. After that the online environment will be quick to load.
+> mybinder.org is a free tier service.  If it has not been used in a while Binder will need to re-containerise the code repository, and push to BinderHub. This will take several minutes. After that the online environment will be quick to load.
 
 ### To download code and run locally
 
 #### Downloading the code
 
 Either clone the repository using git or click on the green "code" button and select "Download Zip".
 
 ```bash
 git clone https://github.com/pythonhealthdatascience/stars-treat-sim
 ```
 
 #### Installing dependencies
 
-[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
 All dependencies can be found in [`binder/environment.yml`]() and are pulled from conda-forge.  To run the code locally, we recommend install [mini-conda](https://docs.conda.io/en/latest/miniconda.html); navigating your terminal (or cmd prompt) to the directory containing the repo and issuing the following command:
 
 ```
 conda env create -f binder/environment.yml
 ```
 
-Activate the conda environment using the following command
+Activate the conda environment using the following command:
 
 ```
 conda activate stars_treat_sim
 ```
 
 #### Running the model
 
-To run 50 multiple replications of across a number of example experiments use the following code
-
+To run 50 multiple replications across a number of example experiments, use the following code:
 
 ```python
 from treat_sim.model import (get_scenarios, run_scenario_analysis,
                              scenario_summary_frame, 
                              DEFAULT_RESULTS_COLLECTION_PERIOD)
 
 if __name__ == '__main__':
@@ -103,36 +102,37 @@
                                     n_reps=50)
 
     results_summary = scenario_summary_frame(results)
     print(results_summary)
 
 ```
 
-Alternative you can design and execute individual experiments by creating a `Scenario` object
+Alternative you can design and execute individual experiments by creating a `Scenario` object:
 
 ```python
 from treat_sim.model import Scenario, multiple_replications
 
 if __name__ == '__main__':
 
     # use all default parameter values
     base_case = Scenario()
 
     results = multiple_replications(base_case).describe().round(2).T
     print(results)
 
 ```
 
-
 ## Repo overview
 
 ```
 .
 ├── binder
 │   └── environment.yml
+├── CHANGES.md
+├── CITATION.cff
 ├── LICENSE
 ├── MANIFEST.in
 ├── notebooks
 │   └── test_package.ipynb
 ├── README.md
 ├── requirements.txt
 ├── setup.py
@@ -140,34 +140,43 @@
     ├── data
     │   └── ed_arrivals.csv
     ├── distributions.py
     ├── __init__.py
     └── model.py
 ```
 
-* `binder` - contains the environment.yml file (sim) and all dependencies managed via conda
-* `data` - directory containing data files used by analysis notebooks. 
+* `binder/` - contains the environment.yml file (sim) and all dependencies managed via conda, used to set-up the notebooks on Binder.
+* `CHANGES.md` - changelog with record of notable changes to project between versions.
+* `CITATION.cff` - citation information for the package.
 * `LICENSE` - details of the MIT permissive license of this work.
-* `notebooks` - contains a notebook to run the model and provides basic enhanced model documentation.
-* `main.py` - an example simpy model to use to test the virtual environment 
-* `README` - what you are reading now!
-* `treat_sim` - contains a packaged version of the model.
-
+* `MANIFEST.in` - files to include in the package.
+* `notebooks/` - contains a notebook to run the model and provides basic enhanced model documentation.
+* `README.md` - what you are reading now!
+* `requirements.txt` - list of packages and minimum versions required.
+* `setup.py` - used to build and distribute package.
+* `treat_sim/` - contains packaged version of the model.
+    * `data/` - directory containing data file used by package.
+    * `distributions.py` - distribution classes.
+    * `__init__.py` - required as part of package - contains author and version.
+    * `model.py` - example SimPy model.
 
 ## Citation
 
 If you use the materials within this repository we would appreciate a citation.
 
+```
+Monks, T., Harper, A., & Heather, A. (2024). Towards Sharing Tools, and Artifacts, for Reusable Simulation: a minimal model example (v1.2.0). Zenodo. https://doi.org/10.5281//zenodo.10026326
+```
+
 ```bibtex
-@software{monks_2023_10026327,
-  author       = {Monks, Thomas and
-                  Harper, Alison},
+@software{stars_treat_sim,
+  author       = {Thomas Monks, Alison Harper and Amy Heather},
   title        = {{Towards Sharing Tools, and Artifacts, for Reusable 
-                   Simulation: a minimal model examplar}},
-  month        = oct,
-  year         = 2023,
+                   Simulation: a minimal model example}},
+  month        = May,
+  year         = 2024,
   publisher    = {Zenodo},
-  version      = {v1.0.0},
-  url 	       = {https://zenodo.org/records/10026327}
+  version      = {v1.2.0},
+  doi          = {10.5281//zenodo.10026326.},
+  url          = {https://doi.org/10.5281//zenodo.10026326}
 }
 ```
-
```

