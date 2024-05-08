# Comparing `tmp/OasisX-1.0.0.tar.gz` & `tmp/oasisx-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OasisX-1.0.0.tar", last modified: Tue Dec  5 10:01:29 2023, max compression
+gzip compressed data, was "oasisx-1.1.0.tar", last modified: Wed May  8 14:20:29 2024, max compression
```

## Comparing `OasisX-1.0.0.tar` & `oasisx-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 10:01:29.593374 OasisX-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-12-05 10:01:17.000000 OasisX-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2023-12-05 10:01:29.593374 OasisX-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-05 10:01:17.000000 OasisX-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-12-05 10:01:17.000000 OasisX-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-05 10:01:29.593374 OasisX-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 10:01:29.589374 OasisX-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 10:01:29.589374 OasisX-1.0.0/src/OasisX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2023-12-05 10:01:29.000000 OasisX-1.0.0/src/OasisX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      476 2023-12-05 10:01:29.000000 OasisX-1.0.0/src/OasisX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 10:01:29.000000 OasisX-1.0.0/src/OasisX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-05 10:01:29.000000 OasisX-1.0.0/src/OasisX.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-05 10:01:29.000000 OasisX-1.0.0/src/OasisX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-05 10:01:29.000000 OasisX-1.0.0/src/OasisX.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 10:01:29.589374 OasisX-1.0.0/src/oasisx/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-12-05 10:01:17.000000 OasisX-1.0.0/src/oasisx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-12-05 10:01:17.000000 OasisX-1.0.0/src/oasisx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8925 2023-12-05 10:01:17.000000 OasisX-1.0.0/src/oasisx/bcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    26434 2023-12-05 10:01:17.000000 OasisX-1.0.0/src/oasisx/fracstep.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2023-12-05 10:01:17.000000 OasisX-1.0.0/src/oasisx/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2023-12-05 10:01:17.000000 OasisX-1.0.0/src/oasisx/ksp.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-05 10:01:17.000000 OasisX-1.0.0/src/oasisx/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-12-05 10:01:17.000000 OasisX-1.0.0/src/oasisx/mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 10:01:29.589374 OasisX-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2023-12-05 10:01:17.000000 OasisX-1.0.0/test/test_bcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2023-12-05 10:01:17.000000 OasisX-1.0.0/test/test_projector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2023-12-05 10:01:17.000000 OasisX-1.0.0/test/test_tentative_velocity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:29.915553 oasisx-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-08 14:20:21.000000 oasisx-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-08 14:20:29.915553 oasisx-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-08 14:20:21.000000 oasisx-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-08 14:20:21.000000 oasisx-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:20:29.915553 oasisx-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:29.911553 oasisx-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:29.915553 oasisx-1.1.0/src/OasisX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-08 14:20:29.000000 oasisx-1.1.0/src/OasisX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-08 14:20:29.000000 oasisx-1.1.0/src/OasisX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:20:29.000000 oasisx-1.1.0/src/OasisX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 14:20:29.000000 oasisx-1.1.0/src/OasisX.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-08 14:20:29.000000 oasisx-1.1.0/src/OasisX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 14:20:29.000000 oasisx-1.1.0/src/OasisX.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:29.915553 oasisx-1.1.0/src/oasisx/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-08 14:20:21.000000 oasisx-1.1.0/src/oasisx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-08 14:20:21.000000 oasisx-1.1.0/src/oasisx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-05-08 14:20:21.000000 oasisx-1.1.0/src/oasisx/bcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28354 2024-05-08 14:20:21.000000 oasisx-1.1.0/src/oasisx/fracstep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-08 14:20:21.000000 oasisx-1.1.0/src/oasisx/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-08 14:20:21.000000 oasisx-1.1.0/src/oasisx/ksp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-08 14:20:21.000000 oasisx-1.1.0/src/oasisx/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-08 14:20:21.000000 oasisx-1.1.0/src/oasisx/mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:29.915553 oasisx-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-08 14:20:21.000000 oasisx-1.1.0/test/test_bcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-08 14:20:21.000000 oasisx-1.1.0/test/test_projector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-08 14:20:21.000000 oasisx-1.1.0/test/test_tentative_velocity.py
```

### Comparing `OasisX-1.0.0/LICENSE` & `oasisx-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OasisX-1.0.0/PKG-INFO` & `oasisx-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OasisX
-Version: 1.0.0
+Version: 1.1.0
 Summary: A modern implementation of Oasis
 Author-email: "Jørgen S. Dokken" <dokken@simula.no>
 License: MIT License
         
         Copyright (c) 2022 Jørgen Schartum Dokken
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,20 +25,21 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: fenics-dolfinx>=0.7.0
+Requires-Dist: fenics-dolfinx>=0.8.0
 Provides-Extra: test
-Requires-Dist: flake8; extra == "test"
+Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: isort; extra == "test"
 Provides-Extra: docs
 Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
 Requires-Dist: seaborn; extra == "docs"
 Requires-Dist: docutils==0.17.1; extra == "docs"
 Provides-Extra: binder
 Requires-Dist: jupyterlab; extra == "binder"
