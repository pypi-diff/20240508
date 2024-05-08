# Comparing `tmp/jax_control_algorithms-0.5.2.tar.gz` & `tmp/jax_control_algorithms-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_control_algorithms-0.5.2.tar", last modified: Wed Mar 27 12:58:03 2024, max compression
+gzip compressed data, was "jax_control_algorithms-0.6.3.tar", last modified: Wed May  8 09:38:01 2024, max compression
```

## Comparing `jax_control_algorithms-0.5.2.tar` & `jax_control_algorithms-0.6.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:58:03.828221 jax_control_algorithms-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-03-27 12:58:03.828221 jax_control_algorithms-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:58:03.824221 jax_control_algorithms-0.5.2/jax_control_algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/jax_control_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/jax_control_algorithms/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/jax_control_algorithms/estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/jax_control_algorithms/jax_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/jax_control_algorithms/plot_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/jax_control_algorithms/sysident.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:58:03.824221 jax_control_algorithms-0.5.2/jax_control_algorithms/trajectory_optim/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/jax_control_algorithms/trajectory_optim/boundary_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/jax_control_algorithms/trajectory_optim/cost_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/jax_control_algorithms/trajectory_optim/dynamics_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/jax_control_algorithms/trajectory_optim/outer_loop_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/jax_control_algorithms/trajectory_optim/penality_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/jax_control_algorithms/trajectory_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/jax_control_algorithms/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:58:03.828221 jax_control_algorithms-0.5.2/jax_control_algorithms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-03-27 12:58:03.000000 jax_control_algorithms-0.5.2/jax_control_algorithms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-27 12:58:03.000000 jax_control_algorithms-0.5.2/jax_control_algorithms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 12:58:03.000000 jax_control_algorithms-0.5.2/jax_control_algorithms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-27 12:58:03.000000 jax_control_algorithms-0.5.2/jax_control_algorithms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 12:58:03.000000 jax_control_algorithms-0.5.2/jax_control_algorithms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 12:58:03.828221 jax_control_algorithms-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:58:03.828221 jax_control_algorithms-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/tests/test_jax_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-27 12:57:53.000000 jax_control_algorithms-0.5.2/tests/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:38:01.456378 jax_control_algorithms-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-08 09:38:01.456378 jax_control_algorithms-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:38:01.456378 jax_control_algorithms-0.6.3/jax_control_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/jax_control_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/jax_control_algorithms/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/jax_control_algorithms/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/jax_control_algorithms/jax_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/jax_control_algorithms/plot_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/jax_control_algorithms/sysident.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:38:01.456378 jax_control_algorithms-0.6.3/jax_control_algorithms/trajectory_optim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/jax_control_algorithms/trajectory_optim/boundary_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/jax_control_algorithms/trajectory_optim/cost_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/jax_control_algorithms/trajectory_optim/dynamics_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/jax_control_algorithms/trajectory_optim/outer_loop_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/jax_control_algorithms/trajectory_optim/penality_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/jax_control_algorithms/trajectory_optim/problem_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14401 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/jax_control_algorithms/trajectory_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/jax_control_algorithms/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:38:01.456378 jax_control_algorithms-0.6.3/jax_control_algorithms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-08 09:38:01.000000 jax_control_algorithms-0.6.3/jax_control_algorithms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-08 09:38:01.000000 jax_control_algorithms-0.6.3/jax_control_algorithms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:38:01.000000 jax_control_algorithms-0.6.3/jax_control_algorithms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 09:38:01.000000 jax_control_algorithms-0.6.3/jax_control_algorithms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 09:38:01.000000 jax_control_algorithms-0.6.3/jax_control_algorithms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:38:01.460378 jax_control_algorithms-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:38:01.456378 jax_control_algorithms-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/tests/test_jax_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-08 09:37:54.000000 jax_control_algorithms-0.6.3/tests/test_notebooks.py
```

### Comparing `jax_control_algorithms-0.5.2/LICENSE` & `jax_control_algorithms-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_control_algorithms-0.5.2/PKG-INFO` & `jax_control_algorithms-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax_control_algorithms
-Version: 0.5.2
+Version: 0.6.3
 Summary: Algorithms for state estimation, control, and system identification in JAX
 Author-email: Christian Klauer <chr.klauer@gmail.com>
 Project-URL: Homepage, https://github.com/christianausb/controlAlgorithms
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `jax_control_algorithms-0.5.2/README.md` & `jax_control_algorithms-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `jax_control_algorithms-0.5.2/jax_control_algorithms/common.py` & `jax_control_algorithms-0.6.3/jax_control_algorithms/common.py`

 * *Files identical despite different names*

### Comparing `jax_control_algorithms-0.5.2/jax_control_algorithms/estimation.py` & `jax_control_algorithms-0.6.3/jax_control_algorithms/estimation.py`

 * *Files identical despite different names*

### Comparing `jax_control_algorithms-0.5.2/jax_control_algorithms/jax_helper.py` & `jax_control_algorithms-0.6.3/jax_control_algorithms/jax_helper.py`

 * *Files identical despite different names*

### Comparing `jax_control_algorithms-0.5.2/jax_control_algorithms/plot_helpers.py` & `jax_control_algorithms-0.6.3/jax_control_algorithms/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `jax_control_algorithms-0.5.2/jax_control_algorithms/sysident.py` & `jax_control_algorithms-0.6.3/jax_control_algorithms/sysident.py`

 * *Files identical despite different names*

