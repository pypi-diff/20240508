# Comparing `tmp/squishyplanet-0.1.0.tar.gz` & `tmp/squishyplanet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squishyplanet-0.1.0.tar", last modified: Thu May  2 20:41:19 2024, max compression
+gzip compressed data, was "squishyplanet-0.1.1.tar", last modified: Wed May  8 21:09:33 2024, max compression
```

## Comparing `squishyplanet-0.1.0.tar` & `squishyplanet-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-02 20:41:19.539962 squishyplanet-0.1.0/
--rw-r--r--   0 cassese    (501) staff       (20)     1068 2024-03-11 14:22:30.000000 squishyplanet-0.1.0/LICENSE
--rw-r--r--   0 cassese    (501) staff       (20)     2561 2024-05-02 20:41:19.539723 squishyplanet-0.1.0/PKG-INFO
--rw-r--r--   0 cassese    (501) staff       (20)     1740 2024-05-02 05:57:27.000000 squishyplanet-0.1.0/README.md
--rw-r--r--   0 cassese    (501) staff       (20)     1000 2024-05-02 20:39:35.000000 squishyplanet-0.1.0/pyproject.toml
--rw-r--r--   0 cassese    (501) staff       (20)       38 2024-05-02 20:41:19.540005 squishyplanet-0.1.0/setup.cfg
--rw-r--r--   0 cassese    (501) staff       (20)       90 2024-04-20 21:39:16.000000 squishyplanet-0.1.0/setup.py
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-02 20:41:19.534128 squishyplanet-0.1.0/squishyplanet/
--rw-r--r--   0 cassese    (501) staff       (20)      233 2024-04-24 13:17:25.000000 squishyplanet-0.1.0/squishyplanet/__init__.py
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-02 20:41:19.537050 squishyplanet-0.1.0/squishyplanet/engine/
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-02 20:41:19.538594 squishyplanet-0.1.0/squishyplanet/engine/development/
--rw-r--r--   0 cassese    (501) staff       (20)     4637 2024-04-20 21:39:16.000000 squishyplanet-0.1.0/squishyplanet/engine/development/lambertian_reflectance.py
--rw-r--r--   0 cassese    (501) staff       (20)     9098 2024-04-20 21:39:16.000000 squishyplanet-0.1.0/squishyplanet/engine/development/quadratic_limb_darkened_transit.py
--rw-r--r--   0 cassese    (501) staff       (20)    44246 2024-04-20 21:39:16.000000 squishyplanet-0.1.0/squishyplanet/engine/development/terminator.py
--rw-r--r--   0 cassese    (501) staff       (20)     4383 2024-04-24 17:49:36.000000 squishyplanet-0.1.0/squishyplanet/engine/development/test_emission_normalization.py
--rw-r--r--   0 cassese    (501) staff       (20)     3273 2024-04-20 21:39:16.000000 squishyplanet-0.1.0/squishyplanet/engine/greens_basis_transform.py
--rw-r--r--   0 cassese    (501) staff       (20)     5153 2024-04-20 21:39:16.000000 squishyplanet-0.1.0/squishyplanet/engine/kepler.py
--rw-r--r--   0 cassese    (501) staff       (20)     6370 2024-04-26 22:30:04.000000 squishyplanet-0.1.0/squishyplanet/engine/parametric_ellipse.py
--rw-r--r--   0 cassese    (501) staff       (20)    55107 2024-05-02 20:35:36.000000 squishyplanet-0.1.0/squishyplanet/engine/phase_curve_utils.py
--rw-r--r--   0 cassese    (501) staff       (20)     3482 2024-04-20 21:39:16.000000 squishyplanet-0.1.0/squishyplanet/engine/planet_2d.py
--rw-r--r--   0 cassese    (501) staff       (20)    24701 2024-04-30 20:17:55.000000 squishyplanet-0.1.0/squishyplanet/engine/planet_3d.py
--rw-r--r--   0 cassese    (501) staff       (20)    24137 2024-04-26 21:48:50.000000 squishyplanet-0.1.0/squishyplanet/engine/polynomial_limb_darkened_transit.py
--rw-r--r--   0 cassese    (501) staff       (20)    51441 2024-05-02 20:35:36.000000 squishyplanet-0.1.0/squishyplanet/oblate_system.py
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-02 20:41:19.539497 squishyplanet-0.1.0/squishyplanet.egg-info/
--rw-r--r--   0 cassese    (501) staff       (20)     2561 2024-05-02 20:41:19.000000 squishyplanet-0.1.0/squishyplanet.egg-info/PKG-INFO
--rw-r--r--   0 cassese    (501) staff       (20)      877 2024-05-02 20:41:19.000000 squishyplanet-0.1.0/squishyplanet.egg-info/SOURCES.txt
--rw-r--r--   0 cassese    (501) staff       (20)        1 2024-05-02 20:41:19.000000 squishyplanet-0.1.0/squishyplanet.egg-info/dependency_links.txt
--rw-r--r--   0 cassese    (501) staff       (20)       75 2024-05-02 20:41:19.000000 squishyplanet-0.1.0/squishyplanet.egg-info/requires.txt
--rw-r--r--   0 cassese    (501) staff       (20)       14 2024-05-02 20:41:19.000000 squishyplanet-0.1.0/squishyplanet.egg-info/top_level.txt
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-02 20:41:19.539170 squishyplanet-0.1.0/tests/
--rw-r--r--   0 cassese    (501) staff       (20)     3962 2024-04-24 21:24:42.000000 squishyplanet-0.1.0/tests/test_against_jaxoplanet_transit.py
--rw-r--r--   0 cassese    (501) staff       (20)     3787 2024-05-01 21:32:33.000000 squishyplanet-0.1.0/tests/test_oblate_system.py
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-08 21:09:33.197397 squishyplanet-0.1.1/
+-rw-r--r--   0 cassese    (501) staff       (20)     1068 2024-03-11 14:22:30.000000 squishyplanet-0.1.1/LICENSE
+-rw-r--r--   0 cassese    (501) staff       (20)     2582 2024-05-08 21:09:33.197166 squishyplanet-0.1.1/PKG-INFO
+-rw-r--r--   0 cassese    (501) staff       (20)     1761 2024-05-02 22:19:44.000000 squishyplanet-0.1.1/README.md
+-rw-r--r--   0 cassese    (501) staff       (20)     1094 2024-05-08 21:09:27.000000 squishyplanet-0.1.1/pyproject.toml
+-rw-r--r--   0 cassese    (501) staff       (20)       38 2024-05-08 21:09:33.197439 squishyplanet-0.1.1/setup.cfg
+-rw-r--r--   0 cassese    (501) staff       (20)       90 2024-04-20 21:39:16.000000 squishyplanet-0.1.1/setup.py
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-08 21:09:33.193449 squishyplanet-0.1.1/squishyplanet/
+-rw-r--r--   0 cassese    (501) staff       (20)      233 2024-04-24 13:17:25.000000 squishyplanet-0.1.1/squishyplanet/__init__.py
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-08 21:09:33.195825 squishyplanet-0.1.1/squishyplanet/engine/
+-rw-r--r--   0 cassese    (501) staff       (20)        0 2024-05-03 15:21:35.000000 squishyplanet-0.1.1/squishyplanet/engine/__init__.py
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-08 21:09:33.196481 squishyplanet-0.1.1/squishyplanet/engine/development/
+-rw-r--r--   0 cassese    (501) staff       (20)     4637 2024-04-20 21:39:16.000000 squishyplanet-0.1.1/squishyplanet/engine/development/lambertian_reflectance.py
+-rw-r--r--   0 cassese    (501) staff       (20)     9098 2024-04-20 21:39:16.000000 squishyplanet-0.1.1/squishyplanet/engine/development/quadratic_limb_darkened_transit.py
+-rw-r--r--   0 cassese    (501) staff       (20)    44246 2024-04-20 21:39:16.000000 squishyplanet-0.1.1/squishyplanet/engine/development/terminator.py
+-rw-r--r--   0 cassese    (501) staff       (20)     4383 2024-04-24 17:49:36.000000 squishyplanet-0.1.1/squishyplanet/engine/development/test_emission_normalization.py
+-rw-r--r--   0 cassese    (501) staff       (20)     3273 2024-04-20 21:39:16.000000 squishyplanet-0.1.1/squishyplanet/engine/greens_basis_transform.py
+-rw-r--r--   0 cassese    (501) staff       (20)     5153 2024-04-20 21:39:16.000000 squishyplanet-0.1.1/squishyplanet/engine/kepler.py
+-rw-r--r--   0 cassese    (501) staff       (20)     6370 2024-04-26 22:30:04.000000 squishyplanet-0.1.1/squishyplanet/engine/parametric_ellipse.py
+-rw-r--r--   0 cassese    (501) staff       (20)    55767 2024-05-06 18:56:11.000000 squishyplanet-0.1.1/squishyplanet/engine/phase_curve_utils.py
+-rw-r--r--   0 cassese    (501) staff       (20)     3482 2024-04-20 21:39:16.000000 squishyplanet-0.1.1/squishyplanet/engine/planet_2d.py
+-rw-r--r--   0 cassese    (501) staff       (20)    28523 2024-05-07 11:56:22.000000 squishyplanet-0.1.1/squishyplanet/engine/planet_3d.py
+-rw-r--r--   0 cassese    (501) staff       (20)    24392 2024-05-08 21:07:53.000000 squishyplanet-0.1.1/squishyplanet/engine/polynomial_limb_darkened_transit.py
+-rw-r--r--   0 cassese    (501) staff       (20)    51442 2024-05-08 21:07:53.000000 squishyplanet-0.1.1/squishyplanet/oblate_system.py
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-08 21:09:33.196942 squishyplanet-0.1.1/squishyplanet.egg-info/
+-rw-r--r--   0 cassese    (501) staff       (20)     2582 2024-05-08 21:09:33.000000 squishyplanet-0.1.1/squishyplanet.egg-info/PKG-INFO
+-rw-r--r--   0 cassese    (501) staff       (20)      910 2024-05-08 21:09:33.000000 squishyplanet-0.1.1/squishyplanet.egg-info/SOURCES.txt
+-rw-r--r--   0 cassese    (501) staff       (20)        1 2024-05-08 21:09:33.000000 squishyplanet-0.1.1/squishyplanet.egg-info/dependency_links.txt
+-rw-r--r--   0 cassese    (501) staff       (20)       75 2024-05-08 21:09:33.000000 squishyplanet-0.1.1/squishyplanet.egg-info/requires.txt
+-rw-r--r--   0 cassese    (501) staff       (20)       14 2024-05-08 21:09:33.000000 squishyplanet-0.1.1/squishyplanet.egg-info/top_level.txt
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-08 21:09:33.196740 squishyplanet-0.1.1/tests/
+-rw-r--r--   0 cassese    (501) staff       (20)     3962 2024-05-08 21:08:21.000000 squishyplanet-0.1.1/tests/test_against_jaxoplanet_transit.py
+-rw-r--r--   0 cassese    (501) staff       (20)    10438 2024-05-08 21:07:53.000000 squishyplanet-0.1.1/tests/test_oblate_system.py
```

### Comparing `squishyplanet-0.1.0/LICENSE` & `squishyplanet-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.0/PKG-INFO` & `squishyplanet-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squishyplanet
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for dealing with non-spherical exoplanets
 Author-email: Ben Cassese <b.c.cassese@columbia.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/ben-cassese/squishyplanet
 Project-URL: Documentation, https://squishyplanet.readthedocs.io/en/latest/
 Keywords: astronomy,exoplanets
 Classifier: Programming Language :: Python