@@ -55,9 +56,13 @@
 
 ### Requirements
 
 [DOLFINx](https://github.com/FEniCS/dolfinx/), which can be installed through apt, conda, docker, spack or manually, see: [DOLFINx installation instructions](https://github.com/FEniCS/dolfinx/#installation) for details
 
 Once you have DOLFINx installed, install a compatible version of Oasisx:
 
-- `python3 -m pip install oasisx` (compatible with version 0.7.2 of DOLFINx)
-- `python3 -m pip install git+https://github.com/computationalPhysiology/oasisx@main` (compatible with version 0.7.2 of DOLFINx)
+- `python3 -m pip install oasisx` (compatible with version 0.8.0 of DOLFINx)
+- `python3 -m pip install git+https://github.com/computationalPhysiology/oasisx@main` (compatible with version the main branch of DOLFINx)
+
+#### Other version compatability
+- oasisx v1.0.0 is compatible with DOLFINx v0.7.x
+- The main branch of oasisx aim to be compatible with the main branch of DOLFINx
```

### Comparing `OasisX-1.0.0/pyproject.toml` & `oasisx-1.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=64.4.0", "wheel"]
 
 
 [project]
 name = "OasisX"
 authors = [{ name = "Jørgen S. Dokken", email = "dokken@simula.no" }]
-version = "1.0.0"
+version = "1.1.0"
 description = "A modern implementation of Oasis"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
-dependencies = ['numpy', 'fenics-dolfinx>=0.7.0']
+dependencies = ['numpy', 'fenics-dolfinx>=0.8.0']
 
 [project.scripts]
 oasisx = "oasisx.__main__:main"
 
 [project.optional-dependencies]
-test = ["flake8", "mypy", "pytest", "pytest-cov"]
+test = ["ruff", "mypy", "pytest", "pytest-cov", "isort"]
 
 docs = [
     "jupyter-book",
     "jupytext",
     "seaborn",
     "docutils==0.17.1",
     # Temporary pin due to https://sourceforge.net/p/docutils/patches/195/
@@ -37,7 +37,48 @@
 addopts = "--cov=oasisx --cov-report html --cov-append --cov-report term-missing -v"
 testpaths = ["test"]
 
 
 [tool.jupytext.formats]
 "docs/" = "ipynb"
 "demo/" = "py:light"
+
+
+[tool.ruff]
+src = ["src", "test", "demo"]
+line-length = 100
+indent-width = 4
+
+[tool.ruff.lint]
+select = [
+    # Pyflakes
+    "F",
+    # Pycodestyle
+    "E",
+    "W",
+    # isort
+    "I001",
+]
+
+
+[tool.ruff.lint.isort]
+known-first-party = ["oasisx"]
+known-third-party = [
+    "basix",
+    "dolfinx",
+    "ffcx",
+    "ufl",
+    "gmsh",
+    "numpy",
+    "pytest",
+]
+section-order = [
+    "future",
+    "standard-library",
+    "mpi",
+    "third-party",
+    "first-party",
+    "local-folder",
+]
+
+[tool.ruff.lint.isort.sections]
+"mpi" = ["mpi4py", "petsc4py"]
```

### Comparing `OasisX-1.0.0/src/OasisX.egg-info/PKG-INFO` & `oasisx-1.1.0/src/OasisX.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OasisX
-Version: 1.0.0
+Version: 1.1.0
 Summary: A modern implementation of Oasis
 Author-email: "Jørgen S. Dokken" <dokken@simula.no>
 License: MIT License
         
         Copyright (c) 2022 Jørgen Schartum Dokken
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,20 +25,21 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: fenics-dolfinx>=0.7.0
+Requires-Dist: fenics-dolfinx>=0.8.0
 Provides-Extra: test
-Requires-Dist: flake8; extra == "test"
+Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: isort; extra == "test"
 Provides-Extra: docs
 Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
 Requires-Dist: seaborn; extra == "docs"
 Requires-Dist: docutils==0.17.1; extra == "docs"
 Provides-Extra: binder
 Requires-Dist: jupyterlab; extra == "binder"
@@ -55,9 +56,13 @@
 
 ### Requirements
 
 [DOLFINx](https://github.com/FEniCS/dolfinx/), which can be installed through apt, conda, docker, spack or manually, see: [DOLFINx installation instructions](https://github.com/FEniCS/dolfinx/#installation) for details
 
 Once you have DOLFINx installed, install a compatible version of Oasisx:
 
-- `python3 -m pip install oasisx` (compatible with version 0.7.2 of DOLFINx)
-- `python3 -m pip install git+https://github.com/computationalPhysiology/oasisx@main` (compatible with version 0.7.2 of DOLFINx)
+- `python3 -m pip install oasisx` (compatible with version 0.8.0 of DOLFINx)
+- `python3 -m pip install git+https://github.com/computationalPhysiology/oasisx@main` (compatible with version the main branch of DOLFINx)
+
+#### Other version compatability
+- oasisx v1.0.0 is compatible with DOLFINx v0.7.x
+- The main branch of oasisx aim to be compatible with the main branch of DOLFINx
```

### Comparing `OasisX-1.0.0/src/oasisx/bcs.py` & `oasisx-1.1.0/src/oasisx/bcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 # Copyright (C) 2022 Jørgen Schartum Dokken
 #
 # This file is part of Oasisx
 # SPDX-License-Identifier:    MIT
 
 
 from enum import Enum
-from typing import Callable, Optional, Tuple, Union, List
-from dolfinx import default_scalar_type
+from typing import Callable, List, Optional, Tuple, Union
+
+from petsc4py import PETSc as _PETSc
+
 import dolfinx.fem as _fem
 import dolfinx.mesh as _dmesh
 import numpy as np
 import numpy.typing as npt
-from petsc4py import PETSc as _PETSc
 import ufl
+from dolfinx import default_scalar_type
+
 __all__ = ["DirichletBC", "PressureBC", "LocatorMethod"]
 
 
 class LocatorMethod(Enum):
     """
     Search methods for Dirichlet BCs
     """
+
     GEOMETRICAL = 1
     TOPOLOGICAL = 2
 
 
 LocatorMethod.TOPOLOGICAL.__doc__ = "Topogical search for dofs"
 LocatorMethod.GEOMETRICAL.__doc__ = "Geometrical search for dofs"
 
 
-class DirichletBC():
+class DirichletBC:
     """
     Create a Dirichlet boundary condition based on topological or geometrical info from the mesh
     This boundary condtion should only be used for velocity function spaces.
 
     Args:
         value: The value the degrees of freedom should have. It can be a float, a
             `dolfinx.fem.Constant` or a lambda-function.
@@ -58,59 +62,68 @@
         **Assigning a geometrical condition**
 
         .. highlight:: python
         .. code-block:: python
 
             bc = DirchletBC(dolfinx.fem.Constant(mesh, 3.), lambda x: np.isclose(x[0]))
     """
+
     _method: LocatorMethod
     _entities: npt.NDArray[np.int32]  # List of entities local to process
     _e_dim: int  # Dimension of entities
 
     _locator: Callable[[npt.NDArray[np.float64]], npt.NDArray[np.bool_]]
     _dofs: npt.NDArray[np.int32]
-    _value: Union[np.float64, _fem.Constant, Callable[[
-        npt.NDArray[np.float64]], npt.NDArray[np.float64]]]
+    _value: Union[
+        np.float64,
+        _fem.Constant,
+        Callable[[npt.NDArray[np.float64]], npt.NDArray[np.float64]],
+    ]
     _bc: _fem.DirichletBC
     _u: Optional[_fem.Function]
 
     __slots__ = tuple(__annotations__)
 
     def __init__(
-        self, value: Union[np.float64, _fem.Constant,
-                           Callable[[npt.NDArray[np.float64]], npt.NDArray[np.float64]]],
+        self,
+        value: Union[
+            np.float64,
+            _fem.Constant,
+            Callable[[npt.NDArray[np.float64]], npt.NDArray[np.float64]],
+        ],
         method: LocatorMethod,
-        marker: Union[Tuple[_dmesh.MeshTags, np.int32],
-                      Callable[[npt.NDArray[np.float64]], npt.NDArray[np.bool_]]]
+        marker: Union[
+            Tuple[_dmesh.MeshTags, np.int32],
+            Callable[[npt.NDArray[np.float64]], npt.NDArray[np.bool_]],
+        ],
     ):
         if method == LocatorMethod.GEOMETRICAL:
             self._method = method
             setattr(self, "_locator", marker)
         elif method == LocatorMethod.TOPOLOGICAL:
             self._method = method
             self._entities = marker[0].find(marker[1])  # type: ignore
             self._e_dim = marker[0].dim  # type:ignore
         self._value = value
 
     def set_dofs(self, dofs: npt.NDArray[np.int32]):
         self._dofs = dofs
 
-    def _locate_dofs(self, V: _fem.FunctionSpaceBase):
+    def _locate_dofs(self, V: _fem.FunctionSpace):
         """
         Locate all dofs satisfying the criterion
         """
         if self._method == LocatorMethod.GEOMETRICAL:
             self._dofs = _fem.locate_dofs_geometrical(V, self._locator)  # type:ignore
         elif self._method == LocatorMethod.TOPOLOGICAL:
+            V.mesh.topology.create_connectivity(self._e_dim, V.mesh.topology.dim)
             self._dofs = _fem.locate_dofs_topological(V, self._e_dim, self._entities)
 
-    def create_bc(self, V: _fem.FunctionSpaceBase):
-        """
-
-        """
+    def create_bc(self, V: _fem.FunctionSpace):
+        """ """
         if not hasattr(self, "_dofs"):
             self._locate_dofs(V)
 
         try:
             self._bc = _fem.dirichletbc(self._value, self._dofs, V)  # type:ignore
         except AttributeError:
             self._u = _fem.Function(V)
@@ -127,16 +140,15 @@
     def apply(self, x: _PETSc.Vec):  # type: ignore
         """
         Apply boundary condition to a PETSc vector
         """
         _fem.petsc.set_bc(x, [self._bc])
 
 
-class PressureBC():
-
+class PressureBC:
     """
     Create a Pressure boundary condition (natural bc) based on a set of facets of a
     mesh and some value.
 
     Args:
         value: The value the degrees of freedom should have. It can be a float, a
             `dolfinx.fem.Constant` or a lambda-function. If `value` is a lambda-function it
@@ -169,67 +181,81 @@
 
             p = OutletPressure(0.)
             entities = np.array([0,3,8],dtype=np.int32)
             values = np.full_like(entities, 2, dtype=np.int32)
             mt  = dolfinx.fem.meshtags(mesh, mesh.topology.dim-1, entities, values)
             bc = PressureBC(p,  (mt, 2))
 
-            Q = dolfinx.fem.FunctionSpace(mesh, ("Lagrange", 1))
+            Q = dolfinx.fem.functionspace(mesh, ("Lagrange", 1))
             # Create appropriate structures for assigning bcs
             bc.create_bc(Q)
             # Update time in bc
             p.t = 1
-        """
+    """
 
     _subdomain_data: _dmesh.MeshTags
     _subdomain_id: Union[np.int32, Tuple[np.int32]]
-    _value: Union[np.float64, _fem.Constant,
-                  Callable[[npt.NDArray[np.float64]], npt.NDArray[np.float64]]]
+    _value: Union[
+        np.float64,
+        _fem.Constant,
+        Callable[[npt.NDArray[np.float64]], npt.NDArray[np.float64]],
+    ]
     _u: _fem.Function
     _rhs: List[ufl.form.Form]
     _bc: _fem.DirichletBC
     __slots__ = tuple(__annotations__)
 
-    def __init__(self, value: Union[np.float64, _fem.Constant,
-                                    Callable[[npt.NDArray[np.float64]], npt.NDArray[np.float64]]],
-                 marker: Tuple[_dmesh.MeshTags, Union[np.int32, Tuple[np.int32]]]):
+    def __init__(
+        self,
+        value: Union[
+            np.float64,
+            _fem.Constant,
+            Callable[[npt.NDArray[np.float64]], npt.NDArray[np.float64]],
+        ],
+        marker: Tuple[_dmesh.MeshTags, Union[np.int32, Tuple[np.int32]]],
+    ):
         self._subdomain_data, self._subdomain_id = marker
         self._value = value
 
-    def create_bcs(self, V: _fem.FunctionSpaceBase, Q: _fem.FunctionSpaceBase):
+    def create_bcs(self, V: _fem.FunctionSpace, Q: _fem.FunctionSpace):
         """
         Create boundary conditions for the pressure conditions for a given velocity and
         pressure function space
 
         Args:
             V: The velocity function space
             Q: The pressure function space
         """
         mesh = V.mesh
         assert mesh.topology == self._subdomain_data.topology
         # Create pressure "Neumann" condition
         v = ufl.TestFunction(V)
-        ds = ufl.Measure("ds", domain=mesh, subdomain_data=self._subdomain_data,
-                         subdomain_id=self._subdomain_id)
+        ds = ufl.Measure(
+            "ds",
+            domain=mesh,
+            subdomain_data=self._subdomain_data,
+            subdomain_id=self._subdomain_id,
+        )
         n = ufl.FacetNormal(mesh)
         try:
             rhs = [self._value * n_i * v.dx(i) * ds for i, n_i in enumerate(n)]
         except TypeError:
             # If input is lambda function interpolate into local function
             self._u = _fem.Function(Q)
             self._u.interpolate(self._value)  # type: ignore
             rhs = [self._u * n_i * v.dx(i) * ds for i, n_i in enumerate(n)]
 
         # Create rhs contribution from natural boundary condition
         self._rhs = rhs
 
         # Create homogenuous boundary condition for pressure correction eq
         boundary_facets = self._subdomain_data.find(self._subdomain_id)  # type: ignore
-        dofs = _fem.locate_dofs_topological(Q, mesh.topology.dim-1, boundary_facets)
-        self._bc = _fem.dirichletbc(default_scalar_type(0.), dofs, Q)
+        mesh.topology.create_connectivity(mesh.topology.dim - 1, mesh.topology.dim)
+        dofs = _fem.locate_dofs_topological(Q, mesh.topology.dim - 1, boundary_facets)
+        self._bc = _fem.dirichletbc(default_scalar_type(0.0), dofs, Q)
 
     def update_bc(self):
         """
         Update boundary condition if input-value is a lambda function
         """
         if hasattr(self, "_u"):
             self._u.interpolate(self._value)
```

### Comparing `OasisX-1.0.0/src/oasisx/fracstep.py` & `oasisx-1.1.0/src/oasisx/fracstep.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 # Copyright (C) 2022 Jørgen Schartum Dokken
 #
 # This file is part of Oasisx
 # SPDX-License-Identifier:    MIT
 
-from typing import List, Optional, Tuple
 import logging
+from typing import List, Optional, Tuple, Union
+
+from mpi4py import MPI as _MPI
+from petsc4py import PETSc as _PETSc
+
+import basix
+import dolfinx.fem.petsc as _petsc
 import numpy as np
 import numpy.typing as npt
 import ufl
-import basix
-import dolfinx.fem.petsc as _petsc
 from dolfinx import cpp as _cpp
+from dolfinx import default_scalar_type
 from dolfinx import fem as _fem
 from dolfinx import la as _la
 from dolfinx import mesh as _dmesh
-from petsc4py import PETSc as _PETSc
-from mpi4py import MPI as _MPI
+
 from .bcs import DirichletBC, PressureBC
+from .function import Projector
 from .ksp import KSPSolver
 
 __all__ = ["FractionalStep_AB_CN"]
 
 
-class FractionalStep_AB_CN():
+class FractionalStep_AB_CN:
     """
     Create the fractional step solver with Adam-Bashforth linearization
     of the convective term, and Crank-Nicholson time discretization.
 
     Args:
         mesh: The computational domain
         u_element: A tuple describing the finite element family and
             degree of the element used for the velocity
         p_element: A tuple describing the finite element family and
             degree of the element used for the pressure
         bcs_u: List of Dirichlet BCs for each component of the velocity
         bcs_p: List of Dirichlet BCs for the pressure
+        rotational: If True, use rotational form of pressure update
         solver_options: Dictionary with keys `'tentative'`, `'pressure'` and `'scalar'`,
             where each key leads to a dictionary of of PETSc options for each problem
         jit_options: Just in time parameters, to optimize form compilation
         options: Options for the Oasis solver.
             `"low_memory_version"` `True`/`False` changes if
             :math:`\\int\\nabla_k p^* v~\\mathrm{d}x` is assembled as
             `True`: directly into a vector or `False`: matrix-vector product.
@@ -51,17 +57,17 @@
     # -----------------------Multi-step variables-------------------------------
     _mesh: _dmesh.Mesh  # The computational domain
 
     # Convenience functions
     _sol_u: _fem.Function  # Tentative velocity as vector function (for outputting)
 
     # Velocity component and mapping to parent space
-    _Vi: List[Tuple[_fem.FunctionSpaceBase, npt.NDArray[np.int32]]]
-    _V: _fem.FunctionSpaceBase  # Velocity function space
-    _Q: _fem.FunctionSpaceBase  # Pressure function space
+    _Vi: List[Tuple[_fem.FunctionSpace, npt.NDArray[np.int32]]]
+    _V: _fem.FunctionSpace  # Velocity function space
+    _Q: _fem.FunctionSpace  # Pressure function space
 
     # Mass matrix for velocity component
     _mass_Vi: _fem.Form
     _M: _PETSc.Mat  # type: ignore
 
     # Boundary conditions
     _bcs_u: List[List[DirichletBC]]
@@ -80,15 +86,15 @@
     _rhs1: List[_fem.Function]  # RHS for each component of the tentative velocity
     _solver_u: KSPSolver
 
     # Adams-Bashforth convection term
     _conv_Vi: _fem.Form
     _uab: List[_fem.Function]  # Explicit part of Adam Bashforth convection term
 
-    # Stiffness matrix for velocity compoenent
+    # Stiffness matrix for velocity component
     _stiffness_Vi: _fem.Form
     _K: _PETSc.Mat  # type: ignore
 
     _p_vdxi: List[_fem.Form]  # Volume contributions of tentative pressure to RHS
     _p_vdxi_Mat: List[_PETSc.Mat]  # type: ignore
     # Low memory version
     _p_vdxi_Vec: List[_PETSc.Vec]  # type: ignore
@@ -117,79 +123,98 @@
     _p_rhs: List[_fem.Form]  # List of rhs for pressure correction
     # Matrices for non-low memory version of RHS assembly
     _divu_Mat: List[_PETSc.Mat]  # type: ignore
     # Pressure Laplacian
     _Ap: _PETSc.Mat  # type: ignore
     _wrk_p: _fem.Function  # Working vector for matrix vector    products in non-low memory version
 
+    # Rotational pressure correction variables
+    _projector_p: Optional[Projector]
+    _xi: Optional[_fem.Constant]
+    _nu: Optional[_fem.Constant]
+
     # ----------------------Velocity update-------------------------------------
     _solver_c: KSPSolver
 
     # grad_i(phi) v_i operator
     _grad_p: List[_fem.Form]
-    _grad_p_Mat: List[_PETSc.Mat]   # type: ignore
+    _grad_p_Mat: List[_PETSc.Mat]  # type: ignore
     # Low memory version
-    _grad_p_Vec: List[_PETSc.Vec]   # type: ignore
+    _grad_p_Vec: List[_PETSc.Vec]  # type: ignore
     _b3: _fem.Function
     # Mass matrix with bcs applied
-    _M_bcs: _PETSc.Mat   # type: ignore
+    _M_bcs: _PETSc.Mat  # type: ignore
 
     # Annotate all functions
     # __slots__ = tuple(__annotations__)
 
-    def __init__(self,
-                 mesh: _dmesh.Mesh,
-                 u_element: Tuple[str, int],
-                 p_element: Tuple[str, int],
-                 bcs_u: List[List[DirichletBC]],
-                 bcs_p: List[PressureBC],
-                 solver_options: Optional[dict] = None,
-                 jit_options: Optional[dict] = None,
-                 body_force: Optional[ufl.core.expr.Expr] = None,
-                 options: Optional[dict] = None):
+    def __init__(
+        self,
+        mesh: _dmesh.Mesh,
+        u_element: Union[Tuple[str, int], basix.finite_element.FiniteElement],
+        p_element: Union[Tuple[str, int], basix.finite_element.FiniteElement],
+        bcs_u: List[List[DirichletBC]],
+        bcs_p: List[PressureBC],
+        rotational: bool = False,
+        solver_options: Optional[dict] = None,
+        jit_options: Optional[dict] = None,
+        body_force: Optional[ufl.core.expr.Expr] = None,
+        options: Optional[dict] = None,
+    ):
         self._mesh = mesh
-
         cellname = mesh.ufl_cell().cellname()
-        v_family = basix.finite_element.string_to_family(u_element[0], cellname)
-        p_family = basix.finite_element.string_to_family(p_element[0], cellname)
-
-        v_el = basix.ufl.element(
-            v_family, cellname, u_element[1], basix.LagrangeVariant.gll_warped,
-            shape=(mesh.geometry.dim,), gdim=mesh.geometry.dim)
-        p_el = basix.ufl.element(
-            p_family, cellname, p_element[1], basix.LagrangeVariant.gll_warped,
-            gdim=mesh.geometry.dim)
+        try:
+            v_family = basix.finite_element.string_to_family(u_element[0], cellname)  # type: ignore
+            v_el = basix.ufl.element(
+                v_family,
+                cellname,
+                u_element[1],  # type: ignore
+                basix.LagrangeVariant.gll_warped,
+                shape=(mesh.geometry.dim,),
+            )
+        except TypeError:
+            v_el = u_element  # type: ignore
+        try:
+            p_family = basix.finite_element.string_to_family(p_element[0], cellname)  # type: ignore
+            p_el = basix.ufl.element(
+                p_family,
+                cellname,
+                p_element[1],  # type: ignore
+                basix.LagrangeVariant.gll_warped,
+            )
+        except TypeError:
+            p_el = p_element  # type: ignore
 
         # Initialize velocity functions for variational problem
-        self._V = _fem.FunctionSpace(mesh, v_el)
+        self._V = _fem.functionspace(mesh, v_el)
         self._sol_u = _fem.Function(self._V, name="u")  # Function for outputting vector functions
 
         self._Vi = [self._V.sub(i).collapse() for i in range(self._V.num_sub_spaces)]
         self._u = [_fem.Function(Vi[0], name=f"u{i}") for (i, Vi) in enumerate(self._Vi)]
         self._u1 = [_fem.Function(Vi[0], name=f"u_{i}1") for (i, Vi) in enumerate(self._Vi)]
         self._u2 = [_fem.Function(Vi[0], name=f"u_{i}2") for (i, Vi) in enumerate(self._Vi)]
         self._uab = [_fem.Function(Vi[0], name=f"u_{i}ab") for (i, Vi) in enumerate(self._Vi)]
 
-        # Create boundary conditons for velocity spaces
+        # Create boundary conditions for velocity spaces
         self._bcs_u = bcs_u
         for bc_i, Vi in zip(self._bcs_u, self._Vi):
             for bc in bc_i:
                 bc.create_bc(Vi[0])
 
         # Working arrays
         self._wrk_vel = [_fem.Function(Vi[0]) for Vi in self._Vi]
         self._wrk_comp = _fem.Function(self._Vi[0][0])
 
         # RHS arrays
         self._rhs1 = [_fem.Function(Vi[0]) for Vi in self._Vi]
         self._b0 = [_fem.Function(Vi[0]) for Vi in self._Vi]
         self._b_first = [_fem.Function(Vi[0]) for Vi in self._Vi]
 
-        # Initialize pressure functions for varitional problem
-        self._Q = _fem.FunctionSpace(mesh, p_el)
+        # Initialize pressure functions for variational problem
+        self._Q = _fem.functionspace(mesh, p_el)
         self._ps = _fem.Function(self._Q)  # Pressure used in tentative velocity scheme
         self._p = _fem.Function(self._Q)
         self._dp = _fem.Function(self._Q)
         self._b2 = _fem.Function(self._Q)
 
         # Create boundary conditions for pressure space
         forms: List[List[ufl.form.Form]] = [[] for _ in range(self._mesh.geometry.dim)]
@@ -200,109 +225,142 @@
                 forms[i].append(bcp.rhs(i))
 
         if len(self._bcs_p) > 0:
             self._p_surf = [_fem.form(sum(form)) for form in forms]
 
         # Create solvers for each step
         solver_options = {} if solver_options is None else solver_options
-        self._solver_u = KSPSolver(mesh.comm, solver_options.get("tentative"),
-                                   prefix="tentative_velocity")
-        self._solver_p = KSPSolver(mesh.comm, solver_options.get("pressure"),
-                                   prefix="pressure_correction")
-        self._solver_c = KSPSolver(mesh.comm, solver_options.get("scalar"),
-                                   prefix="velcoity_update")
+        self._solver_u = KSPSolver(
+            mesh.comm, solver_options.get("tentative"), prefix="tentative_velocity"
+        )
+        self._solver_p = KSPSolver(
+            mesh.comm, solver_options.get("pressure"), prefix="pressure_correction"
+        )
+        if rotational:
+            self._xi = _fem.Constant(mesh, default_scalar_type(0.5))
+            self._nu = _fem.Constant(mesh, default_scalar_type(1))
+            update_expr = self._p + self._dp - self._xi * self._nu * ufl.div(ufl.as_vector(self._u))
+            self._projector_p = Projector(
+                update_expr,
+                self._Q,
+                bcs=[],
+                petsc_options=solver_options.get("scalar"),
+                jit_options=jit_options,
+            )
+        else:
+            self._projector_p = None
+            self._xi = None
+            self._nu = None
+
+        self._solver_c = KSPSolver(
+            mesh.comm, solver_options.get("scalar"), prefix="velocity_update"
+        )
 
         if options is None:
             options = {}
         self._low_memory = options.get("low_memory_version", True)
 
         # Precompile forms and allocate matrices
         jit_options = {} if jit_options is None else jit_options
         if body_force is None:
-            body_force = (0.,) * mesh.geometry.dim
+            body_force = (0.0,) * mesh.geometry.dim
         self._compile_and_allocate_forms(body_force, jit_options)
 
         # Assemble constant matrices
         self._preassemble()
 
         # Set solver operator
         self._solver_p.setOperators(self._Ap)
         self._solver_p.setOptions(self._Ap)
         self._solver_c.setOperators(self._M)
         self._solver_u.setOperators(self._A)
         self._solver_u.setOptions(self._A)
 
-    def _compile_and_allocate_forms(self, body_force: ufl.core.expr.Expr,
-                                    jit_options: dict):
+    def _compile_and_allocate_forms(self, body_force: ufl.core.expr.Expr, jit_options: dict):
         dx = ufl.Measure("dx", domain=self._mesh)
         u = ufl.TrialFunction(self._Vi[0][0])
         v = ufl.TestFunction(self._Vi[0][0])
 
         # -----------------Tentative velocity step----------------------
         self._body_force = []
         for force in body_force:
             try:
                 force = _fem.Constant(self._mesh, force)
             except RuntimeError:
                 pass
-            self._body_force.append(_fem.form(force*v*dx, jit_options=jit_options))
+            self._body_force.append(_fem.form(force * v * dx, jit_options=jit_options))
 
         # Mass matrix for velocity component
-        self._mass_Vi = _fem.form(u*v*dx, jit_options=jit_options)
+        self._mass_Vi = _fem.form(u * v * dx, jit_options=jit_options)
         self._M = _petsc.create_matrix(self._mass_Vi)
         self._A = _petsc.create_matrix(self._mass_Vi)
 
         # Stiffness matrix for velocity component
-        self._stiffness_Vi = _fem.form(ufl.inner(ufl.grad(u), ufl.grad(v))*dx,
-                                       jit_options=jit_options)
+        self._stiffness_Vi = _fem.form(
+            ufl.inner(ufl.grad(u), ufl.grad(v)) * dx, jit_options=jit_options
+        )
         self._K = _petsc.create_matrix(self._stiffness_Vi)
 
         # Pressure contribution
         p = ufl.TrialFunction(self._Q)
         self._p_vdxi_Vec = [_fem.Function(Vi[0]) for Vi in self._Vi]
         if self._low_memory:
-            self._p_vdxi = [_fem.form(self._ps*v.dx(i)*dx, jit_options=jit_options)
-                            for i in range(self._mesh.geometry.dim)]
+            self._p_vdxi = [
+                _fem.form(self._ps * v.dx(i) * dx, jit_options=jit_options)
+                for i in range(self._mesh.geometry.dim)
+            ]
         else:
-            self._p_vdxi = [_fem.form(p*v.dx(i)*dx, jit_options=jit_options)
-                            for i in range(self._mesh.geometry.dim)]
+            self._p_vdxi = [
+                _fem.form(p * v.dx(i) * dx, jit_options=jit_options)
+                for i in range(self._mesh.geometry.dim)
+            ]
             self._p_vdxi_Mat = [_petsc.create_matrix(grad_p) for grad_p in self._p_vdxi]
 
-        # -----------------Pressure currection step----------------------
+        # -----------------Pressure correction step----------------------
 
         # Pressure Laplacian/stiffness matrix
         q = ufl.TestFunction(self._Q)
-        self._stiffness_Q = _fem.form(ufl.inner(ufl.grad(p), ufl.grad(q))*ufl.dx,
-                                      jit_options=jit_options)
+        self._stiffness_Q = _fem.form(
+            ufl.inner(ufl.grad(p), ufl.grad(q)) * ufl.dx, jit_options=jit_options
+        )
         self._Ap = _petsc.create_matrix(self._stiffness_Q)
 
         # RHS for pressure correction (unscaled)
         if self._low_memory:
-            self._p_rhs = [_fem.form(ufl.div(ufl.as_vector(self._u))*q*dx, jit_options=jit_options)]
+            self._p_rhs = [
+                _fem.form(ufl.div(ufl.as_vector(self._u)) * q * dx, jit_options=jit_options)
+            ]
         else:
-            self._p_rhs = [_fem.form(u.dx(i)*q*dx, jit_options=jit_options)
-                           for i in range(self._mesh.geometry.dim)]
+            self._p_rhs = [
+                _fem.form(u.dx(i) * q * dx, jit_options=jit_options)
+                for i in range(self._mesh.geometry.dim)
+            ]
             self._divu_Mat = [_petsc.create_matrix(rhs) for rhs in self._p_rhs]
             self._wrk_p = _fem.Function(self._Q)
 
         # ---------------------------Velocity update-----------------------
         # RHS for velocity update
         self._b3 = _fem.Function(self._Vi[0][0])
         if self._low_memory:
-            self._grad_p = [_fem.form(self._dp.dx(i) * v*dx, jit_options=jit_options)
-                            for i in range(len(self._Vi))]
+            self._grad_p = [
+                _fem.form(self._dp.dx(i) * v * dx, jit_options=jit_options)
+                for i in range(len(self._Vi))
+            ]
         else:
-            self._grad_p = [_fem.form(p.dx(i)*v*dx, jit_options=jit_options)
-                            for i in range(self._mesh.geometry.dim)]
+            self._grad_p = [
+                _fem.form(p.dx(i) * v * dx, jit_options=jit_options)
+                for i in range(self._mesh.geometry.dim)
+            ]
             self._grad_p_Mat = [_petsc.create_matrix(grad_p) for grad_p in self._grad_p]
 
         # Convection term for Adams Bashforth step
-        self._conv_Vi = _fem.form(ufl.inner(ufl.dot(ufl.as_vector(self._uab),
-                                                    ufl.nabla_grad(u)), v)*dx,
-                                  jit_options=jit_options)
+        self._conv_Vi = _fem.form(
+            ufl.inner(ufl.dot(ufl.as_vector(self._uab), ufl.nabla_grad(u)), v) * dx,
+            jit_options=jit_options,
+        )
 
     def _preassemble(self):
         """
         Assemble time independent matrices and vectors
 
         This includes:
         1. Mass matrix for a component of the velocity
@@ -315,16 +373,15 @@
         """
         _petsc.assemble_matrix(self._M, self._mass_Vi)
         self._M.assemble()
         _petsc.assemble_matrix(self._K, self._stiffness_Vi)
         self._K.assemble()
 
         # Assemble stiffness matrix with boundary conditions
-        _petsc.assemble_matrix(self._Ap, self._stiffness_Q, bcs=[
-            bc._bc for bc in self._bcs_p])
+        _petsc.assemble_matrix(self._Ap, self._stiffness_Q, bcs=[bc._bc for bc in self._bcs_p])
         self._Ap.assemble()
         if len(self._bcs_p) == 0:
             nullspace = _PETSc.NullSpace().create(constant=True, comm=self._mesh.comm)
             self._Ap.setNullSpace(nullspace)
             self._Ap.setNearNullSpace(nullspace)
 
         # Assemble constant body forces
@@ -346,16 +403,15 @@
                 # Preassemble u.dx(i)q
                 _petsc.assemble_matrix(self._divu_Mat[i], self._p_rhs[i])
                 self._divu_Mat[i].assemble()
 
         # Create mass matrix with symmetrically applied bcs
         self._M_bcs = self._M.copy()
         for bcu in self._bcs_u[0]:
-            self._M_bcs.zeroRowsColumnsLocal(
-                bcu._bc._cpp_object.dof_indices()[0], 1.)  # type: ignore
+            self._M_bcs.zeroRowsColumnsLocal(bcu._bc._cpp_object.dof_indices()[0], 1.0)  # type: ignore
 
     def assemble_first(self, dt: float, nu: float):
         """
         Assembly routine for first iteration of pressure/velocity system.
 
         .. math::
             A=\\frac{1}{\\delta t}M  + \\frac{1}{2} C +\\frac{1}{2}\\nu K
@@ -377,27 +433,27 @@
         for i, (u_ab, u_1, u_2) in enumerate(zip(self._uab, self._u1, self._u2)):
             u_ab.x.array[:] = 0
             u_ab.x.array[:] = 1.5 * u_1.x.array - 0.5 * u_2.x.array
         self._A.zeroEntries()
         _petsc.assemble_matrix(self._A, a=self._conv_Vi)  # type: ignore
         self._A.assemble()
         self._A.scale(-0.5)  # Negative convection on the rhs
-        self._A.axpy(1./dt, self._M, _PETSc.Mat.Structure.SUBSET_NONZERO_PATTERN)  # type: ignore
+        self._A.axpy(1.0 / dt, self._M, _PETSc.Mat.Structure.SUBSET_NONZERO_PATTERN)  # type: ignore
 
         # Add diffusion
-        self._A.axpy(-0.5*nu, self._K, _PETSc.Mat.Structure.SUBSET_NONZERO_PATTERN)  # type: ignore
+        self._A.axpy(-0.5 * nu, self._K, _PETSc.Mat.Structure.SUBSET_NONZERO_PATTERN)  # type: ignore
 
         # Update Pressure BC
         for bc in self._bcs_p:
             bc.update_bc()
 
         # Compute rhs for all velocity components
         for i, _ in enumerate(self._u):
             self._b_first[i].x.array[:] = 0
-            # Start with transient convection and difffusion
+            # Start with transient convection and diffusion
             self._A.mult(self._u1[i].vector, self._wrk_comp.vector)
             self._wrk_comp.x.scatter_forward()
 
             # Add body force
             self._wrk_comp.x.array[:] += self._b0[i].x.array[:]
 
             self._b_first[i].x.array[:] += self._wrk_comp.x.array[:]
@@ -407,18 +463,18 @@
                 self._wrk_comp.x.array[:] = 0
                 _petsc.assemble_vector(self._wrk_comp.vector, self._p_surf[i])
                 self._wrk_comp.x.scatter_reverse(_la.InsertMode.add)
                 self._b_first[i].x.array[:] += self._wrk_comp.x.array[:]
 
         # Reset matrix for lhs
         self._A.scale(-1)
-        self._A.axpy(2./dt, self._M,  _PETSc.Mat.Structure.SUBSET_NONZERO_PATTERN)  # type: ignore
+        self._A.axpy(2.0 / dt, self._M, _PETSc.Mat.Structure.SUBSET_NONZERO_PATTERN)  # type: ignore
         # NOTE: This would not work if we have different DirichletBCs on different components
         for bcu in self._bcs_u[0]:
-            self._A.zeroRowsLocal(bcu._bc._cpp_object.dof_indices()[0], 1.)  # type: ignore
+            self._A.zeroRowsLocal(bcu._bc._cpp_object.dof_indices()[0], 1.0)  # type: ignore
 
     def velocity_tentative_assemble(self):
         """
         Assemble RHS of tentative velocity equation computing the :math:`p^*`-dependent term of
 
         .. math::
 
@@ -427,22 +483,26 @@
 
         :math:`b(u_k^{n-1})` is computed in :py:obj:`FractionalStep_AB_CN.assemble_first`.
         """
         if self._low_memory:
             # Using the fact that all the gradient forms has the same coefficient
             coeffs = _cpp.fem.pack_coefficients(self._p_vdxi[0]._cpp_object)
             for i in range(self._mesh.geometry.dim):
-                self._p_vdxi_Vec[i].x.array[:] = 0.
+                self._p_vdxi_Vec[i].x.array[:] = 0.0
                 _petsc.assemble_vector(
-                    self._p_vdxi_Vec[i].vector, self._p_vdxi[i], coeffs=coeffs, constants=[])
+                    self._p_vdxi_Vec[i].vector,
+                    self._p_vdxi[i],
+                    coeffs=coeffs,
+                    constants=np.empty(0, dtype=self._p_vdxi_Vec[i].x.array.dtype),
+                )
                 self._p_vdxi_Vec[i].x.scatter_reverse(_la.InsertMode.add)
                 self._p_vdxi_Vec[i].x.scatter_forward()
         else:
             for i in range(self._mesh.geometry.dim):
-                self._p_vdxi_Vec[i].x.array[:] = 0.
+                self._p_vdxi_Vec[i].x.array[:] = 0.0
                 self._p_vdxi_Mat[i].mult(self._ps.vector, self._p_vdxi_Vec[i].vector)
                 self._p_vdxi_Vec[i].x.scatter_forward()
 
         # Update RHS
         for i in range(self._mesh.geometry.dim):
             self._rhs1[i].x.array[:] = self._b_first[i].x.array + self._p_vdxi_Vec[i].x.array
 
@@ -470,74 +530,94 @@
         Assemble RHS for pressure correction term
 
         .. math::
 
             b_c = \\int_{\\Omega} \\mathrm{div} u^l q~\\mathrm{d}x.
 
         """
-        self._b2.x.array[:] = 0.
+        self._b2.x.array[:] = 0.0
         if self._low_memory:
             _petsc.assemble_vector(self._b2.vector, self._p_rhs[0])
         else:
             for i in range(self._mesh.geometry.dim):
                 self._divu_Mat[i].mult(self._u[i].vector, self._wrk_p.vector)
                 self._b2.vector.axpy(1, self._wrk_p.vector)
 
         # Apply boundary conditions to the rhs
         self._b2.x.scatter_reverse(_la.InsertMode.add)
-        self._b2.vector.scale(-1/dt)
+        self._b2.vector.scale(-1 / dt)
 
-        # Set homogenuous Dirichlet boundary condition on pressure correction
+        # Set homogenous Dirichlet boundary condition on pressure correction
         bc_p = [bc._bc for bc in self._bcs_p]
         _petsc.set_bc(self._b2.vector, bc_p)
         self._b2.x.scatter_forward()
 
-    def pressure_solve(self) -> np.int32:
+    def pressure_solve(self, nu: Optional[float] = None, rotational: bool = False) -> np.int32:
         """
         Solve pressure correction problem
         """
         logger = logging.getLogger("oasisx")
 
         # Set difference vector to previous time step
         if len(self._bcs_p) == 0:
             # If pressure nullspace, use mumps to deal with singular matrix
-            nullspace_options = {"ksp_type": "preonly", "pc_type": "lu",
-                                 "pc_factor_mat_solver_type": "mumps",
-                                 "mat_mumps_icntl_24": 1,
-                                 "mat_mumps_icntl_25": 0,
-                                 "ksp_error_if_not_converged": 1}
+            nullspace_options = {
+                "ksp_type": "preonly",
+                "pc_type": "lu",
+                "pc_factor_mat_solver_type": "mumps",
+                "mat_mumps_icntl_24": 1,
+                "mat_mumps_icntl_25": 0,
+                "ksp_error_if_not_converged": 1,
+            }
             logger.debug(f"Updating PETSc options to {nullspace_options}")
             nullspace = self._Ap.getNullSpace()
             nullspace.remove(self._b2.vector)
             self._solver_p.updateOptions(nullspace_options)
             self._solver_p.setOptions(self._Ap)
 
         converged = self._solver_p.solve(self._b2.vector, self._dp)
         if len(self._bcs_p) == 0:
             logger.debug("Making sure that mean of phi is 0 with lack of pressure conditions")
             vol = self._mesh.comm.allreduce(
-                _fem.assemble_scalar(_fem.form(1*ufl.dx(domain=self._mesh))), op=_MPI.SUM)
-            phi_avg = self._mesh.comm.allreduce(
-                _fem.assemble_scalar(_fem.form(self._dp*ufl.dx)),
-                op=_MPI.SUM)/vol
+                _fem.assemble_scalar(_fem.form(1 * ufl.dx(domain=self._mesh))),
+                op=_MPI.SUM,
+            )
+            phi_avg = (
+                self._mesh.comm.allreduce(
+                    _fem.assemble_scalar(_fem.form(self._dp * ufl.dx)), op=_MPI.SUM
+                )
+                / vol
+            )
             self._dp.x.array[:] -= phi_avg
-        self._ps.x.array[:] = self._p.x.array[:] + self._dp.x.array
+
+        if self._projector_p is not None:
+            if nu is not None and self._nu is not None:
+                self._nu.value = nu
+            else:
+                raise RuntimeWarning(
+                    "Kinematic viscosity not set for rotational pressure correction"
+                )
+            error = self._projector_p.solve(assemble_rhs=True)
+            assert error > 0
+            self._ps.x.array[:] = self._projector_p.x.x.array[:]
+        else:
+            self._ps.x.array[:] = self._p.x.array[:] + self._dp.x.array
         return converged
 
     def velocity_update(self, dt) -> npt.NDArray[np.int32]:
         """
         Compute Velocity update
         """
         errors = np.zeros(self._mesh.geometry.dim, dtype=np.int32)
         if self._low_memory:
             for i in range(self._mesh.geometry.dim):
                 # Compute M u^{n-1}
                 self._M.mult(self._u[i].vector, self._b3.vector)
 
-                self._wrk_comp.x.array[:] = 0.
+                self._wrk_comp.x.array[:] = 0.0
                 _petsc.assemble_vector(self._wrk_comp.vector, self._grad_p[i])
                 self._wrk_comp.x.scatter_reverse(_la.InsertMode.add)
 
                 # Subtract
                 self._b3.vector.axpy(-dt, self._wrk_comp.vector)
 
                 # Set bcs
@@ -553,15 +633,15 @@
                 errors[i] = self._solver_c.solve(self._b3.vector, self._u[i])
         else:
             for i in range(self._mesh.geometry.dim):
                 # Compute M u^{n-1}
                 self._M.mult(self._u[i].vector, self._b3.vector)
 
                 # Compute dphi/dx_i vi dx
-                self._wrk_comp.x.array[:] = 0.
+                self._wrk_comp.x.array[:] = 0.0
                 self._grad_p_Mat[i].mult(self._dp.vector, self._wrk_comp.vector)
 
                 # Subtract
                 self._b3.vector.axpy(-dt, self._wrk_comp.vector)
 
                 # Set bcs
                 # bcs_u = [bcu._bc for bcu in self._bcs_u[i]]
@@ -572,16 +652,15 @@
                 # self._b3.vector.axpy(1, self._wrk_comp.vector)
                 # _petsc.set_bc(self._b3.vector, bcs_u)
                 self._b3.x.scatter_forward()
                 errors[i] = self._solver_c.solve(self._b3.vector, self._u[i])
 
         return errors
 
-    def solve(self, dt: float, nu: float, max_error: float = 1e-12,
-              max_iter: int = 10):
+    def solve(self, dt: float, nu: float, max_error: float = 1e-12, max_iter: int = 10):
         """
         Propagate splitting scheme one time step
 
         Args:
             dt: The time step
             nu: The kinematic velocity
             max_error: The maximal difference for inner iterations of solving `u`
@@ -594,21 +673,19 @@
 
         [[bc.update_bc() for bc in bcu] for bcu in self._bcs_u]
         self.assemble_first(dt, nu)
         while inner_it < max_iter and diff > max_error:
             inner_it += 1
             self.velocity_tentative_assemble()
             diff, errors = self.velocity_tentative_solve()
-
             assert (errors > 0).all()
             self.pressure_assemble(dt)
-            error_p = self.pressure_solve()
+            error_p = self.pressure_solve(nu=nu)
             assert error_p > 0
 
-        # assert inner_it != max_iter
         self.velocity_update(dt)
 
         # Propagate solutions u1->u2, u->u1
         for i in range(self._mesh.geometry.dim):
             self._u2[i].x.array[:] = self._u1[i].x.array
             self._u1[i].x.array[:] = self._u[i].x.array
```

### Comparing `OasisX-1.0.0/src/oasisx/function.py` & `oasisx-1.1.0/src/oasisx/function.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright (C) 2022 Jørgen Schartum Dokken
 #
 # This file is part of Oasisx
 # SPDX-License-Identifier:    MIT
 
 from typing import List, Optional
 
+from petsc4py import PETSc as _petsc
+
 import dolfinx.fem
 import ufl
-from petsc4py import PETSc as _petsc
 
 
-class Projector():
+class Projector:
     """
     Projector for a given function.
     Solves Ax=b, where
 
     .. highlight:: python
     .. code-block:: python
 
@@ -28,110 +29,126 @@
         space: Space to project function into
         bcs: List of BCS to apply to projection
         petsc_options: Options to pass to PETSc
         jit_options: Options to pass to just in time compiler
         form_compiler_options: Options to pass to the form compiler
         metadata: Data to pass to the integration measure
     """
+
     # The mass matrix
     _A: _petsc.Mat  # type: ignore
     # The rhs vector
     _b: _petsc.Vec  # type: ignore
     _lhs: dolfinx.fem.forms.Form  # The compiled form for the mass matrix
     _rhs: dolfinx.fem.forms.Form  # The compiled form form the rhs vector
     # The PETSc solver
     _ksp: _petsc.KSP  # type: ignore
     _x: dolfinx.fem.Function  # The solution vector
     _bcs: List[dolfinx.fem.DirichletBC]
     __slots__ = tuple(__annotations__)
 
-    def __init__(self, function: ufl.core.expr.Expr,
-                 space: dolfinx.fem.FunctionSpaceBase,
-                 bcs: List[dolfinx.fem.DirichletBC],
-                 petsc_options: Optional[dict] = None,
-                 jit_options: Optional[dict] = None,
-                 form_compiler_options: Optional[dict] = None,
-                 metadata: Optional[dict] = None):
+    def __init__(
+        self,
+        function: ufl.core.expr.Expr,
+        space: dolfinx.fem.FunctionSpace,
+        bcs: Optional[List[dolfinx.fem.DirichletBC]] = None,
+        petsc_options: Optional[dict] = None,
+        jit_options: Optional[dict] = None,
+        form_compiler_options: Optional[dict] = None,
+        metadata: Optional[dict] = None,
+    ):
         petsc_options = {} if petsc_options is None else petsc_options
         jit_options = {} if jit_options is None else jit_options
         form_compiler_options = {} if form_compiler_options is None else form_compiler_options
 
         # Assemble projection matrix once
         u = ufl.TrialFunction(space)
         v = ufl.TestFunction(space)
         a = ufl.inner(u, v) * ufl.dx(metadata=metadata)
-        self._lhs = dolfinx.fem.form(a, jit_options=jit_options,
-                                     form_compiler_options=form_compiler_options)
+        self._lhs = dolfinx.fem.form(
+            a, jit_options=jit_options, form_compiler_options=form_compiler_options
+        )
+        bcs = [] if bcs is None else bcs
         self._A = dolfinx.fem.petsc.assemble_matrix(self._lhs, bcs=bcs)
         self._A.assemble()
 
         # Compile RHS form and create vector
         L = ufl.inner(function, v) * ufl.dx(metadata=metadata)
-        self._rhs = dolfinx.fem.form(L, jit_options=jit_options,
-                                     form_compiler_options=form_compiler_options)
+        self._rhs = dolfinx.fem.form(
+            L, jit_options=jit_options, form_compiler_options=form_compiler_options
+        )
         self._x = dolfinx.fem.Function(space)
         self._b = dolfinx.fem.Function(space)
-        self._bcs = bcs
+        self._bcs = [] if bcs is None else bcs
 
         # Create Krylov Subspace solver
         self._ksp = _petsc.KSP().create(space.mesh.comm)  # type: ignore
         self._ksp.setOperators(self._A)
 
         # Set PETSc options
-        prefix = f"oasis_projector_{id(self)}"
+        prefix = "oasis_projector"
         opts = _petsc.Options()  # type: ignore
         opts.prefixPush(prefix)
+        self._ksp.setOptionsPrefix(prefix)
         for k, v in petsc_options.items():
             opts[k] = v
         opts.prefixPop()
         self._ksp.setFromOptions()
 
         # Set matrix and vector PETSc options
         self._A.setOptionsPrefix(prefix)
         self._A.setFromOptions()
         self._b.vector.setOptionsPrefix(prefix)
         self._b.vector.setFromOptions()
 
+        for opt in opts.getAll().keys():
+            del opts[opt]
+
+        # Setup preconditioner
+        self._ksp.getPC().setUp()
+
     def assemble_rhs(self):
         """
         Update RHS by re-assembling
         """
-        self._b.x.array[:] = 0.
+        self._b.x.array[:] = 0.0
         dolfinx.fem.petsc.assemble_vector(self._b.vector, self._rhs)
-        dolfinx.fem.petsc.apply_lifting(
-            self._b.vector, [self._lhs], bcs=[self._bcs])
+        if len(self._bcs) > 0:
+            dolfinx.fem.petsc.apply_lifting(self._b.vector, [self._lhs], bcs=[self._bcs])
         self._b.x.scatter_reverse(dolfinx.cpp.la.InsertMode.add)
-        dolfinx.fem.petsc.set_bc(self._b.vector, self._bcs)
+        if len(self._bcs) > 0:
+            dolfinx.fem.petsc.set_bc(self._b.vector, self._bcs)
         self._b.x.scatter_forward()
 
-    def solve(self, assemble_rhs: bool = True):
+    def solve(self, assemble_rhs: bool = True) -> int:
         """
         Compute projection using PETSc a KSP solver
 
         Args:
             assemble_rhs: Re-assemble RHS and re-apply boundary conditions if true
         """
         if assemble_rhs:
             self.assemble_rhs()
 
         self._ksp.solve(self._b.vector, self._x.vector)
+        self._x.x.scatter_forward()
+        return int(self._ksp.getConvergedReason())
 
     @property
     def x(self):
         return self._x
 
     def __del__(self):
         self._ksp.destroy()
         self._A.destroy()
         self._b.vector.destroy()
         self._x.vector.destroy()
 
 
-class LumpedProject():
+class LumpedProject:
     """Projector using a lumped mass matrix"""
+
     __slots__ = ["_form", "_petsc_options", "_bcs"]
 
     def __init__(self):
-        """
-
-        """
+        """ """
         raise NotImplementedError
```

### Comparing `OasisX-1.0.0/src/oasisx/ksp.py` & `oasisx-1.1.0/src/oasisx/ksp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 # Copyright (C) 2022 Jørgen Schartum Dokken
 #
 # This file is part of Oasisx
 # SPDX-License-Identifier:    MIT
 
-from petsc4py import PETSc as _PETSc
-import dolfinx.fem as _fem
 import typing
+
 from mpi4py import MPI
+from petsc4py import PETSc as _PETSc
+
+import dolfinx.fem as _fem
 import numpy as np
 
 
 class KSPSolver:
     _prefix: str
     _ksp: _PETSc.KSP  # type: ignore
     __slots__ = tuple(__annotations__)
 
-    def __init__(self, comm: MPI.Comm,
-                 petsc_options: typing.Optional[dict] = None,
-                 prefix="oasis_solver"):
+    def __init__(
+        self,
+        comm: MPI.Comm,
+        petsc_options: typing.Optional[dict] = None,
+        prefix="oasis_solver",
+    ):
         """Lightweight wrapper around the PETSc KSP solver
         Args:
             comm: MPI communicator used in PETSc Solver
             petsc_options: Options that are passed to the linear
                 algebra backend PETSc. For available choices for the
                 'petsc_options' kwarg, see the `PETSc documentation
                 <https://petsc4py.readthedocs.io/en/stable/manual/ksp/>`_.
         """
         petsc_options = {} if petsc_options is None else petsc_options
-        self._ksp = _PETSc.KSP().create(comm)    # type: ignore
+        self._ksp = _PETSc.KSP().create(comm)  # type: ignore
         self._prefix = prefix
         self.updateOptions(petsc_options)
 
     def updateOptions(self, options: dict):
         """
         Update PETSc options.
 
@@ -41,32 +46,38 @@
         self._ksp.setOptionsPrefix(self._prefix)
         opts = _PETSc.Options()  # type: ignore
         opts.prefixPush(self._prefix)
         for k, v in options.items():
             opts[k] = v
         opts.prefixPop()
         self._ksp.setFromOptions()
+        for opt in opts.getAll().keys():
+            del opts[opt]
 
-    def setOptions(self, op: typing.Union[_PETSc.Mat, _PETSc.Vec]):    # type: ignore
+    def setOptions(self, op: typing.Union[_PETSc.Mat, _PETSc.Vec]):  # type: ignore
         prefix = self._ksp.getOptionsPrefix()
         assert prefix is not None
         op.setOptionsPrefix(prefix)
         op.setFromOptions()
 
-    def setOperators(self,
-                     A: _PETSc.Mat,    # type: ignore
-                     P: typing.Optional[_PETSc.Mat] = None):    # type: ignore
+    def setOperators(
+        self,
+        A: _PETSc.Mat,  # type: ignore
+        P: typing.Optional[_PETSc.Mat] = None,  # type: ignore
+    ):
         if P is None:
             self._ksp.setOperators(A)
         else:
             self._ksp.setOperators(A, P)
 
-    def solve(self,
-              b: _PETSc.Vec,  # type: ignore
-              x: _fem.Function) -> np.int32:
+    def solve(
+        self,
+        b: _PETSc.Vec,  # type: ignore
+        x: _fem.Function,
+    ) -> np.int32:
         self._ksp.solve(b, x.vector)
         x.x.scatter_forward()
         return np.int32(self._ksp.getConvergedReason())
 
     def __del__(self):
         """
         Delete PETSc options manually due to https://gitlab.com/petsc/petsc/-/issues/1201
```

### Comparing `OasisX-1.0.0/test/test_bcs.py` & `oasisx-1.1.0/test/test_bcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 # Copyright (C) 2022 Jørgen Schartum Dokken
 #
 # This file is part of Oasisx
 # SPDX-License-Identifier:    MIT
 #
 # Tests for DirichletBC wrapper
 
+from mpi4py import MPI
+
 import dolfinx
 import dolfinx.fem.petsc
 import numpy as np
 import pytest
 import ufl
-from mpi4py import MPI
+
 from oasisx import DirichletBC, LocatorMethod, PressureBC
 
 
 @pytest.mark.parametrize("P", np.arange(1, 5))
 def test_function_geometrical(P):
     """
     Test assignement of a time dependent function to DirichletBC using geometrical mode
     """
     mesh = dolfinx.mesh.create_unit_square(MPI.COMM_WORLD, 10, 10)
 
     def locator(x):
         return np.isclose(x[0], 1)
 
-    class TimeDependentBC():
+    class TimeDependentBC:
         def __init__(self, t: float):
             self.t = t
 
         def eval(self, x):
             return np.sin(x[0]) + x[1] * self.t
 
     condition_0 = TimeDependentBC(0.1)
 
-    bc = DirichletBC(condition_0.eval,  LocatorMethod.GEOMETRICAL, locator)
+    bc = DirichletBC(condition_0.eval, LocatorMethod.GEOMETRICAL, locator)
 
-    V = dolfinx.fem.FunctionSpace(mesh, ("Lagrange", int(P)))
+    V = dolfinx.fem.functionspace(mesh, ("Lagrange", int(P)))
     bc.create_bc(V)
 
     for t in [0.1, 0.2, 0.3]:
         u = dolfinx.fem.Function(V)
-        u.interpolate(lambda x: np.sin(x[0]) + x[1]*t)
+        u.interpolate(lambda x: np.sin(x[0]) + x[1] * t)
         bc_dx = dolfinx.fem.dirichletbc(u, dolfinx.fem.locate_dofs_geometrical(V, locator))
 
         u_bcx = dolfinx.fem.Function(V)
         dolfinx.fem.petsc.set_bc(u_bcx.vector, [bc_dx])
 
         u_bc = dolfinx.fem.Function(V)
         condition_0.t = t
@@ -60,33 +62,33 @@
     Test assignement of a time dependent function to DirichletBC using topological mode
     """
     mesh = dolfinx.mesh.create_unit_square(MPI.COMM_WORLD, 10, 10)
 
     def locator(x):
         return np.isclose(x[0], 1)
 
-    class TimeDependentBC():
+    class TimeDependentBC:
         def __init__(self, t: float):
             self.t = t
 
         def eval(self, x):
             return np.sin(x[0]) + x[1] * self.t
 
     condition_0 = TimeDependentBC(0.1)
     entities = dolfinx.mesh.locate_entities(mesh, dim, locator)
     value = np.int32(3)
     et = dolfinx.mesh.meshtags(mesh, dim, entities, np.full(len(entities), value, dtype=np.int32))
-    bc = DirichletBC(condition_0.eval,  LocatorMethod.TOPOLOGICAL, (et, value))
+    bc = DirichletBC(condition_0.eval, LocatorMethod.TOPOLOGICAL, (et, value))
 
-    V = dolfinx.fem.FunctionSpace(mesh, ("Lagrange", int(P)))
+    V = dolfinx.fem.functionspace(mesh, ("Lagrange", int(P)))
     bc.create_bc(V)
 
     for t in [0.1, 0.2, 0.3]:
         u = dolfinx.fem.Function(V)
-        u.interpolate(lambda x: np.sin(x[0]) + x[1]*t)
+        u.interpolate(lambda x: np.sin(x[0]) + x[1] * t)
         bc_dx = dolfinx.fem.dirichletbc(u, dolfinx.fem.locate_dofs_topological(V, dim, entities))
 
         u_bcx = dolfinx.fem.Function(V)
         dolfinx.fem.petsc.set_bc(u_bcx.vector, [bc_dx])
 
         u_bc = dolfinx.fem.Function(V)
         condition_0.t = t
@@ -101,19 +103,19 @@
     Test assignement of a time dependent constant to DirichletBC using geometrical mode
     """
     mesh = dolfinx.mesh.create_unit_square(MPI.COMM_WORLD, 10, 10)
 
     def locator(x):
         return np.isclose(x[0], 1)
 
-    time = dolfinx.fem.Constant(mesh, 1.)
+    time = dolfinx.fem.Constant(mesh, 1.0)
 
-    bc = DirichletBC(time,  LocatorMethod.GEOMETRICAL, locator)
+    bc = DirichletBC(time, LocatorMethod.GEOMETRICAL, locator)
 
-    V = dolfinx.fem.FunctionSpace(mesh, ("Lagrange", int(P)))
+    V = dolfinx.fem.functionspace(mesh, ("Lagrange", int(P)))
     bc.create_bc(V)
 
     for t in [0.1, 0.2, 0.3]:
         time.value += t
         bc_dx = dolfinx.fem.dirichletbc(time, dolfinx.fem.locate_dofs_geometrical(V, locator), V)
         u_bcx = dolfinx.fem.Function(V)
         dolfinx.fem.petsc.set_bc(u_bcx.vector, [bc_dx])
@@ -131,30 +133,31 @@
     """
 
     mesh = dolfinx.mesh.create_unit_square(MPI.COMM_WORLD, 10, 10)
 
     def locator(x):
         return np.isclose(x[0], 1)
 
-    time = dolfinx.fem.Constant(mesh, 1.)
+    time = dolfinx.fem.Constant(mesh, 1.0)
 
     entities = dolfinx.mesh.locate_entities(mesh, dim, locator)
     value = np.int32(3)
     et = dolfinx.mesh.meshtags(mesh, dim, entities, np.full(len(entities), value, dtype=np.int32))
     bc = DirichletBC(time, LocatorMethod.TOPOLOGICAL, (et, value))
 
-    V = dolfinx.fem.FunctionSpace(mesh, ("Lagrange", int(P)))
+    V = dolfinx.fem.functionspace(mesh, ("Lagrange", int(P)))
     bc.create_bc(V)
 
     for t in [0.1, 0.2, 0.3]:
         time.value += t
         u = dolfinx.fem.Function(V)
-        u.interpolate(lambda x: np.sin(x[0]) + x[1]*t)
+        u.interpolate(lambda x: np.sin(x[0]) + x[1] * t)
         bc_dx = dolfinx.fem.dirichletbc(
-            time, dolfinx.fem.locate_dofs_topological(V, dim, entities), V)
+            time, dolfinx.fem.locate_dofs_topological(V, dim, entities), V
+        )
 
         u_bcx = dolfinx.fem.Function(V)
         dolfinx.fem.petsc.set_bc(u_bcx.vector, [bc_dx])
 
         u_bc = dolfinx.fem.Function(V)
         bc.apply(u_bc.vector)
         assert np.allclose(u_bcx.x.array, u_bc.x.array)
@@ -163,46 +166,50 @@
 @pytest.mark.parametrize("P", np.arange(2, 4))
 def test_pressure_condition(P):
     mesh = dolfinx.mesh.create_unit_square(MPI.COMM_WORLD, 10, 10)
 
     def locator(x):
         return np.isclose(x[0], 1)
 
-    class TimeDependentBC():
+    class TimeDependentBC:
         def __init__(self, t: float):
             self.t = t
 
         def eval(self, x):
             return np.sin(x[0]) + x[1] * self.t
 
     condition_0 = TimeDependentBC(0.1)
 
-    entities = dolfinx.mesh.locate_entities(mesh, mesh.topology.dim-1, locator)
+    entities = dolfinx.mesh.locate_entities(mesh, mesh.topology.dim - 1, locator)
     value = np.int32(3)
-    et = dolfinx.mesh.meshtags(mesh, mesh.topology.dim-1, entities,
-                               np.full(len(entities), value, dtype=np.int32))
+    et = dolfinx.mesh.meshtags(
+        mesh,
+        mesh.topology.dim - 1,
+        entities,
+        np.full(len(entities), value, dtype=np.int32),
+    )
     bc = PressureBC(condition_0.eval, (et, value))
-    V = dolfinx.fem.FunctionSpace(mesh, ("Lagrange", int(P)))
-    Q = dolfinx.fem.FunctionSpace(mesh, ("Lagrange", int(P-1)))
+    V = dolfinx.fem.functionspace(mesh, ("Lagrange", int(P)))
+    Q = dolfinx.fem.functionspace(mesh, ("Lagrange", int(P - 1)))
     bc.create_bcs(V, Q)
     p = dolfinx.fem.Function(Q)
     p.interpolate(condition_0.eval)
     v = ufl.TestFunction(V)
     n = ufl.FacetNormal(mesh)
     ds = ufl.Measure("ds", domain=mesh, subdomain_data=et, subdomain_id=value)
     for i, ni in enumerate(n):
-        rhs = dolfinx.fem.form(p*n[i]*v.dx(i)*ds)
+        rhs = dolfinx.fem.form(p * n[i] * v.dx(i) * ds)
         b_form = dolfinx.fem.Function(V)
         dolfinx.fem.petsc.assemble_vector(b_form.vector, rhs)
         b_bc = dolfinx.fem.Function(V)
         dolfinx.fem.petsc.assemble_vector(b_bc.vector, dolfinx.fem.form(bc.rhs(i)))
         assert np.allclose(b_form.x.array, b_bc.x.array)
 
-    dofs = dolfinx.fem.locate_dofs_topological(Q, mesh.topology.dim-1, et.find(value))
-    bc_ex = dolfinx.fem.dirichletbc(0., dofs, Q)
+    dofs = dolfinx.fem.locate_dofs_topological(Q, mesh.topology.dim - 1, et.find(value))
+    bc_ex = dolfinx.fem.dirichletbc(0.0, dofs, Q)
     r = dolfinx.fem.Function(Q)
     r.x.array[:] = 10
     dolfinx.fem.petsc.set_bc(r.vector, [bc_ex])
 
     s = dolfinx.fem.Function(Q)
     s.x.array[:] = 10
     dolfinx.fem.petsc.set_bc(s.vector, [bc.bc])
```

### Comparing `OasisX-1.0.0/test/test_projector.py` & `oasisx-1.1.0/test/test_projector.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 # Copyright (C) 2022 Jørgen Schartum Dokken
 #
 # This file is part of Oasisx
 # SPDX-License-Identifier:    MIT
 
-from oasisx import Projector
+from mpi4py import MPI
 
-import dolfinx
 import basix.ufl
-import ufl
-from mpi4py import MPI
+import dolfinx
 import numpy as np
+import ufl
+
+from oasisx import Projector
 
 
 def test_projector():
     mesh = dolfinx.mesh.create_unit_square(MPI.COMM_WORLD, 10, 10)
-    V = dolfinx.fem.FunctionSpace(mesh, ("Lagrange", 2))
+    V = dolfinx.fem.functionspace(mesh, ("Lagrange", 2))
 
     # Interpolate initial solutiom
     u = dolfinx.fem.Function(V)
-    u.interpolate(lambda x: x[0]*x[0]+3*x[1]+2*x[1]*x[1])
+    u.interpolate(lambda x: x[0] * x[0] + 3 * x[1] + 2 * x[1] * x[1])
 
     # Create gradient projector
-    el = basix.ufl.element("DG", mesh.topology.cell_name(), 1,
-                           shape=(mesh.geometry.dim, ), gdim=mesh.geometry.dim)
-    W = dolfinx.fem.FunctionSpace(mesh, el)
-    petsc_options = {"ksp_type": "preonly", "pc_type": "lu",
-                     "pc_factor_mat_solver_type": "mumps"}
+    el = basix.ufl.element("DG", mesh.topology.cell_name(), 1, shape=(mesh.geometry.dim,))
+    W = dolfinx.fem.functionspace(mesh, el)
+    petsc_options = {
+        "ksp_type": "preonly",
+        "pc_type": "lu",
+        "pc_factor_mat_solver_type": "mumps",
+    }
     gradient_projector = Projector(ufl.grad(u), W, [], petsc_options=petsc_options)
     gradient_projector.solve()
 
     # assemle L2 error
     x = ufl.SpatialCoordinate(mesh)
-    u_ex = ufl.as_vector((2*x[0], 3+4*x[1]))
+    u_ex = ufl.as_vector((2 * x[0], 3 + 4 * x[1]))
     ph = gradient_projector.x
-    error_form = dolfinx.fem.form(ufl.inner(u_ex-ph, u_ex-ph)*ufl.dx)
+    error_form = dolfinx.fem.form(ufl.inner(u_ex - ph, u_ex - ph) * ufl.dx)
     L2_squared = dolfinx.fem.assemble_scalar(error_form)
-    u.interpolate(lambda x: x[0]+2*x[1]*x[1])
+    u.interpolate(lambda x: x[0] + 2 * x[1] * x[1])
     assert np.isclose(np.sqrt(L2_squared), 0.0, atol=1e-12)
 
     gradient_projector.assemble_rhs()
     gradient_projector.solve(assemble_rhs=False)
 
-    u_ex_new = ufl.as_vector((1, 4*x[1]))
-    new_error = dolfinx.fem.form(ufl.inner(u_ex_new-ph, u_ex_new-ph)*ufl.dx)
+    u_ex_new = ufl.as_vector((1, 4 * x[1]))
+    new_error = dolfinx.fem.form(ufl.inner(u_ex_new - ph, u_ex_new - ph) * ufl.dx)
     L2_squared_new = dolfinx.fem.assemble_scalar(new_error)
     assert np.isclose(np.sqrt(L2_squared_new), 0.0, atol=1e-12)
```

### Comparing `OasisX-1.0.0/test/test_tentative_velocity.py` & `oasisx-1.1.0/test/test_tentative_velocity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,79 +1,91 @@
 # Copyright (C) 2022 Jørgen Schartum Dokken
 #
 # This file is part of Oasisx
 # SPDX-License-Identifier:    MIT
 
 from typing import List, Optional, Tuple
 
+from mpi4py import MPI
+from petsc4py import PETSc
+
 import dolfinx
 import numpy as np
 import numpy.typing as npt
 import pytest
 import scipy.sparse
 import ufl
-from mpi4py import MPI
-from petsc4py import PETSc
 
 from oasisx import DirichletBC, FractionalStep_AB_CN, LocatorMethod, PressureBC
 
 
-def gather_PETScMatrix(A: PETSc.Mat,  # type: ignore
-                       comm: MPI.Comm,
-                       root: int = 0) -> scipy.sparse.csr_matrix:
+def gather_PETScMatrix(
+    A: PETSc.Mat,  # type: ignore
+    comm: MPI.Comm,
+    root: int = 0,
+) -> scipy.sparse.csr_matrix:
     """
     Given a distributed PETSc matrix, gather in on process 'root' in
     a scipy CSR matrix
     """
     ai, aj, av = A.getValuesCSR()
     aj_all = comm.gather(aj, root=root)  # type: ignore
     av_all = comm.gather(av, root=root)  # type: ignore
     ai_all = comm.gather(ai, root=root)  # type: ignore
     if comm.rank == root:
         ai_cum = [0]
         for ai in ai_all:  # type: ignore
             offsets = ai[1:] + ai_cum[-1]
             ai_cum.extend(offsets)
         return scipy.sparse.csr_matrix(
-            (np.hstack(av_all), np.hstack(aj_all), ai_cum), shape=A.getSize())  # type: ignore
-
-
-def create_tentative_forms(mesh: dolfinx.mesh.Mesh,
-                           el_u: Tuple[str, int],
-                           el_p: Tuple[str, int], dt: float, nu: float,
-                           f: Optional[npt.NDArray[np.float64]]) -> Tuple[ufl.Form, List[ufl.Form],
-                                                                          dolfinx.fem.Function,
-                                                                          dolfinx.fem.Function,
-                                                                          dolfinx.fem.Function]:
+            (np.hstack(av_all), np.hstack(aj_all), ai_cum),  # type: ignore
+            shape=A.getSize(),
+        )
+
+
+def create_tentative_forms(
+    mesh: dolfinx.mesh.Mesh,
+    el_u: Tuple[str, int],
+    el_p: Tuple[str, int],
+    dt: float,
+    nu: float,
+    f: Optional[npt.NDArray[np.float64]],
+) -> Tuple[
+    ufl.Form,
+    List[ufl.Form],
+    dolfinx.fem.Function,
+    dolfinx.fem.Function,
+    dolfinx.fem.Function,
+]:
     """
     Direct implementation of the i-th component of the tentative velocity equation
     """
 
