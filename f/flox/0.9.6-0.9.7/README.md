# Comparing `tmp/flox-0.9.6.tar.gz` & `tmp/flox-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flox-0.9.6.tar", last modified: Wed Mar 27 14:24:59 2024, max compression
+gzip compressed data, was "flox-0.9.7.tar", last modified: Wed May  8 13:41:11 2024, max compression
```

## Comparing `flox-0.9.6.tar` & `flox-0.9.7.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:24:59.416994 flox-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-27 14:24:27.000000 flox-0.9.6/.git_archival.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:24:59.396994 flox-0.9.6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-27 14:24:27.000000 flox-0.9.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:24:59.400994 flox-0.9.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-03-27 14:24:27.000000 flox-0.9.6/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-03-27 14:24:27.000000 flox-0.9.6/.github/workflows/ci-additional.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-03-27 14:24:27.000000 flox-0.9.6/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-27 14:24:27.000000 flox-0.9.6/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-03-27 14:24:27.000000 flox-0.9.6/.github/workflows/testpypi-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-03-27 14:24:27.000000 flox-0.9.6/.github/workflows/upstream-dev-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-27 14:24:27.000000 flox-0.9.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-27 14:24:27.000000 flox-0.9.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-27 14:24:27.000000 flox-0.9.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-03-27 14:24:27.000000 flox-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18029 2024-03-27 14:24:59.416994 flox-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-03-27 14:24:27.000000 flox-0.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:24:59.400994 flox-0.9.6/asv_bench/
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-03-27 14:24:27.000000 flox-0.9.6/asv_bench/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:24:59.400994 flox-0.9.6/asv_bench/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-03-27 14:24:27.000000 flox-0.9.6/asv_bench/benchmarks/README_CI.md
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-27 14:24:27.000000 flox-0.9.6/asv_bench/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-03-27 14:24:27.000000 flox-0.9.6/asv_bench/benchmarks/cohorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-27 14:24:27.000000 flox-0.9.6/asv_bench/benchmarks/combine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-03-27 14:24:27.000000 flox-0.9.6/asv_bench/benchmarks/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:24:59.400994 flox-0.9.6/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-27 14:24:27.000000 flox-0.9.6/ci/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-27 14:24:27.000000 flox-0.9.6/ci/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-27 14:24:27.000000 flox-0.9.6/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-27 14:24:27.000000 flox-0.9.6/ci/minimal-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-27 14:24:27.000000 flox-0.9.6/ci/no-dask.yml
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-27 14:24:27.000000 flox-0.9.6/ci/no-numba.yml
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-27 14:24:27.000000 flox-0.9.6/ci/no-xarray.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-27 14:24:27.000000 flox-0.9.6/ci/upstream-dev-env.yml
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-27 14:24:27.000000 flox-0.9.6/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:24:59.400994 flox-0.9.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-03-27 14:24:27.000000 flox-0.9.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:24:59.404994 flox-0.9.6/docs/diagrams/
--rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/bitmask-patterns-perfect.png
--rw-r--r--   0 runner    (1001) docker     (127)    43022 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/blockwise.png
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/cohorts-month-chunk4.png
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/cohorts-month-chunk5.png
--rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/containment.png
--rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/counties-bitmask-containment.png
--rw-r--r--   0 runner    (1001) docker     (127)    46006 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/map-reduce.png
--rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/new-blockwise-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (127)    38910 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/new-blockwise.svg
--rw-r--r--   0 runner    (1001) docker     (127)   102136 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/new-cohorts-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (127)    60369 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/new-cohorts.svg
--rw-r--r--   0 runner    (1001) docker     (127)   105406 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/new-map-reduce-reindex-False-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (127)    62434 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/new-map-reduce-reindex-False.svg
--rw-r--r--   0 runner    (1001) docker     (127)   101278 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/new-map-reduce-reindex-True-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (127)    62159 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/new-map-reduce-reindex-True.svg
--rw-r--r--   0 runner    (1001) docker     (127)   177642 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/new-split-apply-combine-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (127)   153059 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/nwm-cohorts.png
--rw-r--r--   0 runner    (1001) docker     (127)    61350 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/split-apply-combine.svg
--rw-r--r--   0 runner    (1001) docker     (127)    55442 2024-03-27 14:24:27.000000 flox-0.9.6/docs/diagrams/split-reduce.png
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-03-27 14:24:27.000000 flox-0.9.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-27 14:24:27.000000 flox-0.9.6/docs/requirements-docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:24:59.408994 flox-0.9.6/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:24:59.408994 flox-0.9.6/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/aggregations.md
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/arrays.md
--rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/engines.md
--rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/implementation.md
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/intro.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:24:59.408994 flox-0.9.6/docs/source/user-stories/
--rw-r--r--   0 runner    (1001) docker     (127)    74658 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/user-stories/climatology-hourly.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/user-stories/climatology.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/user-stories/custom-aggregations.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   733833 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/user-stories/hourly-climatology.html
--rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/user-stories/nD-bins.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/user-stories/overlaps.md
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/user-stories.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-27 14:24:27.000000 flox-0.9.6/docs/source/xarray.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:24:59.412994 flox-0.9.6/flox/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-27 14:24:27.000000 flox-0.9.6/flox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 14:24:58.000000 flox-0.9.6/flox/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-03-27 14:24:27.000000 flox-0.9.6/flox/aggregate_flox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-03-27 14:24:27.000000 flox-0.9.6/flox/aggregate_npg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-03-27 14:24:27.000000 flox-0.9.6/flox/aggregate_numbagg.py
--rw-r--r--   0 runner    (1001) docker     (127)    21873 2024-03-27 14:24:27.000000 flox-0.9.6/flox/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-27 14:24:27.000000 flox-0.9.6/flox/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    89711 2024-03-27 14:24:27.000000 flox-0.9.6/flox/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 14:24:27.000000 flox-0.9.6/flox/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-03-27 14:24:27.000000 flox-0.9.6/flox/visualize.py
--rw-r--r--   0 runner    (1001) docker     (127)    25338 2024-03-27 14:24:27.000000 flox-0.9.6/flox/xarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-03-27 14:24:27.000000 flox-0.9.6/flox/xrdtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-03-27 14:24:27.000000 flox-0.9.6/flox/xrutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:24:59.412994 flox-0.9.6/flox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18029 2024-03-27 14:24:59.000000 flox-0.9.6/flox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-03-27 14:24:59.000000 flox-0.9.6/flox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 14:24:59.000000 flox-0.9.6/flox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-27 14:24:59.000000 flox-0.9.6/flox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-27 14:24:59.000000 flox-0.9.6/flox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-03-27 14:24:27.000000 flox-0.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-27 14:24:27.000000 flox-0.9.6/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 14:24:59.416994 flox-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-27 14:24:27.000000 flox-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:24:59.412994 flox-0.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-03-27 14:24:27.000000 flox-0.9.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-27 14:24:27.000000 flox-0.9.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    58998 2024-03-27 14:24:27.000000 flox-0.9.6/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    24647 2024-03-27 14:24:27.000000 flox-0.9.6/tests/test_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.627633 flox-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-08 13:40:54.000000 flox-0.9.7/.git_archival.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.607633 flox-0.9.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-08 13:40:54.000000 flox-0.9.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.607633 flox-0.9.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 13:40:54.000000 flox-0.9.7/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-08 13:40:54.000000 flox-0.9.7/.github/workflows/ci-additional.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-08 13:40:54.000000 flox-0.9.7/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-08 13:40:54.000000 flox-0.9.7/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-08 13:40:54.000000 flox-0.9.7/.github/workflows/testpypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-08 13:40:54.000000 flox-0.9.7/.github/workflows/upstream-dev-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-08 13:40:54.000000 flox-0.9.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-08 13:40:54.000000 flox-0.9.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-08 13:40:54.000000 flox-0.9.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-08 13:40:54.000000 flox-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18029 2024-05-08 13:41:11.627633 flox-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-08 13:40:54.000000 flox-0.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.607633 flox-0.9.7/asv_bench/
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-08 13:40:54.000000 flox-0.9.7/asv_bench/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.607633 flox-0.9.7/asv_bench/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-08 13:40:54.000000 flox-0.9.7/asv_bench/benchmarks/README_CI.md
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-08 13:40:54.000000 flox-0.9.7/asv_bench/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-05-08 13:40:54.000000 flox-0.9.7/asv_bench/benchmarks/cohorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-08 13:40:54.000000 flox-0.9.7/asv_bench/benchmarks/combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-08 13:40:54.000000 flox-0.9.7/asv_bench/benchmarks/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.611633 flox-0.9.7/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-08 13:40:54.000000 flox-0.9.7/ci/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 13:40:54.000000 flox-0.9.7/ci/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-08 13:40:54.000000 flox-0.9.7/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 13:40:54.000000 flox-0.9.7/ci/minimal-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-08 13:40:54.000000 flox-0.9.7/ci/no-dask.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-08 13:40:54.000000 flox-0.9.7/ci/no-numba.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-08 13:40:54.000000 flox-0.9.7/ci/no-xarray.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-08 13:40:54.000000 flox-0.9.7/ci/upstream-dev-env.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 13:40:54.000000 flox-0.9.7/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.611633 flox-0.9.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-08 13:40:54.000000 flox-0.9.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.615633 flox-0.9.7/docs/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/bitmask-patterns-perfect.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43022 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/blockwise.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/cohorts-month-chunk4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/cohorts-month-chunk5.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/containment.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/counties-bitmask-containment.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46006 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/map-reduce.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-blockwise-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    38910 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-blockwise.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   102136 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-cohorts-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    60369 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-cohorts.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   105406 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-map-reduce-reindex-False-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    62434 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-map-reduce-reindex-False.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   101278 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-map-reduce-reindex-True-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    62159 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-map-reduce-reindex-True.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   177642 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/new-split-apply-combine-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   153059 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/nwm-cohorts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61350 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/split-apply-combine.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    55442 2024-05-08 13:40:54.000000 flox-0.9.7/docs/diagrams/split-reduce.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-08 13:40:54.000000 flox-0.9.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 13:40:54.000000 flox-0.9.7/docs/requirements-docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.619633 flox-0.9.7/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.619633 flox-0.9.7/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/aggregations.md
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/arrays.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/engines.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/implementation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/intro.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.619633 flox-0.9.7/docs/source/user-stories/
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories/climatology-hourly-cubed.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    74240 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories/climatology-hourly.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories/climatology.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories/custom-aggregations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   733833 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories/hourly-climatology.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories/nD-bins.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories/overlaps.md
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/user-stories.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-08 13:40:54.000000 flox-0.9.7/docs/source/xarray.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.623633 flox-0.9.7/flox/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-08 13:40:54.000000 flox-0.9.7/flox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 13:41:11.000000 flox-0.9.7/flox/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-05-08 13:40:54.000000 flox-0.9.7/flox/aggregate_flox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-08 13:40:54.000000 flox-0.9.7/flox/aggregate_npg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-08 13:40:54.000000 flox-0.9.7/flox/aggregate_numbagg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21913 2024-05-08 13:40:54.000000 flox-0.9.7/flox/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-08 13:40:54.000000 flox-0.9.7/flox/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96440 2024-05-08 13:40:54.000000 flox-0.9.7/flox/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:54.000000 flox-0.9.7/flox/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-08 13:40:54.000000 flox-0.9.7/flox/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25338 2024-05-08 13:40:54.000000 flox-0.9.7/flox/xarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-08 13:40:54.000000 flox-0.9.7/flox/xrdtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12005 2024-05-08 13:40:54.000000 flox-0.9.7/flox/xrutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.623633 flox-0.9.7/flox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18029 2024-05-08 13:41:11.000000 flox-0.9.7/flox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-08 13:41:11.000000 flox-0.9.7/flox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:41:11.000000 flox-0.9.7/flox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-08 13:41:11.000000 flox-0.9.7/flox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 13:41:11.000000 flox-0.9.7/flox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-08 13:40:54.000000 flox-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-08 13:40:54.000000 flox-0.9.7/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:41:11.627633 flox-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-08 13:40:54.000000 flox-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:41:11.623633 flox-0.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-08 13:40:54.000000 flox-0.9.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-08 13:40:54.000000 flox-0.9.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61218 2024-05-08 13:40:54.000000 flox-0.9.7/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24647 2024-05-08 13:40:54.000000 flox-0.9.7/tests/test_xarray.py
```

### Comparing `flox-0.9.6/.github/workflows/benchmarks.yml` & `flox-0.9.7/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/.github/workflows/ci-additional.yaml` & `flox-0.9.7/.github/workflows/ci-additional.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
       - name: Run doctests
         run: |
           python -m pytest --doctest-modules \
           flox/aggregations.py flox/core.py flox/xarray.py \
           --ignore flox/tests \
           --cov=./ --cov-report=xml
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v4.1.0
+        uses: codecov/codecov-action@v4.3.1
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: RUNNER_OS
           name: codecov-umbrella
           fail_ci_if_error: false
 
