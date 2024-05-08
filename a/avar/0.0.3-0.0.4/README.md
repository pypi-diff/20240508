# Comparing `tmp/avar-0.0.3.tar.gz` & `tmp/avar-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avar-0.0.3.tar", last modified: Thu Apr 18 11:44:43 2024, max compression
+gzip compressed data, was "avar-0.0.4.tar", last modified: Wed May  8 17:27:41 2024, max compression
```

## Comparing `avar-0.0.3.tar` & `avar-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-18 11:44:43.210911 avar-0.0.3/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-18 11:26:07.000000 avar-0.0.3/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      513 2024-04-18 11:44:43.210857 avar-0.0.3/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       45 2024-04-18 11:27:04.000000 avar-0.0.3/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2024-04-18 11:26:07.000000 avar-0.0.3/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      576 2024-04-18 11:44:43.211132 avar-0.0.3/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-18 11:44:43.209167 avar-0.0.3/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-18 11:44:43.209939 avar-0.0.3/src/avar/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-04-18 11:28:55.000000 avar-0.0.3/src/avar/__init__.py
--rwxr-xr-x   0 davidwoodburn   (501) staff       (20)     8541 2024-04-16 21:22:35.000000 avar-0.0.3/src/avar/avar.py
--rwxr-xr-x   0 davidwoodburn   (501) staff       (20)      764 2024-04-18 11:43:11.000000 avar-0.0.3/src/avar/test_avar.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-18 11:44:43.210681 avar-0.0.3/src/avar.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      513 2024-04-18 11:44:43.000000 avar-0.0.3/src/avar.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      265 2024-04-18 11:44:43.000000 avar-0.0.3/src/avar.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-18 11:44:43.000000 avar-0.0.3/src/avar.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       12 2024-04-18 11:44:43.000000 avar-0.0.3/src/avar.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-04-18 11:44:43.000000 avar-0.0.3/src/avar.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-08 17:27:41.709356 avar-0.0.4/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-18 11:26:07.000000 avar-0.0.4/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     3290 2024-05-08 17:27:41.709306 avar-0.0.4/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     2822 2024-05-08 17:26:15.000000 avar-0.0.4/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2024-04-18 11:26:07.000000 avar-0.0.4/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      576 2024-05-08 17:27:41.709575 avar-0.0.4/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-08 17:27:41.707428 avar-0.0.4/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-08 17:27:41.708438 avar-0.0.4/src/avar/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-04-18 11:28:55.000000 avar-0.0.4/src/avar/__init__.py
+-rwxr-xr-x   0 davidwoodburn   (501) staff       (20)    10348 2024-05-08 17:25:34.000000 avar-0.0.4/src/avar/avar.py
+-rwxr-xr-x   0 davidwoodburn   (501) staff       (20)      782 2024-05-08 16:11:36.000000 avar-0.0.4/src/avar/test_avar.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-08 17:27:41.709139 avar-0.0.4/src/avar.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     3290 2024-05-08 17:27:41.000000 avar-0.0.4/src/avar.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      265 2024-05-08 17:27:41.000000 avar-0.0.4/src/avar.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-08 17:27:41.000000 avar-0.0.4/src/avar.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       12 2024-05-08 17:27:41.000000 avar-0.0.4/src/avar.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-08 17:27:41.000000 avar-0.0.4/src/avar.egg-info/top_level.txt
```

### Comparing `avar-0.0.3/LICENSE.txt` & `avar-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `avar-0.0.3/setup.cfg` & `avar-0.0.4/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = avar
-version = 0.0.3
+version = 0.0.4
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Allan variance tools
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/avar
 classifiers =
```

### Comparing `avar-0.0.3/src/avar/avar.py` & `avar-0.0.4/src/avar/avar.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+"""
+Copyright 2024 David Woodburn
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+"""
+
+__author__ = "David Woodburn"
+__license__ = "MIT"
+__date__ = "2024-05-08"
+__maintainer__ = "David Woodburn"
+__email__ = "david.woodburn@icloud.com"
+__status__ = "Development"
+
 import numpy as np
 import scipy.optimize as opt
 
 
 def windows(K, density=64):
     """
     Build an array of averaging window sizes for Allan variances analysis.
