# Comparing `tmp/miepython-2.5.3.tar.gz` & `tmp/miepython-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miepython-2.5.3.tar", last modified: Sat Aug  5 21:30:03 2023, max compression
+gzip compressed data, was "miepython-2.5.4.tar", last modified: Tue May  7 23:40:07 2024, max compression
```

## Comparing `miepython-2.5.3.tar` & `miepython-2.5.4.tar`

### file list

```diff
@@ -1,38 +1,33 @@
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-05 21:30:03.914645 miepython-2.5.3/
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-05 21:30:03.899672 miepython-2.5.3/.github/
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-05 21:30:03.904895 miepython-2.5.3/.github/workflows/
--rw-r--r--   0 prahl      (501) staff       (20)      762 2023-08-05 20:43:21.000000 miepython-2.5.3/.github/workflows/test.yml
--rw-r--r--   0 prahl      (501) staff       (20)      164 2022-01-27 02:10:04.000000 miepython-2.5.3/.gitignore
--rw-r--r--   0 prahl      (501) staff       (20)     5949 2023-08-05 21:28:58.000000 miepython-2.5.3/CHANGELOG.rst
--rw-r--r--   0 prahl      (501) staff       (20)      328 2023-05-26 22:17:36.000000 miepython-2.5.3/CITATION.cff
--rw-r--r--   0 prahl      (501) staff       (20)     1055 2021-03-21 17:45:57.000000 miepython-2.5.3/LICENSE.txt
--rw-r--r--   0 prahl      (501) staff       (20)      450 2023-08-05 21:24:42.000000 miepython-2.5.3/MANIFEST.in
--rw-r--r--   0 prahl      (501) staff       (20)     4246 2023-08-05 21:30:03.914918 miepython-2.5.3/PKG-INFO
--rw-r--r--   0 prahl      (501) staff       (20)     3314 2023-05-26 22:17:36.000000 miepython-2.5.3/README.rst
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-05 21:30:03.906646 miepython-2.5.3/miepython/
--rw-r--r--   0 prahl      (501) staff       (20)     1498 2023-08-05 21:28:50.000000 miepython-2.5.3/miepython/__init__.py
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-05 21:30:03.910738 miepython-2.5.3/miepython/data/
--rw-r--r--   0 prahl      (501) staff       (20)     1337 2022-01-27 02:10:04.000000 miepython-2.5.3/miepython/data/Johnson.txt
--rw-r--r--   0 prahl      (501) staff       (20)     1337 2022-01-27 02:10:04.000000 miepython-2.5.3/miepython/data/ag-Johnson.txt
--rw-r--r--   0 prahl      (501) staff       (20)    36719 2022-01-27 02:10:04.000000 miepython-2.5.3/miepython/data/segelstein81_index.txt
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-05 21:30:03.912953 miepython-2.5.3/miepython/examples/
--rwxr-xr-x   0 prahl      (501) staff       (20)      684 2021-07-09 19:31:22.000000 miepython-2.5.3/miepython/examples/01_dielectric.py
--rwxr-xr-x   0 prahl      (501) staff       (20)      804 2021-07-09 19:33:51.000000 miepython-2.5.3/miepython/examples/02_glass.py
--rwxr-xr-x   0 prahl      (501) staff       (20)      921 2021-07-09 19:46:36.000000 miepython-2.5.3/miepython/examples/03_droplets.py
--rwxr-xr-x   0 prahl      (501) staff       (20)     2717 2022-03-12 23:14:57.000000 miepython-2.5.3/miepython/examples/04_gold.py
--rw-r--r--   0 prahl      (501) staff       (20)    28001 2023-08-04 18:43:45.000000 miepython-2.5.3/miepython/miepython.py
--rw-r--r--   0 prahl      (501) staff       (20)    25628 2023-08-04 18:17:11.000000 miepython-2.5.3/miepython/miepython_nojit.py
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-05 21:30:03.909224 miepython-2.5.3/miepython.egg-info/
--rw-r--r--   0 prahl      (501) staff       (20)     4246 2023-08-05 21:30:03.000000 miepython-2.5.3/miepython.egg-info/PKG-INFO
--rw-r--r--   0 prahl      (501) staff       (20)      673 2023-08-05 21:30:03.000000 miepython-2.5.3/miepython.egg-info/SOURCES.txt
--rw-r--r--   0 prahl      (501) staff       (20)        1 2023-08-05 21:30:03.000000 miepython-2.5.3/miepython.egg-info/dependency_links.txt
--rw-r--r--   0 prahl      (501) staff       (20)       23 2023-08-05 21:30:03.000000 miepython-2.5.3/miepython.egg-info/requires.txt
--rw-r--r--   0 prahl      (501) staff       (20)       10 2023-08-05 21:30:03.000000 miepython-2.5.3/miepython.egg-info/top_level.txt
--rw-r--r--   0 prahl      (501) staff       (20)      179 2023-08-05 20:38:12.000000 miepython-2.5.3/pyproject.toml
--rw-r--r--   0 prahl      (501) staff       (20)      179 2023-08-05 20:42:09.000000 miepython-2.5.3/requirements-dev.txt
--rw-r--r--   0 prahl      (501) staff       (20)       22 2021-04-25 22:33:21.000000 miepython-2.5.3/requirements.txt
--rw-r--r--   0 prahl      (501) staff       (20)     1105 2023-08-05 21:30:03.916087 miepython-2.5.3/setup.cfg
--rw-r--r--   0 prahl      (501) staff       (20)     1095 2022-03-12 23:40:23.000000 miepython-2.5.3/setup.py
-drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-08-05 21:30:03.914081 miepython-2.5.3/tests/
--rwxr-xr-x   0 prahl      (501) staff       (20)    25541 2023-08-05 19:50:31.000000 miepython-2.5.3/tests/test_jit.py
--rwxr-xr-x   0 prahl      (501) staff       (20)    25542 2023-08-05 19:50:38.000000 miepython-2.5.3/tests/test_nojit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:07.010309 miepython-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-05-07 23:39:48.000000 miepython-2.5.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-07 23:39:48.000000 miepython-2.5.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-07 23:39:48.000000 miepython-2.5.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-07 23:39:48.000000 miepython-2.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-07 23:40:07.010309 miepython-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-05-07 23:39:48.000000 miepython-2.5.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:07.010309 miepython-2.5.4/miepython/
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-07 23:39:48.000000 miepython-2.5.4/miepython/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:07.010309 miepython-2.5.4/miepython/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-07 23:39:48.000000 miepython-2.5.4/miepython/data/Johnson.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-07 23:39:48.000000 miepython-2.5.4/miepython/data/ag-Johnson.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    36719 2024-05-07 23:39:48.000000 miepython-2.5.4/miepython/data/segelstein81_index.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:07.010309 miepython-2.5.4/miepython/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      626 2024-05-07 23:39:48.000000 miepython-2.5.4/miepython/examples/01_dielectric.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1116 2024-05-07 23:39:48.000000 miepython-2.5.4/miepython/examples/02_glass.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1401 2024-05-07 23:39:48.000000 miepython-2.5.4/miepython/examples/03_droplets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2728 2024-05-07 23:39:48.000000 miepython-2.5.4/miepython/examples/04_gold.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26657 2024-05-07 23:39:48.000000 miepython-2.5.4/miepython/miepython.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24554 2024-05-07 23:39:48.000000 miepython-2.5.4/miepython/miepython_nojit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:07.010309 miepython-2.5.4/miepython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-07 23:40:06.000000 miepython-2.5.4/miepython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-07 23:40:07.000000 miepython-2.5.4/miepython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:40:06.000000 miepython-2.5.4/miepython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 23:40:06.000000 miepython-2.5.4/miepython.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 23:40:06.000000 miepython-2.5.4/miepython.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-07 23:39:48.000000 miepython-2.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-07 23:39:48.000000 miepython-2.5.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 23:39:48.000000 miepython-2.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-07 23:40:07.010309 miepython-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-07 23:39:48.000000 miepython-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:07.010309 miepython-2.5.4/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27539 2024-05-07 23:39:48.000000 miepython-2.5.4/tests/test_mie.py
```

### Comparing `miepython-2.5.3/CHANGELOG.rst` & `miepython-2.5.4/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 Changelog
 =========
 
+2.5.4 (5/7/2024)
+--------------------
+*   document normalization in docstrings
+*   add version and year to CITATION.cff
+*   remove 'v' from version numbers
+*   add github script and workflow to auto-update CITATION.cff
+*   add conda badge to readme
+*   clean up README.rst
+*   use svg images
+*   use a single tests/test_mie for jit and non-jit tests
+*   support ruff
+*   test python versions 3.7 to 3.12
+*   fix badges
+*   remove unused functions
+*   fix zenodo link
+
 v2.5.3 (8/5/2023)
 -------------------
 *   conda-forge fails because test files are not included
 
 v2.5.1 (8/5/2023)
 -------------------
 *   change tests to accommodate conda-forge
```

### Comparing `miepython-2.5.3/LICENSE.txt` & `miepython-2.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.5.3/miepython/__init__.py` & `miepython-2.5.4/miepython/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     miepython.i_unpolarized(m, x, mu, norm='one')
 
 The scattering matrix
 
     miepython.mie_phase_matrix(m, x, mu)
 
 """
-__version__ = '2.5.3'
+__version__ = '2.5.4'
 __author__ = 'Scott Prahl'
 __email__ = 'scott.prahl@oit.edu'
-__copyright__ = 'Copyright 2017-23, Scott Prahl'
+__copyright__ = '2017-24, Scott Prahl'
 __license__ = 'MIT'
-__url__ = 'https://github.com/scottprahl/miepython.git'
+__url__ = 'https://github.com/scottprahl/miepython'
 
 from .miepython import *
```

### Comparing `miepython-2.5.3/miepython/data/Johnson.txt` & `miepython-2.5.4/miepython/data/Johnson.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.5.3/miepython/data/ag-Johnson.txt` & `miepython-2.5.4/miepython/data/ag-Johnson.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.5.3/miepython/data/segelstein81_index.txt` & `miepython-2.5.4/miepython/data/segelstein81_index.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.5.3/miepython/examples/01_dielectric.py` & `miepython-2.5.4/miepython/examples/01_dielectric.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 #!/usr/bin/env python3
 
-"""
-Plot the extinction efficiency as a function of particle size.
-
-This is a comparision of total extinction for non-absorbing and absorbing
-spheres.
-"""
+"""Plot the extinction efficiency as a function of particle size."""
 
 import numpy as np
 import matplotlib.pyplot as plt
 import miepython
 
-x = np.linspace(0.1, 100, 300)
-
-# mie() will automatically try to do the right thing
+x = np.linspace(0.1, 100, 1000)
 
+plt.figure(figsize=(8, 4.5))
 qext, qsca, qback, g = miepython.mie(1.5, x)
-plt.plot(x, qext, color='red', label="1.5")
+plt.plot(x, qext, color='red', label="$n=1.5$")
 
 qext, qsca, qback, g = miepython.mie(1.5 - 0.1j, x)
-plt.plot(x, qext, color='blue', label="1.5-0.1j")
+plt.plot(x, qext, color='blue', label="$n=1.5-0.1j$")
 
-plt.title("Comparison of extinction for absorbing and non-absorbing spheres")
-plt.xlabel("Size Parameter (-)")
-plt.ylabel("Qext")
+plt.title("Absorbing and Non-absorbing Spheres")
+plt.xlabel("Size Parameter [–]")
+plt.ylabel("Extinction Efficiency $Q_{ext}$ [–]")
 plt.legend()
-# plt.show()
+# plt.savefig('../../docs/01_plot.svg')
+plt.show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `miepython-2.5.3/miepython/examples/02_glass.py` & `miepython-2.5.4/miepython/examples/02_glass.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 #!/usr/bin/env python3
 
-"""
-Plot the scattering efficiency for 4 micron glass spheres.
-
-This graph shows scattering as a function of wavelength.
-"""
-
+"""Plot the scattering efficiency for 4 micron glass spheres."""
 import numpy as np
 import matplotlib.pyplot as plt
 import miepython
 
+
+def n_bk7(wavelength):
+    """
+    Refractive index of BK7 glass at a wavelength.
+
+    Equation is from https://refractiveindex.info/?shelf=glass&book=BK7&page=SCHOTT
+
+    Args:
+        wavelength: wavelength in microns
+    Returns:
+        index of refraction
+    """
+    m_squared = 1 + 1.03961212 / (1 - 0.00600069867 / lambda0**2)
+    m_squared += 0.231792344 / (1 - 0.0200179144 / lambda0**2)
+    m_squared += 1.01046945 / (1 - 103.560653 / lambda0**2)
+    refractive_index = np.sqrt(m_squared)
+    return refractive_index
+
+
 radius = 2                      # in microns
-lambda0 = np.linspace(0.2, 1.2, 200)  # also in microns
+lambda0 = np.linspace(0.2, 1.2, 1000)  # also in microns
 x = 2 * np.pi * radius / lambda0
+m = n_bk7(lambda0)
 
-# from https://refractiveindex.info/?shelf=glass&book=BK7&page=SCHOTT
-m2 = 1 + 1.03961212 / (1 - 0.00600069867 / lambda0**2)
-m2 += 0.231792344 / (1 - 0.0200179144 / lambda0**2)
-m2 += 1.01046945 / (1 - 103.560653 / lambda0**2)
-m = np.sqrt(m2)
-
+plt.figure(figsize=(8, 4.5))
 qext, qsca, qback, g = miepython.mie(m, x)
 plt.plot(lambda0 * 1000, qsca)
 
-plt.title("BK7 glass spheres 4 micron diameter")
-plt.xlabel("Wavelength (nm)")
-plt.ylabel("Scattering Efficiency (-)")
-# plt.show()
+plt.title("4µm diameter BK7 glass spheres")
+plt.xlabel("Wavelength [nm]")
+plt.ylabel("Scattering Efficiency [–]")
+# plt.savefig('../../docs/02_plot.svg')
+plt.show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `miepython-2.5.3/miepython/examples/04_gold.py` & `miepython-2.5.4/miepython/examples/04_gold.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 #!/usr/bin/env python3
 
-"""
-Plot the scattering cross section for 100nm gold spheres.
-
-The resulting graph is as a function of wavelength.
-"""
+"""Plot the scattering cross section for 100nm gold spheres."""
 
 import numpy as np
 import matplotlib.pyplot as plt
 import miepython
 
 # from https://refractiveindex.info/?shelf = main&book = Au&page = Johnson
 # wavelength in microns
@@ -38,29 +34,28 @@
 cross_section_area = np.pi * radius ** 2
 mu_a = 4 * np.pi * ref_k / ref_lam    # nm
 qext, qsca, qback, g = miepython.mie(m, x)
 
 sca_cross_section = qsca * cross_section_area
 abs_cross_section = (qext - qsca) * cross_section_area
 
-plt.subplots(3, 1, figsize=(9, 9))
+plt.subplots(3, 1, figsize=(8, 8))
 plt.subplot(311)
-plt.plot(ref_lam * 1000, ref_n, 'ob')
-plt.plot(ref_lam * 1000, -ref_k, 'sr')
+plt.plot(ref_lam * 1000, ref_n, 'ob', markersize=2)
+plt.plot(ref_lam * 1000, -ref_k, 'sr', markersize=2)
 plt.title("Gold Spheres 200nm diameter")
-plt.xticks([])
 plt.text(700, 1, "real refractive index", color='blue')
 plt.text(1100, -6, "imaginary refractive index", color='red')
 
 plt.subplot(312)
-plt.plot(ref_lam * 1000, 1000 / mu_a, 'ob')
+plt.plot(ref_lam * 1000, 1000 / mu_a, 'ob', markersize=2)
 plt.ylabel("Absorption Depth [nm]")
 
 plt.subplot(313)
-plt.plot(ref_lam * 1000, abs_cross_section, 'ob')
-plt.plot(ref_lam * 1000, sca_cross_section, 'sr')
+plt.plot(ref_lam * 1000, abs_cross_section, 'ob', markersize=2)
+plt.plot(ref_lam * 1000, sca_cross_section, 'sr', markersize=2)
 plt.xlabel("Wavelength (nm)")
-plt.ylabel("Cross Section (µm²)")
+plt.ylabel("Cross Section [µm²]")
 plt.text(700, 0.01, "absorption", color='blue')
 plt.text(750, 0.1, "scattering", color='red')
-plt.savefig("04_plot.png")
-# plt.show()
+# plt.savefig("../../docs/04_plot.svg")
+plt.show()
```

### Comparing `miepython-2.5.3/miepython/miepython.py` & `miepython-2.5.4/miepython/miepython_nojit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-# pylint: disable=invalid-name
 # pylint: disable=unused-argument
-# pylint: disable=too-many-locals
-# pylint: disable=no-member
-# pylint: disable=bare-except
-# pylint: disable=too-many-arguments
 # pylint: disable=too-many-return-statements
 
 """
