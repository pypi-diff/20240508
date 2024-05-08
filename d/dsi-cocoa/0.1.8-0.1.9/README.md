# Comparing `tmp/dsi_cocoa-0.1.8.tar.gz` & `tmp/dsi_cocoa-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsi_cocoa-0.1.8.tar", last modified: Tue May  7 15:48:06 2024, max compression
+gzip compressed data, was "dsi_cocoa-0.1.9.tar", last modified: Wed May  8 16:13:41 2024, max compression
```

## Comparing `dsi_cocoa-0.1.8.tar` & `dsi_cocoa-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:48:06.648960 dsi_cocoa-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:48:06.644960 dsi_cocoa-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:48:06.648960 dsi_cocoa-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/.github/workflows/main.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/.github/workflows/publish.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-07 15:48:06.648960 dsi_cocoa-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/eval-repo.sh
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-07 15:48:06.648960 dsi_cocoa-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:48:06.644960 dsi_cocoa-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:48:06.648960 dsi_cocoa-0.1.8/src/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/src/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/src/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/src/cocoa/evaluate_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/src/cocoa/linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/src/cocoa/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/src/cocoa/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-07 15:48:02.000000 dsi_cocoa-0.1.8/src/cocoa/spring2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:48:06.648960 dsi_cocoa-0.1.8/src/dsi_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-07 15:48:06.000000 dsi_cocoa-0.1.8/src/dsi_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-07 15:48:06.000000 dsi_cocoa-0.1.8/src/dsi_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:48:06.000000 dsi_cocoa-0.1.8/src/dsi_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 15:48:06.000000 dsi_cocoa-0.1.8/src/dsi_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 15:48:06.000000 dsi_cocoa-0.1.8/src/dsi_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 15:48:06.000000 dsi_cocoa-0.1.8/src/dsi_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:41.268186 dsi_cocoa-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:41.264186 dsi_cocoa-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:41.264186 dsi_cocoa-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/.github/workflows/main.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/.github/workflows/publish.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-08 16:13:41.268186 dsi_cocoa-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/eval-repo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-08 16:13:41.268186 dsi_cocoa-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:41.264186 dsi_cocoa-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:41.268186 dsi_cocoa-0.1.9/src/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/src/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/src/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/src/cocoa/evaluate_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/src/cocoa/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/src/cocoa/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/src/cocoa/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/src/cocoa/spring2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:41.268186 dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-08 16:13:41.000000 dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-08 16:13:41.000000 dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:13:41.000000 dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 16:13:41.000000 dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 16:13:41.000000 dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 16:13:41.000000 dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/top_level.txt
```

### Comparing `dsi_cocoa-0.1.8/.github/workflows/main.workflow.yml` & `dsi_cocoa-0.1.9/.github/workflows/main.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.8/.github/workflows/publish.workflow.yml` & `dsi_cocoa-0.1.9/.github/workflows/publish.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.8/.gitignore` & `dsi_cocoa-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.8/.pre-commit-config.yaml` & `dsi_cocoa-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.8/PKG-INFO` & `dsi_cocoa-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.1.8
+Version: 0.1.9
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dsi_cocoa-0.1.8/README.md` & `dsi_cocoa-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.8/pyproject.toml` & `dsi_cocoa-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.8/src/cocoa/evaluate_repo.py` & `dsi_cocoa-0.1.9/src/cocoa/evaluate_repo.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,80 +54,99 @@
             for f in files
             if not any(x in os.path.join(root, f) for x in paths_to_flag)
         ]
 
     for file_path in files_to_process:
         if os.path.exists(file_path):
             if file_path.endswith(".ipynb") or file_path.endswith(".py"):
-                print(f"Analyzing {file_path}:")
                 if file_path.endswith(".ipynb"):
                     analyze_notebook(file_path, no_filter_flag, verbose)
                 elif file_path.endswith(".py"):
                     analyze_python_file(file_path, lint_flag, verbose)
-                print("-" * 80)
 
 
 def analyze_notebook(file_path, no_filter_flag, verbose):
     """Analyze a notebook"""
     num_cells, num_lines, num_functions, max_lines_in_cell = process_notebook(
         file_path
     )
     pyflake_results = pyflakes_notebook(file_path)
