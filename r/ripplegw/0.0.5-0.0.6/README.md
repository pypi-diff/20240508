# Comparing `tmp/ripplegw-0.0.5.tar.gz` & `tmp/ripplegw-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ripplegw-0.0.5.tar", last modified: Fri Feb 16 13:46:22 2024, max compression
+gzip compressed data, was "ripplegw-0.0.6.tar", last modified: Wed May  8 21:37:30 2024, max compression
```

## Comparing `ripplegw-0.0.5.tar` & `ripplegw-0.0.6.tar`

### file list

```diff
@@ -1,36 +1,42 @@
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2024-02-16 13:46:22.225517 ripplegw-0.0.5/
--rw-r--r--   0 thomasedwards   (501) staff       (20)     1088 2022-10-12 22:06:55.000000 ripplegw-0.0.5/LICENSE
--rw-r--r--   0 thomasedwards   (501) staff       (20)     3238 2024-02-16 13:46:22.225055 ripplegw-0.0.5/PKG-INFO
--rw-r--r--   0 thomasedwards   (501) staff       (20)     2650 2024-02-02 13:28:29.000000 ripplegw-0.0.5/README.md
--rw-r--r--   0 thomasedwards   (501) staff       (20)      104 2022-10-12 22:06:55.000000 ripplegw-0.0.5/pyproject.toml
--rw-r--r--   0 thomasedwards   (501) staff       (20)      725 2024-02-16 13:46:22.228020 ripplegw-0.0.5/setup.cfg
--rw-r--r--   0 thomasedwards   (501) staff       (20)       38 2022-10-12 22:06:55.000000 ripplegw-0.0.5/setup.py
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2024-02-16 13:46:22.206036 ripplegw-0.0.5/src/
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2024-02-16 13:46:22.210273 ripplegw-0.0.5/src/ripple/
--rw-r--r--   0 thomasedwards   (501) staff       (20)     9837 2024-02-16 13:38:21.000000 ripplegw-0.0.5/src/ripple/__init__.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)      483 2023-01-06 18:06:40.000000 ripplegw-0.0.5/src/ripple/constants.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)     3156 2024-02-02 13:28:29.000000 ripplegw-0.0.5/src/ripple/noise.py
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2024-02-16 13:46:22.216668 ripplegw-0.0.5/src/ripple/noise_resources/
--rw-r--r--   0 thomasedwards   (501) staff       (20)    48230 2022-10-12 22:06:55.000000 ripplegw-0.0.5/src/ripple/noise_resources/O2_ASD.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)  1117811 2022-10-12 22:06:55.000000 ripplegw-0.0.5/src/ripple/noise_resources/O3a_Livingston_ASD.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)        0 2022-10-12 22:06:55.000000 ripplegw-0.0.5/src/ripple/noise_resources/__init__.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    56415 2022-10-12 22:06:55.000000 ripplegw-0.0.5/src/ripple/noise_resources/aLIGO.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)    10070 2022-10-12 22:06:55.000000 ripplegw-0.0.5/src/ripple/noise_resources/aLIGOZeroDetHighPower.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)    87114 2022-10-12 22:06:55.000000 ripplegw-0.0.5/src/ripple/noise_resources/ce.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)    87132 2022-10-12 22:06:55.000000 ripplegw-0.0.5/src/ripple/noise_resources/et.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)      203 2024-02-16 13:40:16.000000 ripplegw-0.0.5/src/ripple/typing.py
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2024-02-16 13:46:22.219952 ripplegw-0.0.5/src/ripple/waveforms/
--rw-r--r--   0 thomasedwards   (501) staff       (20)    19440 2024-02-02 13:28:29.000000 ripplegw-0.0.5/src/ripple/waveforms/IMRPhenomD.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    53661 2023-01-31 13:59:58.000000 ripplegw-0.0.5/src/ripple/waveforms/IMRPhenomD_QNMdata.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    16243 2024-02-02 13:28:29.000000 ripplegw-0.0.5/src/ripple/waveforms/IMRPhenomD_utils.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)     9046 2024-02-02 13:28:29.000000 ripplegw-0.0.5/src/ripple/waveforms/IMRPhenomPv2.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    13652 2024-02-02 13:28:29.000000 ripplegw-0.0.5/src/ripple/waveforms/IMRPhenomPv2_utils.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    45388 2024-02-02 13:28:29.000000 ripplegw-0.0.5/src/ripple/waveforms/IMRPhenomXAS.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    39958 2024-02-02 13:28:29.000000 ripplegw-0.0.5/src/ripple/waveforms/IMRPhenomX_utils.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)        0 2022-10-12 22:06:55.000000 ripplegw-0.0.5/src/ripple/waveforms/__init__.py
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2024-02-16 13:46:22.224674 ripplegw-0.0.5/src/ripplegw.egg-info/
--rw-r--r--   0 thomasedwards   (501) staff       (20)     3238 2024-02-16 13:46:22.000000 ripplegw-0.0.5/src/ripplegw.egg-info/PKG-INFO
--rw-r--r--   0 thomasedwards   (501) staff       (20)      913 2024-02-16 13:46:22.000000 ripplegw-0.0.5/src/ripplegw.egg-info/SOURCES.txt
--rw-r--r--   0 thomasedwards   (501) staff       (20)        1 2024-02-16 13:46:22.000000 ripplegw-0.0.5/src/ripplegw.egg-info/dependency_links.txt
--rw-r--r--   0 thomasedwards   (501) staff       (20)       17 2024-02-16 13:46:22.000000 ripplegw-0.0.5/src/ripplegw.egg-info/requires.txt
--rw-r--r--   0 thomasedwards   (501) staff       (20)        7 2024-02-16 13:46:22.000000 ripplegw-0.0.5/src/ripplegw.egg-info/top_level.txt
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2024-05-08 21:37:30.895842 ripplegw-0.0.6/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     1088 2022-10-12 22:06:55.000000 ripplegw-0.0.6/LICENSE
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     4293 2024-05-08 21:37:30.895640 ripplegw-0.0.6/PKG-INFO
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     3704 2024-04-29 20:44:00.000000 ripplegw-0.0.6/README.md
+-rw-r--r--   0 thomasedwards   (501) staff       (20)      104 2022-10-12 22:06:55.000000 ripplegw-0.0.6/pyproject.toml
+-rw-r--r--   0 thomasedwards   (501) staff       (20)      725 2024-05-08 21:37:30.897192 ripplegw-0.0.6/setup.cfg
+-rw-r--r--   0 thomasedwards   (501) staff       (20)       38 2022-10-12 22:06:55.000000 ripplegw-0.0.6/setup.py
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2024-05-08 21:37:30.810707 ripplegw-0.0.6/src/
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2024-05-08 21:37:30.814817 ripplegw-0.0.6/src/ripple/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)      809 2024-04-29 20:52:56.000000 ripplegw-0.0.6/src/ripple/FD_waveform.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    16339 2024-04-29 20:11:15.000000 ripplegw-0.0.6/src/ripple/__init__.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)      728 2024-04-29 20:11:15.000000 ripplegw-0.0.6/src/ripple/constants.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     3155 2024-04-29 20:11:15.000000 ripplegw-0.0.6/src/ripple/noise.py
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2024-05-08 21:37:30.832276 ripplegw-0.0.6/src/ripple/noise_resources/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    48230 2022-10-12 22:06:55.000000 ripplegw-0.0.6/src/ripple/noise_resources/O2_ASD.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)  1117811 2022-10-12 22:06:55.000000 ripplegw-0.0.6/src/ripple/noise_resources/O3a_Livingston_ASD.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)        0 2022-10-12 22:06:55.000000 ripplegw-0.0.6/src/ripple/noise_resources/__init__.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    56415 2022-10-12 22:06:55.000000 ripplegw-0.0.6/src/ripple/noise_resources/aLIGO.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    10070 2022-10-12 22:06:55.000000 ripplegw-0.0.6/src/ripple/noise_resources/aLIGOZeroDetHighPower.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    87114 2022-10-12 22:06:55.000000 ripplegw-0.0.6/src/ripple/noise_resources/ce.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    87132 2022-10-12 22:06:55.000000 ripplegw-0.0.6/src/ripple/noise_resources/et.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)      203 2024-04-29 20:11:15.000000 ripplegw-0.0.6/src/ripple/typing.py
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2024-05-08 21:37:30.850641 ripplegw-0.0.6/src/ripple/waveforms/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    19497 2024-05-08 16:00:02.000000 ripplegw-0.0.6/src/ripple/waveforms/IMRPhenomD.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    14996 2024-04-29 20:40:59.000000 ripplegw-0.0.6/src/ripple/waveforms/IMRPhenomD_NRTidalv2.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    53661 2023-01-31 13:59:58.000000 ripplegw-0.0.6/src/ripple/waveforms/IMRPhenomD_QNMdata.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    16243 2024-04-29 20:11:15.000000 ripplegw-0.0.6/src/ripple/waveforms/IMRPhenomD_utils.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     9046 2024-04-29 20:11:15.000000 ripplegw-0.0.6/src/ripple/waveforms/IMRPhenomPv2.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    13652 2024-04-29 20:11:15.000000 ripplegw-0.0.6/src/ripple/waveforms/IMRPhenomPv2_utils.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    45368 2024-04-29 20:11:15.000000 ripplegw-0.0.6/src/ripple/waveforms/IMRPhenomXAS.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    39818 2024-04-29 20:11:15.000000 ripplegw-0.0.6/src/ripple/waveforms/IMRPhenomX_utils.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     4421 2024-04-29 20:11:15.000000 ripplegw-0.0.6/src/ripple/waveforms/IMRPhenom_tidal_utils.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    14949 2024-04-29 20:11:15.000000 ripplegw-0.0.6/src/ripple/waveforms/TaylorF2.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)        0 2022-10-12 22:06:55.000000 ripplegw-0.0.6/src/ripple/waveforms/__init__.py
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2024-05-08 21:37:30.894997 ripplegw-0.0.6/src/ripplegw.egg-info/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     4293 2024-05-08 21:37:30.000000 ripplegw-0.0.6/src/ripplegw.egg-info/PKG-INFO
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     1087 2024-05-08 21:37:30.000000 ripplegw-0.0.6/src/ripplegw.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasedwards   (501) staff       (20)        1 2024-05-08 21:37:30.000000 ripplegw-0.0.6/src/ripplegw.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasedwards   (501) staff       (20)       17 2024-05-08 21:37:30.000000 ripplegw-0.0.6/src/ripplegw.egg-info/requires.txt
+-rw-r--r--   0 thomasedwards   (501) staff       (20)        7 2024-05-08 21:37:30.000000 ripplegw-0.0.6/src/ripplegw.egg-info/top_level.txt
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2024-05-08 21:37:30.894058 ripplegw-0.0.6/test/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     1309 2024-04-29 20:11:15.000000 ripplegw-0.0.6/test/test_conversion.py
```

### Comparing `ripplegw-0.0.5/LICENSE` & `ripplegw-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.5/PKG-INFO` & `ripplegw-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,44 @@
-Metadata-Version: 2.1
-Name: ripplegw
-Version: 0.0.5
-Summary: A small jax package for differentiable and fast gravitational wave data analysis.
-Home-page: https://ripple.readthedocs.io/en/latest/
-Project-URL: Bug Tracker, https://github.com/tedwards2412/ripple
-Keywords: gravitational waves,jax
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: jax
-Requires-Dist: jaxlib
-Requires-Dist: numpy
-
 # Ripple :ocean:
 
 A small `jax` package for differentiable and fast gravitational wave data analysis.
 
 # Getting Started
 
 ### Installation
 
