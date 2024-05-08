# Comparing `tmp/hyperspy_gui_traitsui-2.0.tar.gz` & `tmp/hyperspy_gui_traitsui-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperspy_gui_traitsui-2.0.tar", last modified: Thu Nov 16 18:22:01 2023, max compression
+gzip compressed data, was "hyperspy_gui_traitsui-2.0.1.tar", last modified: Wed May  8 17:13:26 2024, max compression
```

## Comparing `hyperspy_gui_traitsui-2.0.tar` & `hyperspy_gui_traitsui-2.0.1.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 18:22:01.707960 hyperspy_gui_traitsui-2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 18:22:01.703960 hyperspy_gui_traitsui-2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 18:22:01.703960 hyperspy_gui_traitsui-2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/.github/workflows/package_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43960 2023-11-16 18:22:01.707960 hyperspy_gui_traitsui-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 18:22:01.703960 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/axes.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/buttons.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/hyperspy_extension.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/microscope_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/preferences.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2856 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/roi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 18:22:01.707960 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1497 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/tests/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/tests/test_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       62 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21365 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 18:22:01.707960 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43960 2023-11-16 18:22:01.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-11-16 18:22:01.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 18:22:01.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-16 18:22:01.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-16 18:22:01.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-16 18:22:01.000000 hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 18:22:01.707960 hyperspy_gui_traitsui-2.0/images/
--rw-r--r--   0 runner    (1001) docker     (127)    32764 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/images/preferences_gui.png
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-11-16 18:21:37.000000 hyperspy_gui_traitsui-2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 18:22:01.707960 hyperspy_gui_traitsui-2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:26.704028 hyperspy_gui_traitsui-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:26.696027 hyperspy_gui_traitsui-2.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:26.696027 hyperspy_gui_traitsui-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/.github/workflows/package_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43960 2024-05-08 17:13:26.700027 hyperspy_gui_traitsui-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:26.700027 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:26.700027 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/_external/
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/_external/bounds_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/_external/range_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/hyperspy_extension.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/microscope_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/preferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2856 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/roi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:26.700027 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1497 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/tests/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/tests/test_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20730 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:26.700027 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43960 2024-05-08 17:13:26.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-08 17:13:26.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:13:26.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 17:13:26.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-08 17:13:26.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 17:13:26.000000 hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:26.700027 hyperspy_gui_traitsui-2.0.1/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    32764 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/images/preferences_gui.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/prepare_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-08 17:13:18.000000 hyperspy_gui_traitsui-2.0.1/releasing_guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:13:26.704028 hyperspy_gui_traitsui-2.0.1/setup.cfg
```

### Comparing `hyperspy_gui_traitsui-2.0/.github/dependabot.yml` & `hyperspy_gui_traitsui-2.0.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/.github/workflows/codeql.yml` & `hyperspy_gui_traitsui-2.0.1/.github/workflows/codeql.yml`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
   pull_request:
     # The branches below must be a subset of the branches above
     branches: [ "main" ]
     paths-ignore:
       - '**/*.md'
       - '**/*.rst'
       - '**/*.txt'
+      - 'hyperspy_gui_traitsui/_external/*.py'
   schedule:
     # run once a week
     - cron: '16 13 * * 5'
 
 jobs:
   analyze:
     name: Analyze
@@ -39,19 +40,19 @@
 
     steps:
     - name: Checkout repository
       uses: actions/checkout@v4
 
     # Initializes the CodeQL tools for scanning.
     - name: Initialize CodeQL
-      uses: github/codeql-action/init@v2
+      uses: github/codeql-action/init@v3
       with:
         languages: ${{ matrix.language }}
         # If you wish to specify custom queries, you can do so here or in a config file.
         # By default, queries listed here will override any specified in a config file.
         # Prefix the list here with "+" to use these queries and those in the config file.
 
         # Details on CodeQL's query packs refer to : https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/configuring-code-scanning#using-queries-in-ql-packs
         queries: security-extended,security-and-quality
 
     - name: Perform CodeQL Analysis
-      uses: github/codeql-action/analyze@v2
+      uses: github/codeql-action/analyze@v3
```

