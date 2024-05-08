# Comparing `tmp/adbutils-2.6.0.tar.gz` & `tmp/adbutils-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbutils-2.6.0.tar", last modified: Mon May  6 07:05:42 2024, max compression
+gzip compressed data, was "adbutils-2.6.1.tar", last modified: Wed May  8 14:07:24 2024, max compression
```

## Comparing `adbutils-2.6.0.tar` & `adbutils-2.6.1.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.330343 adbutils-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-06 07:05:34.000000 adbutils-2.6.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.326343 adbutils-2.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-06 07:05:34.000000 adbutils-2.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.326343 adbutils-2.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-06 07:05:34.000000 adbutils-2.6.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-06 07:05:34.000000 adbutils-2.6.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-06 07:05:34.000000 adbutils-2.6.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 07:05:42.000000 adbutils-2.6.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-06 07:05:42.000000 adbutils-2.6.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-06 07:05:34.000000 adbutils-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-06 07:05:42.330343 adbutils-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15054 2024-05-06 07:05:34.000000 adbutils-2.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.326343 adbutils-2.6.0/adbutils/
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    17408 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.326343 adbutils-2.6.0/adbutils/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/binaries/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/binaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/install.py
--rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/pidcat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/screenrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    18032 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-06 07:05:34.000000 adbutils-2.6.0/adbutils/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.326343 adbutils-2.6.0/adbutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-06 07:05:42.000000 adbutils-2.6.0/adbutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-06 07:05:42.000000 adbutils-2.6.0/adbutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:05:42.000000 adbutils-2.6.0/adbutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:05:42.000000 adbutils-2.6.0/adbutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 07:05:42.000000 adbutils-2.6.0/adbutils.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 07:05:42.000000 adbutils-2.6.0/adbutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 07:05:42.000000 adbutils-2.6.0/adbutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.322343 adbutils-2.6.0/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.326343 adbutils-2.6.0/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-05-06 07:05:34.000000 adbutils-2.6.0/assets/images/pidcat.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-05-06 07:05:34.000000 adbutils-2.6.0/build_wheel.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-06 07:05:34.000000 adbutils-2.6.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.330343 adbutils-2.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-06 07:05:34.000000 adbutils-2.6.0/docs/PROTOCOL.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.330343 adbutils-2.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-06 07:05:34.000000 adbutils-2.6.0/examples/reset-offline.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 07:05:34.000000 adbutils-2.6.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-06 07:05:34.000000 adbutils-2.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-06 07:05:42.330343 adbutils-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-06 07:05:34.000000 adbutils-2.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.330343 adbutils-2.6.0/test_real_device/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/test_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/test_forward_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/test_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-06 07:05:34.000000 adbutils-2.6.0/test_real_device/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:05:42.330343 adbutils-2.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-06 07:05:34.000000 adbutils-2.6.0/tests/adb_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-06 07:05:34.000000 adbutils-2.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-06 07:05:34.000000 adbutils-2.6.0/tests/test_adb_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:05:34.000000 adbutils-2.6.0/tests/test_adb_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:07:24.672864 adbutils-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-08 14:07:15.000000 adbutils-2.6.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:07:24.668864 adbutils-2.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 14:07:15.000000 adbutils-2.6.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:07:24.668864 adbutils-2.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-08 14:07:15.000000 adbutils-2.6.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-08 14:07:15.000000 adbutils-2.6.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-08 14:07:15.000000 adbutils-2.6.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-08 14:07:24.000000 adbutils-2.6.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-08 14:07:24.000000 adbutils-2.6.1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-08 14:07:15.000000 adbutils-2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-08 14:07:24.672864 adbutils-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15054 2024-05-08 14:07:15.000000 adbutils-2.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:07:24.668864 adbutils-2.6.1/adbutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12816 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17342 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:07:24.668864 adbutils-2.6.1/adbutils/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/binaries/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/binaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/pidcat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/screenrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18032 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-08 14:07:15.000000 adbutils-2.6.1/adbutils/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:07:24.668864 adbutils-2.6.1/adbutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-08 14:07:24.000000 adbutils-2.6.1/adbutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-08 14:07:24.000000 adbutils-2.6.1/adbutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:07:24.000000 adbutils-2.6.1/adbutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:07:24.000000 adbutils-2.6.1/adbutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 14:07:24.000000 adbutils-2.6.1/adbutils.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 14:07:24.000000 adbutils-2.6.1/adbutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 14:07:24.000000 adbutils-2.6.1/adbutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:07:24.664863 adbutils-2.6.1/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:07:24.668864 adbutils-2.6.1/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-05-08 14:07:15.000000 adbutils-2.6.1/assets/images/pidcat.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-05-08 14:07:15.000000 adbutils-2.6.1/build_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 14:07:15.000000 adbutils-2.6.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:07:24.668864 adbutils-2.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-08 14:07:15.000000 adbutils-2.6.1/docs/PROTOCOL.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:07:24.672864 adbutils-2.6.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-08 14:07:15.000000 adbutils-2.6.1/examples/reset-offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 14:07:15.000000 adbutils-2.6.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 14:07:15.000000 adbutils-2.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-08 14:07:24.672864 adbutils-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-08 14:07:15.000000 adbutils-2.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:07:24.672864 adbutils-2.6.1/test_real_device/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-08 14:07:15.000000 adbutils-2.6.1/test_real_device/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-08 14:07:15.000000 adbutils-2.6.1/test_real_device/test_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-08 14:07:15.000000 adbutils-2.6.1/test_real_device/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-08 14:07:15.000000 adbutils-2.6.1/test_real_device/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-08 14:07:15.000000 adbutils-2.6.1/test_real_device/test_forward_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-08 14:07:15.000000 adbutils-2.6.1/test_real_device/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-08 14:07:15.000000 adbutils-2.6.1/test_real_device/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-08 14:07:15.000000 adbutils-2.6.1/test_real_device/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:07:24.672864 adbutils-2.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-08 14:07:15.000000 adbutils-2.6.1/tests/adb_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-08 14:07:15.000000 adbutils-2.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-08 14:07:15.000000 adbutils-2.6.1/tests/test_adb_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-08 14:07:15.000000 adbutils-2.6.1/tests/test_adb_shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-08 14:07:15.000000 adbutils-2.6.1/tests/test_forward.py
```

### Comparing `adbutils-2.6.0/.coveragerc` & `adbutils-2.6.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/.github/workflows/main.yml` & `adbutils-2.6.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/.github/workflows/publish-to-pypi.yml` & `adbutils-2.6.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/.travis.yml` & `adbutils-2.6.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/LICENSE` & `adbutils-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/PKG-INFO` & `adbutils-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.6.0
+Version: 2.6.1
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.6.0/README.md` & `adbutils-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/adbutils/__init__.py` & `adbutils-2.6.1/adbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/adbutils/__main__.py` & `adbutils-2.6.1/adbutils/__main__.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/adbutils/_adb.py` & `adbutils-2.6.1/adbutils/_adb.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from __future__ import annotations
 
 import os
 import socket
 import subprocess
 import typing
 import weakref