-Both waveforms have been tested extensively and match lalsuite implementations to machine precision across all the parameter space. 
+Both waveforms have been tested extensively and match `lalsuite` implementations to machine precision across all the parameter space. 
 
 Ripple can be installed using 
 
 ```
 pip3 install ripplegw
 ```
 
-Note that by default we do not include enable float64 in jax since we want allow users to use float32 to improve performance.
+Note that by default we do not include enable float64 in `jax` since we want allow users to use float32 to improve performance.
 If you require float64, please include the following code at the start of the script:
 
 ```
 from jax import config
 config.update("jax_enable_x64", True)
 ```
 
 See https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html for other common `jax` gotchas.
 
 ### Supported waveforms
 
 - IMRPhenomXAS (aligned spin)
 - IMRPhenomD (aligned spin)
 - IMRPhenomPv2 (Still finalizing sampling checks)
+- TaylorF2 with tidal effects
+- IMRPhenomD_NRTidalv2, verified for the low spin regime (chi1, chi2 < 0.05), further testing is required for higher spins
 
 ### Generating a waveform and its derivative
 
-Generating a waveform is increadibly easy. Below is an example of calling the PhenomXAS waveform model
+Generating a waveform is incredibly easy. Below is an example of calling the PhenomXAS waveform model
 to get the h_+ and h_x polarizations of the waveform model
 
 We start with some basic imports:
 
 ```python
 import jax.numpy as jnp
 
@@ -102,8 +87,28 @@
 
 @jax.jit
 def waveform(theta):
     return IMRPhenomXAS.gen_IMRPhenomXAS_hphc(fs, theta)
 ```
 
 