@@ -64,11 +64,11 @@
     url = {},
     year = 2024,
     month = {},
     publisher = {},
     volume = {},
     number = {},
     author = {},
-    title = {squishyplanet: non-spherical exoplanets in JAX},
+    title = {squishyplanet: modeling transits of non-spherical exoplanets in JAX},
     journal = {}
 }
 ```
```

### Comparing `squishyplanet-0.1.0/README.md` & `squishyplanet-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     url = {},
     year = 2024,
     month = {},
     publisher = {},
     volume = {},
     number = {},
     author = {},
-    title = {squishyplanet: non-spherical exoplanets in JAX},
+    title = {squishyplanet: modeling transits of non-spherical exoplanets in JAX},
     journal = {}
 }
 ```
```

### Comparing `squishyplanet-0.1.0/pyproject.toml` & `squishyplanet-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "squishyplanet"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.9"
 dependencies = [
     "requests",
     "jax",
     "jaxlib",
     "quadax",
     "tqdm",
@@ -34,14 +34,18 @@
 [project.urls]
 Homepage = "https://github.com/ben-cassese/squishyplanet"
 Documentation = "https://squishyplanet.readthedocs.io/en/latest/"
 
 [tool.setuptools]
 include-package-data = true
 
+[tool.setuptools.packages.find]
+where = ["."]
+include = ["squishyplanet", "squishyplanet.*"]
+
 [tool.black]
 line-length = 88
 
 [tool.coverage.run]
 omit = [
     "tests/*",
 ]
```

### Comparing `squishyplanet-0.1.0/squishyplanet/engine/development/lambertian_reflectance.py` & `squishyplanet-0.1.1/squishyplanet/engine/development/lambertian_reflectance.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.0/squishyplanet/engine/development/quadratic_limb_darkened_transit.py` & `squishyplanet-0.1.1/squishyplanet/engine/development/quadratic_limb_darkened_transit.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.0/squishyplanet/engine/development/terminator.py` & `squishyplanet-0.1.1/squishyplanet/engine/development/terminator.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.0/squishyplanet/engine/development/test_emission_normalization.py` & `squishyplanet-0.1.1/squishyplanet/engine/development/test_emission_normalization.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.0/squishyplanet/engine/greens_basis_transform.py` & `squishyplanet-0.1.1/squishyplanet/engine/greens_basis_transform.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.0/squishyplanet/engine/kepler.py` & `squishyplanet-0.1.1/squishyplanet/engine/kepler.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.0/squishyplanet/engine/parametric_ellipse.py` & `squishyplanet-0.1.1/squishyplanet/engine/parametric_ellipse.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.0/squishyplanet/engine/phase_curve_utils.py` & `squishyplanet-0.1.1/squishyplanet/engine/phase_curve_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -905,23 +905,28 @@
 
 
 # still having trouble with this, leaving it for a specific enhancement after 0.1.0
 @jax.jit
 def extended_illumination_reflected_phase_curve(
     sample_radii, sample_thetas, two, three, state, x_c, y_c, z_c, offsets
 ):
+    """
+    WIP, not yet implemented. Hiding behind a NotImplementedError when setting
+    `extended_illumination_npts` to anything greater than 1 when initializing an
+    :class:`OblateSystem` object.
+    """
     pass
-    # # def scan_func(carry, scan_over):
-    # #     two, three = scan_over
-    # #     return None, reflected_phase_curve(
-    # #         sample_radii, sample_thetas, two, three, state, x_c, y_c, z_c
-    # #     )
+    # def scan_func(carry, scan_over):
+    #     two, three = scan_over
+    #     return None, reflected_phase_curve(
+    #         sample_radii, sample_thetas, two, three, state, x_c, y_c, z_c
+    #     )
 
-    # # reflected = jax.lax.scan(scan_func,None,(two, three))[1]
-    # # return jnp.mean(reflected, axis=0)
+    # reflected = jax.lax.scan(scan_func,None,(two, three))[1]
+    # return jnp.mean(reflected, axis=0)
 
     # xo, yo, zo = offsets[..., 0], offsets[..., 1], offsets[..., 2]
     # reflected = jax.vmap(
     #     reflected_phase_curve,
     #     in_axes=(None, None, 0, 0, None, None, None, None, 0, 0, 0),
     # )(sample_radii, sample_thetas, two, three, state, x_c, y_c, z_c, xo, yo, zo)
     # # return jnp.mean(reflected, axis=0)
@@ -1500,14 +1505,26 @@
 @jax.jit
 def stellar_doppler_variations(true_anomalies, stellar_doppler_alpha, period):
     """
     Compute the contributions to a phase curve for a star with Doppler variations.
 
     A simple sinusoid model with a phase of 90 degrees at primary transit meant to
     capture Doppler boosting/flux falling in and out of the bandpass.
+
+    Args:
+        true_anomalies (Array):
+            The true anomaly of the planet at each time step.
+        stellar_doppler_alpha (float):
+            The amplitude of the Doppler variations.
+        period (float):
+            The orbital period of the planet.
+
+    Returns:
+        Array:
+            The contribution to the phase curve from the star's Doppler variations.
     """
 
     amp = stellar_doppler_alpha  # / period**(-1/3)
     phi = true_anomalies - jnp.pi / 2  # orbital phase is zero at primary transit
     phi = jnp.where(phi < 0, phi + 2 * jnp.pi, phi)
     phi = phi / (2 * jnp.pi)
     return amp * jnp.sin(2 * jnp.pi * phi)
@@ -1632,14 +1649,17 @@
             p_zz,
             p_z0,
             p_00,
         )
         surface_star_angle = surface_star_cos_angle(n, x_c, y_c, z_c)
         lamb = lambertian_reflection(surface_star_angle, x, y, z)
 
