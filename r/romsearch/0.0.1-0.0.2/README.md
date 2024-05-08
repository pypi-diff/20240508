# Comparing `tmp/romsearch-0.0.1.tar.gz` & `tmp/romsearch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romsearch-0.0.1.tar", last modified: Mon May  6 15:10:54 2024, max compression
+gzip compressed data, was "romsearch-0.0.2.tar", last modified: Tue May  7 15:35:35 2024, max compression
```

## Comparing `romsearch-0.0.1.tar` & `romsearch-0.0.2.tar`

### file list

```diff
@@ -1,88 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:10:54.028268 romsearch-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:10:54.016269 romsearch-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:10:54.020269 romsearch-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-06 15:10:45.000000 romsearch-0.0.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-06 15:10:45.000000 romsearch-0.0.1/.github/ISSUE_TEMPLATE/console_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-06 15:10:45.000000 romsearch-0.0.1/.github/ISSUE_TEMPLATE/feature_request.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:10:54.020269 romsearch-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-06 15:10:45.000000 romsearch-0.0.1/.github/workflows/build_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-06 15:10:45.000000 romsearch-0.0.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-06 15:10:45.000000 romsearch-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-06 15:10:45.000000 romsearch-0.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-06 15:10:45.000000 romsearch-0.0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 15:10:45.000000 romsearch-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-06 15:10:45.000000 romsearch-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43659 2024-05-06 15:10:54.028268 romsearch-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-06 15:10:45.000000 romsearch-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:10:54.020269 romsearch-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/1g1r.rst
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:10:54.024268 romsearch-0.0.1/docs/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/configs/clonelists.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/configs/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/configs/dats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/configs/defaults.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/configs/platforms.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/configs/regex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/known_issues.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:10:54.024268 romsearch-0.0.1/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/modules/datparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/modules/dupeparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/modules/gamefinder.rst
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/modules/romchooser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/modules/romdownloader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/modules/rommover.rst
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/modules/romparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/modules/romsearch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/reference_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 15:10:45.000000 romsearch-0.0.1/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-06 15:10:45.000000 romsearch-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:10:54.024268 romsearch-0.0.1/romsearch/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:10:54.024268 romsearch-0.0.1/romsearch/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:10:54.024268 romsearch-0.0.1/romsearch/configs/clonelists/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/configs/clonelists/retool.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:10:54.024268 romsearch-0.0.1/romsearch/configs/dats/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/configs/dats/no-intro.yml
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/configs/dats/redump.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/configs/defaults.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:10:54.028268 romsearch-0.0.1/romsearch/configs/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/configs/platforms/Nintendo - GameCube.yml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/configs/platforms/Nintendo - Super Nintendo Entertainment System.yml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/configs/platforms/Sony - PlayStation 2.yml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/configs/platforms/Sony - PlayStation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/configs/regex.yml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/configs/sample_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:10:54.028268 romsearch-0.0.1/romsearch/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/modules/datparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9733 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/modules/dupeparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/modules/gamefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15419 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/modules/romchooser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/modules/romdownloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/modules/rommover.py
--rw-r--r--   0 runner    (1001) docker     (127)    12943 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/modules/romparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/modules/romsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:10:54.028268 romsearch-0.0.1/romsearch/util/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/util/discord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/util/general.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/util/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-06 15:10:45.000000 romsearch-0.0.1/romsearch/util/regex_matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:10:54.028268 romsearch-0.0.1/romsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43659 2024-05-06 15:10:53.000000 romsearch-0.0.1/romsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-06 15:10:54.000000 romsearch-0.0.1/romsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:10:53.000000 romsearch-0.0.1/romsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 15:10:53.000000 romsearch-0.0.1/romsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 15:10:53.000000 romsearch-0.0.1/romsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:10:54.028268 romsearch-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.695399 romsearch-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.679399 romsearch-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.683399 romsearch-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-07 15:35:31.000000 romsearch-0.0.2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-07 15:35:31.000000 romsearch-0.0.2/.github/ISSUE_TEMPLATE/console_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-07 15:35:31.000000 romsearch-0.0.2/.github/ISSUE_TEMPLATE/feature_request.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.683399 romsearch-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-07 15:35:31.000000 romsearch-0.0.2/.github/workflows/build_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-07 15:35:31.000000 romsearch-0.0.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-07 15:35:31.000000 romsearch-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-07 15:35:31.000000 romsearch-0.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-07 15:35:31.000000 romsearch-0.0.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 15:35:31.000000 romsearch-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-07 15:35:31.000000 romsearch-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43659 2024-05-07 15:35:35.695399 romsearch-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-07 15:35:31.000000 romsearch-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.687399 romsearch-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/1g1r.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.687399 romsearch-0.0.2/docs/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configs/clonelists.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configs/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configs/dats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configs/defaults.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configs/platforms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configs/regex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/known_issues.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.687399 romsearch-0.0.2/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/datparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/dupeparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/gamefinder.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/romchooser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/romdownloader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/rommover.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/romparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/romsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/reference_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-07 15:35:31.000000 romsearch-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.687399 romsearch-0.0.2/romsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.691399 romsearch-0.0.2/romsearch/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.691399 romsearch-0.0.2/romsearch/configs/clonelists/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/clonelists/retool.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.691399 romsearch-0.0.2/romsearch/configs/dats/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/dats/no-intro.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/dats/redump.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/defaults.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.691399 romsearch-0.0.2/romsearch/configs/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/platforms/Nintendo - GameCube.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/platforms/Nintendo - Nintendo Entertainment System.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/platforms/Nintendo - Super Nintendo Entertainment System.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/platforms/Sony - PlayStation 2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/platforms/Sony - PlayStation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/regex.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/sample_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.691399 romsearch-0.0.2/romsearch/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/dev/parsing_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.695399 romsearch-0.0.2/romsearch/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/datparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/dupeparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/gamefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15816 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/romchooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/romdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/rommover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/romparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/romsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.695399 romsearch-0.0.2/romsearch/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/util/discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/util/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/util/regex_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.695399 romsearch-0.0.2/romsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43659 2024-05-07 15:35:35.000000 romsearch-0.0.2/romsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-07 15:35:35.000000 romsearch-0.0.2/romsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:35:35.000000 romsearch-0.0.2/romsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 15:35:35.000000 romsearch-0.0.2/romsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 15:35:35.000000 romsearch-0.0.2/romsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:35:35.695399 romsearch-0.0.2/setup.cfg
```

### Comparing `romsearch-0.0.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `romsearch-0.0.2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/.github/ISSUE_TEMPLATE/feature_request.yml` & `romsearch-0.0.2/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/.github/workflows/build_test.yaml` & `romsearch-0.0.2/.github/workflows/build_test.yaml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/.github/workflows/publish.yaml` & `romsearch-0.0.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/.gitignore` & `romsearch-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/.readthedocs.yaml` & `romsearch-0.0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/LICENSE` & `romsearch-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/PKG-INFO` & `romsearch-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romsearch
-Version: 0.0.1
+Version: 0.0.2
 Summary: One Stop ROM Shop
 Author: bbtufty
 Maintainer: bbtufty
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `romsearch-0.0.1/README.md` & `romsearch-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/docs/1g1r.rst` & `romsearch-0.0.2/docs/1g1r.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/docs/Makefile` & `romsearch-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/docs/conf.py` & `romsearch-0.0.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'romsearch'
 copyright = '2024, bbtufty'
 author = 'bbtufty'