+### Citation
+
+Please cite this paper if you've used `ripple` in your work! It's really helpful!
+
+```bibtex
+@article{Edwards:2023sak,
+    author = "Edwards, Thomas D. P. and Wong, Kaze W. K. and Lam, Kelvin K. H. and Coogan, Adam and Foreman-Mackey, Daniel and Isi, Maximiliano and Zimmerman, Aaron",
+    title = "{ripple: Differentiable and Hardware-Accelerated Waveforms for Gravitational Wave Data Analysis}",
+    eprint = "2302.05329",
+    archivePrefix = "arXiv",
+    primaryClass = "astro-ph.IM",
+    month = "2",
+    year = "2023"
+}
+```
+
+### Contributions
+
+Contributions through pull requests are very welcome. Please also feel free to open new issues if there are missing features you'd like to see!
 
+The only requirement for contributions to be considered is that they are run through the black code formatter. This ensures we have a coherent format and makes the code easier to review/read!
```

### Comparing `ripplegw-0.0.5/setup.cfg` & `ripplegw-0.0.6/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ripplegw
-version = 0.0.5
+version = 0.0.6
 description = A small jax package for differentiable and fast gravitational wave data analysis.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = gravitational waves, jax
 url = https://ripple.readthedocs.io/en/latest/
 project_urls = 
 	Bug Tracker = https://github.com/tedwards2412/ripple