@@ -127,14 +127,14 @@
           python -m pip install mypy
 
       - name: Run mypy
         run: |
           python -m mypy --install-types --non-interactive --cobertura-xml-report mypy_report
 
       - name: Upload mypy coverage to Codecov
-        uses: codecov/codecov-action@v4.1.0
+        uses: codecov/codecov-action@v4.3.1
         with:
           file: mypy_report/cobertura.xml
           flags: mypy
           env_vars: PYTHON_VERSION
           name: codecov-umbrella
           fail_ci_if_error: false
```

### Comparing `flox-0.9.6/.github/workflows/ci.yaml` & `flox-0.9.7/.github/workflows/ci.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,19 @@
     runs-on: ${{ matrix.os }}
     defaults:
       run:
         shell: bash -l {0}
     strategy:
       fail-fast: false
       matrix:
-        os: ["ubuntu-latest", "windows-latest"]
+        os: ["ubuntu-latest"]
         python-version: ["3.9", "3.12"]
+        include:
+          - os: "windows-latest"
+            python-version: "3.12"
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0 # Fetch all history for all branches and tags.
       - name: Set environment variables
         run: |
           echo "PYTHON_VERSION=${{ matrix.python-version }}" >> $GITHUB_ENV
@@ -45,15 +48,15 @@
       - name: Install flox
         run: |
           python -m pip install --no-deps -e .
       - name: Run Tests
         run: |
           pytest -n auto --cov=./ --cov-report=xml
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v4.1.0
+        uses: codecov/codecov-action@v4.3.1
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: RUNNER_OS,PYTHON_VERSION
           name: codecov-umbrella
           fail_ci_if_error: false
 
@@ -63,18 +66,16 @@
     defaults:
       run:
         shell: bash -l {0}
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.12"]
-        env: ["no-xarray", "no-dask"]
+        env: ["no-dask"] # "no-xarray", "no-numba"
         include:
-          - env: "no-numba"
-            python-version: "3.12"
           - env: "minimal-requirements"
             python-version: "3.9"
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0 # Fetch all history for all branches and tags.
       - name: Set up conda environment
@@ -89,15 +90,15 @@
       - name: Install flox
         run: |
           python -m pip install --no-deps -e .
       - name: Run tests
         run: |
           python -m pytest -n auto --cov=./ --cov-report=xml
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v4.1.0
+        uses: codecov/codecov-action@v4.3.1
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: RUNNER_OS
           name: codecov-umbrella
           fail_ci_if_error: false
```

### Comparing `flox-0.9.6/.github/workflows/pypi.yaml` & `flox-0.9.7/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/.github/workflows/testpypi-release.yaml` & `flox-0.9.7/.github/workflows/testpypi-release.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/.github/workflows/upstream-dev-ci.yaml` & `flox-0.9.7/.github/workflows/upstream-dev-ci.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/.gitignore` & `flox-0.9.7/.gitignore`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/.pre-commit-config.yaml` & `flox-0.9.7/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ci:
   autoupdate_schedule: quarterly
 
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: "v0.1.9"
+    rev: "v0.3.5"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v4.0.0-alpha.8"
     hooks:
@@ -19,53 +19,53 @@
     hooks:
       - id: check-yaml
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-docstring-first
 
   - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: 23.12.1
+    rev: 24.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
       - id: mdformat
         additional_dependencies:
           - mdformat-black
           - mdformat-myst
 
   - repo: https://github.com/nbQA-dev/nbQA
-    rev: 1.7.1
+    rev: 1.8.5
     hooks:
       - id: nbqa-black
       - id: nbqa-ruff
         args: [--fix]
 
   - repo: https://github.com/kynan/nbstripout
-    rev: 0.6.1
+    rev: 0.7.1
     hooks:
       - id: nbstripout
         args: [--extra-keys=metadata.kernelspec metadata.language_info.version]
 
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
       - id: codespell
         additional_dependencies:
           - tomli
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.15
+    rev: v0.16
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/rhysd/actionlint
-    rev: v1.6.26
+    rev: v1.6.27
     hooks:
       - id: actionlint
         files: ".github/workflows/"
         args:
           [
             "-ignore",
             "SC1090",
```

### Comparing `flox-0.9.6/LICENSE` & `flox-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/PKG-INFO` & `flox-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flox
-Version: 0.9.6
+Version: 0.9.7
 Summary: GroupBy operations for dask.array
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flox-0.9.6/README.md` & `flox-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/asv_bench/asv.conf.json` & `flox-0.9.7/asv_bench/asv.conf.json`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,19 @@
   //
   // "install_command": ["in-dir={env_dir} python -mpip install {wheel_file}"],
   // "uninstall_command": ["return-code=any python -mpip uninstall -y {project}"],
   // "build_command": [
   //     "python setup.py build",
   //     "PIP_NO_BUILD_ISOLATION=false python -mpip wheel --no-deps --no-index -w {build_cache_dir} {build_dir}"
   // ],
+  //
+  "build_command": [
+    "python setup.py build",
+    "python -mpip wheel --no-deps --no-build-isolation --no-index -w {build_cache_dir} {build_dir}"
+  ],
 
   // List of branches to benchmark. If not provided, defaults to "master"
   // (for git) or "default" (for mercurial).
   "branches": ["main"], // for git
   "dvcs": "git",
 
   // timeout in seconds for installing any dependencies in environment
```

### Comparing `flox-0.9.6/asv_bench/benchmarks/README_CI.md` & `flox-0.9.7/asv_bench/benchmarks/README_CI.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/asv_bench/benchmarks/__init__.py` & `flox-0.9.7/asv_bench/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/asv_bench/benchmarks/cohorts.py` & `flox-0.9.7/asv_bench/benchmarks/cohorts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+from functools import cached_property
+
 import dask
 import numpy as np
 import pandas as pd
 
 import flox
 
 
 class Cohorts:
     """Time the core reduction function."""
 
     def setup(self, *args, **kwargs):
         raise NotImplementedError
 
+    @cached_property
+    def result(self):
+        return flox.groupby_reduce(self.array, self.by, func="sum", axis=self.axis)[0]
+
     def containment(self):
         asfloat = self.bitmask().astype(float)
         chunks_per_label = asfloat.sum(axis=0)
         containment = (asfloat.T @ asfloat) / chunks_per_label
         print(containment.nnz / np.prod(containment.shape))
         return containment.todense()
 
@@ -39,34 +45,25 @@
         # Not sure why
         try:
             flox.cache.cache.clear()
         except AttributeError:
             pass
 
     def time_graph_construct(self):
-        flox.groupby_reduce(self.array, self.by, func="sum", axis=self.axis, method="cohorts")
+        flox.groupby_reduce(self.array, self.by, func="sum", axis=self.axis)
 
     def track_num_tasks(self):
-        result = flox.groupby_reduce(
-            self.array, self.by, func="sum", axis=self.axis, method="cohorts"
-        )[0]
-        return len(result.dask.to_dict())
+        return len(self.result.dask.to_dict())
 
     def track_num_tasks_optimized(self):
-        result = flox.groupby_reduce(
-            self.array, self.by, func="sum", axis=self.axis, method="cohorts"
-        )[0]
-        (opt,) = dask.optimize(result)
+        (opt,) = dask.optimize(self.result)
         return len(opt.dask.to_dict())
 
     def track_num_layers(self):
-        result = flox.groupby_reduce(
-            self.array, self.by, func="sum", axis=self.axis, method="cohorts"
-        )[0]
-        return len(result.dask.layers)
+        return len(self.result.dask.layers)
 
     track_num_tasks.unit = "tasks"  # type: ignore[attr-defined] # Lazy
     track_num_tasks_optimized.unit = "tasks"  # type: ignore[attr-defined] # Lazy
     track_num_layers.unit = "layers"  # type: ignore[attr-defined] # Lazy
     for f in [track_num_tasks, track_num_tasks_optimized, track_num_layers]:
         f.repeat = 1  # type: ignore[attr-defined] # Lazy
         f.rounds = 1  # type: ignore[attr-defined] # Lazy
@@ -189,14 +186,27 @@
         TIME = len(self.time)
         self.axis = (2,)
         self.array = dask.array.ones((721, 1440, TIME), chunks=(-1, -1, 10))
         self.by = codes_for_resampling(index, freq="5D")
         self.expected = pd.RangeIndex(self.by.max() + 1)
 
 
+class SingleChunk(Cohorts):
+    """Single chunk along reduction axis: always blockwise."""
+
+    def setup(self, *args, **kwargs):
+        index = pd.date_range("1959-01-01", freq="D", end="1962-12-31")
+        self.time = pd.Series(index)
+        TIME = len(self.time)
+        self.axis = (2,)
+        self.array = dask.array.ones((721, 1440, TIME), chunks=(-1, -1, -1))
+        self.by = codes_for_resampling(index, freq="5D")
+        self.expected = pd.RangeIndex(self.by.max() + 1)
+
+
 class OISST(Cohorts):
     def setup(self, *args, **kwargs):
         self.array = dask.array.ones((1, 14532), chunks=(1, 10))
         self.axis = (1,)
         index = pd.date_range("1981-09-01 12:00", "2021-06-14 12:00", freq="D")
         self.time = pd.Series(index)
         self.by = self.time.dt.dayofyear.values - 1
