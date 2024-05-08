# Comparing `tmp/birdhouse-birdy-0.8.6.tar.gz` & `tmp/birdhouse_birdy-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "birdhouse-birdy-0.8.6.tar", last modified: Mon Mar 18 17:43:47 2024, max compression
+gzip compressed data, was "birdhouse_birdy-0.8.7.tar", last modified: Wed May  8 18:00:32 2024, max compression
```

## Comparing `birdhouse-birdy-0.8.6.tar` & `birdhouse_birdy-0.8.7.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.699933 birdhouse-birdy-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-03-18 17:43:47.699933 birdhouse-birdy-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.695933 birdhouse-birdy-0.8.6/birdhouse_birdy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-03-18 17:43:47.000000 birdhouse-birdy-0.8.6/birdhouse_birdy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-18 17:43:47.000000 birdhouse-birdy-0.8.6/birdhouse_birdy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 17:43:47.000000 birdhouse-birdy-0.8.6/birdhouse_birdy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-18 17:43:47.000000 birdhouse-birdy-0.8.6/birdhouse_birdy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 17:43:47.000000 birdhouse-birdy-0.8.6/birdhouse_birdy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-18 17:43:47.000000 birdhouse-birdy-0.8.6/birdhouse_birdy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-18 17:43:47.000000 birdhouse-birdy-0.8.6/birdhouse_birdy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.679933 birdhouse-birdy-0.8.6/birdy/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.679933 birdhouse-birdy-0.8.6/birdy/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/cli/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.683933 birdhouse-birdy-0.8.6/birdy/client/
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15857 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/client/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/client/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/client/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/client/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.683933 birdhouse-birdy-0.8.6/birdy/ipyleafletwfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/ipyleafletwfs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/ipyleafletwfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15068 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/ipyleafletwfs/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.683933 birdhouse-birdy-0.8.6/birdy/ipyleafletwfs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/ipyleafletwfs/examples/quickstart-template.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.683933 birdhouse-birdy-0.8.6/birdy/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/templates/cmd.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/birdy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.671934 birdhouse-birdy-0.8.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.687934 birdhouse-birdy-0.8.6/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.687934 birdhouse-birdy-0.8.6/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/_static/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/_static/birdhouse_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.687934 birdhouse-birdy-0.8.6/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/notebooks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.687934 birdhouse-birdy-0.8.6/docs/source/notebooks/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/notebooks/demo/agu2018_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/notebooks/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.687934 birdhouse-birdy-0.8.6/docs/source/notebooks/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/notebooks/examples/Interactive.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/notebooks/examples/emu-example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/notebooks/examples/owslib-esgfwps.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/notebooks/examples/owslib.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/notebooks/examples/rook-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/notebooks/examples/twitcher-c3s-magic-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/notebooks/examples/twitcher-magic-cexp-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/docs/source/notebooks/output_sanitize.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/requirements_extra.txt
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-18 17:43:47.699933 birdhouse-birdy-0.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.691933 birdhouse-birdy-0.8.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:43:47.695933 birdhouse-birdy-0.8.6/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/resources/Olympus.tif
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/resources/Olympus_Mons.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/resources/dummy.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/resources/process_description.xml
--rw-r--r--   0 runner    (1001) docker     (127)    27371 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/resources/test.nc
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/resources/wps_52n_caps.xml
--rw-r--r--   0 runner    (1001) docker     (127)    35766 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/resources/wps_52n_desc.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/resources/wps_emu_caps.xml
--rw-r--r--   0 runner    (1001) docker     (127)    52727 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/resources/wps_emu_desc.xml
--rw-r--r--   0 runner    (1001) docker     (127)    34280 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/resources/wps_fly_caps.xml
--rw-r--r--   0 runner    (1001) docker     (127)   398863 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/resources/wps_fly_desc.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-03-18 17:43:43.000000 birdhouse-birdy-0.8.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.970105 birdhouse_birdy-0.8.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    13248 2024-05-08 18:00:32.970105 birdhouse_birdy-0.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.966105 birdhouse_birdy-0.8.7/birdhouse_birdy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13248 2024-05-08 18:00:32.000000 birdhouse_birdy-0.8.7/birdhouse_birdy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-08 18:00:32.000000 birdhouse_birdy-0.8.7/birdhouse_birdy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:00:32.000000 birdhouse_birdy-0.8.7/birdhouse_birdy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 18:00:32.000000 birdhouse_birdy-0.8.7/birdhouse_birdy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:00:32.000000 birdhouse_birdy-0.8.7/birdhouse_birdy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-08 18:00:32.000000 birdhouse_birdy-0.8.7/birdhouse_birdy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 18:00:32.000000 birdhouse_birdy-0.8.7/birdhouse_birdy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.946105 birdhouse_birdy-0.8.7/birdy/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.950105 birdhouse_birdy-0.8.7/birdy/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/cli/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.950105 birdhouse_birdy-0.8.7/birdy/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15857 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/client/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/client/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/client/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.950105 birdhouse_birdy-0.8.7/birdy/ipyleafletwfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/ipyleafletwfs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/ipyleafletwfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15068 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/ipyleafletwfs/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.954105 birdhouse_birdy-0.8.7/birdy/ipyleafletwfs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/ipyleafletwfs/examples/quickstart-template.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.954105 birdhouse_birdy-0.8.7/birdy/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/templates/cmd.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/birdy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.942105 birdhouse_birdy-0.8.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.954105 birdhouse_birdy-0.8.7/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.954105 birdhouse_birdy-0.8.7/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/_static/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/_static/birdhouse_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.958105 birdhouse_birdy-0.8.7/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/notebooks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.958105 birdhouse_birdy-0.8.7/docs/source/notebooks/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/notebooks/demo/agu2018_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/notebooks/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.958105 birdhouse_birdy-0.8.7/docs/source/notebooks/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/notebooks/examples/Interactive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/notebooks/examples/emu-example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/notebooks/examples/owslib-esgfwps.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/notebooks/examples/owslib.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/notebooks/examples/rook-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/notebooks/examples/twitcher-c3s-magic-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/notebooks/examples/twitcher-magic-cexp-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/docs/source/notebooks/output_sanitize.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/requirements_extra.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-08 18:00:32.970105 birdhouse_birdy-0.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.962105 birdhouse_birdy-0.8.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:00:32.962105 birdhouse_birdy-0.8.7/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/resources/Olympus.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/resources/Olympus_Mons.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/resources/dummy.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/resources/process_description.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    27371 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/resources/test.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/resources/wps_52n_caps.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    35766 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/resources/wps_52n_desc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/resources/wps_emu_caps.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    52727 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/resources/wps_emu_desc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    34280 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/resources/wps_fly_caps.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   398863 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/resources/wps_fly_desc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-08 18:00:28.000000 birdhouse_birdy-0.8.7/tests/test_utils.py
```

### Comparing `birdhouse-birdy-0.8.6/CHANGES.rst` & `birdhouse_birdy-0.8.7/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Change History
 **************
 
