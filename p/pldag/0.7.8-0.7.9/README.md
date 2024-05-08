# Comparing `tmp/pldag-0.7.8.tar.gz` & `tmp/pldag-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.7.8.tar", max compression
+gzip compressed data, was "pldag-0.7.9.tar", max compression
```

## Comparing `pldag-0.7.8.tar` & `pldag-0.7.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.7.8/LICENSE
--rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.7.8/README.md
--rw-r--r--   0        0        0    34855 2024-05-01 13:43:39.180071 pldag-0.7.8/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.7.8/pldag/solver/__init__.py
--rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.7.8/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-05-01 13:44:02.390036 pldag-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.7.9/LICENSE
+-rw-r--r--   0        0        0     2833 2024-05-07 07:16:43.962166 pldag-0.7.9/README.md
+-rw-r--r--   0        0        0    35534 2024-05-07 11:41:07.325798 pldag-0.7.9/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.7.9/pldag/solver/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.7.9/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-05-07 11:42:26.996979 pldag-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 pldag-0.7.9/PKG-INFO
```

### Comparing `pldag-0.7.8/LICENSE` & `pldag-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.7.8/README.md` & `pldag-0.7.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,33 +23,33 @@
 
 # Later if we forget the ID, we can retrieve it like this
 id_ref_again = model.id_from_alias("A")
 assert id_ref == id_ref_again
 
 # So if we check when all x, y and z are set to 1, then we
 # expect `id_ref` to be 1+1j
-assert model.test({"x": 1+1j, "y": 1+1j, "z": 1+1j}).get(id_ref) == 1+1j
+assert model.propagate({"x": 1+1j, "y": 1+1j, "z": 1+1j}).get(id_ref) == 1+1j
 
 # And then not all are set, we'll get just 1j (meaning the model doesn't now whether it's true or false)
-assert model.test({"x": 1+1j, "y": 1+1j, "z": 1j}).get(id_ref) == 1j
+assert model.propagate({"x": 1+1j, "y": 1+1j, "z": 1j}).get(id_ref) == 1j
 
 # However, if we now that any variable is not set, being equal to 0, then the model know the composite to be false (or 0j)
-assert model.test({"x": 1+1j, "y": 1+1j, "z": 0j}).get(id_ref) == 0j
+assert model.propagate({"x": 1+1j, "y": 1+1j, "z": 0j}).get(id_ref) == 0j
 ```
 
 There's also a quick way to use a solver. There's no built-in solver but is dependent on existing once. Before using, reinstall the package with the solver variable set to the solver you'd want to use
 ```bash
 pip install pldag[glpk]
 ``` 
 And then you can use it like following
 ```python
 
 from pldag import Solver
 
 # Maximize [x=1, y=0, z=0] such that rules in model holds and variable `id_ref` must be true.
-solution = next(iter(model.solve(objectives=[{"x": 1}], fix={id_ref: 1}, solver=Solver.GLPK)))
+solution = next(iter(model.solve(objectives=[{"x": 1}], assume={id_ref: 1+1j}, solver=Solver.GLPK)))
 
 # Since x=1 and `id_ref` must be set (i.e. all(x,y,z) must be true), we could expect all variables
 # be set.
 assert solution.get(id_ref) == 1+1j
 
 ```
```

### Comparing `pldag-0.7.8/pldag/__init__.py` & `pldag-0.7.9/pldag/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -365,15 +365,15 @@
             )
         )
     
     def negated(self, id: str) -> bool:
         """Get the negated state of the given id"""
         return bool(self._nvec[self._row(id)])
 
-    def propagate_downstream(self, query: dict = {}, freeze: bool = True) -> dict:
+    def propagate(self, query: dict = {}, freeze: bool = True) -> dict:
         """
             Propagates the graph downstream, towards the root node(s), and returns the propagated bounds.
 
             Examples
             --------
             >>> model = PLDAG()
             >>> model.set_primitives("xy")
@@ -640,14 +640,38 @@
                 The ID of the composite constraint.
         """
         return self.set_and([
             self.set_atleast(references, 1),
             self.set_atmost(references, 1),
         ], alias)
     
+    def set_xnor(self, references: List[str], alias: Optional[str] = None) -> str:
+        """
+            Add a composite constraint of an XNOR operation.
+
+            Parameters
+            ----------
+            references : List[str]
+                The references to composite constraints or primitive variables.
+
+            Examples
+            --------
+            >>> model = PLDAG()
+            >>> model.set_primitives("xy")
+            >>> a = model.set_xnor(["x", "y"])
+            >>> model.test({"x": 1+1j, "y": 0j}).get(a)
+            0j
+
+            Returns
+            -------
+            str
+                The ID of the composite constraint.
+        """
+        return self.set_not([self.set_xor(references)], alias)
+    
     def set_imply(self, condition: str, consequence: str, alias: Optional[str] = None) -> str:
         """
             Add a composite constraint of an IMPLY operation.
 
             Parameters
             ----------
             condition : str
@@ -682,31 +706,20 @@
             Add a composite constraint of an EQUAL operation.
 
             Parameters
             ----------
             references : List[str]
                 The references to composite constraints or primitive variables.
 
-            Examples
-            --------
-            >>> model = PLDAG()
-            >>> model.set_primitives("xy")
-            >>> a = model.set_equal("x", "y")
-            >>> model.test({"x": 1j, "y": 1j}).get(a)
-            1j
-
-            >>> model.test({"x": 1+1j, "y": 0j}).get(a)
-            0j
-
             Returns
             -------
             str
                 The ID of the composite constraint.
         """