-from typing import Iterator, Union
+from typing import Iterator, List, Union
 
 from deprecation import deprecated
 
 from adbutils._utils import adb_path
 from adbutils.errors import AdbConnectionError, AdbError, AdbTimeout
 
 from adbutils._proto import *
@@ -320,33 +320,31 @@
 
     def _diff_devices(self, orig: typing.List[DeviceEvent], curr: typing.List[DeviceEvent]):
         for d in set(orig).difference(curr):
             yield DeviceEvent(False, d.serial, 'absent')
         for d in set(curr).difference(orig):
             yield DeviceEvent(True, d.serial, d.status)
 
-    @deprecated(deprecated_in="0.15.0",
-                removed_in="1.0.0",
-                details="use device.forward_list instead",
-                current_version=__version__)
-    def forward_list(self, serial: Union[None, str] = None):
+    def forward_list(self, serial: Union[None, str] = None) -> List[ForwardItem]:
         with self.make_connection() as c:
             list_cmd = "host:list-forward"
             if serial:
                 list_cmd = "host-serial:{}:list-forward".format(serial)
             c.send_command(list_cmd)
             c.check_okay()
             content = c.read_string_block()
+            items = []
             for line in content.splitlines():
                 parts = line.split()
                 if len(parts) != 3:
                     continue
                 if serial and parts[0] != serial:
                     continue
