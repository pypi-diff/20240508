# Comparing `tmp/machine-learning-model-local-0.0.3.tar.gz` & `tmp/machine_learning_model_local-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machine-learning-model-local-0.0.3.tar", last modified: Thu Nov  9 07:52:35 2023, max compression
+gzip compressed data, was "machine_learning_model_local-0.0.4.tar", last modified: Wed May  8 02:47:10 2024, max compression
```

## Comparing `machine-learning-model-local-0.0.3.tar` & `machine_learning_model_local-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 07:52:35.754979 machine-learning-model-local-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2023-11-09 07:52:35.754979 machine-learning-model-local-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-11-09 07:52:04.000000 machine-learning-model-local-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 07:52:35.754979 machine-learning-model-local-0.0.3/machine_learning_model_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 07:52:35.754979 machine-learning-model-local-0.0.3/machine_learning_model_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 07:52:04.000000 machine-learning-model-local-0.0.3/machine_learning_model_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2023-11-09 07:52:04.000000 machine-learning-model-local-0.0.3/machine_learning_model_local/src/machine_learning_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 07:52:35.754979 machine-learning-model-local-0.0.3/machine_learning_model_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2023-11-09 07:52:35.000000 machine-learning-model-local-0.0.3/machine_learning_model_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-11-09 07:52:35.000000 machine-learning-model-local-0.0.3/machine_learning_model_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 07:52:35.000000 machine-learning-model-local-0.0.3/machine_learning_model_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-09 07:52:35.000000 machine-learning-model-local-0.0.3/machine_learning_model_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-11-09 07:52:35.000000 machine-learning-model-local-0.0.3/machine_learning_model_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-11-09 07:52:04.000000 machine-learning-model-local-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-09 07:52:35.754979 machine-learning-model-local-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2023-11-09 07:52:04.000000 machine-learning-model-local-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:47:10.084046 machine_learning_model_local-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-08 02:47:10.084046 machine_learning_model_local-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-08 02:46:48.000000 machine_learning_model_local-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:47:10.084046 machine_learning_model_local-0.0.4/machine_learning_model_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:47:10.084046 machine_learning_model_local-0.0.4/machine_learning_model_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 02:46:48.000000 machine_learning_model_local-0.0.4/machine_learning_model_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-08 02:46:48.000000 machine_learning_model_local-0.0.4/machine_learning_model_local/src/machine_learning_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:47:10.084046 machine_learning_model_local-0.0.4/machine_learning_model_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-08 02:47:10.000000 machine_learning_model_local-0.0.4/machine_learning_model_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 02:47:10.000000 machine_learning_model_local-0.0.4/machine_learning_model_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 02:47:10.000000 machine_learning_model_local-0.0.4/machine_learning_model_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 02:47:10.000000 machine_learning_model_local-0.0.4/machine_learning_model_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-08 02:47:10.000000 machine_learning_model_local-0.0.4/machine_learning_model_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-08 02:46:48.000000 machine_learning_model_local-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 02:47:10.084046 machine_learning_model_local-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 02:46:48.000000 machine_learning_model_local-0.0.4/setup.py
```

### Comparing `machine-learning-model-local-0.0.3/PKG-INFO` & `machine_learning_model_local-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,49 @@
-Metadata-Version: 2.1
-Name: machine-learning-model-local
-Version: 0.0.3
-Summary: PyPI Package for Circles machine-learning-model-local Python
-Home-page: https://github.com/circles
-Author: Circles
-Author-email: info@circlez.ai
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Requires-Dist: logger-local>=0.0.61
-Requires-Dist: database-without-orm-local>=0.0.90
-
 # python-package-template
+
 This repository is designed to help you create local and remote package layers in Python.  
 It focuses on building package layers and does not include GraphQL and REST-API layers.
 
 ## Download Environment
+
 To set up the environment, follow these steps in your terminal:
+
 ```shell
 git clone https://github.com/circles-zone/<your-repo>.git --branch dev  # or other branch
 cd <your-repo>
 git checkout -b BU-<new-branch>  # if a new branch is needed
 python -m venv venv
 pip install -r requirements.txt
 ... <edit your code> ...
 git add .
 git commit -m "Your commit message"
 git push origin BU-<your-branch>
 ```
 
-For more detailed information, refer to the [documentation](https://docs.google.com/document/d/1HKhwlhwLD3S8uJ9LPI7h4Nxu77-DXKZe/edit?usp=sharing&ouid=104468990154530891864&rtpof=true&sd=true).
+For more detailed information, refer to
+the [documentation](https://docs.google.com/document/d/1HKhwlhwLD3S8uJ9LPI7h4Nxu77-DXKZe/edit?usp=sharing&ouid=104468990154530891864&rtpof=true&sd=true).
 
 ## Check List:
 
 ### Directory Structure
 
 Ensure that the root directory has the following structure:
+
 - `.github/`
 - `.vscode/` (optional)
 - `directory_with_same_name_as_the_repo/`
-  - `db/`
-  - `reports/`
-  - `project_name/`
-    - `src/`
-      - `__init__.py`
-      - `example_class.py`
-    - `tests/`
-      - `example_class_test.py`
-    - `__init__.py`
+    - `db/`
+    - `reports/`
+    - `project_name/`
+        - `src/`
+            - `__init__.py`
+            - `example_class.py`
+        - `tests/`
+            - `example_class_test.py`
+        - `__init__.py`
 
 This setup enables easy switching to a mono repo configuration.
 
 ### Database Python Scripts
 
 Place `<table-name>.py` in the `/db` folder if needed.  
 There's no need for a separate file for `_ml` tables.  
@@ -64,32 +55,39 @@
 - Use `/db/<table-name>.py` to create the schema, tables, views (including `_ml_table`).
 - Use `/db/<table-name>_insert.py` to create metadata and test data records.
 
 ### Update `setup.py`
 
 Don't forget to update the `setup.py` file, including the package name and version.  
 Remember to upload the version after every deployment.
+
 ### Working with VS Code
+
 Ensure that you push the `launch.json` file to the repository.  
 This enables running and debugging the code smoothly.
 
 ### Unit Testing
+
 We recommend using `pytest` over the `unittest` package.  
 Create a `pytest.ini` file in the project directory, not the root directory.
 run in termianl: pytest
 
 ## Workflow Completion
-When you've addressed all the TODOs in the repository, using infrastructure classes like Logger, Database, Url, Importer, and others, make sure your Feature Branch GitHub Actions Workflow is green without warnings.  
-All tests should run in GitHub Actions, your code should be well-documented, the `README.md` file should be clear and self-explanatory, test coverage should be above 90%, and all lines of code should be covered by unit tests.
+
+When you've addressed all the TODOs in the repository, using infrastructure classes like Logger, Database, Url,
+Importer, and others, make sure your Feature Branch GitHub Actions Workflow is green without warnings.  
+All tests should run in GitHub Actions, your code should be well-documented, the `README.md` file should be clear and
+self-explanatory, test coverage should be above 90%, and all lines of code should be covered by unit tests.
 
 Once these conditions are met, you can filter and analyze your records in Logz.io.  
 Pull the `dev` branch to your Feature Branch and then create a Pull Request to `dev`.
 
 Good luck :)
 
 ## check your code visibility lint with flake (Mandatory before pusj):
+
 run those command
 python -m pip install flake8 pytest
 flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
 flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
 
 note: you should use autopep8 extension in your code!
```

### Comparing `machine-learning-model-local-0.0.3/pyproject.toml` & `machine_learning_model_local-0.0.4/pyproject.toml`

 * *Files identical despite different names*