-release = '0.0.1'
+release = '0.0.2'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc',
               'sphinx.ext.coverage',
               'sphinx.ext.napoleon',
```

### Comparing `romsearch-0.0.1/docs/configs/config.rst` & `romsearch-0.0.2/docs/configs/config.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/docs/configs/dats.rst` & `romsearch-0.0.2/docs/configs/dats.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/docs/configs/platforms.rst` & `romsearch-0.0.2/docs/configs/platforms.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/docs/configs/regex.rst` & `romsearch-0.0.2/docs/configs/regex.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/docs/configuration.rst` & `romsearch-0.0.2/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/docs/index.rst` & `romsearch-0.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/docs/intro.rst` & `romsearch-0.0.2/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/docs/make.bat` & `romsearch-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/docs/modules/datparser.rst` & `romsearch-0.0.2/docs/modules/datparser.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/docs/modules/dupeparser.rst` & `romsearch-0.0.2/docs/modules/dupeparser.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/docs/modules/romdownloader.rst` & `romsearch-0.0.2/docs/modules/romdownloader.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/pyproject.toml` & `romsearch-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "romsearch"
-version = "0.0.1"
+version = "0.0.2"
 description = "One Stop ROM Shop"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 
 authors = [
     {name = "bbtufty"},
```

### Comparing `romsearch-0.0.1/romsearch/__init__.py` & `romsearch-0.0.2/romsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/romsearch/configs/defaults.yml` & `romsearch-0.0.2/romsearch/configs/defaults.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,86 @@
 default_region: "USA"
 default_language: "En"
 
 datetime_format: "%Y/%m/%d, %H:%M:%S"
 
 platforms:
   - "Nintendo - GameCube"
+  - "Nintendo - Nintendo Entertainment System"
   - "Nintendo - Super Nintendo Entertainment System"
   - "Sony - PlayStation"
   - "Sony - PlayStation 2"
 
 video_types:
   - "NTSC"
   - "PAL"
   - "PAL 60Hz"
   - "MPAL"
   - "SECAM"
 
 regions:
-  - "USA"
-  - "World"
-  - "Canada"
-  - "Europe"
-  - "UK"
-  - "Australia"
-  - "New Zealand"
-  - "Singapore"
-  - "Ireland"
-  - "Japan"
-  - "Asia"
-  - "Thailand"
-  - "Spain"
-  - "Mexico"
-  - "Argentina"
-  - "Latin America"
-  - "Brazil"
-  - "Portugal"
-  - "France"
-  - "Belgium"
-  - "Netherlands"
-  - "Germany"
-  - "Austria"
-  - "Italy"
-  - "Switzerland"
-  - "Hong Kong"
-  - "China"
-  - "Taiwan"
-  - "Korea"
-  - "Russia"
-  - "Ukraine"
-  - "Estonia"
-  - "Poland"
-  - "Latvia"
-  - "Lithuania"
-  - "Denmark"
-  - "Norway"
-  - "Sweden"
-  - "Scandinavia"
-  - "Finland"
-  - "Iceland"
-  - "Hungary"
-  - "Czech"
-  - "Greece"
-  - "Macedonia"
-  - "India"
-  - "South Africa"
-  - "Israel"
-  - "Slovakia"
-  - "Turkey"
-  - "Croatia"
-  - "Slovenia"
-  - "United Arab Emirates"
-  - "Bulgaria"
-  - "Romania"
-  - "Albania"
-  - "Serbia"
-  - "Indonesia"
-  - "Unknown"
+  USA: "USA"
+  World: "World"
+  Canada: "Canada"
+  Europe: "Europe"
+  UK: "UK|United Kingdom"
+  Australia: "Australia"
+  New Zealand: "New Zealand"
+  Singapore: "Singapore"
+  Ireland: "Ireland"
+  Japan: "Japan"
+  Asia: "Asia"
+  Thailand: "Thailand"
+  Spain: "Spain"
+  Mexico: "Mexico"
+  Argentina: "Argentina"
+  Latin America: "Latin America"
+  Brazil: "Brazil"
+  Portugal: "Portugal"
+  France: "France"
+  Belgium: "Belgium"
+  Netherlands: "Netherlands"
+  Germany: "Germany"
+  Austria: "Austria"
+  Italy: "Italy"
+  Switzerland: "Switzerland"
+  Hong Kong: "Hong Kong"
+  China: "China"
+  Taiwan: "Taiwan"
+  Korea: "Korea"
+  Russia: "Russia"
+  Ukraine: "Ukraine"
+  Estonia: "Estonia"
+  Poland: "Poland"
+  Latvia: "Latvia"
+  Lithuania: "Lithuania"
+  Denmark: "Denmark"
+  Norway: "Norway"
+  Sweden: "Sweden"
+  Scandinavia: "Scandinavia"
+  Finland: "Finland"
+  Iceland: "Iceland"
+  Hungary: "Hungary"
+  Czech: "Czech"
+  Greece: "Greece"
+  Macedonia: "Macedonia"
+  India: "India"
+  South Africa: "South Africa"
+  Israel: "Israel"
+  Slovakia: "Slovakia"
+  Turkey: "Turkey"
+  Croatia: "Croatia"
+  Slovenia: "Slovenia"
+  United Arab Emirates: "United Arab Emirates"
+  Bulgaria: "Bulgaria"
+  Romania: "Romania"
+  Albania: "Albania"
+  Serbia: "Serbia"
+  Indonesia: "Indonesia"
+  Unknown: "Unknown"
 
 languages:
   English: "En(?:-[A-Z][A-Z])?"
   Afrikaans: "Af"
   Albanian: "Sq"
   Arabic: "Ar"
   Basque: "Eu"
```

### Comparing `romsearch-0.0.1/romsearch/configs/regex.yml` & `romsearch-0.0.2/romsearch/configs/regex.yml`

 * *Files 17% similar despite different names*

```diff
@@ -53,14 +53,19 @@
   pattern: "\\(@barai\\)"
   group: "demos"
 
 demo:
   pattern: "\\((?:\\w[-.]?\\s*)*Demo(?:(?:,?\\s|-)[\\w0-9\\.]*)*\\)"
   group: "demos"
 
+kiosk:
+  pattern: "\\((?:\\w-?\\s*)*?Kiosk,?(?:\\s\\w*?)*\\)|Kiosk Demo Disc|(PSP System|PS2) Kiosk"
+  group: "demos"
+  search_tags: false
+
 preview:
   pattern: "\\(Preview\\)"
   group: "demos"
 
 sample:
   pattern: "\\(Sample(?:\\s[0-9]*|\\s\\d{4}-\\d{2}-\\d{2})?\\)"
   group: "demos"
@@ -111,15 +116,15 @@
 
 # PROMOTIONAL
 promo:
   pattern: "EPK|Press Kit|\\(Promo\\)"
   group: "promotional"
   search_tags: false
 
-# VERSIONS
+# VERSIONS AND REVISIONS
 version_no:
   pattern: "\\(v[\\.0-9].*?\\)"
   type: "str"
   group: "version"
 
 long_version:
   pattern: "(?!Version Vol\\.|Version \\(|Version$|Version -|Version \\d-)(?: - )?\\(?(?:\\((?:\\w[\\.\\-]?\\s*)*|)[Vv]ers(?:ion|ao)\\s?(?:[\\d\\.\\-]+)+[A-Za-z]?(?: (?:\\d-?)+)?.*?(?:(?:\\w[\\.\\-]?\\s*)*\\))?"
@@ -129,15 +134,14 @@
   group: "version"
 
 revision:
   pattern: "\\(R[eE][vV](?:[ -][0-9A-Z].*?)?\\)"
   type: "str"
   transform_pattern: "R[eE][vV][ -]([0-9A-Z].*?)?"
   transform_repl: "v\\1"
-  group: "version"
 
 # UNLICENSED
 aftermarket:
   pattern: "\\(Aftermarket\\)"
   group: "unlicensed"
 
 homebrew:
@@ -149,14 +153,22 @@
   group: "pirate"
 
 unl:
   pattern: "\\(Unl\\)"
   group: "unlicensed"
 
 # IMPROVED VERSIONS
+c_and_e:
+  pattern: "\\(C&E\\)"
+  group: "improved_version"
+
+cart_present:
+  pattern: "\\(Cart Present\\)"
+  group: "improved_version"
+
 controller_set:
   pattern: "\\(Controller Set\\)"
   group: "improved_version"
 
 culture_publishers:
   pattern: "\\(Culture Publishers\\)"
 
@@ -168,30 +180,69 @@
   pattern: "\\(EDC\\)"
   group: "improved_version"
 
 enhanced:
   pattern: "\\(Enhanced\\)"
   group: "improved_version"
 
+e_reader_edition:
+  pattern: "\\(e-Reader Edition\\)"
+
 gentei:
   pattern: "\\((?:(?!\\(|Gentei.*?)[\\s\\S])*Gentei.*?\\)"
   group: "improved_version"
 
+ideatek:
+  pattern: "\\(Idea-Tek\\)"
+  group: "improved_version"
+
+later:
+  pattern: "\\(Later\\)"
+  group: "improved_version"
+
+mega_soft:
+  pattern: "\\(Mega Soft\\)"
+  group: "improved_version"
+
+nina_03:
+  pattern: "\\(NINA-03\\)"
+  group: "improved_version"
+
+nina_06:
+  pattern: "\\(NINA-06\\)"
+  group: "improved_version"
+
 np:
   pattern: "\\(NP\\)"
   group: "improved_version"
 
 psone_books:
   pattern: "\\(PSone Books\\)"
   group: "improved_version"
 
 renkaban:
   pattern: "\\(Renkaban\\)"
   group: "improved_version"
 
+sachen:
+  pattern: "\\(Sachen\\)"
+  group: "improved_version"
+
+subor_keyboard:
+  pattern: "\\(Subor Keyboard\\)"
+  group: "improved_version"
+
+super_mega:
+  pattern: "\\(Super Mega\\)"
+  group: "improved_version"
+
+txc:
+  pattern: "\\(TXC\\)"
+  group: "improved_version"
+
 # BUDGET EDITIONS
 
 artdink:
   pattern: "\\(Artdink Best Choice\\)"
   group: "budget_edition"
 
 best_of_the_best:
@@ -248,26 +299,34 @@
 
 value_1500:
   pattern: "\\(Value 1500\\)"
   group: "budget_edition"
 
 # MODERN VERSIONS
 
+3ds_virtual_console:
+  pattern: "\\((?:\\w*?,?\\s)*3DS Virtual Console(?:,?\\s\\w*?)*\\)"
+  group: "modern_version"
+
 battle_net:
   pattern: "\\(Battle\\.net\\)"
   group: "modern_version"
 
 castlevania_anniversary:
   pattern: "\\(Castlevania Anniversary Collection\\)"
   group: "modern_version"
 
 castlevania_advance:
   pattern: "\\(Castlevania Advance Collection\\)"
   group: "modern_version"
 
+capcom_classics_mini_mix:
+  pattern: "\\(Capcom Classics Mini Mix\\)"
+  group: "modern_version"
+
 capcom_town:
   pattern: "\\(Capcom Town\\)"
   group: "modern_version"
 
 collection_of_mana:
   pattern: "\\(Collection of Mana\\)"
   group: "modern_version"
@@ -296,26 +355,58 @@
   pattern: "\\(Disney Classic Games\\)"
   group: "modern_version"
 
 gamecube:
   pattern: "\\(Game[Cc]ube.*?\\)"
   group: "modern_version"
 
+iam8bit:
+  pattern: "\\(iam8bit\\)"
+  group: "modern_version"
+
+konami_collector_series:
+  pattern: "\\(Konami Collector's Series\\)"
+  group: "modern_version"
+
 mega_man_x_legacy:
   pattern: "\\(Mega Man X Legacy Collection\\)"
   group: "modern_version"
 
+namco_anthology_1:
+  pattern: "\\(Namco Anthology 1.*?\\)"
+  group: "modern_version"
+
+namco_anthology_2:
+  pattern: "\\(Namco Anthology 2.*?\\)"
+  group: "modern_version"
+
+namcot_collection:
+  pattern: "\\(Namcot Collection.*?\\)"
+  group: "modern_version"
+
+namco_museum_archives:
+  pattern: "\\(Namco Museum Archives Vol [0-9]\\)"
+  group: "modern_version"
+
 qubyte_classic:
   pattern: "\\(QUByte Classics\\)"
   group: "modern_version"
 
 retro_bit:
   pattern: "\\(Retro-Bit\\)"
   group: "modern_version"
 
+retro_bit_generations:
+  pattern: "\\(Retro-Bit Generations\\)"
+  group: "modern_version"
+
+rockman_123:
+  pattern: "\\(Rockman 123\\)"
+  group: "modern_version"
+
 seiken_denetsu_collection:
   pattern: "\\(Seiken Densetsu Collection\\)"
   group: "modern_version"
 
 steam:
   pattern: "\\(Steam\\)"
   group: "modern_version"
@@ -340,51 +431,140 @@
   pattern: "\\(Virtual Console\\)"
   group: "modern_version"
 
 wii:
   pattern: "\\(Wii\\)"
   group: "modern_version"
 
+wii_virtual_console:
+  pattern: "\\((?:\\w*?,?\\s)*Wii Virtual Console(?:,?\\s\\w*?)*\\)"
+  group: "modern_version"
+
+wiiu_virtual_console:
+  pattern: "\\((?:\\w*?,?\\s)*Wii\\s?U Virtual Console(?:,?\\s\\w*?)*\\)"
+  group: "modern_version"
+
+wii_and_wiiu_virtual_console:
+  pattern: "\\((?:\\w*?,?\\s)*Wii Virtual Console, Wii\\s?U Virtual Console(?:,?\\s\\w*?)*\\)"
+  group: "modern_version"
+
 # DEMOTED VERSIONS
 arcade:
   pattern: "\\(Arcade\\)"
   group: "demoted_version"
 
+asder:
+  pattern: "\\(Asder\\)"
+  group: "demoted_version"
+
+caltron:
+  pattern: "\\(Caltron\\)"
+  group: "demoted_version"
+
+competition_cart:
+  pattern: "\\(Competition Cart.*?\\)"
+  group: "demoted_version"
+
+coolboy:
+  pattern: "\\(Coolboy\\)"
+  group: "demoted_version"
+
 debug_version:
   pattern: "\\(Debug Version\\)"
   group: "demoted_version"
 
 earlier:
   pattern: "\\(Earlier\\)"
   group: "demoted_version"
 
 early:
   pattern: "\\(Early\\)"
   group: "demoted_version"
 
-competition_cart:
-  pattern: "\\(Competition Cart.*?\\)"
+famicombox:
+  pattern: "\\(FamicomBox\\)"
+  group: "demoted_version"
+
+fs005:
+  pattern: "\\(FS005\\)"
+  group: "demoted_version"
+
+hwang_shinwei:
+  pattern: "\\(Hwang Shinwei\\)"
+  group: "demoted_version"
+
+jncota:
+  pattern: "\\(Jncota\\)"
   group: "demoted_version"
 
 limited_run:
   pattern: "\\(Limited Run Games\\)"
   group: "demoted_version"
 
+mb91:
+  pattern: "\\(MB-91\\)"
+  group: "demoted_version"
+
+mbc3:
+  pattern: "\\(MBC3\\)"
+  group: "demoted_version"
+
+mbc5:
+  pattern: "\\(MBC5\\)"
+  group: "demoted_version"
+
+micro_genius:
+  pattern: "\\(Micro Genius\\)"
+  group: "demoted_version"
+
+nintendoage:
+  pattern: "\\(NintendoAge\\)"
+  group: "demoted_version"
+
+no_cart_present:
+  pattern: "\\(No Cart Present\\)"
+  group: "demoted_version"
+
+not_for_resale:
+  pattern: "\\(Not for Resale\\)"
+  group: "demoted_version"
+
 piko_interactive:
   pattern: "\\(Piko Interactive\\)"
   group: "demote_version"
 
+rerelease:
+  pattern: "\\(Rerelease\\)"
+  group: "demoted_version"
+
 reprint:
   pattern: "\\(Reprint\\)"
   group: "demoted_version"
 
 shokai_seisanban:
   pattern: "\\(Shokai Seisanban\\)"
   group: "demoted_version"
 
 # GENERALLY IGNORE
 
+60_pin_cart:
+  pattern: "\\(60 pin cart\\)"
+
+72_pin_cart:
+  pattern: "\\(72 pin cart\\)"
+
 strictly_limited:
   pattern: "\\(Strictly Limited Games\\)"
 
-rerelease:
-  pattern: "\\(Rerelease\\)"
+ntdec:
+  pattern: "\\(NTDEC\\)"
+
+ntsc:
+  pattern: "([?:-][\\s])?[(]?NTSC\\)?"
+  flags: "NOFLAG"
+
+pal:
+  pattern: "([?:-][\\s])?[(]?PAL(?: [a-zA-Z]+| 50[Hh]z)?(?:\\)?| (?=\\())"
+  flags: "NOFLAG"
+
+43_406_pcb:
+  pattern: "\\(43-406 PCB\\)"
```

### Comparing `romsearch-0.0.1/romsearch/configs/sample_config.yml` & `romsearch-0.0.2/romsearch/configs/sample_config.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/romsearch/modules/datparser.py` & `romsearch-0.0.2/romsearch/modules/datparser.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/romsearch/modules/dupeparser.py` & `romsearch-0.0.2/romsearch/modules/dupeparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,20 +87,21 @@
         return True
 
     def get_dupe_dict(self):
         """Loop through potentially both the dat files and the retool config file to get out dupes"""
 
         dupe_dict = {}
 
-        if self.use_dat:
-            self.logger.info("Gettings dupes from dat file")
-            dupe_dict = self.get_dat_dupes(dupe_dict)
+        # Prefer retool dupes first
         if self.use_retool:
             self.logger.info("Gettings dupes from retool file")
             dupe_dict = self.get_retool_dupes(dupe_dict)
+        if self.use_dat:
+            self.logger.info("Gettings dupes from dat file")
+            dupe_dict = self.get_dat_dupes(dupe_dict)
 
         dupe_dict = dict(sorted(dupe_dict.items()))
 
         return dupe_dict
 
     def get_dat_dupes(self, dupe_dict=None):
         """Get dupes from the dat that we've already parsed to JSON"""
@@ -170,14 +171,19 @@
         """Get dupes from the retool curated list"""
 
         if dupe_dict is None:
             dupe_dict = {}
 
         retool_dupes = self.get_retool_dupe_dict()
         for retool_dupe in retool_dupes:
+
+            # If we don't have titles within the dupe dict, skip
+            if "titles" not in retool_dupe:
+                continue
+
             group = retool_dupe["group"]
             group_titles = [get_short_name(f["searchTerm"],
                                            default_config=self.default_config,
                                            regex_config=self.regex_config,
                                            )
                             for f in retool_dupe["titles"]]
             priorities = [f.get("priority", 1) for f in retool_dupe["titles"]]
```

### Comparing `romsearch-0.0.1/romsearch/modules/gamefinder.py` & `romsearch-0.0.2/romsearch/modules/gamefinder.py`

 * *Files 11% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     def run(self,
             files,
             ):
 
         self.logger.info(create_bar(f"START GameFinder"))
 
         games_dict = self.get_game_dict(files)
+        games_dict = dict(sorted(games_dict.items()))
 
         self.logger.info(f"Found {len(games_dict)} games:")
         for g in games_dict:
             self.logger.info(f"{g}: {games_dict[g]}")
 
         return games_dict
 
@@ -105,24 +106,25 @@
 
         # Remove any excluded files
         if self.exclude_games is not None:
             games_to_remove = self.get_game_matches(games,
                                                     self.exclude_games,
                                                     )
 
-            for i in sorted(games_to_remove, reverse=True):
-                games.pop(i)
+            if games_to_remove is not None:
+                for i in sorted(games_to_remove, reverse=True):
+                    games.pop(i)
 
         # Include only included files
         if self.include_games is not None:
             games_to_include = self.get_game_matches(games,
                                                      self.include_games,
                                                      )
-
-            games = np.asarray(games)[games_to_include]
+            if games_to_include is not None:
+                games = np.asarray(games)[games_to_include]
 
         # We need to trim down dupes here. Otherwise, the
         #  dict is just the list we already have
         game_dict = None
         if self.filter_dupes:
             game_dict = self.get_filter_dupes(games)
 
@@ -138,18 +140,21 @@
         return game_dict
 
     def get_game_matches(self, files, games_to_match):
         """Get files that match an input list (games_to_match)"""
         games_matched = []
 
         if isinstance(games_to_match, dict):
-            games_to_match = games_to_match.get(self.platform, [])
+            games_to_match = games_to_match.get(self.platform, None)
         else:
             games_to_match = copy.deepcopy(games_to_match)
 
+        if games_to_match is None:
+            return None
+
         games_matched.extend(games_to_match)
 
         idx = []
         for i, f in enumerate(files):
             found_f = False
             # Search within each item since the matches might not be exact
             for game_matched in games_matched:
@@ -182,15 +187,24 @@
 
         # Loop over games, and the dupes dictionary. Also pull out priority
         for g in games:
 
             found_parent_name = get_parent_name(game_name=g,
                                                 dupe_dict=dupes,
                                                 )
-            if found_parent_name not in game_dict:
+
+            found_parent_name_lower = found_parent_name.lower()
+            game_dict_keys = [key for key in game_dict.keys()]
+            game_dict_keys_lower = [key.lower() for key in game_dict.keys()]
+
+            if found_parent_name_lower not in game_dict_keys_lower:
                 game_dict[found_parent_name] = {}
+                final_parent_name = copy.deepcopy(found_parent_name)
+            else:
+                final_parent_idx = game_dict_keys_lower.index(found_parent_name_lower)
+                final_parent_name = game_dict_keys[final_parent_idx]
 
             priority = get_priority(dupe_dict=dupes, parent_name=found_parent_name, game_name=g)
 
-            game_dict[found_parent_name][g] = {"priority": priority}
+            game_dict[final_parent_name][g] = {"priority": priority}
 
         return game_dict
```

### Comparing `romsearch-0.0.1/romsearch/modules/romchooser.py` & `romsearch-0.0.2/romsearch/modules/romchooser.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,30 +193,37 @@
 
     return rom_dict
 
 
 def get_best_roms(files, rom_dict):
     """Get the best ROM(s) from a list, using a scoring system"""
 
+    # Positive scores
     improved_version_score = 1
+    version_score = 10
+    revision_score = 100
+    budget_edition_score = 1000
+
+    # Negative scores
     demoted_version_score = -1
     alternate_version_score = -1
     modern_version_score = -10
-    version_score = 100
     priority_score = -100
 
     file_scores = np.zeros(len(files))
 
     # Improved or demoted versions
     file_scores += improved_version_score * np.array([int(rom_dict[f]["improved_version"]) for f in files])
     file_scores += demoted_version_score * np.array([int(rom_dict[f]["demoted_version"]) for f in files])
+    file_scores += budget_edition_score * np.array([int(rom_dict[f]["budget_edition"]) for f in files])
     file_scores += alternate_version_score * np.array([int(rom_dict[f]["alternate"]) for f in files])
 
     # Version numbering, which needs to be parsed
     file_scores += version_score * add_versioned_score(files, rom_dict, "version")
+    file_scores += revision_score * add_versioned_score(files, rom_dict, "revision")
 
     # Downweight modern versions
     file_scores += modern_version_score * np.array([int(rom_dict[f]["modern_version"]) for f in files])
 
     # Priority scoring, where we subtract 1 so that the highest priority has no changed
     file_scores += priority_score * (np.array([int(rom_dict[f]["priority"]) for f in files]) - 1)
 
@@ -421,14 +428,15 @@
                                                )
 
         # Remove versions we potentially don't want around
         if self.use_best_version:
             self.logger.debug("Getting best version")
             rom_dict = get_best_version(rom_dict)
             rom_dict = remove_unwanted_roms(rom_dict, key_to_check="improved_versions", check_type="include")
