# Comparing `tmp/aiosysbus-1.1.6.tar.gz` & `tmp/aiosysbus-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosysbus-1.1.6.tar", last modified: Sun Feb  4 15:41:26 2024, max compression
+gzip compressed data, was "aiosysbus-1.1.7.tar", last modified: Wed May  8 07:43:46 2024, max compression
```

## Comparing `aiosysbus-1.1.6.tar` & `aiosysbus-1.1.7.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 15:41:26.439315 aiosysbus-1.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 15:41:26.431316 aiosysbus-1.1.6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 15:41:26.431316 aiosysbus-1.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-02-04 15:41:26.439315 aiosysbus-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 15:41:26.435315 aiosysbus-1.1.6/aiosysbus/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/aiosysbus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 15:41:26.435315 aiosysbus-1.1.6/aiosysbus/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/api/call.py
--rw-r--r--   0 runner    (1001) docker     (127)    11998 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/api/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/api/diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/api/dnsdhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15291 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/api/nemo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16913 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/api/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/api/nmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/api/powermgmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/api/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/api/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/api/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/api/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/aiosysbus/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 15:41:26.439315 aiosysbus-1.1.6/aiosysbus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-02-04 15:41:26.000000 aiosysbus-1.1.6/aiosysbus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-04 15:41:26.000000 aiosysbus-1.1.6/aiosysbus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 15:41:26.000000 aiosysbus-1.1.6/aiosysbus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-04 15:41:26.000000 aiosysbus-1.1.6/aiosysbus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-04 15:41:26.000000 aiosysbus-1.1.6/aiosysbus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-04 15:41:26.439315 aiosysbus-1.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 15:41:26.439315 aiosysbus-1.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 15:41:26.439315 aiosysbus-1.1.6/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/tests/fixtures/deviceinfo.json
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-02-04 15:41:09.000000 aiosysbus-1.1.6/tests/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.727547 aiosysbus-1.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.719547 aiosysbus-1.1.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.723547 aiosysbus-1.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-08 07:43:46.727547 aiosysbus-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.723547 aiosysbus-1.1.7/aiosysbus/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/aiosysbus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.727547 aiosysbus-1.1.7/aiosysbus/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/dnsdhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/nemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16914 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/nmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/powermgmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11163 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/aiosysbus/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.727547 aiosysbus-1.1.7/aiosysbus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-08 07:43:46.000000 aiosysbus-1.1.7/aiosysbus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-08 07:43:46.000000 aiosysbus-1.1.7/aiosysbus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:43:46.000000 aiosysbus-1.1.7/aiosysbus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 07:43:46.000000 aiosysbus-1.1.7/aiosysbus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 07:43:46.000000 aiosysbus-1.1.7/aiosysbus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 07:43:46.727547 aiosysbus-1.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.727547 aiosysbus-1.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:43:46.727547 aiosysbus-1.1.7/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/tests/fixtures/deviceinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-08 07:43:38.000000 aiosysbus-1.1.7/tests/test_connection.py
```

### Comparing `aiosysbus-1.1.6/.github/dependabot.yml` & `aiosysbus-1.1.7/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.6/.github/workflows/lint.yml` & `aiosysbus-1.1.7/.github/workflows/lint.yml`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 
       - name: 📦 Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements.txt
 
       - name: Run pre-commit
-        uses: pre-commit/action@v3.0.0
+        uses: pre-commit/action@v3.0.1
```

### Comparing `aiosysbus-1.1.6/.github/workflows/pythonpublish.yml` & `aiosysbus-1.1.7/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.6/.github/workflows/release.yml` & `aiosysbus-1.1.7/.github/workflows/release.yml`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     steps:
       # To use this repository's private action, you must check out the repository
       - name: Checkout
         uses: actions/checkout@v4
 
       - name: Generate changelog
         id: changelog
-        uses: metcalfc/changelog-generator@v4.2.0
+        uses: metcalfc/changelog-generator@v4.3.1
         with:
           mytoken: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Create Release
         id: create_release
         uses: actions/create-release@latest
         env:
```

### Comparing `aiosysbus-1.1.6/.gitignore` & `aiosysbus-1.1.7/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
-example_home.py
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
```

### Comparing `aiosysbus-1.1.6/.pre-commit-config.yaml` & `aiosysbus-1.1.7/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.14
+    rev: v0.4.3
     hooks:
       - id: ruff
         args:
           - --fix
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
@@ -13,22 +13,22 @@
       - id: codespell
         args:
           - --ignore-words-list=fro,hass
           - --skip="./.*,*.csv,*.json,*.ambr"
           - --quiet-level=2
         exclude_types: [csv, json]
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-executables-have-shebangs
         stages: [manual]
       - id: check-json
         exclude: (.vscode|.devcontainer)
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.33.0
+    rev: v1.35.1
     hooks:
       - id: yamllint
         exclude: (.github|.vscode|.devcontainer)
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
@@ -42,12 +42,12 @@
       - id: python-typing-update
         stages: [manual]
         args:
           - --py311-plus
           - --force
           - --keep-updates
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.10.0
     hooks:
       - id: mypy
         args: [--strict, --ignore-missing-imports]
         exclude: ^tests/
```

### Comparing `aiosysbus-1.1.6/LICENSE` & `aiosysbus-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.6/PKG-INFO` & `aiosysbus-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosysbus
-Version: 1.1.6
+Version: 1.1.7
 Summary: Provides asynchronous authentication and access to Livebox
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: livebox,async
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `aiosysbus-1.1.6/README.md` & `aiosysbus-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.6/aiosysbus/__init__.py` & `aiosysbus-1.1.7/aiosysbus/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provides authentication and raw access to Livebox.
 """
+
 from .aiosysbus import AIOSysbus
 from .exceptions import (
     AiosysbusException,
     AuthenticationFailed,
     HttpRequestFailed,
     InsufficientPermissionsError,
     RetrieveFailed,
```

### Comparing `aiosysbus-1.1.6/aiosysbus/aiosysbus.py` & `aiosysbus-1.1.7/aiosysbus/aiosysbus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """API for livebox routeur."""
+
 from __future__ import annotations
 
 import inspect
 import logging
 from typing import Self
 
 from aiohttp import ClientSession
@@ -23,26 +24,28 @@
         username: str,
         password: str,
         session: ClientSession | None = None,
         timeout: int = 120,
         host: str = "192.168.1.1",
         port: int = 80,
         use_tls: bool = False,
+        verify_tls: bool = True,
     ) -> None:
         """Load parameters."""
         self._session = session or ClientSession()
         base_url = yurl.build(
             scheme="https" if use_tls else "http", host=host, port=port, path="/ws"
         )
         self._auth = Auth(
             session=self._session,
             base_url=base_url,
             username=username,
             password=password,
             timeout=timeout,
+            verify_tls=verify_tls,
         )
 
         self._cleanup_session = session is None
         self._authorize = False
 
         # Instantiate Livebox modules
         self._load_modules()