+v0.8.7 (2024-05-07)
+===================
+
+* Fix regression, where loading TIFF files would return a Dataset instead of a DataArray, the behavior prior to 0.8.5. Loading a multi-band TIFF file will now return a DataArray with the bands as dimensions.
+
+
 v0.8.6 (2024-03-18)
 ===================
 
 Changes:
 
 * Restructure the package so that the wheel does not install the testing and docs as non-importable packages.
 * Ensure that data required to run tests and build docs is present in the source distribution (via `Manifest.in` changes).
```

### Comparing `birdhouse-birdy-0.8.6/LICENSE.txt` & `birdhouse_birdy-0.8.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/MANIFEST.in` & `birdhouse_birdy-0.8.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/Makefile` & `birdhouse_birdy-0.8.7/Makefile`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/PKG-INFO` & `birdhouse_birdy-0.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birdhouse-birdy
-Version: 0.8.6
+Version: 0.8.7
 Summary: Birdy provides a command-line tool to work with Web Processing Services.
 Home-page: https://github.com/bird-house/birdy
 Author: Carsten Ehbrecht
 Author-email: ehbrecht@dkrz.de
 License: Apache License v2.0
 Keywords: wps pywps owslib geopython birdy birdhouse
 Classifier: Development Status :: 4 - Beta
@@ -105,19 +105,19 @@
         :alt: GitHub license
 
 .. |Gitter| image:: https://badges.gitter.im/bird-house/birdhouse.svg
         :target: https://gitter.im/bird-house/birdhouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
         :alt: Join the chat at https://gitter.im/bird-house/birdhouse
 
 .. |Binder| image:: https://mybinder.org/badge_logo.svg
-        :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.6?filepath=notebooks
+        :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.7?filepath=notebooks
         :alt: Binder Launcher
 
 .. |NBViewer| image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
-        :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.6/notebooks/
+        :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.7/notebooks/
         :alt: NBViewer
         :height: 20
 
 Authors
 *******
 
 * David Huard <huard.david@ouranos.ca>
@@ -127,14 +127,20 @@
 ************
 
 * Trevor James Smith <smith.trevorj@ouranos.ca> `@Zeitsperre <https://www.github.com/Zeitsperre>`_
 
 Change History
 **************
 
