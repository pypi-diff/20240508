# Comparing `tmp/hypercoast-0.2.0.tar.gz` & `tmp/hypercoast-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypercoast-0.2.0.tar", last modified: Sun May  5 22:18:22 2024, max compression
+gzip compressed data, was "hypercoast-0.3.0.tar", last modified: Wed May  8 15:21:38 2024, max compression
```

## Comparing `hypercoast-0.2.0.tar` & `hypercoast-0.3.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.763610 hypercoast-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.755610 hypercoast-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.755610 hypercoast-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.759610 hypercoast-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.763610 hypercoast-0.2.0/HyperCoast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-05 22:18:22.000000 hypercoast-0.2.0/HyperCoast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-05 22:18:22.000000 hypercoast-0.2.0/HyperCoast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 22:18:22.000000 hypercoast-0.2.0/HyperCoast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-05 22:18:22.000000 hypercoast-0.2.0/HyperCoast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-05 22:18:22.000000 hypercoast-0.2.0/HyperCoast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-05 22:18:22.000000 hypercoast-0.2.0/HyperCoast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-05 22:18:11.000000 hypercoast-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-05 22:18:11.000000 hypercoast-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-05 22:18:22.763610 hypercoast-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-05 22:18:11.000000 hypercoast-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.759610 hypercoast-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/emit.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.759610 hypercoast-0.2.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/examples/emit.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/examples/pace.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/hypercoast.md
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.759610 hypercoast-0.2.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/pace.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/ui.md
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.763610 hypercoast-0.2.0/hypercoast/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-05 22:18:11.000000 hypercoast-0.2.0/hypercoast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-05 22:18:11.000000 hypercoast-0.2.0/hypercoast/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    37765 2024-05-05 22:18:11.000000 hypercoast-0.2.0/hypercoast/emit.py
--rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-05-05 22:18:11.000000 hypercoast-0.2.0/hypercoast/hypercoast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-05-05 22:18:11.000000 hypercoast-0.2.0/hypercoast/pace.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-05-05 22:18:11.000000 hypercoast-0.2.0/hypercoast/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-05 22:18:11.000000 hypercoast-0.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-05 22:18:11.000000 hypercoast-0.2.0/pyproject-codespell.precommit-toml
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-05 22:18:11.000000 hypercoast-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-05 22:18:11.000000 hypercoast-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-05 22:18:11.000000 hypercoast-0.2.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 22:18:22.763610 hypercoast-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.763610 hypercoast-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-05 22:18:11.000000 hypercoast-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-05 22:18:11.000000 hypercoast-0.2.0/tests/test_hypercoast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.513407 hypercoast-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.501407 hypercoast-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.505407 hypercoast-0.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.509407 hypercoast-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.513407 hypercoast-0.3.0/HyperCoast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-08 15:21:38.000000 hypercoast-0.3.0/HyperCoast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-08 15:21:38.000000 hypercoast-0.3.0/HyperCoast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:21:38.000000 hypercoast-0.3.0/HyperCoast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 15:21:38.000000 hypercoast-0.3.0/HyperCoast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 15:21:38.000000 hypercoast-0.3.0/HyperCoast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 15:21:38.000000 hypercoast-0.3.0/HyperCoast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-08 15:21:25.000000 hypercoast-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 15:21:25.000000 hypercoast-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-08 15:21:38.513407 hypercoast-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-08 15:21:25.000000 hypercoast-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.509407 hypercoast-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/emit.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.513407 hypercoast-0.3.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/examples/emit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/examples/pace.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/hypercoast.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.513407 hypercoast-0.3.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/pace.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/ui.md
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.513407 hypercoast-0.3.0/hypercoast/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-08 15:21:25.000000 hypercoast-0.3.0/hypercoast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-08 15:21:25.000000 hypercoast-0.3.0/hypercoast/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37765 2024-05-08 15:21:25.000000 hypercoast-0.3.0/hypercoast/emit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13949 2024-05-08 15:21:25.000000 hypercoast-0.3.0/hypercoast/hypercoast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-05-08 15:21:25.000000 hypercoast-0.3.0/hypercoast/pace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-08 15:21:25.000000 hypercoast-0.3.0/hypercoast/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-08 15:21:25.000000 hypercoast-0.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-08 15:21:25.000000 hypercoast-0.3.0/pyproject-codespell.precommit-toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-08 15:21:25.000000 hypercoast-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 15:21:25.000000 hypercoast-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-08 15:21:25.000000 hypercoast-0.3.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:21:38.513407 hypercoast-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.513407 hypercoast-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 15:21:25.000000 hypercoast-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-08 15:21:25.000000 hypercoast-0.3.0/tests/test_hypercoast.py
```

### Comparing `hypercoast-0.2.0/.github/workflows/docs-build.yml` & `hypercoast-0.3.0/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.2.0/.github/workflows/docs.yml` & `hypercoast-0.3.0/.github/workflows/docs.yml`

 * *Files 25% similar despite different names*

```diff
@@ -5,14 +5,16 @@
             - main
             - master
 jobs:
     deploy:
         runs-on: ubuntu-latest
         steps:
             - uses: actions/checkout@v4