```

### Comparing `ripplegw-0.0.5/src/ripple/noise.py` & `ripplegw-0.0.6/src/ripple/noise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Detector noise power spectral densities.
 """
 
-
 import importlib.resources as pkg_resources
 from typing import Callable, Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
```

### Comparing `ripplegw-0.0.5/src/ripple/noise_resources/O2_ASD.dat` & `ripplegw-0.0.6/src/ripple/noise_resources/O2_ASD.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.5/src/ripple/noise_resources/O3a_Livingston_ASD.dat` & `ripplegw-0.0.6/src/ripple/noise_resources/O3a_Livingston_ASD.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.5/src/ripple/noise_resources/aLIGO.dat` & `ripplegw-0.0.6/src/ripple/noise_resources/aLIGO.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.5/src/ripple/noise_resources/aLIGOZeroDetHighPower.dat` & `ripplegw-0.0.6/src/ripple/noise_resources/aLIGOZeroDetHighPower.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.5/src/ripple/noise_resources/ce.dat` & `ripplegw-0.0.6/src/ripple/noise_resources/ce.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.5/src/ripple/noise_resources/et.dat` & `ripplegw-0.0.6/src/ripple/noise_resources/et.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.5/src/ripple/waveforms/IMRPhenomD.py` & `ripplegw-0.0.6/src/ripple/waveforms/IMRPhenomD.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,19 +139,20 @@
 
     phi_TF2 = (
         phi0 * ((PI * fM_s) ** -(5.0 / 3.0))
         + phi1 * ((PI * fM_s) ** -(4.0 / 3.0))
         + phi2 * ((PI * fM_s) ** -1.0)
         + phi3 * ((PI * fM_s) ** -(2.0 / 3.0))
         + phi4 * ((PI * fM_s) ** -(1.0 / 3.0))
-        + phi5_log * jnp.log(v) + phi5
+        + phi5_log * jnp.log(v)
+        + phi5
         + phi6_log * jnp.log(v) * ((PI * fM_s) ** (1.0 / 3.0))
         + phi6 * ((PI * fM_s) ** (1.0 / 3.0))
         + phi7 * ((PI * fM_s) ** (2.0 / 3.0))
-    ) * (3.0 / (128.0 * eta)) - PI/4.0
+    ) * (3.0 / (128.0 * eta)) - PI / 4.0
     phi_Ins = (
         phi_TF2
         + (
             coeffs[7] * fM_s
             + (3.0 / 4.0) * coeffs[8] * (fM_s ** (4.0 / 3.0))
             + (3.0 / 5.0) * coeffs[9] * (fM_s ** (5.0 / 3.0))
             + (1.0 / 2.0) * coeffs[10] * (fM_s**2.0)
@@ -165,17 +166,15 @@
     m1, m2, _, _ = theta
     m1_s = m1 * gt
     m2_s = m2 * gt
     M_s = m1_s + m2_s
     eta = m1_s * m2_s / (M_s**2.0)
 
     phi_IIa_raw = (
-        coeffs[11] * fM_s
-        + coeffs[12] * jnp.log(fM_s)
-        - coeffs[13] * (fM_s**-3.0) / 3.0
+        coeffs[11] * fM_s + coeffs[12] * jnp.log(fM_s) - coeffs[13] * (fM_s**-3.0) / 3.0
     ) / eta
 
     return phi_IIa_raw
 
 
 def get_IIb_raw_phase(fM_s: Array, theta: Array, coeffs: Array, f_RD, f_damp) -> Array:
     m1, m2, _, _ = theta
@@ -597,14 +596,16 @@
     f_ref: Reference frequency for the waveform
 
     Returns:
     --------
       hp (array): Strain of the plus polarization
       hc (array): Strain of the cross polarization
     """