-Mie scattering calculations for perfect spheres JITTED!.
+Mie scattering calculations for perfect spheres.
 
 Extensive documentation is at <https://miepython.readthedocs.io>
 
 `miepython` is a pure Python module to calculate light scattering of
 a plane wave by non-np.absorbing, partially-np.absorbing, or perfectly conducting
 spheres.
 
@@ -37,15 +32,14 @@
 
     miepython.i_per(m, x, mu)
     miepython.i_par(m, x, mu)
     miepython.i_unpolarized(m, x, mu)
 """
 
 import numpy as np
-from numba import njit, int32, float64, complex128
 
 __all__ = ('ez_mie',
            'ez_intensities',
            'i_par',
            'i_per',
            'i_unpolarized',
            'mie',
@@ -53,15 +47,14 @@
            'mie_phase_matrix',
            'mie_cdf',
            'mie_mu_with_uniform_cdf',
            'generate_mie_costheta',
            )
 
 
-@njit((complex128, int32), cache=True)
 def _Lentz_Dn(z, N):
     """
     Compute the logarithmic derivative of the Ricatti-Bessel function.
 
     Args:
         z: function argument
         N: order of Ricatti-Bessel function
@@ -86,15 +79,14 @@
         ratio = alpha_j1 / alpha_j2
         zinv *= -1
         runratio = ratio * runratio
 
     return -N / z + runratio
 
 
-@njit((complex128, int32, complex128[:]), cache=True)
 def _D_downwards(z, N, D):
     """
     Compute the logarithmic derivative by downwards recurrence.
 
     Args:
         z: function argument
         N: order of Ricatti-Bessel function
@@ -103,15 +95,14 @@
     """
     last_D = _Lentz_Dn(z, N)
     for n in range(N, 0, -1):
         last_D = n / z - 1.0 / (last_D + n / z)
         D[n - 1] = last_D
 
 
-@njit((complex128, int32, complex128[:]), cache=True)
 def _D_upwards(z, N, D):
     """
     Compute the logarithmic derivative by upwards recurrence.
 
     Args:
         z: function argument
         N: order of Ricatti-Bessel function
@@ -120,15 +111,14 @@
     """
     exp = np.exp(-2j * z)
     D[1] = -1 / z + (1 - exp) / ((1 - exp) / z - 1j * (1 + exp))
     for n in range(2, N):
         D[n] = 1 / (n / z - D[n - 1]) - n / z
 
 
-@njit((complex128, float64, int32), cache=True)
 def _D_calc(m, x, N):
     """
     Compute the logarithmic derivative using best method.
 
     Args:
         m: the complex index of refraction of the sphere
         x: the size parameter of the sphere
@@ -144,29 +134,28 @@
     if n < 1 or n > 10 or kappa > 10 or x * kappa >= 3.9 - 10.8 * n + 13.78 * n**2:
         _D_downwards(m * x, N, D)
     else:
         _D_upwards(m * x, N, D)
     return D
 
 
-@njit((complex128, float64), cache=True)
 def _mie_An_Bn(m, x):
     """
     Compute arrays of Mie coefficients A and B for a sphere.
 
     This estimates the size of the arrays based on Wiscombe's formula. The length
     of the arrays is chosen so that the error when the series are summed is
     around 1e-6.
 
     Args:
         m: the complex index of refraction of the sphere
         x: the size parameter of the sphere
 
     Returns:
-        a, b: arrays of Mie coefficents An and Bn
+        An, Bn: arrays of Mie coefficents
     """
     nstop = int(x + 4.05 * x**0.33333 + 2.0) + 1
     a = np.zeros(nstop - 1, dtype=np.complex128)
     b = np.zeros(nstop - 1, dtype=np.complex128)
 
     psi_nm1 = np.sin(x)                   # nm1 = n-1 = 0
     psi_n = psi_nm1 / x - np.cos(x)       # n = 1
@@ -196,39 +185,37 @@
             xi_n = xi
             psi_nm1 = psi_n
             psi_n = xi_n.real
 
     return a, b
 
 
-@njit((complex128, float64), cache=True)
-def _small_conducting_mie(m, x):
+def _small_conducting_mie(_m, x):
     """
     Calculate the efficiencies for a small conducting spheres.
 
     Typically used for small conducting spheres where x < 0.1 and
     m.real == 0
 
     Args:
-        m: the complex index of refraction of the sphere
+        _m: the complex index of refraction of the sphere (unused)
         x: the size parameter of the sphere
 
     Returns:
         qext: the total extinction efficiency
         qsca: the scattering efficiency
         qback: the backscatter efficiency
         g: the average cosine of the scattering phase function
     """
-    ahat1 = complex(0, 2.0 / 3.0 * (1 - 0.2 * x**2))
-    ahat1 /= complex(1 - 0.5 * x**2, 2.0 / 3.0 * x**3)
-
-    bhat1 = complex(0.0, (x**2 - 10.0) / 30.0)
-    bhat1 /= complex(1 + 0.5 * x**2, -x**3 / 3.0)
-    ahat2 = complex(0.0, x**2 / 30.0)
-    bhat2 = complex(0.0, -x**2 / 45.0)
+    ahat1 = complex(0, 2.0 / 3.0 * (1 - 0.2 * x**2)) / \
+        complex(1 - 0.5 * x**2, 2.0 / 3.0 * x**3)
+    bhat1 = complex(0.0, (x**2 - 10.0) / 30.0) / \
+        complex(1 + 0.5 * x**2, -x**3 / 3.0)
+    ahat2 = complex(0.0, x**2 / 30.)
+    bhat2 = complex(0.0, -x**2 / 45.)
 
     qsca = x**4 * (6 * np.abs(ahat1)**2
                    + 6 * np.abs(bhat1)**2
                    + 10 * np.abs(ahat2)**2
                    + 10 * np.abs(bhat2)**2)
     qext = qsca
     g = ahat1.imag * (ahat2.imag + bhat1.imag)
@@ -237,15 +224,14 @@
     g *= 6 * x**4 / qsca
 
     qback = 9 * x**4 * np.abs(ahat1 - bhat1 - 5 / 3 * (ahat2 - bhat2))**2
 
     return [qext, qsca, qback, g]
 
 
-@njit((complex128, float64), cache=True)
 def _small_mie(m, x):
     """
     Calculate the efficiencies for a small sphere.
 
     Typically used for small spheres where x<0.1
 
     Args:
@@ -261,18 +247,16 @@
     m2 = m * m
     x2 = x * x
 
     D = m2 + 2 + (1 - 0.7 * m2) * x2
     D -= (8 * m**4 - 385 * m2 + 350) * x**4 / 1400.0
     D += 2j * (m2 - 1) * x**3 * (1 - 0.1 * x2) / 3
     ahat1 = 2j * (m2 - 1) / 3 * (1 - 0.1 * x2 + (4 * m2 + 5) * x**4 / 1400) / D
-
     bhat1 = 1j * x2 * (m2 - 1) / 45 * (1 + (2 * m2 - 5) / 70 * x2)
     bhat1 /= 1 - (2 * m2 - 5) / 30 * x2
-
     ahat2 = 1j * x2 * (m2 - 1) / 15 * (1 - x2 / 14)
     ahat2 /= 2 * m2 + 3 - (2 * m2 - 7) / 14 * x2
 
     T = np.abs(ahat1)**2 + np.abs(bhat1)**2 + 5 / 3 * np.abs(ahat2)**2
     temp = ahat2 + bhat1
     g = (ahat1 * temp.conjugate()).real / T
 
@@ -285,15 +269,14 @@
 
     sback = 1.5 * x**3 * (ahat1 - bhat1 - 5 * ahat2 / 3)
     qback = 4 * np.abs(sback)**2 / x2
 
     return [qext, qsca, qback, g]
 
 
-@njit((complex128, float64), cache=True)
 def _mie_scalar(m, x):
     """
     Calculate the efficiencies for a sphere when both m and x are scalars.
 
     Args:
         m: the complex index of refraction of the sphere
         x: the size parameter of the sphere
@@ -384,205 +367,78 @@
             xx = x[i]
 
         qext[i], qsca[i], qback[i], g[i] = _mie_scalar(mm, xx)
 
     return qext, qsca, qback, g
 
 
-@njit((complex128, float64, float64[:]), cache=True)
-def _small_mie_conducting_S1_S2(m, x, mu):
-    """
-    Calculate the scattering amplitudes for small conducting spheres.
-
-    The spheres are small perfectly conducting (reflecting) spheres (x<0.1).
-    The amplitude functions have been normalized so that when integrated
-    over all 4𝜋 solid angles, the integral will be qext(𝜋x²).
-
-    The units are weird, sr**(-0.5)
-
-    Args:
-        m: the complex index of refraction of the sphere
-        x: the size parameter of the sphere
-        mu: the angles, cos(theta), to calculate scattering amplitudes
-
-    Returns:
-        S1, S2: the scattering amplitudes at each angle mu [sr**(-0.5)]
-    """
-    ahat1 = 2j / 3 * (1 - 0.2 * x**2) / (1 - 0.5 * x**2 + 2j / 3 * x**3)
-    bhat1 = 1j / 3 * (0.1 * x**2 - 1) / (1 + 0.5 * x**2 - 1j / 3 * x**3)
-    ahat2 = 1j / 30 * x**2
-    bhat2 = -1j * x**2 / 45
-
-    S1 = 1.5 * x**3 * (ahat1 + bhat1 * mu
-                       + 5 / 3 * ahat2 * mu
-                       + 5 / 3 * bhat2 * (2 * mu**2 - 1))
-
-    S2 = 1.5 * x**3 * (bhat1 + ahat1 * mu
-                       + 5 / 3 * bhat2 * mu
-                       + 5 / 3 * ahat2 * (2 * mu**2 - 1))
-
-    qext = x**4 * (6 * np.abs(ahat1)**2
-                   + 6 * np.abs(bhat1)**2
-                   + 10 * np.abs(ahat2)**2
-                   + 10 * np.abs(bhat2)**2)
-
-    norm = np.sqrt(qext * np.pi * x**2)
-    S1 /= norm
-    S2 /= norm
-
-    return [S1, S2]
-
-
-@njit((complex128, float64, float64[:]), cache=True)
-def _small_mie_S1_S2(m, x, mu):
-    """
-    Calculate the scattering amplitude functions for small spheres (x<0.1).
-
-    The amplitude functions have been normalized so that when integrated
-    over all 4*pi solid angles, the integral will be qext*pi*x**2.
-
-    The units are weird, sr**(-0.5)
-
-    Args:
-        m: the complex index of refraction of the sphere
-        x: the size parameter of the sphere
-        mu: the angles, cos(theta), to calculate scattering amplitudes
-
-    Returns:
-        S1, S2: the scattering amplitudes at each angle mu [sr**(-0.5)]
-    """
-    m2 = m * m
-    m4 = m2 * m2
-    x2 = x * x
-    x3 = x2 * x
-    x4 = x2 * x2
-
-    D = m2 + 2 + (1 - 0.7 * m2) * x2
-    D -= (8 * m4 - 385 * m2 + 350) * x4 / 1400.0
-    D += 2j * (m2 - 1) * x3 * (1 - 0.1 * x2) / 3
-    ahat1 = 2j * (m2 - 1) / 3 * (1 - 0.1 * x2 + (4 * m2 + 5) * x4 / 1400) / D
-    bhat1 = 1j * x2 * (m2 - 1) / 45 * (1 + (2 * m2 - 5) / 70 * x2)
-    bhat1 /= 1 - (2 * m2 - 5) / 30 * x2
-    ahat2 = 1j * x2 * (m2 - 1) / 15 * (1 - x2 / 14)
-    ahat2 /= 2 * m2 + 3 - (2 * m2 - 7) / 14 * x2
-
-    S1 = 1.5 * x3 * (ahat1 + bhat1 * mu + 5 / 3 * ahat2 * mu)
-    S2 = 1.5 * x3 * (bhat1 + ahat1 * mu + 5 / 3 * ahat2 * (2 * mu**2 - 1))
-
-    # norm = sqrt(qext*pi*x**2)
-    norm = np.sqrt(np.pi * 6 * x**3 * (ahat1 + bhat1 + 5 * ahat2 / 3).real)
-    S1 /= norm
-    S2 /= norm
-
-    return [S1, S2]
-
-
-@njit((complex128, float64, int32), cache=True)
-def normalization_factor(m, x, norm_int):
+def normalization_factor(m, x, norm_str):
     """
     Figure out scattering function normalization.
 
     Args:
-        a: complex array of An coefficients
-        b: complex array of Bn coefficients
+        m: complex index of refraction of sphere
         x: dimensionless sphere size
-        norm_int: integer that specifies normalization
+        norm_str: string describing type of normalization
 
     Returns:
         scaling factor needed for scattering function
     """
-    # Qsca normalization
-    if norm_int == 3:
-        return x * np.sqrt(np.pi)
-
-    # Bohren Normalization
-    if norm_int == 5:
-        return 0.5
-
-    # Wiscombe Normalization
-    if norm_int == 6:
-        return 1
-
-    # calculate qsca and qext
-    qext, qsca, _, _ = _mie_scalar(m, x)
-
-    # albedo Normalization
-    if norm_int == 0:
-        return x * np.sqrt(np.pi * qext)
-
-    # Unity normalization
-    if norm_int == 1:
-        return x * np.sqrt(qsca * np.pi)
+    factor = None
+    norm = norm_str.lower()
 
-    # 4pi Normalization
-    if norm_int == 2:
-        return x * np.sqrt(qsca / 4)
-
-    # Qext Normalization
-    if norm_int == 4:  # 4pi
-        return x * np.sqrt(qsca * np.pi / qext)
-
-    raise ValueError("norm-int must be in the range 0..6")
-
-
-def norm_string_to_integer(s):
-    """
-    Encode normalization choice as an integer.
-
-    This is needed because these string operations cannot be
-    done in a jitted function under numba.  We cannot use enums for
-    the same reason!
-
-    Args:
-        s: string describing normalization desired.
-
-    Returns:
-        integer used in _mie_S1_S2() determine normalization
-    """
-    norm = s.lower()
+    if norm in ['bohren']:
+        factor = 1 / 2
 
-    if norm in ['a', 'albedo']:
-        return 0
+    elif norm in ['wiscombe']:
+        factor = 1
 
-    if norm in ['1', 'one', 'unity']:
-        return 1
+    elif norm in ['qsca', 'scattering_efficiency']:
+        factor = x * np.sqrt(np.pi)
 
-    if norm in ['four_pi', '4pi']:
-        return 2
+    else:
+        qext, qsca, _, _ = _mie_scalar(m, x)
 
-    if norm in ['qsca', 'scattering_efficiency']:
-        return 3
+        if norm in ['a', 'albedo']:
+            factor = x * np.sqrt(np.pi * qext)
 
-    if norm in ['qext', 'extinction_efficiency']:
-        return 4
+        if norm in ['1', 'one', 'unity']:
+            factor = x * np.sqrt(qsca * np.pi)
 
-    if norm in ['bohren']:
-        return 5
+        if norm in ['four_pi', '4pi']:
+            factor = x * np.sqrt(qsca / 4)
 
-    if norm in ['wiscombe']:
-        return 6
+        if norm in ['qext', 'extinction_efficiency']:
+            factor = x * np.sqrt(qsca * np.pi / qext)
 
-    raise ValueError("normalization must be one of 'albedo' (default), 'one'"
-                     "'4pi', 'qext', 'qsca', 'bohren', or 'wiscombe'")
+    if factor is None:
+        raise ValueError("normalization must be one of 'albedo' (default), 'one'"
+                         "'4pi', 'qext', 'qsca', 'bohren', or 'wiscombe'")
+    return factor
 
 
-@njit((complex128, float64, float64[:], int32), cache=True)
-def _mie_S1_S2(m, x, mu, norm_int):
+def mie_S1_S2(m, x, mu, norm='albedo'):
     """
     Calculate the scattering amplitude functions for spheres.
 
     The amplitude functions have been normalized so that when integrated
     over all 4*pi solid angles, the integral will be qext*pi*x**2.
 
+    The normalization is controlled by `norm` and should be one of
+    ['albedo', 'one', '4pi', 'qext', 'qsca', 'bohren', or 'wiscombe']
+    The normalization describes the integral of the scattering phase
+    function over all 4𝜋 steradians.
+
     The units are weird, sr**(-0.5)
 
     Args:
         m: the complex index of refraction of the sphere
         x: the size parameter of the sphere
-        mu: array of angles, cos(theta), to calculate scattering amplitudes
+        mu: the angles, cos(theta), to calculate scattering amplitudes
+        norm: (optional) string describing scattering function normalization
 
     Returns:
         S1, S2: the scattering amplitudes at each angle mu [sr**(-0.5)]
     """
     a, b = _mie_An_Bn(m, x)
 
     nangles = len(mu)
@@ -591,59 +447,31 @@
 
     nstop = len(a)
     for k in range(nangles):
         pi_nm2 = 0
         pi_nm1 = 1
         for n in range(1, nstop):
             tau_nm1 = n * mu[k] * pi_nm1 - (n + 1) * pi_nm2
-
             S1[k] += (2 * n + 1) * (pi_nm1 * a[n - 1]
                                     + tau_nm1 * b[n - 1]) / (n + 1) / n
-
             S2[k] += (2 * n + 1) * (tau_nm1 * a[n - 1]
                                     + pi_nm1 * b[n - 1]) / (n + 1) / n
 
             temp = pi_nm1
             pi_nm1 = ((2 * n + 1) * mu[k] * pi_nm1 - (n + 1) * pi_nm2) / n
             pi_nm2 = temp
 
-    normalization = normalization_factor(m, x, norm_int)
+    normalization = normalization_factor(m, x, norm)
 
     S1 /= normalization
     S2 /= normalization
 
     return [S1, S2]
 
 
-def mie_S1_S2(m, x, mu, norm='albedo'):
-    """
-    Calculate the scattering amplitude functions for spheres.
-
-    The amplitude functions have been normalized so that when integrated
-    over all 4*pi solid angles, the integral will be qext*pi*x**2.
-
-    The units are weird, sr**(-0.5)
-
-    Args:
-        m: the complex index of refraction of the sphere
-        x: the size parameter of the sphere
-        mu: cos(theta) or array of angles [cos(theta_i)]
-
-    Returns:
-        S1, S2: the scattering amplitudes at each angle mu [sr**(-0.5)]
-    """
-    norm_int = norm_string_to_integer(norm)
-    if np.isscalar(mu):
-        mu_array = np.array([mu], dtype=float)
-        s1, s2 = _mie_S1_S2(m, x, mu_array, norm_int)
-        return s1[0], s2[0]
-
-    return _mie_S1_S2(m, x, mu, norm_int)
-
-
 def mie_phase_matrix(m, x, mu, norm='albedo'):
     """
     Calculate the scattering (Mueller) matrix.
 
     If mu has length N, then the returned matrix is 4x4xN.  If mu is a scalar
     then the matrix is 4x4
 
@@ -652,25 +480,31 @@
     *An Introduction to Atmospheric Radiation*, Second Edition.
 
     or
 
     Bohren and Huffman, *Absorption and Scattering of Light by Small Particles*,
     JOHN WILEY & SONS, page 112, (1983).
 
+    The normalization is controlled by `norm` and should be one of
+    ['albedo', 'one', '4pi', 'qext', 'qsca', 'bohren', or 'wiscombe']
+    The normalization describes the integral of the scattering phase
+    function over all 4𝜋 steradians.
+
     Args:
         m: the complex index of refraction of the sphere
         x: the size parameter of the sphere
-        mu: the angles, cos(theta), for the phase scattering matrix
+        mu: the angles, cos(theta), of the phase scattering matrix
+        norm: (optional) string describing scattering function normalization
 
     Returns:
         p: the phase scattering matrix [sr**(-1.0)]
     """
+    mu = np.atleast_1d(mu)
     s1, s2 = mie_S1_S2(m=m, x=x, mu=mu, norm=norm)
 
-    mu = np.atleast_1d(mu)
     s1_star = np.conjugate(s1)
     s2_star = np.conjugate(s2)
     m1 = (s1 * s1_star).real
     m2 = (s2 * s2_star).real
     s21 = (0.5 * (s1 * s2_star + s2 * s1_star)).real
     d21 = (-0.5j * (s1 * s2_star - s2 * s1_star)).real
     phase = np.zeros(shape=(4, 4, mu.size))
@@ -682,15 +516,15 @@
     phase[2, 3] = -d21
     phase[3, 2] = d21
     phase[3, 3] = s21
 
     return phase.squeeze()
 
 
-def mie_cdf(m, x, num, norm='albedo'):
+def mie_cdf(m, x, num):
     """
     Create a CDF for unpolarized scattering uniformly spaced in cos(theta).
 
     The CDF covers scattered (exit) angles ranging from 180 to 0 degrees.
     (The cosines are uniformly distributed over -1 to 1.) Because the angles
     are uniformly distributed in cos(theta), the scattering function is not
     sampled uniformly and therefore huge array sizes are needed to adequately
@@ -705,29 +539,20 @@
         num: length of desired CDF array
 
     Returns:
         mu: array of cosines of angles
         cdf: array of cumulative distribution function values
     """
     mu = np.linspace(-1, 1, num)
-    s1, s2 = mie_S1_S2(m, x, mu, norm)
-
-    s = (np.abs(s1)**2 + np.abs(s2)**2) / 2
-
-    cdf = np.zeros(num)
-    total = 0
-    for i in range(num):
-        # need the extra 2pi because scattering normalized over 4π steradians
-        total += s[i] * 2 * np.pi * (2 / num)
-        cdf[i] = total
-
+    intensity_per_mu = i_unpolarized(m, x, mu, norm='4pi') / num
+    cdf = np.cumsum(intensity_per_mu)
     return mu, cdf
 
 
-def mie_mu_with_uniform_cdf(m, x, num, norm='albedo'):
+def mie_mu_with_uniform_cdf(m, x, num):
     """
     Create a CDF for unpolarized scattering for uniform CDF.
 
     The CDF covers scattered (exit) angles ranging from 180 to 0 degrees.
     (The cosines are uniformly distributed over -1 to 1.) These angles mu
     correspond to uniform spacing of the cumulative distribution function
     for unpolarized Mie scattering where cdf[i] = i/(num-1).
@@ -745,15 +570,15 @@
         num: length of desired CDF array
 
     Returns:
         mu: array of cosines of angles (irregularly spaced)
         cdf: array of cumulative distribution function values
     """
     big_num = 2000                  # large to work with x up to 10
-    big_mu, big_cdf = mie_cdf(m, x, big_num, norm)
+    big_mu, big_cdf = mie_cdf(m, x, big_num)
     mu = np.empty(num)
     cdf = np.empty(num)
 
     mu[0] = -1                       # cos[180 degrees] is -1
     cdf[0] = 0                       # initial cdf is zero
 
     big_k = 0                        # index into big_cdf
@@ -766,16 +591,16 @@
         delta = big_cdf[big_k] - target
         delta_cdf = big_cdf[big_k] - big_cdf[big_k - 1]
         delta_mu = big_mu[big_k] - big_mu[big_k - 1]
 
         mu[k] = big_mu[big_k] - delta / delta_cdf * delta_mu   # interpolate
         cdf[k] = target
 
-#       print(' mu[',k,']=% .5f'%mu[k],' cdf[',k,']=% .5f'%cdf[k],
-#       'cdf=',big_cdf[big_k], fraction)
+#       print(' mu[', k, ']=% .5f'%mu[k], ' cdf[', k, ']=% .5f'%cdf[k],
+#       'cdf=', big_cdf[big_k], fraction)
 
     mu[num - 1] = 1                    # cos[0 degrees] is 1
     cdf[num - 1] = 1                   # last cdf is one
 
     return [mu, cdf]
 
 
@@ -787,16 +612,16 @@
     New random angles are generated by selecting a random interval
     mu[i] to mu[i+1] and choosing an angle uniformly distributed over
     the interval.
 
     Args:
        mu_cdf: a cumulative distribution function
 
-    Returns
-       The cosine of the scattering angle
+    Returns:
+       an array of random scattering angle cosines based on the CDF supplied.
     """
     # the following should be equivalent to these four lines
     # index = np.random.randint(0, high=len(mu_cdf))
     num = len(mu_cdf) - 1
     index = int(np.random.random() * num)
     if index >= num:
         index = num - 1
@@ -812,21 +637,27 @@
     Return the scattered intensity in a plane normal to the incident light.
 
     This is the scattered intensity in a plane that is perpendicular to the
     field of the incident plane wave. The intensity is normalized such
     that the integral of the unpolarized intensity over 4π steradians
     is equal to the single scattering albedo.
 
+    The normalization is controlled by `norm` and should be one of
+    ['albedo', 'one', '4pi', 'qext', 'qsca', 'bohren', or 'wiscombe']
+    The normalization describes the integral of the scattering phase
+    function over all 4𝜋 steradians.
+
     Args:
-       m: the complex index of refraction of the sphere
-       x: the size parameter of the sphere
-       mu: the angles, cos(theta), to calculate intensities
+        m: the complex index of refraction of the sphere
+        x: the size parameter of the sphere
+        mu: the angles, cos(theta), to calculate intensities
+        norm: (optional) string describing scattering function normalization
 
