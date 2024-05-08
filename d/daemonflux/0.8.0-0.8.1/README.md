# Comparing `tmp/daemonflux-0.8.0.tar.gz` & `tmp/daemonflux-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daemonflux-0.8.0.tar", last modified: Wed Apr 10 13:35:29 2024, max compression
+gzip compressed data, was "daemonflux-0.8.1.tar", last modified: Wed May  8 11:34:36 2024, max compression
```

## Comparing `daemonflux-0.8.0.tar` & `daemonflux-0.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:35:29.227994 daemonflux-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-10 13:35:09.000000 daemonflux-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-10 13:35:29.227994 daemonflux-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-10 13:35:09.000000 daemonflux-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-10 13:35:09.000000 daemonflux-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-10 13:35:29.227994 daemonflux-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:35:29.227994 daemonflux-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:35:29.227994 daemonflux-0.8.0/src/daemonflux/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-10 13:35:09.000000 daemonflux-0.8.0/src/daemonflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28411 2024-04-10 13:35:09.000000 daemonflux-0.8.0/src/daemonflux/flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-10 13:35:09.000000 daemonflux-0.8.0/src/daemonflux/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:35:29.227994 daemonflux-0.8.0/src/daemonflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-10 13:35:29.000000 daemonflux-0.8.0/src/daemonflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-10 13:35:29.000000 daemonflux-0.8.0/src/daemonflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:35:29.000000 daemonflux-0.8.0/src/daemonflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 13:35:29.000000 daemonflux-0.8.0/src/daemonflux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 13:35:29.000000 daemonflux-0.8.0/src/daemonflux.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:35:29.227994 daemonflux-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14455 2024-04-10 13:35:09.000000 daemonflux-0.8.0/tests/test_daemonflux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:34:36.150452 daemonflux-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-08 11:34:15.000000 daemonflux-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-08 11:34:36.150452 daemonflux-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-05-08 11:34:15.000000 daemonflux-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-08 11:34:15.000000 daemonflux-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-08 11:34:36.154452 daemonflux-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:34:36.150452 daemonflux-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:34:36.150452 daemonflux-0.8.1/src/daemonflux/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-08 11:34:15.000000 daemonflux-0.8.1/src/daemonflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28867 2024-05-08 11:34:15.000000 daemonflux-0.8.1/src/daemonflux/flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-08 11:34:15.000000 daemonflux-0.8.1/src/daemonflux/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:34:36.150452 daemonflux-0.8.1/src/daemonflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-08 11:34:36.000000 daemonflux-0.8.1/src/daemonflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-08 11:34:36.000000 daemonflux-0.8.1/src/daemonflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:34:36.000000 daemonflux-0.8.1/src/daemonflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-08 11:34:36.000000 daemonflux-0.8.1/src/daemonflux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 11:34:36.000000 daemonflux-0.8.1/src/daemonflux.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:34:36.150452 daemonflux-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14656 2024-05-08 11:34:15.000000 daemonflux-0.8.1/tests/test_daemonflux.py
```

### Comparing `daemonflux-0.8.0/LICENSE` & `daemonflux-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `daemonflux-0.8.0/PKG-INFO` & `daemonflux-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daemonflux
-Version: 0.8.0
+Version: 0.8.1
 Summary: Tabulated representation of a muon-calibrated muon and neutrino flux model
 Home-page: https://github.com/mceq-project/daemonflux
 Download-URL: https://pypi.python.org/pypi/daemonflux
 Author: Anatoli Fedynitch
 Maintainer-email: afedynitch@gmail.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `daemonflux-0.8.0/README.md` & `daemonflux-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `daemonflux-0.8.0/setup.cfg` & `daemonflux-0.8.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = daemonflux
-version = 0.8.0
+version = 0.8.1
 author = Anatoli Fedynitch
 maintainer_email = afedynitch@gmail.com
 description = Tabulated representation of a muon-calibrated muon and neutrino flux model
 license = BSD 3-Clause License
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mceq-project/daemonflux
```

### Comparing `daemonflux-0.8.0/src/daemonflux/__init__.py` & `daemonflux-0.8.1/src/daemonflux/__init__.py`

 * *Files identical despite different names*

### Comparing `daemonflux-0.8.0/src/daemonflux/flux.py` & `daemonflux-0.8.1/src/daemonflux/flux.py`

 * *Files 6% similar despite different names*