### Comparing `hyperspy_gui_traitsui-2.0/.github/workflows/release.yml` & `hyperspy_gui_traitsui-2.0.1/.github/workflows/release.yml`

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

### Comparing `hyperspy_gui_traitsui-2.0/.github/workflows/tests.yml` & `hyperspy_gui_traitsui-2.0.1/.github/workflows/tests.yml`

 * *Files 5% similar despite different names*

```diff
@@ -30,25 +30,26 @@
           - PYTHON_VERSION: '3.8'
             OLDEST_SUPPORTED_VERSION: true
             # Matching setup.py
             DEPENDENCIES: traits==5.0 traitsui==6.1 pyqt5==5.12.0
 
     steps:
       - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
 
       - name: Fetch tags upstream
         if: ${{ github.repository_owner != 'hyperspy' }}
         # Needs to fetch the tags from upstream to get the
         # correct version with setuptools_scm
         run: |
           git remote add upstream https://github.com/hyperspy/hyperspy_gui_traitsui.git
-          git fetch --prune --unshallow
           git fetch upstream --tags
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         name: Install Python
         with:
           python-version: ${{ matrix.PYTHON_VERSION }}
 
       - name: Display version
         run: |
           python --version
@@ -67,18 +68,18 @@
           sudo apt-get install libxcb-icccm4
           sudo apt-get install libxcb-image0
           sudo apt-get install libxcb-keysyms1
           sudo apt-get install libxcb-randr0
           sudo apt-get install libxcb-render-util0
           sudo apt-get install libxcb-xinerama0
 
-      - name: Install HyperSpy (RELEASE_next_major)
+      - name: Install HyperSpy (RELEASE_next_minor)
         if: contains( matrix.LABEL, 'RnM')
         run: |
-          pip install git+https://github.com/hyperspy/hyperspy.git@RELEASE_next_major
+          pip install git+https://github.com/hyperspy/hyperspy.git@RELEASE_next_minor
 
       - name: Install HyperSpy (RELEASE_next_patch)
         if: contains( matrix.LABEL, 'RnP')
         run: |
           pip install git+https://github.com/hyperspy/hyperspy.git@RELEASE_next_patch
 
       - name: Install exSpy
@@ -97,8 +98,10 @@
       - name: Run test suite
         run: |
           sudo apt-get install xvfb
           xvfb-run pytest ${{ env.PYTEST_ARGS }} ${{ env.PYTEST_ARGS_COVERAGE }}
 
       - name: Upload coverage to Codecov
         if: ${{ always() }} && ${{ env.PYTEST_ARGS_COVERAGE }} 
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `hyperspy_gui_traitsui-2.0/.gitignore` & `hyperspy_gui_traitsui-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/CHANGES.md` & `hyperspy_gui_traitsui-2.0.1/CHANGES.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 ..
   Add a single entry in the corresponding section below.
   See https://keepachangelog.com for details
 