+        mask = ~(((x) ** 2 + (y) ** 2 < 1) & ((z) < 0))
+        lamb = lamb * mask
+
         # emission stuff
         em = emission_at_timestep(
             x,
             y,
             z,
             transform_matrix,
             state["r"],
```

### Comparing `squishyplanet-0.1.0/squishyplanet/engine/planet_2d.py` & `squishyplanet-0.1.1/squishyplanet/engine/planet_2d.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.1.0/squishyplanet/engine/polynomial_limb_darkened_transit.py` & `squishyplanet-0.1.1/squishyplanet/engine/polynomial_limb_darkened_transit.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,15 +464,20 @@
             state["projected_r"],
             state["projected_f"],
             state["projected_theta"],
             positions[0, :],
             positions[1, :],
         )
         r2 = state["projected_r"] * (1 - state["projected_f"])
-        largest_r = jnp.max(jnp.array([state["projected_r"], r2]))
+        r1 = state["projected_r"]
+        # force the shapes to match: if user inputs a scaler for one value but the
+        # others are still (1,) there'd be a problem. all is fine if they're all
+        # scalars or all arrays though
+        r1 = jnp.ones_like(r2) * r1
+        largest_r = jnp.max(jnp.array([r1, r2]))
 
     else:
         state["prec"] = jnp.where(state["tidally_locked"], state["f"], state["prec"])
 
         # the coefficients of the implicit 3d surface
         three = planet_3d_coeffs(**state)
         # the coefficients of the implicit 2d surface