-                yield ForwardItem(*parts)
+                items.append(ForwardItem(*parts))
+            return items
 
     @deprecated(deprecated_in="0.15.0",
                 removed_in="1.0.0",
                 details="use Device.forward instead",
                 current_version=__version__)
     def forward(self, serial, local, remote, norebind=False):
         """
@@ -387,22 +385,24 @@
             c.send_command(":".join(cmds))
             c.check_okay()
 
     @deprecated(deprecated_in="0.15.0",
                 removed_in="1.0.0",
                 details="use Device.reverse_list instead",
                 current_version=__version__)
-    def reverse_list(self, serial: Union[None, str] = None):
+    def reverse_list(self, serial: str) -> List[ReverseItem]:
         with self.make_connection() as c:
             c.send_command("host:transport:" + serial)
             c.check_okay()
             c.send_command("reverse:list-forward")
             c.check_okay()
             content = c.read_string_block()
+            items = []
             for line in content.splitlines():
                 parts = line.split()
                 if len(parts) != 3:
                     continue
-                yield ReverseItem(*parts[1:])
+                items.append(ReverseItem(*parts[1:]))
+            return items
```

### Comparing `adbutils-2.6.0/adbutils/_deprecated.py` & `adbutils-2.6.1/adbutils/_deprecated.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/adbutils/_device.py` & `adbutils-2.6.1/adbutils/_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import socket
 import subprocess
 import threading
 import typing
 from typing import List, Optional, Union
 
 from PIL import Image, UnidentifiedImageError
+from deprecation import deprecated
 
 from adbutils._deprecated import DeprecatedExtension
 from adbutils.install import InstallExtension
 from adbutils.screenrecord import ScreenrecordExtension
 from adbutils.screenshot import ScreenshotExtesion
 
 from adbutils._adb import AdbConnection, BaseClient
@@ -62,17 +63,15 @@
     def serial(self) -> str:
         return self._serial
 
     def open_transport(
         self, command: str = None, timeout: float = _DEFAULT_SOCKET_TIMEOUT
     ) -> AdbConnection:
         # connect has it own timeout
-        c = self._client.make_connection()
-        if timeout:
-            c.conn.settimeout(timeout)
+        c = self._client.make_connection(timeout=timeout)
 
         if command:
             if self._transport_id:
                 c.send_command(f"host-transport-id:{self._transport_id}:{command}")
                 c.check_okay()
             elif self._serial:
                 c.send_command(f"host-serial:{self._serial}:{command}")
@@ -260,23 +259,16 @@
             ):  # yapf: disable
                 return int(f.local[len("tcp:") :])
         local_port = get_free_port()
         self.forward("tcp:" + str(local_port), remote)
         return local_port
 
     def forward_list(self) -> List[ForwardItem]:
-        c = self.open_transport("list-forward")
-        content = c.read_string_block()
-        items = []
-        for line in content.splitlines():
-            parts = line.split()
-            if len(parts) != 3:
-                continue
-            items.append(ForwardItem(*parts))
-        return items
+        items = self._client.forward_list()
+        return [item for item in items if item.serial == self._serial]
 
     def reverse(self, remote: str, local: str, norebind: bool = False):
         """
         Args:
             serial (str): device serial
             remote, local (str):
                 - tcp:<port>
@@ -353,16 +345,18 @@
             raise NotImplementedError("Unsupported color format")
         buffer = c.read(size)
         if len(buffer) != size:
             raise UnidentifiedImageError("framebuffer size not match", size, len(buffer))
         image = Image.frombytes(color_format, (width, height), buffer)
         return image
 