-    Returns
-       The intensity at each angle in the array mu.  Units [1/sr]
+    Returns:
+        The intensity at each angle in the array mu.  Units [1/sr]
     """
     s1, _ = mie_S1_S2(m, x, mu, norm)
     intensity = np.abs(s1)**2
     return intensity.astype('float')
 
 
 def i_par(m, x, mu, norm='albedo'):
@@ -834,42 +665,55 @@
     Return the scattered intensity in a plane parallel to the incident light.
 
     This is the scattered intensity in a plane that is parallel to the
     field of the incident plane wave. The intensity is normalized such
     that the integral of the unpolarized intensity over 4π steradians
     is equal to the single scattering albedo.
 
+    The normalization is controlled by `norm` and should be one of
+    ['albedo', 'one', '4pi', 'qext', 'qsca', 'bohren', or 'wiscombe']
+    The normalization describes the integral of the scattering phase
+    function over all 4𝜋 steradians.
+
     Args:
-       m: the complex index of refraction of the sphere
-       x: the size parameter
-       mu: the cos(theta) of each direction desired
+        m: the complex index of refraction of the sphere
+        x: the size parameter
+        mu: the cos(theta) of each direction desired
+        norm: (optional) string describing scattering function normalization
 
-    Returns
-       The intensity at each angle in the array mu.  Units [1/sr]
+    Returns:
+        The intensity at each angle in the array mu.  Units [1/sr]
     """
     _, s2 = mie_S1_S2(m, x, mu, norm)
     intensity = np.abs(s2)**2
     return intensity.astype('float')
 
 
 def i_unpolarized(m, x, mu, norm='albedo'):
     """
     Return the unpolarized scattered intensity at specified angles.
 
     This is the average value for randomly polarized incident light.
-    The intensity is normalized such that the integral of the unpolarized
-    intensity over 4π steradians is equal to the single scattering albedo.
+    The intensity is normalized such
+    that the integral of the unpolarized intensity over 4π steradians
+    is equal to the single scattering albedo.
+
+    The normalization is controlled by `norm` and should be one of
+    ['albedo', 'one', '4pi', 'qext', 'qsca', 'bohren', or 'wiscombe']
+    The normalization describes the integral of the scattering phase
+    function over all 4𝜋 steradians.
 
     Args:
-       m: the complex index of refraction of the sphere
-       x: the size parameter
-       mu: the cos(theta) of each direction desired
+        m: the complex index of refraction of the sphere
+        x: the size parameter
+        mu: the cos(theta) of each direction desired
+        norm: (optional) string describing scattering function normalization
 
-    Returns
-       The intensity at each angle in the array mu.  Units [1/sr]
+    Returns:
+        The intensity at each angle in the array mu.  Units [1/sr]
     """
     s1, s2 = mie_S1_S2(m, x, mu, norm)
     intensity = (np.abs(s1)**2 + np.abs(s2)**2) / 2
     return intensity.astype('float')
 
 
 def ez_mie(m, d, lambda0, n_env=1.0):
@@ -879,18 +723,18 @@
     Args:
         m: the complex index of refraction of the sphere [-]
         d: the diameter of the sphere                    [same units as lambda0]
         lambda0: wavelength in a vacuum                  [same units as d]
         n_env: real index of medium around sphere, optional.
 
     Returns:
-        qext: the total extinction efficiency                  [-].
-        qsca: the scattering efficiency                        [-].
-        qback: the backscatter efficiency                      [-].
-        g: the average cosine of the scattering phase function [-].
+        qext: the total extinction efficiency                  [-]
+        qsca: the scattering efficiency                        [-]
+        qback: the backscatter efficiency                      [-]
+        g: the average cosine of the scattering phase function [-]
     """
     m_env = m / n_env
     x_env = np.pi * d / (lambda0 / n_env)
     return mie(m_env, x_env)
 
 
 def ez_intensities(m, d, lambda0, mu, n_env=1.0, norm='albedo'):
@@ -902,20 +746,26 @@
 
     The scattered intensity is normalized such that the integral of the
     unpolarized intensity over 4𝜋 steradians is equal to the single scattering
     albedo.  The scattered intensity has units of inverse steradians [1/sr].
 
     The unpolarized scattering is the average of the two scattered intensities.
 
+    The normalization is controlled by `norm` and should be one of
+    ['albedo', 'one', '4pi', 'qext', 'qsca', 'bohren', or 'wiscombe']
+    The normalization describes the integral of the scattering phase
+    function over all 4𝜋 steradians.
+
     Args:
         m: the complex index of refraction of the sphere [-]
         d: the diameter of the sphere                    [same units as lambda0]
         lambda0: wavelength in a vacuum                  [same units as d]
         mu: the cos(theta) of each direction desired     [-]
-        n_env: real index of medium around sphere, optional
+        n_env: real index of medium around sphere, optional.
+        norm: (optional) string describing scattering function normalization
 
     Returns:
         ipar, iper: scattered intensity in parallel and perpendicular planes [1/sr]
     """
     m_env = m / n_env
     lambda_env = lambda0 / n_env
     x_env = np.pi * d / lambda_env
```

### Comparing `miepython-2.5.3/miepython/miepython_nojit.py` & `miepython-2.5.4/miepython/miepython.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,9 @@
-# pylint: disable=invalid-name
-# pylint: disable=unused-argument
-# pylint: disable=too-many-locals
-# pylint: disable=no-member
-# pylint: disable=bare-except
-# pylint: disable=too-many-arguments
-# pylint: disable=too-many-return-statements
-
 """
-Mie scattering calculations for perfect spheres.
+Mie scattering calculations for perfect spheres JITTED!.
 
 Extensive documentation is at <https://miepython.readthedocs.io>
 
 `miepython` is a pure Python module to calculate light scattering of
 a plane wave by non-np.absorbing, partially-np.absorbing, or perfectly conducting
 spheres.
 
@@ -37,14 +29,15 @@
 
     miepython.i_per(m, x, mu)
     miepython.i_par(m, x, mu)
     miepython.i_unpolarized(m, x, mu)
 """
 
 import numpy as np
+from numba import njit, int32, float64, complex128
 
 __all__ = ('ez_mie',
            'ez_intensities',
            'i_par',
            'i_per',
            'i_unpolarized',
            'mie',
@@ -52,14 +45,15 @@
            'mie_phase_matrix',
            'mie_cdf',
            'mie_mu_with_uniform_cdf',
            'generate_mie_costheta',
            )
 
 
+@njit((complex128, int32), cache=True)
 def _Lentz_Dn(z, N):
     """
     Compute the logarithmic derivative of the Ricatti-Bessel function.
 
     Args:
         z: function argument
         N: order of Ricatti-Bessel function
@@ -84,14 +78,15 @@
         ratio = alpha_j1 / alpha_j2
         zinv *= -1
         runratio = ratio * runratio
 
     return -N / z + runratio
 
 
+@njit((complex128, int32, complex128[:]), cache=True)
 def _D_downwards(z, N, D):
     """
     Compute the logarithmic derivative by downwards recurrence.
 
     Args:
         z: function argument
         N: order of Ricatti-Bessel function
@@ -100,14 +95,15 @@
     """
     last_D = _Lentz_Dn(z, N)
     for n in range(N, 0, -1):
         last_D = n / z - 1.0 / (last_D + n / z)
         D[n - 1] = last_D
 
 
+@njit((complex128, int32, complex128[:]), cache=True)
 def _D_upwards(z, N, D):
     """
     Compute the logarithmic derivative by upwards recurrence.
 
     Args:
         z: function argument
         N: order of Ricatti-Bessel function
@@ -116,14 +112,15 @@
     """
     exp = np.exp(-2j * z)
     D[1] = -1 / z + (1 - exp) / ((1 - exp) / z - 1j * (1 + exp))
     for n in range(2, N):
         D[n] = 1 / (n / z - D[n - 1]) - n / z
 
 
+@njit((complex128, float64, int32), cache=True)
 def _D_calc(m, x, N):
     """
     Compute the logarithmic derivative using best method.
 
     Args:
         m: the complex index of refraction of the sphere
         x: the size parameter of the sphere
@@ -139,28 +136,29 @@
     if n < 1 or n > 10 or kappa > 10 or x * kappa >= 3.9 - 10.8 * n + 13.78 * n**2:
         _D_downwards(m * x, N, D)
     else:
         _D_upwards(m * x, N, D)
     return D
 
 
+@njit((complex128, float64), cache=True)
 def _mie_An_Bn(m, x):
     """
     Compute arrays of Mie coefficients A and B for a sphere.
 
     This estimates the size of the arrays based on Wiscombe's formula. The length
     of the arrays is chosen so that the error when the series are summed is
     around 1e-6.
 
     Args:
         m: the complex index of refraction of the sphere
         x: the size parameter of the sphere
 
     Returns:
-        An, Bn: arrays of Mie coefficents
+        a, b: arrays of Mie coefficents An and Bn
     """
     nstop = int(x + 4.05 * x**0.33333 + 2.0) + 1
     a = np.zeros(nstop - 1, dtype=np.complex128)
     b = np.zeros(nstop - 1, dtype=np.complex128)
 
     psi_nm1 = np.sin(x)                   # nm1 = n-1 = 0
     psi_n = psi_nm1 / x - np.cos(x)       # n = 1
@@ -190,37 +188,39 @@
             xi_n = xi
             psi_nm1 = psi_n
             psi_n = xi_n.real
 
     return a, b
 
 
-def _small_conducting_mie(m, x):
+@njit((complex128, float64), cache=True)
+def _small_conducting_mie(_m, x):
     """
     Calculate the efficiencies for a small conducting spheres.
 
     Typically used for small conducting spheres where x < 0.1 and
     m.real == 0
 
     Args:
-        m: the complex index of refraction of the sphere
+        _m: the complex index of refraction of the sphere (unused)
         x: the size parameter of the sphere
 
     Returns:
         qext: the total extinction efficiency
         qsca: the scattering efficiency
         qback: the backscatter efficiency
         g: the average cosine of the scattering phase function
     """
-    ahat1 = complex(0, 2.0 / 3.0 * (1 - 0.2 * x**2)) / \
-        complex(1 - 0.5 * x**2, 2.0 / 3.0 * x**3)
-    bhat1 = complex(0.0, (x**2 - 10.0) / 30.0) / \
-        complex(1 + 0.5 * x**2, -x**3 / 3.0)
-    ahat2 = complex(0.0, x**2 / 30.)
-    bhat2 = complex(0.0, -x**2 / 45.)
+    ahat1 = complex(0, 2.0 / 3.0 * (1 - 0.2 * x**2))
+    ahat1 /= complex(1 - 0.5 * x**2, 2.0 / 3.0 * x**3)
+
+    bhat1 = complex(0.0, (x**2 - 10.0) / 30.0)
+    bhat1 /= complex(1 + 0.5 * x**2, -x**3 / 3.0)
+    ahat2 = complex(0.0, x**2 / 30.0)
+    bhat2 = complex(0.0, -x**2 / 45.0)
 
     qsca = x**4 * (6 * np.abs(ahat1)**2
                    + 6 * np.abs(bhat1)**2
                    + 10 * np.abs(ahat2)**2
                    + 10 * np.abs(bhat2)**2)
     qext = qsca
     g = ahat1.imag * (ahat2.imag + bhat1.imag)
@@ -229,14 +229,15 @@
     g *= 6 * x**4 / qsca
 
     qback = 9 * x**4 * np.abs(ahat1 - bhat1 - 5 / 3 * (ahat2 - bhat2))**2
 
     return [qext, qsca, qback, g]
 
 
+@njit((complex128, float64), cache=True)
 def _small_mie(m, x):
     """
     Calculate the efficiencies for a small sphere.
 
     Typically used for small spheres where x<0.1
 
     Args:
@@ -252,16 +253,18 @@
     m2 = m * m
     x2 = x * x
 
     D = m2 + 2 + (1 - 0.7 * m2) * x2
     D -= (8 * m**4 - 385 * m2 + 350) * x**4 / 1400.0
     D += 2j * (m2 - 1) * x**3 * (1 - 0.1 * x2) / 3
     ahat1 = 2j * (m2 - 1) / 3 * (1 - 0.1 * x2 + (4 * m2 + 5) * x**4 / 1400) / D
+
     bhat1 = 1j * x2 * (m2 - 1) / 45 * (1 + (2 * m2 - 5) / 70 * x2)
     bhat1 /= 1 - (2 * m2 - 5) / 30 * x2
+
     ahat2 = 1j * x2 * (m2 - 1) / 15 * (1 - x2 / 14)
     ahat2 /= 2 * m2 + 3 - (2 * m2 - 7) / 14 * x2
 
     T = np.abs(ahat1)**2 + np.abs(bhat1)**2 + 5 / 3 * np.abs(ahat2)**2
     temp = ahat2 + bhat1
     g = (ahat1 * temp.conjugate()).real / T
 
@@ -274,14 +277,15 @@
 
     sback = 1.5 * x**3 * (ahat1 - bhat1 - 5 * ahat2 / 3)
     qback = 4 * np.abs(sback)**2 / x2
 
     return [qext, qsca, qback, g]
 
 
+@njit((complex128, float64), cache=True)
 def _mie_scalar(m, x):
     """
     Calculate the efficiencies for a sphere when both m and x are scalars.
 
     Args:
         m: the complex index of refraction of the sphere
         x: the size parameter of the sphere
@@ -372,157 +376,126 @@
             xx = x[i]
 
         qext[i], qsca[i], qback[i], g[i] = _mie_scalar(mm, xx)
 
     return qext, qsca, qback, g
 
 
-def _small_mie_conducting_S1_S2(m, x, mu):
+@njit((complex128, float64, int32), cache=True)
+def normalization_factor(m, x, norm_int):
     """
-    Calculate the scattering amplitudes for small conducting spheres.
-
-    The spheres are small perfectly conducting (reflecting) spheres (x<0.1).
-    The amplitude functions have been normalized so that when integrated
-    over all 4𝜋 solid angles, the integral will be qext(𝜋x²).
-
-    The units are weird, sr**(-0.5)
+    Figure out scattering function normalization.
 
     Args:
         m: the complex index of refraction of the sphere
-        x: the size parameter of the sphere
-        mu: the angles, cos(theta), to calculate scattering amplitudes
+        x: dimensionless sphere size
+        norm_int: integer that specifies normalization
 
     Returns:
-        S1, S2: the scattering amplitudes at each angle mu [sr**(-0.5)]
-    """
-    ahat1 = 2j / 3 * (1 - 0.2 * x**2) / (1 - 0.5 * x**2 + 2j / 3 * x**3)
-    bhat1 = 1j / 3 * (0.1 * x**2 - 1) / (1 + 0.5 * x**2 - 1j / 3 * x**3)
-    ahat2 = 1j / 30 * x**2
-    bhat2 = -1j * x**2 / 45
-
-    S1 = 1.5 * x**3 * (ahat1 + bhat1 * mu
-                       + 5 / 3 * ahat2 * mu
-                       + 5 / 3 * bhat2 * (2 * mu**2 - 1))
-
-    S2 = 1.5 * x**3 * (bhat1 + ahat1 * mu
-                       + 5 / 3 * bhat2 * mu
-                       + 5 / 3 * ahat2 * (2 * mu**2 - 1))
-
-    qext = x**4 * (6 * np.abs(ahat1)**2
-                   + 6 * np.abs(bhat1)**2
-                   + 10 * np.abs(ahat2)**2
-                   + 10 * np.abs(bhat2)**2)
-
-    norm = np.sqrt(qext * np.pi * x**2)
-    S1 /= norm
-    S2 /= norm
-
-    return [S1, S2]
-
-
-def _small_mie_S1_S2(m, x, mu):
+        scaling factor needed for scattering function
     """
-    Calculate the scattering amplitude functions for small spheres (x<0.1).
+    norm = None
 
-    The amplitude functions have been normalized so that when integrated
-    over all 4*pi solid angles, the integral will be qext*pi*x**2.
-
-    The units are weird, sr**(-0.5)
-
-    Args:
-        m: the complex index of refraction of the sphere
-        x: the size parameter of the sphere
-        mu: the angles, cos(theta), to calculate scattering amplitudes
-
-    Returns:
-        S1, S2: the scattering amplitudes at each angle mu [sr**(-0.5)]
-    """
-    m2 = m * m
-    m4 = m2 * m2
-    x2 = x * x
-    x3 = x2 * x
-    x4 = x2 * x2
+    # Qsca normalization
+    if norm_int == 3:
+        norm = x * np.sqrt(np.pi)
+
+    # Bohren Normalization
+    elif norm_int == 5:
+        norm = 0.5
+
+    # Wiscombe Normalization
+    elif norm_int == 6:
+        norm = 1
 
