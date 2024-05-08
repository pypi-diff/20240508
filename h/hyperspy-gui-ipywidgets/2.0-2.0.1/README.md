# Comparing `tmp/hyperspy_gui_ipywidgets-2.0.tar.gz` & `tmp/hyperspy_gui_ipywidgets-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperspy_gui_ipywidgets-2.0.tar", last modified: Thu Nov 16 17:58:40 2023, max compression
+gzip compressed data, was "hyperspy_gui_ipywidgets-2.0.1.tar", last modified: Wed May  8 09:43:27 2024, max compression
```

## Comparing `hyperspy_gui_ipywidgets-2.0.tar` & `hyperspy_gui_ipywidgets-2.0.1.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 17:58:40.841831 hyperspy_gui_ipywidgets-2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 17:58:40.833831 hyperspy_gui_ipywidgets-2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 17:58:40.833831 hyperspy_gui_ipywidgets-2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/.github/workflows/package_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44172 2023-11-16 17:58:40.837831 hyperspy_gui_ipywidgets-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 17:58:40.833831 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7260 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/axes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      165 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/custom_widgets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3905 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/hyperspy_extension.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/microscope_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/roi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 17:58:40.837831 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/test_microscope_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/test_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/test_roi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39885 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 17:58:40.837831 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44172 2023-11-16 17:58:40.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2023-11-16 17:58:40.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 17:58:40.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-16 17:58:40.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-11-16 17:58:40.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-16 17:58:40.000000 hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 17:58:40.837831 hyperspy_gui_ipywidgets-2.0/images/
--rw-r--r--   0 runner    (1001) docker     (127)    29384 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/images/preferences_gui.png
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2023-11-16 17:58:27.000000 hyperspy_gui_ipywidgets-2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 17:58:40.841831 hyperspy_gui_ipywidgets-2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:43:27.550968 hyperspy_gui_ipywidgets-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:43:27.546968 hyperspy_gui_ipywidgets-2.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:43:27.546968 hyperspy_gui_ipywidgets-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/.github/workflows/package_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44196 2024-05-08 09:43:27.550968 hyperspy_gui_ipywidgets-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:43:27.546968 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/axes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      303 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/custom_widgets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3905 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/hyperspy_extension.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/microscope_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/roi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:43:27.550968 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/test_microscope_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/test_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/test_roi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10513 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39594 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:43:27.550968 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44196 2024-05-08 09:43:27.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-08 09:43:27.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:43:27.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 09:43:27.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-08 09:43:27.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 09:43:27.000000 hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:43:27.550968 hyperspy_gui_ipywidgets-2.0.1/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/images/preferences_gui.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/prepare_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-08 09:43:17.000000 hyperspy_gui_ipywidgets-2.0.1/releasing_guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:43:27.550968 hyperspy_gui_ipywidgets-2.0.1/setup.cfg
```

### Comparing `hyperspy_gui_ipywidgets-2.0/.github/dependabot.yml` & `hyperspy_gui_ipywidgets-2.0.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/.github/workflows/release.yml` & `hyperspy_gui_ipywidgets-2.0.1/.github/workflows/release.yml`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     runs-on: ubuntu-latest
     name: Upload to pypi
     permissions:
       # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
     steps:
     - name: Download dist
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
 
     - name: Display downloaded files
       run: |
         ls -shR
       working-directory: dist
 
     - uses: pypa/gh-action-pypi-publish@release/v1
@@ -48,8 +48,8 @@
     name: Create GitHub Release
     runs-on: ubuntu-latest
     steps:
       - name: Checkout code
         uses: actions/checkout@v4
       - name: Create Release
         if: ${{ startsWith(github.ref, 'refs/tags/') && github.repository_owner == 'hyperspy' }}
-        uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
+        uses: softprops/action-gh-release@9d7c94cfd0a1f3ed45544c887983e9fa900f0564
```

### Comparing `hyperspy_gui_ipywidgets-2.0/.github/workflows/tests.yml` & `hyperspy_gui_ipywidgets-2.0.1/.github/workflows/tests.yml`

 * *Files 7% similar despite different names*