+    assert len(params) == 8, "Incorrect number of parameters"
+
     iota = params[7]
     h0 = gen_IMRPhenomD(f, params, f_ref)
 
     hp = h0 * (1 / 2 * (1 + jnp.cos(iota) ** 2))
     hc = -1j * h0 * jnp.cos(iota)
 
     return hp, hc
```

### Comparing `ripplegw-0.0.5/src/ripple/waveforms/IMRPhenomD_QNMdata.py` & `ripplegw-0.0.6/src/ripple/waveforms/IMRPhenomD_QNMdata.py`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.5/src/ripple/waveforms/IMRPhenomD_utils.py` & `ripplegw-0.0.6/src/ripple/waveforms/IMRPhenomD_utils.py`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.5/src/ripple/waveforms/IMRPhenomPv2.py` & `ripplegw-0.0.6/src/ripple/waveforms/IMRPhenomPv2.py`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.5/src/ripple/waveforms/IMRPhenomPv2_utils.py` & `ripplegw-0.0.6/src/ripple/waveforms/IMRPhenomPv2_utils.py`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.5/src/ripple/waveforms/IMRPhenomXAS.py` & `ripplegw-0.0.6/src/ripple/waveforms/IMRPhenomXAS.py`

 * *Files 0% similar despite different names*

```diff
@@ -840,16 +840,15 @@
             -27312085.0
             - 10287648.0 * chi1**2.0 * (1.0 + delta)
             + 24.0
             * (
                 428652.0 * chi2**2 * (-1 + delta)
                 + (
                     -1975055.0
-                    + 10584.0
-                    * (81.0 * chi1**2.0 - 94.0 * chi1 * chi2 + 81.0 * chi2**2)
+                    + 10584.0 * (81.0 * chi1**2.0 - 94.0 * chi1 * chi2 + 81.0 * chi2**2)
                 )
                 * eta
                 + 1473794.0 * eta2
             )
         )
         / 8.128512e6
     ) * (PI ** (4.0 / 3.0))
