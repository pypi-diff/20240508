# Comparing `tmp/pymrm-1.3.1.tar.gz` & `tmp/pymrm-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymrm-1.3.1.tar", last modified: Fri Apr 19 10:03:53 2024, max compression
+gzip compressed data, was "pymrm-1.3.2.tar", last modified: Wed May  8 19:54:52 2024, max compression
```

## Comparing `pymrm-1.3.1.tar` & `pymrm-1.3.2.tar`

### file list

```diff
@@ -1,32 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 10:03:53.904431 pymrm-1.3.1/
--rw-rw-rw-   0        0        0       57 2024-02-01 11:20:15.000000 pymrm-1.3.1/.gitignore
-drwxrwxrwx   0        0        0        0 2024-04-19 10:03:53.506790 pymrm-1.3.1/.vscode/
--rw-rw-rw-   0        0        0      236 2024-04-17 10:45:15.000000 pymrm-1.3.1/.vscode/settings.json
--rw-rw-rw-   0        0        0      634 2023-07-13 10:36:17.000000 pymrm-1.3.1/Makefile
--rw-rw-rw-   0        0        0     2297 2024-04-19 10:03:53.904431 pymrm-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1461 2024-04-17 14:36:26.000000 pymrm-1.3.1/README.md
--rw-rw-rw-   0        0        0     2002 2024-04-18 08:57:14.000000 pymrm-1.3.1/conf.py
--rw-rw-rw-   0        0        0      107 2023-07-13 10:48:43.000000 pymrm-1.3.1/conf.rst
-drwxrwxrwx   0        0        0        0 2024-04-19 10:03:53.518103 pymrm-1.3.1/exercises/
-drwxrwxrwx   0        0        0        0 2024-04-19 10:03:53.680204 pymrm-1.3.1/exercises/L1/
--rw-rw-rw-   0        0        0   108820 2024-04-18 09:46:22.000000 pymrm-1.3.1/exercises/L1/Exercise 1.1 - First order reaction in a batch reactor.ipynb
--rw-rw-rw-   0        0        0   235060 2024-04-18 22:42:07.000000 pymrm-1.3.1/exercises/L1/Exercise 1.2 - Equilibrium-consecutive reaction system in a batch reactor.ipynb
--rw-rw-rw-   0        0        0    53526 2024-04-18 15:10:57.000000 pymrm-1.3.1/exercises/L1/Exercise 1.3 - Steady-state 1D adiabatic fixed bed reactor model.ipynb
--rw-rw-rw-   0        0        0      526 2024-04-18 11:22:50.000000 pymrm-1.3.1/exercises/debugging_pymrm_local.ipynb
--rwxrwxrwx   0        0        0      800 2023-07-13 10:36:17.000000 pymrm-1.3.1/make.bat
--rw-rw-rw-   0        0        0       49 2023-07-13 10:56:28.000000 pymrm-1.3.1/modules.rst
--rw-rw-rw-   0        0        0      243 2024-04-18 19:29:56.000000 pymrm-1.3.1/mrm_environment.yml
--rw-rw-rw-   0        0        0      111 2024-04-18 19:29:43.000000 pymrm-1.3.1/mrm_requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-19 10:03:53.863604 pymrm-1.3.1/pymrm/
--rw-rw-rw-   0        0        0      389 2024-04-17 13:10:51.000000 pymrm-1.3.1/pymrm/__init__.py
--rw-rw-rw-   0        0        0    50806 2024-04-18 15:21:55.000000 pymrm-1.3.1/pymrm/pymrm.py
--rw-rw-rw-   0        0        0   702896 2024-04-18 22:28:18.000000 pymrm-1.3.1/pymrm/pymrm_examples.ipynb
-drwxrwxrwx   0        0        0        0 2024-04-19 10:03:53.904431 pymrm-1.3.1/pymrm.egg-info/
--rw-rw-rw-   0        0        0     2297 2024-04-19 10:03:53.000000 pymrm-1.3.1/pymrm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      651 2024-04-19 10:03:53.000000 pymrm-1.3.1/pymrm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 10:03:53.000000 pymrm-1.3.1/pymrm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-19 10:03:53.000000 pymrm-1.3.1/pymrm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-19 10:03:53.000000 pymrm-1.3.1/pymrm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1060 2024-04-18 15:44:05.000000 pymrm-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 10:03:53.904431 pymrm-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      121 2023-07-13 10:48:43.000000 pymrm-1.3.1/test_mrm.rst
+drwxrwxrwx   0        0        0        0 2024-05-08 19:54:52.558676 pymrm-1.3.2/
+-rw-rw-rw-   0        0        0       57 2024-02-01 11:20:15.000000 pymrm-1.3.2/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-08 19:54:52.027504 pymrm-1.3.2/.vscode/
+-rw-rw-rw-   0        0        0      236 2024-04-17 10:45:15.000000 pymrm-1.3.2/.vscode/settings.json
+-rw-rw-rw-   0        0        0      634 2023-07-13 10:36:17.000000 pymrm-1.3.2/Makefile
+-rw-rw-rw-   0        0        0     2297 2024-05-08 19:54:52.557676 pymrm-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1461 2024-04-17 14:36:26.000000 pymrm-1.3.2/README.md
+-rw-rw-rw-   0        0        0     2002 2024-04-18 08:57:14.000000 pymrm-1.3.2/conf.py
+-rw-rw-rw-   0        0        0      107 2023-07-13 10:48:43.000000 pymrm-1.3.2/conf.rst
+drwxrwxrwx   0        0        0        0 2024-05-08 19:54:52.293623 pymrm-1.3.2/examples/
+-rw-rw-rw-   0        0        0    52232 2024-05-03 13:52:02.000000 pymrm-1.3.2/examples/L3_convection_diffusion_ex3.4.ipynb
+-rw-rw-rw-   0        0        0    72097 2024-05-01 15:57:28.000000 pymrm-1.3.2/examples/L3_demo_diffusion_reaction.ipynb
+-rw-rw-rw-   0        0        0    72371 2024-05-01 15:56:54.000000 pymrm-1.3.2/examples/L3_demo_mrm_implementation_as_class.ipynb
+-rw-rw-rw-   0        0        0    93517 2024-05-03 19:56:03.000000 pymrm-1.3.2/examples/L3_multicomponent_diffusion_ex3.2.ipynb
+-rw-rw-rw-   0        0        0    35311 2024-05-03 13:21:05.000000 pymrm-1.3.2/examples/L3_particle_model_ex3.5.ipynb
+-rw-rw-rw-   0        0        0    19000 2024-05-03 20:56:31.000000 pymrm-1.3.2/examples/L3_particle_model_non_linear.ipynb
+-rw-rw-rw-   0        0        0    21475 2024-05-08 10:51:08.000000 pymrm-1.3.2/examples/L5_convection_diffusion_2D.ipynb
+-rw-rw-rw-   0        0        0    12885 2024-05-08 18:45:38.000000 pymrm-1.3.2/examples/L5_demo.ipynb
+-rw-rw-rw-   0        0        0   116764 2024-04-24 07:32:19.000000 pymrm-1.3.2/examples/annular_flow_reaction.ipynb
+-rw-rw-rw-   0        0        0      526 2024-04-18 11:22:50.000000 pymrm-1.3.2/examples/debugging_pymrm_local.ipynb
+-rw-rw-rw-   0        0        0    38100 2024-05-08 19:40:14.000000 pymrm-1.3.2/examples/different_diffusion_coefficients.ipynb
+-rw-rw-rw-   0        0        0   702981 2024-04-20 14:00:38.000000 pymrm-1.3.2/examples/pymrm_examples.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-08 19:54:51.929590 pymrm-1.3.2/exercises/
+drwxrwxrwx   0        0        0        0 2024-05-08 19:54:52.417149 pymrm-1.3.2/exercises/L1/
+-rw-rw-rw-   0        0        0   108821 2024-04-22 15:15:06.000000 pymrm-1.3.2/exercises/L1/Exercise 1.1 - First order reaction in a batch reactor.ipynb
+-rw-rw-rw-   0        0        0   235059 2024-04-23 07:15:48.000000 pymrm-1.3.2/exercises/L1/Exercise 1.2 - Equilibrium-consecutive reaction system in a batch reactor.ipynb
+-rw-rw-rw-   0        0        0   120538 2024-04-22 15:15:09.000000 pymrm-1.3.2/exercises/L1/Exercise 1.3 - Steady-state 1D adiabatic fixed bed reactor model.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-08 19:54:52.443357 pymrm-1.3.2/exercises/L2/
+-rw-rw-rw-   0        0        0    97596 2024-04-29 20:12:56.000000 pymrm-1.3.2/exercises/L2/Exercise 2.1 - Single component convection.ipynb
+-rw-rw-rw-   0        0        0     3192 2024-04-25 20:59:16.000000 pymrm-1.3.2/exercises/L2/Exercise 2.1 - Single component convection.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:54:52.476962 pymrm-1.3.2/exercises/L3/
+-rw-rw-rw-   0        0        0    23669 2024-05-01 11:30:11.000000 pymrm-1.3.2/exercises/L3/Exercise 3.1 - one component 1D diffusion.ipynb
+-rw-rw-rw-   0        0        0   109502 2024-05-01 22:31:57.000000 pymrm-1.3.2/exercises/L3/Exercise 3.2 - counter diffusion.ipynb
+-rw-rw-rw-   0        0        0    58536 2024-04-28 23:25:55.000000 pymrm-1.3.2/exercises/L3/Exercise 3.3 - Multi-component 1D counter-current convection with reaction.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-08 19:54:52.493476 pymrm-1.3.2/exercises/L4/
+-rw-rw-rw-   0        0        0    38580 2024-05-02 08:34:30.000000 pymrm-1.3.2/exercises/L4/Exercise 4.1 - Counter-current column processes.ipynb
+-rw-rw-rw-   0        0        0     6148 2024-05-03 07:45:07.000000 pymrm-1.3.2/exercises/L4/Exercise 4.2 - Reactor model for heterogeneous bubble columns.ipynb
+-rwxrwxrwx   0        0        0      800 2023-07-13 10:36:17.000000 pymrm-1.3.2/make.bat
+-rw-rw-rw-   0        0        0       49 2023-07-13 10:56:28.000000 pymrm-1.3.2/modules.rst
+-rw-rw-rw-   0        0        0      243 2024-05-08 19:51:43.000000 pymrm-1.3.2/mrm_environment.yml
+-rw-rw-rw-   0        0        0     2528 2024-04-19 14:16:59.000000 pymrm-1.3.2/mrm_python_install.md
+-rw-rw-rw-   0        0        0      111 2024-05-08 19:51:29.000000 pymrm-1.3.2/mrm_requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 19:54:52.514702 pymrm-1.3.2/pymrm/
+-rw-rw-rw-   0        0        0      389 2024-04-17 13:10:51.000000 pymrm-1.3.2/pymrm/__init__.py
+-rw-rw-rw-   0        0        0    51028 2024-05-08 19:11:07.000000 pymrm-1.3.2/pymrm/pymrm.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:54:52.555766 pymrm-1.3.2/pymrm.egg-info/
+-rw-rw-rw-   0        0        0     2297 2024-05-08 19:54:51.000000 pymrm-1.3.2/pymrm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1571 2024-05-08 19:54:51.000000 pymrm-1.3.2/pymrm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 19:54:51.000000 pymrm-1.3.2/pymrm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-08 19:54:51.000000 pymrm-1.3.2/pymrm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-08 19:54:51.000000 pymrm-1.3.2/pymrm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1060 2024-05-08 19:42:09.000000 pymrm-1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 19:54:52.558676 pymrm-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      121 2023-07-13 10:48:43.000000 pymrm-1.3.2/test_mrm.rst
```

### Comparing `pymrm-1.3.1/Makefile` & `pymrm-1.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.1/PKG-INFO` & `pymrm-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymrm
-Version: 1.3.1
+Version: 1.3.2
 Summary: Functions for multiphase reactor modeling
 Author-email: "E.A.J.F. Peters" <e.a.j.f.peters@tue.nl>, "M. van Sint Annaland" <M.v.SintAnnaland@tue.nl>, "M. Galanti" <m.galanti@tue.nl>, "D.R. Rieder" <d.r.rieder@tue.nl>
 Maintainer-email: "E.A.J.F. Peters" <e.a.j.f.peters@tue.nl>
 Project-URL: Homepage, https://gitlab.tue.nl/SMM/research_projects/eajfpeters/pymrm/
 Project-URL: Repository, https://gitlab.tue.nl/SMM/research_projects/eajfpeters/pymrm/
 Keywords: MRM,modeling,multiphase,diffusion,convection
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pymrm-1.3.1/README.md` & `pymrm-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.1/conf.py` & `pymrm-1.3.2/conf.py`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.1/exercises/L1/Exercise 1.1 - First order reaction in a batch reactor.ipynb` & `pymrm-1.3.2/exercises/L1/Exercise 1.1 - First order reaction in a batch reactor.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333334%*

 * *Differences: {"'cells'": "{2: {'source': ['## a) Forward Euler Discretization']}}"}*

```diff
@@ -28,15 +28,15 @@
                 "dt = 0.1           # time step [s]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# a) Forward Euler Discretization"
