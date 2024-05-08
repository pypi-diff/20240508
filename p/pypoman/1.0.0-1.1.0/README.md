# Comparing `tmp/pypoman-1.0.0.tar.gz` & `tmp/pypoman-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypoman-1.0.0.tar", last modified: Thu May 18 15:31:38 2023, max compression
+gzip compressed data, was "pypoman-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pypoman-1.0.0.tar` & `pypoman-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
--rw-r--r--   0        0        0     2742 2023-05-18 15:16:51.976844 pypoman-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0       80 2023-05-18 15:16:51.976844 pypoman-1.0.0/.gitignore
--rw-r--r--   0        0        0      681 2023-05-18 15:31:01.794211 pypoman-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    35141 2021-02-06 12:59:19.279343 pypoman-1.0.0/LICENSE
--rw-r--r--   0        0        0     4241 2022-05-30 20:21:12.028658 pypoman-1.0.0/README.md
--rw-r--r--   0        0        0        6 2021-02-06 12:59:19.279343 pypoman-1.0.0/doc/.gitignore
--rw-r--r--   0        0        0     1531 2023-02-02 13:58:26.059716 pypoman-1.0.0/doc/Makefile
--rw-r--r--   0        0        0     9244 2023-05-18 15:19:21.095529 pypoman-1.0.0/doc/src/conf.py
--rw-r--r--   0        0        0      956 2021-10-13 09:23:53.563423 pypoman-1.0.0/doc/src/index.rst
--rw-r--r--   0        0        0     1505 2021-10-13 09:35:52.660876 pypoman-1.0.0/examples/point_to_polytope_projection.py
--rw-r--r--   0        0        0     1678 2021-10-13 09:35:29.380588 pypoman-1.0.0/examples/polytope_projection.py
--rw-r--r--   0        0        0     2231 2021-10-13 09:33:53.575393 pypoman-1.0.0/examples/vertex_enumeration.py
--rw-r--r--   0        0        0     1776 2023-05-18 15:30:57.704534 pypoman-1.0.0/pypoman/__init__.py
--rw-r--r--   0        0        0     9426 2023-05-18 15:16:51.976844 pypoman-1.0.0/pypoman/bretl.py
--rw-r--r--   0        0        0     4848 2023-05-18 15:16:51.976844 pypoman-1.0.0/pypoman/duality.py
--rw-r--r--   0        0        0     5362 2023-05-18 15:16:51.976844 pypoman-1.0.0/pypoman/intersection.py
--rw-r--r--   0        0        0     3251 2023-05-18 15:19:50.511485 pypoman-1.0.0/pypoman/lp.py
--rw-r--r--   0        0        0     1876 2023-05-18 15:16:51.980844 pypoman-1.0.0/pypoman/misc.py
--rw-r--r--   0        0        0     5688 2023-05-18 15:20:32.783160 pypoman-1.0.0/pypoman/polygon.py
--rw-r--r--   0        0        0     2214 2023-05-18 15:20:53.807889 pypoman-1.0.0/pypoman/polyhedron.py
--rw-r--r--   0        0        0     8769 2023-05-18 15:16:51.980844 pypoman-1.0.0/pypoman/projection.py
--rw-r--r--   0        0        0     1846 2023-05-18 15:16:51.980844 pypoman-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       59 2023-05-18 15:16:51.980844 pypoman-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1403 2023-05-18 15:16:51.980844 pypoman-1.0.0/tests/test_halfspace_enumeration.py
--rw-r--r--   0        0        0     2407 2023-05-18 15:16:51.980844 pypoman-1.0.0/tests/test_vertex_enumeration.py
--rw-r--r--   0        0        0     1250 2023-05-18 15:16:51.980844 pypoman-1.0.0/tox.ini
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 pypoman-1.0.0/setup.py
--rw-r--r--   0        0        0     5680 1970-01-01 00:00:00.000000 pypoman-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3483 2024-05-08 17:14:04.593961 pypoman-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       89 2024-05-08 16:18:29.902306 pypoman-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1365 2024-05-08 17:14:25.773911 pypoman-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35141 2024-05-08 16:18:29.902306 pypoman-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4764 2024-05-08 16:39:46.569175 pypoman-1.1.0/README.md
+-rw-r--r--   0        0        0        6 2024-05-08 16:18:29.902306 pypoman-1.1.0/doc/.gitignore
+-rw-r--r--   0        0        0     1531 2024-05-08 16:18:29.902306 pypoman-1.1.0/doc/Makefile
+-rw-r--r--   0        0        0     4213 2024-01-01 07:09:57.523400 pypoman-1.1.0/doc/src/conf.py
+-rw-r--r--   0        0        0      956 2024-05-08 16:18:29.902306 pypoman-1.1.0/doc/src/index.rst
+-rw-r--r--   0        0        0      837 2024-01-01 07:05:42.063799 pypoman-1.1.0/examples/point_to_polytope_projection.py
+-rw-r--r--   0        0        0      960 2024-01-01 07:06:06.631760 pypoman-1.1.0/examples/polytope_projection.py
+-rw-r--r--   0        0        0     1407 2024-01-01 07:06:29.071725 pypoman-1.1.0/examples/vertex_enumeration.py
+-rw-r--r--   0        0        0     1085 2024-05-08 17:14:36.293886 pypoman-1.1.0/pypoman/__init__.py
+-rw-r--r--   0        0        0     8832 2024-05-08 16:36:25.761734 pypoman-1.1.0/pypoman/bretl.py
+-rw-r--r--   0        0        0     4155 2024-05-08 16:36:27.853731 pypoman-1.1.0/pypoman/duality.py
+-rw-r--r--   0        0        0     4671 2024-05-08 16:36:31.101726 pypoman-1.1.0/pypoman/intersection.py
+-rw-r--r--   0        0        0     2562 2024-05-08 16:36:32.865723 pypoman-1.1.0/pypoman/lp.py
+-rw-r--r--   0        0        0      525 2024-05-08 16:36:34.177721 pypoman-1.1.0/pypoman/misc.py
+-rw-r--r--   0        0        0     4961 2024-05-08 16:36:36.129717 pypoman-1.1.0/pypoman/polygon.py
+-rw-r--r--   0        0        0     1545 2024-05-08 16:36:37.437715 pypoman-1.1.0/pypoman/polyhedron.py
+-rw-r--r--   0        0        0     8212 2024-01-01 07:08:17.919556 pypoman-1.1.0/pypoman/projection.py
+-rw-r--r--   0        0        0     1940 2024-05-08 16:58:43.371599 pypoman-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-05-08 16:18:29.902306 pypoman-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2616 2024-05-08 17:14:04.593961 pypoman-1.1.0/tests/test_duality.py
+-rw-r--r--   0        0        0     2422 2024-01-01 07:08:26.855542 pypoman-1.1.0/tests/test_intersection.py
+-rw-r--r--   0        0        0      737 2024-01-01 07:08:31.439534 pypoman-1.1.0/tests/test_lp.py
+-rw-r--r--   0        0        0     1399 2024-01-01 07:08:34.711529 pypoman-1.1.0/tests/test_polygon.py
+-rw-r--r--   0        0        0      989 2024-01-01 07:08:38.119524 pypoman-1.1.0/tests/test_polyhedron.py
+-rw-r--r--   0        0        0     1957 2024-01-01 07:08:42.051518 pypoman-1.1.0/tests/test_projection.py
+-rw-r--r--   0        0        0     1180 2024-05-08 17:14:04.593961 pypoman-1.1.0/tox.ini
+-rw-r--r--   0        0        0     6314 1970-01-01 00:00:00.000000 pypoman-1.1.0/PKG-INFO
```

### Comparing `pypoman-1.0.0/.github/workflows/test.yml` & `pypoman-1.1.0/.github/workflows/ci.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,119 @@
 name: CI
 
 on:
     push:
-        branches: [ master ]
+        branches: [ main ]
     pull_request:
-        branches: [ master ]
+        branches: [ main ]
     workflow_dispatch:
 
 jobs:
-    lint:
-        name: "Code style"
+    coverage:
+        name: "Coverage"
         runs-on: ubuntu-latest
 
         steps:
             - name: "Checkout sources"
               uses: actions/checkout@v3
 
-            - name: "Set up Python ${{ matrix.python-version }}"
+            - name: "Set up Python 3.8"
               uses: actions/setup-python@v4
               with:
-                  python-version: "${{ matrix.python-version }}"
+                  python-version: "3.8"
 
-            - name: "Install dependencies"
+            - name: "Install Debian dependencies"
               run: |
-                  python -m pip install --upgrade pip
-                  python -m pip install tox
+                  sudo apt install libgmp3-dev
 
-            - name: "Test with tox for ${{ matrix.os }}"
+            - name: "Install PyPI dependencies"
               run: |
-                  tox -e lint
+                  python -m pip install --upgrade pip
+                  python -m pip install coveralls tox
+
+            - name: "Check code coverage"
               env:
                   MOSEKLM_LICENSE_FILE: ${{ secrets.MSK_LICENSE }}
-                  PLATFORM: ubuntu-latest
+              run: |
+                  tox -e coverage
 
-    coverage:
-        name: "Coverage"
+            - name: "Coveralls"
+              env:
+                  GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+              run: |
+                  coveralls --service=github --rcfile=pyproject.toml
+
+    lint:
+        name: "Code style"
         runs-on: ubuntu-latest
 
         steps:
             - name: "Checkout sources"
               uses: actions/checkout@v3
 
-            - name: "Set up Python 3.8"
+            - name: "Set up Python ${{ matrix.python-version }}"
               uses: actions/setup-python@v4
               with:
-                  python-version: "3.8"
+                  python-version: "${{ matrix.python-version }}"
 
-            - name: "Install dependencies"
+            - name: "Install Debian dependencies"
               run: |