### Comparing `jax_control_algorithms-0.5.2/jax_control_algorithms/trajectory_optim/boundary_function.py` & `jax_control_algorithms-0.6.3/jax_control_algorithms/trajectory_optim/boundary_function.py`

 * *Files identical despite different names*

### Comparing `jax_control_algorithms-0.5.2/jax_control_algorithms/trajectory_optim/cost_function.py` & `jax_control_algorithms-0.6.3/jax_control_algorithms/trajectory_optim/cost_function.py`

 * *Files identical despite different names*

### Comparing `jax_control_algorithms-0.5.2/jax_control_algorithms/trajectory_optim/dynamics_constraints.py` & `jax_control_algorithms-0.6.3/jax_control_algorithms/trajectory_optim/dynamics_constraints.py`

 * *Files identical despite different names*

### Comparing `jax_control_algorithms-0.5.2/jax_control_algorithms/trajectory_optim/outer_loop_solver.py` & `jax_control_algorithms-0.6.3/jax_control_algorithms/trajectory_optim/outer_loop_solver.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import jax
 import jax.numpy as jnp
 import jaxopt
+from functools import partial
 
 from jax_control_algorithms.jax_helper import *
+from jax_control_algorithms.trajectory_optim.penality_method import control_convergence_of_iteration
+from jax_control_algorithms.trajectory_optim.problem_definition import *
+from jax_control_algorithms.trajectory_optim.penality_method import eval_objective_of_penalty_method
 """
     Implements the nested solver loops
 
     - An outer loop varies parameters for the penalty method, while
     - the inner solver (BGFS) is executed in each iteration of the outer loop to solve 
       the non-linear optimization problem that is defined by the penalty method
 
@@ -27,183 +31,193 @@
 
         s*(x < 0) = infinity
         s*(x >= 0) = 0
 
 """
 
 
-def _print_loop_info(loop_par, is_max_iter_reached_and_not_finished, print_errors):
-    lax.cond(loop_par['is_abort'], lambda: jax.debug.print("-> abort as convergence has stopped"), lambda: None)
+def _print_loop_info(loop_par: OuterLoopVariables, is_max_iter_reached_and_not_finished, print_errors):
+    lax.cond(loop_par.is_abort, lambda: jax.debug.print("-> abort as convergence has stopped"), lambda: None)
     if print_errors:
         lax.cond(
             is_max_iter_reached_and_not_finished,
             lambda: jax.debug.print("❌ max. iterations reached without a feasible solution"), lambda: None
         )
-        lax.cond(jnp.logical_not(loop_par['is_X_finite']), lambda: jax.debug.print("❌ found non finite numerics"), lambda: None)
+        lax.cond(jnp.logical_not(loop_par.is_X_finite), lambda: jax.debug.print("❌ found non finite numerics"), lambda: None)
 
 
-def _iterate(i, loop_var, solver_settings, objective_fn, verification_fn):
+def _iterate(loop_var: OuterLoopVariables, functions, solver_settings : SolverSettings):
+
+    i = loop_var.i
 
     # get the penalty parameter
