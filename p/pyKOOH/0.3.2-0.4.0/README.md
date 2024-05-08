# Comparing `tmp/pykooh-0.3.2.tar.gz` & `tmp/pykooh-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykooh-0.3.2.tar", last modified: Sat Sep  4 04:58:04 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pykooh-0.3.2.tar` & `pykooh-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-04 04:58:04.571072 pykooh-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (121)      615 2021-09-04 04:57:51.000000 pykooh-0.3.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-09-04 04:57:51.000000 pykooh-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      172 2021-09-04 04:57:51.000000 pykooh-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4470 2021-09-04 04:58:04.571072 pykooh-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2553 2021-09-04 04:57:51.000000 pykooh-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-04 04:58:04.567072 pykooh-0.3.2/pykooh/
--rw-r--r--   0 runner    (1001) docker     (121)     3484 2021-09-04 04:57:51.000000 pykooh-0.3.2/pykooh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-09-04 04:57:51.000000 pykooh-0.3.2/pykooh/smooth_numba.py
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2021-09-04 04:57:51.000000 pykooh-0.3.2/pykooh/smoothing.c
--rw-r--r--   0 runner    (1001) docker     (121)      179 2021-09-04 04:57:51.000000 pykooh-0.3.2/pykooh/smoothing.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-04 04:58:04.571072 pykooh-0.3.2/pykooh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4470 2021-09-04 04:58:04.000000 pykooh-0.3.2/pykooh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      336 2021-09-04 04:58:04.000000 pykooh-0.3.2/pykooh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-04 04:58:04.000000 pykooh-0.3.2/pykooh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-04 04:58:04.000000 pykooh-0.3.2/pykooh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-09-04 04:58:04.000000 pykooh-0.3.2/pykooh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-09-04 04:58:04.000000 pykooh-0.3.2/pykooh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-09-04 04:57:51.000000 pykooh-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-09-04 04:58:04.571072 pykooh-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2021-09-04 04:57:51.000000 pykooh-0.3.2/setup.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pykooh-0.4.0/HISTORY.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pykooh-0.4.0/MANIFEST.in
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 pykooh-0.4.0/Makefile
+-rw-r--r--   0        0        0   291232 2020-02-02 00:00:00.000000 pykooh-0.4.0/example.ipynb
+-rw-r--r--   0        0        0   109161 2020-02-02 00:00:00.000000 pykooh-0.4.0/implementation.ipynb
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pykooh-0.4.0/requirements.txt
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pykooh-0.4.0/requirements_dev.txt
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 pykooh-0.4.0/requirements_rtfd.txt
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 pykooh-0.4.0/setup.cfg
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 pykooh-0.4.0/setup.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pykooh-0.4.0/src/pykooh/__init__.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pykooh-0.4.0/src/pykooh/smooth_cython.pyx
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pykooh-0.4.0/src/pykooh/smooth_numba.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pykooh-0.4.0/src/pykooh/smoothing.c
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pykooh-0.4.0/src/pykooh/smoothing.h
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pykooh-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pykooh-0.4.0/tests/test_init.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 pykooh-0.4.0/tests/test_konno_ohmachi.py
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 pykooh-0.4.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0    91390 2020-02-02 00:00:00.000000 pykooh-0.4.0/tests/data/RSN4863_CHUETSU_65036EW.AT2
+-rw-r--r--   0        0        0    91390 2020-02-02 00:00:00.000000 pykooh-0.4.0/tests/data/RSN4863_CHUETSU_65036NS.AT2
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 pykooh-0.4.0/tests/data/example_ts.mseed
+-rw-r--r--   0        0        0    56832 2020-02-02 00:00:00.000000 pykooh-0.4.0/tests/data/test_data.npz
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 pykooh-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pykooh-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pykooh-0.4.0/README.md
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 pykooh-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 pykooh-0.4.0/PKG-INFO
```

### Comparing `pykooh-0.3.2/LICENSE` & `pykooh-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pykooh-0.3.2/README.rst` & `pykooh-0.4.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,59 @@
-pykooh
-======
+# pykooh
 