-                  python -m pip install --upgrade pip
-                  python -m pip install coveralls tox
+                  sudo apt install libgmp3-dev
 
-            - name: "Check code coverage"
-              env:
-                  MOSEKLM_LICENSE_FILE: ${{ secrets.MSK_LICENSE }}
+            - name: "Install PyPI dependencies"
               run: |
-                  tox -e coverage
+                  python -m pip install --upgrade pip
+                  python -m pip install tox
 
-            - name: "Coveralls"
-              env:
-                  GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+            - name: "Test with tox for ${{ matrix.os }}"
               run: |
-                  coveralls --service=github --rcfile=pyproject.toml
+                  tox -e lint
+              env:
+                  MOSEKLM_LICENSE_FILE: ${{ secrets.MSK_LICENSE }}
+                  PLATFORM: ubuntu-latest
 
     test:
         name: "Test ${{ matrix.os }} with python-${{ matrix.python-version }}"
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
-                os: [ubuntu-latest, macos-latest, windows-latest]
+                os: [ubuntu-latest, windows-latest]
                 python-version: ["3.8", "3.9", "3.10"]
 
         steps:
             - name: "Checkout sources"
               uses: actions/checkout@v3
 
             - name: "Set up Python ${{ matrix.python-version }}"
               uses: actions/setup-python@v4
               with:
                   python-version: "${{ matrix.python-version }}"
 
-            - name: "Install dependencies"
+            - name: "Install Debian dependencies"
+              if: matrix.os == 'ubuntu-latest'
+              run: |
+                  sudo apt install libgmp-dev
+
+            - name: "Install macOS dependencies"
+              if: matrix.os == 'macos-latest'
+              run: |
+                  brew install gmp
+
+            - name: "Install PyPI dependencies"
               run: |
                   python -m pip install --upgrade pip
                   python -m pip install tox tox-gh-actions
 
             - name: "Test with tox for ${{ matrix.os }}"
               env:
                   MOSEKLM_LICENSE_FILE: ${{ secrets.MSK_LICENSE }}
                   PLATFORM: ${{ matrix.os }}
               run: |
                   tox
+
+    ci_success:
+        name: "CI success"
+        runs-on: ubuntu-latest
+        needs: [coverage, lint, test]
+        steps:
+            - run: echo "CI workflow completed successfully"
```

### Comparing `pypoman-1.0.0/LICENSE` & `pypoman-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypoman-1.0.0/README.md` & `pypoman-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # Polyhedron manipulation in Python
 