+              with:
+                  fetch-depth: 0
             - uses: actions/setup-python@v5
               with:
                   python-version: "3.11"
 
             - name: Install dependencies
               run: |
                   python -m pip install --upgrade pip
```

### Comparing `hypercoast-0.2.0/.github/workflows/installation.yml` & `hypercoast-0.3.0/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.2.0/.github/workflows/macos.yml` & `hypercoast-0.3.0/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.2.0/.github/workflows/pypi.yml` & `hypercoast-0.3.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.2.0/.github/workflows/ubuntu.yml` & `hypercoast-0.3.0/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.2.0/.github/workflows/windows.yml` & `hypercoast-0.3.0/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.2.0/.gitignore` & `hypercoast-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hypercoast-0.2.0/.pre-commit-config.yaml` & `hypercoast-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.2.0/HyperCoast.egg-info/PKG-INFO` & `hypercoast-0.3.0/HyperCoast.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -22,14 +22,15 @@
 Requires-Dist: hvplot
 Requires-Dist: leafmap
 Requires-Dist: localtileserver
 Requires-Dist: netcdf4
 Requires-Dist: numpy
 Requires-Dist: rioxarray
 Requires-Dist: s3fs
+Requires-Dist: scipy
 Requires-Dist: xarray
 Provides-Extra: all
 Requires-Dist: HyperCoast[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: cartopy; extra == "extra"
 
 # HyperCoast
@@ -44,20 +45,24 @@
 **A Python package for visualizing and analyzing hyperspectral data in coastal regions**
 
 -   Free software: MIT License
 -   Documentation: <https://hypercoast.org>
 
 ## Features
 
--   Interactive visualization and analysis of hyperspectral data (e.g., [EMIT](https://earth.jpl.nasa.gov/emit/), [PACE](https://pace.gsfc.nasa.gov/))
+-   Interactive visualization and analysis of hyperspectral data (e.g., [EMIT](https://earth.jpl.nasa.gov/emit), [PACE](https://pace.gsfc.nasa.gov))
 -   Interactive extraction and visualization of spectral signatures
 -   Saving spectral signatures as CSV files
 
-## Demo
+## Demos
 
--   Visualizing spectral signature interactively
+-   Visualizing NASA [EMIT](https://earth.jpl.nasa.gov/emit) data interactively
 
 ![](https://i.imgur.com/zeyABMq.gif)
 
+-   Visualizing NASA [PACE](https://pace.gsfc.nasa.gov) data interactively
+
+![](https://i.imgur.com/HBMjW6o.gif)
+
 ## Acknowledgement
 
 This projects draws inspiration and adapts source code from the [nasa/EMIT-Data-Resources](https://github.com/nasa/EMIT-Data-Resources) repository. Credit goes to the original authors.
```

### Comparing `hypercoast-0.2.0/HyperCoast.egg-info/SOURCES.txt` & `hypercoast-0.3.0/HyperCoast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypercoast-0.2.0/LICENSE` & `hypercoast-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hypercoast-0.2.0/PKG-INFO` & `hypercoast-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -22,14 +22,15 @@
 Requires-Dist: hvplot
 Requires-Dist: leafmap
 Requires-Dist: localtileserver
 Requires-Dist: netcdf4
 Requires-Dist: numpy
 Requires-Dist: rioxarray
 Requires-Dist: s3fs
+Requires-Dist: scipy
 Requires-Dist: xarray
 Provides-Extra: all
 Requires-Dist: HyperCoast[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: cartopy; extra == "extra"
 
 # HyperCoast
@@ -44,20 +45,24 @@
 **A Python package for visualizing and analyzing hyperspectral data in coastal regions**
 
 -   Free software: MIT License
 -   Documentation: <https://hypercoast.org>
 
 ## Features
 
--   Interactive visualization and analysis of hyperspectral data (e.g., [EMIT](https://earth.jpl.nasa.gov/emit/), [PACE](https://pace.gsfc.nasa.gov/))
+-   Interactive visualization and analysis of hyperspectral data (e.g., [EMIT](https://earth.jpl.nasa.gov/emit), [PACE](https://pace.gsfc.nasa.gov))
 -   Interactive extraction and visualization of spectral signatures
 -   Saving spectral signatures as CSV files
 
-## Demo
+## Demos
 
--   Visualizing spectral signature interactively
+-   Visualizing NASA [EMIT](https://earth.jpl.nasa.gov/emit) data interactively
 
 ![](https://i.imgur.com/zeyABMq.gif)
 
+-   Visualizing NASA [PACE](https://pace.gsfc.nasa.gov) data interactively
+
+![](https://i.imgur.com/HBMjW6o.gif)
+
 ## Acknowledgement
 
 This projects draws inspiration and adapts source code from the [nasa/EMIT-Data-Resources](https://github.com/nasa/EMIT-Data-Resources) repository. Credit goes to the original authors.
```

### Comparing `hypercoast-0.2.0/README.md` & `hypercoast-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -10,20 +10,24 @@
 **A Python package for visualizing and analyzing hyperspectral data in coastal regions**
 
 -   Free software: MIT License
 -   Documentation: <https://hypercoast.org>
 
 ## Features
 
--   Interactive visualization and analysis of hyperspectral data (e.g., [EMIT](https://earth.jpl.nasa.gov/emit/), [PACE](https://pace.gsfc.nasa.gov/))
+-   Interactive visualization and analysis of hyperspectral data (e.g., [EMIT](https://earth.jpl.nasa.gov/emit), [PACE](https://pace.gsfc.nasa.gov))
 -   Interactive extraction and visualization of spectral signatures
 -   Saving spectral signatures as CSV files
 
-## Demo
+## Demos
 
--   Visualizing spectral signature interactively
+-   Visualizing NASA [EMIT](https://earth.jpl.nasa.gov/emit) data interactively
 
 ![](https://i.imgur.com/zeyABMq.gif)
 
+-   Visualizing NASA [PACE](https://pace.gsfc.nasa.gov) data interactively
+
+![](https://i.imgur.com/HBMjW6o.gif)
+
 ## Acknowledgement
 
 This projects draws inspiration and adapts source code from the [nasa/EMIT-Data-Resources](https://github.com/nasa/EMIT-Data-Resources) repository. Credit goes to the original authors.
```

### Comparing `hypercoast-0.2.0/docs/contributing.md` & `hypercoast-0.3.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.2.0/docs/examples/emit.ipynb` & `hypercoast-0.3.0/docs/examples/emit.ipynb`

 * *Files identical despite different names*

### Comparing `hypercoast-0.2.0/docs/index.md` & `hypercoast-0.3.0/docs/index.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,20 +9,24 @@
 **A Python package for visualizing and analyzing hyperspectral data in coastal regions**
 
 -   Free software: MIT License
 -   Documentation: <https://hypercoast.org>
 
 ## Features
 
--   Interactive visualization and analysis of hyperspectral data (e.g., [EMIT](https://earth.jpl.nasa.gov/emit/), [PACE](https://pace.gsfc.nasa.gov/))
+-   Interactive visualization and analysis of hyperspectral data (e.g., [EMIT](https://earth.jpl.nasa.gov/emit), [PACE](https://pace.gsfc.nasa.gov))
 -   Interactive extraction and visualization of spectral signatures
 -   Saving spectral signatures as CSV files
 
-## Demo
+## Demos
 
--   Visualizing spectral signature interactively
+-   Visualizing NASA [EMIT](https://earth.jpl.nasa.gov/emit) data interactively
 
 ![](https://i.imgur.com/zeyABMq.gif)
 
+-   Visualizing NASA [PACE](https://pace.gsfc.nasa.gov) data interactively
+
+![](https://i.imgur.com/HBMjW6o.gif)
+
 ## Acknowledgement
 
 This projects draws inspiration and adapts source code from the [nasa/EMIT-Data-Resources](https://github.com/nasa/EMIT-Data-Resources) repository. Credit goes to the original authors.
```

### Comparing `hypercoast-0.2.0/docs/installation.md` & `hypercoast-0.3.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.2.0/hypercoast/common.py` & `hypercoast-0.3.0/hypercoast/common.py`

 * *Files identical despite different names*

### Comparing `hypercoast-0.2.0/hypercoast/emit.py` & `hypercoast-0.3.0/hypercoast/emit.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,23 +222,23 @@
     if isinstance(data, str):
         data = read_emit(data, ortho=True)
 
     ds_geo = data.transpose("wavelengths", "latitude", "longitude")
     ds_geo.to_netcdf(output, **kwargs)
 
 
-def emit_to_image(data, output=None, wavelengths=None, method="nearest", **kwargs):
+def emit_to_image(data, wavelengths=None, method="nearest", output=None, **kwargs):
     """
     Converts an EMIT dataset to an image.
 
     Args:
         data (xarray.Dataset or str): The dataset containing the EMIT data or the file path to the dataset.
-        output (str, optional): The file path where the image will be saved. If None, the image will be returned as a PIL Image object. Defaults to None.
         wavelengths (array-like, optional): The specific wavelengths to select. If None, all wavelengths are selected. Defaults to None.
         method (str, optional): The method to use for data selection. Defaults to "nearest".
+        output (str, optional): The file path where the image will be saved. If None, the image will be returned as a PIL Image object. Defaults to None.
         **kwargs: Additional keyword arguments to be passed to `leafmap.array_to_image`.
 
     Returns:
         rasterio.Dataset or None: The image converted from the dataset. If `output` is provided, the image will be saved to the specified file and the function will return None.
     """
     from leafmap import array_to_image
```

### Comparing `hypercoast-0.2.0/hypercoast/hypercoast.py` & `hypercoast-0.3.0/hypercoast/hypercoast.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Main module."""
 
 import ipyleaflet
 import leafmap
 import xarray as xr
+import numpy as np
 from .common import download_file, netcdf_groups
 from .emit import read_emit, plot_emit, viz_emit, emit_to_netcdf, emit_to_image
 from .pace import *
 
 
 class Map(leafmap.Map):
     """
@@ -125,15 +126,15 @@
         self,
         source,
         wavelengths=None,
         indexes=None,
         colormap=None,
         vmin=None,
         vmax=None,
-        nodata=None,
+        nodata=np.nan,
         attribution=None,
         layer_name="EMIT",
         zoom_to_layer=True,
         visible=True,
         array_args={},
         **kwargs,
     ):
@@ -180,14 +181,84 @@
             zoom_to_layer=zoom_to_layer,
             visible=visible,
             array_args=array_args,
             **kwargs,
         )
 
         self.cog_layer_dict[layer_name]["xds"] = xds
+        self.cog_layer_dict[layer_name]["type"] = "EMIT"
+
+    def add_pace(
+        self,
+        source,
+        wavelengths=None,
+        indexes=None,
+        colormap="jet",
+        vmin=None,
+        vmax=None,
+        nodata=np.nan,
+        attribution=None,
+        layer_name="PACE",
+        zoom_to_layer=True,
+        visible=True,
+        method="nearest",
+        gridded=False,
+        array_args={},
+        **kwargs,
+    ):
+        """Add a PACE dataset to the map.
+            If you are using this function in JupyterHub on a remote server (e.g., Binder, Microsoft Planetary Computer) and
+            if the raster does not render properly, try installing jupyter-server-proxy using `pip install jupyter-server-proxy`,
+            then running the following code before calling this function. For more info, see https://bit.ly/3JbmF93.
+
+            import os
+            os.environ['LOCALTILESERVER_CLIENT_PREFIX'] = 'proxy/{port}'
+
+        Args:
+            source (str): The path to the GeoTIFF file or the URL of the Cloud Optimized GeoTIFF.
+            indexes (int, optional): The band(s) to use. Band indexing starts at 1. Defaults to None.
+            colormap (str, optional): The name of the colormap from `matplotlib` to use when plotting a single band. See https://matplotlib.org/stable/gallery/color/colormap_reference.html. Default is greyscale.
+            vmin (float, optional): The minimum value to use when colormapping the palette when plotting a single band. Defaults to None.
+            vmax (float, optional): The maximum value to use when colormapping the palette when plotting a single band. Defaults to None.
+            nodata (float, optional): The value from the band to use to interpret as not valid data. Defaults to None.
+            attribution (str, optional): Attribution for the source raster. This defaults to a message about it being a local file.. Defaults to None.
+            layer_name (str, optional): The layer name to use. Defaults to 'EMIT'.
+            zoom_to_layer (bool, optional): Whether to zoom to the extent of the layer. Defaults to True.
+            visible (bool, optional): Whether the layer is visible. Defaults to True.
+            array_args (dict, optional): Additional arguments to pass to `array_to_memory_file` when reading the raster. Defaults to {}.
+        """
+
+        if isinstance(source, str):
+
+            source = read_pace(source)
+
+        image = pace_to_image(
+            source, wavelengths=wavelengths, method=method, gridded=gridded
+        )
+
+        if isinstance(wavelengths, list) and len(wavelengths) > 1:
+            colormap = None
+
+        self.add_raster(
+            image,
+            indexes=indexes,
+            colormap=colormap,
+            vmin=vmin,
+            vmax=vmax,
+            nodata=nodata,
+            attribution=attribution,
+            layer_name=layer_name,
+            zoom_to_layer=zoom_to_layer,
+            visible=visible,
+            array_args=array_args,
+            **kwargs,
+        )
+
+        self.cog_layer_dict[layer_name]["xds"] = source
+        self.cog_layer_dict[layer_name]["type"] = "PACE"
 
     def set_plot_options(
         self,
         add_marker_cluster=False,
         plot_type=None,
         overlay=False,
         position="bottomright",
```

### Comparing `hypercoast-0.2.0/hypercoast/ui.py` & `hypercoast-0.3.0/hypercoast/ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """This module contains the user interface for the hypercoast package.
 """
 
 import os
 import ipyleaflet
 import ipywidgets as widgets
 import numpy as np
+import xarray as xr
 from bqplot import pyplot as plt
 from IPython.core.display import display
 from ipyfilechooser import FileChooser
+from .pace import extract_pace
 
 
 class SpectralWidget(widgets.HBox):
     """
     A widget for spectral data visualization on a map.
 
     Attributes:
@@ -136,22 +138,36 @@
                     markers = self._host_map._plot_markers
                     marker_cluster = self._host_map._plot_marker_cluster
                     markers.append(ipyleaflet.Marker(location=latlon))
                     marker_cluster.markers = markers
                     self._host_map._plot_marker_cluster = marker_cluster
 
                     ds = self._host_map.cog_layer_dict[layer_name]["xds"]
-                    da = ds.sel(latitude=lat, longitude=lon, method="nearest")[
-                        "reflectance"
-                    ]
-
-                    if "wavelengths" not in self._host_map._spectral_data:
-                        self._host_map._spectral_data["wavelengths"] = ds[
-                            "wavelengths"
-                        ].values
+                    if self._host_map.cog_layer_dict[layer_name]["type"] == "EMIT":
+                        da = ds.sel(latitude=lat, longitude=lon, method="nearest")[
+                            "reflectance"
+                        ]
+
+                        if "wavelengths" not in self._host_map._spectral_data:
+                            self._host_map._spectral_data["wavelengths"] = ds[
+                                "wavelengths"
+                            ].values
+                    elif self._host_map.cog_layer_dict[layer_name]["type"] == "PACE":
+                        try:
+                            da = extract_pace(ds, lat, lon)
+                        except:
+                            da = xr.DataArray(
+                                np.full(len(ds["wavelength"]), np.nan),
+                                dims=["wavelength"],
+                                coords={"wavelength": ds["wavelength"]},
+                            )
+                        if "wavelengths" not in self._host_map._spectral_data:
+                            self._host_map._spectral_data["wavelengths"] = ds[
+                                "wavelength"
+                            ].values
 
                     self._host_map._spectral_data[f"({lat:.4f} {lon:.4f})"] = da.values
 
                     da[da < 0] = np.nan
                     # fig, ax = plt.subplots()
                     # da.plot.line(ax=ax)
                     # display(fig)
```

### Comparing `hypercoast-0.2.0/mkdocs.yml` & `hypercoast-0.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.2.0/pyproject.toml` & `hypercoast-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HyperCoast"
-version = "0.2.0"
+version = "0.3.0"
 dynamic = [
     "dependencies",
 ]
 description = "A Python package for processing hyperspectral data in coastal regions"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.2.0"
+current_version = "0.3.0"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

