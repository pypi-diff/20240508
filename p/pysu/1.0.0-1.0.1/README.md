# Comparing `tmp/pysu-1.0.0.tar.gz` & `tmp/pysu-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysu-1.0.0.tar", last modified: Thu Apr 11 23:38:31 2024, max compression
+gzip compressed data, was "pysu-1.0.1.tar", last modified: Wed May  8 11:05:42 2024, max compression
```

## Comparing `pysu-1.0.0.tar` & `pysu-1.0.1.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.224209 pysu-1.0.0/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      605 2024-04-11 23:38:17.000000 pysu-1.0.0/.bumpversion.cfg
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1541 2024-04-11 23:38:17.000000 pysu-1.0.0/.cookiecutterrc
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      172 2024-04-11 13:41:26.000000 pysu-1.0.0/.coveragerc
--rw-r--r--   0 ionel     (1000) ionel     (1000)       27 2024-04-11 13:05:36.000000 pysu-1.0.0/.dockerignore
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2024-04-11 13:41:26.000000 pysu-1.0.0/.editorconfig
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.219209 pysu-1.0.0/.github/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.221209 pysu-1.0.0/.github/workflows/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3973 2024-04-11 13:41:26.000000 pysu-1.0.0/.github/workflows/github-actions.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      702 2024-04-11 13:47:47.000000 pysu-1.0.0/.pre-commit-config.yaml
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       70 2024-04-11 13:41:26.000000 pysu-1.0.0/AUTHORS.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)      461 2024-04-11 23:32:09.000000 pysu-1.0.0/CHANGELOG.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2313 2024-04-11 13:41:26.000000 pysu-1.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1337 2024-04-11 13:41:26.000000 pysu-1.0.0/LICENSE
--rw-r--r--   0 ionel     (1000) ionel     (1000)      424 2024-04-11 16:29:05.000000 pysu-1.0.0/MANIFEST.in
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2726 2024-04-11 23:38:31.224209 pysu-1.0.0/PKG-INFO
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2132 2024-04-11 23:38:17.000000 pysu-1.0.0/README.rst
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.222209 pysu-1.0.0/ci/
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2867 2024-04-11 13:41:26.000000 pysu-1.0.0/ci/bootstrap.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.222209 pysu-1.0.0/ci/py27/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3160 2024-04-11 13:05:36.000000 pysu-1.0.0/ci/py27/Dockerfile
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.222209 pysu-1.0.0/ci/py34/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3160 2024-04-11 13:05:36.000000 pysu-1.0.0/ci/py34/Dockerfile
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.222209 pysu-1.0.0/ci/py35/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3160 2024-04-11 13:05:36.000000 pysu-1.0.0/ci/py35/Dockerfile
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       72 2024-04-11 13:41:26.000000 pysu-1.0.0/ci/requirements.txt
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.222209 pysu-1.0.0/ci/templates/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.220209 pysu-1.0.0/ci/templates/.github/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.222209 pysu-1.0.0/ci/templates/.github/workflows/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1812 2024-04-11 13:41:26.000000 pysu-1.0.0/ci/templates/.github/workflows/github-actions.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3170 2024-04-11 13:05:36.000000 pysu-1.0.0/ci/templates/Dockerfile
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1352 2024-04-11 13:41:26.000000 pysu-1.0.0/pyproject.toml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      901 2024-04-11 13:41:26.000000 pysu-1.0.0/pytest.ini
--rw-r--r--   0 ionel     (1000) ionel     (1000)       38 2024-04-11 23:38:31.224209 pysu-1.0.0/setup.cfg
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2819 2024-04-11 23:38:17.000000 pysu-1.0.0/setup.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.220209 pysu-1.0.0/src/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.222209 pysu-1.0.0/src/pysu/
--rw-r--r--   0 ionel     (1000) ionel     (1000)       22 2024-04-11 23:38:17.000000 pysu-1.0.0/src/pysu/__init__.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      378 2024-04-11 13:47:13.000000 pysu-1.0.0/src/pysu/__main__.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3055 2024-04-11 16:09:52.000000 pysu-1.0.0/src/pysu/cli.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.223209 pysu-1.0.0/src/pysu.egg-info/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2726 2024-04-11 23:38:31.000000 pysu-1.0.0/src/pysu.egg-info/PKG-INFO
--rw-r--r--   0 ionel     (1000) ionel     (1000)      767 2024-04-11 23:38:31.000000 pysu-1.0.0/src/pysu.egg-info/SOURCES.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-04-11 23:38:31.000000 pysu-1.0.0/src/pysu.egg-info/dependency_links.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)       39 2024-04-11 23:38:31.000000 pysu-1.0.0/src/pysu.egg-info/entry_points.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-04-11 23:38:30.000000 pysu-1.0.0/src/pysu.egg-info/not-zip-safe
--rw-r--r--   0 ionel     (1000) ionel     (1000)        5 2024-04-11 23:38:31.000000 pysu-1.0.0/src/pysu.egg-info/top_level.txt
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.223209 pysu-1.0.0/tests/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3165 2024-04-11 16:08:38.000000 pysu-1.0.0/tests/test-alpine.Dockerfile
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3281 2024-04-11 16:08:45.000000 pysu-1.0.0/tests/test-debian.Dockerfile
--rw-r--r--   0 ionel     (1000) ionel     (1000)      404 2024-04-11 23:32:03.000000 pysu-1.0.0/tests/test_docker.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      347 2024-04-11 15:01:08.000000 pysu-1.0.0/tests/test_pysu.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1487 2024-04-11 13:41:26.000000 pysu-1.0.0/tox.ini
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-08 11:05:42.499924 pysu-1.0.1/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      605 2024-05-08 11:05:33.000000 pysu-1.0.1/.bumpversion.cfg
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1541 2024-05-08 11:05:33.000000 pysu-1.0.1/.cookiecutterrc
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      172 2024-05-08 10:37:17.000000 pysu-1.0.1/.coveragerc
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       27 2024-04-11 13:05:36.000000 pysu-1.0.1/.dockerignore
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2024-05-08 10:37:17.000000 pysu-1.0.1/.editorconfig
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-08 11:05:42.494924 pysu-1.0.1/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-08 11:05:42.496924 pysu-1.0.1/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3989 2024-05-08 10:46:56.000000 pysu-1.0.1/.github/workflows/github-actions.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      678 2024-05-08 10:37:17.000000 pysu-1.0.1/.gitignore
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      702 2024-05-08 10:46:45.000000 pysu-1.0.1/.pre-commit-config.yaml
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       70 2024-05-08 10:37:17.000000 pysu-1.0.1/AUTHORS.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      524 2024-05-08 10:46:45.000000 pysu-1.0.1/CHANGELOG.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2313 2024-05-08 10:37:17.000000 pysu-1.0.1/CONTRIBUTING.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)     1337 2024-05-08 10:37:17.000000 pysu-1.0.1/LICENSE
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      424 2024-05-08 10:46:45.000000 pysu-1.0.1/MANIFEST.in
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2789 2024-05-08 11:05:42.499924 pysu-1.0.1/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2132 2024-05-08 11:05:33.000000 pysu-1.0.1/README.rst
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-08 11:05:42.497924 pysu-1.0.1/ci/
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2867 2024-05-08 10:37:17.000000 pysu-1.0.1/ci/bootstrap.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-08 11:05:42.497924 pysu-1.0.1/ci/py27/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3160 2024-04-11 13:05:36.000000 pysu-1.0.1/ci/py27/Dockerfile
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-08 11:05:42.497924 pysu-1.0.1/ci/py34/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3160 2024-04-11 13:05:36.000000 pysu-1.0.1/ci/py34/Dockerfile
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-08 11:05:42.497924 pysu-1.0.1/ci/py35/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3160 2024-04-11 13:05:36.000000 pysu-1.0.1/ci/py35/Dockerfile
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       72 2024-05-08 10:37:17.000000 pysu-1.0.1/ci/requirements.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-08 11:05:42.497924 pysu-1.0.1/ci/templates/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-08 11:05:42.494924 pysu-1.0.1/ci/templates/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-08 11:05:42.497924 pysu-1.0.1/ci/templates/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1814 2024-05-08 10:37:17.000000 pysu-1.0.1/ci/templates/.github/workflows/github-actions.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3170 2024-04-11 13:05:36.000000 pysu-1.0.1/ci/templates/Dockerfile
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1352 2024-05-08 10:37:17.000000 pysu-1.0.1/pyproject.toml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      901 2024-05-08 10:37:17.000000 pysu-1.0.1/pytest.ini
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       38 2024-05-08 11:05:42.499924 pysu-1.0.1/setup.cfg
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2819 2024-05-08 11:05:33.000000 pysu-1.0.1/setup.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-08 11:05:42.494924 pysu-1.0.1/src/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-08 11:05:42.497924 pysu-1.0.1/src/pysu/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       22 2024-05-08 11:05:33.000000 pysu-1.0.1/src/pysu/__init__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      378 2024-05-08 10:46:45.000000 pysu-1.0.1/src/pysu/__main__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3025 2024-05-08 10:46:45.000000 pysu-1.0.1/src/pysu/cli.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-08 11:05:42.498924 pysu-1.0.1/src/pysu.egg-info/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2789 2024-05-08 11:05:42.000000 pysu-1.0.1/src/pysu.egg-info/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      778 2024-05-08 11:05:42.000000 pysu-1.0.1/src/pysu.egg-info/SOURCES.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-05-08 11:05:42.000000 pysu-1.0.1/src/pysu.egg-info/dependency_links.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       39 2024-05-08 11:05:42.000000 pysu-1.0.1/src/pysu.egg-info/entry_points.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-05-08 11:05:41.000000 pysu-1.0.1/src/pysu.egg-info/not-zip-safe
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        5 2024-05-08 11:05:42.000000 pysu-1.0.1/src/pysu.egg-info/top_level.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-08 11:05:42.498924 pysu-1.0.1/tests/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3165 2024-04-11 16:08:38.000000 pysu-1.0.1/tests/test-alpine.Dockerfile
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3281 2024-04-11 16:08:45.000000 pysu-1.0.1/tests/test-debian.Dockerfile
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      404 2024-04-11 23:32:03.000000 pysu-1.0.1/tests/test_docker.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      347 2024-04-11 15:01:08.000000 pysu-1.0.1/tests/test_pysu.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1487 2024-05-08 10:37:17.000000 pysu-1.0.1/tox.ini
```

### Comparing `pysu-1.0.0/.bumpversion.cfg` & `pysu-1.0.1/.bumpversion.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.0
+current_version = 1.0.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `pysu-1.0.0/.cookiecutterrc` & `pysu-1.0.1/.cookiecutterrc`

 * *Files 0% similar despite different names*