```diff
@@ -377,24 +377,24 @@
         Parameters
         ----------
         exp : str, optional
             Experiment name, default is an empty string.
         """
         return self._get_flux_instance(exp)._params
 
-    def flux(self, grid, zenith_deg, quantity, params={}, exp=""):
+    def flux(self, energy, zenith_deg, quantity, params={}, exp=""):
         """
-        The flux of a given quantity for the specified energy grid and zenith angles.
+        The flux of a given quantity for the specified energy energy and zenith angles.
 
         The flux is multiplied by E^3 in units of GeV^2/(cm^2 s sr).
 
         Parameters
         ----------
-        grid : np.ndarray
-            The energy grid in units of GeV.
+        energy : float or np.ndarray
+            The energy energy in units of GeV.
         zenith_deg : float or str or list of float
             The zenith angle in degrees. If "average", the average flux over all
             zenith angles will be returned.
         quantity : str
             The type of flux to be returned.
         params : Dict[str, float], optional
             A dictionary of parameter values to shift daemonflux off the baseline.
@@ -405,26 +405,26 @@
             The flux multiplied by E^3 in units of GeV^2/(cm^2 s sr).
 
         Raises
         ------
         Exception
             If `zenith_deg` is "average" but splines do not contain average flux.
         """
-        return self._get_flux_instance(exp).flux(grid, zenith_deg, quantity, params)
+        return self._get_flux_instance(exp).flux(energy, zenith_deg, quantity, params)
 
-    def error(self, grid, zenith_deg, quantity, only_hadronic=False, exp=""):
+    def error(self, energy, zenith_deg, quantity, only_hadronic=False, exp=""):
         """
-        The flux of a given quantity for the specified energy grid and zenith angles.
+        The flux of a given quantity for the specified energy energy and zenith angles.
 
         The error is multiplied by E^3 in units of GeV^2/(cm^2 s sr).
 
         Parameters
         ----------
-        grid : np.ndarray
-            The energy grid for which to compute the error.
+        energy : float or np.ndarray
+            The energy energy for which to compute the error.
         zenith_deg : float or str or list of float
             The zenith angle in degrees, or a list of zenith angles.
         quantity : str
             The quantity to compute the error for.
         only_hadronic : bool, optional
             Whether to only include the hadronic error, excluding the cosmic ray flux
             error, by default False.
@@ -436,15 +436,15 @@
 
         Raises
         ------
         Exception
             If `zenith_deg` is "average" but splines do not contain average flux.
         """
         return self._get_flux_instance(exp).error(
-            grid,
+            energy,
             zenith_deg,
             quantity,
             only_hadronic,
         )
 
     def chi2(self, params={}, exp=""):
         """
@@ -570,90 +570,91 @@
             assert pars.cov.shape[0] == len(pars.known_parameters) == len(pars.values)
 
             yield
 
             self._params = prev
             assert pars.cov.shape[0] == len(pars.known_parameters) == len(pars.values)
 
-    def _check_input(self, grid: np.ndarray, quantity: str) -> None:
+    def _check_input(self, energy: Union[np.ndarray, float], quantity: str) -> None:
         """
-        Check the validity of the input grid and quantity.
+        Check the validity of the input energy and quantity.
 
         Parameters
         ----------
-        grid : np.ndarray
-            The energy grid.
+        energy : float or np.ndarray
+            The energy energy.
         quantity : str
             The quantity to be calculated.
 
         Raises
         ------
         AssertionError
-            If the energy grid is out of range or if the quantity is unknown.
+            If the energy energy is out of range or if the quantity is unknown.
         """
-        assert np.max(grid) <= 1e9 and np.min(grid) >= 5e-2, "Energy out of range"
+        assert np.max(energy) <= 1e9 and np.min(energy) >= 5e-2, "Energy out of range"
         assert quantity in self._quantities, "Quantity must be one of {0}.".format(
             ", ".join(self._quantities)
         )
 
     def _flux_from_spl(
         self,
-        grid: np.ndarray,
+        energy: Union[np.ndarray, float],
         zenith_deg: str,
         quantity: str,
         params: Dict[str, float],
     ) -> np.ndarray:
         """
         Calculate the flux based on spline representation.
 
         Parameters
         ----------
-        grid : numpy.ndarray
+        energy : float or numpy.ndarray
             The grid of energies for which the flux is calculated.
         zenith_deg : str
             The zenith angle in degrees for which the flux is calculated.
         quantity : str
             The type of quantity for which the flux is calculated.
         params : Dict[str, float], optional
             The parameters for the flux calculation.
         """
         jac = self._jac_spl[zenith_deg]
         fl = self._fl_spl[zenith_deg]
         with self._temporary_parameters(params):
             corrections = 1 + np.sum(
-                [v * jac[dk][quantity](np.log(grid)) for (dk, v) in self._params],
+                [v * jac[dk][quantity](np.log(energy)) for (dk, v) in self._params],
                 axis=0,
             )
-        return np.exp(fl[quantity](np.log(grid))) * corrections
+        return (np.exp(fl[quantity](np.log(energy))) * corrections).squeeze()
 
     def _flux_from_interp(
         self,
-        grid: np.ndarray,
+        energy: Union[np.ndarray, float],
         zenith_deg: Union[float, str, np.ndarray],
         quantity: str,
         params: Dict[str, float],
     ) -> np.ndarray:
         from scipy.interpolate import interp1d
 
+        energy = np.atleast_1d(energy).astype("float64")
         zenith_darr = np.atleast_1d(zenith_deg).astype("float64")
         zenith_carr = np.cos(np.deg2rad(zenith_darr))
 
         idxmin, idxmax = self._interpolation_domain(zenith_darr)
-        interp_array = np.zeros((idxmax - idxmin, len(grid)))
+        interp_array = np.zeros((idxmax - idxmin, len(energy)))
         for i, idx in enumerate(range(idxmin, idxmax)):
             interp_array[i, :] = self._flux_from_spl(
-                grid, self.zenith_angles[idx], quantity, params
+                energy, self.zenith_angles[idx], quantity, params
             )
         return interp1d(self._zenith_cos_arr[idxmin:idxmax], interp_array, axis=0)(
             zenith_carr
         ).T.squeeze()
 
     def _error_from_spl(
         self,
-        grid: np.ndarray,
+        energy: Union[np.ndarray, float],
         zenith_deg: Union[float, str, np.ndarray],
         quantity: str,
         only_hadronic: bool,
     ) -> np.ndarray:
         if self._debug > 2:
             print(
                 f"Return {quantity} flux for {zenith_deg}, only_hadronic=",
@@ -661,38 +662,41 @@
             )
 
         with self._temporary_exclude_parameters("GSF" if only_hadronic else None):
             jac = self._jac_spl[zenith_deg]
 
             jacfl = np.vstack(
                 [
-                    jac[par][quantity](np.log(grid))
+                    jac[par][quantity](np.log(energy))
                     for par in self._params.known_parameters
                 ]
             ).T
             error = np.sqrt(np.diag(grid_cov(jacfl, self._params.cov)))
-            return np.exp(self._fl_spl[zenith_deg][quantity](np.log(grid))) * error
+            return (
+                np.exp(self._fl_spl[zenith_deg][quantity](np.log(energy))) * error
+            ).squeeze()
 
     def _error_from_interp(
         self,
-        grid: np.ndarray,
+        energy: Union[np.ndarray, float],
         zenith_deg: Union[float, str, np.ndarray],
         quantity: str,
         only_hadronic: bool,
     ) -> np.ndarray:
         from scipy.interpolate import interp1d
 
+        energy = np.atleast_1d(energy).astype("float64")
         zenith_darr = np.atleast_1d(zenith_deg).astype("float64")
         zenith_carr = np.cos(np.deg2rad(zenith_darr))
 
         idxmin, idxmax = self._interpolation_domain(zenith_darr)
-        interp_array = np.zeros((idxmax - idxmin, len(grid)))
+        interp_array = np.zeros((idxmax - idxmin, len(energy)))
         for i, idx in enumerate(range(idxmin, idxmax)):
             interp_array[i, :] = self._error_from_spl(
-                grid, self.zenith_angles[idx], quantity, only_hadronic
+                energy, self.zenith_angles[idx], quantity, only_hadronic
             )
         return interp1d(self._zenith_cos_arr[idxmin:idxmax], interp_array, axis=0)(
             zenith_carr
         ).T.squeeze()
 
     def _interpolation_domain(
         self, zenith_angles_deg: Union[float, np.ndarray]
@@ -733,108 +737,108 @@
             if idxmax > len(self._zenith_deg_arr):
                 idxmin -= 1
                 idxmax -= 1
         return idxmin, idxmax
 
     def flux(
         self,
-        grid: np.ndarray,
+        energy: Union[float, np.ndarray],
         zenith_deg: Union[float, str, np.ndarray],
         quantity: str,
         params: Dict[str, float] = {},
-    ) -> np.ndarray:
+    ) -> Union[float, np.ndarray]:
         """
-        Compute the flux at the given energy grid, zenith angle, and quantity.
+        Compute the flux at the given energy energy, zenith angle, and quantity.
 
         Parameters
         ----------
-        grid : np.ndarray
-            The energy grid in units of GeV.
+        energy : float or np.ndarray
+            The energy energy in units of GeV.
         zenith_deg : float or str or list of float
             The zenith angle in degrees. If "average", the average flux over all
             zenith angles will be returned.
         quantity : str
             The type of flux to be returned.
         params : Dict[str, float], optional
             A dictionary of parameter values to shift daemonflux off the baseline.
 
         Returns
         -------
-        np.ndarray
+        float or np.ndarray
             The flux multiplied by E^3 in units of GeV^2/(cm^2 s sr).
 
         Raises
         ------
         Exception
             If `zenith_deg` is "average" but splines do not contain average flux.
         """
-        self._check_input(grid, quantity)
+        self._check_input(energy, quantity)
         # handle the case where the zenith angle is "average"
         if isinstance(zenith_deg, str) and zenith_deg == "average":
             if not self._spl_contains_average:
                 raise Exception("Splines do not contain average flux")
-            return self._flux_from_spl(grid, zenith_deg, quantity, params)
+            return self._flux_from_spl(energy, zenith_deg, quantity, params)
 
         # handle the case where the zenith angle is a single value or an array
         if not is_iterable(zenith_deg) and float(zenith_deg) in self._zenith_deg_arr:
             return self._flux_from_spl(
-                grid, format_angle(float(zenith_deg)), quantity, params
+                energy, format_angle(float(zenith_deg)), quantity, params
             )
         else:
-            return self._flux_from_interp(grid, zenith_deg, quantity, params)
+            return self._flux_from_interp(energy, zenith_deg, quantity, params)
 
     def error(
         self,
-        grid: np.ndarray,
+        energy: Union[float, np.ndarray],
         zenith_deg: Union[float, str],
         quantity: str,
         only_hadronic: bool = False,
-    ) -> np.ndarray:
+    ) -> Union[float, np.ndarray]:
         """
         Return the error of the flux estimation for the given parameters.
 
         The error is multiplied by E^3 in units of GeV^2/(cm^2 s sr).
 
         Parameters
         ----------
-        grid : np.ndarray
-            The energy grid for which to compute the error.
+        energy : float or np.ndarray
+            The energy energy for which to compute the error.
         zenith_deg : float or str
             The zenith angle in degrees. If a string, it must be "average".
         quantity : str
             The quantity to compute the error for.
         only_hadronic : bool, optional
             Whether to only include the hadronic error, excluding the cosmic ray flux
             error, by default False.
 
         Returns
         -------
-        np.ndarray
+        float or np.ndarray
             The error of the flux estimation.
 
         Raises
         ------
         Exception
             If `zenith_deg` is "average" but splines do not contain average flux.
         """
-        self._check_input(grid, quantity)
+        self._check_input(energy, quantity)
 
         # handle the case where the zenith angle is "average"
         if isinstance(zenith_deg, str) and zenith_deg == "average":
             if not self._spl_contains_average:
                 raise Exception("Splines do not contain average flux")
-            return self._error_from_spl(grid, zenith_deg, quantity, only_hadronic)
+            return self._error_from_spl(energy, zenith_deg, quantity, only_hadronic)
 
         # handle the case where the zenith angle is a single value or an array
         if not is_iterable(zenith_deg) and float(zenith_deg) in self._zenith_deg_arr:
             return self._error_from_spl(
-                grid, format_angle(zenith_deg), quantity, only_hadronic
+                energy, format_angle(zenith_deg), quantity, only_hadronic
             )
         else:
-            return self._error_from_interp(grid, zenith_deg, quantity, only_hadronic)
+            return self._error_from_interp(energy, zenith_deg, quantity, only_hadronic)
 
     def chi2(self, params={}):
         """
         Returns the chi-square value of the parameters.
 
         Parameters
         ----------
```