+            rom_dict = remove_unwanted_roms(rom_dict, key_to_check="budget_edition", check_type="include")
             rom_dict = remove_unwanted_roms(rom_dict, key_to_check="demoted_versions", check_type="exclude")
             rom_dict = remove_unwanted_roms(rom_dict, key_to_check="modern_versions", check_type="exclude")
             rom_dict = remove_unwanted_roms(rom_dict, key_to_check="alternate", check_type="exclude")
             rom_dict = get_best_rom_per_region(rom_dict,
                                                self.region_preferences,
                                                )
```

### Comparing `romsearch-0.0.1/romsearch/modules/romdownloader.py` & `romsearch-0.0.2/romsearch/modules/romdownloader.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/romsearch/modules/rommover.py` & `romsearch-0.0.2/romsearch/modules/rommover.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/romsearch/modules/romparser.py` & `romsearch-0.0.2/romsearch/modules/romparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,14 +217,18 @@
         # Loop over the variants, see if we get a match
         found_cat = False
         for retool_dict in self.retool["variants"]:
 
             if found_cat:
                 continue
 
+            # If we don't have titles within the dupe dict, skip
+            if "titles" not in retool_dict:
+                continue
+
             retool_variants = [f["searchTerm"].lower() for f in retool_dict["titles"]]
 
             if game_name.lower() in retool_variants:
 
                 found_cat = True
 
                 # If we have categories, set these to True
