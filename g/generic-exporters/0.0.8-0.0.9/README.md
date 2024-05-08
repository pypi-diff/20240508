# Comparing `tmp/generic_exporters-0.0.8.tar.gz` & `tmp/generic_exporters-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generic_exporters-0.0.8.tar", last modified: Sat Apr 27 20:29:02 2024, max compression
+gzip compressed data, was "generic_exporters-0.0.9.tar", last modified: Sun May  5 21:46:12 2024, max compression
```

## Comparing `generic_exporters-0.0.8.tar` & `generic_exporters-0.0.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.690675 generic_exporters-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    53248 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/.coverage
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.674675 generic_exporters-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.678675 generic_exporters-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/.github/workflows/deploy-docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-27 20:29:02.690675 generic_exporters-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.678675 generic_exporters-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.674675 generic_exporters-0.0.8/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.674675 generic_exporters-0.0.8/docs/_build/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.678675 generic_exporters-0.0.8/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/_build/html/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.682675 generic_exporters-0.0.8/generic_exporters/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/_awaitable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/_mathable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.682675 generic_exporters-0.0.8/generic_exporters/processors/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/TODO.md
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.686675 generic_exporters-0.0.8/generic_exporters/processors/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/exporters/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.686675 generic_exporters-0.0.8/generic_exporters/processors/exporters/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/exporters/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/exporters/datastores/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.686675 generic_exporters-0.0.8/generic_exporters/processors/exporters/datastores/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/exporters/datastores/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/exporters/datastores/timeseries/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/exporters/datastores/timeseries/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/exporters/datastores/timeseries/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/exporters/datastores/timeseries/victoria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/exporters/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/framer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/processors/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/generic_exporters/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.686675 generic_exporters-0.0.8/generic_exporters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-27 20:29:02.000000 generic_exporters-0.0.8/generic_exporters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-27 20:29:02.000000 generic_exporters-0.0.8/generic_exporters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 20:29:02.000000 generic_exporters-0.0.8/generic_exporters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-27 20:29:02.000000 generic_exporters-0.0.8/generic_exporters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 20:29:02.000000 generic_exporters-0.0.8/generic_exporters.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 20:29:02.690675 generic_exporters-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.686675 generic_exporters-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.686675 generic_exporters-0.0.8/tests/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.686675 generic_exporters-0.0.8/tests/processors/exporters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.686675 generic_exporters-0.0.8/tests/processors/exporters/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/processors/exporters/datastores/test_multi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:29:02.686675 generic_exporters-0.0.8/tests/processors/exporters/datastores/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/processors/exporters/datastores/timeseries/test_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/processors/exporters/datastores/timeseries/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/processors/exporters/datastores/timeseries/test_victoria.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/processors/exporters/test_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/processors/exporters/test_exporter_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/processors/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/test_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/test_mathable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-27 20:28:51.000000 generic_exporters-0.0.8/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.157331 generic_exporters-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    53248 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/.coverage
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.145331 generic_exporters-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.145331 generic_exporters-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-05 21:46:12.157331 generic_exporters-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.149331 generic_exporters-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.145331 generic_exporters-0.0.9/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.145331 generic_exporters-0.0.9/docs/_build/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.149331 generic_exporters-0.0.9/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/_build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/_build/html/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.149331 generic_exporters-0.0.9/generic_exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/_awaitable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/_mathable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.153331 generic_exporters-0.0.9/generic_exporters/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/TODO.md
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.153331 generic_exporters-0.0.9/generic_exporters/processors/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/exporters/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.153331 generic_exporters-0.0.9/generic_exporters/processors/exporters/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/exporters/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/exporters/datastores/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.153331 generic_exporters-0.0.9/generic_exporters/processors/exporters/datastores/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/exporters/datastores/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/exporters/datastores/timeseries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/exporters/datastores/timeseries/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/exporters/datastores/timeseries/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/exporters/datastores/timeseries/victoria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/exporters/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/framer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/processors/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/generic_exporters/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.157331 generic_exporters-0.0.9/generic_exporters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-05 21:46:12.000000 generic_exporters-0.0.9/generic_exporters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-05 21:46:12.000000 generic_exporters-0.0.9/generic_exporters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:46:12.000000 generic_exporters-0.0.9/generic_exporters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-05 21:46:12.000000 generic_exporters-0.0.9/generic_exporters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 21:46:12.000000 generic_exporters-0.0.9/generic_exporters.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 21:46:12.157331 generic_exporters-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.157331 generic_exporters-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.157331 generic_exporters-0.0.9/tests/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.157331 generic_exporters-0.0.9/tests/processors/exporters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.157331 generic_exporters-0.0.9/tests/processors/exporters/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/processors/exporters/datastores/test_multi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:46:12.157331 generic_exporters-0.0.9/tests/processors/exporters/datastores/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/processors/exporters/datastores/timeseries/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/processors/exporters/datastores/timeseries/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/processors/exporters/datastores/timeseries/test_victoria.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/processors/exporters/test_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/processors/exporters/test_exporter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/processors/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/test_mathable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-05 21:45:58.000000 generic_exporters-0.0.9/tests/test_timeseries.py
```

### Comparing `generic_exporters-0.0.8/.coverage` & `generic_exporters-0.0.9/.coverage`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/.github/workflows/deploy-docs.yaml` & `generic_exporters-0.0.9/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/.github/workflows/pages.yml` & `generic_exporters-0.0.9/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/.github/workflows/pytest.yaml` & `generic_exporters-0.0.9/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/.github/workflows/release.yaml` & `generic_exporters-0.0.9/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/docs/Makefile` & `generic_exporters-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/docs/_build/html/_static/alabaster.css` & `generic_exporters-0.0.9/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/docs/_build/html/_static/basic.css` & `generic_exporters-0.0.9/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/docs/_build/html/_static/doctools.js` & `generic_exporters-0.0.9/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/docs/_build/html/_static/language_data.js` & `generic_exporters-0.0.9/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/docs/_build/html/_static/pygments.css` & `generic_exporters-0.0.9/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/docs/_build/html/_static/searchtools.js` & `generic_exporters-0.0.9/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/docs/_build/html/_static/sphinx_highlight.js` & `generic_exporters-0.0.9/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/docs/conf.py` & `generic_exporters-0.0.9/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     'a_sync': ('https://bobthebuidler.github.io/ez-a-sync', None),
     'aiohttp': ('https://docs.aiohttp.org/', None),
     'bqplot': ('https://bqplot.github.io/bqplot/', None),
     'msgspec': ('https://jcristharif.com/msgspec/', None),
     'pandas': ('https://pandas.pydata.org/pandas-docs/', None),
     'pony': ('https://docs.ponyorm.org/', None),
     'python': ('https://docs.python.org/3', None),
+    'typing_extensions': ('https://typing-extensions.readthedocs.io/en/latest/', None),
 }
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'alabaster'
 html_static_path = ['_static']
```