-    D = m2 + 2 + (1 - 0.7 * m2) * x2
-    D -= (8 * m4 - 385 * m2 + 350) * x4 / 1400.0
-    D += 2j * (m2 - 1) * x3 * (1 - 0.1 * x2) / 3
+    else:
+        # calculate qsca and qext
+        qext, qsca, _, _ = _mie_scalar(m, x)
 
-    ahat1 = 2j * (m2 - 1) / 3 * (1 - 0.1 * x2 + (4 * m2 + 5) * x4 / 1400) / D
+        # albedo Normalization
+        if norm_int == 0:
+            norm = x * np.sqrt(np.pi * qext)
 
-    bhat1 = 1j * x2 * (m2 - 1) / 45 * (1 + (2 * m2 - 5) / 70 * x2)
-    bhat1 /= 1 - (2 * m2 - 5) / 30 * x2
+        # Unity normalization
+        elif norm_int == 1:
+            norm = x * np.sqrt(qsca * np.pi)
 
-    ahat2 = 1j * x2 * (m2 - 1) / 15 * (1 - x2 / 14)
-    ahat2 /= 2 * m2 + 3 - (2 * m2 - 7) / 14 * x2
+        # 4pi Normalization
+        elif norm_int == 2:
+            norm = x * np.sqrt(qsca / 4)
 
-    S1 = 1.5 * x3 * (ahat1 + bhat1 * mu + 5 / 3 * ahat2 * mu)
-    S2 = 1.5 * x3 * (bhat1 + ahat1 * mu + 5 / 3 * ahat2 * (2 * mu**2 - 1))
+        # Qext Normalization
+        elif norm_int == 4:  # 4pi
+            norm = x * np.sqrt(qsca * np.pi / qext)
 
-    # norm = sqrt(qext*pi*x**2)
-    norm = np.sqrt(np.pi * 6 * x**3 * (ahat1 + bhat1 + 5 * ahat2 / 3).real)
-    S1 /= norm
-    S2 /= norm
+    if norm is None:
+        raise ValueError("norm-int must be in the range 0..6")
 
-    return [S1, S2]
+    return norm
 
 
-def normalization_factor(m, x, norm_str):
+def norm_string_to_integer(s):
     """
-    Figure out scattering function normalization.
+    Encode normalization choice as an integer.
+
+    This is needed because these string operations cannot be
+    done in a jitted function under numba.  We cannot use enums for
+    the same reason!
 
     Args:
-        m: complex index of refraction of sphere
-        x: dimensionless sphere size
-        norm_str: string describing type of normalization
+        s: string describing normalization desired.
 
     Returns:
-        scaling factor needed for scattering function
+        integer used in _mie_S1_S2() determine normalization
     """
-    norm = norm_str.lower()
-
-    if norm in ['bohren']:
-        return 1 / 2
+    ii = None
+    norm = s.lower()
 
-    if norm in ['wiscombe']:
-        return 1
+    if norm in ['a', 'albedo']:
+        ii = 0
 
-    if norm in ['qsca', 'scattering_efficiency']:
-        return x * np.sqrt(np.pi)
+    elif norm in ['1', 'one', 'unity']:
+        ii = 1
 
-    qext, qsca, _, _ = _mie_scalar(m, x)
+    elif norm in ['four_pi', '4pi']:
+        ii = 2
 
-    if norm in ['a', 'albedo']:
-        return x * np.sqrt(np.pi * qext)
+    elif norm in ['qsca', 'scattering_efficiency']:
+        ii = 3
 
-    if norm in ['1', 'one', 'unity']:
-        return x * np.sqrt(qsca * np.pi)
+    elif norm in ['qext', 'extinction_efficiency']:
+        ii = 4
 
-    if norm in ['four_pi', '4pi']:
-        return x * np.sqrt(qsca / 4)
+    elif norm in ['bohren']:
+        ii = 5
 
-    if norm in ['qext', 'extinction_efficiency']:
-        return x * np.sqrt(qsca * np.pi / qext)
+    elif norm in ['wiscombe']:
+        ii = 6
 
-    raise ValueError("normalization must be one of 'albedo' (default), 'one'"
-                     "'4pi', 'qext', 'qsca', 'bohren', or 'wiscombe'")
+    if ii is None:
+        raise ValueError("normalization must be one of 'albedo' (default), 'one'"
+                         "'4pi', 'qext', 'qsca', 'bohren', or 'wiscombe'")
+    return ii
 
 
-def mie_S1_S2(m, x, mu, norm='albedo'):
+@njit((complex128, float64, float64[:], int32), cache=True)
+def _mie_S1_S2(m, x, mu, norm_int):
     """
     Calculate the scattering amplitude functions for spheres.
 
     The amplitude functions have been normalized so that when integrated
     over all 4*pi solid angles, the integral will be qext*pi*x**2.
 
     The units are weird, sr**(-0.5)
 
     Args:
         m: the complex index of refraction of the sphere
         x: the size parameter of the sphere
-        mu: the angles, cos(theta), to calculate scattering amplitudes
+        mu: array of angles, cos(theta), to calculate scattering amplitudes
+        norm_int: integer describing type of normalization
 
     Returns:
         S1, S2: the scattering amplitudes at each angle mu [sr**(-0.5)]
     """
     a, b = _mie_An_Bn(m, x)
 
     nangles = len(mu)
@@ -531,31 +504,57 @@
 
     nstop = len(a)
     for k in range(nangles):
         pi_nm2 = 0
         pi_nm1 = 1
         for n in range(1, nstop):
             tau_nm1 = n * mu[k] * pi_nm1 - (n + 1) * pi_nm2
-            S1[k] += (2 * n + 1) * (pi_nm1 * a[n - 1]
-                                    + tau_nm1 * b[n - 1]) / (n + 1) / n
-            S2[k] += (2 * n + 1) * (tau_nm1 * a[n - 1]
-                                    + pi_nm1 * b[n - 1]) / (n + 1) / n
-
+            S1[k] += (2 * n + 1) * (pi_nm1 * a[n - 1] + tau_nm1 * b[n - 1]) / (n + 1) / n
+            S2[k] += (2 * n + 1) * (tau_nm1 * a[n - 1] + pi_nm1 * b[n - 1]) / (n + 1) / n
             temp = pi_nm1
             pi_nm1 = ((2 * n + 1) * mu[k] * pi_nm1 - (n + 1) * pi_nm2) / n
             pi_nm2 = temp
 
-    normalization = normalization_factor(m, x, norm)
+    normalization = normalization_factor(m, x, norm_int)
 
     S1 /= normalization
     S2 /= normalization
 
     return [S1, S2]
 
 
+def mie_S1_S2(m, x, mu, norm='albedo'):
+    """
+    Calculate the scattering amplitude functions for spheres.
+
+    The normalization is controlled by `norm` and should be one of
+    ['albedo', 'one', '4pi', 'qext', 'qsca', 'bohren', or 'wiscombe']
+    The normalization describes the integral of the scattering phase
+    function over all 4𝜋 steradians.
+
+    The units are weird, sr**(-0.5)
+
+    Args:
+        m: the complex index of refraction of the sphere
+        x: the size parameter of the sphere
+        mu: cos(theta) or array of angles [cos(theta_i)]
+        norm: (optional) string describing scattering function normalization
+
+    Returns:
+        S1, S2: the scattering amplitudes at each angle mu [sr**(-0.5)]
+    """
+    norm_int = norm_string_to_integer(norm)
+    if np.isscalar(mu):
+        mu_array = np.array([mu], dtype=float)
+        s1, s2 = _mie_S1_S2(m, x, mu_array, norm_int)
+        return s1[0], s2[0]
+
+    return _mie_S1_S2(m, x, mu, norm_int)
+
+
 def mie_phase_matrix(m, x, mu, norm='albedo'):
     """
     Calculate the scattering (Mueller) matrix.
 
     If mu has length N, then the returned matrix is 4x4xN.  If mu is a scalar
     then the matrix is 4x4
 
@@ -564,25 +563,31 @@
     *An Introduction to Atmospheric Radiation*, Second Edition.
 
     or
 
     Bohren and Huffman, *Absorption and Scattering of Light by Small Particles*,
     JOHN WILEY & SONS, page 112, (1983).
 
+    The normalization is controlled by `norm` and should be one of
+    ['albedo', 'one', '4pi', 'qext', 'qsca', 'bohren', or 'wiscombe']
+    The normalization describes the integral of the scattering phase
+    function over all 4𝜋 steradians.
+
     Args:
         m: the complex index of refraction of the sphere
         x: the size parameter of the sphere
-        mu: the angles, cos(theta), of the phase scattering matrix
+        mu: the angles, cos(theta), for the phase scattering matrix
+        norm: (optional) string describing scattering function normalization
 
     Returns:
         p: the phase scattering matrix [sr**(-1.0)]
     """
-    mu = np.atleast_1d(mu)
     s1, s2 = mie_S1_S2(m=m, x=x, mu=mu, norm=norm)
 
+    mu = np.atleast_1d(mu)
     s1_star = np.conjugate(s1)
     s2_star = np.conjugate(s2)
     m1 = (s1 * s1_star).real
     m2 = (s2 * s2_star).real
     s21 = (0.5 * (s1 * s2_star + s2 * s1_star)).real
     d21 = (-0.5j * (s1 * s2_star - s2 * s1_star)).real
     phase = np.zeros(shape=(4, 4, mu.size))
@@ -594,15 +599,15 @@
     phase[2, 3] = -d21
     phase[3, 2] = d21
     phase[3, 3] = s21
 
     return phase.squeeze()
 
 
-def mie_cdf(m, x, num, norm='albedo'):
+def mie_cdf(m, x, num):
     """
     Create a CDF for unpolarized scattering uniformly spaced in cos(theta).
 
     The CDF covers scattered (exit) angles ranging from 180 to 0 degrees.
     (The cosines are uniformly distributed over -1 to 1.) Because the angles
     are uniformly distributed in cos(theta), the scattering function is not
     sampled uniformly and therefore huge array sizes are needed to adequately
@@ -617,29 +622,20 @@
         num: length of desired CDF array
 
     Returns:
         mu: array of cosines of angles
         cdf: array of cumulative distribution function values
     """
     mu = np.linspace(-1, 1, num)
-    s1, s2 = mie_S1_S2(m, x, mu, norm)
-
-    s = (np.abs(s1)**2 + np.abs(s2)**2) / 2
-
-    cdf = np.zeros(num)
-    total = 0
-    for i in range(num):
-        # need the extra 2pi because scattering normalized over 4π steradians
-        total += s[i] * 2 * np.pi * (2 / num)
-        cdf[i] = total
-
+    intensity_per_mu = i_unpolarized(m, x, mu, norm='4pi') / num
+    cdf = np.cumsum(intensity_per_mu)
     return mu, cdf
 
 
-def mie_mu_with_uniform_cdf(m, x, num, norm='albedo'):
+def mie_mu_with_uniform_cdf(m, x, num):
     """
     Create a CDF for unpolarized scattering for uniform CDF.
 
     The CDF covers scattered (exit) angles ranging from 180 to 0 degrees.
     (The cosines are uniformly distributed over -1 to 1.) These angles mu
     correspond to uniform spacing of the cumulative distribution function
     for unpolarized Mie scattering where cdf[i] = i/(num-1).
@@ -657,15 +653,15 @@
         num: length of desired CDF array
 
     Returns:
         mu: array of cosines of angles (irregularly spaced)
         cdf: array of cumulative distribution function values
     """
     big_num = 2000                  # large to work with x up to 10
-    big_mu, big_cdf = mie_cdf(m, x, big_num, norm)
+    big_mu, big_cdf = mie_cdf(m, x, big_num)
     mu = np.empty(num)
     cdf = np.empty(num)
 
     mu[0] = -1                       # cos[180 degrees] is -1
     cdf[0] = 0                       # initial cdf is zero
 
     big_k = 0                        # index into big_cdf
@@ -678,16 +674,16 @@
         delta = big_cdf[big_k] - target
         delta_cdf = big_cdf[big_k] - big_cdf[big_k - 1]
         delta_mu = big_mu[big_k] - big_mu[big_k - 1]
 
         mu[k] = big_mu[big_k] - delta / delta_cdf * delta_mu   # interpolate
         cdf[k] = target
 
-#       print(' mu[', k, ']=% .5f'%mu[k], ' cdf[', k, ']=% .5f'%cdf[k],
-#       'cdf=', big_cdf[big_k], fraction)
+#       print(' mu[',k,']=% .5f'%mu[k],' cdf[',k,']=% .5f'%cdf[k],
+#       'cdf=',big_cdf[big_k], fraction)
 
     mu[num - 1] = 1                    # cos[0 degrees] is 1
     cdf[num - 1] = 1                   # last cdf is one
 
     return [mu, cdf]
 
 
@@ -699,16 +695,16 @@
     New random angles are generated by selecting a random interval
     mu[i] to mu[i+1] and choosing an angle uniformly distributed over
     the interval.
 
     Args:
        mu_cdf: a cumulative distribution function
 