-|PyPi Cheese Shop| |Build Status| |Code Quality| |Test Coverage| |License| |DOI|
+[![PyPi Cheese
+Shop](https://img.shields.io/pypi/v/pykooh.svg)](https://img.shields.io/pypi/v/pykooh.svg)
+[![Build
+Status](https://github.com/arkottke/pykooh/actions/workflows/python-app.yml/badge.svg)](https://github.com/arkottke/pykooh/actions/workflows/python-app.yml)
+[![Code
+Quality](https://app.codacy.com/project/badge/Grade/c8a3110f14e444a598713b002c20f979)](https://www.codacy.com/manual/arkottke/pykooh)
+[![Test
+Coverage](https://api.codacy.com/project/badge/Coverage/c8a3110f14e444a598713b002c20f979)](https://www.codacy.com/manual/arkottke/pykooh)
+![License](https://img.shields.io/badge/license-MIT-blue.svg)
+[![DOI](https://zenodo.org/badge/183696586.svg)](https://zenodo.org/badge/latestdoi/183696586)
 
 Konno Ohmachi filter implemented in Numba.
 
-This code implements Konno-Ohmachi spectral smoothing as defined in::
+This code implements Konno-Ohmachi spectral smoothing as defined in:
 
     Konno, K. and Ohmachi, T., 1998. Ground-motion characteristics estimated
     from spectral ratio between horizontal and vertical components of
     microtremor. Bulletin of the Seismological Society of America, 88(1),
     pp.228-241.
 
-This code was originally written for smoothing sub-module in gmprocess_
-by Bruce Worden. Dave Boore has provided notes_
+This code was originally written for smoothing sub-module in
+[gmprocess](https://github.com/usgs/groundmotion-processing/tree/master/gmprocess/smoothing)
+by Bruce Worden. Dave Boore has provided
+[notes](http://daveboore.com/daves_notes/notes%20on%20smoothing%20over%20logarithmically%20spaced%20freqs.pd)
 on this topic, which also may be of interest. Notes regarding the
 characteristics of the Konno-Ohmachi filter and the implementation are
-provided in the implementation_ Jupyter Notebook.
+provided in the [implementation](implemenation.ipynb) Jupyter Notebook.
 
-.. _gmprocess: https://github.com/usgs/groundmotion-processing/tree/master/gmprocess/smoothing
-.. _notes: http://daveboore.com/daves_notes/notes%20on%20smoothing%20over%20logarithmically%20spaced%20freqs.pd
-.. _implementation: implemenation.ipynb
+# Installation
 
-Installation
-============
+`pykooh` is available via `pip` and can be installed with:
 
-``pykooh`` is available via ``pip`` and can be installed with:
+    pip install pykooh
 
-::
+By default, `pykooh` uses `numba` for the fast implementation of the
+filter. Performance can be increased by using `cython`, but this
+requires a C complier. If a C compiler is available, install `cython`
+required dependencies with:
 
-   pip install pykooh
+    pip install pykooh[cython]
 
-By default, ``pykooh`` uses ``numba`` for the fast implementation of the filter.
-Performance can be increased by using ``cython``, but this requires a C
-complier. If a C compiler is available, install ``cython`` required
-dependencies with:
-
-::
-
-   pip install pykooh[cython]
-
-Usage
-=====
+# Usage
 
 Smooth a signal using a bandwith of 30.
 
-.. code:: python
-
-   import pykooh
-   signal_smooth = pykooh.smooth(freqs, freqs_raw, signal_raw, 30)
-
-Additional examples and comparison with ``obspy`` are provided in example_.
-
-.. _example: example.ipynb
-
-Citation
-========
+```python
+import pykooh
+signal_smooth = pykooh.smooth(freqs, freqs_raw, signal_raw, 30)
+```
 
-Please cite this software using the following DOI_.
+Additional examples and comparison with `obspy` are provided in
+[example](example.ipynb).
 
-.. _DOI: https://zenodo.org/badge/latestdoi/183696586
+# Citation
 
-.. |PyPi Cheese Shop| image:: https://img.shields.io/pypi/v/pykooh.svg
-   :target: https://img.shields.io/pypi/v/pykooh.svg
-.. |Build Status| image:: https://travis-ci.org/arkottke/pykooh.svg?branch=master
-   :target: https://travis-ci.org/arkottke/pykooh
-.. |Code Quality| image:: https://app.codacy.com/project/badge/Grade/c8a3110f14e444a598713b002c20f979
-   :target: https://www.codacy.com/manual/arkottke/pykooh
-.. |Test Coverage| image:: https://api.codacy.com/project/badge/Coverage/c8a3110f14e444a598713b002c20f979
-   :target: https://www.codacy.com/manual/arkottke/pykooh
-.. |License| image:: https://img.shields.io/badge/license-MIT-blue.svg
-.. |DOI| image:: https://zenodo.org/badge/183696586.svg
-   :target: https://zenodo.org/badge/latestdoi/183696586
+Please cite this software using the following
+[DOI](https://zenodo.org/badge/latestdoi/183696586).
```

### Comparing `pykooh-0.3.2/pykooh/__init__.py` & `pykooh-0.4.0/src/pykooh/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,28 @@
-"""pykooh - Efficient implementatins of the Konno Omachi filter in Python.
+"""pykooh - Efficient implementatins of the Konno Omachi filter in Python."""
 
-"""
-import numpy as np
+from importlib.metadata import version
 
-from pkg_resources import get_distribution
+import numpy as np
 
 try:
     from . import smooth_cython
 
     has_cython = True
 except ImportError:
     has_cython = False
     smooth_cython = None
 
 from . import smooth_numba
 
-
 __author__ = "Albert Kottke"
-__copyright__ = "Copyright 2019-2020 Albert Kottke"
+__copyright__ = "Copyright 2019-2024 Albert Kottke"
 __license__ = "MIT"
-__title__ = "pykooh"
-__version__ = get_distribution("pykooh").version
-del get_distribution
+__title__ = "pyKOOH"
+__version__ = version("pyKOOH")
 
 
 def smooth(ko_freqs, freqs, spectrum, b, use_cython=True):
     # Only work on the absolute value
     spectrum = np.abs(spectrum)
 
     if has_cython and use_cython:
@@ -67,15 +64,17 @@
         Frequency of the spectrum
     effect_amp: :class:`np.ndarray`
         Effective amplitude spectrum.
 
     """
 
     # Calculate the average power of the two components
-    avg = np.abs(np.sqrt(0.5 * (fourier_amps_h1 ** 2 + fourier_amps_h2 ** 2)))
+    avg = np.abs(
+        np.sqrt(0.5 * (np.abs(fourier_amps_h1) ** 2 + np.abs(fourier_amps_h2) ** 2))
+    )
 
     if freqs_ea is None:
         # Frequency range is 100 points per decades
         start = 1 if np.isclose(freqs[0], 0) else 0
         left = np.floor(np.log10(freqs[start])).astype(int)
         right = np.ceil(np.log10(freqs[-1])).astype(int)
         ndecades = right - left
```

### Comparing `pykooh-0.3.2/pykooh/smooth_numba.py` & `pykooh-0.4.0/src/pykooh/smooth_numba.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Numba implementation."""
 
-import numpy as np
 import numba
+import numpy as np
 
 
 @numba.jit(nopython=True)
 def smooth(ko_freqs, freqs, spectrum, b):
     max_ratio = pow(10.0, (3.0 / b))
     min_ratio = 1.0 / max_ratio
```

### Comparing `pykooh-0.3.2/pykooh/smoothing.c` & `pykooh-0.4.0/src/pykooh/smoothing.c`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #include <math.h>
 #include "smoothing.h"
 
-/* 
- * This code implements Konno-Ohmachi spectral smoothing as defined in their 
- * paper: 
+/*
+ * This code implements Konno-Ohmachi spectral smoothing as defined in their
+ * paper:
  * Konno, K. and Ohmachi, T., 1998. Ground-motion characteristics estimated
  * from spectral ratio between horizontal and vertical components of
  * microtremor. Bulletin of the Seismological Society of America, 88(1),
  * pp.228-241.
  * The function below is partially based on a Python version by Albert
  * Kottke and found here:
  * https://github.com/arkottke/notebooks/blob/master/effective_amp_spectrum.ipynb
  * It was rewritten and optimized in C by Bruce Worden.
  */
 void konno_ohmachi_c(
-        double *spec, 
-        double *freqs, 
+        double *spec,
+        double *freqs,
         int ns,
-        double *ko_freqs, 
-        double *ko_smooth, 
+        double *ko_freqs,
+        double *ko_smooth,
         int nks,
         double b) {
     int i, j;
     double window_total, total, x, fc, freq, frat, window;
     double max_ratio = pow(10.0, (3.0 / b));
     double min_ratio = 1.0 / max_ratio;
```