```

### Comparing `romsearch-0.0.1/romsearch/modules/romsearch.py` & `romsearch-0.0.2/romsearch/modules/romsearch.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/romsearch/util/__init__.py` & `romsearch-0.0.2/romsearch/util/__init__.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/romsearch/util/general.py` & `romsearch-0.0.2/romsearch/util/general.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/romsearch/util/io.py` & `romsearch-0.0.2/romsearch/util/io.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/romsearch/util/logger.py` & `romsearch-0.0.2/romsearch/util/logger.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/romsearch/util/regex_matching.py` & `romsearch-0.0.2/romsearch/util/regex_matching.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.1/romsearch.egg-info/PKG-INFO` & `romsearch-0.0.2/romsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romsearch
-Version: 0.0.1
+Version: 0.0.2
 Summary: One Stop ROM Shop
 Author: bbtufty
 Maintainer: bbtufty
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `romsearch-0.0.1/romsearch.egg-info/SOURCES.txt` & `romsearch-0.0.2/romsearch.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -47,17 +47,20 @@
 romsearch/configs/defaults.yml
 romsearch/configs/regex.yml
 romsearch/configs/sample_config.yml
 romsearch/configs/clonelists/retool.yml
 romsearch/configs/dats/no-intro.yml
 romsearch/configs/dats/redump.yml
 romsearch/configs/platforms/Nintendo - GameCube.yml
+romsearch/configs/platforms/Nintendo - Nintendo Entertainment System.yml
 romsearch/configs/platforms/Nintendo - Super Nintendo Entertainment System.yml
 romsearch/configs/platforms/Sony - PlayStation 2.yml
 romsearch/configs/platforms/Sony - PlayStation.yml
+romsearch/dev/__init__.py
+romsearch/dev/parsing_tools.py
 romsearch/modules/__init__.py
 romsearch/modules/datparser.py
 romsearch/modules/dupeparser.py
 romsearch/modules/gamefinder.py
 romsearch/modules/romchooser.py
 romsearch/modules/romdownloader.py
 romsearch/modules/rommover.py
```