-[![PyPI package](https://img.shields.io/pypi/v/pypoman)](https://pypi.org/project/pypoman/)
-[![Documentation](https://img.shields.io/badge/documentation-online-brightgreen?logo=read-the-docs&style=flat)](https://scaron.info/doc/pypoman/)
-![Status](https://img.shields.io/pypi/status/pypoman)
+[![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/pypoman/ci.yml?branch=main)](https://github.com/stephane-caron/pypoman/actions)
+[![Coverage](https://coveralls.io/repos/github/stephane-caron/pypoman/badge.svg?branch=main)](https://coveralls.io/github/stephane-caron/pypoman?branch=main)
+[![Documentation](https://img.shields.io/badge/docs-online-brightgreen?logo=read-the-docs&style=flat)](https://scaron.info/doc/pypoman/)
+[![PyPI version](https://img.shields.io/pypi/v/pypoman)](https://pypi.org/project/pypoman/)
+[![PyPI downloads](https://pepy.tech/badge/pypoman/month)](https://pepy.tech/project/pypoman)
 
-This library allows common operations over [convex polyhedra](https://en.wikipedia.org/wiki/Convex_polyhedron) such as [polytope projection](https://scaron.info/doc/pypoman/index.html#module-pypoman.projection) and [vertex enumeration](https://scaron.info/doc/pypoman/index.html#module-pypoman.duality).
-
-See the [API documentation](https://scaron.info/doc/pypoman/) for details.
+This library allows common operations over [convex polyhedra](https://en.wikipedia.org/wiki/Convex_polyhedron) such as [polytope projection](https://scaron.info/doc/pypoman/index.html#module-pypoman.projection) and [vertex enumeration](https://scaron.info/doc/pypoman/index.html#module-pypoman.duality). Check out the [API documentation](https://scaron.info/doc/pypoman/) for details.
 
 ## Installation
 
-Install system packages (here for Debian-based distributions) for Python and GLPK by:
+Install system packages for Python and GLPK, for instance for Debian-based Linux distributions:
 
 ```console
-$ sudo apt-get install cython libglpk-dev python python-dev python-pip python-scipy
+$ sudo apt-get install cython libglpk-dev python python-dev python-pip
 ```
 
 Then, install the library by:
 
 ```console
 $ pip install pypoman
 ```
 
+Some functions, such as point-polytope projection and polygon intersection, are optional and not installed by default. To enable all of them, run:
+
+```console
+$ pip install pypoman[all]
+```
+
 ## Examples
 
 ### Vertex enumeration
 
 We can compute the list of vertices of a polytope described in halfspace representation by $A x \leq b$:
 
 ```python
@@ -98,21 +104,25 @@
 E = zeros((p, n))
 E[0, 0] = 1.
 E[1, 1] = 1.
 f = zeros(p)
 proj = (E, f)  # proj(x) = E * x + f
 
 vertices = project_polytope(proj, ineq, eq, method='bretl')
+```
+
+We can then plot the projected polytope:
+
+```python
+import pylab
 
-if __name__ == "__main__":   # plot projected polytope
-    import pylab
-    pylab.ion()
-    pylab.figure()
-    plot_polygon(vertices)
+pylab.ion()
+pylab.figure()
+plot_polygon(vertices)
 ```
 
 ## See also
 
-- A short introduction to [Polyhedra and polytopes](https://scaron.info/teaching/polyhedra-and-polytopes.html)
+- A short introduction to [Polyhedra and polytopes](https://scaron.info/blog/polyhedra-and-polytopes.html)
 - Komei Fukuda's [Frequently Asked Questions in Polyhedral Computation](https://www.inf.ethz.ch/personal/fukudak/polyfaq/polyfaq.html)
 - The [Polyhedron](http://doc.sagemath.org/html/en/reference/discrete_geometry/sage/geometry/polyhedron/constructor.html) class in [Sage](http://www.sagemath.org/)
 - [StabiliPy](https://github.com/haudren/stabilipy): a Python package implementing a more general recursive method for polytope projection
```

### Comparing `pypoman-1.0.0/doc/Makefile` & `pypoman-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pypoman-1.0.0/doc/src/index.rst` & `pypoman-1.1.0/doc/src/index.rst`

 * *Files identical despite different names*

### Comparing `pypoman-1.0.0/pypoman/bretl.py` & `pypoman-1.1.0/pypoman/bretl.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2016 Quang-Cuong Pham <cuong.pham@normalesup.org>
-# Copyright (C) 2017-2020 Stephane Caron <stephane.caron@normalesup.org>
-#
-# This file is part of pypoman <https://github.com/stephane-caron/pypoman>.
-#
-# pypoman is free software: you can redistribute it and/or modify it under the
-# terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
-#
-# pypoman is distributed in the hope that it will be useful, but WITHOUT ANY
-# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License along with
-# pypoman. If not, see <http://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: GPL-3.0-or-later
+# Copyright (C) 2016 Quang-Cuong Pham
+# Copyright (C) 2017 Stéphane Caron
 
 """Iterative projection algorithm by [Bretl08]_."""
 
 from typing import Any, List, Optional, Tuple, Union
 
 import numpy as np
 from numpy.random import random
@@ -39,16 +26,16 @@
 
     def __init__(self, p: Union[List[float], np.ndarray]):
         """
         Initialize vertex from point coordinates.
 
         Parameters
         ----------
-        p : array
-            2D coordinates.
+        p :
+            2D coordinates of the vertex.
         """
         self.x = p[0]
         self.y = p[1]
         self.next = None
         self.expanded = False
 
     def expand(
@@ -103,19 +90,19 @@
 
     def __init__(self, v1: Vertex, v2: Vertex, v3: Vertex):
         """
         Initialize polygon from inscribed triangle.
 
         Parameters
         ----------
-        v1 : array
+        v1 :
             First vertex of the initial triangle.
-        v2 : array
+        v2 :
             Second vertex of the initial triangle.
-        v3 : array
+        v3 :
             Third vertex of the initial triangle.
         """
         v1.next = v2
         v2.next = v3
         v3.next = v1
         self.vertices = [v1, v2, v3]
 
@@ -173,20 +160,23 @@
         Note
         ----
         Assumes all vertices are on the positive halfplane.
         """
         minsd = 1e10
         ibottom = 0
         for i in range(len(self.vertices)):
-            v = self.vertices[i]
-            if (v.y + v.next.y) < minsd:
+            vertex = self.vertices[i]
+            next_vertex = vertex.next
+            if next_vertex is None:
+                raise ValueError("Invalid expanded vertex with no successor")
+            if (vertex.y + next_vertex.y) < minsd:
                 ibottom = i
-                minsd = v.y + v.next.y
-        for v in self.vertices:
-            v.checked = False
+                minsd = vertex.y + next_vertex.y
+        for vertex in self.vertices:
+            vertex.checked = False
         vcur = self.vertices[ibottom]
         newvertices = []
         while not vcur.checked:
             vcur.checked = True
             newvertices.append(vcur)
             vcur = vcur.next
         newvertices.reverse()
@@ -222,20 +212,20 @@
     lp: Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray],
     solver: Optional[str] = GLPK_IF_AVAILABLE,
 ) -> np.ndarray:
     """Optimize in one direction.
 
     Parameters
     ----------
-    vdir : (3,) array
-        Direction in which the optimization is performed.
-    lp : array tuple
+    vdir :
+        Direction (3D vector) in which the optimization is performed.
+    lp :
         Tuple `(q, G, h, A, b)` defining the LP. See
         :func:`pypoman.lp..solve_lp` for details.
-    solver : string, optional
+    solver :
         Backend LP solver to call.
 
     Returns
     -------
     :
         Vector ``z`` representing the maximum vertex of the polygon in the
         direction `vdir`.
@@ -254,18 +244,18 @@
 ) -> np.ndarray:
     """Optimize in one direction.
 
     Parameters
     ----------
     theta :
         Angle of the direction in which the optimization is performed.
-    lp : array tuple
+    lp :
         Tuple `(q, G, h, A, b)` defining the LP. See
         :func:`pypoman.lp..solve_lp` for details.
-    solver : string, optional
+    solver :
         Backend LP solver to call.
 
     Returns
     -------
     :
         Vector ``z`` representing the maximum vertex of the polygon in the
         direction `vdir`.
@@ -309,14 +299,14 @@
             step *= 0.25 + 0.5 * random()
             theta += step - 2.0 * np.pi
         z = optimize_angle(theta, lp, solver)
         if all([norm(z - z0) > 1e-5 for z0 in init_vertices]):
             init_vertices.append(z)
         max_iter -= 1
     if len(init_vertices) < 3:
-        raise Exception("problem is not linearly feasible")
+        raise ValueError("problem is not linearly feasible")
     v0 = Vertex(init_vertices[0])
     v1 = Vertex(init_vertices[1])
     v2 = Vertex(init_vertices[2])
     polygon = Polygon(v0, v1, v2)
     polygon.iter_expand(lp, max_iter)
     return polygon
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pypoman-1.0.0/pypoman/intersection.py` & `pypoman-1.1.0/pypoman/intersection.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2018-2020 Stephane Caron <stephane.caron@normalesup.org>
-#
-# This file is part of pypoman <https://github.com/stephane-caron/pypoman>.
-#
-# pypoman is free software: you can redistribute it and/or modify it under the
-# terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
-#
-# pypoman is distributed in the hope that it will be useful, but WITHOUT ANY
-# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License along with
-# pypoman. If not, see <http://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: GPL-3.0-or-later
+# Copyright 2018 Stéphane Caron
 
 """Intersections between lines and polyhedra."""
 
 from typing import List, Tuple
 
 import numpy as np
 from scipy.spatial import ConvexHull
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pypoman-1.0.0/pypoman/lp.py` & `pypoman-1.1.0/pypoman/lp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2018-2020 Stephane Caron <stephane.caron@normalesup.org>
-#
-# This file is part of pypoman <https://github.com/stephane-caron/pypoman>.
-#
-# pypoman is free software: you can redistribute it and/or modify it under the
-# terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
-#
-# pypoman is distributed in the hope that it will be useful, but WITHOUT ANY
-# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License along with
-# pypoman. If not, see <http://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: GPL-3.0-or-later
+# Copyright 2018 Stéphane Caron
 
 """Functions for linear programming."""
 
 from typing import Optional, Union
+from warnings import warn
 
 import cvxopt
 import cvxopt.solvers
 import numpy as np
 from cvxopt.solvers import lp
 
-from .misc import warn
-
 cvxopt.solvers.options["show_progress"] = False  # disable cvxopt output
 
 GLPK_IF_AVAILABLE: Optional[str] = None
 try:
     import cvxopt.glpk
 
     GLPK_IF_AVAILABLE = "glpk"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pypoman-1.0.0/pypoman/polygon.py` & `pypoman-1.1.0/pypoman/polygon.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2018-2020 Stephane Caron <stephane.caron@normalesup.org>
-#
-# This file is part of pypoman <https://github.com/stephane-caron/pypoman>.
-#
-# pypoman is free software: you can redistribute it and/or modify it under the
-# terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
-#
-# pypoman is distributed in the hope that it will be useful, but WITHOUT ANY
-# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License along with
-# pypoman. If not, see <http://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: GPL-3.0-or-later
+# Copyright 2018 Stéphane Caron
 
 """Functions on polygons, that is, 2D polyhedra."""
 
+from typing import List, Optional
+
 import numpy as np
 from matplotlib.patches import Polygon
-from numpy import array, dot, hstack
 from pylab import axis, gca
 from scipy.spatial import ConvexHull
-from typing import List
 
 from .polyhedron import compute_chebyshev_center
 
 
 def __compute_polygon_hull(B: np.ndarray, c: np.ndarray):
     r"""Compute the vertex representation of a polygon.
 
@@ -50,42 +37,42 @@
     Returns
     -------
     vertices : list of arrays
         List of 2D vertices in counterclowise order.
 
     Notes
     -----
-    The origin [0, 0] should lie inside the polygon (:math:`c \\geq 0`) in
+    The origin [0, 0] should lie inside the polygon (:math:`c \geq 0`) in
     order to build the polar form. If you don't have this guarantee, call
     ``compute_polar_polygon()`` instead.
 
     Checking that :math:`c > 0` is not optional. The rest of the algorithm can
     be executed when some coordinates :math:`c_i < 0`, but the result would be
     wrong.
     """
     assert (
         B.shape[1] == 2
     ), "Input (B, c) is not a polygon: B.shape = %s" % str(B.shape)
     assert all(
         c > 0
     ), "Polygon should contain the origin, but min(c) = %.2f" % min(c)
 
-    B_polar = hstack(
+    B_polar = np.hstack(
         [
             (B[:, column] * 1.0 / c).reshape((B.shape[0], 1))
             for column in range(2)
         ]
     )
 
     def axis_intersection(i, j):
         ai, bi = c[i], B[i]
         aj, bj = c[j], B[j]
         x = (ai * bj[1] - aj * bi[1]) * 1.0 / (bi[0] * bj[1] - bj[0] * bi[1])
         y = (bi[0] * aj - bj[0] * ai) * 1.0 / (bi[0] * bj[1] - bj[0] * bi[1])
-        return array([x, y])
+        return np.array([x, y])
 
     # QHULL OPTIONS:
     #
     # - ``Pp`` -- do not report precision problems
     # - ``Q0`` -- no merging with C-0 and Qx
     #
     # ``Q0`` avoids [this bug](https://github.com/scipy/scipy/issues/6484).
@@ -128,54 +115,54 @@
     -------
     :
         List of 2D vertices in counterclockwise order.
     """
     x = None
     if not all(c > 0):
         x = compute_chebyshev_center(B, c)
-        c = c - dot(B, x)
+        c = c - np.dot(B, x)
     if not all(c > 0):
-        raise Exception("Polygon is empty (min. dist. to edge %.2f)" % min(c))
+        raise ValueError("Polygon is empty (min. dist. to edge %.2f)" % min(c))
     vertices = __compute_polygon_hull(B, c)
     if x is not None:
         vertices = [v + x for v in vertices]
     return vertices
 
 
 def plot_polygon(
-    points,
-    alpha=0.4,
-    color="g",
-    linestyle="solid",
-    fill=True,
-    linewidth=None,
-    resize=False,
-):
+    points: np.ndarray,
+    alpha: float = 0.4,
+    color: str = "g",
+    linestyle: str = "solid",
+    fill: bool = True,
+    linewidth: Optional[float] = None,
+    resize: bool = False,
+) -> None:
     """
     Plot a polygon in matplotlib.
 
     Parameters
     ----------
-    points : list of arrays
-        List of poitns.
-    alpha : scalar, optional
+    points :
+        Array or list of points.
+    alpha :
         Transparency value.
-    color : string, optional
+    color :
         Color in matplotlib format.
-    linestyle : scalar, optional
+    linestyle :
         Line style in matplotlib format.
-    fill : bool, optional
+    fill :
         When ``True``, fills the area inside the polygon.
-    linewidth : scalar, optional
+    linewidth :
         Line width in matplotlib format.
-    resize : bool, optional
+    resize :
         When ``True``, resets axis limits to center on the polygon.
     """
-    if type(points) is list:
-        points = array(points)
+    if isinstance(points, list):
+        points = np.array(points)
     ax = gca()
     hull = ConvexHull(points)
     points = points[hull.vertices, :]
     if resize:
         xmin1, xmax1, ymin1, ymax1 = axis()
         xmin2, ymin2 = 1.5 * points.min(axis=0)
         xmax2, ymax2 = 1.5 * points.max(axis=0)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pypoman-1.0.0/pypoman/projection.py` & `pypoman-1.1.0/pypoman/projection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2018-2020 Stephane Caron <stephane.caron@normalesup.org>
-#
-# This file is part of pypoman <https://github.com/stephane-caron/pypoman>.
-#
-# pypoman is free software: you can redistribute it and/or modify it under the
-# terms of the GNU General Public License as published by the Free Software
-# Foundation, either version 3 of the License, or (at your option) any later
-# version.
-#
-# pypoman is distributed in the hope that it will be useful, but WITHOUT ANY
-# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License along with
-# pypoman. If not, see <http://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: GPL-3.0-or-later
+# Copyright 2018 Stéphane Caron
 
 """Polytope projection functions."""
 
 from typing import List, Optional, Tuple
 
 import cdd
 import cvxopt
@@ -158,46 +145,51 @@
         return project_polytope_bretl(proj, ineq, eq, **kwargs)
     vertices, rays = project_polyhedron(proj, ineq, eq)
     assert not rays, "Projection is not a polytope"
     return vertices
 
 
 def project_polytope_bretl(
-    proj, ineq, eq, max_radius=1e5, max_iter=1000, init_angle=None
-):
+    proj: Tuple[np.ndarray, np.ndarray],
+    ineq: Tuple[np.ndarray, np.ndarray],
+    eq: Tuple[np.ndarray, np.ndarray],
+    max_radius: float = 1e5,
+    max_iter: int = 1000,
+    init_angle: Optional[float] = None,
+) -> List[np.ndarray]:
     r"""Project a polytope into a 2D polygon using the IP algorithm.
 
     The incremental projection algorithm is detailed in [Bretl08]_. The 2D
     affine projection :math:`y = E x + f` is applied to the polyhedron defined
     by:
 
     .. math::
 
         A x & \leq b \\
         C x & = d
 
     Parameters
     ----------
-    proj : pair of arrays
+    proj :
         Pair (`E`, `f`) describing the affine projection.
-    ineq : pair of arrays
+    ineq :
         Pair (`A`, `b`) describing the inequality constraint.
-    eq : pair of arrays, optional
+    eq :
         Pair (`C`, `d`) describing the equality constraint.
-    max_radius : scalar, optional
+    max_radius :
         Maximum distance from origin (in [m]) used to make sure the output
         is bounded.
-    max_iter : integer, optional
+    max_iter :
         Maximum number of calls to the LP solver.
-    init_angle : scalar, optional
+    init_angle :
         Angle in [rad] giving the direction of the initial ray cast.
 
     Returns
     -------
-    vertices : list of arrays
+    :
         List of vertices of the projected polygon.
     """
     (E, f), (A, b), (C, d) = proj, ineq, eq
     assert E.shape[0] == f.shape[0] == 2
 
     # Inequality constraints: A_ext * [ x  u  v ] <= b_ext iff
     # (1) A * x <= b and (2) |u|, |v| <= max_radius
@@ -234,38 +226,44 @@
     )
     polygon.sort_vertices()
     vertices_list = polygon.export_vertices()
     vertices = [np.array([v.x, v.y]) for v in vertices_list]
     return vertices
 
 
-def project_point_to_polytope(point, ineq, solver="quadprog", **kwargs):
+def project_point_to_polytope(
+    point: np.ndarray,
+    ineq: Tuple[np.ndarray, np.ndarray],
+    qpsolver: str,
+    **kwargs,
+) -> np.ndarray:
     """
     Projet a point onto a polytope in H-representation.
 
     Parameters
     ----------
-    point : array
+    point :
         Point to project.
-    ineq : pair of arrays
+    ineq :
         Pair (`A`, `b`) describing the inequality constraint.
-    solver : string
-        Name of the quadratic programming solver to use.
+    qpsolver :
+        Name of the backend quadratic programming solver to use, to be picked
+        in ``qpsolvers.available_solvers``.
 
     Returns
     -------
-    projection : array
+    :
         Projected point.
 
     Note
     ----
     This function requires `qpsolvers <https://pypi.org/project/qpsolvers/>`_.
     """
     try:
         from qpsolvers import solve_ls
     except ImportError as e:
         raise ImportError(
             "This function requires qpsolvers: pip install qpsolvers"
         ) from e
 
     P = np.eye(len(point))
-    return solve_ls(P, point, G=ineq[0], h=ineq[1], solver=solver, **kwargs)
+    return solve_ls(P, point, G=ineq[0], h=ineq[1], solver=qpsolver, **kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pypoman-1.0.0/pyproject.toml` & `pypoman-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,45 +15,50 @@
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
 ]
 dependencies = [
-    "cvxopt",
-    "matplotlib",
-    "numpy",
-    "pycddlib",
-    "scipy",
+    "cvxopt >=1.2.6",
+    "matplotlib >=3.3.4",
+    "numpy >=1.15.4",
+    "pycddlib >=2.1.4",
+    "scipy >=1.7.0",
 ]
 keywords = ["convex, polyhedron, polyhedra, polytope, projection, duality"]
 
+[project.optional-dependencies]
+all = [
+    "pyclipper >=1.3.0",
+    "qpsolvers >=3.3.1",
+]
+
 [project.urls]
 Documentation = "https://scaron.info/doc/pypoman/"
 Source = "https://github.com/stephane-caron/pypoman"
 Tracker = "https://github.com/stephane-caron/pypoman/issues"
-Changelog = "https://github.com/stephane-caron/pypoman/blob/master/CHANGELOG.md"
+Changelog = "https://github.com/stephane-caron/pypoman/blob/main/CHANGELOG.md"
 
 [tool.black]
 line-length = 79
 
 [tool.coverage]
 report.include = ["pypoman/*"]
 
-[tool.ruff]
+[tool.lint]
 line-length = 79
 select = [
     # pyflakes
     "F",
     # pycodestyle
     "E",
     "W",
@@ -63,9 +68,9 @@
     "D"
 ]
 ignore = [
     "D401",  # good for methods but not for class docstrings
     "D405",  # British-style section names are also "proper"!
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
```

### Comparing `pypoman-1.0.0/PKG-INFO` & `pypoman-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 Metadata-Version: 2.1
 Name: pypoman
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python module for polyhedral geometry.
 Keywords: convex, polyhedron, polyhedra, polytope, projection, duality
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Requires-Dist: cvxopt
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: pycddlib
-Requires-Dist: scipy
-Project-URL: Changelog, https://github.com/stephane-caron/pypoman/blob/master/CHANGELOG.md
+Requires-Dist: cvxopt >=1.2.6
+Requires-Dist: matplotlib >=3.3.4
+Requires-Dist: numpy >=1.15.4
+Requires-Dist: pycddlib >=2.1.4
+Requires-Dist: scipy >=1.7.0
+Requires-Dist: pyclipper >=1.3.0 ; extra == "all"
+Requires-Dist: qpsolvers >=3.3.1 ; extra == "all"
+Project-URL: Changelog, https://github.com/stephane-caron/pypoman/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://scaron.info/doc/pypoman/
 Project-URL: Source, https://github.com/stephane-caron/pypoman
 Project-URL: Tracker, https://github.com/stephane-caron/pypoman/issues
+Provides-Extra: all
 
 # Polyhedron manipulation in Python
 
-[![PyPI package](https://img.shields.io/pypi/v/pypoman)](https://pypi.org/project/pypoman/)
-[![Documentation](https://img.shields.io/badge/documentation-online-brightgreen?logo=read-the-docs&style=flat)](https://scaron.info/doc/pypoman/)
-![Status](https://img.shields.io/pypi/status/pypoman)
+[![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/pypoman/ci.yml?branch=main)](https://github.com/stephane-caron/pypoman/actions)
+[![Coverage](https://coveralls.io/repos/github/stephane-caron/pypoman/badge.svg?branch=main)](https://coveralls.io/github/stephane-caron/pypoman?branch=main)
+[![Documentation](https://img.shields.io/badge/docs-online-brightgreen?logo=read-the-docs&style=flat)](https://scaron.info/doc/pypoman/)
+[![PyPI version](https://img.shields.io/pypi/v/pypoman)](https://pypi.org/project/pypoman/)
+[![PyPI downloads](https://pepy.tech/badge/pypoman/month)](https://pepy.tech/project/pypoman)
 
-This library allows common operations over [convex polyhedra](https://en.wikipedia.org/wiki/Convex_polyhedron) such as [polytope projection](https://scaron.info/doc/pypoman/index.html#module-pypoman.projection) and [vertex enumeration](https://scaron.info/doc/pypoman/index.html#module-pypoman.duality).
-
-See the [API documentation](https://scaron.info/doc/pypoman/) for details.
+This library allows common operations over [convex polyhedra](https://en.wikipedia.org/wiki/Convex_polyhedron) such as [polytope projection](https://scaron.info/doc/pypoman/index.html#module-pypoman.projection) and [vertex enumeration](https://scaron.info/doc/pypoman/index.html#module-pypoman.duality). Check out the [API documentation](https://scaron.info/doc/pypoman/) for details.
 
 ## Installation
 
-Install system packages (here for Debian-based distributions) for Python and GLPK by:
+Install system packages for Python and GLPK, for instance for Debian-based Linux distributions:
 
 ```console
-$ sudo apt-get install cython libglpk-dev python python-dev python-pip python-scipy
+$ sudo apt-get install cython libglpk-dev python python-dev python-pip
 ```
 
 Then, install the library by:
 
 ```console
 $ pip install pypoman
 ```
 
+Some functions, such as point-polytope projection and polygon intersection, are optional and not installed by default. To enable all of them, run:
+
+```console
+$ pip install pypoman[all]
+```
+
 ## Examples
 
 ### Vertex enumeration
 
 We can compute the list of vertices of a polytope described in halfspace representation by $A x \leq b$:
 
 ```python
@@ -130,22 +138,26 @@
 E = zeros((p, n))
 E[0, 0] = 1.
 E[1, 1] = 1.
 f = zeros(p)
 proj = (E, f)  # proj(x) = E * x + f
 
 vertices = project_polytope(proj, ineq, eq, method='bretl')
+```
+
+We can then plot the projected polytope:
+
+```python
+import pylab
 
-if __name__ == "__main__":   # plot projected polytope
-    import pylab
-    pylab.ion()
-    pylab.figure()
-    plot_polygon(vertices)
+pylab.ion()
+pylab.figure()
+plot_polygon(vertices)
 ```
 
 ## See also
 
-- A short introduction to [Polyhedra and polytopes](https://scaron.info/teaching/polyhedra-and-polytopes.html)
+- A short introduction to [Polyhedra and polytopes](https://scaron.info/blog/polyhedra-and-polytopes.html)
 - Komei Fukuda's [Frequently Asked Questions in Polyhedral Computation](https://www.inf.ethz.ch/personal/fukudak/polyfaq/polyfaq.html)
 - The [Polyhedron](http://doc.sagemath.org/html/en/reference/discrete_geometry/sage/geometry/polyhedron/constructor.html) class in [Sage](http://www.sagemath.org/)
 - [StabiliPy](https://github.com/haudren/stabilipy): a Python package implementing a more general recursive method for polytope projection
```