```diff
@@ -25,25 +25,30 @@
           - PYTHON_VERSION: '3.12'
             LABEL: -minimum
           - PYTHON_VERSION: '3.12'
             LABEL: -RnM
 
     steps:
       - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
+
+      - name: get repository name
+        shell: bash
+        run: echo "REPOSITORY_NAME=${GITHUB_REPOSITORY#*/}" >> $GITHUB_ENV
 
       - name: Fetch tags upstream
         if: ${{ github.repository_owner != 'hyperspy' }}
         # Needs to fetch the tags from upstream to get the
         # correct version with setuptools_scm
         run: |
-          git remote add upstream https://github.com/hyperspy/hyperspy_gui_ipywidgets.git
-          git fetch --prune --unshallow
+          git remote add upstream https://github.com/hyperspy/${{ env.REPOSITORY_NAME }}.git
           git fetch upstream --tags
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         name: Install Python
         with:
           python-version: ${{ matrix.PYTHON_VERSION }}
 
       - name: Display version
         run: |
           python --version
@@ -70,8 +75,10 @@
 
       - name: Run test suite
         run: |
           pytest ${{ env.PYTEST_ARGS }} ${{ env.PYTEST_ARGS_COVERAGE }}
 
       - name: Upload coverage to Codecov
         if: ${{ always() }} && ${{ env.PYTEST_ARGS_COVERAGE }} 
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `hyperspy_gui_ipywidgets-2.0/.gitignore` & `hyperspy_gui_ipywidgets-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/CHANGES.md` & `hyperspy_gui_ipywidgets-2.0.1/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 ..
   Add a single entry in the corresponding section below.
   See https://keepachangelog.com for details
 
