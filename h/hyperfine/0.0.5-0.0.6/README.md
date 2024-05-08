# Comparing `tmp/hyperfine-0.0.5.tar.gz` & `tmp/hyperfine-0.0.6.tar.gz`

## Comparing `hyperfine-0.0.5.tar` & `hyperfine-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/_version.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/demagnetization.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/distributions.py
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/dpass.py
--rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/minuit.py
--rw-r--r--   0        0        0    13475 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/srim.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/bnmr/__init__.py
--rw-r--r--   0        0        0    14249 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/bnmr/lineshape.py
--rw-r--r--   0        0        0    18998 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/bnmr/meissner.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/bnmr/nlme.py
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/bnmr/susceptibility.py
--rw-r--r--   0        0        0     8229 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/musr/__init__.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/musr/_meissner.py
--rw-r--r--   0        0        0    26336 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/musr/meissner.py
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/superconductivity/__init__.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/superconductivity/_muhlschlegel.py
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/superconductivity/bcs.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/superconductivity/ccf.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/superconductivity/interpolation.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/superconductivity/intertype.py
--rw-r--r--   0        0        0    18362 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/superconductivity/london.py
--rw-r--r--   0        0        0    15737 2020-02-02 00:00:00.000000 hyperfine-0.0.5/hyperfine/superconductivity/pippard.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 hyperfine-0.0.5/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 hyperfine-0.0.5/LICENSE
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 hyperfine-0.0.5/README.md
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 hyperfine-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 hyperfine-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/_version.py
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/demagnetization.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/distributions.py
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/dpass.py
+-rw-r--r--   0        0        0    10136 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/minuit.py
+-rw-r--r--   0        0        0    13475 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/srim.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/bnmr/__init__.py
+-rw-r--r--   0        0        0    14249 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/bnmr/lineshape.py
+-rw-r--r--   0        0        0    18998 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/bnmr/meissner.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/bnmr/nlme.py
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/bnmr/susceptibility.py
+-rw-r--r--   0        0        0     8229 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/musr/__init__.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/musr/_meissner.py
+-rw-r--r--   0        0        0    26336 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/musr/meissner.py
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/superconductivity/__init__.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/superconductivity/_muhlschlegel.py
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/superconductivity/bcs.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/superconductivity/ccf.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/superconductivity/interpolation.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/superconductivity/intertype.py
+-rw-r--r--   0        0        0    18362 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/superconductivity/london.py
+-rw-r--r--   0        0        0    15737 2020-02-02 00:00:00.000000 hyperfine-0.0.6/hyperfine/superconductivity/pippard.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 hyperfine-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 hyperfine-0.0.6/LICENSE
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 hyperfine-0.0.6/README.md
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 hyperfine-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 hyperfine-0.0.6/PKG-INFO
```

### Comparing `hyperfine-0.0.5/hyperfine/demagnetization.py` & `hyperfine-0.0.6/hyperfine/demagnetization.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/distributions.py` & `hyperfine-0.0.6/hyperfine/distributions.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/dpass.py` & `hyperfine-0.0.6/hyperfine/dpass.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/minuit.py` & `hyperfine-0.0.6/hyperfine/minuit.py`

 * *Files 19% similar despite different names*

```diff
@@ -74,33 +74,105 @@
                 # parameter pair combination
                 covariance[par1][par2] = minuit.covariance[par1, par2]
 
     # return the covariance matrix
     return covariance
 
 