-    Returns
-       an array of random scattering angle cosines based on the CDF supplied.
+    Returns:
+       The cosine of the scattering angle
     """
     # the following should be equivalent to these four lines
     # index = np.random.randint(0, high=len(mu_cdf))
     num = len(mu_cdf) - 1
     index = int(np.random.random() * num)
     if index >= num:
         index = num - 1
@@ -724,21 +720,27 @@
     Return the scattered intensity in a plane normal to the incident light.
 
     This is the scattered intensity in a plane that is perpendicular to the
     field of the incident plane wave. The intensity is normalized such
     that the integral of the unpolarized intensity over 4π steradians
     is equal to the single scattering albedo.
 
+    The normalization is controlled by `norm` and should be one of
+    ['albedo', 'one', '4pi', 'qext', 'qsca', 'bohren', or 'wiscombe']
+    The normalization describes the integral of the scattering phase
+    function over all 4𝜋 steradians.
+
     Args:
-       m: the complex index of refraction of the sphere
-       x: the size parameter of the sphere
-       mu: the angles, cos(theta), to calculate intensities
+        m: the complex index of refraction of the sphere
+        x: the size parameter of the sphere
+        mu: the angles, cos(theta), to calculate intensities
+        norm: (optional) string describing scattering function normalization
 
-    Returns
-       The intensity at each angle in the array mu.  Units [1/sr]
+    Returns:
+        The intensity at each angle in the array mu.  Units [1/sr]
     """
     s1, _ = mie_S1_S2(m, x, mu, norm)
     intensity = np.abs(s1)**2
     return intensity.astype('float')
 
 
 def i_par(m, x, mu, norm='albedo'):
@@ -746,43 +748,54 @@
     Return the scattered intensity in a plane parallel to the incident light.
 
     This is the scattered intensity in a plane that is parallel to the
     field of the incident plane wave. The intensity is normalized such
     that the integral of the unpolarized intensity over 4π steradians
     is equal to the single scattering albedo.
 
+    The normalization is controlled by `norm` and should be one of
+    ['albedo', 'one', '4pi', 'qext', 'qsca', 'bohren', or 'wiscombe']
+    The normalization describes the integral of the scattering phase
+    function over all 4𝜋 steradians.
+
     Args:
-       m: the complex index of refraction of the sphere
-       x: the size parameter
-       mu: the cos(theta) of each direction desired
+        m: the complex index of refraction of the sphere
+        x: the size parameter of the sphere
+        mu: the angles, cos(theta), to calculate intensities
+        norm: (optional) string describing scattering function normalization
 
-    Returns
-       The intensity at each angle in the array mu.  Units [1/sr]
+    Returns:
+        The intensity at each angle in the array mu.  Units [1/sr]
     """
     _, s2 = mie_S1_S2(m, x, mu, norm)
     intensity = np.abs(s2)**2
     return intensity.astype('float')
 
 
 def i_unpolarized(m, x, mu, norm='albedo'):
     """
     Return the unpolarized scattered intensity at specified angles.
 
     This is the average value for randomly polarized incident light.
-    The intensity is normalized such
-    that the integral of the unpolarized intensity over 4π steradians
-    is equal to the single scattering albedo.
+    The intensity is normalized such that the integral of the unpolarized
+    intensity over 4π steradians is equal to the single scattering albedo.
+
+    The normalization is controlled by `norm` and should be one of
+    ['albedo', 'one', '4pi', 'qext', 'qsca', 'bohren', or 'wiscombe']
+    The normalization describes the integral of the scattering phase
+    function over all 4𝜋 steradians.
 
     Args:
-       m: the complex index of refraction of the sphere
-       x: the size parameter
-       mu: the cos(theta) of each direction desired
+        m: the complex index of refraction of the sphere
+        x: the size parameter of the sphere
+        mu: the angles, cos(theta), to calculate intensities
+        norm: (optional) string describing scattering function normalization
 
-    Returns
-       The intensity at each angle in the array mu.  Units [1/sr]
+    Returns:
+        The intensity at each angle in the array mu.  Units [1/sr]
     """
     s1, s2 = mie_S1_S2(m, x, mu, norm)
     intensity = (np.abs(s1)**2 + np.abs(s2)**2) / 2
     return intensity.astype('float')
 
 
 def ez_mie(m, d, lambda0, n_env=1.0):
@@ -792,18 +805,18 @@
     Args:
         m: the complex index of refraction of the sphere [-]
         d: the diameter of the sphere                    [same units as lambda0]
         lambda0: wavelength in a vacuum                  [same units as d]
         n_env: real index of medium around sphere, optional.
 
     Returns:
-        qext: the total extinction efficiency                  [-]
-        qsca: the scattering efficiency                        [-]
-        qback: the backscatter efficiency                      [-]
-        g: the average cosine of the scattering phase function [-]
+        qext: the total extinction efficiency                  [-].
+        qsca: the scattering efficiency                        [-].
+        qback: the backscatter efficiency                      [-].
+        g: the average cosine of the scattering phase function [-].
     """
     m_env = m / n_env
     x_env = np.pi * d / (lambda0 / n_env)
     return mie(m_env, x_env)
 
 
 def ez_intensities(m, d, lambda0, mu, n_env=1.0, norm='albedo'):
@@ -815,20 +828,26 @@
 
     The scattered intensity is normalized such that the integral of the
     unpolarized intensity over 4𝜋 steradians is equal to the single scattering
     albedo.  The scattered intensity has units of inverse steradians [1/sr].
 
     The unpolarized scattering is the average of the two scattered intensities.
 
+    The normalization is controlled by `norm` and should be one of
+    ['albedo', 'one', '4pi', 'qext', 'qsca', 'bohren', or 'wiscombe']
+    The normalization describes the integral of the scattering phase
+    function over all 4𝜋 steradians.
+
     Args:
         m: the complex index of refraction of the sphere [-]
         d: the diameter of the sphere                    [same units as lambda0]
         lambda0: wavelength in a vacuum                  [same units as d]
         mu: the cos(theta) of each direction desired     [-]
-        n_env: real index of medium around sphere, optional.
+        n_env: real index of medium around sphere, optional
+        norm: (optional) string describing scattering function normalization
 
     Returns:
         ipar, iper: scattered intensity in parallel and perpendicular planes [1/sr]
     """
     m_env = m / n_env
     lambda_env = lambda0 / n_env
     x_env = np.pi * d / lambda_env
```

### Comparing `miepython-2.5.3/miepython.egg-info/SOURCES.txt` & `miepython-2.5.4/miepython.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-.gitignore
 CHANGELOG.rst
 CITATION.cff
 LICENSE.txt
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
-.github/workflows/test.yml
 miepython/__init__.py
 miepython/miepython.py
 miepython/miepython_nojit.py
 miepython.egg-info/PKG-INFO
 miepython.egg-info/SOURCES.txt
 miepython.egg-info/dependency_links.txt
 miepython.egg-info/requires.txt
@@ -21,9 +19,8 @@
 miepython/data/Johnson.txt
 miepython/data/ag-Johnson.txt
 miepython/data/segelstein81_index.txt
 miepython/examples/01_dielectric.py
 miepython/examples/02_glass.py
 miepython/examples/03_droplets.py
 miepython/examples/04_gold.py
-tests/test_jit.py
-tests/test_nojit.py
+tests/test_mie.py
```

### Comparing `miepython-2.5.3/setup.cfg` & `miepython-2.5.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: MIT License
 	Intended Audience :: Science/Research
 	Programming Language :: Python
 	Topic :: Scientific/Engineering :: Physics
 	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 
 [options]
 packages = miepython
 install_requires = 
 	numpy
 	matplotlib
 	numba
@@ -38,21 +40,20 @@
 	data/*.txt
 
 [flake8]
 ignore = W503, D212, N802, N803, N806, E501
 per-file-ignores = 
 	__init__.py:F401,F403
 	setup.py:D100
-	tests/test_jit.py:D100,D101,D102
-	tests/test_nojit.py:D100,D101,D102
+	tests/test_mie.py:D100,D101,D102
 	tests/conftest.py:D100,D101,D102,D103
 exclude = 
 	.git,
 	__pycache__,
 	docs
-max-line-length = 99
+max-line-length = 110
 docstring-convention = google
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `miepython-2.5.3/setup.py` & `miepython-2.5.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Setup for module miepython."""
 import re
 import os.path
 from setuptools import setup
 
 project = 'miepython'
 
 
@@ -22,14 +23,15 @@
     with open(fn, 'r', encoding='utf-8') as f:
         contents = f.read()
     return contents
 
 
 setup(
     name=project,
+    python_requires='>=3.7',
     long_description=get_contents('README.rst'),
     long_description_content_type='text/x-rst',
     version=get_init_property('__version__'),
     author=get_init_property('__author__'),
     author_email=get_init_property('__email__'),
     license=get_init_property('__license__'),
     url=get_init_property('__url__')
```

### Comparing `miepython-2.5.3/tests/test_jit.py` & `miepython-2.5.4/tests/test_mie.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,367 +1,318 @@
 #! /usr/bin/env python3
-# pylint: disable=invalid-name
 # pylint: disable=unused-variable
-# pylint: disable=missing-function-docstring
-# pylint: disable=missing-class-docstring
-# pylint: disable=missing-module-docstring
-# pylint: disable=line-too-long
+# pylint: disable=too-many-public-methods
+# pylint: disable=protected-access
 
+"""
+Test cases for miepython.
+
+This tests both the jitted and non-jitted versions of the code.  The BaseTestMiePython
+class tests the jitted (normal version) and the
+"""
 import unittest
+import importlib
 import numpy as np
-import miepython
-
-# the low level tests use functions that should not be exported.  These work
-# but now that the higher level tests pass, these are skipped
 
-# class low_level(unittest.TestCase):
-#
-#     def test_01_log_derivatives(self):
-#         m = 1.0
-#         x = 1.0
-#         nstop = 10
-#         dn = miepython._D_calc(m, x, nstop)
-#         self.assertAlmostEqual(dn[9].real, 9.95228198, delta=0.00001)
-#
-#         x = 62
-#         m = 1.28 - 1.37j
-#         nstop = 50
-#         dn = _D_calc(m, x, nstop)
-#         self.assertAlmostEqual(dn[10].real, 0.004087, delta=0.00001)
-#         self.assertAlmostEqual(dn[10].imag, 1.0002620, delta=0.00001)
-#
-#     def test_02_an_bn(self):
-#         m = 4.0/3.0
-#         x = 50
-#         a, b = miepython.mie_An_Bn(m, x)
-# #        print(a)
-#     #        self.assertAlmostEqual(a[0].real, 0.5311058892948411929, delta=0.00000001)
-#     #        self.assertAlmostEqual(a[1].imag, -0.4990314856310943073, delta=0.00000001)
-#     #        self.assertAlmostEqual(b[1].real, 0.093412567968, delta=0.00001)
-#     #        self.assertAlmostEqual(b[1].imag, -0.067160541299, delta=0.00001)
-#
-#         m = 1.5-1.1j
-#         x = 2
-#         a, b = miepython.mie_An_Bn(m, x)
-#         self.assertAlmostEqual(a[0].real, 0.555091767665, delta=0.00001)
-#         self.assertAlmostEqual(a[0].imag, 0.158587776121, delta=0.00001)
-#         self.assertAlmostEqual(a[1].real, 0.386759705234, delta=0.00001)
-#         self.assertAlmostEqual(a[1].imag, 0.076275273072, delta=0.00001)
-#         self.assertAlmostEqual(b[1].real, 0.093412567968, delta=0.00001)
-#         self.assertAlmostEqual(b[1].imag, -0.067160541299, delta=0.00001)
-#
-#         m = 1.1-25j
-#         x = 2
-#         a, b = miepython.mie_An_Bn(m, x)
-#         self.assertAlmostEqual(a[1].real, 0.324433578437, delta=0.0001)
-#         self.assertAlmostEqual(a[1].imag, 0.465627763266, delta=0.0001)
-#         self.assertAlmostEqual(b[1].real, 0.060464399088, delta=0.0001)
-#         self.assertAlmostEqual(b[1].imag, -0.236805417045, delta=0.0001)
 
-
-class NonAbsorbing(unittest.TestCase):
+class BaseTestMiePython(unittest.TestCase):
+    """All tests for Mie."""
+    miepython = None  # This will be set by subclasses
+
+    @classmethod
+    def setUpClass(cls):
+        """This allows both jitted and non-jitted code to be used."""
+        if cls is BaseTestMiePython:
+            cls.miepython = importlib.import_module('miepython.miepython')
 
     def test_03_bh_dielectric(self):
+        """Bohren and Huffman test."""
         m = 1.55
         lambda0 = 0.6328
         radius = 0.525
         x = 2 * np.pi * radius / lambda0
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
 
         self.assertAlmostEqual(qext, 3.10543, delta=0.00001)
         self.assertAlmostEqual(qsca, 3.10543, delta=0.00001)
         self.assertAlmostEqual(qback, 2.92534, delta=0.00001)
         self.assertAlmostEqual(g, 0.63314, delta=0.00001)
 
-    def test_05_wiscombe_non_absorbing(self):
+    def test_05_old_wiscombe_non_absorbing(self):
+        """Wiscombe old MIEV0 cases 1-4."""
+        m = complex(1.5, 0.0)
+        x = 10
+        s1 = 4.322E+00 + 4.868E+00 * 1j
+        G = abs(2 * s1 / x)**2
+        qext, qsca, qback, g = self.miepython.mie(m, x)
+        self.assertAlmostEqual(qsca, 2.8820, delta=1e-4)
+        self.assertAlmostEqual(qback, G, delta=1e-4)
+
+        # OLD MIEV0 Test Case 2
+        m = complex(1.5, 0.0)
+        x = 100
+        s1 = 4.077E+01 + 5.175E+01 * 1j
+        G = abs(2 * s1 / x)**2
+        qext, qsca, qback, g = self.miepython.mie(m, x)
+        self.assertAlmostEqual(qsca, 2.0944, delta=1e-4)
+        self.assertAlmostEqual(qback, G, delta=1e-4)
+
+        # OLD MIEV0 Test Case 3
+        m = complex(1.5, 0.0)
+        x = 1000
+        G = 4 * 2.576E+06 / x**2
+        qext, qsca, qback, g = self.miepython.mie(m, x)
+        self.assertAlmostEqual(qsca, 2.0139, delta=1e-4)
+        self.assertAlmostEqual(qback, G, delta=1e-3)
+
+        # OLD MIEV0 Test Case 4
+        m = complex(1.5, 0.0)
+        x = 5000.0
+        G = 4 * 2.378E+08 / x**2
+        qext, qsca, qback, g = self.miepython.mie(m, x)
+        self.assertAlmostEqual(qsca, 2.0086, delta=1e-4)
+        self.assertAlmostEqual(qback, G, delta=3e-3)
 
-        # MIEV0 Test Case 5
+    def test_05_wiscombe_non_absorbing(self):
+        """Wiscombe test cases 5-8."""
         m = complex(0.75, 0.0)
         x = 0.099
         s1 = 1.81756e-8 - 1.64810e-4 * 1j
         G = abs(2 * s1 / x)**2
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 0.000007, delta=1e-6)
         self.assertAlmostEqual(g, 0.001448, delta=1e-6)
         self.assertAlmostEqual(qback, G, delta=1e-6)
 
         # MIEV0 Test Case 6
         m = complex(0.75, 0.0)
         x = 0.101
         s1 = 2.04875E-08 - 1.74965E-04 * 1j
         G = abs(2 * s1 / x)**2
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 0.000008, delta=1e-6)
         self.assertAlmostEqual(g, 0.001507, delta=1e-6)
         self.assertAlmostEqual(qback, G, delta=1e-6)
 
         # MIEV0 Test Case 7
         m = complex(0.75, 0.0)
         x = 10.0
         s1 = -1.07857E+00 - 3.60881E-02 * 1j
         G = abs(2 * s1 / x)**2
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 2.232265, delta=1e-6)
         self.assertAlmostEqual(g, 0.896473, delta=1e-6)
         self.assertAlmostEqual(qback, G, delta=1e-6)
 
         # MIEV0 Test Case 8
         m = complex(0.75, 0.0)
         x = 1000.0
         s1 = 1.70578E+01 + 4.84251E+02 * 1j
         G = abs(2 * s1 / x)**2
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 1.997908, delta=1e-6)
         self.assertAlmostEqual(g, 0.844944, delta=1e-6)
         self.assertAlmostEqual(qback, G, delta=1e-6)
 