```

### Comparing `aiosysbus-1.1.6/aiosysbus/api/__init__.py` & `aiosysbus-1.1.7/aiosysbus/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.6/aiosysbus/api/call.py` & `aiosysbus-1.1.7/aiosysbus/api/call.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """DECT, VoiceService and Phone book."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ..auth import Auth
```

### Comparing `aiosysbus-1.1.6/aiosysbus/api/device.py` & `aiosysbus-1.1.7/aiosysbus/api/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Devices."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ..auth import Auth
```

### Comparing `aiosysbus-1.1.6/aiosysbus/api/diagnostic.py` & `aiosysbus-1.1.7/aiosysbus/api/diagnostic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Diagnostics and data statistics."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ..auth import Auth
```

### Comparing `aiosysbus-1.1.6/aiosysbus/api/dnsdhcp.py` & `aiosysbus-1.1.7/aiosysbus/api/dnsdhcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Livebox DHCP v4,v6 and Dynamic DNS update."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ..auth import Auth
```

### Comparing `aiosysbus-1.1.6/aiosysbus/api/nemo.py` & `aiosysbus-1.1.7/aiosysbus/api/nemo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """NeMo information."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ..auth import Auth
```

### Comparing `aiosysbus-1.1.6/aiosysbus/api/network.py` & `aiosysbus-1.1.7/aiosysbus/api/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Network settings."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ..auth import Auth
```

### Comparing `aiosysbus-1.1.6/aiosysbus/api/nmc.py` & `aiosysbus-1.1.7/aiosysbus/api/nmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """NMC."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ..auth import Auth
```

### Comparing `aiosysbus-1.1.6/aiosysbus/api/powermgmt.py` & `aiosysbus-1.1.7/aiosysbus/api/powermgmt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Power Management."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ..auth import Auth
```

### Comparing `aiosysbus-1.1.6/aiosysbus/api/schedule.py` & `aiosysbus-1.1.7/aiosysbus/api/schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Scheduler for Internet access."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ..auth import Auth
```

### Comparing `aiosysbus-1.1.6/aiosysbus/api/services.py` & `aiosysbus-1.1.7/aiosysbus/api/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Services and co."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ..auth import Auth
```

### Comparing `aiosysbus-1.1.6/aiosysbus/api/storage.py` & `aiosysbus-1.1.7/aiosysbus/api/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Storage & co."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ..auth import Auth
```

### Comparing `aiosysbus-1.1.6/aiosysbus/api/system.py` & `aiosysbus-1.1.7/aiosysbus/api/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """System information."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ..auth import Auth
```

### Comparing `aiosysbus-1.1.6/aiosysbus/api/user.py` & `aiosysbus-1.1.7/aiosysbus/api/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Users."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from ..auth import Auth
```

### Comparing `aiosysbus-1.1.6/aiosysbus/auth.py` & `aiosysbus-1.1.7/aiosysbus/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """API Access for livebox."""
+
 from __future__ import annotations
 
 import asyncio
 import logging
 import socket
 from typing import Any
 
@@ -46,21 +47,23 @@
     def __init__(
         self,
         session: ClientSession,
         base_url: URL,
         username: str,
         password: str,
         timeout: int,
+        verify_tls: bool,
     ) -> None:
         """Init class."""
         self.session = session
         self.base_url = base_url
         self.username = username
         self.password = password
         self.timeout = timeout
+        self.verify_tls = verify_tls
 
         self.session_token: str | None = None
         self.session_permissions: str | None = None
         self.retry = MAX_RETRY
 
         self._cookies: dict[str, str] = {}
 