```diff
@@ -36,12 +36,12 @@
     setup_py_uses_setuptools_scm: 'no'
     sphinx_docs: 'no'
     sphinx_docs_hosting: https://python-su.readthedocs.io/
     sphinx_doctest: 'no'
     sphinx_theme: sphinx-rtd-theme
     test_matrix_separate_coverage: 'no'
     tests_inside_package: 'no'
-    version: 1.0.0
+    version: 1.0.1
     version_manager: bump2version
     website: https://blog.ionelmc.ro
     year_from: '2016'
     year_to: '2024'
```

### Comparing `pysu-1.0.0/.github/workflows/github-actions.yml` & `pysu-1.0.1/.github/workflows/github-actions.yml`

 * *Files 1% similar despite different names*

```diff
@@ -19,99 +19,99 @@
             toxpython: 'python3.8'
             python_arch: 'x64'
             tox_env: 'py38'
             os: 'ubuntu-latest'
           - name: 'py38 (macos)'
             python: '3.8'
             toxpython: 'python3.8'
-            python_arch: 'x64'
+            python_arch: 'arm64'
             tox_env: 'py38'
             os: 'macos-latest'
           - name: 'py39 (ubuntu)'
             python: '3.9'
             toxpython: 'python3.9'
             python_arch: 'x64'
             tox_env: 'py39'
             os: 'ubuntu-latest'
           - name: 'py39 (macos)'
             python: '3.9'
             toxpython: 'python3.9'
-            python_arch: 'x64'
+            python_arch: 'arm64'
             tox_env: 'py39'
             os: 'macos-latest'
           - name: 'py310 (ubuntu)'
             python: '3.10'
             toxpython: 'python3.10'
             python_arch: 'x64'
             tox_env: 'py310'
             os: 'ubuntu-latest'
           - name: 'py310 (macos)'
             python: '3.10'
             toxpython: 'python3.10'
-            python_arch: 'x64'
+            python_arch: 'arm64'
             tox_env: 'py310'
             os: 'macos-latest'
           - name: 'py311 (ubuntu)'
             python: '3.11'
             toxpython: 'python3.11'
             python_arch: 'x64'
             tox_env: 'py311'
             os: 'ubuntu-latest'
           - name: 'py311 (macos)'
             python: '3.11'
             toxpython: 'python3.11'
-            python_arch: 'x64'
+            python_arch: 'arm64'
             tox_env: 'py311'
             os: 'macos-latest'
           - name: 'py312 (ubuntu)'
             python: '3.12'
             toxpython: 'python3.12'
             python_arch: 'x64'
             tox_env: 'py312'
             os: 'ubuntu-latest'
           - name: 'py312 (macos)'
             python: '3.12'
             toxpython: 'python3.12'
-            python_arch: 'x64'
+            python_arch: 'arm64'
             tox_env: 'py312'
             os: 'macos-latest'
           - name: 'pypy38 (ubuntu)'
             python: 'pypy-3.8'
             toxpython: 'pypy3.8'
             python_arch: 'x64'
             tox_env: 'pypy38'
             os: 'ubuntu-latest'
           - name: 'pypy38 (macos)'
             python: 'pypy-3.8'
             toxpython: 'pypy3.8'
-            python_arch: 'x64'
+            python_arch: 'arm64'
             tox_env: 'pypy38'
             os: 'macos-latest'
           - name: 'pypy39 (ubuntu)'
             python: 'pypy-3.9'
             toxpython: 'pypy3.9'
             python_arch: 'x64'
             tox_env: 'pypy39'
             os: 'ubuntu-latest'
           - name: 'pypy39 (macos)'
             python: 'pypy-3.9'
             toxpython: 'pypy3.9'
-            python_arch: 'x64'
+            python_arch: 'arm64'
             tox_env: 'pypy39'
             os: 'macos-latest'
           - name: 'pypy310 (ubuntu)'
             python: 'pypy-3.10'
             toxpython: 'pypy3.10'
             python_arch: 'x64'
             tox_env: 'pypy310'
             os: 'ubuntu-latest'
           - name: 'pypy310 (macos)'
             python: 'pypy-3.10'
             toxpython: 'pypy3.10'
-            python_arch: 'x64'
+            python_arch: 'arm64'
             tox_env: 'pypy310'
             os: 'macos-latest'
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - uses: actions/setup-python@v5
```