```

### Comparing `ripplegw-0.0.5/src/ripple/waveforms/IMRPhenomX_utils.py` & `ripplegw-0.0.6/src/ripple/waveforms/IMRPhenomX_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,25 +302,17 @@
         + (
             (
                 -24.181508118588667
                 + 115.49264174560281 * eta
                 - 380.19778216022763 * eta**2
             )
             * S
-            + (
-                24.72585609641552
-                - 328.3762360751952 * eta
-                + 725.6024119989094 * eta**2
-            )
+            + (24.72585609641552 - 328.3762360751952 * eta + 725.6024119989094 * eta**2)
             * S**2
-            + (
-                23.404604124552
-                - 646.3410199799737 * eta
-                + 1941.8836639529036 * eta**2
-            )
+            + (23.404604124552 - 646.3410199799737 * eta + 1941.8836639529036 * eta**2)
             * S**3
             + (
                 -12.814828278938885
                 - 325.92980012408367 * eta
                 + 1320.102640190539 * eta**2
             )
             * S**4
@@ -468,17 +460,15 @@
     numerator = (
         NoSpin_coeffs[0]
         + NoSpin_coeffs[1] * eta
         + NoSpin_coeffs[2] * eta**2
         + NoSpin_coeffs[3] * eta**3
         + NoSpin_coeffs[4] * eta**4
     )
-    denominator = (
-        NoSpin_coeffs[5] + NoSpin_coeffs[6] * eta + NoSpin_coeffs[7] * eta**2
-    )
+    denominator = NoSpin_coeffs[5] + NoSpin_coeffs[6] * eta + NoSpin_coeffs[7] * eta**2
     return numerator / denominator
 
 
 def Amp_Eqspin_CV(EqSpin_coeffs, eta, S):
     numeratorS0 = (
         EqSpin_coeffs[0]
         + EqSpin_coeffs[1] * eta
```

### Comparing `ripplegw-0.0.5/src/ripplegw.egg-info/PKG-INFO` & `ripplegw-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ripplegw
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small jax package for differentiable and fast gravitational wave data analysis.
 Home-page: https://ripple.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/tedwards2412/ripple
 Keywords: gravitational waves,jax
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,41 +19,43 @@
 
 A small `jax` package for differentiable and fast gravitational wave data analysis.
 
 # Getting Started
 
 ### Installation
 
-Both waveforms have been tested extensively and match lalsuite implementations to machine precision across all the parameter space. 
+Both waveforms have been tested extensively and match `lalsuite` implementations to machine precision across all the parameter space. 
 
 Ripple can be installed using 
 
 ```
 pip3 install ripplegw
 ```
 
-Note that by default we do not include enable float64 in jax since we want allow users to use float32 to improve performance.
+Note that by default we do not include enable float64 in `jax` since we want allow users to use float32 to improve performance.
 If you require float64, please include the following code at the start of the script:
 
 ```
 from jax import config
 config.update("jax_enable_x64", True)
 ```
 
 See https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html for other common `jax` gotchas.
 
 ### Supported waveforms
 
 - IMRPhenomXAS (aligned spin)
 - IMRPhenomD (aligned spin)
 - IMRPhenomPv2 (Still finalizing sampling checks)
+- TaylorF2 with tidal effects
+- IMRPhenomD_NRTidalv2, verified for the low spin regime (chi1, chi2 < 0.05), further testing is required for higher spins
 
 ### Generating a waveform and its derivative
 
-Generating a waveform is increadibly easy. Below is an example of calling the PhenomXAS waveform model
+Generating a waveform is incredibly easy. Below is an example of calling the PhenomXAS waveform model
 to get the h_+ and h_x polarizations of the waveform model
 
 We start with some basic imports:
 
 ```python
 import jax.numpy as jnp
 
@@ -102,8 +104,28 @@
 
 @jax.jit
 def waveform(theta):
     return IMRPhenomXAS.gen_IMRPhenomXAS_hphc(fs, theta)
 ```
 
 
+### Citation
 
+Please cite this paper if you've used `ripple` in your work! It's really helpful!
+
+```bibtex
+@article{Edwards:2023sak,
+    author = "Edwards, Thomas D. P. and Wong, Kaze W. K. and Lam, Kelvin K. H. and Coogan, Adam and Foreman-Mackey, Daniel and Isi, Maximiliano and Zimmerman, Aaron",
+    title = "{ripple: Differentiable and Hardware-Accelerated Waveforms for Gravitational Wave Data Analysis}",
+    eprint = "2302.05329",
+    archivePrefix = "arXiv",
+    primaryClass = "astro-ph.IM",
+    month = "2",
+    year = "2023"
+}
+```
+
+### Contributions
+
+Contributions through pull requests are very welcome. Please also feel free to open new issues if there are missing features you'd like to see!
+
+The only requirement for contributions to be considered is that they are run through the black code formatter. This ensures we have a coherent format and makes the code easier to review/read!
```

### Comparing `ripplegw-0.0.5/src/ripplegw.egg-info/SOURCES.txt` & `ripplegw-0.0.6/src/ripplegw.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+src/ripple/FD_waveform.py
 src/ripple/__init__.py
 src/ripple/constants.py
 src/ripple/noise.py
 src/ripple/typing.py
 src/ripple/noise_resources/O2_ASD.dat
 src/ripple/noise_resources/O3a_Livingston_ASD.dat
 src/ripple/noise_resources/__init__.py
 src/ripple/noise_resources/aLIGO.dat
 src/ripple/noise_resources/aLIGOZeroDetHighPower.dat
 src/ripple/noise_resources/ce.dat
 src/ripple/noise_resources/et.dat
 src/ripple/waveforms/IMRPhenomD.py
+src/ripple/waveforms/IMRPhenomD_NRTidalv2.py
 src/ripple/waveforms/IMRPhenomD_QNMdata.py
 src/ripple/waveforms/IMRPhenomD_utils.py
 src/ripple/waveforms/IMRPhenomPv2.py
 src/ripple/waveforms/IMRPhenomPv2_utils.py
 src/ripple/waveforms/IMRPhenomXAS.py
 src/ripple/waveforms/IMRPhenomX_utils.py
+src/ripple/waveforms/IMRPhenom_tidal_utils.py
+src/ripple/waveforms/TaylorF2.py
 src/ripple/waveforms/__init__.py
 src/ripplegw.egg-info/PKG-INFO
 src/ripplegw.egg-info/SOURCES.txt
 src/ripplegw.egg-info/dependency_links.txt
 src/ripplegw.egg-info/requires.txt
-src/ripplegw.egg-info/top_level.txt
+src/ripplegw.egg-info/top_level.txt
+test/test_conversion.py
```