+## v2.0.1 (2024-08-05)
+* Add releasing guide and release script ([#59](https://github.com/hyperspy/hyperspy_gui_traitsui/pull/59)).
+* Add `ipympl` dependency as convenience ([#58])(https://github.com/hyperspy/hyperspy_gui_ipywidgets/pull/58).
+* Fix regression with editable installation ([#55](https://github.com/hyperspy/hyperspy_gui_ipywidgets/pull/55)).
+
+
 ## v2.0 (2023-11-15)
 * Consolidate package metadata in `pyproject.toml` ([#49](https://github.com/hyperspy/hyperspy_gui_ipywidgets/pull/49)).
 * Support HyperSpy 2.0 and set HyperSpy requirement to >=2.0 ([#48](https://github.com/hyperspy/hyperspy_gui_ipywidgets/pull/48)).
 
 ## v1.5.0 (2022-04-26)
 
 * Improve rendering changelog on github and fix hyperlinks in `README.md` ([#41](https://github.com/hyperspy/hyperspy_gui_ipywidgets/pull/41)).
```

### Comparing `hyperspy_gui_ipywidgets-2.0/LICENSE` & `hyperspy_gui_ipywidgets-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/PKG-INFO` & `hyperspy_gui_ipywidgets-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperspy_gui_ipywidgets
-Version: 2.0
+Version: 2.0.1
 Summary: ipywidgets GUI elements for the HyperSpy framework.
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -700,14 +700,15 @@
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hyperspy>=2.0rc0
 Requires-Dist: ipywidgets>=7.0
 Requires-Dist: link_traits
+Requires-Dist: ipympl
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-rerunfailures; extra == "tests"
 Requires-Dist: setuptools-scm; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
```

### Comparing `hyperspy_gui_ipywidgets-2.0/README.md` & `hyperspy_gui_ipywidgets-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/__init__.py` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,27 +14,41 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with  HyperSpy.  If not, see <http://www.gnu.org/licenses/>.
 
 
 import importlib
+from importlib.metadata import version
 from pathlib import Path
 
 
-if Path(__file__).parent.parent.name == "site-packages":  # pragma: no cover
-    # Tested in the "Package & Test" workflow on GitHub CI
-    from importlib.metadata import version
-
-    __version__ = version("hyperspy_gui_ipywidgets")
-else:
-    # Editable install
-    from setuptools_scm import get_version
+__version__ = version("rosettasciio")
 
-    __version__ = get_version(Path(__file__).parent.parent)
+# For development version, `setuptools_scm` will be used at build time
+# to get the dev version, in case of missing vcs information (git archive,
+# shallow repository), the fallback version defined in pyproject.toml will
+# be used
+
+# if we have a editable install from a git repository try to use
+# `setuptools_scm` to find a more accurate version:
+# `importlib.metadata` will provide the version at installation
+# time and for editable version this may be different
+
+# we only do that if we have enough git history, e.g. not shallow checkout
+_root = Path(__file__).resolve().parents[1]
+if (_root / ".git").exists() and not (_root / ".git/shallow").exists():
+    try:
+        # setuptools_scm may not be installed
+        from setuptools_scm import get_version
+
+        __version__ = get_version(_root)
+    except ImportError:  # pragma: no cover
+        # setuptools_scm not install, we keep the existing __version__
+        pass
 
 
 __all__ = [
     'axes',
     'microscope_parameters',
     'model',
     'preferences',
@@ -45,15 +59,15 @@
 
 
 def __dir__():
     return sorted(__all__)
 
 
 def __getattr__(name):
+    # lazy loading of module: this is only call when the attribute "name" is not found
+    # in the module
+    # See https://peps.python.org/pep-0562/
     if name in __all__:
-        if name == "__version__":
-            return __version__
-        else:
-            return importlib.import_module(
-                "." + name, 'hyperspy_gui_ipywidgets'
-                )
+        return importlib.import_module(
+            "." + name, 'hyperspy_gui_ipywidgets'
+            )
     raise AttributeError(f"module {__name__!r} has no attribute {name!r}")
```

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/axes.py` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/axes.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/hyperspy_extension.yaml` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/hyperspy_extension.yaml`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/microscope_parameters.py` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/microscope_parameters.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/model.py` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/model.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/preferences.py` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/preferences.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/roi.py` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/roi.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/test_axes.py` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/test_import.py` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/test_microscope_parameters.py` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/test_microscope_parameters.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/test_model.py` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/test_preferences.py` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/test_preferences.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 
-from numpy.random import random, uniform
 import ipywidgets
+from numpy.random import random, uniform
+import pytest
 
 import hyperspy.api as hs
 from hyperspy_gui_ipywidgets.tests.utils import KWARGS
 
 
-def test_preferences():
-    wd = hs.preferences.gui(**KWARGS)["ipywidgets"]["wdict"]
+module_list = [hs]
+try:
+    import exspy
+    module_list.append(exspy)
+except Exception:
+    # exspy is not installed
+    pass
+
+
+@pytest.mark.parametrize("module", module_list)
+def test_preferences(module):
+    wd = module.preferences.gui(**KWARGS)["ipywidgets"]["wdict"]
     for tabkey, tabvalue in wd.items():
         if tabkey.startswith("tab_"):
             for key, value in tabvalue.items():
                 assert getattr(
-                    getattr(hs.preferences, tabkey[4:]), key) == value.value
+                    getattr(module.preferences, tabkey[4:]), key) == value.value
                 value_bk = value.value
                 if isinstance(value, ipywidgets.Checkbox):
                     value.value = not value
                 elif isinstance(value, ipywidgets.FloatText):
                     value.value = random()
                 elif isinstance(value, ipywidgets.Text):
                     value.value = "qwerty"
                 elif isinstance(value, ipywidgets.FloatSlider):
                     value.value = uniform(low=value.min, high=value.max)
                 elif isinstance(value, ipywidgets.Dropdown):
                     options = set(value.options) - set(value.value)
                     value.value = options.pop()
                 assert getattr(
-                    getattr(hs.preferences, tabkey[4:]), key) == value.value
+                    getattr(module.preferences, tabkey[4:]), key) == value.value
                 value.value = value_bk
```

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/test_roi.py` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/test_roi.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tests/test_tools.py` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tests/test_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,58 +119,14 @@
         wd["zero_fill"] = True
         wd["left"].value = 15.
         wd["right"].value = 50.
         wd["apply_button"]._click_handlers(wd["apply_button"])    # Trigger it
         np.testing.assert_allclose(s.data[2:], s2.data[2:], atol=1E-5)
         np.testing.assert_allclose(np.zeros(2), s2.data[:2])
 
-    # Test will need to be update to be more robust
-    # for now, mark it as flaky
-    @pytest.mark.flaky(reruns=3)
-    def test_spikes_removal_tool(self):
-        s = hs.signals.Signal1D(np.ones((2, 3, 30)))
-        # Add three spikes
-        s.data[1, 0, 1] += 2
-        s.data[0, 2, 29] += 1
-        s.data[1, 2, 14] += 5
-        wd = s.spikes_removal_tool(**KWARGS)["ipywidgets"]["wdict"]
-
-        def next():
-            wd["next_button"]._click_handlers(wd["next_button"])
-
-        def previous():
-            wd["previous_button"]._click_handlers(wd["previous_button"])
-
-        def remove():
-            wd["remove_button"]._click_handlers(wd["remove_button"])
-        wd["threshold"].value = 1.5
-        next()
-        assert s.axes_manager.indices == (0, 1)
-        wd["threshold"].value = 0.5
-        assert s.axes_manager.indices == (0, 0)
-        next()
-        assert s.axes_manager.indices == (2, 0)
-        next()
-        assert s.axes_manager.indices == (0, 1)
-        previous()
-        assert s.axes_manager.indices == (2, 0)
-        wd["add_noise"].value = False
-        remove()
-        assert s.data[0, 2, 29] == 1
-        assert s.axes_manager.indices == (0, 1)
-        remove()
-        assert s.data[1, 0, 1] == 1
-        assert s.axes_manager.indices == (2, 1)
-        np.random.seed(1)
-        wd["add_noise"].value = True
-        wd["spline_order"].value = 1
-        remove()
-        assert s.data[1, 2, 14] <= 2
-        assert s.axes_manager.indices == (0, 0)
-
     def test_constrast_editor(self):
         # To get this test to work, matplotlib backend needs to set to 'Agg'
         np.random.seed(1)
         im = hs.signals.Signal2D(np.random.random((32, 32)))
         im.plot()
         ceditor = ImageContrastEditor(im._plot.signal_plot)
         ceditor.ax.figure.canvas.draw_idle()
@@ -268,7 +224,55 @@
     wd["new_length"].value = 10
     wd["units"].value = "mm"
     wd["apply_button"]._click_handlers(wd["apply_button"])
     assert s.axes_manager[0].scale == 0.5
     assert s.axes_manager[1].scale == 0.5
     assert s.axes_manager[0].units == "mm"
     assert s.axes_manager[1].units == "mm"
+
+
+def test_spikes_removal_tool():
+    s = hs.signals.Signal1D(np.ones((2, 3, 30)))
+    s.add_gaussian_noise(std=1, random_state=0)
+
+    # The maximum value that we expect after removing a spikes
+    max_value_after_spike_removal = 10
+
+    # Add three spikes
+    s.data[1, 0, 1] += 40
+    s.data[0, 2, 29] += 20
+    s.data[1, 2, 14] += 100
+    wd = s.spikes_removal_tool(**KWARGS)["ipywidgets"]["wdict"]
+
+    def next():
+        wd["next_button"]._click_handlers(wd["next_button"])
+
+    def previous():
+        wd["previous_button"]._click_handlers(wd["previous_button"])
+
+    def remove():
+        wd["remove_button"]._click_handlers(wd["remove_button"])
+    wd["threshold"].value = 25
+    next()
+    assert s.axes_manager.indices == (0, 1)
+    wd["threshold"].value = 15
+    assert s.axes_manager.indices == (0, 0)
+    next()
+    assert s.axes_manager.indices == (2, 0)
+    next()
+    assert s.axes_manager.indices == (0, 1)
+    previous()
+    assert s.axes_manager.indices == (2, 0)
+    wd["add_noise"].value = False
+    remove()
+    assert s.data[0, 2, 29] < max_value_after_spike_removal
+    assert s.axes_manager.indices == (0, 1)
+    remove()
+    assert s.data[1, 0, 1] < max_value_after_spike_removal
+    assert s.axes_manager.indices == (2, 1)
+    np.random.seed(1)
+    wd["add_noise"].value = True
+    wd["spline_order"].value = 1
+    remove()
+    assert s.data[1, 2, 14] < max_value_after_spike_removal
+    # After going through the whole dataset, come back to (0, 0) position
+    assert s.axes_manager.indices == (0, 0)
```

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/tools.py` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -809,21 +809,14 @@
     previous.on_click(on_previous_clicked)
 
     def on_remove_clicked(b):
         obj.apply()
     remove.on_click(on_remove_clicked)
     labeled_spline_order = labelme("Spline order", spline_order)
 
-    def enable_interpolator_kind(change):
-        if change.new == "Spline":
-            for child in labeled_spline_order.children:
-                child.layout.display = ""
-        else:
-            for child in labeled_spline_order.children:
-                child.layout.display = "none"
     link((obj, "threshold"), (threshold, "value"))
     link((obj, "add_noise"), (add_noise, "value"))
     link((obj, "default_spike_width"),
          (default_spike_width, "value"))
     link((obj, "spline_order"), (spline_order, "value"))
     link((obj, "index"), (progress_bar, "value"))
     # Trigger the function that controls the visibility  as
```

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets/utils.py` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets/utils.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets.egg-info/PKG-INFO` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hyperspy-gui-ipywidgets
-Version: 2.0
+Name: hyperspy_gui_ipywidgets
+Version: 2.0.1
 Summary: ipywidgets GUI elements for the HyperSpy framework.
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -700,14 +700,15 @@
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hyperspy>=2.0rc0
 Requires-Dist: ipywidgets>=7.0
 Requires-Dist: link_traits
+Requires-Dist: ipympl
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-rerunfailures; extra == "tests"
 Requires-Dist: setuptools-scm; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
```

### Comparing `hyperspy_gui_ipywidgets-2.0/hyperspy_gui_ipywidgets.egg-info/SOURCES.txt` & `hyperspy_gui_ipywidgets-2.0.1/hyperspy_gui_ipywidgets.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .gitignore
 CHANGES.md
 LICENSE
 README.md
+prepare_release.py
 pyproject.toml
+releasing_guide.md
 .github/dependabot.yml
 .github/workflows/package_and_test.yml
 .github/workflows/release.yml
 .github/workflows/tests.yml
 hyperspy_gui_ipywidgets/__init__.py
 hyperspy_gui_ipywidgets/axes.py
 hyperspy_gui_ipywidgets/conftest.py
```

### Comparing `hyperspy_gui_ipywidgets-2.0/images/preferences_gui.png` & `hyperspy_gui_ipywidgets-2.0.1/images/preferences_gui.png`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_ipywidgets-2.0/pyproject.toml` & `hyperspy_gui_ipywidgets-2.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,20 @@
   "Operating System :: Unix",
   "Operating System :: MacOS",
 ]
 dependencies = [
   "hyperspy>=2.0rc0",
   "ipywidgets>=7.0",
   "link_traits",
+  "ipympl", # for convenience
 ]
 dynamic = ["version"]
 
 [project.entry-points."hyperspy.extensions"]
-hyperspy-gui-ipywidgets = "hyperspy_gui_ipywidgets"
+hyperspy_gui_ipywidgets = "hyperspy_gui_ipywidgets"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 tests = [
   "pytest",
@@ -66,14 +67,15 @@
 
 [tool.coverage.run]
 branch = true
 source = ["hyperspy_gui_ipywidgets"]
 omit = [
   "hyperspy_gui_ipywidgets/tests/*",
   "hyperspy_gui_ipywidgets/conftest.py",
+  "prepare_release.py",
 ]
 
 [tool.coverage.report]
 precision = 2
 
 [tool.pytest.ini_options]
 #  "-ra",  # Display summary: "all except passes"
@@ -87,7 +89,9 @@
 include = ["hyperspy_gui_ipywidgets*"]
 
 [tool.setuptools.package-data]
 "*" = ["*.yaml"]
 
 [tool.setuptools_scm]
 # Presence enables setuptools_scm, the version will be determine at build time from git
+# The version will be updated by the `prepare_release.py` script
+fallback_version = "2.0.2.dev0"
```