+## v2.0.1 (2024-08-05)
+
+* Fix getting matplotlib backend for matplotlib >= 3.10.dev ([#78](https://github.com/hyperspy/hyperspy_gui_traitsui/pull/78)).
+* Use `qt` instead of `qt4` when setting `ETSConfig.toolkit` ([#78](https://github.com/hyperspy/hyperspy_gui_traitsui/pull/78)).
+* Fix slider in image contrast editor on python >=3.10 ([#76](https://github.com/hyperspy/hyperspy_gui_traitsui/pull/76)).
+* Fix getting version with editable installation ([#75](https://github.com/hyperspy/hyperspy_gui_traitsui/pull/75)).
+* Add releasing guide and release script ([#75](https://github.com/hyperspy/hyperspy_gui_traitsui/pull/75)).
+* Fix regression with editable installation ([#74](https://github.com/hyperspy/hyperspy_gui_traitsui/pull/74)).
+
 ## v2.0 (2023-11-16)
 
 * Consolidate package metadata into `pyproject.toml` ([#67](https://github.com/hyperspy/hyperspy_gui_traitsui/pull/67))
 * Support HyperSpy 2.0 and set HyperSpy requirement to >=2.0 ([#65](https://github.com/hyperspy/hyperspy_gui_traitsui/pull/65))
 * Remove use of deprecated HyperSpy preferences `warn_if_guis_are_missing` ([#58](https://github.com/hyperspy/hyperspy_gui_traitsui/pull/58))
 * Remove `integrate_in_range` widgets, as the corresponding method has been removed in hyperspy 2.0. ([#53](https://github.com/hyperspy/hyperspy_gui_traitsui/pull/53))
 * Added github action for code scanning using the codeQL engine ([#51](https://github.com/hyperspy/hyperspy_gui_traitsui/pull/51))
```

### Comparing `hyperspy_gui_traitsui-2.0/LICENSE` & `hyperspy_gui_traitsui-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/PKG-INFO` & `hyperspy_gui_traitsui-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperspy_gui_traitsui
-Version: 2.0
+Version: 2.0.1
 Summary: traitsui GUI elements for the HyperSpy framework.
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -697,18 +697,18 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: hyperspy>=2.0rc0
+Requires-Dist: hyperspy>=2.1.0.dev119
 Requires-Dist: link_traits
 Requires-Dist: traits>=5.0
-Requires-Dist: traitsui!=8.0.0,>=6.1
+Requires-Dist: traitsui>=7.3
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-rerunfailures; extra == "tests"
 Requires-Dist: setuptools-scm; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
```

### Comparing `hyperspy_gui_traitsui-2.0/README.md` & `hyperspy_gui_traitsui-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/__init__.py` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,33 +14,47 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with  HyperSpy.  If not, see <http://www.gnu.org/licenses/>.
 
 
 import importlib
+from importlib.metadata import version
 import logging
 from pathlib import Path
 
 import matplotlib
 from traits.etsconfig.api import ETSConfig
 
 from hyperspy.defaults_parser import preferences
 
 
-if Path(__file__).parent.parent.name == "site-packages":  # pragma: no cover
-    # Tested in the "Package & Test" workflow on GitHub CI
-    from importlib.metadata import version
-
-    __version__ = version("hyperspy_gui_traitsui")
-else:
-    # Editable install
-    from setuptools_scm import get_version
+__version__ = version("hyperspy_gui_traitsui")
 
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
     'messages',
     'microscope_parameters',
@@ -83,21 +97,21 @@
                     ETSConfig.toolkit, toolkit))
     except ValueError:
         _logger.debug("Setting ETS toolkit to %s failed" % toolkit)
         set_ets_toolkit("null")
 
 
 # Get the backend from matplotlib
-backend = matplotlib.get_backend()
+backend = matplotlib.get_backend().lower()
 _logger.debug('Loading hyperspy.traitsui_gui')
 _logger.debug('Current MPL backend: %s', backend)
-if "WX" in backend:
+if "wx" in backend:
     set_ets_toolkit("wx")
-elif "Qt" in backend:
-    set_ets_toolkit("qt4")
+elif "qt" in backend:
+    set_ets_toolkit("qt")
 elif ETSConfig.toolkit == "":
     # The toolkit has not been set and no supported toolkit is available, so
     # setting it to "null"
     set_ets_toolkit("null")
     _logger.warning(
         f"The {backend} matplotlib backend is not compatible with the "
         "traitsui GUI elements. For more information, read "
```

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/axes.py` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/axes.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/buttons.py` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/buttons.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/hyperspy_extension.yaml` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/hyperspy_extension.yaml`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/messages.py` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/messages.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/microscope_parameters.py` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/microscope_parameters.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/model.py` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/model.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/preferences.py` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/preferences.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/roi.py` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/roi.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/tests/test_axes.py` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/tests/test_import.py` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/tests/test_model.py` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/tests/test_tools.py` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui/tools.py` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from packaging.version import Version
-
 import traitsui
 import traitsui.api as tu
 from traitsui.menu import OKButton, CancelButton, OKCancelButtons
 
 from hyperspy_gui_traitsui.axes import get_navigation_sliders_group
 from hyperspy_gui_traitsui.buttons import (
     OurApplyButton,HelpButton, OurResetButton
@@ -324,27 +322,15 @@
         buttons=[OKButton, CancelButton],
         title='Load file')
     return obj, {"view": view}
 
 
 @add_display_arg
 def image_contrast_editor_traitsui(obj, **kwargs):
-    # In traitsui 8.0.0, traitsui.qt4 was changed to traitsui.qt
-    if Version(traitsui.__version__) >= Version('8.0.0'):
-        from traitsui.qt.extra.bounds_editor import BoundsEditor
-    else:
-        from traitsui.qt4.extra.bounds_editor import BoundsEditor
-
-    # format has been deprecated in Release 7.3.0, replaced by format_str
-    # https://github.com/enthought/traitsui/pull/1684
-    # Remove and simplify when minimum traitsui version is 7.3.0
-    FORMAT_STR = 'format' if Version(traitsui.__version__) < Version('7.0.0') \
-        else 'format_str'
-    def get_format_dict(formatting):
-        return {FORMAT_STR:formatting}
+    from hyperspy_gui_traitsui._external.bounds_editor import BoundsEditor
 
     view = tu.View(
         tu.Group(
             tu.Item('ss_left_value',
                     label='Min',
                     show_label=True,
                     style='readonly',
@@ -359,20 +345,20 @@
             show_border=True
             ),
         tu.Group(
             tu.Item('auto',
                     label='Auto',
                     show_label=True,
                     ),
-            tu.Item('vmin_percentile',
+            tu.Item('percentile_range',
                     label='vmin/vmax percentile',
                     editor=BoundsEditor(
                         low_name='vmin_percentile',
                         high_name='vmax_percentile',
-                        **get_format_dict('%.2f'),
+                        format_str='%.2f',
                         )),
             show_border=True,
             ),
         tu.Group(
             tu.Item('bins',
                     label='Bins',
                     show_label=True,
@@ -384,35 +370,35 @@
             tu.Item('gamma',
                     label='Gamma',
                     show_label=True,
                     visible_when='norm == "Power"',
                     editor=tu.RangeEditor(low=0.1,
                                           high=3.,
                                           mode="slider",
-                                          **get_format_dict('%.2f'),
+                                          format_str='%.2f',
                                           ),
                     ),
             tu.Item('linthresh',
                     label='Linear threshold',
                     show_label=True,
                     visible_when='norm == "Symlog"',
                     editor=tu.RangeEditor(low=0.01,
                                           high=1.,
                                           mode="slider",
-                                          **get_format_dict('%.2f'),
+                                          format_str='%.2f',
                                           ),
                     ),
             tu.Item('linscale',
                     label='Linear scale',
                     show_label=True,
                     visible_when='norm == "Symlog"',
                     editor=tu.RangeEditor(low=0.,
                                           high=10.,
                                           mode="slider",
-                                          **get_format_dict('%.2f'),
+                                          format_str='%.2f',
                                           ),
                     ),
             show_border=True,
             ),
         tu.Item('_'),
         handler=ImageContrastHandler,
         buttons=[OKButton,
```

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui.egg-info/PKG-INFO` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hyperspy-gui-traitsui
-Version: 2.0
+Name: hyperspy_gui_traitsui
+Version: 2.0.1
 Summary: traitsui GUI elements for the HyperSpy framework.
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -697,18 +697,18 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: hyperspy>=2.0rc0
+Requires-Dist: hyperspy>=2.1.0.dev119
 Requires-Dist: link_traits
 Requires-Dist: traits>=5.0
-Requires-Dist: traitsui!=8.0.0,>=6.1
+Requires-Dist: traitsui>=7.3
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-rerunfailures; extra == "tests"
 Requires-Dist: setuptools-scm; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
```

### Comparing `hyperspy_gui_traitsui-2.0/hyperspy_gui_traitsui.egg-info/SOURCES.txt` & `hyperspy_gui_traitsui-2.0.1/hyperspy_gui_traitsui.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 .gitignore
 CHANGES.md
 LICENSE
 README.md
+prepare_release.py
 pyproject.toml
+releasing_guide.md
 .github/dependabot.yml
 .github/workflows/codeql.yml
 .github/workflows/package_and_test.yml
 .github/workflows/release.yml
 .github/workflows/tests.yml
 hyperspy_gui_traitsui/__init__.py
 hyperspy_gui_traitsui/axes.py
 hyperspy_gui_traitsui/buttons.py
-hyperspy_gui_traitsui/conftest.py
 hyperspy_gui_traitsui/hyperspy_extension.yaml
 hyperspy_gui_traitsui/messages.py
 hyperspy_gui_traitsui/microscope_parameters.py
 hyperspy_gui_traitsui/model.py
 hyperspy_gui_traitsui/preferences.py
 hyperspy_gui_traitsui/roi.py
 hyperspy_gui_traitsui/tools.py
 hyperspy_gui_traitsui/utils.py
 hyperspy_gui_traitsui.egg-info/PKG-INFO
 hyperspy_gui_traitsui.egg-info/SOURCES.txt
 hyperspy_gui_traitsui.egg-info/dependency_links.txt
 hyperspy_gui_traitsui.egg-info/entry_points.txt
 hyperspy_gui_traitsui.egg-info/requires.txt
 hyperspy_gui_traitsui.egg-info/top_level.txt
+hyperspy_gui_traitsui/_external/bounds_editor.py
+hyperspy_gui_traitsui/_external/range_slider.py
 hyperspy_gui_traitsui/tests/__init__.py
 hyperspy_gui_traitsui/tests/test_axes.py
 hyperspy_gui_traitsui/tests/test_import.py
 hyperspy_gui_traitsui/tests/test_model.py
 hyperspy_gui_traitsui/tests/test_tools.py
 hyperspy_gui_traitsui/tests/utils.py
 images/preferences_gui.png
```

### Comparing `hyperspy_gui_traitsui-2.0/images/preferences_gui.png` & `hyperspy_gui_traitsui-2.0.1/images/preferences_gui.png`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-2.0/pyproject.toml` & `hyperspy_gui_traitsui-2.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -28,23 +28,23 @@
   "Programming Language :: Python :: 3.12",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX",
   "Operating System :: Unix",
   "Operating System :: MacOS",
 ]
 dependencies = [
-  "hyperspy>=2.0rc0",
+  "hyperspy>=2.1.0.dev119",
   "link_traits",
   "traits>=5.0",
-  "traitsui>=6.1,!=8.0.0",
+  "traitsui>=7.3",
 ]
 dynamic = ["version"]
 
 [project.entry-points."hyperspy.extensions"]
-hyperspy-gui-traitsui = "hyperspy_gui_traitsui"
+hyperspy_gui_traitsui = "hyperspy_gui_traitsui"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 tests = [
   "pytest",
@@ -67,14 +67,15 @@
 
 [tool.coverage.run]
 branch = true
 source = ["hyperspy_gui_traitsui"]
 omit = [
   "hyperspy_gui_traitsui/tests/*",
   "hyperspy_gui_traitsui/conftest.py",
+  "prepare_release.py",
 ]
 
 [tool.coverage.report]
 precision = 2
 
 [tool.pytest.ini_options]
 #  "-ra",  # Display summary: "all except passes"
@@ -87,8 +88,8 @@
 [tool.setuptools.packages.find]
 include = ["hyperspy_gui_traitsui*"]
 
 [tool.setuptools.package-data]
 "*" = ["*.yaml"]
 
 [tool.setuptools_scm]
-# Presence enables setuptools_scm, the version will be determine at build time from git
+fallback_version = "2.0.2.dev0"
```