### Comparing `pysu-1.0.0/.pre-commit-config.yaml` & `pysu-1.0.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 #   pre-commit install --install-hooks
 # To update the versions:
 #   pre-commit autoupdate
 exclude: '^(\.tox|ci/templates|\.bumpversion\.cfg)(/|$)'
 # Note the order is intentional to avoid multiple passes of the hooks
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.5
+    rev: v0.4.3
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix, --show-fixes, --unsafe-fixes]
   - repo: https://github.com/psf/black
-    rev: 24.3.0
+    rev: 24.4.2
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.6.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
```

### Comparing `pysu-1.0.0/CONTRIBUTING.rst` & `pysu-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pysu-1.0.0/LICENSE` & `pysu-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysu-1.0.0/PKG-INFO` & `pysu-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysu
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple Python-based setuid+setgid+setgroups+exec. A port of https://github.com/tianon/gosu
 Home-page: https://github.com/ionelmc/python-su
 Author: Ionel Cristian Mărieș
 Author-email: contact@ionelmc.ro
 License: BSD-2-Clause
 Project-URL: Changelog, https://github.com/ionelmc/python-su/blob/master/CHANGELOG.rst
 Project-URL: Issue Tracker, https://github.com/ionelmc/python-su/issues
@@ -89,14 +89,19 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
+1.0.1 (2024-05-08)
+------------------
+
+* Removed debug print.
+
 1.0.0 (2024-04-12)
 ------------------
 
 * Dropped support for old Pythons. Minium supported version is 3.8.
 * Improved error handling and reporting.
 * Increased compatibility with `gosu <https://github.com/tianon/gosu>`_.