@@ -81,15 +84,19 @@
             )
 
         try:
             _LOGGER.debug("METHOD:%s URL:%s", method, self.base_url)
             _LOGGER.debug("DATA:%s", json)
             async with asyncio.timeout(self.timeout):
                 response = await self.session.request(
-                    method, self.base_url, json=json, headers=headers
+                    method,
+                    self.base_url,
+                    json=json,
+                    headers=headers,
+                    verify_ssl=self.verify_tls,
                 )
         except (asyncio.CancelledError, asyncio.TimeoutError) as error:
             raise TimeoutExceededError(
                 "Timeout occurred while connecting to Livebox"
             ) from error
         except (ClientError, socket.gaierror) as error:
             raise HttpRequestFailed(
```

### Comparing `aiosysbus-1.1.6/aiosysbus/exceptions.py` & `aiosysbus-1.1.7/aiosysbus/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.6/aiosysbus.egg-info/PKG-INFO` & `aiosysbus-1.1.7/aiosysbus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosysbus
-Version: 1.1.6
+Version: 1.1.7
 Summary: Provides asynchronous authentication and access to Livebox
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: livebox,async
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `aiosysbus-1.1.6/aiosysbus.egg-info/SOURCES.txt` & `aiosysbus-1.1.7/aiosysbus.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 MANIFEST.in
 README.md
 example.py
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 .github/dependabot.yml
+.github/workflows/auto-approve.yml
 .github/workflows/lint.yml
 .github/workflows/pythonpublish.yml
 .github/workflows/release.yml
 aiosysbus/__init__.py
 aiosysbus/aiosysbus.py
 aiosysbus/auth.py
 aiosysbus/exceptions.py
```

### Comparing `aiosysbus-1.1.6/example.py` & `aiosysbus-1.1.7/example.py`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.6/pyproject.toml` & `aiosysbus-1.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools","setuptools-scm", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "aiosysbus"
-dynamic = ["version"]
+dynamic     = ["version"]
 license     = {text = "GPL-3"}
 description = "Provides asynchronous authentication and access to Livebox"
 readme      = "README.md"
 authors     = [
     {name = "Cyr-ius", email = "cyr-ius@ipocus.net"}
 ]
 keywords    = ["livebox", "async"]
```

### Comparing `aiosysbus-1.1.6/tests/fixtures/deviceinfo.json` & `aiosysbus-1.1.7/tests/fixtures/deviceinfo.json`

 * *Files identical despite different names*

### Comparing `aiosysbus-1.1.6/tests/test_connection.py` & `aiosysbus-1.1.7/tests/test_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests connection."""
+
 from __future__ import annotations
 
 import asyncio
 import logging
 from unittest.mock import AsyncMock, patch
 
 import aiohttp
@@ -39,17 +40,20 @@
 
     return mock
 
 
 @pytest.mark.asyncio
 async def test_challenge_error() -> None:
     """Test connect."""
-    with pytest.raises(
-        AiosysbusException, match="An error occurred while retrieving the challenge"
-    ), patch("aiohttp.ClientSession.request", side_effect=aiohttp.ClientError):
+    with (
+        pytest.raises(
+            AiosysbusException, match="An error occurred while retrieving the challenge"
+        ),
+        patch("aiohttp.ClientSession.request", side_effect=aiohttp.ClientError),
+    ):
         api = AIOSysbus("username", "password")
         await api.async_connect()
 
 
 @pytest.mark.asyncio
 @patch("aiohttp.ClientSession.request", new_callable=create_resp)
 async def test_connect(mock_post) -> None:
@@ -68,62 +72,70 @@
 
 @pytest.mark.asyncio
 @patch("aiohttp.ClientSession.request", new_callable=create_resp)
 async def test_connect_error(mock_post) -> None:
     """Test connect."""
     mock_post.side_effect = aiohttp.ClientError
     api = AIOSysbus("username", "password")
-    with pytest.raises(
-        AiosysbusException, match="Error occurred while communicating with Livebox"
-    ), patch("aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()):
+    with (
+        pytest.raises(
+            AiosysbusException, match="Error occurred while communicating with Livebox"
+        ),
+        patch("aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()),
+    ):
         await api.async_connect()
 
     mock_post.side_effect = asyncio.TimeoutError
     api = AIOSysbus("username", "password")
-    with pytest.raises(
-        AiosysbusException, match="Timeout occurred while connecting to Livebox"
-    ), patch("aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()):
+    with (
+        pytest.raises(
+            AiosysbusException, match="Timeout occurred while connecting to Livebox"
+        ),
+        patch("aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()),
+    ):
         await api.async_connect()
 
 
 @pytest.mark.asyncio
 @patch("aiohttp.ClientSession.request", new_callable=create_resp)
 async def test_get_lan(mock_post) -> None:
     gdr = {"NumberOfReadings": 1, "InterfaceName": ["eth0"]}
 
     mock_post.return_value.json.return_value = {"result": {"lan": "1.2.3.4"}}
 
     api = AIOSysbus("username", "password")
-    with patch(
-        "aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()
-    ), patch(
-        "aiosysbus.auth.Auth.async_get_session_token",
-        return_value=("123456789", "admin"),
+    with (
+        patch("aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()),
+        patch(
+            "aiosysbus.auth.Auth.async_get_session_token",
+            return_value=("123456789", "admin"),
+        ),
     ):
         await api.async_connect()
-        response = await api.homelan.async_get_lan(gdr)
+        response = await api.nmc.async_get_lan_ip(gdr)
 
     assert mock_post.return_value.json.return_value.get("result") == response
 
 
 @pytest.mark.asyncio
 @patch("aiohttp.ClientSession.request", new_callable=create_resp)
 async def test_get_api_without_connect(mock_post) -> None:
     gdr = {"NumberOfReadings": 1, "InterfaceName": ["eth0"]}
 
     mock_post.return_value.json.return_value = {"result": {"lan": "1.2.3.4"}}
 
     api = AIOSysbus("username", "password")
-    with patch(
-        "aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()
-    ), patch(
-        "aiosysbus.auth.Auth.async_get_session_token",
-        return_value=("123456789", "admin"),
+    with (
+        patch("aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()),
+        patch(
+            "aiosysbus.auth.Auth.async_get_session_token",
+            return_value=("123456789", "admin"),
+        ),
     ):
-        response = await api.homelan.async_get_lan(gdr)
+        response = await api.nmc.async_get_lan_ip(gdr)
 
     assert mock_post.return_value.json.return_value.get("result") == response
     assert api._auth.session_token == "123456789"
     assert api._auth.session_permissions == "admin"
 
 
 @pytest.mark.asyncio
@@ -131,40 +143,44 @@
 async def test_error_500(mock_post) -> None:
     """Test connect."""
     data = {"data": {"error": "Server unavailable"}}
 
     mock_post.return_value.status = 500
     mock_post.return_value.json.return_value = data
     api = AIOSysbus("username", "password")
-    with pytest.raises(HttpRequestFailed) as error, patch(
-        "aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()
-    ), patch(
-        "aiosysbus.auth.Auth.async_get_session_token",
-        return_value=("123456789", "admin"),
+    with (
+        pytest.raises(HttpRequestFailed) as error,
+        patch("aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()),
+        patch(
+            "aiosysbus.auth.Auth.async_get_session_token",
+            return_value=("123456789", "admin"),
+        ),
     ):
         await api.async_connect()
-        await api.homelan.async_get_lan()
+        await api.nmc.async_get_lan_ip()
 
     assert error.value.args[0] == data
 
 
 @pytest.mark.asyncio
 @patch("aiohttp.ClientSession.request", new_callable=create_resp)
 async def test_error_contenttype(mock_post) -> None:
     """Test connect."""
     mock_post.return_value.headers = CIMultiDict(
         {("Content-Type", "plain/text"), ("Set-Cookie", "e2c29097/sessid=;")}
     )
 
     api = AIOSysbus("username", "password")
-    with pytest.raises(UnexpectedResponse) as error, patch(
-        "aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()
-    ), patch(
-        "aiosysbus.auth.Auth.async_get_session_token",
-        return_value=("123456789", "admin"),
+    with (
+        pytest.raises(UnexpectedResponse) as error,
+        patch("aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()),
+        patch(
+            "aiosysbus.auth.Auth.async_get_session_token",
+            return_value=("123456789", "admin"),
+        ),
     ):
         await api.async_connect()
         await api.storageservice.async_get_physical_mediums()
 
     assert (
         error.value.args[0]
         == "Unexpected response, content-type incorrect (plain/text)"
@@ -179,36 +195,40 @@
 
     mock_post.return_value.status = 500
     mock_post.return_value.headers = CIMultiDict(
         {("Content-Type", "plain/text"), ("Set-Cookie", "e2c29097/sessid=;")}
     )
     mock_post.return_value.json.return_value = data
     api = AIOSysbus("username", "password")
-    with pytest.raises(HttpRequestFailed) as error, patch(
-        "aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()
-    ), patch(
-        "aiosysbus.auth.Auth.async_get_session_token",
-        return_value=("123456789", "admin"),
+    with (
+        pytest.raises(HttpRequestFailed) as error,
+        patch("aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()),
+        patch(
+            "aiosysbus.auth.Auth.async_get_session_token",
+            return_value=("123456789", "admin"),
+        ),
     ):
         await api.async_connect()
         await api.speedtest.async_get_wan_results()
 
     assert error.value.args[0] == "RAW Text"
 
 
 @pytest.mark.asyncio
 @patch("aiohttp.ClientSession.request", new_callable=create_resp)
 async def test_retry_error(mock_post) -> None:
     """Test connect."""
     data = {"result": {"errors": "Server unavailable"}}
     mock_post.return_value.json.return_value = data
     api = AIOSysbus("username", "password")
-    with pytest.raises(RetrieveFailed) as error, patch(
-        "aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()
-    ), patch(
-        "aiosysbus.auth.Auth.async_get_session_token",
-        return_value=("123456789", "admin"),
+    with (
+        pytest.raises(RetrieveFailed) as error,
+        patch("aiosysbus.auth.Auth._async_get_challenge", return_value=AsyncMock()),
+        patch(
+            "aiosysbus.auth.Auth.async_get_session_token",
+            return_value=("123456789", "admin"),
+        ),
     ):
         await api.async_connect()
         await api.topologydiagnostics.async_get_topodiags()
 
     assert error.value.args[0] == "Server unavailable"
```