-    print_results("PyFlakes", pyflake_results, verbose=verbose)
-    if no_filter_flag or (
-        num_cells > MAX_CELLS_PER_NOTEBOOK
+
+    if (
+        pyflake_results
+        or num_cells > MAX_CELLS_PER_NOTEBOOK
         or max_lines_in_cell > MAX_LINES_PER_CELL
         or num_functions > MAX_FUNCTIONS_PER_NOTEBOOK
     ):
-        print(f"\tNumber of cells: {num_cells}")
-        print(f"\tLines of code: {num_lines}")
-        print(f"\tNumber of function definitions: {num_functions}")
-        print(f"\tMax lines in a cell: {max_lines_in_cell}")
+        print(f"Analyzing {file_path}:")
+        if pyflake_results:
+            print_results("PyFlakes", pyflake_results, verbose=verbose)
+
+        if num_cells > MAX_CELLS_PER_NOTEBOOK:
+            print(f"\tMax number of cells exceeded: {num_cells}")
+        if max_lines_in_cell > MAX_LINES_PER_CELL:
+            print(
+                f"\tMax number of lines per cell exceeded: {max_lines_in_cell}"
+            )
+        if num_functions > MAX_FUNCTIONS_PER_NOTEBOOK:
+            print(f"\tFunction definitions detected: {num_functions}")
+
+        print("-" * 80)
 
 
 def analyze_python_file(file_path, lint_flag, verbose):
     """Analyze a Python file"""
     pyflake_results = pyflakes_python_file(file_path)
-    pylint_warnings = get_pylint_warnings(file_path)
     black_results = black_python_file(file_path)
+    functions_no_docstrings = functions_without_docstrings(file_path)
+    contains_subprocess = code_contains_subprocess(file_path)
+    code_in_functions = is_code_in_functions_or_main(file_path)
+    pylint_warnings = get_pylint_warnings(file_path)
 
-    if lint_flag:
-        print_results("Pylint", pylint_warnings, verbose=verbose)
-
-    print_results("PyFlakes", pyflake_results, verbose=verbose)
-
-    if black_results:
-        print(f"\tPlease run black. {len(black_results)} changes needed.")
-
-    if not is_code_in_functions_or_main(file_path):
-        print("\tCode outside functions or main block detected.")
-
-    if code_contains_subprocess(file_path):
-        print("\tWarning: subprocess usage detected.")
+    if (
+        (lint_flag and pylint_warnings)
+        or pyflake_results
+        or black_results
+        or functions_no_docstrings
+        or contains_subprocess
+        or not code_in_functions
+    ):
+        print(f"Analyzing {file_path}:")
 
-    functions_no_docstrings = functions_without_docstrings(file_path)
-    if functions_no_docstrings:
-        print(
-            "\tFunctions without docstrings detected:", functions_no_docstrings
-        )
+        if pyflake_results:
+            print_results("PyFlakes", pyflake_results, verbose=verbose)
+        if black_results:
+            print(f"\tBlack found {len(black_results)} issues")
+        if functions_no_docstrings:
+            print(
+                "\tFunctions without docstrings detected:",
+                functions_no_docstrings,
+            )
+        if contains_subprocess:
+            print("\tSubprocess usage detected.")
+        if not code_in_functions:
+            print("\tCode outside functions or main block detected.")
+        if lint_flag:
+            print_results("Pylint", pylint_warnings, verbose=verbose)
+        print("-" * 80)
 
 
 def print_results(tool_name, results, verbose=False):
     """Print results from pylint or pyflake"""
     if results:
         if verbose:
-            print(f"{tool_name} found {len(results)} issues:")
+            print(f"\t{tool_name} found {len(results)} issues:")
             for result in results:
-                print(f"  {result}")
+                print(f"\t  {result}")
         else:
-            print(f"{tool_name} found {len(results)} issues:")
+            print(f"\t{tool_name} found {len(results)} issues:")
             for result in results[:5]:
-                print(f"  {result}")
+                print(f"\t  {result}")
             if len(results) > 5:
-                print(f"  ...and {len(results) - 5} more issues.")
+                print(f"\t  ...and {len(results) - 5} more issues.")
 
 
 def evaluate_repo(path_or_url, lint_flag, start_date=None, verbose=False):
     """
     This is the entry point to running the automated code review.
     """
```

### Comparing `dsi_cocoa-0.1.8/src/cocoa/linting.py` & `dsi_cocoa-0.1.9/src/cocoa/linting.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.8/src/cocoa/notebooks.py` & `dsi_cocoa-0.1.9/src/cocoa/notebooks.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.8/src/cocoa/repo.py` & `dsi_cocoa-0.1.9/src/cocoa/repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.8/src/cocoa/spring2024.py` & `dsi_cocoa-0.1.9/src/cocoa/spring2024.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.8/src/dsi_cocoa.egg-info/PKG-INFO` & `dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.1.8
+Version: 0.1.9
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dsi_cocoa-0.1.8/src/dsi_cocoa.egg-info/SOURCES.txt` & `dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