```

### Comparing `flox-0.9.6/asv_bench/benchmarks/combine.py` & `flox-0.9.7/asv_bench/benchmarks/combine.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/asv_bench/benchmarks/reduce.py` & `flox-0.9.7/asv_bench/benchmarks/reduce.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/ci/upstream-dev-env.yml` & `flox-0.9.7/ci/upstream-dev-env.yml`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/Makefile` & `flox-0.9.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/bitmask-patterns-perfect.png` & `flox-0.9.7/docs/diagrams/bitmask-patterns-perfect.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/blockwise.png` & `flox-0.9.7/docs/diagrams/blockwise.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/cohorts-month-chunk4.png` & `flox-0.9.7/docs/diagrams/cohorts-month-chunk4.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/cohorts-month-chunk5.png` & `flox-0.9.7/docs/diagrams/cohorts-month-chunk5.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/containment.png` & `flox-0.9.7/docs/diagrams/containment.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/counties-bitmask-containment.png` & `flox-0.9.7/docs/diagrams/counties-bitmask-containment.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/map-reduce.png` & `flox-0.9.7/docs/diagrams/map-reduce.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/new-blockwise-annotated.svg` & `flox-0.9.7/docs/diagrams/new-blockwise-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/new-blockwise.svg` & `flox-0.9.7/docs/diagrams/new-blockwise.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/new-cohorts-annotated.svg` & `flox-0.9.7/docs/diagrams/new-cohorts-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/new-cohorts.svg` & `flox-0.9.7/docs/diagrams/new-cohorts.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/new-map-reduce-reindex-False-annotated.svg` & `flox-0.9.7/docs/diagrams/new-map-reduce-reindex-False-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/new-map-reduce-reindex-False.svg` & `flox-0.9.7/docs/diagrams/new-map-reduce-reindex-False.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/new-map-reduce-reindex-True-annotated.svg` & `flox-0.9.7/docs/diagrams/new-map-reduce-reindex-True-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/new-map-reduce-reindex-True.svg` & `flox-0.9.7/docs/diagrams/new-map-reduce-reindex-True.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/new-split-apply-combine-annotated.svg` & `flox-0.9.7/docs/diagrams/new-split-apply-combine-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/nwm-cohorts.png` & `flox-0.9.7/docs/diagrams/nwm-cohorts.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/split-apply-combine.svg` & `flox-0.9.7/docs/diagrams/split-apply-combine.svg`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/diagrams/split-reduce.png` & `flox-0.9.7/docs/diagrams/split-reduce.png`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/make.bat` & `flox-0.9.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/source/aggregations.md` & `flox-0.9.7/docs/source/aggregations.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/source/api.rst` & `flox-0.9.7/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/source/arrays.md` & `flox-0.9.7/docs/source/arrays.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/source/conf.py` & `flox-0.9.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/source/engines.md` & `flox-0.9.7/docs/source/engines.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/source/implementation.md` & `flox-0.9.7/docs/source/implementation.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/source/index.md` & `flox-0.9.7/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/source/intro.md` & `flox-0.9.7/docs/source/intro.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/source/user-stories/climatology-hourly.ipynb` & `flox-0.9.7/docs/source/user-stories/climatology-hourly.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874131944444444%*

 * *Differences: {"'cells'": "{0: {'id': '0'}, 1: {'id': '1'}, 2: {'id': '2'}, 3: {'id': '3'}, 4: {'id': '4'}, 5: "*

 * *            "{'id': '5'}, 6: {'id': '6'}, 7: {'id': '7'}, 8: {'id': '8'}, 9: {'id': '9'}, 10: "*

 * *            "{'id': '10'}, 11: {'id': '11'}}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "84e8bbee-90cc-4e6a-bf89-c56dc19c11ca",
+            "id": "0",
             "metadata": {},
             "source": [
                 "# More climatology reductions\n",
                 "\n",
                 "This one is motivated by\n",
                 "[this Pangeo Discourse post](https://discourse.pangeo.io/t/dask-xarray-and-swap-memory-polution-on-local-linux-cluster/2453/5)\n",
                 "and follows\n",
@@ -22,15 +22,15 @@
                 "   Y, 744) being reduced to (X, Y, 24) i.e. 744/24=31x decrease in chunk size,\n",
                 "   so this should work well memory wise.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "727f490e-906a-4537-ac5e-3c67985cd6d5",
+            "id": "1",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "/Users/dcherian/mambaforge/envs/dcpy/lib/python3.8/site-packages/distributed/node.py:180: UserWarning: Port 8787 is already in use.\n",
@@ -69,15 +69,15 @@
                 "client = Client(memory_limit=\"2 GiB\", threads_per_worker=1, n_workers=4)\n",
                 "client.cluster"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6085684f-cafa-450c-8448-d5c9c1cbb55f",
+            "id": "2",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "dask  : 2022.3.0\n",
@@ -94,24 +94,24 @@
                 "\n",
                 "\n",
                 "%watermark -iv"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5380714a-b35f-4fb0-8b3d-7528ef7a7595",
+            "id": "3",
             "metadata": {},
             "source": [
                 "## Create data\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2aa66559-b2dd-4b46-b32b-f1ce2270c3de",
+            "id": "4",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
@@ -632,24 +632,24 @@
                 "    coords={\"time\": pd.date_range(\"2021-01-01\", \"2021-12-31 23:59\", freq=\"H\")},\n",
                 ")\n",
                 "ds"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3a350782-b747-4e5e-8b8b-15fab72c0d2c",
+            "id": "5",
             "metadata": {},
             "source": [
                 "Here's just plain xarray: 10000 tasks and one chunk per hour in the output\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ecc77698-5879-4b7c-ad97-891fb104d295",
+            "id": "6",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
@@ -1169,24 +1169,24 @@
             ],
             "source": [
                 "ds.tp.groupby(\"time.hour\").mean()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "beccd9f8-ad62-4cd8-86cc-acfe14f13023",
+            "id": "7",
             "metadata": {},
             "source": [
                 "And flox: 600 tasks and all hours in a single chunk\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0a3da8e5-863a-4602-9176-0a9adc689563",
+            "id": "8",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
@@ -1672,33 +1672,33 @@
                 "hourly = flox.xarray.xarray_reduce(ds.tp, ds.time.dt.hour, func=\"mean\")\n",
                 "hourly"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8aa1a641-1ce1-4264-96dc-d11bb1d4ab57",
+            "id": "9",
             "metadata": {},
             "outputs": [],
             "source": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e37c5aa2-c77a-4d87-8db4-5052c675c42d",
+            "id": "10",
             "metadata": {},
             "outputs": [],
             "source": [
                 "with performance_report(\"hourly-climatology.html\"):\n",
                 "    hourly.compute()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "494766c2-305a-4518-b2b7-a85bcc7fd5b2",
+            "id": "11",
             "metadata": {},
             "source": [
                 "View the performance report\n",
                 "[here](https://rawcdn.githack.com/dcherian/flox/592c46ba0bb859f732968b68426b6332caebc213/docs/source/user-stories/hourly-climatology.html),\n",
                 "and a video of the dask dashboard\n",
                 "[here](https://drive.google.com/file/d/1uY36DiTbv1w7TefbrCEyBcOli5NiaNUP/view?usp=sharing)\n"
             ]
```