+v0.8.7 (2024-05-07)
+===================
+
+* Fix regression, where loading TIFF files would return a Dataset instead of a DataArray, the behavior prior to 0.8.5. Loading a multi-band TIFF file will now return a DataArray with the bands as dimensions.
+
+
 v0.8.6 (2024-03-18)
 ===================
 
 Changes:
 
 * Restructure the package so that the wheel does not install the testing and docs as non-importable packages.
 * Ensure that data required to run tests and build docs is present in the source distribution (via `Manifest.in` changes).
```

### Comparing `birdhouse-birdy-0.8.6/README.rst` & `birdhouse_birdy-0.8.7/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,14 @@
         :alt: GitHub license
 
 .. |Gitter| image:: https://badges.gitter.im/bird-house/birdhouse.svg
         :target: https://gitter.im/bird-house/birdhouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
         :alt: Join the chat at https://gitter.im/bird-house/birdhouse
 
 .. |Binder| image:: https://mybinder.org/badge_logo.svg
-        :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.6?filepath=notebooks
+        :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.7?filepath=notebooks
         :alt: Binder Launcher
 
 .. |NBViewer| image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
-        :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.6/notebooks/
+        :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.7/notebooks/
         :alt: NBViewer
         :height: 20
```

### Comparing `birdhouse-birdy-0.8.6/birdhouse_birdy.egg-info/PKG-INFO` & `birdhouse_birdy-0.8.7/birdhouse_birdy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birdhouse-birdy
-Version: 0.8.6
+Version: 0.8.7
 Summary: Birdy provides a command-line tool to work with Web Processing Services.
 Home-page: https://github.com/bird-house/birdy
 Author: Carsten Ehbrecht
 Author-email: ehbrecht@dkrz.de
 License: Apache License v2.0
 Keywords: wps pywps owslib geopython birdy birdhouse
 Classifier: Development Status :: 4 - Beta
@@ -105,19 +105,19 @@
         :alt: GitHub license
 
 .. |Gitter| image:: https://badges.gitter.im/bird-house/birdhouse.svg
         :target: https://gitter.im/bird-house/birdhouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
         :alt: Join the chat at https://gitter.im/bird-house/birdhouse
 
 .. |Binder| image:: https://mybinder.org/badge_logo.svg
-        :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.6?filepath=notebooks
+        :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.7?filepath=notebooks
         :alt: Binder Launcher
 
 .. |NBViewer| image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
-        :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.6/notebooks/
+        :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.7/notebooks/
         :alt: NBViewer
         :height: 20
 
 Authors
 *******
 
 * David Huard <huard.david@ouranos.ca>
@@ -127,14 +127,20 @@
 ************
 
 * Trevor James Smith <smith.trevorj@ouranos.ca> `@Zeitsperre <https://www.github.com/Zeitsperre>`_
 
 Change History
 **************
 
+v0.8.7 (2024-05-07)
+===================
+
+* Fix regression, where loading TIFF files would return a Dataset instead of a DataArray, the behavior prior to 0.8.5. Loading a multi-band TIFF file will now return a DataArray with the bands as dimensions.
+
+
 v0.8.6 (2024-03-18)
 ===================
 
 Changes:
 
 * Restructure the package so that the wheel does not install the testing and docs as non-importable packages.
 * Ensure that data required to run tests and build docs is present in the source distribution (via `Manifest.in` changes).