```

### Comparing `squishyplanet-0.1.0/squishyplanet/oblate_system.py` & `squishyplanet-0.1.1/squishyplanet/oblate_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,15 +496,15 @@
             )
             assert not (
                 self._state["compute_reflected_phase_curve"]
                 | self._state["compute_emitted_phase_curve"]
                 | self._state["compute_stellar_ellipsoidal_variations"]
                 | self._state["compute_stellar_doppler_variations"]
             ), (
-                "parameterize_with_projected_ellipse is incompatible with phase"
+                "parameterize_with_projected_ellipse is incompatible with phase "
                 "curve calculations"
             )
 
             assert self._state["tidally_locked"] == False, (
                 "parameterize_with_projected_ellipse is incompatible with "
                 "tidally_locked=True"
             )
```

### Comparing `squishyplanet-0.1.0/squishyplanet.egg-info/PKG-INFO` & `squishyplanet-0.1.1/squishyplanet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squishyplanet
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for dealing with non-spherical exoplanets
 Author-email: Ben Cassese <b.c.cassese@columbia.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/ben-cassese/squishyplanet
 Project-URL: Documentation, https://squishyplanet.readthedocs.io/en/latest/
 Keywords: astronomy,exoplanets
 Classifier: Programming Language :: Python
@@ -64,11 +64,11 @@
     url = {},
     year = 2024,
     month = {},
     publisher = {},
     volume = {},
     number = {},
     author = {},