-    def test_05_old_wiscombe_non_absorbing(self):
-
-        # OLD MIEV0 Test Case 1
-        m = complex(1.5, 0.0)
-        x = 10
-        s1 = 4.322E+00 + 4.868E+00 * 1j
-        G = abs(2 * s1 / x)**2
-        qext, qsca, qback, g = miepython.mie(m, x)
-        self.assertAlmostEqual(qsca, 2.8820, delta=1e-4)
-        self.assertAlmostEqual(qback, G, delta=1e-4)
-
-        # OLD MIEV0 Test Case 2
-        m = complex(1.5, 0.0)
-        x = 100
-        s1 = 4.077E+01 + 5.175E+01 * 1j
-        G = abs(2 * s1 / x)**2
-        qext, qsca, qback, g = miepython.mie(m, x)
-        self.assertAlmostEqual(qsca, 2.0944, delta=1e-4)
-        self.assertAlmostEqual(qback, G, delta=1e-4)
-
-        # OLD MIEV0 Test Case 3
-        m = complex(1.5, 0.0)
-        x = 1000
-        G = 4 * 2.576E+06 / x**2
-        qext, qsca, qback, g = miepython.mie(m, x)
-        self.assertAlmostEqual(qsca, 2.0139, delta=1e-4)
-        self.assertAlmostEqual(qback, G, delta=1e-3)
-
-        # OLD MIEV0 Test Case 4
-        m = complex(1.5, 0.0)
-        x = 5000.0
-        G = 4 * 2.378E+08 / x**2
-        qext, qsca, qback, g = miepython.mie(m, x)
-        self.assertAlmostEqual(qsca, 2.0086, delta=1e-4)
-        self.assertAlmostEqual(qback, G, delta=3e-3)
-
-    def test_04_non_dielectric(self):
-        m = 1.55 - 0.1j
-        lambda0 = 0.6328
-        radius = 0.525
-        x = 2 * np.pi * radius / lambda0
-        qext, qsca, qback, g = miepython.mie(m, x)
-
-        self.assertAlmostEqual(qext, 2.86165188243, delta=1e-7)
-        self.assertAlmostEqual(qsca, 1.66424911991, delta=1e-7)
-        self.assertAlmostEqual(qback, 0.20599534080, delta=1e-7)
-        self.assertAlmostEqual(g, 0.80128972639, delta=1e-7)
-
-
-class Absorbing(unittest.TestCase):
     def test_06_wiscombe_water_absorbing(self):
-
-        # MIEV0 Test Case 9
+        """Wiscombe tests 9 - 11."""
         m = complex(1.33, -0.00001)
         x = 1.0
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 0.093923, delta=1e-6)
         self.assertAlmostEqual(g, 0.184517, delta=1e-6)
 
         # MIEV0 Test Case 10
         m = complex(1.33, -0.00001)
         x = 100.0
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 2.096594, delta=1e-6)
         self.assertAlmostEqual(g, 0.868959, delta=1e-6)
 
         # MIEV0 Test Case 11
         m = complex(1.33, -0.00001)
         x = 10000.0
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(g, 0.907840, delta=1e-6)
         self.assertAlmostEqual(qsca, 1.723857, delta=1e-6)
 
     def test_07_wiscombe_absorbing(self):
-
-        # MIEV0 Test Case 12
+        """Wiscombe tests 12-15."""
         m = 1.5 - 1j
         x = 0.055
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 0.000011, delta=1e-6)
         self.assertAlmostEqual(g, 0.000491, delta=1e-6)
 
         # MIEV0 Test Case 13
         m = 1.5 - 1j
         x = 0.056
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 0.000012, delta=1e-6)
         self.assertAlmostEqual(g, 0.000509, delta=1e-6)
 
         # MIEV0 Test Case 14
         m = 1.5 - 1j
         x = 1
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 0.6634538, delta=1e-6)
         self.assertAlmostEqual(g, 0.192136, delta=1e-6)
 
         # MIEV0 Test Case 15
         m = 1.5 - 1j
         x = 100
         x = 100.0
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 1.283697, delta=1e-3)
         self.assertAlmostEqual(qext, 2.097502, delta=1e-2)
         self.assertAlmostEqual(g, 0.850252, delta=1e-3)
 
         # MIEV0 Test Case 16
         m = 1.5 - 1j
         x = 10000
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 1.236575, delta=1e-6)
         self.assertAlmostEqual(qext, 2.004368, delta=1e-6)
         self.assertAlmostEqual(g, 0.846309, delta=1e-6)
 
     def test_08_wiscombe_more_absorbing(self):
-
-        # MIEV0 Test Case 17
+        """Wiscombe tests 17-19."""
         m = 10.0 - 10.0j
         x = 1.0
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 2.049405, delta=1e-6)
         self.assertAlmostEqual(g, -0.110664, delta=1e-6)
 
         # MIEV0 Test Case 18
         m = 10.0 - 10.0j
         x = 100.0
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 1.836785, delta=1e-6)
         self.assertAlmostEqual(g, 0.556215, delta=1e-6)
 
         # MIEV0 Test Case 19
         m = 10.0 - 10.0j
         x = 10000.0
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 1.795393, delta=1e-6)
         self.assertAlmostEqual(g, 0.548194, delta=1e-6)
 
     def test_09_single_nonmagnetic(self):
+        """Single non-magnetic sphere."""
         m = 1.5 - 0.5j
         x = 2.5
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
 
         self.assertAlmostEqual(qext, 2.562873497454734, delta=1e-7)
         self.assertAlmostEqual(qsca, 1.097071819088392, delta=1e-7)
         self.assertAlmostEqual(qback, 0.123586468179818, delta=1e-7)
         self.assertAlmostEqual(g, 0.748905978948507, delta=1e-7)
 
+    def test_04_non_dielectric(self):
+        """Another absorbing test case."""
+        m = 1.55 - 0.1j
+        lambda0 = 0.6328
+        radius = 0.525
+        x = 2 * np.pi * radius / lambda0
+        qext, qsca, qback, g = self.miepython.mie(m, x)
 
-class PerfectlyReflecting(unittest.TestCase):
+        self.assertAlmostEqual(qext, 2.86165188243, delta=1e-7)
+        self.assertAlmostEqual(qsca, 1.66424911991, delta=1e-7)
+        self.assertAlmostEqual(qback, 0.20599534080, delta=1e-7)
+        self.assertAlmostEqual(g, 0.80128972639, delta=1e-7)
 
     def test_11_wiscombe_perfectly_reflecting(self):
-
-        # MIEV0 Test Case 0
+        """Wiscombe MIEV0 tests 0-4."""
         m = 0
         x = 0.001
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 3.3333E-12, delta=1e-13)
 
         # MIEV0 Test Case 1
         m = 0
         x = 0.099
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 0.000321, delta=1e-4)
         self.assertAlmostEqual(g, -0.397357, delta=1e-3)
 
         # MIEV0 Test Case 2
         m = 0
         x = 0.101
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 0.000348, delta=1e-6)
         self.assertAlmostEqual(g, -0.397262, delta=1e-6)
 
         # MIEV0 Test Case 3
         m = 0
         x = 100
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 2.008102, delta=1e-6)
         self.assertAlmostEqual(g, 0.500926, delta=1e-6)
 
         # MIEV0 Test Case 4
         m = 0
         x = 10000
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qsca, 2.000289, delta=1e-6)
         self.assertAlmostEqual(g, 0.500070, delta=1e-6)
 
-
-class Small(unittest.TestCase):
-
     def test_10_small_spheres(self):
-        # MIEV0 Test Case 5
+        """Wiscombe MIEV0 tests 5-6 and others."""
         m = 0.75
         x = 0.099
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qext, 0.000007, delta=1e-6)
         self.assertAlmostEqual(g, 0.001448, delta=1e-6)
 
         # MIEV0 Test Case 6
         m = 0.75
         x = 0.101
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qext, 0.000008, delta=1e-6)
         self.assertAlmostEqual(g, 0.001507, delta=1e-6)
 
         m = 1.5 - 1j
         x = 0.055
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qext, 0.101491, delta=1e-6)
         self.assertAlmostEqual(g, 0.000491, delta=1e-6)
         x = 0.056
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qext, 0.103347, delta=1e-6)
         self.assertAlmostEqual(g, 0.000509, delta=1e-6)
 
         m = 1e-10 - 1e10j
         x = 0.099
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qext, 0.000321, delta=1e-6)
         self.assertAlmostEqual(g, -0.397357, delta=1e-4)
         x = 0.101
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qext, 0.000348, delta=1e-6)
         self.assertAlmostEqual(g, -0.397262, delta=1e-6)
 
         m = 0 - 1e10j
         x = 0.099
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qext, 0.000321, delta=1e-6)
         self.assertAlmostEqual(g, -0.397357, delta=1e-4)
         x = 0.101
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
         self.assertAlmostEqual(qext, 0.000348, delta=1e-6)
         self.assertAlmostEqual(g, -0.397262, delta=1e-4)
 
-
-class AngleScattering(unittest.TestCase):
-
     def test_12_scatter_function(self):
+        """Absorbing sphere."""
         x = 1.0
         m = 1.5 - 1.0j
         theta = np.arange(0, 181, 30)
         mu = np.cos(theta * np.pi / 180)
 
-        qext, qsca, qback, g = miepython.mie(m, x)
-        S1, S2 = miepython.mie_S1_S2(m, x, mu)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
+        S1, S2 = self.miepython.mie_S1_S2(m, x, mu)
         S1 *= np.sqrt(np.pi * x**2 * qext)
         S2 *= np.sqrt(np.pi * x**2 * qext)
 
         self.assertAlmostEqual(S1[0].real, 0.584080, delta=1e-6)
         self.assertAlmostEqual(S1[0].imag, 0.190515, delta=1e-6)
         self.assertAlmostEqual(S2[0].real, 0.584080, delta=1e-6)
         self.assertAlmostEqual(S2[0].imag, 0.190515, delta=1e-6)
@@ -393,21 +344,22 @@
 
         self.assertAlmostEqual(S1[6].real, 0.348844, delta=1e-6)
         self.assertAlmostEqual(S1[6].imag, 0.146829, delta=1e-6)
         self.assertAlmostEqual(S2[6].real, -0.348844, delta=1e-6)
         self.assertAlmostEqual(S2[6].imag, -0.146829, delta=1e-6)
 
     def test_13_unity_normalization(self):
+        """Test unity normalization."""
         x = 1.0
         m = 1.5 - 1.0j
         theta = np.arange(0, 181, 30)
         mu = np.cos(theta * np.pi / 180)
 
-        qext, qsca, qback, g = miepython.mie(m, x)
-        S1, S2 = miepython.mie_S1_S2(m, x, mu, norm='wiscombe')
+        qext, qsca, qback, g = self.miepython.mie(m, x)
+        S1, S2 = self.miepython.mie_S1_S2(m, x, mu, norm='wiscombe')
 
         self.assertAlmostEqual(S1[0].real, 0.584080, delta=1e-6)
         self.assertAlmostEqual(S1[0].imag, 0.190515, delta=1e-6)
         self.assertAlmostEqual(S2[0].real, 0.584080, delta=1e-6)
         self.assertAlmostEqual(S2[0].imag, 0.190515, delta=1e-6)
 
         self.assertAlmostEqual(S1[1].real, 0.565702, delta=1e-6)
@@ -437,90 +389,121 @@
 
         self.assertAlmostEqual(S1[6].real, 0.348844, delta=1e-6)
         self.assertAlmostEqual(S1[6].imag, 0.146829, delta=1e-6)
         self.assertAlmostEqual(S2[6].real, -0.348844, delta=1e-6)
         self.assertAlmostEqual(S2[6].imag, -0.146829, delta=1e-6)
 
     def test_i_unpolarized_01(self):
+        """Test normalization of unpolarized light."""
         m = 1.5 - 1.5j
         x = 2
         mu = np.linspace(-1, 1, 1000)
-        qext, qsca, _, _ = miepython.mie(m, x)
+        qext, qsca, _, _ = self.miepython.mie(m, x)
         expected = [qsca / qext, 1.0, 4 * np.pi, qsca, qext, qsca * 4 * np.pi * x**2, qsca * np.pi * x**2]
 
         for i, norm in enumerate(['albedo', 'one', '4pi', 'qsca', 'qext', 'bohren', 'wiscombe']):
-            intensity = miepython.i_unpolarized(m, x, mu, norm)
+            intensity = self.miepython.i_unpolarized(m, x, mu, norm)
             total = 2 * np.pi * (mu[1] - mu[0]) * np.sum(intensity)
             self.assertAlmostEqual(total / expected[i], 1.0, delta=4e-3)
 
     def test_i_par_i_per_01(self):