```

### Comparing `birdhouse-birdy-0.8.6/birdhouse_birdy.egg-info/SOURCES.txt` & `birdhouse_birdy-0.8.7/birdhouse_birdy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/cli/__init__.py` & `birdhouse_birdy-0.8.7/birdy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/cli/base.py` & `birdhouse_birdy-0.8.7/birdy/cli/base.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/cli/misc.py` & `birdhouse_birdy-0.8.7/birdy/cli/misc.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/cli/run.py` & `birdhouse_birdy-0.8.7/birdy/cli/run.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/cli/types.py` & `birdhouse_birdy-0.8.7/birdy/cli/types.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/client/__init__.py` & `birdhouse_birdy-0.8.7/birdy/client/__init__.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/client/base.py` & `birdhouse_birdy-0.8.7/birdy/client/base.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/client/converters.py` & `birdhouse_birdy-0.8.7/birdy/client/converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
     def check_dependencies(self):  # noqa: D102
         self._check_import("rioxarray")
 
     def convert(self):  # noqa: D102
         import xarray  # isort: skip
         import rioxarray  # noqa
 
-        return xarray.open_dataset(self.file, engine="rasterio")
+        return xarray.open_dataarray(self.file, engine="rasterio")
 
 
 # TODO: Add test for this.
 class GeotiffGdalConverter(BaseConverter):  # noqa: D101
     mimetypes = ["image/tiff; subtype=geotiff"]
     extensions = ["tiff", "tif"]
     priority = 1
```

### Comparing `birdhouse-birdy-0.8.6/birdy/client/notebook.py` & `birdhouse_birdy-0.8.7/birdy/client/notebook.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/client/outputs.py` & `birdhouse_birdy-0.8.7/birdy/client/outputs.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/client/utils.py` & `birdhouse_birdy-0.8.7/birdy/client/utils.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/dependencies.py` & `birdhouse_birdy-0.8.7/birdy/dependencies.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/ipyleafletwfs/README.md` & `birdhouse_birdy-0.8.7/birdy/ipyleafletwfs/README.md`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/ipyleafletwfs/__init__.py` & `birdhouse_birdy-0.8.7/birdy/ipyleafletwfs/__init__.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/ipyleafletwfs/base.py` & `birdhouse_birdy-0.8.7/birdy/ipyleafletwfs/base.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb` & `birdhouse_birdy-0.8.7/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/ipyleafletwfs/examples/quickstart-template.ipynb` & `birdhouse_birdy-0.8.7/birdy/ipyleafletwfs/examples/quickstart-template.ipynb`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb` & `birdhouse_birdy-0.8.7/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/templates/cmd.py.j2` & `birdhouse_birdy-0.8.7/birdy/templates/cmd.py.j2`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/birdy/utils.py` & `birdhouse_birdy-0.8.7/birdy/utils.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/docs/source/_static/birdhouse_logo.svg` & `birdhouse_birdy-0.8.7/docs/source/_static/birdhouse_logo.svg`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/docs/source/_static/favicon.ico` & `birdhouse_birdy-0.8.7/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/docs/source/conf.py` & `birdhouse_birdy-0.8.7/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = ""
 # The full version, including alpha/beta/rc tags.