-    V = dolfinx.fem.FunctionSpace(mesh, el_u)
-    Q = dolfinx.fem.FunctionSpace(mesh, el_p)
+    V = dolfinx.fem.functionspace(mesh, el_u)
+    Q = dolfinx.fem.functionspace(mesh, el_p)
 
     u = ufl.TrialFunction(V)
     v = ufl.TestFunction(V)
     p = dolfinx.fem.Function(Q)
     u_n = dolfinx.fem.Function(V)
     u_n2 = dolfinx.fem.Function(V)
 
     dx = ufl.Measure("dx", domain=mesh)
     u_ab = ufl.as_vector((1.5 * u_n - 0.5 * u_n2, 1.5 * u_n - 0.5 * u_n2))
     u_avg = 0.5 * (u + u_n)
-    F = 1./dt * (u - u_n) * v * dx
+    F = 1.0 / dt * (u - u_n) * v * dx
     F += ufl.dot(u_ab, ufl.grad(u_avg)) * v * dx
     F += nu * ufl.inner(ufl.grad(u_avg), ufl.grad(v)) * dx
     a, L = ufl.system(F)
     Ls = []
     for i in range(mesh.geometry.dim):
         if f is None:
-            Ls.append(L + p*v.dx(i)*dx)
+            Ls.append(L + p * v.dx(i) * dx)
         else:
-            Ls.append(L + p*v.dx(i)*dx + f[i]*v*dx)
+            Ls.append(L + p * v.dx(i) * dx + f[i] * v * dx)
 
     return a, Ls, u_n, u_n2, p
 
 
 @pytest.mark.parametrize("body_force", [True, False])
 @pytest.mark.parametrize("low_memory", [True, False])
 def test_tentative(low_memory, body_force):
@@ -103,47 +115,58 @@
     left_facets = dolfinx.mesh.locate_entities_boundary(mesh, dim, left_edge)
     left_value = 1
     tb_facets = dolfinx.mesh.locate_entities_boundary(mesh, dim, top_and_bottom)
     tb_value = 2
     right_facets = dolfinx.mesh.locate_entities_boundary(mesh, dim, outlet)
     right_value = 3
     facets = np.hstack([left_facets, tb_facets, right_facets])
-    values = np.hstack([np.full_like(left_facets, left_value, dtype=np.int32),
-                        np.full_like(tb_facets, tb_value, dtype=np.int32),
-                        np.full_like(right_facets, right_value, dtype=np.int32)])
+    values = np.hstack(
+        [
+            np.full_like(left_facets, left_value, dtype=np.int32),
+            np.full_like(tb_facets, tb_value, dtype=np.int32),
+            np.full_like(right_facets, right_value, dtype=np.int32),
+        ]
+    )
     sort = np.argsort(facets)
     facet_tags = dolfinx.mesh.meshtags(mesh, dim, facets[sort], values[sort])
 
     # Create boundary conditions