### Comparing `daemonflux-0.8.0/src/daemonflux/utils.py` & `daemonflux-0.8.1/src/daemonflux/utils.py`

 * *Files identical despite different names*

### Comparing `daemonflux-0.8.0/src/daemonflux.egg-info/PKG-INFO` & `daemonflux-0.8.1/src/daemonflux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daemonflux
-Version: 0.8.0
+Version: 0.8.1
 Summary: Tabulated representation of a muon-calibrated muon and neutrino flux model
 Home-page: https://github.com/mceq-project/daemonflux
 Download-URL: https://pypi.python.org/pypi/daemonflux
 Author: Anatoli Fedynitch
 Maintainer-email: afedynitch@gmail.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `daemonflux-0.8.0/tests/test_daemonflux.py` & `daemonflux-0.8.1/tests/test_daemonflux.py`

 * *Files 2% similar despite different names*

```diff
@@ -388,7 +388,12 @@
         uncorrelated_hadr_errors=True,
         debug=1,
     )
     assert np.allclose(
         fl.params.cov[: fl.params._n_non_gsf, : fl.params._n_non_gsf],
         np.diag(np.ones(fl.params._n_non_gsf)),
     )
+
+
+def test_scalar_energy_arg(test_flux_calibrated):
+    assert test_flux_calibrated.flux(100.0, 15.0, "numuflux").shape == ()
+    assert test_flux_calibrated.error(100.0, 15.0, "numuflux").shape == ()
```