+                "## a) Forward Euler Discretization"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
```

### Comparing `pymrm-1.3.1/exercises/L1/Exercise 1.2 - Equilibrium-consecutive reaction system in a batch reactor.ipynb` & `pymrm-1.3.2/exercises/L1/Exercise 1.2 - Equilibrium-consecutive reaction system in a batch reactor.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99875%*

 * *Differences: {"'cells'": "{7: {'execution_count': 4}}"}*

```diff
@@ -204,15 +204,15 @@
             "metadata": {},
             "source": [
                 "## c) Backward Euler Discretization "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "t: 0.0000, c: [1.000000000 0.000000000 0.000000000]\n",
```

### Comparing `pymrm-1.3.1/exercises/debugging_pymrm_local.ipynb` & `pymrm-1.3.2/examples/debugging_pymrm_local.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.1/make.bat` & `pymrm-1.3.2/make.bat`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.1/pymrm/pymrm.py` & `pymrm-1.3.2/pymrm/pymrm.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,35 +558,39 @@
             math.prod(shape_f_t), math.prod(shape_t)))
         Conv.sort_indices()
 
     conv_bc = csc_array((values_bc.ravel(), i_f_bc.ravel(), [
                          0, i_f_bc.size]), shape=(math.prod(shape_f_t),1))
     return Conv, conv_bc
 