-    title = {squishyplanet: non-spherical exoplanets in JAX},
+    title = {squishyplanet: modeling transits of non-spherical exoplanets in JAX},
     journal = {}
 }
 ```
```

### Comparing `squishyplanet-0.1.0/squishyplanet.egg-info/SOURCES.txt` & `squishyplanet-0.1.1/squishyplanet.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 squishyplanet/__init__.py
 squishyplanet/oblate_system.py
 squishyplanet.egg-info/PKG-INFO
 squishyplanet.egg-info/SOURCES.txt
 squishyplanet.egg-info/dependency_links.txt
 squishyplanet.egg-info/requires.txt
 squishyplanet.egg-info/top_level.txt
+squishyplanet/engine/__init__.py
 squishyplanet/engine/greens_basis_transform.py
 squishyplanet/engine/kepler.py
 squishyplanet/engine/parametric_ellipse.py
 squishyplanet/engine/phase_curve_utils.py
 squishyplanet/engine/planet_2d.py
 squishyplanet/engine/planet_3d.py
 squishyplanet/engine/polynomial_limb_darkened_transit.py
```

### Comparing `squishyplanet-0.1.0/tests/test_against_jaxoplanet_transit.py` & `squishyplanet-0.1.1/tests/test_against_jaxoplanet_transit.py`

 * *Files identical despite different names*