-    def push(self, local: str, remote: str) -> str:
-        return self.adb_output("push", local, remote)
+    @deprecated(deprecated_in="2.6.0", removed_in="3.0.0", current_version=__version__, details="use sync.push instead")
+    def push(self, local: str, remote: str):
+        """ alias for sync.push """
+        self.sync.push(local, remote)
 
     def create_connection(
         self, network: Network, address: Union[int, str]
     ) -> socket.socket:
         """
         Used to connect a socket (unix of tcp) on the device
```

### Comparing `adbutils-2.6.0/adbutils/_proto.py` & `adbutils-2.6.1/adbutils/_proto.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/adbutils/_utils.py` & `adbutils-2.6.1/adbutils/_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/adbutils/errors.py` & `adbutils-2.6.1/adbutils/errors.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/adbutils/install.py` & `adbutils-2.6.1/adbutils/install.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/adbutils/pidcat.py` & `adbutils-2.6.1/adbutils/pidcat.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/adbutils/screenrecord.py` & `adbutils-2.6.1/adbutils/screenrecord.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/adbutils/screenshot.py` & `adbutils-2.6.1/adbutils/screenshot.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/adbutils/shell.py` & `adbutils-2.6.1/adbutils/shell.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/adbutils/sync.py` & `adbutils-2.6.1/adbutils/sync.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/adbutils.egg-info/PKG-INFO` & `adbutils-2.6.1/adbutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.6.0
+Version: 2.6.1
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.6.0/adbutils.egg-info/SOURCES.txt` & `adbutils-2.6.1/adbutils.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -47,8 +47,9 @@
 test_real_device/test_forward_reverse.py
 test_real_device/test_import.py
 test_real_device/test_record.py
 test_real_device/test_utils.py
 tests/adb_server.py
 tests/conftest.py
 tests/test_adb_server.py
-tests/test_adb_shell.py
+tests/test_adb_shell.py
+tests/test_forward.py
```

### Comparing `adbutils-2.6.0/assets/images/pidcat.png` & `adbutils-2.6.1/assets/images/pidcat.png`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/build_wheel.py` & `adbutils-2.6.1/build_wheel.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/docs/PROTOCOL.md` & `adbutils-2.6.1/docs/PROTOCOL.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+# ADB Protocol
+Tested with adb 1.0.41, Capture data with Charles
+
+Charles settings
+
+Proxy->Port Forwarding
+
+```
+TCP Local(5555) -> Remote(localhost:5037)
+```
+
+execute adb command, e.g. `adb -P 5555 devices`, now data should be seen in charles.
+
 ## host version
 ```
 >send
 000chost:version
 
 <recv
 00000000  4f 4b 41 59 30 30 30 34 30 30 32 39               OKAY00040029    
@@ -14,50 +27,75 @@
 
 <recv
 00000000  46 41 49 4c 30 30 32 37 64 65 76 69 63 65 20 27   FAIL0027device '
 00000010  47 42 47 35 54 31 39 37 31 31 30 30 32 37 36 39   GBG5T19711002769
 00000020  30 30 31 34 27 20 6e 6f 74 20 66 6f 75 6e 64      0014' not found 
 ```
 
-## reverse --list
+## forward
+```
+$ adb forward --list
+>send
+0011host:list-forward
+
+<recv
+OKAY0020emulator-5554 tcp:5678 tcp:8765
+
+$ adb forward --remove-all
+>send
+000ehost:tport:any0014host:killforward-all
+
+<recv
+00000000  4f 4b 41 59 08 00 00 00 00 00 00 00 4f 4b 41 59   OKAY        OKAY
+00000010  4f 4b 41 59                                       OKAY            
+
+$ adb -s emulator-5554 forward tcp:1234 tcp:4321
+>send
+001fhost:tport:serial:emulator-5554001ehost:forward:tcp:1234;tcp:4321
+
+<recv
+00000000  4f 4b 41 59 08 00 00 00 00 00 00 00 4f 4b 41 59   OKAY        OKAY
+00000010  4f 4b 41 59 30 30 30 34 31 32 33 34               OKAY00041234    
+```
+
+## reverse
 adb help
 ```
 reverse --list           list all reverse socket connections from device
  reverse [--no-rebind] REMOTE LOCAL
      reverse socket connection using:
        tcp:<port> (<remote> may be "tcp:0" to pick any open port)
        localabstract:<unix domain socket name>
        localreserved:<unix domain socket name>
        localfilesystem:<unix domain socket name>
  reverse --remove REMOTE  remove specific reverse socket connection
  reverse --remove-all     remove all reverse socket connections from device
 ```
 
 ```
+$ adb reverse --list
 >send
 0022host:tport:serial:GBG5T197110027690014
 
 <recv
 00000000  4f 4b 41 59 06 00 00 00 00 00 00 00               OKAY        
-```
 
-```
 >send
 reverse:list-forward
 
 <recv
 00000000  4f 4b 41 59                                       OKAY
 00000010  30 30 33 63 75 73 62 20 6c 6f 63 61 6c 61 62 73   003cusb localabs
 00000020  74 72 61 63 74 3a 67 6e 69 72 65 68 74 65 74 20   tract:gnirehtet 
 00000030  74 63 70 3a 33 31 34 31 36 0a 75 73 62 20 74 63   tcp:31416 usb tc
 00000040  70 3a 35 31 32 33 20 74 63 70 3a 37 38 39 30 0a   p:5123 tcp:7890 
 ```
 
-## adb -s GBG5T197110027690014 reverse localabstract:test tcp:12345
 ```
+$ adb -s GBG5T197110027690014 reverse localabstract:test tcp:12345
 >send
 001fhost:tport:serial:emulator-5554002creverse:forward:localabstract:test;tcp:12345
 
 <recv
 00000000  4f 4b 41 59 03 00 00 00 00 00 00 00 4f 4b 41 59   OKAY        OKAY
 00000010  4f 4b 41 59                                       OKAY            
 ```
```

### Comparing `adbutils-2.6.0/examples/reset-offline.py` & `adbutils-2.6.1/examples/reset-offline.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/setup.cfg` & `adbutils-2.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/test_real_device/conftest.py` & `adbutils-2.6.1/test_real_device/conftest.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/test_real_device/test_adb.py` & `adbutils-2.6.1/test_real_device/test_adb.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/test_real_device/test_deprecated.py` & `adbutils-2.6.1/test_real_device/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/test_real_device/test_device.py` & `adbutils-2.6.1/test_real_device/test_device.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/test_real_device/test_forward_reverse.py` & `adbutils-2.6.1/test_real_device/test_forward_reverse.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/test_real_device/test_utils.py` & `adbutils-2.6.1/test_real_device/test_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/tests/adb_server.py` & `adbutils-2.6.1/tests/adb_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,19 +90,24 @@
 @register_command("host:kill")
 async def host_kill(ctx: Context):
     await ctx.send(b"OKAY")
     await ctx.close()
     await ctx.server.stop()
     # os.kill(os.getpid(), signal.SIGINT)
 
+@register_command("host:list-forward")
+async def host_list_forward(ctx: Context):
+    await ctx.send(b"OKAY")
+    await ctx.send(encode_string("123456 tcp:1234 tcp:4321"))
+
+
 SHELL_OUTPUTS = {
     "pwd": "/",
 }
 
-
 @register_command(re.compile("host:tport:serial:.*"))
 async def host_tport_serial(ctx: Context):
     serial = ctx.command.split(":")[-1]
     if serial == "not-found":
         await ctx.send(b"FAIL")
         await ctx.send(encode("device not found"))
     else:
```

### Comparing `adbutils-2.6.0/tests/conftest.py` & `adbutils-2.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/tests/test_adb_server.py` & `adbutils-2.6.1/tests/test_adb_server.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.0/tests/test_adb_shell.py` & `adbutils-2.6.1/tests/test_adb_shell.py`

 * *Files identical despite different names*