+def correlation2dict(minuit: Minuit) -> dict:
+    """Convert the correlation matrix to a serializable dictionary.
+
+    Convert the correlation matrix (i.e., derived from the MIGRAD or HESSE errors)
+    determined by the MINUIT2 minimizer to a *serializable* dictionary
+    (i.e., one that is compatible with JSON).
+
+    Args:
+        minuit: The ``iminuit.Minuit`` object.
+
+    Returns:
+        A serializable dictionary containing the correlation matrix.
+    """
+
+    # empty dictionary to hold the matrix
+    correlation = {}
+
+    # check if the covariance matrix exists
+    if minuit.covariance is not None:
+        # loop over all fit parameters
+        for par1 in minuit.parameters:
+            # for each parameter, create an empty dictionary...
+            correlation[par1] = {}
+            # loop over all fit parameters
+            for par2 in minuit.parameters:
+                # ...to be filled with the (normalized) covariance for each
+                # parameter pair combination
+                correlation[par1][par2] = minuit.covariance[par1, par2] / np.sqrt(
+                    minuit.covariance[par1, par1] * minuit.covariance[par2, par2]
+                )
+
+    # return the covariance matrix
+    return correlation
+
+
+def fmin2dict(minuit: Minuit) -> dict:
+    """Convert the metadata about the cost function minimum to a serializable dictionary.
+
+    Convert the contents of ``iminuit.Minuit.fmin`` (i.e, an ``iminuit.util.FMin`` object)
+    to a *serializable* dictionary (i.e., one that is compatible with JSON).
+    The ``iminuit.util.FMin`` object provides detailed metadata about the function minimum
+    (e.g., the value of the cost function, validity of the minimum, etc.).
+    The metadata is useful for checking what happened when a fit didn't converge.
+
+    Args:
+        minuit: The ``iminuit.Minuit`` object.
+
+    Returns:
+        A serializable dictionary containing the metadata about the cost function minimum.
+    """
+
+    # create an empty dictionary
+    fmin = {}
+
+    if minuit.fmin is None:
+        # return the empty dictionary if the cost function has not been minimized
+        return fmin
+
+    else:
+        # populate the dictionary with all of fmin's public attributes
+        for key in sorted(dir(minuit.fmin)):
+            if key.startswith("_"):
+                continue
+            value = getattr(minuit.fmin, key)
+            fmin[key] = value
+
+        return fmin
+
+
 def minuit2json(minuit: Minuit, filename: str) -> None:
     """Serialize fitting results from an ``iminuit.Minuit`` object to a JSON file.
 
     Serialization includes data for: ``values``, ``errors``, ``limits``,
-    ``fixed``, ``covariance``, and ``merrors``.
+    ``fixed``, ``covariance``, ``merrors``, and ``fmin``. Parameter correlations
+    (derived from ``covariance``) are also included.
 
     Args:
         minuit: The ``iminuit.Minuit`` object.
         filename: Name of JSON file to save the serialized fit results.
     """
 
     # convert the results to a dictionary
     results = {
         "values": minuit.values.to_dict(),
         "errors": minuit.errors.to_dict(),
         "limits": minuit.limits.to_dict(),
         "fixed": minuit.fixed.to_dict(),
         "covariance": covariance2dict(minuit),
+        "correlation": correlation2dict(minuit),
         "merrors": minos2dict(minuit),
+        "fmin": fmin2dict(minuit),
     }
 
     # write the results dictionary to a file
     with open(filename, "w") as fh:
         json.dump(results, fh, indent="\t")
```

### Comparing `hyperfine-0.0.5/hyperfine/srim.py` & `hyperfine-0.0.6/hyperfine/srim.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/bnmr/lineshape.py` & `hyperfine-0.0.6/hyperfine/bnmr/lineshape.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/bnmr/meissner.py` & `hyperfine-0.0.6/hyperfine/bnmr/meissner.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/bnmr/nlme.py` & `hyperfine-0.0.6/hyperfine/bnmr/nlme.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/bnmr/susceptibility.py` & `hyperfine-0.0.6/hyperfine/bnmr/susceptibility.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/musr/__init__.py` & `hyperfine-0.0.6/hyperfine/musr/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/musr/_meissner.py` & `hyperfine-0.0.6/hyperfine/musr/_meissner.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/musr/meissner.py` & `hyperfine-0.0.6/hyperfine/musr/meissner.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/superconductivity/__init__.py` & `hyperfine-0.0.6/hyperfine/superconductivity/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/superconductivity/_muhlschlegel.py` & `hyperfine-0.0.6/hyperfine/superconductivity/_muhlschlegel.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/superconductivity/bcs.py` & `hyperfine-0.0.6/hyperfine/superconductivity/bcs.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/superconductivity/ccf.py` & `hyperfine-0.0.6/hyperfine/superconductivity/ccf.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/superconductivity/interpolation.py` & `hyperfine-0.0.6/hyperfine/superconductivity/interpolation.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/superconductivity/intertype.py` & `hyperfine-0.0.6/hyperfine/superconductivity/intertype.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/superconductivity/london.py` & `hyperfine-0.0.6/hyperfine/superconductivity/london.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/hyperfine/superconductivity/pippard.py` & `hyperfine-0.0.6/hyperfine/superconductivity/pippard.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/.gitignore` & `hyperfine-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/LICENSE` & `hyperfine-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/README.md` & `hyperfine-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/pyproject.toml` & `hyperfine-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.5/PKG-INFO` & `hyperfine-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hyperfine
-Version: 0.0.5
+Version: 0.0.6
 Project-URL: Homepage, https://github.com/rmlmcfadden/hyperfine
 Project-URL: Documentation, https://hyperfine.readthedocs.io/
 Project-URL: Repository, https://github.com/rmlmcfadden/hyperfine.git
 Project-URL: Issues, https://github.com/rmlmcfadden/hyperfine/issues
 Author-email: "Ryan M. L. McFadden" <rmlm@triumf.ca>
 License-Expression: MIT
 License-File: LICENSE
```