```

### Comparing `pysu-1.0.0/README.rst` & `pysu-1.0.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/pysu
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pysu.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/pysu
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/ionelmc/python-su/v1.0.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/ionelmc/python-su/v1.0.1.svg
     :alt: Commits since latest release
-    :target: https://github.com/ionelmc/python-su/compare/v1.0.0...master
+    :target: https://github.com/ionelmc/python-su/compare/v1.0.1...master
 
 
 
 .. end-badges
 
 Simple Python-based setuid+setgid+setgroups+exec. A port of https://github.com/tianon/gosu
```

### Comparing `pysu-1.0.0/ci/bootstrap.py` & `pysu-1.0.1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pysu-1.0.0/ci/py27/Dockerfile` & `pysu-1.0.1/ci/py27/Dockerfile`

 * *Files identical despite different names*

### Comparing `pysu-1.0.0/ci/py34/Dockerfile` & `pysu-1.0.1/ci/py34/Dockerfile`

 * *Files identical despite different names*

### Comparing `pysu-1.0.0/ci/py35/Dockerfile` & `pysu-1.0.1/ci/py35/Dockerfile`

 * *Files identical despite different names*

### Comparing `pysu-1.0.0/ci/templates/.github/workflows/github-actions.yml` & `pysu-1.0.1/ci/templates/.github/workflows/github-actions.yml`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 {% else %}
 {% set python %}{{ prefix[2] }}.{{ prefix[3:] }}{% endset %}
 {% set cpython %}cp{{ prefix[2:] }}{% endset %}
 {% set toxpython %}python{{ prefix[2] }}.{{ prefix[3:] }}{% endset %}
 {% endif %}
 {% for os, python_arch in [
     ['ubuntu', 'x64'],
-    ['macos', 'x64'],
+    ['macos', 'arm64'],
 ] %}
           - name: '{{ env }} ({{ os }})'
             python: '{{ python }}'
             toxpython: '{{ toxpython }}'
             python_arch: '{{ python_arch }}'
             tox_env: '{{ env }}'
             os: '{{ os }}-latest'
```