+        """Test normalization of i_par and i_per."""
         m = 1.5 - 1.5j
         x = 2
         mu = np.linspace(-1, 1, 10000)
-        qext, qsca, _, _ = miepython.mie(m, x)
+        qext, qsca, _, _ = self.miepython.mie(m, x)
+        expected = [qsca / qext, 1.0, 4 * np.pi, qsca, qext, qsca * 4 * np.pi * x**2, qsca * np.pi * x**2]
+
+        for i, norm in enumerate(['albedo', 'one', '4pi', 'qsca', 'qext', 'bohren', 'wiscombe']):
+            iper = self.miepython.i_per(m, x, mu, norm)
+            total1 = 2 * np.pi * (mu[1] - mu[0]) * np.sum(iper)
+            ipar = self.miepython.i_par(m, x, mu, norm)
+            total2 = 2 * np.pi * (mu[1] - mu[0]) * np.sum(ipar)
+            total = (total1 + total2) / 2
+            self.assertAlmostEqual(total / expected[i], 1, delta=1e-3)
+
+    def test_i_par_i_per_02(self):
+        """Test normalization of i_par and i_per for small spheres."""
+        m = 1.5 - 0j
+        x = 0.05
+        mu = np.linspace(-1, 1, 10000)
+        qext, qsca, _, _ = self.miepython.mie(m, x)
+        expected = [qsca / qext, 1.0, 4 * np.pi, qsca, qext, qsca * 4 * np.pi * x**2, qsca * np.pi * x**2]
+
+        for i, norm in enumerate(['albedo', 'one', '4pi', 'qsca', 'qext', 'bohren', 'wiscombe']):
+            iper = self.miepython.i_per(m, x, mu, norm)
+            total1 = 2 * np.pi * (mu[1] - mu[0]) * np.sum(iper)
+            ipar = self.miepython.i_par(m, x, mu, norm)
+            total2 = 2 * np.pi * (mu[1] - mu[0]) * np.sum(ipar)
+            total = (total1 + total2) / 2
+            self.assertAlmostEqual(total / expected[i], 1, delta=1e-3)
+
+    def test_i_par_i_per_03(self):
+        """Test normalization of i_par and i_per for small conducting spheres."""
+        m = 0 - 10j
+        x = 0.05
+        mu = np.linspace(-1, 1, 10000)
+        qext, qsca, _, _ = self.miepython.mie(m, x)
         expected = [qsca / qext, 1.0, 4 * np.pi, qsca, qext, qsca * 4 * np.pi * x**2, qsca * np.pi * x**2]
 
         for i, norm in enumerate(['albedo', 'one', '4pi', 'qsca', 'qext', 'bohren', 'wiscombe']):
-            iper = miepython.i_per(m, x, mu, norm)
+            iper = self.miepython.i_per(m, x, mu, norm)
             total1 = 2 * np.pi * (mu[1] - mu[0]) * np.sum(iper)
-            ipar = miepython.i_par(m, x, mu, norm)
+            ipar = self.miepython.i_par(m, x, mu, norm)
             total2 = 2 * np.pi * (mu[1] - mu[0]) * np.sum(ipar)
             total = (total1 + total2) / 2
             self.assertAlmostEqual(total / expected[i], 1, delta=1e-3)
 
     def test_molecular_hydrogen(self):
+        """Test very small spheres."""
         m = 1.00013626
         x = 0.0006403246172921872
         mu = np.linspace(-1, 1, 100)
-        ph = miepython.i_unpolarized(m, x, mu)
+        ph = self.miepython.i_unpolarized(m, x, mu)
         self.assertAlmostEqual(ph[1], 0.1169791, delta=1e-5)
 
-
-class MiePhaseMatrix(unittest.TestCase):
     def test_mie_phase_matrix_basic(self):
-        """Element (0, 0) of array returned by mie_phase_matrix should match output
-        of i_unpolarized."""
+        """Element (0, 0) of mie_phase_matrix should match i_unpolarized."""
         m = 1.5 - 1.5j
         x = 2
         mu = np.linspace(-1, 1, 1000)
 
-        p = miepython.mie_phase_matrix(m, x, mu)  # result to be validated
-        p00 = miepython.i_unpolarized(m, x, mu)  # reference result
+        p = self.miepython.mie_phase_matrix(m, x, mu)  # result to be validated
+        p00 = self.miepython.i_unpolarized(m, x, mu)  # reference result
 
         assert np.allclose(p[0, 0], p00, rtol=1e-9)
 
     def test_mie_phase_matrix_mu_scalar(self):
         """mie_phase_matrix returns (4, 4) array when mu is scalar."""
-        assert miepython.mie_phase_matrix(m=1.5, x=2.0, mu=0.0).shape == (4, 4)
+        assert self.miepython.mie_phase_matrix(m=1.5, x=2.0, mu=0.0).shape == (4, 4)
 
     def test_mie_phase_matrix_symmetry(self):
-        """Upper left 2X2 block is symmetric and lower right 2X2 block is
-        antisymmetric."""
-        p = miepython.mie_phase_matrix(m=1.5, x=2.0, mu=np.linspace(-1, 1, 10))
+        """Upper left 2X2 block is symmetric and lower right 2X2 block is antisymmetric."""
+        p = self.miepython.mie_phase_matrix(m=1.5, x=2.0, mu=np.linspace(-1, 1, 10))
         assert np.allclose(p[0, 1], p[1, 0])
         assert np.allclose(p[2, 3], -p[3, 2])
 
     def test_mie_phase_matrix_unity(self):
-        """Element p[0, 0, :]**2 = sum of squares of other three"""
+        """Element p[0, 0, :]**2 = sum of squares of other three."""
         m = 1.5 - 1.5j
         x = 2
         mu = np.linspace(-1, 1, 1000)
 
-        p = miepython.mie_phase_matrix(m, x, mu)  # result to be validated
+        p = self.miepython.mie_phase_matrix(m, x, mu)  # result to be validated
 
         assert np.allclose(p[0, 0]**2, p[0, 1]**2 + p[2, 2]**2 + p[2, 3]**2, rtol=1e-9)
 
     def test_mie_phase_matrix_bohren(self):
-        """Compare with output from Bohren's program
+        """
+        Compare with output from Bohren's program.
 
         s33 and s34 elements are normalized by s11
         s11 is normalized to 1 in the forward direction
         pol is -s12 normalized by s11
         """
-
         mm = np.array([[000.00, 0.100000E+01, 0.000000E+00, 0.100000E+01, 0.000000E+00],
                        [009.00, 0.785390E+00, -0.459811E-02, 0.999400E+00, 0.343261E-01],
                        [018.00, 0.356897E+00, -0.458541E-01, 0.986022E+00, 0.160184E+00],
                        [027.00, 0.766119E-01, -0.364744E+00, 0.843603E+00, 0.394076E+00],
                        [036.00, 0.355355E-01, -0.534997E+00, 0.686967E+00, -0.491787E+00],
                        [045.00, 0.701845E-01, 0.959953E-02, 0.959825E+00, -0.280434E+00],
                        [054.00, 0.574313E-01, 0.477927E-01, 0.985371E+00, 0.163584E+00],
@@ -541,49 +524,49 @@
                        ])
 
         m = 1.55
         x = 5.213
         theta = np.linspace(0, 180, 21)
 
         mu = np.cos(np.radians(theta))
-        p = miepython.mie_phase_matrix(m, x, mu, norm='bohren')  # result to be validated
+        p = self.miepython.mie_phase_matrix(m, x, mu, norm='bohren')  # result to be validated
 
         assert np.allclose(theta, mm[:, 0], rtol=1e-9)
         assert np.allclose(p[0, 0, :] / p[0, 0, 0], mm[:, 1], atol=1e-3)
         assert np.allclose(-p[0, 1, :] / p[0, 0, :], mm[:, 2], atol=1e-3)
         assert np.allclose(p[2, 2, :] / p[0, 0, :], mm[:, 3], atol=1e-3)
         assert np.allclose(p[3, 2, :] / p[0, 0, :], mm[:, 4], atol=1e-3)
 
-
-class NotebookTests(unittest.TestCase):
     def test_nb1_x(self):
+        """First test."""
         N = 500
         m = 1.5
         x = np.linspace(0.1, 20, N)  # also in microns
-        qext, qsca, qback, g = miepython.mie(m, x)
+        qext, qsca, qback, g = self.miepython.mie(m, x)
 
         self.assertAlmostEqual(qsca[0], 2.3084093592198083e-05, delta=1e-6)
         self.assertAlmostEqual(qsca[100], 4.105960809066763, delta=1e-6)
         self.assertAlmostEqual(qsca[200], 1.9947867190110644, delta=1e-6)
         self.assertAlmostEqual(qsca[300], 2.4652591512196405, delta=1e-6)
         self.assertAlmostEqual(qsca[400], 2.472171798724846, delta=1e-6)
         self.assertAlmostEqual(qsca[499], 2.03583698038088, delta=1e-6)
 
     def test_nb1_rho(self):
+        """Second test."""
         N = 500
         m = 1.5
         rho = np.linspace(0.1, 20, N)
 
         m = 1.5
         x15 = rho / 2 / (m - 1)
-        qext, scal5, qback, g = miepython.mie(m, x15)
+        qext, scal5, qback, g = self.miepython.mie(m, x15)
 
         m = 1.1
         x11 = rho / 2 / (m - 1)
-        qext, scal1, qback, g = miepython.mie(m, x11)
+        qext, scal1, qback, g = self.miepython.mie(m, x11)
 
         self.assertAlmostEqual(scal1[0], 0.0006616369953521216, delta=1e-6)
         self.assertAlmostEqual(scal1[99], 3.449616595439377, delta=1e-6)
         self.assertAlmostEqual(scal1[199], 1.6837703285684387, delta=1e-6)
         self.assertAlmostEqual(scal1[299], 2.3167184401740495, delta=1e-6)
         self.assertAlmostEqual(scal1[399], 2.218210809017406, delta=1e-6)
         self.assertAlmostEqual(scal1[499], 1.876467571615533, delta=1e-6)
@@ -592,41 +575,80 @@
         self.assertAlmostEqual(scal5[99], 4.07295075914037, delta=1e-6)
         self.assertAlmostEqual(scal5[199], 1.8857586341949146, delta=1e-6)
         self.assertAlmostEqual(scal5[299], 2.464763930426085, delta=1e-6)
         self.assertAlmostEqual(scal5[399], 2.430569030744473, delta=1e-6)
         self.assertAlmostEqual(scal5[499], 2.03583698038088, delta=1e-6)
 
     def test_nb1_spheres(self):
+        """Third test."""
         N = 500
         m = 1.0
         r = 500                            # nm
         lambda0 = np.linspace(300, 800, N)  # also in nm
 
         mwater = 4 / 3   # rough approximation
         mm = m / mwater
         xx = 2 * np.pi * r * mwater / lambda0
-        qext, qsca, qback, g = miepython.mie(mm, xx)
+        qext, qsca, qback, g = self.miepython.mie(mm, xx)
 
         self.assertAlmostEqual(qsca[0], 1.5525047718022498, delta=1e-6)
         self.assertAlmostEqual(qsca[99], 2.1459528526672678, delta=1e-6)
         self.assertAlmostEqual(qsca[199], 2.365171370327149, delta=1e-6)
         self.assertAlmostEqual(qsca[299], 2.2039860928542128, delta=1e-6)
         self.assertAlmostEqual(qsca[399], 1.9261758931397088, delta=1e-6)
         self.assertAlmostEqual(qsca[499], 1.640006561518987, delta=1e-6)
 
     def test_nb1_ezmie(self):
+        """Fourth test."""
         m_sphere = 1.0
         n_water = 4 / 3
         d = 1000
         lambda0 = np.linspace(300, 800)
-        qext, qsca, qback, g = miepython.ez_mie(m_sphere, d, lambda0, n_water)
+        qext, qsca, qback, g = self.miepython.ez_mie(m_sphere, d, lambda0, n_water)
 
         self.assertAlmostEqual(qsca[0], 1.5525047718022498, delta=1e-6)
         self.assertAlmostEqual(qsca[9], 2.107970892634116, delta=1e-6)
         self.assertAlmostEqual(qsca[19], 2.3654333205160074, delta=1e-6)
         self.assertAlmostEqual(qsca[29], 2.213262310704816, delta=1e-6)
         self.assertAlmostEqual(qsca[39], 1.9314911518355427, delta=1e-6)
         self.assertAlmostEqual(qsca[49], 1.640006561518987, delta=1e-6)
 
+    def test_02_an_bn(self):
+        """Test An and Bn."""
+        m = 1.5-1.1j
+        x = 2
+        a, b = self.miepython._mie_An_Bn(m, x)
+        self.assertAlmostEqual(a[0].real, 0.555091767665, delta=0.00001)
+        self.assertAlmostEqual(a[0].imag, 0.158587776121, delta=0.00001)
+        self.assertAlmostEqual(a[1].real, 0.386759705234, delta=0.00001)
+        self.assertAlmostEqual(a[1].imag, 0.076275273072, delta=0.00001)
+        self.assertAlmostEqual(b[1].real, 0.093412567968, delta=0.00001)
+        self.assertAlmostEqual(b[1].imag, -0.067160541299, delta=0.00001)
+
+        m = 1.1-25j
+        x = 2
+        a, b = self.miepython._mie_An_Bn(m, x)
+        self.assertAlmostEqual(a[1].real, 0.324433578437, delta=0.0001)
+        self.assertAlmostEqual(a[1].imag, 0.465627763266, delta=0.0001)
+        self.assertAlmostEqual(b[1].real, 0.060464399088, delta=0.0001)
+        self.assertAlmostEqual(b[1].imag, -0.236805417045, delta=0.0001)
+
+    def test_01_log_derivatives(self):
+        """Test log derivative calculation."""
+        x = 62
+        m = 1.28 - 1.37j
+        nstop = 50
+        dn = self.miepython._D_calc(m, x, nstop)
+        self.assertAlmostEqual(dn[10].real, 0.004087, delta=0.00001)
+        self.assertAlmostEqual(dn[10].imag, 1.0002620, delta=0.00001)
+
+
+class TestWithoutJIT(BaseTestMiePython):
+    """Test non-jitted code."""
+    @classmethod
+    def setUpClass(cls):
+        """Import miepython.miepython_nojit as miepython."""
+        cls.miepython = importlib.import_module('miepython.miepython_nojit')
+
 
 if __name__ == '__main__':
     unittest.main()
```