-        return self.set_xor([
+        return self.set_or([
             self.set_and(references),
             self.set_not(references),
         ], alias)
     
     @lru_cache
     def to_polyhedron(self, double_binding: bool = True, **assume: Dict[str, complex]) -> tuple:
 
@@ -738,16 +751,20 @@
         # 2) +mx*A + sum(-X) >= -(d-1)       (+A v -X)
 
         # For atmost constraints:
         # 1) (-mx-d)A + sum(-X) >= -mx       (-A v +X)
         # 2) (-d+mn+1)A + sum(+X) >= (-d+1)     (+A v -X)
 
         # Create the matrix
-        A = np.zeros((self._amat.shape[0] * 2, self._amat.shape[1]), dtype=np.int64)
-        b = np.zeros(self._amat.shape[0] * 2, dtype=np.int64)
+        if double_binding:
+            A = np.zeros((self._amat.shape[0] * 2, self._amat.shape[1]), dtype=np.int64)
+            b = np.zeros(self._amat.shape[0] * 2, dtype=np.int64)
+        else:
+            A = np.zeros(self._amat.shape, dtype=np.int64)
+            b = np.zeros(self._amat.shape[0], dtype=np.int64)
 
         # Find max of inner bounds for each composite
         ad = self._amat.dot(self._dvec)
         mn = ad.real
         mx = ad.imag
 
         # Extract `d` vector from bias
@@ -761,19 +778,21 @@
         A_X = np.unique(A_X_ri)
         # X -> A row indices
         X_A_ri = adj_points.T[0] + adj_points.T[0].max() + 1
         X_A = np.unique(X_A_ri)
 
         # Fill the matrix with adjacency points
         A[A_X_ri, adj_points.T[1]] = -1
-        A[X_A_ri, adj_points.T[1]] = -1
+        if double_binding:
+            A[X_A_ri, adj_points.T[1]] = -1
 
         # Assign 1 instead of -1 to the at least A -> X, and at most constraints for X -> A.
         A[A_X[~self._nvec], :] *= -1
-        A[X_A[self._nvec], :] *= -1
+        if double_binding:
+            A[X_A[self._nvec], :] *= -1
 
         # Composite index in matrix
         cidx = np.array(list(self._imap.values()))[self._cvec]
 
         # Set coef and bias for at least aux variable A->X
         # 1) (-d+mn)A + sum(-X) >= mn            (-A v +X)
         A[A_X[~self._nvec], cidx[~self._nvec]] = -d[~self._nvec]+mn[~self._nvec]
@@ -962,15 +981,15 @@
             [{'x': 0j, 'y': 1+1j, 'z': 0j}]
 
             Returns
             -------
             List[Dict[str, complex]]
                 The solutions for the objectives.
         """
-        A, b = self.to_polyhedron(**assume)
+        A, b = self.to_polyhedron(double_binding=True, **assume)
         variables = self._col_vars
         obj_mat = np.zeros((len(objectives), len(variables)), dtype=np.int64)
         for i, obj in enumerate(objectives):
             obj_mat[i, [self._col(k) for k in obj]] = list(obj.values())
 
         if solver == Solver.GLPK:
             from pldag.solver.glpk_solver import solve_lp
```

### Comparing `pldag-0.7.8/pldag/solver/glpk_solver.py` & `pldag-0.7.9/pldag/solver/glpk_solver.py`

 * *Files identical despite different names*

### Comparing `pldag-0.7.8/PKG-INFO` & `pldag-0.7.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.7.8
+Version: 0.7.9
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -39,34 +39,34 @@
 
 # Later if we forget the ID, we can retrieve it like this
 id_ref_again = model.id_from_alias("A")
 assert id_ref == id_ref_again
 
 # So if we check when all x, y and z are set to 1, then we
 # expect `id_ref` to be 1+1j
-assert model.test({"x": 1+1j, "y": 1+1j, "z": 1+1j}).get(id_ref) == 1+1j
+assert model.propagate({"x": 1+1j, "y": 1+1j, "z": 1+1j}).get(id_ref) == 1+1j
 
 # And then not all are set, we'll get just 1j (meaning the model doesn't now whether it's true or false)
-assert model.test({"x": 1+1j, "y": 1+1j, "z": 1j}).get(id_ref) == 1j
+assert model.propagate({"x": 1+1j, "y": 1+1j, "z": 1j}).get(id_ref) == 1j
 
 # However, if we now that any variable is not set, being equal to 0, then the model know the composite to be false (or 0j)
-assert model.test({"x": 1+1j, "y": 1+1j, "z": 0j}).get(id_ref) == 0j
+assert model.propagate({"x": 1+1j, "y": 1+1j, "z": 0j}).get(id_ref) == 0j
 ```
 
 There's also a quick way to use a solver. There's no built-in solver but is dependent on existing once. Before using, reinstall the package with the solver variable set to the solver you'd want to use
 ```bash
 pip install pldag[glpk]
 ``` 
 And then you can use it like following
 ```python
 
 from pldag import Solver
 
 # Maximize [x=1, y=0, z=0] such that rules in model holds and variable `id_ref` must be true.
-solution = next(iter(model.solve(objectives=[{"x": 1}], fix={id_ref: 1}, solver=Solver.GLPK)))
+solution = next(iter(model.solve(objectives=[{"x": 1}], assume={id_ref: 1+1j}, solver=Solver.GLPK)))
 
 # Since x=1 and `id_ref` must be set (i.e. all(x,y,z) must be true), we could expect all variables
 # be set.
 assert solution.get(id_ref) == 1+1j
 
 ```
```