-def construct_coefficient_matrix(coeffs, shape=None):
+def construct_coefficient_matrix(coeffs, shape=None, axis=None):
     """
     Construct a diagional matrix with coefficients on its diagonal.
     This is useful to create a matrix containing transport coefficients 
     from a field contained in a ndarray. 
 
     Args:
         coeffs (ndarray): values of the coefficients in a field
         shape (tuple, optional): Shape of the multidimensional field. With this option, some of the dimensions of coeffs can be choosen singleton.
+        axis: In case of broadcasting along 'axis' used shape will be shape[axis+1] (can be useful for face-values)
 
     Returns:
         csc_array: matrix Coeff with coefficients on its diagonal.
-        csc_array: The conv_bc matrix.
     """
     if(shape == None):
         shape = coeffs.shape
         Coeff = csc_array(diags(coeffs.flatten(), format='csc'))
     else:
-        reps = [shape[i] // coeffs.shape[i] if i < len(coeffs.shape) else shape[i] for i in range(len(shape))]
-        coeffs_loc = np.tile(coeffs, reps)
-        Coeff = csc_array(diags(coeffs_loc.flatten(), format='csc_array'))
+        shape = list(shape)
+        if (axis != None):
+            shape[axis] += 1
+        coeffs_copy = np.array(coeffs)
+        reps = [shape[i] // coeffs_copy.shape[i] if i < len(coeffs_copy.shape) else shape[i] for i in range(len(shape))]
+        coeffs_copy = np.tile(coeffs_copy, reps)
+        Coeff = csc_array(diags(coeffs_copy.flatten(), format='csc'))
     return Coeff
 
 def numjac_local(f, c, eps_jac=1e-6, axis=-1):
     """
     Compute the local numerical Jacobian matrix and function values for the given function and initial values.
     
     The function 'f' is assumed to be local, meaning it can be dependent on other components in the array along the 'axis' dimension.
```

### Comparing `pymrm-1.3.1/pymrm/pymrm_examples.ipynb` & `pymrm-1.3.2/examples/pymrm_examples.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993432971014493%*

 * *Differences: {"'cells'": "{23: {'execution_count': 32, 'source': {insert: [(13, 'def wrapper_fun(x, "*

 * *            "*args):\\n'), (14, '    g, Jac = fun(x, *args)\\n'), (15, '    return g, "*

 * *            "Jac.toarray()\\n'), (16, '\\n'), (17, 'sol = optim.root(wrapper_fun, x0, args=args, "*

 * *            "jac=True)\\n')], delete: [13]}}}"}*

```diff
@@ -921,15 +921,15 @@
                 "cbar_ax = fig.add_axes([0.92, ax.get_position().y0, 0.02, ax.get_position().y1-ax.get_position().y0])  # Adjust the parameters as needed [left, bottom, width, height]\n",
                 "plt.colorbar(contour, cax=cbar_ax)\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 32,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Solution SciPy root:\n",
@@ -970,15 +970,19 @@
                 "    return g,Jac\n",
                 "\n",
                 "# Initial guess\n",
                 "x0 = np.array([0.5, 0.5])\n",
                 "args = (2,3)\n",
                 "\n",
                 "# Solve the system\n",
-                "sol = optim.root(lambda x: (fun(x, *args)[0], fun(x, *args)[1].toarray()), x0, jac=True)\n",
+                "def wrapper_fun(x, *args):\n",
+                "    g, Jac = fun(x, *args)\n",
+                "    return g, Jac.toarray()\n",
+                "\n",
+                "sol = optim.root(wrapper_fun, x0, args=args, jac=True)\n",
                 "print(f\"Solution SciPy root:\\n {sol}\\n\")\n",
                 "\n",
                 "sol2 = mrm.newton(fun, x0, args=args)\n",
                 "print(f\"Solution pymrm newton:\\n {sol2}\\n\")"
             ]
         }
     ],
```

### Comparing `pymrm-1.3.1/pymrm.egg-info/PKG-INFO` & `pymrm-1.3.2/pymrm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymrm
-Version: 1.3.1
+Version: 1.3.2
 Summary: Functions for multiphase reactor modeling
 Author-email: "E.A.J.F. Peters" <e.a.j.f.peters@tue.nl>, "M. van Sint Annaland" <M.v.SintAnnaland@tue.nl>, "M. Galanti" <m.galanti@tue.nl>, "D.R. Rieder" <d.r.rieder@tue.nl>
 Maintainer-email: "E.A.J.F. Peters" <e.a.j.f.peters@tue.nl>
 Project-URL: Homepage, https://gitlab.tue.nl/SMM/research_projects/eajfpeters/pymrm/
 Project-URL: Repository, https://gitlab.tue.nl/SMM/research_projects/eajfpeters/pymrm/
 Keywords: MRM,modeling,multiphase,diffusion,convection
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pymrm-1.3.1/pyproject.toml` & `pymrm-1.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pymrm"
-version = "1.3.1"
+version = "1.3.2"
 dependencies = [
     "numpy>=1.26",
     "scipy>=1.13",
 ]
 authors = [
     {name = "E.A.J.F. Peters", email = "e.a.j.f.peters@tue.nl"},
     {name = "M. van Sint Annaland", email= "M.v.SintAnnaland@tue.nl"},
```