### Comparing `pysu-1.0.0/ci/templates/Dockerfile` & `pysu-1.0.1/ci/templates/Dockerfile`

 * *Files identical despite different names*

### Comparing `pysu-1.0.0/pyproject.toml` & `pysu-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysu-1.0.0/pytest.ini` & `pysu-1.0.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `pysu-1.0.0/setup.py` & `pysu-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="pysu",
-    version="1.0.0",
+    version="1.0.1",
     license="BSD-2-Clause",
     description="Simple Python-based setuid+setgid+setgroups+exec. A port of https://github.com/tianon/gosu",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
     author="Ionel Cristian Mărieș",
```

### Comparing `pysu-1.0.0/src/pysu/cli.py` & `pysu-1.0.1/src/pysu/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             uid = pw.pw_uid
     else:
         uid = os.getuid()
         try:
             pw = pwd.getpwuid(uid)
         except KeyError:
             pw = None
-    print(pw, file=sys.stderr)
+
     if pw:
         home = pw.pw_dir
         name = pw.pw_name
     else:
         home = "/"
         name = user
```

### Comparing `pysu-1.0.0/src/pysu.egg-info/PKG-INFO` & `pysu-1.0.1/src/pysu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysu
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple Python-based setuid+setgid+setgroups+exec. A port of https://github.com/tianon/gosu
 Home-page: https://github.com/ionelmc/python-su
 Author: Ionel Cristian Mărieș
 Author-email: contact@ionelmc.ro
 License: BSD-2-Clause
 Project-URL: Changelog, https://github.com/ionelmc/python-su/blob/master/CHANGELOG.rst
 Project-URL: Issue Tracker, https://github.com/ionelmc/python-su/issues
@@ -89,14 +89,19 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
+1.0.1 (2024-05-08)
+------------------
+
+* Removed debug print.
+
 1.0.0 (2024-04-12)
 ------------------
 
 * Dropped support for old Pythons. Minium supported version is 3.8.
 * Improved error handling and reporting.
 * Increased compatibility with `gosu <https://github.com/tianon/gosu>`_.
```

### Comparing `pysu-1.0.0/src/pysu.egg-info/SOURCES.txt` & `pysu-1.0.1/src/pysu.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .bumpversion.cfg
 .cookiecutterrc
 .coveragerc
 .dockerignore
 .editorconfig
+.gitignore
 .pre-commit-config.yaml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
```

### Comparing `pysu-1.0.0/tests/test-alpine.Dockerfile` & `pysu-1.0.1/tests/test-alpine.Dockerfile`

 * *Files identical despite different names*

### Comparing `pysu-1.0.0/tests/test-debian.Dockerfile` & `pysu-1.0.1/tests/test-debian.Dockerfile`

 * *Files identical despite different names*

### Comparing `pysu-1.0.0/tox.ini` & `pysu-1.0.1/tox.ini`

 * *Files identical despite different names*

