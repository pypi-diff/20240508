# Comparing `tmp/causalchamber-0.1.0.tar.gz` & `tmp/causalchamber-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/juan/ETH/causal-chamber/dist/.tmp-fvdo31oo/causalchamber-0.1.0.tar", last modified: Wed Apr 17 12:34:14 2024, max compression
+gzip compressed data, was "/home/juan/ETH/causal-chamber/dist/.tmp-iwbs2de4/causalchamber-0.1.1.tar", last modified: Wed May  8 12:48:37 2024, max compression
```

## Comparing `causalchamber-0.1.0.tar` & `causalchamber-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-17 12:34:14.000000 causalchamber-0.1.0/
--rw-rw-r--   0 juan      (1000) juan      (1000)     1071 2024-01-25 19:03:57.000000 causalchamber-0.1.0/LICENSE.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)     6099 2024-04-17 12:34:14.000000 causalchamber-0.1.0/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)    10132 2024-04-17 11:43:21.000000 causalchamber-0.1.0/README.md
--rw-rw-r--   0 juan      (1000) juan      (1000)      790 2024-04-17 12:33:49.000000 causalchamber-0.1.0/pyproject.toml
--rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-04-17 12:34:14.000000 causalchamber-0.1.0/setup.cfg
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/
--rw-rw-r--   0 juan      (1000) juan      (1000)     5493 2024-04-17 11:22:00.000000 causalchamber-0.1.0/src/README.md
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber/
--rw-rw-r--   0 juan      (1000) juan      (1000)      451 2024-04-17 09:32:38.000000 causalchamber-0.1.0/src/causalchamber/__init__.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber/datasets/
--rw-rw-r--   0 juan      (1000) juan      (1000)       20 2024-03-18 20:46:26.000000 causalchamber-0.1.0/src/causalchamber/datasets/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     6594 2024-04-17 11:02:53.000000 causalchamber-0.1.0/src/causalchamber/datasets/main.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2804 2024-04-17 11:02:53.000000 causalchamber-0.1.0/src/causalchamber/datasets/sampling.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     7216 2024-04-17 11:02:53.000000 causalchamber-0.1.0/src/causalchamber/datasets/utils.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    13592 2024-04-17 11:52:55.000000 causalchamber-0.1.0/src/causalchamber/ground_truth.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber/models/
--rw-rw-r--   0 juan      (1000) juan      (1000)      304 2024-03-18 20:52:51.000000 causalchamber-0.1.0/src/causalchamber/models/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     4753 2024-04-17 11:02:54.000000 causalchamber-0.1.0/src/causalchamber/models/image_capture.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1320 2024-04-17 11:02:54.000000 causalchamber-0.1.0/src/causalchamber/models/light_tunnel_models.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5050 2024-04-17 11:02:54.000000 causalchamber-0.1.0/src/causalchamber/models/wind_tunnel_models.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     3938 2024-04-17 11:02:54.000000 causalchamber-0.1.0/src/causalchamber/models/wind_tunnel_simulators.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber/test/
--rw-rw-r--   0 juan      (1000) juan      (1000)     3848 2024-04-17 11:02:47.000000 causalchamber-0.1.0/src/causalchamber/test/test_downloads.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     3713 2024-04-17 11:02:53.000000 causalchamber-0.1.0/src/causalchamber/utils.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber.egg-info/
--rw-rw-r--   0 juan      (1000) juan      (1000)     6099 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber.egg-info/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     6039 2024-03-26 15:37:00.000000 causalchamber-0.1.0/src/causalchamber.egg-info/PKG-INFO~
--rw-rw-r--   0 juan      (1000) juan      (1000)      813 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber.egg-info/SOURCES.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber.egg-info/dependency_links.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       71 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber.egg-info/requires.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       23 2024-04-17 12:34:14.000000 causalchamber-0.1.0/src/causalchamber.egg-info/top_level.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)     1693 2024-03-26 15:30:27.000000 causalchamber-0.1.0/src/examples.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-08 12:48:37.000000 causalchamber-0.1.1/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1071 2024-04-18 00:37:05.000000 causalchamber-0.1.1/LICENSE.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6049 2024-05-08 12:48:37.000000 causalchamber-0.1.1/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)    10156 2024-04-18 05:22:56.000000 causalchamber-0.1.1/README.md
+-rw-rw-r--   0 juan      (1000) juan      (1000)      790 2024-05-08 12:47:38.000000 causalchamber-0.1.1/pyproject.toml
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-05-08 12:48:37.000000 causalchamber-0.1.1/setup.cfg
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-08 12:48:36.000000 causalchamber-0.1.1/src/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5443 2024-04-18 05:19:27.000000 causalchamber-0.1.1/src/README.md
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-08 12:48:37.000000 causalchamber-0.1.1/src/causalchamber/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      457 2024-04-18 05:22:56.000000 causalchamber-0.1.1/src/causalchamber/__init__.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-08 12:48:37.000000 causalchamber-0.1.1/src/causalchamber/datasets/
+-rw-rw-r--   0 juan      (1000) juan      (1000)       20 2024-04-18 00:37:05.000000 causalchamber-0.1.1/src/causalchamber/datasets/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6594 2024-04-18 00:37:05.000000 causalchamber-0.1.1/src/causalchamber/datasets/main.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2804 2024-04-18 00:37:05.000000 causalchamber-0.1.1/src/causalchamber/datasets/sampling.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     7216 2024-04-18 00:37:05.000000 causalchamber-0.1.1/src/causalchamber/datasets/utils.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    13592 2024-04-18 00:37:05.000000 causalchamber-0.1.1/src/causalchamber/ground_truth.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-08 12:48:37.000000 causalchamber-0.1.1/src/causalchamber/models/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      304 2024-04-18 00:37:05.000000 causalchamber-0.1.1/src/causalchamber/models/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4753 2024-04-18 00:37:05.000000 causalchamber-0.1.1/src/causalchamber/models/image_capture.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1320 2024-04-18 00:37:05.000000 causalchamber-0.1.1/src/causalchamber/models/light_tunnel_models.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5050 2024-04-18 00:37:05.000000 causalchamber-0.1.1/src/causalchamber/models/wind_tunnel_models.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3938 2024-04-18 00:37:05.000000 causalchamber-0.1.1/src/causalchamber/models/wind_tunnel_simulators.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-08 12:48:37.000000 causalchamber-0.1.1/src/causalchamber/test/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3848 2024-04-18 00:37:05.000000 causalchamber-0.1.1/src/causalchamber/test/test_downloads.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3713 2024-04-18 00:37:05.000000 causalchamber-0.1.1/src/causalchamber/utils.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-08 12:48:37.000000 causalchamber-0.1.1/src/causalchamber.egg-info/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6049 2024-05-08 12:48:36.000000 causalchamber-0.1.1/src/causalchamber.egg-info/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)      776 2024-05-08 12:48:36.000000 causalchamber-0.1.1/src/causalchamber.egg-info/SOURCES.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-05-08 12:48:36.000000 causalchamber-0.1.1/src/causalchamber.egg-info/dependency_links.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       71 2024-05-08 12:48:36.000000 causalchamber-0.1.1/src/causalchamber.egg-info/requires.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       23 2024-05-08 12:48:36.000000 causalchamber-0.1.1/src/causalchamber.egg-info/top_level.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1693 2024-04-18 00:37:05.000000 causalchamber-0.1.1/src/examples.py
```

### Comparing `causalchamber-0.1.0/LICENSE.txt` & `causalchamber-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `causalchamber-0.1.0/PKG-INFO` & `causalchamber-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: causalchamber
-Version: 0.1.0
+Version: 0.1.1
 Summary: Access the datasets and models from the causal chambers.
 Author-email: Juan L Gamella <juangamella@gmail.com>
 Project-URL: Homepage, https://causalchamber.org
 Project-URL: Repository, https://github.com/juangamella/causal-chamber
 Project-URL: Issues, https://github.com/juangamella/causal-chamber/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Welcome to the `causalchamber` package
 
 [![PyPI version](https://badge.fury.io/py/causalchamber.svg)](https://badge.fury.io/py/causalchamber)
 [![Downloads](https://static.pepy.tech/badge/causalchamber)](https://pepy.tech/project/causalchamber)
@@ -88,15 +88,15 @@
 
 # Output:
 # ['200', '500', 'full']
 ```
 
 ## Mechanistic models
 