-    class Inlet():
+    class Inlet:
         def __init__(self, t):
             self.t = t
 
         def eval(self, x):
-            return (1+self.t) * np.sin(np.pi*x[1])
+            return (1 + self.t) * np.sin(np.pi * x[1])
 
     inlet = Inlet(0)
 
-    bc_tb = DirichletBC(0., LocatorMethod.TOPOLOGICAL, (facet_tags, tb_value))
+    bc_tb = DirichletBC(0.0, LocatorMethod.TOPOLOGICAL, (facet_tags, tb_value))
     bc_inlet_x = DirichletBC(inlet.eval, LocatorMethod.TOPOLOGICAL, (facet_tags, left_value))
-    bc_inlet_y = DirichletBC(0., LocatorMethod.TOPOLOGICAL, (facet_tags, left_value))
+    bc_inlet_y = DirichletBC(0.0, LocatorMethod.TOPOLOGICAL, (facet_tags, left_value))
     bcs_u = [[bc_inlet_x, bc_tb], [bc_inlet_y, bc_tb]]
-    p_value = 4.
+    p_value = 4.0
     bcs_p = [PressureBC(p_value, (facet_tags, right_value))]
 
     # Create fractional step solver
     solver = FractionalStep_AB_CN(
-        mesh, el_u, el_p, bcs_u=bcs_u, bcs_p=bcs_p,
-        solver_options=solver_options, options=options, body_force=f)
+        mesh,
+        el_u,
+        el_p,
+        bcs_u=bcs_u,
+        bcs_p=bcs_p,
+        solver_options=solver_options,
+        options=options,
+        body_force=f,
+    )
 
     dt = 0.1
     nu = 0.5
 
     # Set some almost sensible initial conditions