-release = "0.8.6"
+release = "0.8.7"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
```

### Comparing `birdhouse-birdy-0.8.6/docs/source/development.rst` & `birdhouse_birdy-0.8.7/docs/source/development.rst`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/docs/source/examples.rst` & `birdhouse_birdy-0.8.7/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/docs/source/installation.rst` & `birdhouse_birdy-0.8.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/docs/source/notebooks/README.md` & `birdhouse_birdy-0.8.7/docs/source/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/docs/source/notebooks/demo/agu2018_demo.ipynb` & `birdhouse_birdy-0.8.7/docs/source/notebooks/demo/agu2018_demo.ipynb`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/docs/source/notebooks/examples/Interactive.ipynb` & `birdhouse_birdy-0.8.7/docs/source/notebooks/examples/Interactive.ipynb`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/docs/source/notebooks/examples/emu-example.ipynb` & `birdhouse_birdy-0.8.7/docs/source/notebooks/examples/emu-example.ipynb`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/docs/source/notebooks/examples/owslib-esgfwps.ipynb` & `birdhouse_birdy-0.8.7/docs/source/notebooks/examples/owslib-esgfwps.ipynb`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/docs/source/notebooks/examples/owslib.ipynb` & `birdhouse_birdy-0.8.7/docs/source/notebooks/examples/owslib.ipynb`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/docs/source/notebooks/examples/rook-demo.ipynb` & `birdhouse_birdy-0.8.7/docs/source/notebooks/examples/rook-demo.ipynb`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/docs/source/notebooks/examples/twitcher-c3s-magic-demo.ipynb` & `birdhouse_birdy-0.8.7/docs/source/notebooks/examples/twitcher-c3s-magic-demo.ipynb`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/docs/source/notebooks/examples/twitcher-magic-cexp-demo.ipynb` & `birdhouse_birdy-0.8.7/docs/source/notebooks/examples/twitcher-magic-cexp-demo.ipynb`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/docs/source/notebooks/output_sanitize.cfg` & `birdhouse_birdy-0.8.7/docs/source/notebooks/output_sanitize.cfg`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/setup.cfg` & `birdhouse_birdy-0.8.7/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.6
+current_version = 0.8.7
 commit = True
 tag = False
 
 [metadata]
 description-file = README.rst
 
 [bumpversion:file:birdy/__init__.py]
```

### Comparing `birdhouse-birdy-0.8.6/setup.py` & `birdhouse_birdy-0.8.7/setup.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/tests/resources/Olympus.tif` & `birdhouse_birdy-0.8.7/tests/resources/Olympus.tif`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/tests/resources/Olympus_Mons.geojson` & `birdhouse_birdy-0.8.7/tests/resources/Olympus_Mons.geojson`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/tests/resources/dummy.nc` & `birdhouse_birdy-0.8.7/tests/resources/dummy.nc`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/tests/resources/process_description.xml` & `birdhouse_birdy-0.8.7/tests/resources/process_description.xml`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/tests/resources/test.nc` & `birdhouse_birdy-0.8.7/tests/resources/test.nc`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/tests/resources/wps_52n_caps.xml` & `birdhouse_birdy-0.8.7/tests/resources/wps_52n_caps.xml`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/tests/resources/wps_52n_desc.xml` & `birdhouse_birdy-0.8.7/tests/resources/wps_52n_desc.xml`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/tests/resources/wps_emu_caps.xml` & `birdhouse_birdy-0.8.7/tests/resources/wps_emu_caps.xml`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/tests/resources/wps_emu_desc.xml` & `birdhouse_birdy-0.8.7/tests/resources/wps_emu_desc.xml`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/tests/resources/wps_fly_caps.xml` & `birdhouse_birdy-0.8.7/tests/resources/wps_fly_caps.xml`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/tests/resources/wps_fly_desc.xml` & `birdhouse_birdy-0.8.7/tests/resources/wps_fly_desc.xml`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/tests/test_cli.py` & `birdhouse_birdy-0.8.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/tests/test_client.py` & `birdhouse_birdy-0.8.7/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.6/tests/test_converters.py` & `birdhouse_birdy-0.8.7/tests/test_converters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # noqa: D100
 
 import json
 import os
 import tempfile
 
 import pytest
+import xarray as xr
 from common import resource_file
 
 from birdy.client import converters
 
 
 def test_all_subclasses():  # noqa: D103
     c = converters.all_subclasses(converters.BaseConverter)
@@ -97,9 +98,9 @@
     assert isinstance(b, bytes)
 
 
 def test_raster_tif():
     pytest.importorskip("rioxarray")
     fn = resource_file("Olympus.tif")
 
-    ds = converters.convert(fn, path="/tmp")
-    assert "band_data" in ds.variables
+    da = converters.convert(fn, path="/tmp")
+    assert isinstance(da, xr.DataArray)
```

### Comparing `birdhouse-birdy-0.8.6/tests/test_utils.py` & `birdhouse_birdy-0.8.7/tests/test_utils.py`

 * *Files identical despite different names*