-    penalty_parameter = loop_var['penalty_parameter_trace'][i]
-    is_maximal_penalty_parameter_reached = i >= loop_var['penalty_parameter_trace'].shape[0] - 1
+    penalty_parameter = loop_var.penalty_parameter_trace[i]
+    n_outer_iterations_target = loop_var.penalty_parameter_trace.shape[0]
+    is_maximal_penalty_parameter_reached = i >= n_outer_iterations_target - 1
 
     #
-    parameters_passed_to_inner_solver = loop_var['parameters_of_dynamic_model'] + (
+    parameters_passed_to_inner_solver = loop_var.parameters_of_dynamic_model + (
         penalty_parameter,
-        loop_var['opt_c_eq'],
+        loop_var.opt_c_eq,
     )
 
     # run inner solver
-    gd = jaxopt.BFGS(fun=objective_fn, value_and_grad=False, tol=loop_var['tol_inner'], maxiter=solver_settings['max_iter_inner'])
-    res = gd.run(loop_var['variables'], parameters=parameters_passed_to_inner_solver)
+    # objective_fn = eval_feasibility_metric_of_penalty_method(variables, parameters_of_dynamic_model, functions : Functions)
+    objective_fn = partial(eval_objective_of_penalty_method, functions=functions)
+
+    gd = jaxopt.BFGS(fun=objective_fn, value_and_grad=False, tol=loop_var.tol_inner, maxiter=solver_settings.max_iter_inner)
+    res = gd.run(loop_var.variables, parameters=parameters_passed_to_inner_solver)
     variables_updated_by_inner_solver = res.params
 
-    # run callback to verify the solution
-    verification_state_next, is_solution_feasible, is_equality_constraints_fulfilled, is_abort, is_X_finite, i_best = verification_fn(
-        loop_var['verification_state'], i, res, variables_updated_by_inner_solver, loop_var['parameters_of_dynamic_model'],
-        penalty_parameter
+    # run verify the solution and control the convergence of to the equality constraints
+    (
+        controller_state_next, is_equality_constraints_fulfilled, is_abort, is_X_finite, i_best,
+        max_eq_error, opt_c_eq_next, lam
+    ) = control_convergence_of_iteration(
+        loop_var.controller_state,
+        i,
+        n_outer_iterations_target,
+        res,
+        variables_updated_by_inner_solver,
+        loop_var.parameters_of_dynamic_model,
+        penalty_parameter,
+        loop_var.opt_c_eq,
+        loop_var.lam,
+        functions,
+        eq_tol=solver_settings.eq_tol,
+        verbose=True
     )
 
     # update the state of the optimization variables in case the outer loop shall not be aborted
-    variables_next = tree_where(is_abort, loop_var['variables'], variables_updated_by_inner_solver)
-
-    # update opt_c_eq: in case the equality constraints are not satisfies yet, increase opt_c_eq by multiplication with lam > 1
-    # otherwise leave opt_c_eq untouched.
-    opt_c_eq_next = loop_var['opt_c_eq'] * jnp.where(is_equality_constraints_fulfilled, 1.0, loop_var['lam'])
+    variables_next = tree_where(is_abort, loop_var.variables, variables_updated_by_inner_solver)
 
     # solution found?
-    is_finished = jnp.logical_and(is_solution_feasible, is_maximal_penalty_parameter_reached)
+    is_finished = jnp.logical_and(controller_state_next.is_converged, is_maximal_penalty_parameter_reached)
 
-    return variables_next, verification_state_next, opt_c_eq_next, is_finished, is_abort, is_X_finite
+    return variables_next, controller_state_next, opt_c_eq_next, lam, is_finished, is_abort, is_X_finite
 
 
 def _run_outer_loop(
-    i, variables, parameters_of_dynamic_model, opt_c_eq, verification_state_init, solver_settings, objective_fn, verification_fn,
-    verbose, print_errors, target_dtype
+    i, variables, model_to_solve: ModelToSolve, opt_c_eq, verification_state_init, solver_settings : SolverSettings, verbose, print_errors,
+    target_dtype
 ):
     """
         Execute the outer loop of the optimization process: herein in each iteration, the parameters of the
         boundary function and the quality cost weight factor are adjusted so that in the final iteration 
         the equality and inequality constraints are fulfilled.
     """
 
     # convert dtypes to the target datatype used in the computation
     (
         variables,
-        parameters_of_dynamic_model,
+        # model_to_solve,
         penalty_parameter_trace,
         opt_c_eq,
         verification_state_init,
-        lam,
         tol_inner,
     ) = convert_dtype(
         (
             variables,
-            parameters_of_dynamic_model,
-            solver_settings['penalty_parameter_trace'],
+            # model_to_solve.parameters_of_dynamic_model, # model_to_solve, # model_to_solve.
+            solver_settings.penalty_parameter_trace,
             opt_c_eq,
             verification_state_init,
-            solver_settings['lam'],
-            solver_settings['tol_inner'],
-        ), target_dtype
+            solver_settings.tol_inner,
+        ),
+        target_dtype
     )
 
     # loop:
-    def run_outer_loop_body(loop_var):
+    def run_outer_loop_body(loop_var: OuterLoopVariables):
 
         # loop iteration variable i
-        i = loop_var['i']
+        i = loop_var.i
 
-        variables_next, verification_state_next, opt_c_eq_next, is_finished, is_abort, is_X_finite = _iterate(
-            i, loop_var, solver_settings, objective_fn, verification_fn
+        variables_next, verification_state_next, opt_c_eq_next, lam, is_finished, is_abort, is_X_finite = _iterate(
+            loop_var, model_to_solve.functions, solver_settings
         )
 
         if verbose:
             lax.cond(is_finished, lambda: jax.debug.print("✅ found feasible solution"), lambda: None)
 
-        loop_var = {
-            'is_finished': is_finished,
-            'is_abort': is_abort,
-            'is_X_finite': is_X_finite,
-            'variables': variables_next,
-            'parameters_of_dynamic_model': loop_var['parameters_of_dynamic_model'],
-            'penalty_parameter_trace': penalty_parameter_trace,
-            'opt_c_eq': opt_c_eq_next,
-            'i': loop_var['i'] + 1,
-            'verification_state': verification_state_next,
-            'tol_inner': loop_var['tol_inner'],
-            'lam': loop_var['lam'],
-        }
+        loop_var = OuterLoopVariables(
+            is_finished=is_finished,
+            is_abort=is_abort,
+            is_X_finite=is_X_finite,
+            variables=variables_next,
+            parameters_of_dynamic_model=loop_var.parameters_of_dynamic_model,
+            penalty_parameter_trace=penalty_parameter_trace,
+            opt_c_eq=opt_c_eq_next,
+            lam=lam,
+            i=loop_var.i + 1,
+            controller_state=verification_state_next,
+            tol_inner=loop_var.tol_inner,
+        )
 
         return loop_var
 
-    def eval_outer_loop_condition(loop_var):
-        is_n_iter_not_reached = loop_var['i'] < solver_settings['max_iter_boundary_method']
+    def eval_outer_loop_condition(loop_var: OuterLoopVariables):
+        is_n_iter_not_reached = loop_var.i < solver_settings.max_iter_boundary_method
 
         is_max_iter_reached_and_not_finished = jnp.logical_and(
             jnp.logical_not(is_n_iter_not_reached),
-            jnp.logical_not(loop_var['is_finished']),
+            jnp.logical_not(loop_var.is_finished),
         )
 
         is_continue_iteration = jnp.logical_and(
-            jnp.logical_not(loop_var['is_abort']),
-            jnp.logical_and(jnp.logical_not(loop_var['is_finished']), is_n_iter_not_reached)
+            jnp.logical_not(loop_var.is_abort), jnp.logical_and(jnp.logical_not(loop_var.is_finished), is_n_iter_not_reached)
         )
 
         if verbose:
             _print_loop_info(loop_var, is_max_iter_reached_and_not_finished, print_errors)
 
         return is_continue_iteration
 
     # variables that are passed amount the loop-iterations
-    loop_var = {
-        'is_finished': jnp.array(False, dtype=jnp.bool_),
-        'is_abort': jnp.array(False, dtype=jnp.bool_),
-        'is_X_finite': jnp.array(True, dtype=jnp.bool_),
-        'variables': variables,
-        'parameters_of_dynamic_model': parameters_of_dynamic_model,
-        'penalty_parameter_trace': penalty_parameter_trace,
-        'opt_c_eq': opt_c_eq,
-        'i': i,
-        'verification_state': verification_state_init,
-        'tol_inner': tol_inner,
-        'lam': lam,
-    }
+    loop_var = OuterLoopVariables(
+        is_finished=jnp.array(False, dtype=jnp.bool_),
+        is_abort=jnp.array(False, dtype=jnp.bool_),
+        is_X_finite=jnp.array(True, dtype=jnp.bool_),
+        variables=variables,
+        parameters_of_dynamic_model=model_to_solve.parameters_of_dynamic_model,
+        penalty_parameter_trace=penalty_parameter_trace,
+        opt_c_eq=opt_c_eq,
+        lam=jnp.array(jnp.nan),
+        i=i,
+        controller_state=verification_state_init,
+        tol_inner=tol_inner,
+    )
 
-    loop_var = lax.while_loop(eval_outer_loop_condition, run_outer_loop_body, loop_var)
+    loop_var: OuterLoopVariables = lax.while_loop(eval_outer_loop_condition, run_outer_loop_body, loop_var)
 
-    n_iter = loop_var['i']
+    n_iter = loop_var.i
 
-    return loop_var['variables'], loop_var['opt_c_eq'], n_iter, loop_var['verification_state']
+    return loop_var.variables, loop_var.opt_c_eq, n_iter, loop_var.controller_state
 
 
 def run_outer_loop_solver(
-    variables, parameters_of_dynamic_model, solver_settings, trace_init, objective_, verification_fn_, max_float32_iterations,
-    enable_float64, verbose
+    variables, model_to_solve, solver_settings : SolverSettings, trace_init, max_float32_iterations, enable_float64, verbose
 ):
     """
         execute the solution finding process
     """
 
-    opt_c_eq = solver_settings['c_eq_init']
+    opt_c_eq = solver_settings.c_eq_init
     i = 0
-    verification_state = (trace_init, jnp.array(0, dtype=jnp.bool_))
+    verification_state = ConvergenceControllerState(trace=trace_init, is_converged=jnp.array(0, dtype=jnp.bool_))
 
     # iterations that are performed using float32 datatypes
     if max_float32_iterations > 0:
         variables, opt_c_eq, n_iter_f32, verification_state = _run_outer_loop(
             i,
             variables,
-            parameters_of_dynamic_model,
+            model_to_solve,
             jnp.array(opt_c_eq, dtype=jnp.float32),
             verification_state,
             solver_settings,
-            objective_,
-            verification_fn_,
             verbose,
             True if verbose else False,  # show_errors
             target_dtype=jnp.float32
         )
 
         i = i + n_iter_f32
 
@@ -214,20 +228,18 @@
             )
 
     # iterations that are performed using float64 datatypes
     if enable_float64:
         variables, opt_c_eq, n_iter_f64, verification_state = _run_outer_loop(
             i,
             variables,
-            parameters_of_dynamic_model,
+            model_to_solve,
             jnp.array(opt_c_eq, dtype=jnp.float64),
             verification_state,
             solver_settings,
-            objective_,
-            verification_fn_,
             verbose,
             True if verbose else False,  # show_errors
             target_dtype=jnp.float64
         )
         i = i + n_iter_f64
 
     n_iter = i
```

### Comparing `jax_control_algorithms-0.5.2/jax_control_algorithms/trajectory_optimization.py` & `jax_control_algorithms-0.6.3/jax_control_algorithms/trajectory_optimization.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,61 +10,54 @@
 
 from dataclasses import dataclass
 from typing import Callable
 
 from jax_control_algorithms.trajectory_optim.dynamics_constraints import eval_dynamics_equality_constraints
 from jax_control_algorithms.trajectory_optim.penality_method import *
 from jax_control_algorithms.trajectory_optim.outer_loop_solver import run_outer_loop_solver
+from jax_control_algorithms.trajectory_optim.problem_definition import *
 
 """
     Perform trajectory optimization of a dynamic system by finding the control sequence that 
     minimizes a cost function under inequality constraints. Terminal constraints are optional.
 
 """
 
-@dataclass(frozen=True)
-class Functions:
-    f: Callable
-    initial_guess: Callable = None
-    g: Callable = None
-    terminal_constraints: Callable = None
-    inequality_constraints: Callable = None
-    cost: Callable = None
-    running_cost: Callable = None
-    transform_parameters: Callable = None
+
+
+@dataclass
+class SolverReturn:
+    is_converged: bool
+    n_iter: jnp.ndarray
+    c_eq: jnp.ndarray
+    c_ineq: jnp.ndarray
+    trace: tuple
 
 
 @dataclass()
 class ProblemDefinition:
     functions: Functions
     x0: jnp.ndarray
     parameters: any = None
 
-    def run(self, x0=None, parameters=None, verbose: bool = False, solver_settings=None):
+    def run(self, x0=None, parameters=None, verbose: bool = False, solver_settings:SolverSettings=None) -> SolverReturn:
         solver_return = optimize_trajectory(
             self.functions,
             self.x0 if x0 is None else x0,
             self.parameters if parameters is None else parameters,
             get_default_solver_settings() if solver_settings is None else solver_settings,
             enable_float64=True,
             max_float32_iterations=0,
             max_trace_entries=100,
             verbose=verbose,
         )
 
         return solver_return
 
 
-@dataclass
-class SolverReturn:
-    is_converged: bool
-    n_iter: jnp.ndarray
-    c_eq: jnp.ndarray
-    c_ineq: jnp.ndarray
-    trace: tuple
 
 
 def constraint_geq(x, v):
     """
         define 'greater than' inequality constraint
         
         x >= v
@@ -102,40 +95,29 @@
 
     assert X_guess.shape[0] == n_steps
     assert X_guess.shape[1] == n_states
 
     return
 
 
-def generate_penalty_parameter_trace(t_start, t_final, n_steps):
-    """
-    Generate a sequence of penalty factors to be used in the optimization process
 
-    Args:
-        t_start: Initial penalty parameter t of the penalty method
-        t_final: maximal penalty parameter t to apply
-        n_steps: the length of the trace
-    """
-    lam = (t_final / t_start)**(1 / (n_steps - 1))
-    t_trace = t_start * lam**jnp.arange(n_steps)
-    return t_trace, lam
 
 
-def get_default_solver_settings():
-
-    solver_settings = {
-        'max_iter_boundary_method': 40,
-        'max_iter_inner': 5000,
-        'c_eq_init': 100.0,
-        'lam': 1.6,
-        'eq_tol': 0.0001,
-        'penalty_parameter_trace': generate_penalty_parameter_trace(t_start=0.5, t_final=100.0, n_steps=13)[0],
-        'tol_inner': 0.0001,
-    }
+def get_default_solver_settings() -> SolverSettings:
+
+    # solver_settings = {
+    #     'max_iter_boundary_method': 40,
+    #     'max_iter_inner': 5000,
+    #     'c_eq_init': 100.0,
+    #     'eq_tol': 0.0001,
+    #     'penalty_parameter_trace': generate_penalty_parameter_trace(t_start=0.5, t_final=100.0, n_steps=13)[0],
+    #     'tol_inner': 0.0001,
+    # }
 
+    solver_settings = SolverSettings()
     return solver_settings
 
 
 def _transform_parameters(functions, parameters):
 
     #
     if callable(functions.transform_parameters):
@@ -356,42 +338,27 @@
             n_states=n_states,
             n_inputs=n_inputs
         )
 
     K = _build_sampling_index_vector(n_steps)
 
     # pack parameters and variables
-    parameters_of_dynamic_model = (K, parameters, x0)
-    static_parameters = (
-        functions.f, functions.terminal_constraints, functions.inequality_constraints, functions.cost, functions.running_cost
-    )
+    model_to_solve = ModelToSolve(functions=functions, parameters_of_dynamic_model=ParametersOfModelToSolve(K=K, x0=x0, parameters=parameters))
     variables = (X_guess, U_guess)
 
-    # pass static parameters into objective function
-    objective_ = partial(eval_objective_of_penalty_method, static_parameters=static_parameters)
-    feasibility_metric_ = partial(eval_feasibility_metric_of_penalty_method, static_parameters=static_parameters)
-
-    # verification function (non specific to given problem to solve)
-    verification_fn_ = partial(
-        verify_convergence_of_iteration,
-        feasibility_metric_fn=feasibility_metric_,
-        eq_tol=solver_settings['eq_tol'],
-        verbose=verbose
-    )
-
     # trace vars
     trace_init = init_trace_memory(
         max_trace_entries, (jnp.float32, jnp.float32, jnp.int32, jnp.float32, jnp.float32),
         (jnp.nan, jnp.nan, -1, jnp.nan * jnp.zeros_like(X_guess), jnp.nan * jnp.zeros_like(U_guess))
     )
 
     # run solver
     variables_star, is_converged, n_iter, trace = run_outer_loop_solver(
-        variables, parameters_of_dynamic_model, solver_settings, trace_init, objective_, verification_fn_, max_float32_iterations,
-        enable_float64, verbose
+        variables, model_to_solve, solver_settings, trace_init,
+        max_float32_iterations, enable_float64, verbose
     )
 
     # unpack results for optimized variables
     X_opt, U_opt = variables_star
 
     # evaluate the constraint functions one last time to return the residuals
     c_eq = eval_dynamics_equality_constraints(functions.f, functions.terminal_constraints, X_opt, U_opt, K, x0, parameters)
@@ -417,22 +384,22 @@
 
 
 class Solver:
     """
         High-level interface to the solver
     """
 
-    def __init__(self, problem_def_fn):
+    def __init__(self, problem_def_fn, solver_settings : SolverSettings = get_default_solver_settings()):
         self.problem_def_fn = problem_def_fn
 
         # get problem definition
         self.problem_definition = problem_def_fn()
         assert type(self.problem_definition) is ProblemDefinition
 
-        self.solver_settings = get_default_solver_settings()
+        self.solver_settings = solver_settings
 
         self.enable_float64 = True
         self.max_float32_iterations = 0
         self.verbose = True
 
         # status of latest run
         self.success = False
```

### Comparing `jax_control_algorithms-0.5.2/jax_control_algorithms/ui.py` & `jax_control_algorithms-0.6.3/jax_control_algorithms/ui.py`

 * *Files identical despite different names*

### Comparing `jax_control_algorithms-0.5.2/jax_control_algorithms.egg-info/PKG-INFO` & `jax_control_algorithms-0.6.3/jax_control_algorithms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax_control_algorithms
-Version: 0.5.2
+Version: 0.6.3
 Summary: Algorithms for state estimation, control, and system identification in JAX
 Author-email: Christian Klauer <chr.klauer@gmail.com>
 Project-URL: Homepage, https://github.com/christianausb/controlAlgorithms
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `jax_control_algorithms-0.5.2/jax_control_algorithms.egg-info/SOURCES.txt` & `jax_control_algorithms-0.6.3/jax_control_algorithms.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,10 @@
 jax_control_algorithms.egg-info/requires.txt
 jax_control_algorithms.egg-info/top_level.txt
 jax_control_algorithms/trajectory_optim/boundary_function.py
 jax_control_algorithms/trajectory_optim/cost_function.py
 jax_control_algorithms/trajectory_optim/dynamics_constraints.py
 jax_control_algorithms/trajectory_optim/outer_loop_solver.py
 jax_control_algorithms/trajectory_optim/penality_method.py
+jax_control_algorithms/trajectory_optim/problem_definition.py
 tests/test_jax_helper.py
 tests/test_notebooks.py
```

### Comparing `jax_control_algorithms-0.5.2/pyproject.toml` & `jax_control_algorithms-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "testbook",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jax_control_algorithms"
-version = "0.5.2"
+version = "0.6.3"
 authors = [
   { name="Christian Klauer", email="chr.klauer@gmail.com" },
 ]
 description = "Algorithms for state estimation, control, and system identification in JAX"
 readme = "README.md"
 
 dependencies = [
```

### Comparing `jax_control_algorithms-0.5.2/tests/test_jax_helper.py` & `jax_control_algorithms-0.6.3/tests/test_jax_helper.py`

 * *Files identical despite different names*

### Comparing `jax_control_algorithms-0.5.2/tests/test_notebooks.py` & `jax_control_algorithms-0.6.3/tests/test_notebooks.py`

 * *Files identical despite different names*