-The `causalchamber` [package](https://pypi.org/project/causalchamber/) also contains Python implementations of the mechanistic models described in appendix IV of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
+The `causalchamber` [package](https://pypi.org/project/causalchamber/) also contains Python implementations of the mechanistic models described in appendix IV of the original [paper](https://arxiv.org/pdf/2404.11341.pdf). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
 ```Python
 import numpy as np
 from causalchamber.models import model_a1
 model_a1(L=np.linspace(0,1,10), L_min=0.1, omega_max=314.15)
 
 # Output:
 
@@ -105,15 +105,15 @@
 #        279.24444444, 314.15      ])
 ```
 
 The implementations can be found in the [`src/causalchamber/models`](src/causalchamber/models) directory. You can find examples of using the models in the [`case_studies/mechanistic_models.ipynb`](https://github.com/juangamella/causal-chamber-paper/blob/main/case_studies/mechanistic_models.ipynb) notebook in the separate [paper repository](https://github.com/juangamella/causal-chamber-paper).
 
 ## Causal ground-truth graphs
 
-The graphs for the causal ground truths given in Fig. 3 of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>) can be found as adjacency matrices in  the `ground_truths/` directory of the [project repository](https://github.com/juangamella/causal-chamber). The adjacencies can also be loaded through the `causalchamber` [package](https://pypi.org/project/causalchamber/), e.g., 
+The graphs for the causal ground truths given in Fig. 3 of the original [paper](https://arxiv.org/pdf/2404.11341.pdf) can be found as adjacency matrices in  the `ground_truths/` directory of the [project repository](https://github.com/juangamella/causal-chamber). The adjacencies can also be loaded through the `causalchamber` [package](https://pypi.org/project/causalchamber/), e.g., 
 ```python
 from causalchamber.ground_truth import graph
 graph(chamber="lt", configuration="standard")
 
 # Output:
 
 #              red  green  blue  osr_c  v_c  current  pol_1  pol_2  osr_angle_1  \
```

### Comparing `causalchamber-0.1.0/README.md` & `causalchamber-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # The Causal Chambers: Dataset Repository
 
 ![The Causal Chambers: (left) the wind tunnel, and (right) the light tunnel with the front panel removed to show its interior.](https://causalchamber.s3.eu-central-1.amazonaws.com/downloadables/the_chambers.jpg)
 
-This repository contains datasets collected from the _causal chambers_, the two devices described in the 2024 paper [*The Causal Chambers: Real Physical Systems as a Testbed for AI Methodology*](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>) by Juan L. Gamella, Jonas Peters and Peter Bühlmann. The repository is updated as we collect new datasets from the chambers.
+This repository contains datasets collected from the _causal chambers_, the two devices described in the 2024 paper [*The Causal Chambers: Real Physical Systems as a Testbed for AI Methodology*](https://arxiv.org/pdf/2404.11341.pdf) by Juan L. Gamella, Jonas Peters and Peter Bühlmann. The repository is updated as we collect new datasets from the chambers.
 
 The datasets are publicly available through a permissive [CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/). This means you are free to use, share and modify the datasets as long as you give appropriate credit and communicate changes. If you use the datasets in your scientific work, please consider citing:
 
 ```
 @article{gamella2024chamber,
   title={The Causal Chambers: Real Physical Systems as a Testbed for AI Methodology},
   author={Gamella, Juan L. and B\"uhlmann, Peter and Peters, Jonas},
-  journal={arXiv preprint arXiv:TODO},
+  journal={arXiv preprint arXiv:2404.11341},
   year={2024}
 }
 ```
 
-This repository also contains the source code for the `causalchamber` [package](https://pypi.org/project/causalchamber/) to directly [import the datasets into your Python code](#downloading-the-datasets). The package also provides Python implementations of the [mechanistic models](#mechanistic-models) described in appendix IV of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>).
+This repository also contains the source code for the `causalchamber` [package](https://pypi.org/project/causalchamber/) to directly [import the datasets into your Python code](#downloading-the-datasets). The package also provides Python implementations of the [mechanistic models](#mechanistic-models) described in appendix IV of the original [paper](https://arxiv.org/pdf/2404.11341.pdf).
 
 Here you can also find the resources to [build the chambers](#building-the-chambers), and the datasheets for all chamber components (see [`hardware/`](hardware/)).
 
 The code to reproduce the case studies in the original paper can be found in the separate [paper repository](https://github.com/juangamella/causal-chamber-paper).
 
 ## Available datasets
 
-Each dataset is described in detail in its corresponding page (click the dataset name). The chamber configurations are described in Fig. 3 of the manuscript.
+We are open to suggestions of additional experiments that may prove interesting; please reach out to the [corresponding author](https://github.com/juangamella).
+
+Each dataset below is described in detail in its corresponding page (click the dataset name). The chamber configurations are described in Fig. 3 of the manuscript.
 
 | Dataset name | Notes | Chamber | Config. |
 |--------:|:--------------------------------|:--------:|:--------:|
 | [lt_camera_walks_v1](datasets/lt_camera_walks_v1/) | Image data for the ICA case study (task d3, Fig. 6). | Light tunnel | camera |
 | [lt_color_regression_v1](datasets/lt_color_regression_v1/) | Image data for task b2 in the OOD case study (Fig. 5) | Light tunnel | camera |
 | [lt_interventions_standard_v1](datasets/lt_interventions_standard_v1/) | Observational and interventional data from the light tunnel, used for the causal discovery case study in Fig. 5. | Light tunnel | standard |
 | [lt_walks_v1](datasets/lt_walks_v1/) | Random and deterministic walks of the light-tunnel actuators. Used in the ICA case study (task d1), Fig. 6. | Light tunnel | standard |
@@ -51,15 +53,15 @@
 
 If you use Python, you can directly import a dataset into your code through the `causalchamber` [package](https://pypi.org/project/causalchamber/). You can install it using pip, e.g. by typing
 
 ```
 pip install causalchamber
 ```
 
-in an appropriate shell. Datasets can then be accessed directly from your Python code. For example, you can access the light-intensity data for the symbolic regression case study ([Fig. 6e](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>)) as follows:
+in an appropriate shell. Datasets can then be accessed directly from your Python code. For example, you can access the light-intensity data for the symbolic regression case study ([Fig. 6e](https://arxiv.org/pdf/2404.11341.pdf)) as follows:
 
 ```python
 from causalchamber.datasets import Dataset
 
 # Download the dataset and store it, e.g., in the current directory
 dataset = Dataset(name='lt_malus_v1', root='./', download=True)
 
@@ -85,15 +87,15 @@
 #  'white_128',
 #  'white_255',
 #  'white_64']
 ```
 
 ## Mechanistic models
 
-The `causalchamber` [package](https://pypi.org/project/causalchamber/) also contains Python implementations of the mechanistic models described in appendix IV of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
+The `causalchamber` [package](https://pypi.org/project/causalchamber/) also contains Python implementations of the mechanistic models described in appendix IV of the original [paper](https://arxiv.org/pdf/2404.11341.pdf). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
 ```Python
 import numpy as np
 from causalchamber.models import model_a1
 model_a1(L=np.linspace(0,1,10), L_min=0.1, omega_max=314.15)
 
 # Output:
 
@@ -102,15 +104,15 @@
 #        279.24444444, 314.15      ])
 ```
 
 The implementations can be found in the [`src/causalchamber/models`](src/causalchamber/models) directory. You can find examples of using the models in the [`case_studies/mechanistic_models.ipynb`](https://github.com/juangamella/causal-chamber-paper/blob/main/case_studies/mechanistic_models.ipynb) notebook in the separate [paper repository](https://github.com/juangamella/causal-chamber-paper).
 
 ## Causal ground-truth graphs
 
-The graphs for the causal ground truths given in Fig. 3 of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>) can be found as adjacency matrices in  the [`ground_truths/`](ground_truths/) directory. The adjacencies can also be loaded through the `causalchamber` [package](https://pypi.org/project/causalchamber/), e.g., 
+The graphs for the causal ground truths given in Fig. 3 of the original [paper](https://arxiv.org/pdf/2404.11341.pdf) can be found as adjacency matrices in  the [`ground_truths/`](ground_truths/) directory. The adjacencies can also be loaded through the `causalchamber` [package](https://pypi.org/project/causalchamber/), e.g., 
 ```python
 from causalchamber.ground_truth import graph
 graph(chamber="lt", configuration="standard")
 
 # Output:
 
 #              red  green  blue  osr_c  v_c  current  pol_1  pol_2  osr_angle_1  \
@@ -130,15 +132,15 @@
 # '$\\theta_1$'
 ```
 
 Setting `enclose=False` will return the name without surrounding `$`.
 
 ## Building the chambers
 
-You can find the resources to build the chambers in [`hardware/`](hardware/), together with the datasheets for all physical components (see appendix VI of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>)).
+You can find the resources to build the chambers in [`hardware/`](hardware/), together with the datasheets for all physical components (see appendix VI of the original [paper](https://arxiv.org/pdf/2404.11341.pdf)).
 
 ## Licenses
 
 All images and `.csv` files in the datasets are licensed under a [CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/). A copy of the license can be found in [LICENSE_DATASETS.txt](LICENSE_DATASETS.txt).
 
 The code, e.g., for the `causalchamber` package and mechanistic models, is shared under the [MIT license](https://opensource.org/license/mit/). A copy of the license can also be found in [LICENSE_SOFTWARE.txt](LICENSE_SOFTWARE.txt).
```

### Comparing `causalchamber-0.1.0/pyproject.toml` & `causalchamber-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "causalchamber"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Juan L Gamella", email="juangamella@gmail.com" },
 ]
 description = "Access the datasets and models from the causal chambers."
 readme = "src/README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy>=1.18.0",
```

### Comparing `causalchamber-0.1.0/src/README.md` & `causalchamber-0.1.1/src/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 # Output:
 # ['200', '500', 'full']
 ```
 
 ## Mechanistic models
 
-The `causalchamber` [package](https://pypi.org/project/causalchamber/) also contains Python implementations of the mechanistic models described in appendix IV of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
+The `causalchamber` [package](https://pypi.org/project/causalchamber/) also contains Python implementations of the mechanistic models described in appendix IV of the original [paper](https://arxiv.org/pdf/2404.11341.pdf). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
 ```Python
 import numpy as np
 from causalchamber.models import model_a1
 model_a1(L=np.linspace(0,1,10), L_min=0.1, omega_max=314.15)
 
 # Output:
 
@@ -90,15 +90,15 @@
 #        279.24444444, 314.15      ])
 ```
 
 The implementations can be found in the [`src/causalchamber/models`](src/causalchamber/models) directory. You can find examples of using the models in the [`case_studies/mechanistic_models.ipynb`](https://github.com/juangamella/causal-chamber-paper/blob/main/case_studies/mechanistic_models.ipynb) notebook in the separate [paper repository](https://github.com/juangamella/causal-chamber-paper).
 
 ## Causal ground-truth graphs
 
-The graphs for the causal ground truths given in Fig. 3 of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>) can be found as adjacency matrices in  the `ground_truths/` directory of the [project repository](https://github.com/juangamella/causal-chamber). The adjacencies can also be loaded through the `causalchamber` [package](https://pypi.org/project/causalchamber/), e.g., 
+The graphs for the causal ground truths given in Fig. 3 of the original [paper](https://arxiv.org/pdf/2404.11341.pdf) can be found as adjacency matrices in  the `ground_truths/` directory of the [project repository](https://github.com/juangamella/causal-chamber). The adjacencies can also be loaded through the `causalchamber` [package](https://pypi.org/project/causalchamber/), e.g., 
 ```python
 from causalchamber.ground_truth import graph
 graph(chamber="lt", configuration="standard")
 
 # Output:
 
 #              red  green  blue  osr_c  v_c  current  pol_1  pol_2  osr_angle_1  \
```

### Comparing `causalchamber-0.1.0/src/causalchamber/datasets/main.py` & `causalchamber-0.1.1/src/causalchamber/datasets/main.py`

 * *Files identical despite different names*

### Comparing `causalchamber-0.1.0/src/causalchamber/datasets/sampling.py` & `causalchamber-0.1.1/src/causalchamber/datasets/sampling.py`

 * *Files identical despite different names*

### Comparing `causalchamber-0.1.0/src/causalchamber/datasets/utils.py` & `causalchamber-0.1.1/src/causalchamber/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `causalchamber-0.1.0/src/causalchamber/ground_truth.py` & `causalchamber-0.1.1/src/causalchamber/ground_truth.py`

 * *Files identical despite different names*

### Comparing `causalchamber-0.1.0/src/causalchamber/models/image_capture.py` & `causalchamber-0.1.1/src/causalchamber/models/image_capture.py`

 * *Files identical despite different names*

### Comparing `causalchamber-0.1.0/src/causalchamber/models/light_tunnel_models.py` & `causalchamber-0.1.1/src/causalchamber/models/light_tunnel_models.py`

 * *Files identical despite different names*

### Comparing `causalchamber-0.1.0/src/causalchamber/models/wind_tunnel_models.py` & `causalchamber-0.1.1/src/causalchamber/models/wind_tunnel_models.py`

 * *Files identical despite different names*

### Comparing `causalchamber-0.1.0/src/causalchamber/models/wind_tunnel_simulators.py` & `causalchamber-0.1.1/src/causalchamber/models/wind_tunnel_simulators.py`

 * *Files identical despite different names*

### Comparing `causalchamber-0.1.0/src/causalchamber/test/test_downloads.py` & `causalchamber-0.1.1/src/causalchamber/test/test_downloads.py`

 * *Files identical despite different names*

### Comparing `causalchamber-0.1.0/src/causalchamber/utils.py` & `causalchamber-0.1.1/src/causalchamber/utils.py`

 * *Files identical despite different names*

### Comparing `causalchamber-0.1.0/src/causalchamber.egg-info/PKG-INFO` & `causalchamber-0.1.1/src/causalchamber.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: causalchamber
-Version: 0.1.0
+Version: 0.1.1
 Summary: Access the datasets and models from the causal chambers.
 Author-email: Juan L Gamella <juangamella@gmail.com>
 Project-URL: Homepage, https://causalchamber.org
 Project-URL: Repository, https://github.com/juangamella/causal-chamber
 Project-URL: Issues, https://github.com/juangamella/causal-chamber/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Welcome to the `causalchamber` package
 
 [![PyPI version](https://badge.fury.io/py/causalchamber.svg)](https://badge.fury.io/py/causalchamber)
 [![Downloads](https://static.pepy.tech/badge/causalchamber)](https://pepy.tech/project/causalchamber)
@@ -88,15 +88,15 @@
 
 # Output:
 # ['200', '500', 'full']
 ```
 
 ## Mechanistic models
 
-The `causalchamber` [package](https://pypi.org/project/causalchamber/) also contains Python implementations of the mechanistic models described in appendix IV of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
+The `causalchamber` [package](https://pypi.org/project/causalchamber/) also contains Python implementations of the mechanistic models described in appendix IV of the original [paper](https://arxiv.org/pdf/2404.11341.pdf). The models follow the same nomenclature as in the paper, e.g., to import and run model A1 of the steady-state fan speed:
 ```Python
 import numpy as np
 from causalchamber.models import model_a1
 model_a1(L=np.linspace(0,1,10), L_min=0.1, omega_max=314.15)
 
 # Output:
 
@@ -105,15 +105,15 @@
 #        279.24444444, 314.15      ])
 ```
 
 The implementations can be found in the [`src/causalchamber/models`](src/causalchamber/models) directory. You can find examples of using the models in the [`case_studies/mechanistic_models.ipynb`](https://github.com/juangamella/causal-chamber-paper/blob/main/case_studies/mechanistic_models.ipynb) notebook in the separate [paper repository](https://github.com/juangamella/causal-chamber-paper).
 
 ## Causal ground-truth graphs
 
-The graphs for the causal ground truths given in Fig. 3 of the original [paper](<https://placehold.co/600x400?text=Placeholder:\nArxiv link!>) can be found as adjacency matrices in  the `ground_truths/` directory of the [project repository](https://github.com/juangamella/causal-chamber). The adjacencies can also be loaded through the `causalchamber` [package](https://pypi.org/project/causalchamber/), e.g., 
+The graphs for the causal ground truths given in Fig. 3 of the original [paper](https://arxiv.org/pdf/2404.11341.pdf) can be found as adjacency matrices in  the `ground_truths/` directory of the [project repository](https://github.com/juangamella/causal-chamber). The adjacencies can also be loaded through the `causalchamber` [package](https://pypi.org/project/causalchamber/), e.g., 
 ```python
 from causalchamber.ground_truth import graph
 graph(chamber="lt", configuration="standard")
 
 # Output:
 
 #              red  green  blue  osr_c  v_c  current  pol_1  pol_2  osr_angle_1  \
```

### Comparing `causalchamber-0.1.0/src/causalchamber.egg-info/SOURCES.txt` & `causalchamber-0.1.1/src/causalchamber.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 pyproject.toml
 src/README.md
 src/examples.py
 src/causalchamber/__init__.py
 src/causalchamber/ground_truth.py
 src/causalchamber/utils.py
 src/causalchamber.egg-info/PKG-INFO
-src/causalchamber.egg-info/PKG-INFO~
 src/causalchamber.egg-info/SOURCES.txt
 src/causalchamber.egg-info/dependency_links.txt
 src/causalchamber.egg-info/requires.txt
 src/causalchamber.egg-info/top_level.txt
 src/causalchamber/datasets/__init__.py
 src/causalchamber/datasets/main.py
 src/causalchamber/datasets/sampling.py
```

### Comparing `causalchamber-0.1.0/src/examples.py` & `causalchamber-0.1.1/src/examples.py`

 * *Files identical despite different names*