### Comparing `flox-0.9.6/docs/source/user-stories/climatology.ipynb` & `flox-0.9.7/docs/source/user-stories/custom-aggregations.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9195438171953132%*

 * *Differences: {"'cells'": "{0: {'id': '0', 'source': {insert: [(0, '# Custom Aggregations\\n'), (2, 'This "*

 * *            "notebook is motivated by a\\n'), (3, "*

 * *            "'[post](https://discourse.pangeo.io/t/using-xhistogram-to-bin-measurements-at-particular-stations/2365/4)\\n'), "*

 * *            "(5, '\\n'), (6, '> Even better would be a command that lets me simply do the "*

 * *            'following.\\n\'), (7, \'>\\n\'), (8, ">     A = da.groupby([\'lon_bins\', '*

 * *            '\'lat_bins\']).mode()\\n"), (9, \'\\n\'), (10 […]*

```diff
@@ -1,361 +1,276 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "4e9bf3f9-0952-493c-a8df-4a1d851c37a9",
+            "id": "0",
             "metadata": {},
             "source": [
-                "# Strategies for climatology calculations\n",
+                "# Custom Aggregations\n",
                 "\n",
-                "This notebook is motivated by\n",
-                "[this post](https://discourse.pangeo.io/t/understanding-optimal-zarr-chunking-scheme-for-a-climatology/2335)\n",
-                "on the Pangeo discourse forum.\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "85ac0588-ff00-43cc-b952-7ab775b24e4a",
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "import dask.array\n",
-                "import pandas as pd\n",
-                "import xarray as xr\n",
+                "This notebook is motivated by a\n",
+                "[post](https://discourse.pangeo.io/t/using-xhistogram-to-bin-measurements-at-particular-stations/2365/4)\n",
+                "on the Pangeo discourse forum.\n",
                 "\n",
-                "import flox\n",
-                "import flox.xarray"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "82f46621-1b6c-4a14-ac0f-3aa5121dad54",
-            "metadata": {},
-            "source": [
-                "Let's first create an example Xarray Dataset representing the OISST dataset,\n",
-                "with chunk sizes matching that in the post.\n"
+                "> Even better would be a command that lets me simply do the following.\n",
+                ">\n",
+                ">     A = da.groupby(['lon_bins', 'lat_bins']).mode()\n",
+                "\n",
+                "This notebook will describe how to accomplish this using a custom `Aggregation`.\n",
+                "\n",
+                "\n",
+                "```{tip}\n",
+                "flox now supports `mode`, `nanmode`, `quantile`, `nanquantile`, `median`, `nanmedian` using exactly the same \n",
+                "approach as shown below\n",
+                "```\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9a91d2e2-bd6d-4b35-8002-5fac76c4c5b3",
+            "id": "1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "oisst = xr.DataArray(\n",
-                "    dask.array.ones((14532, 720, 1440), chunks=(20, -1, -1)),\n",
-                "    dims=(\"time\", \"lat\", \"lon\"),\n",
-                "    coords={\"time\": pd.date_range(\"1981-09-01 12:00\", \"2021-06-14 12:00\", freq=\"D\")},\n",
-                "    name=\"sst\",\n",
+                "import numpy as np\n",
+                "import numpy_groupies as npg\n",
+                "import xarray as xr\n",
+                "\n",
+                "import flox.xarray\n",
+                "from flox import Aggregation\n",
+                "from flox.aggregations import mean\n",
+                "\n",
+                "# define latitude and longitude bins\n",
+                "binsize = 1.0  # 1\u00b0x1\u00b0 bins\n",
+                "lon_min, lon_max, lat_min, lat_max = [-180, 180, -65, 65]\n",
+                "lon_bins = np.arange(lon_min, lon_max, binsize)\n",
+                "lat_bins = np.arange(lat_min, lat_max, binsize)\n",
+                "\n",
+                "size = 28397\n",
+                "\n",
+                "\n",
+                "da = xr.DataArray(\n",
+                "    np.random.randint(0, 7, size=size),\n",
+                "    dims=\"profile\",\n",
+                "    coords={\n",
+                "        \"lat\": (\n",
+                "            \"profile\",\n",
+                "            (np.random.random(size) - 0.5) * (lat_max - lat_min),\n",
+                "        ),\n",
+                "        \"lon\": (\n",
+                "            \"profile\",\n",
+                "            (np.random.random(size) - 0.5) * (lon_max - lon_min),\n",
+                "        ),\n",
+                "    },\n",
+                "    name=\"label\",\n",
                 ")\n",
-                "oisst"
+                "da"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b7f519ee-e575-492c-a70b-8dad63a8c222",
+            "id": "2",
             "metadata": {},
             "source": [
-                "To account for Feb-29 being present in some years, we'll construct a time vector to group by as \"mmm-dd\" string.\n",
+                "## A built-in reduction\n",
                 "\n",
-                "For more options, see https://strftime.org/"
+                "First a simple example of lat-lon binning using a built-in reduction: mean\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3c42a618-47bc-4c83-a902-ec4cf3420180",
+            "id": "3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "day = oisst.time.dt.strftime(\"%h-%d\").rename(\"day\")\n",
-                "day"
+                "binned_mean = flox.xarray.xarray_reduce(\n",
+                "    da,\n",
+                "    da.lat,\n",
+                "    da.lon,\n",
+                "    func=\"mean\",  # built-in\n",
+                "    expected_groups=(lat_bins, lon_bins),\n",
+                "    isbin=(True, True),\n",
+                ")\n",
+                "binned_mean.plot()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "6d913e7f-25bd-43c4-98b6-93bcb420c524",
+            "id": "4",
             "metadata": {},
             "source": [
-                "## map-reduce\n",
+                "## Aggregations\n",
                 "\n",
-                "The default\n",
-                "[method=\"map-reduce\"](https://flox.readthedocs.io/en/latest/implementation.html#method-map-reduce)\n",
-                "doesn't work so well. We aggregate all days in a single ~3GB chunk.\n",
+                "flox knows how to interperet `func=\"mean\"` because it's been implemented in\n",
+                "`aggregations.py` as an\n",
+                "[Aggregation](https://flox.readthedocs.io/en/latest/generated/flox.aggregations.Aggregation.html)\n",
                 "\n",
-                "For this to work well, we'd want smaller chunks in space and bigger chunks in\n",
-                "time.\n"
+                "An `Aggregation` is a blueprint for computing an aggregation, with both numpy\n",
+                "and dask data.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ef2a14de-7526-40e3-8a97-28e84d6d6f20",
+            "id": "5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "flox.xarray.xarray_reduce(\n",
-                "    oisst,\n",
-                "    day,\n",
-                "    func=\"mean\",\n",
-                "    method=\"map-reduce\",\n",
-                ")"
+                "print(type(mean))\n",
+                "mean"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "442ad701-ea45-4555-9550-ec9daecfbea3",
+            "id": "6",
             "metadata": {},
             "source": [
-                "## Rechunking for map-reduce\n",
+                "Here's how the mean Aggregation is created\n",
                 "\n",
-                "We can split each chunk along the `lat`, `lon` dimensions to make sure the\n",
-                "output chunk sizes are more reasonable\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "322c7776-9a21-4115-8ac9-9c7c6c6e2c91",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "flox.xarray.xarray_reduce(\n",
-                "    oisst.chunk({\"lat\": -1, \"lon\": 120}),\n",
-                "    day,\n",
-                "    func=\"mean\",\n",
-                "    method=\"map-reduce\",\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "833f72eb-1501-4362-ae55-ec419c9f0ac1",
-            "metadata": {},
-            "source": [
-                "But what if we didn't want to rechunk the dataset so drastically (note the 10x\n",
-                "increase in tasks). For that let's try `method=\"cohorts\"`\n",
+                "```python\n",
+                "mean = Aggregation(\n",
+                "    name=\"mean\",\n",
                 "\n",
-                "## method=cohorts\n",
+                "    # strings in the following are built-in grouped reductions\n",
+                "    # implemented by the underlying  \"engine\": flox or numpy_groupies or numbagg\n",
                 "\n",
-                "We can take advantage of patterns in the groups here \"day of year\".\n",
-                "Specifically:\n",
+                "    # for pure  numpy inputs\n",
+                "    numpy=\"mean\",\n",
                 "\n",
-                "1. The groups at an approximately periodic interval, 365 or 366 days\n",
-                "2. The chunk size 20 is smaller than the period of 365 or 366. This means, that\n",
-                "   to construct the mean for days 1-20, we just need to use the chunks that\n",
-                "   contain days 1-20.\n",
-                "\n",
-                "This strategy is implemented as\n",
-                "[method=\"cohorts\"](https://flox.readthedocs.io/en/latest/implementation.html#method-cohorts)\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "a3bafc32-7e13-41b8-90eb-b27955393392",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "flox.xarray.xarray_reduce(\n",
-                "    oisst,\n",
-                "    day,\n",
-                "    func=\"mean\",\n",
-                "    method=\"cohorts\",\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "b4e1ba0b-20e5-466a-9199-38b47029a0ed",
-            "metadata": {},
-            "source": [
-                "By default cohorts doesn't work so well for this problem because the period\n",
-                "isn't regular (365 vs 366) and the period isn't divisible by the chunk size. So\n",
-                "the groups end up being \"out of phase\" (for a visual illustration\n",
-                "[click here](https://flox.readthedocs.io/en/latest/implementation.html#method-cohorts)).\n",
-                "Now we have the opposite problem: the chunk sizes on the output are too small.\n",
+                "    # The next are for dask inputs and describe how to reduce\n",
+                "    # the data in parallel\n",
+                "    chunk=(\"sum\", \"nanlen\"), # first compute these blockwise : (grouped_sum, grouped_count)\n",
+                "    combine=(\"sum\", \"sum\"), #  reduce intermediate results (sum the sums, sum the counts)\n",
+                "    finalize=lambda sum_, count: sum_ / count, # final mean value (divide sum by count)\n",
                 "\n",
-                "Let us inspect the cohorts"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "13ce5531-0d6c-4c89-bc44-dc2c24fa4e47",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# integer codes for each \"day\"\n",
-                "codes, _ = pd.factorize(day.data)\n",
-                "preferred_method, cohorts = flox.core.find_group_cohorts(\n",
-                "    labels=codes,\n",
-                "    chunks=(oisst.chunksizes[\"time\"],),\n",
+                "    fill_value=(0, 0),  # fill value for intermediate  sums and counts when groups have no members\n",
+                "    dtypes=(None, np.intp),  # optional dtypes for intermediates\n",
+                "    final_dtype=np.floating,  # final dtype for output\n",
                 ")\n",
-                "print(len(cohorts))"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "068b4109-b7f4-4c16-918d-9a18ff2ed183",
-            "metadata": {},
-            "source": [
-                "Looking more closely, we can see many cohorts with a single entry. "
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "57983cd0-a2e0-4d16-abe6-9572f6f252bf",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "cohorts.values()"
+                "```\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "bcbdbb3b-2aed-4f3f-ad20-efabb52b5e68",
+            "id": "7",
             "metadata": {},
             "source": [
-                "## Rechunking data for cohorts\n",
+                "## Defining a custom aggregation\n",
                 "\n",
-                "Can we fix the \"out of phase\" problem by rechunking along time?\n",
+                "First we'll need a function that executes the grouped reduction given numpy\n",
+                "inputs.\n",
                 "\n",
-                "First lets see where the current chunk boundaries are"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "40d393a5-7a4e-4d33-997b-4c422a0b8100",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "oisst.chunksizes[\"time\"][:10]"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "cd0033a3-d211-4aef-a284-c9fd3f75f6e4",
-            "metadata": {},
-            "source": [
-                "We'll choose to rechunk such that a single month in is a chunk. This is not too different from the current chunking but will help your periodicity problem"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "5914a350-a7db-49b3-9504-6d63ff874f5e",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "newchunks = xr.ones_like(day).astype(int).resample(time=\"M\").count()"
+                "Custom functions are required to have this signature (copied form\n",
+                "numpy_groupies):\n",
+                "\n",
+                "```python\n",
+                "\n",
+                "def custom_grouped_reduction(\n",
+                "    group_idx, array, *, axis=-1, size=None, fill_value=None, dtype=None\n",
+                "):\n",
+                "    \"\"\"\n",
+                "    Parameters\n",
+                "    ----------\n",
+                "\n",
+                "    group_idx : np.ndarray, 1D\n",
+                "        integer codes for group labels (1D)\n",
+                "    array : np.ndarray, nD\n",
+                "        values to reduce (nD)\n",
+                "    axis : int\n",
+                "        axis of array along which to reduce. Requires array.shape[axis] == len(group_idx)\n",
+                "    size : int, optional\n",
+                "        expected number of groups. If none, output.shape[-1] == number of uniques in group_idx\n",
+                "    fill_value : optional\n",
+                "        fill_value for when number groups in group_idx is less than size\n",
+                "    dtype : optional\n",
+                "        dtype of output\n",
+                "\n",
+                "    Returns\n",
+                "    -------\n",
+                "\n",
+                "    np.ndarray with array.shape[-1] == size, containing a single value per group\n",
+                "    \"\"\"\n",
+                "    pass\n",
+                "```\n",
+                "\n",
+                "Since numpy_groupies does not implement a median, we'll do it ourselves by\n",
+                "passing `np.median` to `numpy_groupies.aggregate_numpy.aggregate`. This will\n",
+                "loop over all groups, and then execute `np.median` on the group members in\n",
+                "serial. It is not fast, but quite convenient.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "90a884bc-1b71-4874-8143-73b3b5c41458",
+            "id": "8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "rechunked = oisst.chunk(time=tuple(newchunks.data))"
+                "def grouped_median(group_idx, array, *, axis=-1, size=None, fill_value=None, dtype=None):\n",
+                "    return npg.aggregate_numpy.aggregate(\n",
+                "        group_idx,\n",
+                "        array,\n",
+                "        func=np.median,\n",
+                "        axis=axis,\n",
+                "        size=size,\n",
+                "        fill_value=fill_value,\n",
+                "        dtype=dtype,\n",
+                "    )"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "12b7a27f-ebab-4673-bb9f-80620389994b",
+            "id": "9",
             "metadata": {},
             "source": [
-                "And now our cohorts contain more than one group\n"
+                "Now we create the `Aggregation`\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f522fb82-764d-4e4e-8337-a5123e3088f8",
+            "id": "10",
             "metadata": {},
             "outputs": [],
             "source": [
-                "preferrd_method, new_cohorts = flox.core.find_group_cohorts(\n",
-                "    labels=codes,\n",
-                "    chunks=(rechunked.chunksizes[\"time\"],),\n",
+                "agg_median = Aggregation(\n",
+                "    name=\"median\",\n",
+                "    numpy=grouped_median,\n",
+                "    fill_value=-1,\n",
+                "    chunk=None,\n",
+                "    combine=None,\n",
                 ")\n",
-                "# one cohort per month!\n",
-                "len(new_cohorts)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "4e2b6f70-c057-4783-ad55-21b20ff27e7f",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "new_cohorts.values()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "949ac39c-dd84-4375-a884-0c1c3c382a8f",
-            "metadata": {},
-            "source": [
-                "Now the groupby reduction **looks OK** in terms of number of tasks but remember\n",
-                "that rechunking to get to this point involves some communication overhead.\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "8f1e45f9-5b18-482a-8c76-66f81ff5710f",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "flox.xarray.xarray_reduce(rechunked, day, func=\"mean\", method=\"cohorts\")"
+                "agg_median"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "93c58969-5c99-4bc0-90ee-9cef468bf78b",
+            "id": "11",
             "metadata": {},
             "source": [
-                "## How about other climatologies?\n",
-                "\n",
-                "Let's try monthly\n"
+                "And apply it!\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e559ea33-5499-48ff-9a2e-5141c3a69fea",
+            "id": "12",
             "metadata": {},
             "outputs": [],
             "source": [
-                "flox.xarray.xarray_reduce(oisst, oisst.time.dt.month, func=\"mean\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "a00de8eb-e414-4920-8dcd-b64afbf91b62",
-            "metadata": {},
-            "source": [
-                "This looks great. Why?\n",
-                "\n",
-                "It's because each chunk (size 20) is smaller than number of days in a typical\n",
-                "month. `flox` initially applies the groupby-reduction blockwise. For the chunk\n",
-                "size of 20, we will have at most 2 groups in each chunk, so the initial\n",
-                "blockwise reduction is quite effective - at least a 10x reduction in size from\n",
-                "20 elements in time to at most 2 elements in time.\n",
-                "\n",
-                "For this kind of problem, `\"map-reduce\"` works quite well.\n"
+                "flox.xarray.xarray_reduce(\n",
+                "    da,\n",
+                "    da.lat,\n",
+                "    da.lon,\n",
+                "    func=agg_median,\n",
+                "    expected_groups=(lat_bins, lon_bins),\n",
+                "    isbin=(True, True),\n",
+                "    fill_value=np.nan,\n",
+                ")"
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
```

### Comparing `flox-0.9.6/docs/source/user-stories/hourly-climatology.html` & `flox-0.9.7/docs/source/user-stories/hourly-climatology.html`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/source/user-stories/nD-bins.ipynb` & `flox-0.9.7/docs/source/user-stories/nD-bins.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868551587301587%*

 * *Differences: {"'cells'": "{0: {'id': '0'}, 1: {'id': '1'}, 2: {'id': '2'}, 3: {'id': '3'}, 4: {'id': '4'}, 5: "*

 * *            "{'id': '5'}, 6: {'id': '6'}, 7: {'id': '7'}, 8: {'id': '8'}, 9: {'id': '9'}, 10: "*

 * *            "{'id': '10'}, 11: {'id': '11'}, 12: {'id': '12'}, 13: {'id': '13'}, 14: {'id': '14'}, "*

 * *            "15: {'id': '15'}, 16: {'id': '16'}, 17: {'id': '17'}, 18: {'id': '18'}, 19: {'id': "*

 * *            "'19'}, 20: {'id': '20'}}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "e970d800-c612-482a-bb3a-b1eb7ad53d88",
+            "id": "0",
             "metadata": {
                 "tags": [],
                 "user_expressions": []
             },
             "source": [
                 "# Binning with multi-dimensional bins\n",
                 "\n",
@@ -24,15 +24,15 @@
                 "> (`forecast_with_lon_lat_time_dims.quantile(q=[.33,.66],dim='time')`) depend on\n",
                 "> `lon` and `lat`.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "01f1a2ef-de62-45d0-a04e-343cd78debc5",
+            "id": "1",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import math\n",
                 "\n",
@@ -42,36 +42,36 @@
                 "\n",
                 "import flox\n",
                 "import flox.xarray"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0be3e214-0cf0-426f-8ebb-669cc5322310",
+            "id": "2",
             "metadata": {
                 "user_expressions": []
             },
             "source": [
                 "## Create test data\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "ce239000-e053-4fc3-ad14-e9e0160da869",
+            "id": "3",
             "metadata": {
                 "user_expressions": []
             },
             "source": [
                 "Data to be reduced\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7659c24e-f5a1-4e59-84c0-5ec965ef92d2",
+            "id": "4",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "array = xr.DataArray(\n",
                 "    np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12]]),\n",
@@ -79,26 +79,26 @@
                 "    name=\"array\",\n",
                 ")\n",
                 "array"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "da0c0ac9-ad75-42cd-a1ea-99069f5bef00",
+            "id": "5",
             "metadata": {
                 "user_expressions": []
             },
             "source": [
                 "Array to group by\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4601e744-5d22-447e-97ce-9644198d485e",
+            "id": "6",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "by = xr.DataArray(\n",
                 "    np.array([[1, 2, 3], [3, 4, 5], [5, 6, 7], [6, 7, 9]]),\n",
@@ -106,27 +106,27 @@
                 "    name=\"by\",\n",
                 ")\n",
                 "by"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "61c21c94-7b6e-46a6-b9c2-59d7b2d40c81",
+            "id": "7",
             "metadata": {
                 "tags": [],
                 "user_expressions": []
             },
             "source": [
                 "Multidimensional bins:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "863a1991-ab8d-47c0-aa48-22b422fcea8c",
+            "id": "8",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "bins = by + 0.5\n",
                 "bins = xr.DataArray(\n",
@@ -135,15 +135,15 @@
                 "    name=\"bins\",\n",
                 ")\n",
                 "bins"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e65ecaba-d1cc-4485-ae58-c390cb2ebfab",
+            "id": "9",
             "metadata": {
                 "user_expressions": []
             },
             "source": [
                 "## Concept\n",
                 "\n",
                 "The key idea is that GroupBy is two steps:\n",
@@ -170,27 +170,27 @@
                 "The core `factorize_` function (which wraps `pd.cut`) only handles 1D bins, so\n",
                 "we use `xr.apply_ufunc` to vectorize it for us.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "aa33ab2c-0ecf-4198-a033-2a77f5d83c99",
+            "id": "10",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "factorize_loop_dim = \"time\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "afcddcc1-dd57-461e-a649-1f8bcd30342f",
+            "id": "11",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "def factorize_nd_bins_core(by, bins):\n",
                 "    group_idx, *_, props = flox.core.factorize_(\n",
@@ -213,15 +213,15 @@
                 "    vectorize=True,\n",
                 ")\n",
                 "codes"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1661312a-dc61-4a26-bfd8-12c2dc01eb15",
+            "id": "12",
             "metadata": {
                 "user_expressions": []
             },
             "source": [
                 "### Offset the codes\n",
                 "\n",
                 "These are integer codes appropriate for a single timestep.\n",
@@ -230,15 +230,15 @@
                 "different from \"bin 0\" for `time=1` (taken from\n",
                 "[this StackOverflow thread](https://stackoverflow.com/questions/46256279/bin-elements-per-row-vectorized-2d-bincount-for-numpy)).\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0e5801cb-a79c-4670-ad10-36bb19f1a6ff",
+            "id": "13",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "N = math.prod([codes.sizes[d] for d in codes.dims if d != factorize_loop_dim])\n",
                 "offset = xr.DataArray(np.arange(codes.sizes[factorize_loop_dim]), dims=factorize_loop_dim)\n",
@@ -246,28 +246,28 @@
                 "offset_codes = (codes + offset * (N - 1)).rename(by.name)\n",
                 "offset_codes.data[codes == -1] = -1\n",
                 "offset_codes"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "6c06c48b-316b-4a33-9bc3-921acd10bcba",
+            "id": "14",
             "metadata": {
                 "user_expressions": []
             },
             "source": [
                 "### Reduce\n",
                 "\n",
                 "Now that we have appropriate codes, let's apply the reduction\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2cf1295e-4585-48b9-ac2b-9e00d03b2b9a",
+            "id": "15",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "interim = flox.xarray.xarray_reduce(\n",
                 "    array,\n",
@@ -279,28 +279,28 @@
                 "    expected_groups=pd.RangeIndex(9),\n",
                 ")\n",
                 "interim"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3539509b-d9b4-4342-a679-6ada6f285dfb",
+            "id": "16",
             "metadata": {
                 "user_expressions": []
             },
             "source": [
                 "## Make final result\n",
                 "\n",
                 "Now reshape that 1D result appropriately.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b1389d37-d76d-4a50-9dfb-8710258de3fd",
+            "id": "17",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "final = (\n",
                 "    interim.coarsen(by=3)\n",
@@ -312,37 +312,37 @@
                 "    .drop_vars(\"by\")\n",
                 ")\n",
                 "final"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a98b5e60-94af-45ae-be1b-4cb47e2d77ba",
+            "id": "18",
             "metadata": {
                 "user_expressions": []
             },
             "source": [
                 "I think this is the expected answer.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "053a8643-f6d9-4fd1-b014-230fa716449c",
+            "id": "19",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "array.isel(space=slice(1, None)).rename({\"space\": \"bin_number\"}).identical(final)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "619ba4c4-7c87-459a-ab86-c187d3a86c67",
+            "id": "20",
             "metadata": {
                 "tags": [],
                 "user_expressions": []
             },
             "source": [
                 "## TODO\n",
                 "\n",
```

### Comparing `flox-0.9.6/docs/source/user-stories/overlaps.md` & `flox-0.9.7/docs/source/user-stories/overlaps.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/docs/source/xarray.md` & `flox-0.9.7/docs/source/xarray.md`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/flox/aggregate_flox.py` & `flox-0.9.7/flox/aggregate_flox.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/flox/aggregate_npg.py` & `flox-0.9.7/flox/aggregate_npg.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/flox/aggregate_numbagg.py` & `flox-0.9.7/flox/aggregate_numbagg.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/flox/aggregations.py` & `flox-0.9.7/flox/aggregations.py`

 * *Files 0% similar despite different names*

```diff
@@ -619,17 +619,19 @@
 
     final_dtype = _normalize_dtype(dtype_ or agg.dtype_init["final"], array_dtype, fill_value)
     agg.dtype = {
         "user": dtype,  # Save to automatically choose an engine
         "final": final_dtype,
         "numpy": (final_dtype,),
         "intermediate": tuple(
-            _normalize_dtype(int_dtype, np.result_type(array_dtype, final_dtype), int_fv)
-            if int_dtype is None
-            else np.dtype(int_dtype)
+            (
+                _normalize_dtype(int_dtype, np.result_type(array_dtype, final_dtype), int_fv)
+                if int_dtype is None
+                else np.dtype(int_dtype)
+            )
             for int_dtype, int_fv in zip(
                 agg.dtype_init["intermediate"], agg.fill_value["intermediate"]
             )
         ),
     }
 
     # Replace sentinel fill values according to dtype
```

### Comparing `flox-0.9.6/flox/core.py` & `flox-0.9.7/flox/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 import logging
 import math
 import operator
 import sys
 import warnings
 from collections import namedtuple
 from collections.abc import Sequence
+from concurrent.futures import ThreadPoolExecutor
 from functools import partial, reduce
 from itertools import product
 from numbers import Integral
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Literal,
     TypedDict,
+    TypeVar,
     Union,
     overload,
 )
 
 import numpy as np
 import numpy_groupies as npg
 import pandas as pd
@@ -34,15 +36,17 @@
     _atleast_1d,
     _initialize_aggregation,
     generic_aggregate,
     quantile_new_dims_func,
 )
 from .cache import memoize
 from .xrutils import (
+    is_chunked_array,
     is_duck_array,
+    is_duck_cubed_array,
     is_duck_dask_array,
     isnull,
     module_available,
     notnull,
 )
 
 if module_available("numpy", minversion="2.0.0"):
@@ -59,18 +63,19 @@
         if sys.version_info < (3, 11):
             from typing_extensions import Unpack
         else:
             from typing import Unpack
     except (ModuleNotFoundError, ImportError):
         Unpack: Any  # type: ignore[no-redef]
 
+    import cubed.Array as CubedArray
     import dask.array.Array as DaskArray
     from dask.typing import Graph
 
-    T_DuckArray = Union[np.ndarray, DaskArray]  # Any ?
+    T_DuckArray = Union[np.ndarray, DaskArray, CubedArray]  # Any ?
     T_By = T_DuckArray
     T_Bys = tuple[T_By, ...]
     T_ExpectIndex = pd.Index
     T_ExpectIndexTuple = tuple[T_ExpectIndex, ...]
     T_ExpectIndexOpt = Union[T_ExpectIndex, None]
     T_ExpectIndexOptTuple = tuple[T_ExpectIndexOpt, ...]
     T_Expect = Union[Sequence, np.ndarray, T_ExpectIndex]
@@ -89,17 +94,18 @@
     T_FillValues = Union[np.typing.ArrayLike, Sequence[np.typing.ArrayLike], None]
     T_Engine = Literal["flox", "numpy", "numba", "numbagg"]
     T_EngineOpt = None | T_Engine
     T_Method = Literal["map-reduce", "blockwise", "cohorts"]
     T_MethodOpt = None | Literal["map-reduce", "blockwise", "cohorts"]
     T_IsBins = Union[bool | Sequence[bool]]
 
+T = TypeVar("T")
 
 IntermediateDict = dict[Union[str, Callable], Any]
-FinalResultsDict = dict[str, Union["DaskArray", np.ndarray]]
+FinalResultsDict = dict[str, Union["DaskArray", "CubedArray", np.ndarray]]
 FactorProps = namedtuple("FactorProps", "offset_group nan_sentinel nanmask")
 
 # This dummy axis is inserted using np.expand_dims
 # and then reduced over during the combine stage by
 # _simple_combine.
 DUMMY_AXIS = -2
 
@@ -133,14 +139,18 @@
     if needs_masking:
         mask = np.isin(groups, seen_groups, assume_unique=True, invert=True)
         if mask.any():
             result[..., groups[mask]] = fill_value
     return result
 
 
+def identity(x: T) -> T:
+    return x
+
+
 def _issorted(arr: np.ndarray) -> bool:
     return bool((arr[:-1] <= arr[1:]).all())
 
 
 def _is_arg_reduction(func: T_Agg) -> bool:
     if isinstance(func, str) and func in ["argmin", "argmax", "nanargmax", "nanargmin"]:
         return True
@@ -241,42 +251,85 @@
         (slice(s, s + dim) for s, dim in zip(starts, shapes))
         for starts, shapes in zip(cumdims, chunks)
     )
     return product(*slices)
 
 
 def _compute_label_chunk_bitmask(labels, chunks, nlabels):
+    def make_bitmask(rows, cols):
+        data = np.broadcast_to(np.array(1, dtype=np.uint8), rows.shape)
+        return csc_array((data, (rows, cols)), dtype=bool, shape=(nchunks, nlabels))
+
     assert isinstance(labels, np.ndarray)
     shape = tuple(sum(c) for c in chunks)
     nchunks = math.prod(len(c) for c in chunks)
+    approx_chunk_size = math.prod(c[0] for c in chunks)
 
-    labels = np.broadcast_to(labels, shape[-labels.ndim :])
+    # Shortcut for 1D with size-1 chunks
+    if shape == (nchunks,):
+        rows_array = np.arange(nchunks)
+        cols_array = labels
+        mask = labels >= 0
+        return make_bitmask(rows_array[mask], cols_array[mask])
 
+    labels = np.broadcast_to(labels, shape[-labels.ndim :])
     cols = []
-    # Add one to handle the -1 sentinel value
-    label_is_present = np.zeros((nlabels + 1,), dtype=bool)
     ilabels = np.arange(nlabels)
-    for region in slices_from_chunks(chunks):
+
+    def chunk_unique(labels, slicer, nlabels, label_is_present=None):
+        if label_is_present is None:
+            label_is_present = np.empty((nlabels + 1,), dtype=bool)
+        label_is_present[:] = False
+        subset = labels[slicer]
         # This is a quite fast way to find unique integers, when we know how many there are
         # inspired by a similar idea in numpy_groupies for first, last
         # instead of explicitly finding uniques, repeatedly write True to the same location
-        subset = labels[region]
-        # The reshape is not strictly necessary but is about 100ms faster on a test problem.
         label_is_present[subset.reshape(-1)] = True
         # skip the -1 sentinel by slicing
         # Faster than np.argwhere by a lot
         uniques = ilabels[label_is_present[:-1]]
-        cols.append(uniques)
-        label_is_present[:] = False
+        return uniques
+
+    # TODO: refine this heuristic.
+    # The general idea is that with the threadpool, we repeatedly allocate memory
+    # for `label_is_present`. We trade that off against the parallelism across number of chunks.
+    # For large enough number of chunks (relative to number of labels), it makes sense to
+    # suffer the extra allocation in exchange for parallelism.
+    THRESHOLD = 2
+    if nlabels < THRESHOLD * approx_chunk_size:
+        logger.debug(
+            "Using threadpool since num_labels %s < %d * chunksize %s",
+            nlabels,
+            THRESHOLD,
+            approx_chunk_size,
+        )
+        with ThreadPoolExecutor() as executor:
+            futures = [
+                executor.submit(chunk_unique, labels, slicer, nlabels)
+                for slicer in slices_from_chunks(chunks)
+            ]
+            cols = tuple(f.result() for f in futures)
+
+    else:
+        logger.debug(
+            "Using serial loop since num_labels %s > %d * chunksize %s",
+            nlabels,
+            THRESHOLD,
+            approx_chunk_size,
+        )
+        cols = []
+        # Add one to handle the -1 sentinel value
+        label_is_present = np.empty((nlabels + 1,), dtype=bool)
+        for region in slices_from_chunks(chunks):
+            uniques = chunk_unique(labels, region, nlabels, label_is_present)
+            cols.append(uniques)
     rows_array = np.repeat(np.arange(nchunks), tuple(len(col) for col in cols))
     cols_array = np.concatenate(cols)
-    data = np.broadcast_to(np.array(1, dtype=np.uint8), rows_array.shape)
-    bitmask = csc_array((data, (rows_array, cols_array)), dtype=bool, shape=(nchunks, nlabels))
 
-    return bitmask
+    return make_bitmask(rows_array, cols_array)
 
 
 # @memoize
 def find_group_cohorts(
     labels, chunks, expected_groups: None | pd.RangeIndex = None, merge: bool = False
 ) -> tuple[T_Method, dict]:
     """
@@ -305,21 +358,26 @@
     cohorts: dict_values
         Iterable of cohorts
     """
     # To do this, we must have values in memory so casting to numpy should be safe
     labels = np.asarray(labels)
 
     shape = tuple(sum(c) for c in chunks)
+    nchunks = math.prod(len(c) for c in chunks)
 
     # assumes that `labels` are factorized
     if expected_groups is None:
         nlabels = labels.max() + 1
     else:
         nlabels = expected_groups[-1] + 1
 
+    # 1. Single chunk, blockwise always
+    if nchunks == 1:
+        return "blockwise", {(0,): list(range(nlabels))}
+
     labels = np.broadcast_to(labels, shape[-labels.ndim :])
     bitmask = _compute_label_chunk_bitmask(labels, chunks, nlabels)
 
     CHUNK_AXIS, LABEL_AXIS = 0, 1
     chunks_per_label = bitmask.sum(axis=CHUNK_AXIS)
 
     # can happen when `expected_groups` is passed but not all labels are present
@@ -339,29 +397,29 @@
     # Invert the label_chunks mapping so we know which labels occur together.
     def invert(x) -> tuple[np.ndarray, ...]:
         arr = label_chunks[x]
         return tuple(arr)
 
     chunks_cohorts = tlz.groupby(invert, label_chunks.keys())
 
-    # 1. Every group is contained to one block, use blockwise here.
+    # 2. Every group is contained to one block, use blockwise here.
     if bitmask.shape[CHUNK_AXIS] == 1 or (chunks_per_label == 1).all():
         logger.info("find_group_cohorts: blockwise is preferred.")
         return "blockwise", chunks_cohorts
 
-    # 2. Perfectly chunked so there is only a single cohort
+    # 3. Perfectly chunked so there is only a single cohort
     if len(chunks_cohorts) == 1:
         logger.info("Only found a single cohort. 'map-reduce' is preferred.")
         return "map-reduce", chunks_cohorts if merge else {}
 
-    # 3. Our dataset has chunksize one along the axis,
+    # 4. Our dataset has chunksize one along the axis,
     single_chunks = all(all(a == 1 for a in ac) for ac in chunks)
-    # 4. Every chunk only has a single group, but that group might extend across multiple chunks
+    # 5. Every chunk only has a single group, but that group might extend across multiple chunks
     one_group_per_chunk = (bitmask.sum(axis=LABEL_AXIS) == 1).all()
-    # 5. Existing cohorts don't overlap, great for time grouping with perfect chunking
+    # 6. Existing cohorts don't overlap, great for time grouping with perfect chunking
     no_overlapping_cohorts = (np.bincount(np.concatenate(tuple(chunks_cohorts.keys()))) == 1).all()
     if one_group_per_chunk or single_chunks or no_overlapping_cohorts:
         logger.info("find_group_cohorts: cohorts is preferred, chunking is perfect.")
         return "cohorts", chunks_cohorts
 
     # We'll use containment to measure degree of overlap between labels.
     # Containment C = |Q & S| / |Q|
@@ -386,14 +444,15 @@
     sparsity = bitmask.nnz / math.prod(bitmask.shape)
     preferred_method: Literal["map-reduce"] | Literal["cohorts"]
     logger.debug(
         "sparsity of bitmask is {}, threshold is {}".format(  # noqa
             sparsity, MAX_SPARSITY_FOR_COHORTS
         )
     )
+    # 7. Groups seem fairly randomly distributed, use "map-reduce".
     if sparsity > MAX_SPARSITY_FOR_COHORTS:
         if not merge:
             logger.info(
                 "find_group_cohorts: bitmask sparsity={}, merge=False, choosing 'map-reduce'".format(  # noqa
                     sparsity
                 )
             )
@@ -650,42 +709,39 @@
     by: T_Bys,
     axes: T_Axes,
     *,
     fastpath: Literal[True],
     expected_groups: T_ExpectIndexOptTuple | None = None,
     reindex: bool = False,
     sort: bool = True,
-) -> tuple[np.ndarray, tuple[np.ndarray, ...], tuple[int, ...], int, int, None]:
-    ...
+) -> tuple[np.ndarray, tuple[np.ndarray, ...], tuple[int, ...], int, int, None]: ...
 
 
 @overload
 def factorize_(
     by: T_Bys,
     axes: T_Axes,
     *,
     expected_groups: T_ExpectIndexOptTuple | None = None,
     reindex: bool = False,
     sort: bool = True,
     fastpath: Literal[False] = False,
-) -> tuple[np.ndarray, tuple[np.ndarray, ...], tuple[int, ...], int, int, FactorProps]:
-    ...
+) -> tuple[np.ndarray, tuple[np.ndarray, ...], tuple[int, ...], int, int, FactorProps]: ...
 
 
 @overload
 def factorize_(
     by: T_Bys,
     axes: T_Axes,
     *,
     expected_groups: T_ExpectIndexOptTuple | None = None,
     reindex: bool = False,
     sort: bool = True,
     fastpath: bool = False,
-) -> tuple[np.ndarray, tuple[np.ndarray, ...], tuple[int, ...], int, int, FactorProps | None]:
-    ...
+) -> tuple[np.ndarray, tuple[np.ndarray, ...], tuple[int, ...], int, int, FactorProps | None]: ...
 
 
 def factorize_(
     by: T_Bys,
     axes: T_Axes,
     *,
     expected_groups: T_ExpectIndexOptTuple | None = None,
@@ -1420,15 +1476,18 @@
 
     full_tuple = tuple(i if ax not in mesh else mesh[ax] for ax, i in enumerate(noiter))
 
     return full_tuple
 
 
 def subset_to_blocks(
-    array: DaskArray, flatblocks: Sequence[int], blkshape: tuple[int] | None = None
+    array: DaskArray,
+    flatblocks: Sequence[int],
+    blkshape: tuple[int] | None = None,
+    reindexer=identity,
 ) -> DaskArray:
     """
     Advanced indexing of .blocks such that we always get a regular array back.
 
     Parameters
     ----------
     array : dask.array
@@ -1446,28 +1505,29 @@
 
     if blkshape is None:
         blkshape = array.blocks.shape
 
     index = _normalize_indexes(array, flatblocks, blkshape)
 
     if all(not isinstance(i, np.ndarray) and i == slice(None) for i in index):
-        return array
+        return dask.array.map_blocks(reindexer, array, meta=array._meta)
 
     # These rest is copied from dask.array.core.py with slight modifications
     index = normalize_index(index, array.numblocks)
     index = tuple(slice(k, k + 1) if isinstance(k, Integral) else k for k in index)
 
-    name = "blocks-" + tokenize(array, index)
+    name = "groupby-cohort-" + tokenize(array, index)
     new_keys = array._key_array[index]
 
     squeezed = tuple(np.squeeze(i) if isinstance(i, np.ndarray) else i for i in index)
     chunks = tuple(tuple(np.array(c)[i].tolist()) for c, i in zip(array.chunks, squeezed))
 
     keys = itertools.product(*(range(len(c)) for c in chunks))
-    layer: Graph = {(name,) + key: tuple(new_keys[key].tolist()) for key in keys}
+    layer: Graph = {(name,) + key: (reindexer, tuple(new_keys[key].tolist())) for key in keys}
+
     graph = HighLevelGraph.from_collections(name, layer, dependencies=[array])
 
     return dask.array.Array(graph, name, chunks, meta=array)
 
 
 def _extract_unknown_groups(reduced, dtype) -> tuple[DaskArray]:
     import dask.array
@@ -1633,34 +1693,34 @@
             else:
                 assert expected_groups is not None
                 groups = (expected_groups.to_numpy(),)
                 group_chunks = ((len(expected_groups),),)
 
         elif method == "cohorts":
             assert chunks_cohorts
+            block_shape = array.blocks.shape[-len(axis) :]
+
             reduced_ = []
             groups_ = []
             for blks, cohort in chunks_cohorts.items():
-                index = pd.Index(cohort)
-                subset = subset_to_blocks(intermediate, blks, array.blocks.shape[-len(axis) :])
-                reindexed = dask.array.map_blocks(
-                    reindex_intermediates, subset, agg, index, meta=subset._meta
-                )
+                cohort_index = pd.Index(cohort)
+                reindexer = partial(reindex_intermediates, agg=agg, unique_groups=cohort_index)
+                reindexed = subset_to_blocks(intermediate, blks, block_shape, reindexer)
                 # now that we have reindexed, we can set reindex=True explicitlly
                 reduced_.append(
                     tree_reduce(
                         reindexed,
                         combine=partial(combine, agg=agg, reindex=True),
-                        aggregate=partial(aggregate, expected_groups=index, reindex=True),
+                        aggregate=partial(aggregate, expected_groups=cohort_index, reindex=True),
                     )
                 )
                 # This is done because pandas promotes to 64-bit types when an Index is created
                 # So we use the index to generate the return value for consistency with "map-reduce"
                 # This is important on windows
-                groups_.append(index.values)
+                groups_.append(cohort_index.values)
 
             reduced = dask.array.concatenate(reduced_, axis=-1)
             groups = (np.concatenate(groups_),)
             group_chunks = (tuple(len(cohort) for cohort in groups_),)
 
     elif method == "blockwise":
         reduced = intermediate
@@ -1714,14 +1774,117 @@
         concatenate=False,
         new_axes=new_axes,
     )
 
     return (result, groups)
 
 
+def cubed_groupby_agg(
+    array: CubedArray,
+    by: T_By,
+    agg: Aggregation,
+    expected_groups: pd.Index | None,
+    axis: T_Axes = (),
+    fill_value: Any = None,
+    method: T_Method = "map-reduce",
+    reindex: bool = False,
+    engine: T_Engine = "numpy",
+    sort: bool = True,
+    chunks_cohorts=None,
+) -> tuple[CubedArray, tuple[np.ndarray | CubedArray]]:
+    import cubed
+    import cubed.core.groupby
+
+    # I think _tree_reduce expects this
+    assert isinstance(axis, Sequence)
+    assert all(ax >= 0 for ax in axis)
+
+    inds = tuple(range(array.ndim))
+
+    by_input = by
+
+    # Unifying chunks is necessary for argreductions.
+    # We need to rechunk before zipping up with the index
+    # let's always do it anyway
+    if not is_chunked_array(by):
+        # chunk numpy arrays like the input array
+        chunks = tuple(array.chunks[ax] if by.shape[ax] != 1 else (1,) for ax in range(-by.ndim, 0))
+
+        by = cubed.from_array(by, chunks=chunks, spec=array.spec)
+    _, (array, by) = cubed.core.unify_chunks(array, inds, by, inds[-by.ndim :])
+
+    # Cubed's groupby_reduction handles the generation of "intermediates", and the
+    # "map-reduce" combination step, so we don't have to do that here.
+    # Only the equivalent of "_simple_combine" is supported, there is no
+    # support for "_grouped_combine".
+    labels_are_unknown = is_chunked_array(by_input) and expected_groups is None
+    do_simple_combine = not _is_arg_reduction(agg) and not labels_are_unknown
+
+    assert do_simple_combine
+    assert method == "map-reduce"
+    assert expected_groups is not None
+    assert reindex is True
+    assert len(axis) == 1  # one axis/grouping
+
+    def _groupby_func(a, by, axis, intermediate_dtype, num_groups):
+        blockwise_method = partial(
+            _get_chunk_reduction(agg.reduction_type),
+            func=agg.chunk,
+            fill_value=agg.fill_value["intermediate"],
+            dtype=agg.dtype["intermediate"],
+            reindex=reindex,
+            user_dtype=agg.dtype["user"],
+            axis=axis,
+            expected_groups=expected_groups,
+            engine=engine,
+            sort=sort,
+        )
+        out = blockwise_method(a, by)
+        # Convert dict to one that cubed understands, dropping groups since they are
+        # known, and the same for every block.
+        return {f"f{idx}": intermediate for idx, intermediate in enumerate(out["intermediates"])}
+
+    def _groupby_combine(a, axis, dummy_axis, dtype, keepdims):
+        # this is similar to _simple_combine, except the dummy axis and concatenation is handled by cubed
+        # only combine over the dummy axis, to preserve grouping along 'axis'
+        dtype = dict(dtype)
+        out = {}
+        for idx, combine in enumerate(agg.simple_combine):
+            field = f"f{idx}"
+            out[field] = combine(a[field], axis=dummy_axis, keepdims=keepdims)
+        return out
+
+    def _groupby_aggregate(a):
+        # Convert cubed dict to one that _finalize_results works with
+        results = {"groups": expected_groups, "intermediates": a.values()}
+        out = _finalize_results(results, agg, axis, expected_groups, fill_value, reindex)
+        return out[agg.name]
+
+    # convert list of dtypes to a structured dtype for cubed
+    intermediate_dtype = [(f"f{i}", dtype) for i, dtype in enumerate(agg.dtype["intermediate"])]
+    dtype = agg.dtype["final"]
+    num_groups = len(expected_groups)
+
+    result = cubed.core.groupby.groupby_reduction(
+        array,
+        by,
+        func=_groupby_func,
+        combine_func=_groupby_combine,
+        aggregate_func=_groupby_aggregate,
+        axis=axis,
+        intermediate_dtype=intermediate_dtype,
+        dtype=dtype,
+        num_groups=num_groups,
+    )
+
+    groups = (expected_groups.to_numpy(),)
+
+    return (result, groups)
+
+
 def _collapse_blocks_along_axes(reduced: DaskArray, axis: T_Axes, group_chunks) -> DaskArray:
     import dask.array
     from dask.highlevelgraph import HighLevelGraph
 
     nblocks = tuple(reduced.numblocks[ax] for ax in axis)
     output_chunks = reduced.chunks[: -len(axis)] + ((1,) * (len(axis) - 1),) + group_chunks
 
@@ -1819,23 +1982,21 @@
                 f"array {idx} in `by` has shape {b.shape}."
             )
 
 
 @overload
 def _convert_expected_groups_to_index(
     expected_groups: tuple[None, ...], isbin: Sequence[bool], sort: bool
-) -> tuple[None, ...]:
-    ...
+) -> tuple[None, ...]: ...
 
 
 @overload
 def _convert_expected_groups_to_index(
     expected_groups: T_ExpectTuple, isbin: Sequence[bool], sort: bool
-) -> T_ExpectIndexTuple:
-    ...
+) -> T_ExpectIndexTuple: ...
 
 
 def _convert_expected_groups_to_index(
     expected_groups: T_ExpectOptTuple, isbin: Sequence[bool], sort: bool
 ) -> T_ExpectIndexOptTuple:
     out: list[T_ExpectIndexOpt] = []
     for ex, isbin_ in zip(expected_groups, isbin):
@@ -1915,21 +2076,19 @@
         kwargs["by"] = by
         group_idx, found_groups, grp_shape, *_ = factorize_(**kwargs)
 
     return (group_idx,), found_groups, grp_shape
 
 
 @overload
-def _validate_expected_groups(nby: int, expected_groups: None) -> tuple[None, ...]:
-    ...
+def _validate_expected_groups(nby: int, expected_groups: None) -> tuple[None, ...]: ...
 
 
 @overload
-def _validate_expected_groups(nby: int, expected_groups: T_ExpectedGroups) -> T_ExpectTuple:
-    ...
+def _validate_expected_groups(nby: int, expected_groups: T_ExpectedGroups) -> T_ExpectTuple: ...
 
 
 def _validate_expected_groups(nby: int, expected_groups: T_ExpectedGroupsOpt) -> T_ExpectOptTuple:
     if expected_groups is None:
         return (None,) * nby
 
     if nby == 1 and not isinstance(expected_groups, tuple):
@@ -2161,14 +2320,15 @@
                     "or set engine=None to use the default."
                 )
 
     bys: T_Bys = tuple(np.asarray(b) if not is_duck_array(b) else b for b in by)
     nby = len(bys)
     by_is_dask = tuple(is_duck_dask_array(b) for b in bys)
     any_by_dask = any(by_is_dask)
+    provided_expected = expected_groups is not None
 
     if (
         engine == "numbagg"
         and _is_arg_reduction(func)
         and (any_by_dask or is_duck_dask_array(array))
     ):
         # There is only one test that fails, but I can't figure
@@ -2236,14 +2396,15 @@
     if axis is None:
         axis_ = tuple(array.ndim + np.arange(-by_.ndim, 0))
     else:
         axis_ = normalize_axis_tuple(axis, array.ndim)
     nax = len(axis_)
 
     has_dask = is_duck_dask_array(array) or is_duck_dask_array(by_)
+    has_cubed = is_duck_cubed_array(array) or is_duck_cubed_array(by_)
 
     if _is_first_last_reduction(func):
         if has_dask and nax != 1:
             raise ValueError(
                 "For dask arrays: first, last, nanfirst, nanlast reductions are "
                 "only supported along a single axis. Please reshape appropriately."
             )
@@ -2276,15 +2437,15 @@
     # When axis is a subset of possible values; then npg will
     # apply the fill_value to groups that don't exist along a particular axis (for e.g.)
     # since these count as a group that is absent. thoo!
     # fill_value applies to all-NaN groups as well as labels in expected_groups that are not found.
     #     The only way to do this consistently is mask out using min_count
     #     Consider np.sum([np.nan]) = np.nan, np.nansum([np.nan]) = 0
     if min_count is None:
-        if nax < by_.ndim or fill_value is not None:
+        if nax < by_.ndim or (fill_value is not None and provided_expected):
             min_count_: int = 1
         else:
             min_count_ = 0
     else:
         min_count_ = min_count
 
     # TODO: set in xarray?
@@ -2298,15 +2459,38 @@
 
     # Need to set this early using `agg`
     # It cannot be done in the core loop of chunk_reduce
     # since we "prepare" the data for flox.
     kwargs["engine"] = _choose_engine(by_, agg) if engine is None else engine
 
     groups: tuple[np.ndarray | DaskArray, ...]
-    if not has_dask:
+    if has_cubed:
+        if method is None:
+            method = "map-reduce"
+
+        if method != "map-reduce":
+            raise NotImplementedError(
+                "Reduction for Cubed arrays is only implemented for method 'map-reduce'."
+            )
+
+        partial_agg = partial(cubed_groupby_agg, **kwargs)
+
+        result, groups = partial_agg(
+            array,
+            by_,
+            expected_groups=expected_,
+            agg=agg,
+            reindex=reindex,
+            method=method,
+            sort=sort,
+        )
+
+        return (result, groups)
+
+    elif not has_dask:
         results = _reduce_blockwise(
             array, by_, agg, expected_groups=expected_, reindex=reindex, sort=sort, **kwargs
         )
         groups = (results["groups"],)
         result = results[agg.name]
 
     else:
```

### Comparing `flox-0.9.6/flox/visualize.py` & `flox-0.9.7/flox/visualize.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/flox/xarray.py` & `flox-0.9.7/flox/xarray.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/flox/xrdtypes.py` & `flox-0.9.7/flox/xrdtypes.py`

 * *Files identical despite different names*

### Comparing `flox-0.9.6/flox/xrutils.py` & `flox-0.9.7/flox/xrutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import datetime
 import importlib
 from collections.abc import Iterable
 from typing import Any, Optional
 
 import numpy as np
 import pandas as pd
-from numpy.core.multiarray import normalize_axis_index  # type: ignore[attr-defined]
 from packaging.version import Version
 
 try:
     import cftime
 except ImportError:
     cftime = None
 
@@ -21,45 +20,92 @@
     import dask.array
 
     dask_array_type = dask.array.Array
 except ImportError:
     dask_array_type = ()  # type: ignore[assignment, misc]
 
 
+def module_available(module: str, minversion: Optional[str] = None) -> bool:
+    """Checks whether a module is installed without importing it.
+
+    Use this for a lightweight check and lazy imports.
+
+    Parameters
+    ----------
+    module : str
+        Name of the module.
+
+    Returns
+    -------
+    available : bool
+        Whether the module is installed.
+    """
+    has = importlib.util.find_spec(module) is not None
+    if has:
+        mod = importlib.import_module(module)
+        return Version(mod.__version__) >= Version(minversion) if minversion is not None else True
+    else:
+        return False
+
+
+if module_available("numpy", minversion="2.0.0"):
+    from numpy.lib.array_utils import (  # type: ignore[import-not-found]
+        normalize_axis_index,
+    )
+else:
+    from numpy.core.numeric import normalize_axis_index  # type: ignore[attr-defined]
+
+
 def asarray(data, xp=np):
     return data if is_duck_array(data) else xp.asarray(data)
 
 
 def is_duck_array(value: Any) -> bool:
     """Checks if value is a duck array."""
     if isinstance(value, np.ndarray):
         return True
     return (
         hasattr(value, "ndim")
         and hasattr(value, "shape")
         and hasattr(value, "dtype")
-        and hasattr(value, "__array_function__")
-        and hasattr(value, "__array_ufunc__")
+        and (
+            (hasattr(value, "__array_function__") and hasattr(value, "__array_ufunc__"))
+            or hasattr(value, "__array_namespace__")
+        )
     )
 
 
+def is_chunked_array(x) -> bool:
+    """True if dask or cubed"""
+    return is_duck_dask_array(x) or (is_duck_array(x) and hasattr(x, "chunks"))
+
+
 def is_dask_collection(x):
     try:
         import dask
 
         return dask.is_dask_collection(x)
 
     except ImportError:
         return False
 
 
 def is_duck_dask_array(x):
     return is_duck_array(x) and is_dask_collection(x)
 
 
+def is_duck_cubed_array(x):
+    try:
+        import cubed
+
+        return is_duck_array(x) and isinstance(x, cubed.Array)
+    except ImportError:
+        return False
+
+
 class ReprObject:
     """Object that prints as the given value, for use with sentinel values."""
 
     __slots__ = ("_value",)
 
     def __init__(self, value: str):
         self._value = value
@@ -329,30 +375,7 @@
     rev = (slice(None),) * axis + (slice(None, None, -1),)
     idx_last = -1 - np.argmax(~pd.isnull(values)[rev], axis=axis)
     result = _select_along_axis(values, idx_last, axis)
     if keepdims:
         return np.expand_dims(result, axis=axis)
     else:
         return result
-
-
-def module_available(module: str, minversion: Optional[str] = None) -> bool:
-    """Checks whether a module is installed without importing it.
-
-    Use this for a lightweight check and lazy imports.
-
-    Parameters
-    ----------
-    module : str
-        Name of the module.
-
-    Returns
-    -------
-    available : bool
-        Whether the module is installed.
-    """
-    has = importlib.util.find_spec(module) is not None
-    if has:
-        mod = importlib.import_module(module)
-        return Version(mod.__version__) >= Version(minversion) if minversion is not None else True
-    else:
-        return False
```

### Comparing `flox-0.9.6/flox.egg-info/PKG-INFO` & `flox-0.9.7/flox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flox
-Version: 0.9.6
+Version: 0.9.7
 Summary: GroupBy operations for dask.array
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flox-0.9.6/flox.egg-info/SOURCES.txt` & `flox-0.9.7/flox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 docs/source/engines.md
 docs/source/implementation.md
 docs/source/index.md
 docs/source/intro.md
 docs/source/user-stories.md
 docs/source/xarray.md
 docs/source/_static/style.css
+docs/source/user-stories/climatology-hourly-cubed.ipynb
 docs/source/user-stories/climatology-hourly.ipynb
 docs/source/user-stories/climatology.ipynb
 docs/source/user-stories/custom-aggregations.ipynb
 docs/source/user-stories/hourly-climatology.html
 docs/source/user-stories/nD-bins.ipynb
 docs/source/user-stories/overlaps.md
 flox/__init__.py
```

### Comparing `flox-0.9.6/pyproject.toml` & `flox-0.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
 exclude=["asv_bench/pkgs"]
 
 [[tool.mypy.overrides]]
 module=[
     "asv_runner.*",
     "cachey",
     "cftime",
+    "cubed.*",
     "dask.*",
     "importlib_metadata",
     "numba",
     "numbagg.*",
     "numpy_groupies.*",
     "matplotlib.*",
     "pandas",
```

### Comparing `flox-0.9.6/tests/__init__.py` & `flox-0.9.7/tests/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     # Our development version is something like '0.10.9+aac7bfc'
     # This function just ignored the git commit id.
     vstring = vstring.split("+")[0]
     return packaging.version.Version(vstring)
 
 
 has_cftime, requires_cftime = _importorskip("cftime")
+has_cubed, requires_cubed = _importorskip("cubed")
 has_dask, requires_dask = _importorskip("dask")
 has_numba, requires_numba = _importorskip("numba")
 has_numbagg, requires_numbagg = _importorskip("numbagg")
 has_scipy, requires_scipy = _importorskip("scipy")
 has_xarray, requires_xarray = _importorskip("xarray")
```

### Comparing `flox-0.9.6/tests/test_core.py` & `flox-0.9.7/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,18 @@
 
 from . import (
     ALL_FUNCS,
     BLOCKWISE_FUNCS,
     SCIPY_STATS_FUNCS,
     assert_equal,
     assert_equal_tuple,
+    has_cubed,
     has_dask,
     raise_if_dask_computes,
+    requires_cubed,
     requires_dask,
 )
 
 logger = logging.getLogger("flox")
 logger.setLevel(logging.DEBUG)
 
 labels = np.array([0, 0, 2, 2, 2, 1, 1, 2, 2, 1, 1, 0])
@@ -57,14 +59,18 @@
     dask.config.set(scheduler="sync")
 else:
 
     def dask_array_ones(*args):
         return None
 
 
+if has_cubed:
+    import cubed
+
+
 DEFAULT_QUANTILE = 0.9
 
 if TYPE_CHECKING:
     from flox.core import T_Agg, T_Engine, T_ExpectedGroupsOpt, T_Method
 
 
 def _get_array_func(func: str) -> Callable:
@@ -473,14 +479,57 @@
 
     with raise_if_dask_computes():
         actual, groups = groupby_reduce(array, by, engine=engine, **kwargs, sort=True)
     assert_equal(groups, np.array([0, 1, 2], np.int64))
     assert_equal(expected, actual)
 
 
+@requires_cubed
+@pytest.mark.parametrize("reindex", [True])
+@pytest.mark.parametrize("func", ALL_FUNCS)
+@pytest.mark.parametrize("add_nan", [False, True])
+@pytest.mark.parametrize(
+    "shape, array_chunks, group_chunks",
+    [
+        ((12,), (3,), 3),  # form 1
+    ],
+)
+def test_groupby_agg_cubed(func, shape, array_chunks, group_chunks, add_nan, engine, reindex):
+    """Tests groupby_reduce with cubed arrays against groupby_reduce with numpy arrays"""
+
+    if func in ["first", "last"] or func in BLOCKWISE_FUNCS:
+        pytest.skip()
+
+    if "arg" in func and (engine in ["flox", "numbagg"] or reindex):
+        pytest.skip()
+
+    array = cubed.array_api.ones(shape, chunks=array_chunks)
+
+    labels = np.array([0, 0, 2, 2, 2, 1, 1, 2, 2, 1, 1, 0])
+    if add_nan:
+        labels = labels.astype(float)
+        labels[:3] = np.nan  # entire block is NaN when group_chunks=3
+        labels[-2:] = np.nan
+
+    kwargs = dict(
+        func=func,
+        expected_groups=[0, 1, 2],
+        fill_value=False if func in ["all", "any"] else 123,
+        reindex=reindex,
+    )
+
+    expected, _ = groupby_reduce(array.compute(), labels, engine="numpy", **kwargs)
+    actual, _ = groupby_reduce(array.compute(), labels, engine=engine, **kwargs)
+    assert_equal(actual, expected)
+
+    # TODO: raise_if_cubed_computes
+    actual, _ = groupby_reduce(array, labels, engine=engine, **kwargs)
+    assert_equal(expected, actual)
+
+
 def test_numpy_reduce_axis_subset(engine):
     # TODO: add NaNs
     by = labels2d
     array = np.ones_like(by, dtype=np.int64)
     kwargs = dict(func="count", engine=engine, fill_value=0)
     result, _ = groupby_reduce(array, by, **kwargs, axis=1)
     assert_equal(result, np.array([[2, 3], [2, 3]], dtype=np.intp))
@@ -893,29 +942,44 @@
     assert_equal(groups.astype(np.int64), np.arange(366, dtype=np.int64))
 
 
 @requires_dask
 @pytest.mark.parametrize("chunksize", (12,) + tuple(range(1, 13)) + (-1,))
 def test_method_guessing(chunksize):
     # just a regression test
-    labels = np.tile(np.arange(1, 13), 30)
+    labels = np.tile(np.arange(0, 12), 30)
     by = dask.array.from_array(labels, chunks=chunksize) - 1
     preferred_method, chunks_cohorts = find_group_cohorts(labels, by.chunks[slice(-1, None)])
     if chunksize == -1:
         assert preferred_method == "blockwise"
-        assert chunks_cohorts == {(0,): list(range(1, 13))}
+        assert chunks_cohorts == {(0,): list(range(12))}
     elif chunksize in (1, 2, 3, 4, 6):
         assert preferred_method == "cohorts"
         assert len(chunks_cohorts) == 12 // chunksize
     else:
         assert preferred_method == "map-reduce"
         assert chunks_cohorts == {}
 
 
 @requires_dask
+@pytest.mark.parametrize("ndim", [1, 2, 3])
+def test_single_chunk_method_is_blockwise(ndim):
+    for by_ndim in range(1, ndim + 1):
+        chunks = (5,) * (ndim - by_ndim) + (-1,) * by_ndim
+        assert len(chunks) == ndim
+        array = dask.array.ones(shape=(10,) * ndim, chunks=chunks)
+        by = np.zeros(shape=(10,) * by_ndim, dtype=int)
+        method, chunks_cohorts = find_group_cohorts(
+            by, chunks=[array.chunks[ax] for ax in range(-by.ndim, 0)]
+        )
+        assert method == "blockwise"
+        assert chunks_cohorts == {(0,): [0]}
+
+
+@requires_dask
 @pytest.mark.parametrize(
     "chunk_at,expected",
     [
         [1, ((1, 6, 1, 6, 1, 6, 1, 6, 1, 1),)],
         [0, ((7, 7, 7, 7, 2),)],
         [3, ((3, 4, 3, 4, 3, 4, 3, 4, 2),)],
     ],
@@ -1397,22 +1461,26 @@
     expected = tuple(np.array(i) if isinstance(i, list) else i for i in expected)
     actual = _normalize_indexes(array, flatblocks, array.blocks.shape)
     assert_equal_tuple(expected, actual)
 
 
 @requires_dask
 def test_subset_block_passthrough():
+    from flox.core import identity
+
     # full slice pass through
     array = dask.array.ones((5,), chunks=(1,))
+    expected = dask.array.map_blocks(identity, array)
     subset = subset_to_blocks(array, np.arange(5))
-    assert subset.name == array.name
+    assert subset.name == expected.name
 
     array = dask.array.ones((5, 5), chunks=1)
+    expected = dask.array.map_blocks(identity, array)
     subset = subset_to_blocks(array, np.arange(25))
-    assert subset.name == array.name
+    assert subset.name == expected.name
 
 
 @requires_dask
 @pytest.mark.parametrize(
     "flatblocks, expectidx",
     [
         (np.arange(10), (slice(2), slice(None))),
```

### Comparing `flox-0.9.6/tests/test_xarray.py` & `flox-0.9.7/tests/test_xarray.py`

 * *Files identical despite different names*