-    inlet.t = -2*dt
+    inlet.t = -2 * dt
     solver._u2[0].interpolate(inlet.eval)
     solver._u2[1].interpolate(inlet.eval)
     inlet.t = -dt
     solver._u1[0].interpolate(inlet.eval)
     solver._u1[1].interpolate(inlet.eval)
     inlet.t = dt
     bc_inlet_x.update_bc()
@@ -156,36 +179,47 @@
     # Reference implementation
     a, Ls, u_n, u_n2, p = create_tentative_forms(mesh, el_u, el_p, dt, nu, f)
     V = u_n.function_space
     # Create bcs and boundary conditions
     p.interpolate(lambda x: x[1])
     ux = dolfinx.fem.Function(V)
     ux.interpolate(inlet.eval)
-    inlet.t = -2*dt
+    inlet.t = -2 * dt
     u_n2.interpolate(inlet.eval)
     inlet.t = -dt
     u_n.interpolate(inlet.eval)
-    bcs_u = [[
-        dolfinx.fem.dirichletbc(ux, dolfinx.fem.locate_dofs_topological(V, dim, left_facets)),
-        dolfinx.fem.dirichletbc(0., dolfinx.fem.locate_dofs_topological(V, dim, tb_facets), V)],
-        [dolfinx.fem.dirichletbc(0., dolfinx.fem.locate_dofs_topological(V, dim, left_facets), V),
-         dolfinx.fem.dirichletbc(0., dolfinx.fem.locate_dofs_topological(V, dim, tb_facets), V)],
-        [dolfinx.fem.dirichletbc(0., dolfinx.fem.locate_dofs_topological(V, dim, left_facets), V),
-         dolfinx.fem.dirichletbc(0., dolfinx.fem.locate_dofs_topological(V, dim, tb_facets), V)]]
+    bcs_u = [
+        [
+            dolfinx.fem.dirichletbc(ux, dolfinx.fem.locate_dofs_topological(V, dim, left_facets)),
+            dolfinx.fem.dirichletbc(0.0, dolfinx.fem.locate_dofs_topological(V, dim, tb_facets), V),
+        ],
+        [
+            dolfinx.fem.dirichletbc(
+                0.0, dolfinx.fem.locate_dofs_topological(V, dim, left_facets), V
+            ),
+            dolfinx.fem.dirichletbc(0.0, dolfinx.fem.locate_dofs_topological(V, dim, tb_facets), V),
+        ],
+        [
+            dolfinx.fem.dirichletbc(
+                0.0, dolfinx.fem.locate_dofs_topological(V, dim, left_facets), V
+            ),
+            dolfinx.fem.dirichletbc(0.0, dolfinx.fem.locate_dofs_topological(V, dim, tb_facets), V),
+        ],
+    ]
     n = ufl.FacetNormal(mesh)
     v = ufl.TestFunction(V)
     ds = ufl.Measure("ds", domain=mesh, subdomain_data=facet_tags, subdomain_id=right_value)
     A = dolfinx.fem.petsc.assemble_matrix(dolfinx.fem.form(a))
     A.assemble()
     for bc in bcs_u[0]:
-        A.zeroRowsLocal(bc._cpp_object.dof_indices()[0], 1.)
+        A.zeroRowsLocal(bc._cpp_object.dof_indices()[0], 1.0)
     bs = []
     for i in range(mesh.geometry.dim):
         b = dolfinx.fem.petsc.assemble_vector(dolfinx.fem.form(Ls[i]))
-        dolfinx.fem.petsc.assemble_vector(b, dolfinx.fem.form(p_value*v.dx(i)*n[i]*ds))
+        dolfinx.fem.petsc.assemble_vector(b, dolfinx.fem.form(p_value * v.dx(i) * n[i] * ds))
         b.ghostUpdate(addv=PETSc.InsertMode.ADD, mode=PETSc.ScatterMode.REVERSE)
         dolfinx.fem.petsc.set_bc(b, bcs_u[i])
         b.ghostUpdate(addv=PETSc.InsertMode.INSERT, mode=PETSc.ScatterMode.FORWARD)
 
         bs.append(b)
 
     # Compare matrices
```