### Comparing `generic_exporters-0.0.8/docs/make.bat` & `generic_exporters-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/_awaitable.py` & `generic_exporters-0.0.9/generic_exporters/_awaitable.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/_constant.py` & `generic_exporters-0.0.9/generic_exporters/_constant.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/_mathable.py` & `generic_exporters-0.0.9/generic_exporters/_mathable.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/_time.py` & `generic_exporters-0.0.9/generic_exporters/_time.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/dataset.py` & `generic_exporters-0.0.9/generic_exporters/dataset.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/metric.py` & `generic_exporters-0.0.9/generic_exporters/metric.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/plan.py` & `generic_exporters-0.0.9/generic_exporters/plan.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/processors/_base.py` & `generic_exporters-0.0.9/generic_exporters/processors/_base.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/processors/exporters/_base.py` & `generic_exporters-0.0.9/generic_exporters/processors/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/processors/exporters/datastores/default.py` & `generic_exporters-0.0.9/generic_exporters/processors/exporters/datastores/default.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/processors/exporters/datastores/timeseries/multi.py` & `generic_exporters-0.0.9/generic_exporters/processors/exporters/datastores/timeseries/multi.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/processors/exporters/datastores/timeseries/sql.py` & `generic_exporters-0.0.9/generic_exporters/processors/exporters/datastores/timeseries/sql.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/processors/exporters/datastores/timeseries/victoria.py` & `generic_exporters-0.0.9/generic_exporters/processors/exporters/datastores/timeseries/victoria.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/processors/exporters/exporter.py` & `generic_exporters-0.0.9/generic_exporters/processors/exporters/exporter.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/processors/framer.py` & `generic_exporters-0.0.9/generic_exporters/processors/framer.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/processors/plotter.py` & `generic_exporters-0.0.9/generic_exporters/processors/plotter.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters/timeseries.py` & `generic_exporters-0.0.9/generic_exporters/timeseries.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/generic_exporters.egg-info/SOURCES.txt` & `generic_exporters-0.0.9/generic_exporters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/setup.py` & `generic_exporters-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/tests/fixtures.py` & `generic_exporters-0.0.9/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/tests/processors/exporters/datastores/test_multi.py` & `generic_exporters-0.0.9/tests/processors/exporters/datastores/test_multi.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/tests/processors/exporters/datastores/timeseries/test_sql.py` & `generic_exporters-0.0.9/tests/processors/exporters/datastores/timeseries/test_sql.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/tests/processors/exporters/datastores/timeseries/test_victoria.py` & `generic_exporters-0.0.9/tests/processors/exporters/datastores/timeseries/test_victoria.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/tests/processors/test_base.py` & `generic_exporters-0.0.9/tests/processors/test_base.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/tests/test_constant.py` & `generic_exporters-0.0.9/tests/test_constant.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/tests/test_dataset.py` & `generic_exporters-0.0.9/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/tests/test_mathable.py` & `generic_exporters-0.0.9/tests/test_mathable.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/tests/test_metric.py` & `generic_exporters-0.0.9/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/tests/test_plan.py` & `generic_exporters-0.0.9/tests/test_plan.py`

 * *Files identical despite different names*

### Comparing `generic_exporters-0.0.8/tests/test_timeseries.py` & `generic_exporters-0.0.9/tests/test_timeseries.py`

 * *Files identical despite different names*