@@ -33,35 +61,47 @@
 def variance(y, M):
     """
     Calculate the Allan variance of y with the array of averaging window sizes
     specified by M.
 
     Parameters
     ----------
-    y : (K,) float np.ndarray
-        Array of `K` values in time.
+    y : (K,) or (J, K) float np.ndarray
+        Array of `K` values in time or matrix of rows of such arrays.
     M : (I,) integer np.ndarray
         Array of `I` averaging window sizes. Each element of `M` must be an
         integer.
 
     Returns
     -------
     v : (I,) float np.ndarray
         Array of `I` Allan variances.
     """
 
-    v = np.zeros(len(M))
-    Y = np.cumsum(y)
-    for n_tau, m in enumerate(M):
-        Yc = Y[(2*m - 1):] # Ending integrals
-        Yb = Y[(m - 1):(-m)] # Middle integrals
-        Yj = Y[:(1 - 2*m)] # Beginning integrals
-        yj = y[:(1 - 2*m)] # Beginning
-        delta = (Yc - 2*Yb + Yj - yj)/m
-        v[n_tau] = np.mean(delta**2)/2
+    if np.ndim(y) == 1:
+        v = np.zeros(len(M))
+        Y = np.cumsum(y)
+        for n_tau, m in enumerate(M):
+            Yc = Y[(2*m - 1):] # Ending integrals
+            Yb = Y[(m - 1):(-m)] # Middle integrals
+            Yj = Y[:(1 - 2*m)] # Beginning integrals
+            yj = y[:(1 - 2*m)] # Beginning
+            delta = (Yc - 2*Yb + Yj - yj)/m
+            v[n_tau] = np.mean(delta**2)/2
+    else:
+        J, K = y.shape
+        v = np.zeros((J, len(M)))
+        Y = np.cumsum(y, axis=1)
+        for n_tau, m in enumerate(M):
+            Yc = Y[:, (2*m - 1):] # Ending integrals
+            Yb = Y[:, (m - 1):(-m)] # Middle integrals
+            Yj = Y[:, :(1 - 2*m)] # Beginning integrals
+            yj = y[:, :(1 - 2*m)] # Beginning
+            delta = (Yc - 2*Yb + Yj - yj)/m
+            v[:, n_tau] = np.mean(delta**2, axis=1)/2
 
     return v
 
 
 def ideal(tau, vc, taub=None):
     """
     Generate an ideal Allan variance curve given the component variances.
@@ -81,15 +121,15 @@
     va : (I,) np.ndarray
         Array of ideal Allan variances.
     va_comps : (5, I) np.ndarray
         Matrix of the 5 ideal Allan variance components.
     """
 
     # Get the flicker Allan variance.
-    if taub is None:
+    if (taub is None) or (taub == 0.0):
         flkr = (2*np.log(2))/np.pi + 0*tau
     else:
         p = np.exp(-tau[0]/taub)
         M = tau/tau[0]
         flkr = 1.0/M**2*(M*(1 - p)**2 + 2*p*M*(1 - p) - 2*p*(1 - p**M)
             - p*(1 - p**M)**2)/(1 - p)**2
```

### Comparing `avar-0.0.3/src/avar/test_avar.py` & `avar-0.0.4/src/avar/test_avar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 import numpy as np
 import avar
-import trm
+import itrm
 
 # Constants
 T = 0.01
 t_dur = 200.0
 J = 100
 vc = np.array([0.5, 1.0, 7.85, 0.5, 0.1]) * 1e-9
 taub = 0.5305
@@ -18,17 +18,17 @@
 M = avar.windows(K)
 tau = M*T
 va_real = np.zeros(len(M))
 tic = time.perf_counter()
 for j in range(J):
     n = avar.noise(vc, K, T, taub)
     va_real += avar.variance(n, M)/J
-    trm.progress(j, J, tic)
+    itrm.progress(j, J, tic)
 
 # Get the ideal and fitted Allan variances.
 va_ideal, _ = avar.ideal(tau, vc, taub)
 va_fit, vc_fit = avar.fit(tau, va_real, taub)
 
 # Show the results.
-trm.table(np.array([vc, vc_fit]), left=["true", "fit"])
+itrm.table(np.array([vc, vc_fit]), left=["true", "fit"])
 y = np.array([va_real, va_ideal, va_fit])
-trm.plot(np.log10(tau), np.log10(y), rows=0.95)
+itrm.iplot(np.log10(tau), np.log10(y), label="Allan variance")
```

