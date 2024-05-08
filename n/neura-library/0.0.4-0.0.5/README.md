# Comparing `tmp/neura_library-0.0.4.tar.gz` & `tmp/neura_library-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neura_library-0.0.4.tar", last modified: Sun Apr 21 20:29:21 2024, max compression
+gzip compressed data, was "neura_library-0.0.5.tar", last modified: Wed May  8 15:22:47 2024, max compression
```

## Comparing `neura_library-0.0.4.tar` & `neura_library-0.0.5.tar`

### file list

```diff
@@ -1,182 +1,188 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.485972 neura_library-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-21 20:29:15.000000 neura_library-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-21 20:29:21.485972 neura_library-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-21 20:29:15.000000 neura_library-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-21 20:29:15.000000 neura_library-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-21 20:29:15.000000 neura_library-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 20:29:21.485972 neura_library-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.453972 neura_library-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.481972 neura_library-0.0.4/src/neura_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-21 20:29:21.000000 neura_library-0.0.4/src/neura_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-21 20:29:21.000000 neura_library-0.0.4/src/neura_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 20:29:21.000000 neura_library-0.0.4/src/neura_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-21 20:29:21.000000 neura_library-0.0.4/src/neura_library.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-21 20:29:21.000000 neura_library-0.0.4/src/neura_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 20:29:21.000000 neura_library-0.0.4/src/neura_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.457972 neura_library-0.0.4/src/neuralib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.461972 neura_library-0.0.4/src/neuralib/argp/
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/argp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/argp/_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18987 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/argp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/argp/dispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.461972 neura_library-0.0.4/src/neuralib/atlas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15498 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/allen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.461972 neura_library-0.0.4/src/neuralib/atlas/brainrender/
--rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/brainrender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/brainrender/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/brainrender/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/brainrender/main_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    13091 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/brainrender/probe_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/brainrender/roi_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/brainrender/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.465972 neura_library-0.0.4/src/neuralib/atlas/ccf/
--rw-r--r--   0 runner    (1001) docker     (127)    15822 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/ccf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33730 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/ccf/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    13041 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/ccf/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/ccf/norm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/ccf/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.465972 neura_library-0.0.4/src/neuralib/atlas/cellatlas/
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/cellatlas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/cellatlas/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.465972 neura_library-0.0.4/src/neuralib/atlas/ibl/
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/ibl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/ibl/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    55607 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/atlas/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.465972 neura_library-0.0.4/src/neuralib/bokeh_model/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/bokeh_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11440 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/bokeh_model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/bokeh_model/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/bokeh_model/example_multi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.465972 neura_library-0.0.4/src/neuralib/bokeh_model/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/bokeh_model/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/bokeh_model/examples/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/bokeh_model/examples/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/bokeh_model/examples/view_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/bokeh_model/examples/view_animal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/bokeh_model/examples/view_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/bokeh_model/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/bokeh_model/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/bokeh_model/view_brain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.465972 neura_library-0.0.4/src/neuralib/calimg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/calimg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.465972 neura_library-0.0.4/src/neuralib/calimg/scan_image/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/calimg/scan_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/calimg/scan_image/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.465972 neura_library-0.0.4/src/neuralib/calimg/scanbox/
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/calimg/scanbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/calimg/scanbox/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/calimg/scanbox/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.469972 neura_library-0.0.4/src/neuralib/calimg/suite2p/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/calimg/suite2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/calimg/suite2p/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/calimg/suite2p/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.469972 neura_library-0.0.4/src/neuralib/imglib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/imglib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/imglib/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/imglib/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    13647 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/imglib/labeller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/imglib/norm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.469972 neura_library-0.0.4/src/neuralib/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.469972 neura_library-0.0.4/src/neuralib/model/bayes_decoding/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/model/bayes_decoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/model/bayes_decoding/position.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.469972 neura_library-0.0.4/src/neuralib/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/persistence/cli_persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)    27622 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/persistence/persistence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.473972 neura_library-0.0.4/src/neuralib/plot/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/plot/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/plot/colormap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/plot/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/plot/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/plot/setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/plot/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/plot/venn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.473972 neura_library-0.0.4/src/neuralib/scanner/
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/scanner/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/scanner/czi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/scanner/lsm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.473972 neura_library-0.0.4/src/neuralib/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/segmentation/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.473972 neura_library-0.0.4/src/neuralib/segmentation/cellpose/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/segmentation/cellpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/segmentation/cellpose/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/segmentation/cellpose/run_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/segmentation/cellpose/run_subproc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.473972 neura_library-0.0.4/src/neuralib/segmentation/stardist/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/segmentation/stardist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/segmentation/stardist/run_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.477972 neura_library-0.0.4/src/neuralib/stimpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/stimpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/stimpy/baselog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/stimpy/baseprot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/stimpy/camlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/stimpy/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/stimpy/math_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/stimpy/preference.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/stimpy/protocol_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/stimpy/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    23178 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/stimpy/stimpy_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/stimpy/stimpy_git.py
--rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/stimpy/stimpy_pyv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/stimpy/stimulus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/stimpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.477972 neura_library-0.0.4/src/neuralib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.477972 neura_library-0.0.4/src/neuralib/tools/pkl_parq_view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/tools/pkl_parq_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/tools/pkl_parq_view/main_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.477972 neura_library-0.0.4/src/neuralib/tools/slack_bot/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/tools/slack_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/tools/slack_bot/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.481972 neura_library-0.0.4/src/neuralib/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/color_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/profile_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/segement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/util_cv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/util_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/util_verbose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.481972 neura_library-0.0.4/src/neuralib/wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.481972 neura_library-0.0.4/src/neuralib/wrapper/deeplabcut/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/wrapper/deeplabcut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/wrapper/deeplabcut/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/wrapper/deeplabcut/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.481972 neura_library-0.0.4/src/neuralib/wrapper/facemap/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/wrapper/facemap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/wrapper/facemap/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/wrapper/facemap/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.481972 neura_library-0.0.4/src/neuralib/wrapper/rastermap/
--rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/wrapper/rastermap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-21 20:29:15.000000 neura_library-0.0.4/src/neuralib/wrapper/rastermap/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:29:21.481972 neura_library-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-21 20:29:15.000000 neura_library-0.0.4/test/test_argp.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-21 20:29:15.000000 neura_library-0.0.4/test/test_argp_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-21 20:29:15.000000 neura_library-0.0.4/test/test_csv_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-21 20:29:15.000000 neura_library-0.0.4/test/test_persistence_autoinc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-21 20:29:15.000000 neura_library-0.0.4/test/test_protocol_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-21 20:29:15.000000 neura_library-0.0.4/test/test_pyvstim_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    62204 2024-04-21 20:29:15.000000 neura_library-0.0.4/test/test_stimpy_bitbucket_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    16421 2024-04-21 20:29:15.000000 neura_library-0.0.4/test/test_stimpy_github_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.853161 neura_library-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-08 15:22:40.000000 neura_library-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-05-08 15:22:47.853161 neura_library-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-08 15:22:40.000000 neura_library-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-08 15:22:40.000000 neura_library-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-08 15:22:40.000000 neura_library-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:22:47.853161 neura_library-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.825161 neura_library-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.853161 neura_library-0.0.5/src/neura_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-05-08 15:22:47.000000 neura_library-0.0.5/src/neura_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-08 15:22:47.000000 neura_library-0.0.5/src/neura_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:22:47.000000 neura_library-0.0.5/src/neura_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-08 15:22:47.000000 neura_library-0.0.5/src/neura_library.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-08 15:22:47.000000 neura_library-0.0.5/src/neura_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 15:22:47.000000 neura_library-0.0.5/src/neura_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.829161 neura_library-0.0.5/src/neuralib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.833161 neura_library-0.0.5/src/neuralib/argp/
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/argp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/argp/_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18987 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/argp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/argp/dispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.833161 neura_library-0.0.5/src/neuralib/atlas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.833161 neura_library-0.0.5/src/neuralib/atlas/brainrender/
+-rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/brainrender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/brainrender/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/brainrender/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/brainrender/main_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13091 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/brainrender/probe_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/brainrender/roi_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/brainrender/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.833161 neura_library-0.0.5/src/neuralib/atlas/ccf/
+-rw-r--r--   0 runner    (1001) docker     (127)    15822 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/ccf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33730 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/ccf/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/ccf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/ccf/norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/ccf/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.833161 neura_library-0.0.5/src/neuralib/atlas/cellatlas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/cellatlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/cellatlas/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.837161 neura_library-0.0.5/src/neuralib/atlas/ibl/
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/ibl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/ibl/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55607 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/atlas/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.837161 neura_library-0.0.5/src/neuralib/bokeh_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11440 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/example_multi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.837161 neura_library-0.0.5/src/neuralib/bokeh_model/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/examples/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/examples/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/examples/view_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/examples/view_animal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/examples/view_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/bokeh_model/view_brain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.837161 neura_library-0.0.5/src/neuralib/calimg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.837161 neura_library-0.0.5/src/neuralib/calimg/scan_image/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/scan_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/scan_image/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.837161 neura_library-0.0.5/src/neuralib/calimg/scanbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/scanbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/scanbox/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/scanbox/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.841161 neura_library-0.0.5/src/neuralib/calimg/suite2p/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/suite2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/suite2p/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/suite2p/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/calimg/suite2p/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.841161 neura_library-0.0.5/src/neuralib/imglib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/imglib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/imglib/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/imglib/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/imglib/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13647 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/imglib/labeller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/imglib/norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/imglib/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.841161 neura_library-0.0.5/src/neuralib/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.841161 neura_library-0.0.5/src/neuralib/model/bayes_decoding/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/model/bayes_decoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/model/bayes_decoding/position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.841161 neura_library-0.0.5/src/neuralib/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/persistence/cli_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27622 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/persistence/persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.841161 neura_library-0.0.5/src/neuralib/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/plot/venn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.845161 neura_library-0.0.5/src/neuralib/scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/scanner/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/scanner/czi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/scanner/lsm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.845161 neura_library-0.0.5/src/neuralib/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.845161 neura_library-0.0.5/src/neuralib/segmentation/cellpose/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/cellpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/cellpose/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/cellpose/run_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/cellpose/run_subproc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.845161 neura_library-0.0.5/src/neuralib/segmentation/stardist/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/stardist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/segmentation/stardist/run_2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.845161 neura_library-0.0.5/src/neuralib/stimpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/baselog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/baseprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/camlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/math_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/preference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/protocol_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23153 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/stimpy_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/stimpy_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/stimpy_pyv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/stimulus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/stimpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.849161 neura_library-0.0.5/src/neuralib/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.849161 neura_library-0.0.5/src/neuralib/tools/pkl_parq_view/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/tools/pkl_parq_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/tools/pkl_parq_view/main_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.849161 neura_library-0.0.5/src/neuralib/tools/slack_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/tools/slack_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/tools/slack_bot/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.849161 neura_library-0.0.5/src/neuralib/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/color_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/profile_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/segement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/util_clazz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/util_cv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/util_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/util_verbose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.849161 neura_library-0.0.5/src/neuralib/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.853161 neura_library-0.0.5/src/neuralib/wrapper/deeplabcut/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/deeplabcut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/deeplabcut/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/deeplabcut/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.853161 neura_library-0.0.5/src/neuralib/wrapper/facemap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/facemap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/facemap/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/facemap/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.853161 neura_library-0.0.5/src/neuralib/wrapper/rastermap/
+-rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/rastermap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-08 15:22:40.000000 neura_library-0.0.5/src/neuralib/wrapper/rastermap/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:22:47.853161 neura_library-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_argp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_argp_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_csv_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_persistence_autoinc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_protocol_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_pyvstim_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62204 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_stimpy_bitbucket_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16421 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_stimpy_github_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-08 15:22:40.000000 neura_library-0.0.5/test/test_util_func.py
```

### Comparing `neura_library-0.0.4/LICENSE` & `neura_library-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/PKG-INFO` & `neura_library-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neura-library
-Version: 0.0.4
+Version: 0.0.5
 Summary: Utility tools for system neuroscience research, including Open Source Wrapper or Parser
 Author-email: Yu-Ting Wei <ytsimon2004@gmail.com>, Ta-Shun Su <antoniost29@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, YT.WEI
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `neura_library-0.0.4/README.md` & `neura_library-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/pyproject.toml` & `neura_library-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "neura-library"
-version = "0.0.4"
+version = "0.0.5"
 requires-python = ">=3.9"
 description = "Utility tools for system neuroscience research, including Open Source Wrapper or Parser"
 authors = [
     { name = "Yu-Ting Wei", email = "ytsimon2004@gmail.com" },
     { name = "Ta-Shun Su", email = "antoniost29@gmail.com" }
 ]
 license = { file = "LICENSE" }
```

### Comparing `neura_library-0.0.4/src/neura_library.egg-info/PKG-INFO` & `neura_library-0.0.5/src/neura_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neura-library
-Version: 0.0.4
+Version: 0.0.5
 Summary: Utility tools for system neuroscience research, including Open Source Wrapper or Parser
 Author-email: Yu-Ting Wei <ytsimon2004@gmail.com>, Ta-Shun Su <antoniost29@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, YT.WEI
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `neura_library-0.0.4/src/neura_library.egg-info/SOURCES.txt` & `neura_library-0.0.5/src/neura_library.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 src/neura_library.egg-info/top_level.txt
 src/neuralib/__init__.py
 src/neuralib/argp/__init__.py
 src/neuralib/argp/_type.py
 src/neuralib/argp/core.py
 src/neuralib/argp/dispatch.py
 src/neuralib/atlas/__init__.py
-src/neuralib/atlas/allen.py
+src/neuralib/atlas/_structure.py
+src/neuralib/atlas/data.py
 src/neuralib/atlas/map.py
 src/neuralib/atlas/plot.py
 src/neuralib/atlas/type.py
 src/neuralib/atlas/util.py
 src/neuralib/atlas/view.py
 src/neuralib/atlas/brainrender/__init__.py
 src/neuralib/atlas/brainrender/core.py
@@ -53,20 +54,23 @@
 src/neuralib/calimg/scan_image/__init__.py
 src/neuralib/calimg/scan_image/wrapper.py
 src/neuralib/calimg/scanbox/__init__.py
 src/neuralib/calimg/scanbox/core.py
 src/neuralib/calimg/scanbox/viewer.py
 src/neuralib/calimg/suite2p/__init__.py
 src/neuralib/calimg/suite2p/core.py
+src/neuralib/calimg/suite2p/plot.py
 src/neuralib/calimg/suite2p/signals.py
 src/neuralib/imglib/__init__.py
+src/neuralib/imglib/color.py
 src/neuralib/imglib/factory.py
 src/neuralib/imglib/io.py
 src/neuralib/imglib/labeller.py
 src/neuralib/imglib/norm.py
+src/neuralib/imglib/transform.py
 src/neuralib/model/__init__.py
 src/neuralib/model/bayes_decoding/__init__.py
 src/neuralib/model/bayes_decoding/position.py
 src/neuralib/persistence/__init__.py
 src/neuralib/persistence/cli_persistence.py
 src/neuralib/persistence/persistence.py
 src/neuralib/plot/__init__.py
@@ -117,14 +121,15 @@
 src/neuralib/util/gpu.py
 src/neuralib/util/io.py
 src/neuralib/util/json.py
 src/neuralib/util/profile_test.py
 src/neuralib/util/segement.py
 src/neuralib/util/table.py
 src/neuralib/util/tqdm.py
+src/neuralib/util/util_clazz.py
 src/neuralib/util/util_cv2.py
 src/neuralib/util/util_type.py
 src/neuralib/util/util_verbose.py
 src/neuralib/util/utils.py
 src/neuralib/util/version.py
 src/neuralib/wrapper/__init__.py
 src/neuralib/wrapper/deeplabcut/__init__.py
@@ -138,8 +143,9 @@
 test/test_argp.py
 test/test_argp_dispatch.py
 test/test_csv_context_manager.py
 test/test_persistence_autoinc.py
 test/test_protocol_parser.py
 test/test_pyvstim_parser.py
 test/test_stimpy_bitbucket_parser.py
-test/test_stimpy_github_parser.py
+test/test_stimpy_github_parser.py
+test/test_util_func.py
```

### Comparing `neura_library-0.0.4/src/neuralib/argp/__init__.py` & `neura_library-0.0.5/src/neuralib/argp/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/argp/_type.py` & `neura_library-0.0.5/src/neuralib/argp/_type.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/argp/core.py` & `neura_library-0.0.5/src/neuralib/argp/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/argp/dispatch.py` & `neura_library-0.0.5/src/neuralib/argp/dispatch.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/atlas/allen.py` & `neura_library-0.0.5/src/neuralib/atlas/ccf/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,275 +1,192 @@
-from __future__ import annotations
-
-import io
-from io import BytesIO
-from pathlib import Path
-from pprint import pprint
-from typing import ClassVar, TypedDict, Literal
-
-import allensdk.core.structure_tree
-import numpy as np
-import pandas as pd
-import polars as pl
-from allensdk.core.reference_space_cache import ReferenceSpaceCache
-
-from neuralib.atlas.util import PLANE_TYPE, ALLEN_SOURCE_TYPE
-from neuralib.atlas.view import AbstractSliceView
-from neuralib.util.io import CCF_CACHE_DIRECTORY
-from neuralib.util.tqdm import download_with_tqdm
-from neuralib.util.util_type import PathLike, DataFrame
-from neuralib.util.util_verbose import fprint
-from neuralib.util.utils import uglob
-
-__all__ = ['AllenReferenceWrapper',
-           'create_allen_structure_dict']
-
-
-class StructureTreeDict(TypedDict):
-    """allen structure tree dict"""
-    acronym: str
-    graph_id: int
-    graph_order: int
-    id: int
-    name: str
-    structure_id_path: list[int]
-    structure_set_ids: list[int]
-    rgb_triplet: list[int]
-
-
-class AllenReferenceWrapper:
-    """Class for load the data in allen"""
-
-    REFERENCE_SPACE_KEY: ClassVar[str] = 'ccf_2017'
-    STRUCTURE_GRAPH_ID: ClassVar[int] = 1
-
-    def __init__(self,
-                 resolution: int = 10,
-                 output: PathLike | None = None):
-        """
-        :param resolution: resolution in um
-        :param output: output directory for downloading cache. By default, save in ``CCF_CACHE_DIRECTORY``
-        """
-
-        if output is None:
-            output = CCF_CACHE_DIRECTORY
-
-        if not output.exists():
-            output.mkdir(parents=True, exist_ok=True)
-
-        self.source_root = Path(output)
-        self.reference = ReferenceSpaceCache(resolution,
-                                             self.REFERENCE_SPACE_KEY,
-                                             manifest=self.source_root / 'manifest.json')
-
-    # ============== #
-    # Structure Tree #
-    # ============== #
-
-    @classmethod
-    def load_structure_tree(cls, version: Literal['2017', 'old'] = '2017') -> pl.DataFrame:
-        """
-        Load structure tree dataframe
-
-        :param version: {'2017', 'old'}
-        :return: structure tree dataframe
-
-        ::
-
-            ┌───────────┬──────────┬───────────────────────────────┬─────────┬──────────┬─────────────┬───────────────┬────────┬─────────────────────┬───────┬──────────┬─────────────┬───────────────────┬───────────────────┬─────────────────────────┬──────────────────────────────┬────────┬───────────┬──────────────────────┬──────────────┬───────────────────────────────┐
-            │ id        ┆ atlas_id ┆ name                          ┆ acronym ┆ st_level ┆ ontology_id ┆ hemisphere_id ┆ weight ┆ parent_structure_id ┆ depth ┆ graph_id ┆ graph_order ┆ structure_id_path ┆ color_hex_triplet ┆ neuro_name_structure_id ┆ neuro_name_structure_id_path ┆ failed ┆ sphinx_id ┆ structure_name_facet ┆ failed_facet ┆ safe_name                     │
-            │ ---       ┆ ---      ┆ ---                           ┆ ---     ┆ ---      ┆ ---         ┆ ---           ┆ ---    ┆ ---                 ┆ ---   ┆ ---      ┆ ---         ┆ ---               ┆ ---               ┆ ---                     ┆ ---                          ┆ ---    ┆ ---       ┆ ---                  ┆ ---          ┆ ---                           │
-            │ i64       ┆ f64      ┆ str                           ┆ str     ┆ str      ┆ i64         ┆ i64           ┆ i64    ┆ f64                 ┆ i64   ┆ i64      ┆ i64         ┆ list[i64]         ┆ str               ┆ str                     ┆ str                          ┆ str    ┆ i64       ┆ i64                  ┆ i64          ┆ str                           │
-            ╞═══════════╪══════════╪═══════════════════════════════╪═════════╪══════════╪═════════════╪═══════════════╪════════╪═════════════════════╪═══════╪══════════╪═════════════╪═══════════════════╪═══════════════════╪═════════════════════════╪══════════════════════════════╪════════╪═══════════╪══════════════════════╪══════════════╪═══════════════════════════════╡
-            │ 997       ┆ -1.0     ┆ root                          ┆ root    ┆ null     ┆ 1           ┆ 3             ┆ 8690   ┆ -1.0                ┆ 0     ┆ 1        ┆ 0           ┆ [997]             ┆ FFFFFF            ┆ null                    ┆ null                         ┆ f      ┆ 1         ┆ 385153371            ┆ 734881840    ┆ root                          │
-            │ 8         ┆ 0.0      ┆ Basic cell groups and regions ┆ grey    ┆ null     ┆ 1           ┆ 3             ┆ 8690   ┆ 997.0               ┆ 1     ┆ 1        ┆ 1           ┆ [997, 8]          ┆ BFDAE3            ┆ null                    ┆ null                         ┆ f      ┆ 2         ┆ 2244697386           ┆ 734881840    ┆ Basic cell groups and regions │
-            │ …         ┆ …        ┆ …                             ┆ …       ┆ …        ┆ …           ┆ …             ┆ …      ┆ …                   ┆ …     ┆ …        ┆ …           ┆ …                 ┆ …                 ┆ …                       ┆ …                            ┆ …      ┆ …         ┆ …                    ┆ …            ┆ …                             │
-            │ 65        ┆ 715.0    ┆ parafloccular sulcus          ┆ pfs     ┆ null     ┆ 1           ┆ 3             ┆ 8690   ┆ 1040.0              ┆ 3     ┆ 1        ┆ 1324        ┆ [997, 1024, … 65] ┆ AAAAAA            ┆ null                    ┆ null                         ┆ f      ┆ 1325      ┆ 771629690            ┆ 734881840    ┆ parafloccular sulcus          │
-            │ 624       ┆ 926.0    ┆ Interpeduncular fossa         ┆ IPF     ┆ null     ┆ 1           ┆ 3             ┆ 8690   ┆ 1024.0              ┆ 2     ┆ 1        ┆ 1325        ┆ [997, 1024, 624]  ┆ AAAAAA            ┆ null                    ┆ null                         ┆ f      ┆ 1326      ┆ 1476705011           ┆ 734881840    ┆ Interpeduncular fossa         │
-            │ 304325711 ┆ -2.0     ┆ retina                        ┆ retina  ┆ null     ┆ 1           ┆ 3             ┆ 8690   ┆ 997.0               ┆ 1     ┆ 1        ┆ 1326        ┆ [997, 304325711]  ┆ 7F2E7E            ┆ null                    ┆ null                         ┆ f      ┆ 1327      ┆ 3295290839           ┆ 734881840    ┆ retina                        │
-            └───────────┴──────────┴───────────────────────────────┴─────────┴──────────┴─────────────┴───────────────┴────────┴─────────────────────┴───────┴──────────┴─────────────┴───────────────────┴───────────────────┴─────────────────────────┴──────────────────────────────┴────────┴───────────┴──────────────────────┴──────────────┴───────────────────────────────┘
-
-        """
-        if version == '2017':
-            filename = 'structure_tree_safe_2017.csv'
-        elif version == 'old':
-            filename = 'structure_tree_safe.csv'
-        else:
-            raise ValueError('')
-
-        #
-        filepath = CCF_CACHE_DIRECTORY / filename
-        if not filepath.exists():
-            cls._request_structure_tree(filepath, filename)
-
-        ret = (pl.read_csv(filepath)
-               .with_columns(pl.col('parent_structure_id').fill_null(-1))
-               .with_columns(pl.col('structure_id_path').map_elements(lambda it: tuple(map(int, it[1:-1].split('/'))))))
-        #
-        if '2017' in Path(filepath).name:
-            ret = ret.with_columns(pl.col('atlas_id').fill_null(-2))
-        else:
-            ret = ret.with_columns(pl.col('name').alias('safe_name'))
-
-        return ret
-
-    @classmethod
-    def _request_structure_tree(cls, dest: PathLike, filename: str) -> Path:
-        url = f'https://raw.githubusercontent.com/cortex-lab/allenCCF/master/{filename}'
-        resp = download_with_tqdm(url)
-
-        if resp.status_code == 200:
-            df = pd.read_csv(io.BytesIO(resp.content))
-            pl.from_pandas(df).write_csv(dest)
-            fprint(f'DOWNLOAD! {filename} in {dest.parent}', vtype='io')
-
-        else:
-            raise RuntimeError('download structure FAIL!')
-
-        return dest
-
-    def structure_tree(self) -> allensdk.core.structure_tree.StructureTree:
-        return self.reference.get_structure_tree(structure_graph_id=self.STRUCTURE_GRAPH_ID)
-
-    def get_structures_by_name(self, name: list[str]) -> list[StructureTreeDict]:
-        return self.structure_tree().get_structures_by_name(name)
-
-    # ========== #
-    # Annotation #
-    # ========== #
-
-    @classmethod
-    def load_slice_view(cls,
-                        source: ALLEN_SOURCE_TYPE,
-                        plane_type: PLANE_TYPE,
-                        resolution: int = 10) -> AbstractSliceView:
-        """
-        Load the slice view
-
-        :param source: ``ALLEN_SOURCE_TYPE``
-        :param plane_type: ``PLANE_TYPE``
-        :param resolution: resolution in um
-        :return: :class:`~neuralib.atlas.view.AbstractSliceView()`
-        """
-
-        if source in ('npy', 'nrrd'):
-            pattern = f'annotation*{resolution}*.{source}'
-
-            try:
-                f = uglob(CCF_CACHE_DIRECTORY, pattern)
-            except FileNotFoundError:
-                f = cls._request_allen_src(source, resolution, CCF_CACHE_DIRECTORY)
-
-            if source == 'npy':
-                data = np.load(f)
-            elif source == 'nrrd':
-                import nrrd
-                data = nrrd.read(f)[0]
-            else:
-                raise ValueError('')
-
-        elif source == 'template':
-            f = CCF_CACHE_DIRECTORY / f'template_volume_{resolution}um.npy'
-            if not f.exists():
-                f = cls._request_allen_src('template', resolution, CCF_CACHE_DIRECTORY)
-            data = np.load(f)
-
-        else:
-            raise ValueError('')
-
-        return AbstractSliceView(source, plane_type, resolution, data)
-
-    @classmethod
-    def _request_allen_src(cls, src_type: ALLEN_SOURCE_TYPE,
-                           resolution: int,
-                           dest: PathLike) -> Path:
-        """
-
-        :param src_type: ALLEN_SOURCE_TYPE = Literal['npy', 'nrrd', 'template']
-                * nrrd: source directly from Alleninstitute
-                    Seealso: https://download.alleninstitute.org/informatics-archive/current-release/mouse_ccf/annotation/
-                * annotation / template: adapted version from cortex-lab
-                    Seealso: https://github.com/cortex-lab/allenCCF
-        :param resolution:
-        :param dest:
-        :return:
-        """
-
-        if src_type == 'nrrd':
-            from allensdk.api.queries.mouse_connectivity_api import MouseConnectivityApi
-            mcapi = MouseConnectivityApi()
-            version = MouseConnectivityApi.CCF_VERSION_DEFAULT
-            filename = f'annotation_{resolution}.nrrd'
-            mcapi.download_annotation_volume(version, resolution, dest / filename)
-            out = Path(dest) / filename
-            fprint(f'DOWNLOAD! {filename} in {dest}', vtype='io')
-
-        elif src_type in ('annotation', 'template'):
-
-            if src_type == 'annotation':
-                url = 'https://figshare.com/ndownloader/files/44925493'
-                filename = 'annotation_volume_10um_by_index.npy'
-            elif src_type == 'template':
-                url = 'https://figshare.com/ndownloader/files/44925496'
-                filename = 'template_volume_10um.npy'
-            else:
-                raise ValueError('')
-
-            out = Path(dest) / filename
-            fprint(f'DOWNLOADING... {filename} from {url}', vtype='io')
-
-            resp = download_with_tqdm(url)
-            if resp.status_code == 200:
-                fprint(f'DOWNLOAD! {filename} in {dest}', vtype='io')
-
-                with BytesIO(resp.content) as f:
-
-                    data = np.load(f, allow_pickle=True)
-                np.save(out, data)
-
-            else:
-                raise RuntimeError('download allen src FAIL!')
-        else:
-            raise ValueError('')
-
-        return out
-
-    # ====== #
-    # Others #
-    # ====== #
-
-    @classmethod
-    def load_structure_voxel(cls, to_pandas=False) -> DataFrame:
-        """TODO not test yet"""
-        file = CCF_CACHE_DIRECTORY / 'voxel_count_and_differences.csv'
-        df = (
-            pl.read_csv(file)
-            .select(pl.col(['acronym', 'name', 'total_voxel_count']))
-            .drop_nulls()
-            .sort('total_voxel_count', descending=True)
+"""
+Atlas CCF
+===============
+
+:author:
+    Yu-Ting Wei
+
+
+This module provide analysis pipeline for the data acquired from allenccf mouse brain registration tool
+
+specifically for the ROIs distribution across the whole brain
+
+.. seealso:: `<https://github.com/cortex-lab/allenCCF>`_
+
+
+Data Folder structure should follow::
+
+    ANIMAL_001/ (root)
+        ├── raw/ (optional)
+        ├── zproj/
+        │    └── ANIMAL_001_g*_s*_{channel}.tif
+        ├── roi/
+        │    └── ANIMAL_001_g*_s*_{channel}.roi
+        ├── roi_cpose/
+        │    └── ANIMAL_001_g*_s*_{channel}.roi
+        ├── resize/ (src for the allenccf)
+        │    ├── ANIMAL_001_g*_s*_resize.tif
+        │    └── processed/
+        │           ├── ANIMAL_001_g*_s*_resize_processed.tif
+        │           └── transformations/
+        │                 ├── ANIMAL_001_g*_s*_resize_processed_transformed.tif
+        │                 ├── ANIMAL_001_g*_s*_resize_processed_transform_data.mat
+        │                 └── labelled_regions/
+        │                       ├── {*channel}_roitable.csv
+        │                       └── parsed_data /
+        │                             └── parsed_csv_merge.csv
+        │
+        └── output_files/ (for generate output fig)
+
+
+
+Example Raw data csv (``{*channel}_roitable.csv`` in the folder structure)::
+
+    ┌───────────────────────────────────┬─────────┬─────────────┬─────────────┬─────────────┬─────────┐
+    │ name                              ┆ acronym ┆ AP_location ┆ DV_location ┆ ML_location ┆ avIndex │
+    │ ---                               ┆ ---     ┆ ---         ┆ ---         ┆ ---         ┆ ---     │
+    │ str                               ┆ str     ┆ f64         ┆ f64         ┆ f64         ┆ i64     │
+    ╞═══════════════════════════════════╪═════════╪═════════════╪═════════════╪═════════════╪═════════╡
+    │ Entorhinal area lateral part lay… ┆ ENTl5   ┆ -4.35       ┆ 3.98        ┆ 4.23        ┆ 504     │
+    │ Entorhinal area lateral part lay… ┆ ENTl3   ┆ -4.35       ┆ 4.09        ┆ 4.25        ┆ 501     │
+    │ Entorhinal area lateral part lay… ┆ ENTl2   ┆ -4.35       ┆ 3.42        ┆ 4.44        ┆ 497     │
+    │ Entorhinal area lateral part lay… ┆ ENTl2   ┆ -4.35       ┆ 3.56        ┆ 4.46        ┆ 497     │
+    │ Primary visual area layer 6a      ┆ VISp6a  ┆ -4.23       ┆ 1.65        ┆ -2.28       ┆ 191     │
+    │ …                                 ┆ …       ┆ …           ┆ …           ┆ …           ┆ …       │
+    │ Laterointermediate area layer 4   ┆ VISli4  ┆ -3.54       ┆ 2.04        ┆ 4.01        ┆ 210     │
+    │ Temporal association areas layer… ┆ TEa6b   ┆ -3.54       ┆ 2.89        ┆ 4.02        ┆ 367     │
+    │ alveus                            ┆ alv     ┆ -3.54       ┆ 3.52        ┆ 4.14        ┆ 1246    │
+    │ Field CA1                         ┆ CA1     ┆ -3.54       ┆ 3.61        ┆ 4.15        ┆ 458     │
+    │ optic radiation                   ┆ or      ┆ -3.54       ┆ 3.77        ┆ 4.25        ┆ 1217    │
+    └───────────────────────────────────┴─────────┴─────────────┴─────────────┴─────────────┴─────────┘
+
+
+Parsing Pipeline
+-------------------
+
+Do the following procedure
+
+1. concat roi from different channels
+2. add column(fields) for user-specific manner. e.g., 'channel', 'source', ...
+3. converge to hierarchical level / family based on allen brain region tree (Wang et al 2020).
+   see :meth:`~neuralib.atlas.map.merge_until_level()` in `neuralib.atlas.map.py <https://github.com/ytsimon2004/neuralib/blob/main/src/neuralib/atlas/map.py>`_
+
+
+.. code-block:: python
+
+    from neuralib.atlas.ccf.classifier import UserInjectionConfig, RoiClassifier
+    from neuralib.atlas.ccf.core import AbstractCCFDir
+
+    # prepare ccf folder structure
+    root = ...
+    ccf_dir = AbstractCCFDir(root, with_overlap_sources=True)  # assume count overlap channel rois separately
+
+    # example of injection configuration
+    USER_CONFIG = UserInjectionConfig(
+        area='RSP',
+        hemisphere='ipsi',
+        ignore=True,
+        fluor_repr=dict(
+            rfp='pRSC',
+            gfp='aRSC',
+            overlap='overlap'
         )
+    )
+
+    classifier = RoiClassifier(ccf_dir, merge_level=2, plane='coronal', config=USER_CONFIG)
+    print(classifier.parsed_df)
+
+
+output::
+
+    ┌───────────────────────────────────┬─────────┬─────────────┬─────────────┬─────────────┬─────────┬─────────┬────────┬───────────────────────────┬──────────────┬────────┬────────────┬────────────┬────────────┬────────────┬────────────┬───────────┐
+    │ name                              ┆ acronym ┆ AP_location ┆ DV_location ┆ ML_location ┆ avIndex ┆ channel ┆ source ┆ abbr                      ┆ acronym_abbr ┆ hemi.  ┆ merge_ac_0 ┆ merge_ac_1 ┆ merge_ac_2 ┆ merge_ac_3 ┆ merge_ac_4 ┆ family    │
+    │ ---                               ┆ ---     ┆ ---         ┆ ---         ┆ ---         ┆ ---     ┆ ---     ┆ ---    ┆ ---                       ┆ ---          ┆ ---    ┆ ---        ┆ ---        ┆ ---        ┆ ---        ┆ ---        ┆ ---       │
+    │ str                               ┆ str     ┆ f64         ┆ f64         ┆ f64         ┆ i64     ┆ str     ┆ str    ┆ str                       ┆ str          ┆ str    ┆ str        ┆ str        ┆ str        ┆ str        ┆ str        ┆ str       │
+    ╞═══════════════════════════════════╪═════════╪═════════════╪═════════════╪═════════════╪═════════╪═════════╪════════╪═══════════════════════════╪══════════════╪════════╪════════════╪════════════╪════════════╪════════════╪════════════╪═══════════╡
+    │ Ectorhinal area/Layer 5           ┆ ECT5    ┆ -3.03       ┆ 4.34        ┆ -4.5        ┆ 377     ┆ gfp     ┆ aRSC   ┆ Ectorhinal area           ┆ ECT          ┆ contra ┆ ECT        ┆ ECT        ┆ ECT        ┆ ECT        ┆ ECT        ┆ ISOCORTEX │
+    │ Perirhinal area layer 6a          ┆ PERI6a  ┆ -3.03       ┆ 4.42        ┆ -4.37       ┆ 372     ┆ gfp     ┆ aRSC   ┆ Perirhinal area           ┆ PERI         ┆ contra ┆ PERI       ┆ PERI       ┆ PERI       ┆ PERI       ┆ PERI       ┆ ISOCORTEX │
+    │ …                                 ┆ …       ┆ …           ┆ …           ┆ …           ┆ …       ┆ …       ┆ …      ┆ …                         ┆ …            ┆ …      ┆ …          ┆ …          ┆ …          ┆ …          ┆ …          ┆ …         │
+    │ Ventral auditory area layer 6a    ┆ AUDv6a  ┆ -2.91       ┆ 3.52        ┆ 4.46        ┆ 156     ┆ rfp     ┆ pRSC   ┆ Ventral auditory area     ┆ AUDv         ┆ ipsi   ┆ AUD        ┆ AUD        ┆ AUD        ┆ AUD        ┆ AUDv       ┆ ISOCORTEX │
+    │ Ectorhinal area/Layer 6a          ┆ ECT6a   ┆ -2.91       ┆ 4.14        ┆ 4.47        ┆ 378     ┆ rfp     ┆ pRSC   ┆ Ectorhinal area           ┆ ECT          ┆ ipsi   ┆ ECT        ┆ ECT        ┆ ECT        ┆ ECT        ┆ ECT        ┆ ISOCORTEX │
+    │ Temporal association areas layer… ┆ TEa5    ┆ -2.91       ┆ 4.02        ┆ 4.55        ┆ 365     ┆ rfp     ┆ pRSC   ┆ Temporal association area ┆ TEa          ┆ ipsi   ┆ TEa        ┆ TEa        ┆ TEa        ┆ TEa        ┆ TEa        ┆ ISOCORTEX │
+    └───────────────────────────────────┴─────────┴─────────────┴─────────────┴─────────────┴─────────┴─────────┴────────┴───────────────────────────┴──────────────┴────────┴────────────┴────────────┴────────────┴────────────┴────────────┴───────────┘
+
+
+Do the ROIs normalization
+---------------------
+
+three normalization provided (:class:`~neuralib.atlas.ccf.norm.MouseBrainRoiNormHandler`)
+
+1. ``channel``: normalize to fraction of rois for a specific color fluorescence channel
+
+2. ``volume``: normalize to the volume size per region (cellatlas-based)
+
+3. ``cell``: normalize to the total cell counts per region (cellatlas-based)
+
+
+.. code-block:: python
+
+    from neuralib.atlas.ccf.classifier import RoiClassifiedNormTable
+    from neuralib.atlas.ccf.norm import MouseBrainRoiNormHandler
+
+    norm = MouseBrainRoiNormHandler(norm_type='volume')
+
+    # use the classifier constructed above
+    norm_data: RoiClassifiedNormTable = classifier.get_classified_data(norm)
+    print(norm_data.data)
+
+
+output::
+
+    ┌─────────┬────────────┬────────┬───────────┬───┬───────────┬───────────┬─────────────────┬────────┐
+    │ channel ┆ merge_ac_2 ┆ n_rois ┆ percent   ┆ … ┆ Volumes   ┆ n_neurons ┆ *volume_norm_n_r┆ animal │
+    │ ---     ┆ ---        ┆ ---    ┆ ---       ┆   ┆ [mm^3]    ┆ ---       ┆ ois             ┆ ---    │
+    │ str     ┆ str        ┆ i64    ┆ f64       ┆   ┆ ---       ┆ i64       ┆ ---             ┆ str    │
+    │         ┆            ┆        ┆           ┆   ┆ f64       ┆           ┆ f64             ┆        │
+    ╞═════════╪════════════╪════════╪═══════════╪═══╪═══════════╪═══════════╪═════════════════╪════════╡
+    │ overlap ┆ ACA        ┆ 423    ┆ 30.344333 ┆ … ┆ 5.222484  ┆ 337372    ┆ 80.995934       ┆ YW051  │
+    │ gfp     ┆ MO         ┆ 3352   ┆ 24.545987 ┆ … ┆ 22.248234 ┆ 985411    ┆ 150.663641      ┆ YW051  │
+    │ rfp     ┆ ACA        ┆ 1383   ┆ 23.791502 ┆ … ┆ 5.222484  ┆ 337372    ┆ 264.816494      ┆ YW051  │
+    │ gfp     ┆ ACA        ┆ 3130   ┆ 22.920328 ┆ … ┆ 5.222484  ┆ 337372    ┆ 599.331616      ┆ YW051  │
+    │ …       ┆ …          ┆ …      ┆ …         ┆ … ┆ …         ┆ …         ┆ …               ┆ …      │
+    │ overlap ┆ SS         ┆ 1      ┆ 0.071736  ┆ … ┆ 37.177937 ┆ 2384622   ┆ 0.026898        ┆ YW051  │
+    │ overlap ┆ ECT        ┆ 1      ┆ 0.071736  ┆ … ┆ 3.457703  ┆ 387378    ┆ 0.289209        ┆ YW051  │
+    │ overlap ┆ TEa        ┆ 1      ┆ 0.071736  ┆ … ┆ 3.860953  ┆ 386396    ┆ 0.259003        ┆ YW051  │
+    │ rfp     ┆ TT         ┆ 1      ┆ 0.017203  ┆ … ┆ 1.734078  ┆ 124596    ┆ 0.576675        ┆ YW051  │
+    └─────────┴────────────┴────────┴───────────┴───┴───────────┴───────────┴─────────────────┴────────┘
+
+
+
+Do the ROI subregions query
+-----------------
+
+Example for query the ROIs in visual cortex
+
+.. code-block:: python
 
-        if to_pandas:
-            df = df.to_pandas()
+    from neuralib.atlas.ccf.query import RoiAreaQuery
 
-        return df
+    # use the classifier constructed above
+    df = classifier.parsed_df
+    result = RoiAreaQuery.by(df, 'VIS).get_subregion_result
+    print(result.data)
 
 
-# ==================== #
+output::
 
-def create_allen_structure_dict(verbose=False) -> dict[str, str]:
-    """
-    Get the acronym/name pairing from structure_tree.csv
+    ┌─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬────────┐
+    │ source  ┆ VISam   ┆ VISp    ┆ VISpm   ┆ VISl    ┆ VISal   ┆ VISpor  ┆ VISli   ┆ VISpl   ┆ VISC   │
+    │ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---    │
+    │ str     ┆ f64     ┆ f64     ┆ f64     ┆ f64     ┆ f64     ┆ f64     ┆ f64     ┆ f64     ┆ f64    │
+    ╞═════════╪═════════╪═════════╪═════════╪═════════╪═════════╪═════════╪═════════╪═════════╪════════╡
+    │ aRSC    ┆ 25.4669 ┆ 34.0318 ┆ 23.0979 ┆ 6.42369 ┆ 6.37813 ┆ 1.77676 ┆ 2.27790 ┆ 0.0     ┆ 0.5466 │
+    │         ┆ 7       ┆ 91      ┆ 5       ┆         ┆ 2       ┆ 5       ┆ 4       ┆         ┆ 97     │
+    │ pRSC    ┆ 15.1445 ┆ 36.1079 ┆ 29.5568 ┆ 10.7129 ┆ 3.04431 ┆ 2.38921 ┆ 1.92678 ┆ 1.07899 ┆ 0.0385 │
+    │         ┆ 09      ┆         ┆ 4       ┆ 09      ┆ 6       ┆         ┆ 2       ┆ 8       ┆ 36     │
+    │ overlap ┆ 48.5294 ┆ 8.82352 ┆ 31.25   ┆ 4.04411 ┆ 3.30882 ┆ 2.57352 ┆ 1.10294 ┆ 0.0     ┆ 0.3676 │
+    │         ┆ 12      ┆ 9       ┆         ┆ 8       ┆ 4       ┆ 9       ┆ 1       ┆         ┆ 47     │
+    └─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴────────┘
 
-    :return: key: acronym; value: full name
-    """
-    tree = AllenReferenceWrapper.load_structure_tree()
-    tree = tree.select('name', 'acronym').sort('name')
 
-    ret = {
-        acry: name
-        for name, acry in tree.iter_rows()
-    }
-    if verbose:
-        pprint(ret)
 
-    return ret
+"""
```

### Comparing `neura_library-0.0.4/src/neuralib/atlas/brainrender/__init__.py` & `neura_library-0.0.5/src/neuralib/atlas/brainrender/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/atlas/brainrender/core.py` & `neura_library-0.0.5/src/neuralib/atlas/brainrender/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/atlas/brainrender/main_app.py` & `neura_library-0.0.5/src/neuralib/atlas/brainrender/main_app.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/atlas/brainrender/probe_rst.py` & `neura_library-0.0.5/src/neuralib/atlas/brainrender/probe_rst.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/atlas/brainrender/roi_rst.py` & `neura_library-0.0.5/src/neuralib/atlas/brainrender/roi_rst.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/atlas/brainrender/util.py` & `neura_library-0.0.5/src/neuralib/atlas/brainrender/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/atlas/ccf/__init__.py` & `neura_library-0.0.5/src/neuralib/atlas/ccf/query.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,192 +1,240 @@
-"""
-Atlas CCF
-===============
+from __future__ import annotations
 
-:author:
-    Yu-Ting Wei
-
-
-This module provide analysis pipeline for the data acquired from allenccf mouse brain registration tool
-
-specifically for the ROIs distribution across the whole brain
-
-.. seealso:: `<https://github.com/cortex-lab/allenCCF>`_
-
-
-Data Folder structure should follow::
-
-    ANIMAL_001/ (root)
-        ├── raw/ (optional)
-        ├── zproj/
-        │    └── ANIMAL_001_g*_s*_{channel}.tif
-        ├── roi/
-        │    └── ANIMAL_001_g*_s*_{channel}.roi
-        ├── roi_cpose/
-        │    └── ANIMAL_001_g*_s*_{channel}.roi
-        ├── resize/ (src for the allenccf)
-        │    ├── ANIMAL_001_g*_s*_resize.tif
-        │    └── processed/
-        │           ├── ANIMAL_001_g*_s*_resize_processed.tif
-        │           └── transformations/
-        │                 ├── ANIMAL_001_g*_s*_resize_processed_transformed.tif
-        │                 ├── ANIMAL_001_g*_s*_resize_processed_transform_data.mat
-        │                 └── labelled_regions/
-        │                       ├── {*channel}_roitable.csv
-        │                       └── parsed_data /
-        │                             └── parsed_csv_merge.csv
-        │
-        └── output_files/ (for generate output fig)
-
-
-
-Example Raw data csv (``{*channel}_roitable.csv`` in the folder structure)::
-
-    ┌───────────────────────────────────┬─────────┬─────────────┬─────────────┬─────────────┬─────────┐
-    │ name                              ┆ acronym ┆ AP_location ┆ DV_location ┆ ML_location ┆ avIndex │
-    │ ---                               ┆ ---     ┆ ---         ┆ ---         ┆ ---         ┆ ---     │
-    │ str                               ┆ str     ┆ f64         ┆ f64         ┆ f64         ┆ i64     │
-    ╞═══════════════════════════════════╪═════════╪═════════════╪═════════════╪═════════════╪═════════╡
-    │ Entorhinal area lateral part lay… ┆ ENTl5   ┆ -4.35       ┆ 3.98        ┆ 4.23        ┆ 504     │
-    │ Entorhinal area lateral part lay… ┆ ENTl3   ┆ -4.35       ┆ 4.09        ┆ 4.25        ┆ 501     │
-    │ Entorhinal area lateral part lay… ┆ ENTl2   ┆ -4.35       ┆ 3.42        ┆ 4.44        ┆ 497     │
-    │ Entorhinal area lateral part lay… ┆ ENTl2   ┆ -4.35       ┆ 3.56        ┆ 4.46        ┆ 497     │
-    │ Primary visual area layer 6a      ┆ VISp6a  ┆ -4.23       ┆ 1.65        ┆ -2.28       ┆ 191     │
-    │ …                                 ┆ …       ┆ …           ┆ …           ┆ …           ┆ …       │
-    │ Laterointermediate area layer 4   ┆ VISli4  ┆ -3.54       ┆ 2.04        ┆ 4.01        ┆ 210     │
-    │ Temporal association areas layer… ┆ TEa6b   ┆ -3.54       ┆ 2.89        ┆ 4.02        ┆ 367     │
-    │ alveus                            ┆ alv     ┆ -3.54       ┆ 3.52        ┆ 4.14        ┆ 1246    │
-    │ Field CA1                         ┆ CA1     ┆ -3.54       ┆ 3.61        ┆ 4.15        ┆ 458     │
-    │ optic radiation                   ┆ or      ┆ -3.54       ┆ 3.77        ┆ 4.25        ┆ 1217    │
-    └───────────────────────────────────┴─────────┴─────────────┴─────────────┴─────────────┴─────────┘
-
-
-Parsing Pipeline
--------------------
-
-Do the following procedure
-
-1. concat roi from different channels
-2. add column(fields) for user-specific manner. e.g., 'channel', 'source', ...
-3. converge to hierarchical level / family based on allen brain region tree (Wang et al 2020).
-   see :meth:`~neuralib.atlas.map.merge_until_level()` in `neuralib.atlas.map.py <https://github.com/ytsimon2004/neuralib/blob/main/src/neuralib/atlas/map.py>`_
-
-
-.. code-block:: python
-
-    from neuralib.atlas.ccf.classifier import UserInjectionConfig, RoiClassifier
-    from neuralib.atlas.ccf.core import AbstractCCFDir
-
-    # prepare ccf folder structure
-    root = ...
-    ccf_dir = AbstractCCFDir(root, with_overlap_sources=True)  # assume count overlap channel rois separately
-
-    # example of injection configuration
-    USER_CONFIG = UserInjectionConfig(
-        area='RSP',
-        hemisphere='ipsi',
-        ignore=True,
-        fluor_repr=dict(
-            rfp='pRSC',
-            gfp='aRSC',
-            overlap='overlap'
-        )
-    )
-
-    classifier = RoiClassifier(ccf_dir, merge_level=2, plane='coronal', config=USER_CONFIG)
-    print(classifier.parsed_df)
-
-
-output::
-
-    ┌───────────────────────────────────┬─────────┬─────────────┬─────────────┬─────────────┬─────────┬─────────┬────────┬───────────────────────────┬──────────────┬────────┬────────────┬────────────┬────────────┬────────────┬────────────┬───────────┐
-    │ name                              ┆ acronym ┆ AP_location ┆ DV_location ┆ ML_location ┆ avIndex ┆ channel ┆ source ┆ abbr                      ┆ acronym_abbr ┆ hemi.  ┆ merge_ac_0 ┆ merge_ac_1 ┆ merge_ac_2 ┆ merge_ac_3 ┆ merge_ac_4 ┆ family    │
-    │ ---                               ┆ ---     ┆ ---         ┆ ---         ┆ ---         ┆ ---     ┆ ---     ┆ ---    ┆ ---                       ┆ ---          ┆ ---    ┆ ---        ┆ ---        ┆ ---        ┆ ---        ┆ ---        ┆ ---       │
-    │ str                               ┆ str     ┆ f64         ┆ f64         ┆ f64         ┆ i64     ┆ str     ┆ str    ┆ str                       ┆ str          ┆ str    ┆ str        ┆ str        ┆ str        ┆ str        ┆ str        ┆ str       │
-    ╞═══════════════════════════════════╪═════════╪═════════════╪═════════════╪═════════════╪═════════╪═════════╪════════╪═══════════════════════════╪══════════════╪════════╪════════════╪════════════╪════════════╪════════════╪════════════╪═══════════╡
-    │ Ectorhinal area/Layer 5           ┆ ECT5    ┆ -3.03       ┆ 4.34        ┆ -4.5        ┆ 377     ┆ gfp     ┆ aRSC   ┆ Ectorhinal area           ┆ ECT          ┆ contra ┆ ECT        ┆ ECT        ┆ ECT        ┆ ECT        ┆ ECT        ┆ ISOCORTEX │
-    │ Perirhinal area layer 6a          ┆ PERI6a  ┆ -3.03       ┆ 4.42        ┆ -4.37       ┆ 372     ┆ gfp     ┆ aRSC   ┆ Perirhinal area           ┆ PERI         ┆ contra ┆ PERI       ┆ PERI       ┆ PERI       ┆ PERI       ┆ PERI       ┆ ISOCORTEX │
-    │ …                                 ┆ …       ┆ …           ┆ …           ┆ …           ┆ …       ┆ …       ┆ …      ┆ …                         ┆ …            ┆ …      ┆ …          ┆ …          ┆ …          ┆ …          ┆ …          ┆ …         │
-    │ Ventral auditory area layer 6a    ┆ AUDv6a  ┆ -2.91       ┆ 3.52        ┆ 4.46        ┆ 156     ┆ rfp     ┆ pRSC   ┆ Ventral auditory area     ┆ AUDv         ┆ ipsi   ┆ AUD        ┆ AUD        ┆ AUD        ┆ AUD        ┆ AUDv       ┆ ISOCORTEX │
-    │ Ectorhinal area/Layer 6a          ┆ ECT6a   ┆ -2.91       ┆ 4.14        ┆ 4.47        ┆ 378     ┆ rfp     ┆ pRSC   ┆ Ectorhinal area           ┆ ECT          ┆ ipsi   ┆ ECT        ┆ ECT        ┆ ECT        ┆ ECT        ┆ ECT        ┆ ISOCORTEX │
-    │ Temporal association areas layer… ┆ TEa5    ┆ -2.91       ┆ 4.02        ┆ 4.55        ┆ 365     ┆ rfp     ┆ pRSC   ┆ Temporal association area ┆ TEa          ┆ ipsi   ┆ TEa        ┆ TEa        ┆ TEa        ┆ TEa        ┆ TEa        ┆ ISOCORTEX │
-    └───────────────────────────────────┴─────────┴─────────────┴─────────────┴─────────────┴─────────┴─────────┴────────┴───────────────────────────┴──────────────┴────────┴────────────┴────────────┴────────────┴────────────┴────────────┴───────────┘
-
-
-Do the ROIs normalization
----------------------
-
-three normalization provided (:class:`~neuralib.atlas.ccf.norm.MouseBrainRoiNormHandler`)
-
-1. ``channel``: normalize to fraction of rois for a specific color fluorescence channel
-
-2. ``volume``: normalize to the volume size per region (cellatlas-based)
-
-3. ``cell``: normalize to the total cell counts per region (cellatlas-based)
-
-
-.. code-block:: python
-
-    from neuralib.atlas.ccf.classifier import RoiClassifiedNormTable
-    from neuralib.atlas.ccf.norm import MouseBrainRoiNormHandler
-
-    norm = MouseBrainRoiNormHandler(norm_type='volume')
-
-    # use the classifier constructed above
-    norm_data: RoiClassifiedNormTable = classifier.get_classified_data(norm)
-    print(norm_data.data)
-
-
-output::
-
-    ┌─────────┬────────────┬────────┬───────────┬───┬───────────┬───────────┬─────────────────┬────────┐
-    │ channel ┆ merge_ac_2 ┆ n_rois ┆ percent   ┆ … ┆ Volumes   ┆ n_neurons ┆ *volume_norm_n_r┆ animal │
-    │ ---     ┆ ---        ┆ ---    ┆ ---       ┆   ┆ [mm^3]    ┆ ---       ┆ ois             ┆ ---    │
-    │ str     ┆ str        ┆ i64    ┆ f64       ┆   ┆ ---       ┆ i64       ┆ ---             ┆ str    │
-    │         ┆            ┆        ┆           ┆   ┆ f64       ┆           ┆ f64             ┆        │
-    ╞═════════╪════════════╪════════╪═══════════╪═══╪═══════════╪═══════════╪═════════════════╪════════╡
-    │ overlap ┆ ACA        ┆ 423    ┆ 30.344333 ┆ … ┆ 5.222484  ┆ 337372    ┆ 80.995934       ┆ YW051  │
-    │ gfp     ┆ MO         ┆ 3352   ┆ 24.545987 ┆ … ┆ 22.248234 ┆ 985411    ┆ 150.663641      ┆ YW051  │
-    │ rfp     ┆ ACA        ┆ 1383   ┆ 23.791502 ┆ … ┆ 5.222484  ┆ 337372    ┆ 264.816494      ┆ YW051  │
-    │ gfp     ┆ ACA        ┆ 3130   ┆ 22.920328 ┆ … ┆ 5.222484  ┆ 337372    ┆ 599.331616      ┆ YW051  │
-    │ …       ┆ …          ┆ …      ┆ …         ┆ … ┆ …         ┆ …         ┆ …               ┆ …      │
-    │ overlap ┆ SS         ┆ 1      ┆ 0.071736  ┆ … ┆ 37.177937 ┆ 2384622   ┆ 0.026898        ┆ YW051  │
-    │ overlap ┆ ECT        ┆ 1      ┆ 0.071736  ┆ … ┆ 3.457703  ┆ 387378    ┆ 0.289209        ┆ YW051  │
-    │ overlap ┆ TEa        ┆ 1      ┆ 0.071736  ┆ … ┆ 3.860953  ┆ 386396    ┆ 0.259003        ┆ YW051  │
-    │ rfp     ┆ TT         ┆ 1      ┆ 0.017203  ┆ … ┆ 1.734078  ┆ 124596    ┆ 0.576675        ┆ YW051  │
-    └─────────┴────────────┴────────┴───────────┴───┴───────────┴───────────┴─────────────────┴────────┘
-
-
-
-Do the ROI subregions query
------------------
-
-Example for query the ROIs in visual cortex
-
-.. code-block:: python
-
-    from neuralib.atlas.ccf.query import RoiAreaQuery
-
-    # use the classifier constructed above
-    df = classifier.parsed_df
-    result = RoiAreaQuery.by(df, 'VIS).get_subregion_result
-    print(result.data)
-
-
-output::
-
-    ┌─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬────────┐
-    │ source  ┆ VISam   ┆ VISp    ┆ VISpm   ┆ VISl    ┆ VISal   ┆ VISpor  ┆ VISli   ┆ VISpl   ┆ VISC   │
-    │ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---    │
-    │ str     ┆ f64     ┆ f64     ┆ f64     ┆ f64     ┆ f64     ┆ f64     ┆ f64     ┆ f64     ┆ f64    │
-    ╞═════════╪═════════╪═════════╪═════════╪═════════╪═════════╪═════════╪═════════╪═════════╪════════╡
-    │ aRSC    ┆ 25.4669 ┆ 34.0318 ┆ 23.0979 ┆ 6.42369 ┆ 6.37813 ┆ 1.77676 ┆ 2.27790 ┆ 0.0     ┆ 0.5466 │
-    │         ┆ 7       ┆ 91      ┆ 5       ┆         ┆ 2       ┆ 5       ┆ 4       ┆         ┆ 97     │
-    │ pRSC    ┆ 15.1445 ┆ 36.1079 ┆ 29.5568 ┆ 10.7129 ┆ 3.04431 ┆ 2.38921 ┆ 1.92678 ┆ 1.07899 ┆ 0.0385 │
-    │         ┆ 09      ┆         ┆ 4       ┆ 09      ┆ 6       ┆         ┆ 2       ┆ 8       ┆ 36     │
-    │ overlap ┆ 48.5294 ┆ 8.82352 ┆ 31.25   ┆ 4.04411 ┆ 3.30882 ┆ 2.57352 ┆ 1.10294 ┆ 0.0     ┆ 0.3676 │
-    │         ┆ 12      ┆ 9       ┆         ┆ 8       ┆ 4       ┆ 9       ┆ 1       ┆         ┆ 47     │
-    └─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴────────┘
-
-
-
-"""
+import attrs
+import polars as pl
+from typing_extensions import Self, Final, final
+
+from neuralib.atlas.ccf.classifier import supply_overlap_dataframe
+from neuralib.atlas.type import Source, Area
+from neuralib.atlas.util import get_margin_merge_level
+
+__all__ = ['RoiAreaQuery', 'SubregionResult']
+
+from neuralib.util.util_verbose import fprint
+
+
+@final
+class RoiAreaQuery:
+    """class for finding a subset of rois from a specific area"""
+
+    def __init__(self,
+                 parsed_df: pl.DataFrame,
+                 area: Area,
+                 source_order: tuple[Source, ...] | None = None,
+                 force_set_show_col_level: int | None = None):
+        """
+        :param parsed_df: parsed dataframe from ccf pipeline
+        :param area: area name
+        :param source_order: order of the unique sources
+        :param force_set_show_col_level: force set show col to which level.
+            use case: if a low level area name is classified and show in high level (i.e., TH).
+            Then directly specify the level number instead of auto inferred by hierarchical_query()
+
+            **Please use carefully**
+
+            Note that it results in subregions mixed in different level
+
+            for example, if one level contain both HIP and HPF, it will quantify and calculate the percentage together,
+            however, they are not in the same level for actual allen tree level. it's due to the raw data issue
+            (Rois are not classified correctly initially in allenCCF pipeline)
+        """
+
+        self.parsed_df: Final[pl.DataFrame] = parsed_df
+        self.area: Final[Area] = area
+
+        if source_order is None:
+            self.source_order = tuple(self.parsed_df['source'].unique().to_list())
+        else:
+            self.source_order = source_order
+
+        self._query_col = get_margin_merge_level(self.parsed_df, self.area, 'lowest')
+
+        # infer after query if not force set
+        self._show_col: str | None = None if force_set_show_col_level is None else f'merge_ac_{force_set_show_col_level}'
+        self.query_result: Final[pl.DataFrame] = self._hierarchical_query()
+
+    def __repr__(self):
+        q = f'Query -> {self.query_col}'
+        s = f'Show -> {self.show_col}'
+        res = self.query_result.select('name', self.query_col, self.show_col)
+        return '\n'.join([q, s, str(res)])
+
+    @classmethod
+    def by(cls, df: pl.DataFrame,
+           area: Area, *,
+           source_order: tuple[Source, ...] | None = None,
+           force_set_show_col_level: int | None = None) -> Self:
+        """
+        Query which area
+
+        :param df: ccf parsed dataframe
+        :param area: area name
+        :param source_order: order of the unique sources
+        :param force_set_show_col_level: force set show col to which level.
+            use case: if a low level area name is classified and show in high level (i.e., TH).
+            Then directly specify the level number instead of auto inferred by hierarchical_query()
+
+            **Please use carefully**
+
+            Note that it results in subregions mixed in different level
+
+            for example, if one level contain both HIP and HPF, it will quantify and calculate the percentage together,
+            however, they are not in the same level for actual allen tree level. it's due to the raw data issue
+            (Rois are not classified correctly initially in allenCCF pipeline)
+        :return:
+        """
+
+        return RoiAreaQuery(df, area, source_order=source_order, force_set_show_col_level=force_set_show_col_level)
+
+    @property
+    def query_col(self) -> str:
+        """which column for the area name query (base column query source)"""
+        return self._query_col
+
+    @property
+    def show_col(self) -> str:
+        """highest merge level column for a given area (to show)"""
+        return self._show_col
+
+    def _hierarchical_query(self) -> pl.DataFrame:
+        """Get the query dataframe
+        Auto infer query col & show_col based on area name"""
+        if self._show_col is None:
+            highest_lv = int(get_margin_merge_level(self.parsed_df, self.area, 'highest').split('_')[-1])
+            self._show_col = f'merge_ac_{highest_lv + 1}'
+
+            if self._show_col not in self.parsed_df.columns:
+                fprint(f'{self._show_col} exceed level, force show *acronym*', vtype='warning')
+                self._show_col = 'acronym'
+
+        return self.parsed_df.filter(pl.col(self.query_col) == self.area)
+
+    def get_subregion_result(self, unit: str,
+                             supply_overlap: bool = True) -> SubregionResult:
+        """
+        Get subregion results
+
+        :param unit: {'n_rois', 'percent'}
+        :param supply_overlap: add overlap roi counts into other channel(s)
+        :return: :class:`SubregionResult`
+        """
+        dat = self.query_result.select(['source', self.show_col])
+
+        if supply_overlap:
+            dat = supply_overlap_dataframe(dat)
+
+        df = (dat.group_by(['source', self.show_col])
+              .agg(pl.col(self.show_col).count().alias('n_rois'))
+              .with_columns((pl.col('n_rois') / pl.col('n_rois').sum().over('source') * 100).alias('percent'))
+              .sort('percent', descending=True))
+
+        idx = {val: idx for idx, val in enumerate(self.source_order)}
+        ch_sort = pl.col('source').replace(idx)
+
+        #
+        numbers = df.group_by('source').agg(pl.col('n_rois').sum())
+        numbers = numbers.sort(ch_sort)
+
+        ch_count_all = self.parsed_df.group_by('source').len()
+        roi_profile = (numbers.join(ch_count_all, on='source')
+                       .with_columns((pl.col('n_rois') / pl.col('len')).alias('total_perc'))
+                       .sort(ch_sort))
+        #
+        df = (df.pivot(columns=self._show_col, index='source', values=unit, aggregate_function='first')
+              .fill_null(0))
+
+        df = df.sort(ch_sort)
+
+        return SubregionResult(self, unit, df, roi_profile)
+
+
+@attrs.define
+class SubregionResult:
+    source_query: RoiAreaQuery
+    """source query"""
+
+    unit: str = attrs.field(validator=attrs.validators.in_(('n_rois', 'percent')))
+    """Note that percent are normalized by queried dataframe"""
+
+    data: pl.DataFrame
+    """
+    * Optional with animal col::
+    
+        ┌─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬────────┐
+        │ source  ┆ VISam   ┆ VISp    ┆ VISpm   ┆ VISl    ┆ VISal   ┆ VISpor  ┆ VISli   ┆ VISpl   ┆ VISC   │
+        │ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---     ┆ ---    │
+        │ str     ┆ f64     ┆ f64     ┆ f64     ┆ f64     ┆ f64     ┆ f64     ┆ f64     ┆ f64     ┆ f64    │
+        ╞═════════╪═════════╪═════════╪═════════╪═════════╪═════════╪═════════╪═════════╪═════════╪════════╡
+        │ aRSC    ┆ 25.4669 ┆ 34.0318 ┆ 23.0979 ┆ 6.42369 ┆ 6.37813 ┆ 1.77676 ┆ 2.27790 ┆ 0.0     ┆ 0.5466 │
+        │         ┆ 7       ┆ 91      ┆ 5       ┆         ┆ 2       ┆ 5       ┆ 4       ┆         ┆ 97     │
+        │ pRSC    ┆ 15.1445 ┆ 36.1079 ┆ 29.5568 ┆ 10.7129 ┆ 3.04431 ┆ 2.38921 ┆ 1.92678 ┆ 1.07899 ┆ 0.0385 │
+        │         ┆ 09      ┆         ┆ 4       ┆ 09      ┆ 6       ┆         ┆ 2       ┆ 8       ┆ 36     │
+        │ overlap ┆ 48.5294 ┆ 8.82352 ┆ 31.25   ┆ 4.04411 ┆ 3.30882 ┆ 2.57352 ┆ 1.10294 ┆ 0.0     ┆ 0.3676 │
+        │         ┆ 12      ┆ 9       ┆         ┆ 8       ┆ 4       ┆ 9       ┆ 1       ┆         ┆ 47     │
+        └─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴────────┘
+    """
+
+    roi_profile: pl.DataFrame
+    """
+    roi profile::
+    
+        ┌─────────┬────────┬───────┬────────────┐
+        │ source  ┆ n_rois ┆ count ┆ total_perc │
+        │ ---     ┆ ---    ┆ ---   ┆ ---        │
+        │ str     ┆ u32    ┆ u32   ┆ f64        │
+        ╞═════════╪════════╪═══════╪════════════╡
+        │ aRSC    ┆ 899    ┆ 11403 ┆ 0.078839   │
+        │ pRSC    ┆ 6744   ┆ 26280 ┆ 0.256621   │
+        │ overlap ┆ 225    ┆ 3470  ┆ 0.064841   │
+        └─────────┴────────┴───────┴────────────┘
+    """
+
+    def del_overlap(self) -> Self:
+        """keep same `source_query` but delete the `overlap` data and roi_profile"""
+        expr = pl.col('source') != 'overlap'
+        dat = self.data.filter(expr)
+        profile = self.roi_profile.filter(expr)
+        return attrs.evolve(self, data=dat, roi_profile=profile)
+
+    def with_animal(self, animal: str) -> Self:
+        """add animal col for batch/statistic purpose"""
+        data = self.data.with_columns(pl.lit(animal).alias('animal'))
+        return attrs.evolve(self, data=data)
+
+    @property
+    def sources(self) -> list[Source]:
+        """list of sources"""
+        return self.data['source'].to_list()
+
+    @property
+    def channel_weight(self) -> pl.DataFrame:
+        """fraction foreach source in all rois"""
+        return self.roi_profile.drop('n_rois', 'count')
+
+    @property
+    def weight_list(self) -> list[float]:
+        """list of perc"""
+        return self.channel_weight.get_column('total_perc').to_list()
+
+    @property
+    def values(self) -> pl.DataFrame:
+        """numerical data without source column"""
+        return self.data.select(pl.exclude('source'))
+
+    @property
+    def areas(self) -> list[Area]:
+        """list of areas"""
+        return self.values.columns
+
+    @property
+    def n_areas(self) -> int:
+        """number of areas"""
+        return len(self.areas)
+
+    @property
+    def n_rois_info(self) -> list[str]:
+        """info for plotting"""
+        return [
+            f'{self.source_query.area} -> {row[0]}: {row[1]} ({round(self.weight_list[i], 3)})'
+            for i, row in enumerate(self.roi_profile.iter_rows())
+        ]
```

### Comparing `neura_library-0.0.4/src/neuralib/atlas/ccf/classifier.py` & `neura_library-0.0.5/src/neuralib/atlas/ccf/classifier.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/atlas/ccf/core.py` & `neura_library-0.0.5/src/neuralib/atlas/ccf/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 
 import attrs
 import numpy as np
 import polars as pl
 from scipy.io import loadmat
 from scipy.io.matlab import MatlabOpaque
 
-from neuralib.atlas.allen import AllenReferenceWrapper
 from neuralib.atlas.util import PLANE_TYPE
-from neuralib.atlas.view import SlicePlane
+from neuralib.atlas.view import SlicePlane, load_slice_view
 from neuralib.util.util_type import PathLike
 from neuralib.util.util_verbose import fprint
 from neuralib.util.utils import uglob, joinn
 
 __all__ = [
     'AbstractCCFDir',
     'CCFBaseDir',
@@ -392,16 +391,15 @@
         return self.matrix.slice_index
 
     @property
     def angle_xy(self) -> tuple[float, float]:
         return self.matrix.angle_xy
 
     def get_slice_plane(self) -> SlicePlane:
-        ret = (AllenReferenceWrapper
-               .load_slice_view('template', self.plane_type, self.resolution)
+        ret = (load_slice_view('ccf_template', self.plane_type, allen_annotation_res=self.resolution)
                .plane_at(self.slice_index))
 
         if np.any([a != 0 for a in self.matrix.angle_xy]):
             ret = ret.with_angle_offset(-self.matrix.angle_xy[0], self.matrix.angle_xy[1])
 
         return ret
```

### Comparing `neura_library-0.0.4/src/neuralib/atlas/ccf/norm.py` & `neura_library-0.0.5/src/neuralib/atlas/ccf/norm.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/atlas/cellatlas/__init__.py` & `neura_library-0.0.5/src/neuralib/atlas/cellatlas/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ====================
 
 cell atlas about cell types and volume information for each brain area
 
 .. seealso:: `<https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1010739#sec047>`_
 
 Example of loading the dataframe
----------------
+----------------------------------
 
 .. code-block:: python
 
     from neuralib.atlas.cellatlas import CellAtlas
     catlas = CellAtlas.load_from_csv()
     print(catlas.dataframe)
 
@@ -28,15 +28,15 @@
     │ …                              ┆ …              ┆ …         │
     │ Zona incerta                   ┆ 2.157641       ┆ 136765    │
     │ posteromedial visual area      ┆ 1.2225625      ┆ 197643    │
     └────────────────────────────────┴────────────────┴───────────┘
 
 
 Example of loading the sync dataframe between cellatlas/allen brain acronym
----------------
+------------------------------------------------------------------------------
 
 .. code-block:: python
 
     from neuralib.atlas.cellatlas import CellAtlas
     print(catlas.load_sync_allen_structure_tree())
```

### Comparing `neura_library-0.0.4/src/neuralib/atlas/cellatlas/core.py` & `neura_library-0.0.5/src/neuralib/atlas/cellatlas/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import dataclasses
 import io
 from pathlib import Path
 
 import pandas as pd
 import polars as pl
 
-from neuralib.atlas.allen import AllenReferenceWrapper
+from neuralib.atlas.data import load_structure_tree
 from neuralib.util.io import ATLAS_CACHE_DIRECTORY
 from neuralib.util.util_verbose import fprint
 
 __all__ = ['CellAtlas']
 
 
 @dataclasses.dataclass
@@ -130,17 +130,15 @@
                 └────────────────────────────────┴────────────────┴───────────┴─────────┘
         """
         out = ATLAS_CACHE_DIRECTORY / 'cellatlas_allen_sync.csv'
 
         if not out.exists() or force_save:
             ctlas = cls.load_from_csv()
 
-            allen = (AllenReferenceWrapper.load_structure_tree()
-                     .select('name', 'acronym')
-                     .sort('name'))
+            allen = load_structure_tree().select('name', 'acronym').sort('name')
 
             df = (
                 ctlas.dataframe
                 .rename({'Brain region': 'name'})
                 .join(allen, on='name')
             )
```

### Comparing `neura_library-0.0.4/src/neuralib/atlas/ibl/__init__.py` & `neura_library-0.0.5/src/neuralib/atlas/ibl/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/atlas/ibl/plot.py` & `neura_library-0.0.5/src/neuralib/atlas/ibl/plot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/atlas/map.py` & `neura_library-0.0.5/src/neuralib/atlas/map.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/atlas/plot.py` & `neura_library-0.0.5/src/neuralib/atlas/plot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/atlas/util.py` & `neura_library-0.0.5/src/neuralib/atlas/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from __future__ import annotations
 
 from pathlib import Path
+from pprint import pprint
 from typing import Literal, NamedTuple, Iterable
 
 import numpy as np
 import pandas as pd
 import polars as pl
 
+from neuralib.atlas.data import load_structure_tree
 from neuralib.atlas.map import NUM_MERGE_LAYER
 from neuralib.atlas.type import Source, HEMISPHERE_TYPE
 from neuralib.util.util_type import DataFrame
 from neuralib.util.util_verbose import fprint
 
 __all__ = [
     'ALLEN_CCF_10um_BREGMA',
-    'ALLEN_SOURCE_TYPE',
     'PLANE_TYPE',
     #
     'SourceCoordinates',
     'iter_source_coordinates',
     'get_margin_merge_level',
     'roi_points_converter',
+    'create_allen_structure_dict'
 ]
 
 # allen CCF 10um volume coordinates, refer to allenCCF/Browsing Functions/allenCCFbregma.m
 ALLEN_CCF_10um_BREGMA = np.array([540, 0, 570])  # AP, DV, LR
-ALLEN_SOURCE_TYPE = Literal['annotation', 'nrrd', 'template']
 
 PLANE_TYPE = Literal['coronal', 'sagittal', 'transverse']
 
 
 class SourceCoordinates(NamedTuple):
     source: Source
     coordinates: np.ndarray
@@ -65,15 +66,15 @@
     :param file: parsed csv file after
     :param only_areas: only show rois in region(s)
     :param region_col: if None, auto infer, and check the lowest merge level contain all the regions specified
     :param hemisphere
     :param to_brainrender: convert the coordinates to brain render
     :param to_um
     :param ret_order: whether specify the source generator order
-    :return :class:`SourceCoordinates`
+    :return: :class:`SourceCoordinates`
     """
     df = pl.read_csv(file)
     #
     if only_areas is not None and len(only_areas) != 0:
         if isinstance(only_areas, str):
             only_areas = [only_areas]
 
@@ -104,15 +105,15 @@
                            areas: list[str] | str,
                            margin: Literal['lowest', 'highest']) -> str:
     """Get the lowest or highest merge level (i.e., parsed_csv) containing all the regions
 
     :param df: parsed csv
     :param areas: an area or a list of areas
     :param margin: get the either lowest of highest merge level for a given area
-    :return col name if parsed csv
+    :return: col name if parsed csv
     """
     if not isinstance(areas, (tuple, list)):
         areas = [areas]
 
     eval_merge = [f'merge_ac_{i}' for i in range(NUM_MERGE_LAYER)]
 
     if margin == 'lowest':
@@ -168,7 +169,26 @@
     if to_brainrender:
         points[:, 0] /= -1  # increment toward posterior
         points[:, 2] /= -1  # increment toward left hemisphere
         bregma = ALLEN_CCF_10um_BREGMA * 10  # pixel to um
         points += bregma  # roi relative to bregma
 
     return points
+
+
+def create_allen_structure_dict(verbose=False) -> dict[str, str]:
+    """
+    Get the acronym/name pairing from structure_tree.csv
+
+    :return: key: acronym; value: full name
+    """
+    tree = load_structure_tree()
+    tree = tree.select('name', 'acronym').sort('name')
+
+    ret = {
+        acry: name
+        for name, acry in tree.iter_rows()
+    }
+    if verbose:
+        pprint(ret)
+
+    return ret
```

### Comparing `neura_library-0.0.4/src/neuralib/atlas/view.py` & `neura_library-0.0.5/src/neuralib/atlas/view.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,51 +7,82 @@
 import attrs
 import numpy as np
 from matplotlib.axes import Axes
 from matplotlib.image import AxesImage
 from matplotlib.transforms import CompositeGenericTransform
 from typing_extensions import Self
 
-from neuralib.atlas.util import PLANE_TYPE, ALLEN_CCF_10um_BREGMA, ALLEN_SOURCE_TYPE
+from neuralib.atlas.data import DATA_SOURCE_TYPE, load_ccf_annotation, load_ccf_template, load_allensdk_annotation
+from neuralib.atlas.util import PLANE_TYPE, ALLEN_CCF_10um_BREGMA
 from neuralib.imglib.factory import ImageProcFactory
 from neuralib.plot import plot_figure
+from neuralib.util.util_type import PathLike
 
 __all__ = [
+    'load_slice_view',
     'AbstractSliceView',
     'SlicePlane'
 ]
 
 
+def load_slice_view(source: DATA_SOURCE_TYPE,
+                    plane_type: PLANE_TYPE, *,
+                    output_dir: PathLike | None = None,
+                    allen_annotation_res: int = 10) -> 'AbstractSliceView':
+    """
+    Load the mouse brain slice view
+
+    :param source: {'ccf_annotation', 'ccf_template', 'allensdk_annotation'}
+    :param plane_type: {'coronal', 'sagittal', 'transverse'}
+    :param output_dir: output directory for caching
+    :param allen_annotation_res: volume resolution in um. default is 10 um
+    :return: :class:`AbstractSliceView`
+    """
+    if source == 'ccf_annotation':
+        data = load_ccf_annotation(output_dir)
+        res = 10
+    elif source == 'ccf_template':
+        data = load_ccf_template(output_dir)
+        res = 10
+    elif source == 'allensdk_annotation':
+        data = load_allensdk_annotation(resolution=allen_annotation_res, output_dir=output_dir)
+        res = allen_annotation_res
+    else:
+        raise ValueError('')
+
+    return AbstractSliceView(source, plane_type, res, data)
+
+
 class AbstractSliceView(metaclass=abc.ABCMeta):
-    source_type: Final[ALLEN_SOURCE_TYPE]
+    source_type: Final[DATA_SOURCE_TYPE]
     plane_type: Final[PLANE_TYPE]
     resolution: Final[int]
     """um/pixel"""
     reference: Final[np.ndarray]
     """(AP, DV, ML)"""
 
     grid_x: Final[np.ndarray]
     grid_y: Final[np.ndarray]
 
     reference_verbose: str = ''
 
-    def __new__(cls, source_type: ALLEN_SOURCE_TYPE,
+    def __new__(cls, source_type: DATA_SOURCE_TYPE,
                 plane: PLANE_TYPE,
                 resolution: int,
                 reference: np.ndarray):
         if plane == 'coronal':
             return object.__new__(CoronalSliceView)
         elif plane == 'sagittal':
             return object.__new__(SagittalSliceView)
         elif plane == 'transverse':
             return object.__new__(TransverseSliceView)
         else:
             raise ValueError('')
 
-    def __init__(self, source_type: ALLEN_SOURCE_TYPE,
+    def __init__(self, source_type: DATA_SOURCE_TYPE,
                  plane: PLANE_TYPE,
                  resolution: int,
                  reference: np.ndarray):
         """
 
         :param source_type:
         :param plane:
@@ -395,18 +426,17 @@
         #
         image = self.image.astype(float)
         image[image <= 10] = np.nan
         im_view = ax.imshow(image, cmap='Greys', extent=(x0, x1, y0, y1), clip_on=False, transform=aff_trans, **kwargs)
 
         #
         if with_annotation:
-            from neuralib.atlas.allen import AllenReferenceWrapper
-            ann_img = (AllenReferenceWrapper
-                       .load_slice_view('npy', self.view.plane_type, self.view.resolution)
-                       .plane(self.plane_offset))
+            ann_img = load_slice_view('ccf_annotation',
+                                      self.view.plane_type,
+                                      allen_annotation_res=self.view.resolution).plane(self.plane_offset)
             ann = ImageProcFactory(ann_img).covert_grey_scale().edge_detection(10, 0).image
 
             ann = ann.astype(float)
             ann[ann <= 10] = np.nan
 
             im_ann = ax.imshow(ann, cmap='binary', extent=(x0, x1, y0, y1), alpha=0.3, clip_on=False,
                                interpolation='none', vmin=0, vmax=255, transform=aff_trans)
```

### Comparing `neura_library-0.0.4/src/neuralib/bokeh_model/base.py` & `neura_library-0.0.5/src/neuralib/bokeh_model/base.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/bokeh_model/example.py` & `neura_library-0.0.5/src/neuralib/bokeh_model/example.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/bokeh_model/example_multi.py` & `neura_library-0.0.5/src/neuralib/bokeh_model/example_multi.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/bokeh_model/examples/view_all.py` & `neura_library-0.0.5/src/neuralib/bokeh_model/examples/view_all.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/bokeh_model/examples/view_animal.py` & `neura_library-0.0.5/src/neuralib/bokeh_model/examples/view_animal.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/bokeh_model/examples/view_figure.py` & `neura_library-0.0.5/src/neuralib/bokeh_model/examples/view_figure.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/bokeh_model/tool.py` & `neura_library-0.0.5/src/neuralib/bokeh_model/tool.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/bokeh_model/util.py` & `neura_library-0.0.5/src/neuralib/bokeh_model/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/bokeh_model/view_brain.py` & `neura_library-0.0.5/src/neuralib/bokeh_model/view_brain.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/calimg/scan_image/wrapper.py` & `neura_library-0.0.5/src/neuralib/calimg/scan_image/wrapper.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/calimg/scanbox/__init__.py` & `neura_library-0.0.5/src/neuralib/calimg/scanbox/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/calimg/scanbox/core.py` & `neura_library-0.0.5/src/neuralib/calimg/scanbox/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/calimg/scanbox/viewer.py` & `neura_library-0.0.5/src/neuralib/calimg/scanbox/viewer.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/calimg/suite2p/core.py` & `neura_library-0.0.5/src/neuralib/calimg/suite2p/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/calimg/suite2p/signals.py` & `neura_library-0.0.5/src/neuralib/calimg/suite2p/signals.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,37 +26,33 @@
                       n: int | np.ndarray | list[int],
                       signal_type: SIGNAL_TYPE = 'df_f',
                       normalize: bool = True,
                       dff: bool = True,
                       correct_neuropil: bool = True,
                       method: BASELINE_METHOD = 'maximin') -> tuple[np.ndarray, np.ndarray]:
     """
-    select which signal type that used for analysis, can be either {df_f} and {spks}
+    Select neuronal signals for analysis. For single cell (F,) OR multiple cells (N, F)
 
     :param s2p: suite 2p result
     :param n: neuron index or index array
     :param signal_type: signal type. :data:`~neuralib.calimg.suite2p.core.SIGNAL_TYPE` {'df_f', 'spks'}
-    :param normalize: do normalize
-    :param dff: do dff_signal
+    :param normalize: 01 normalization for each neuron
+    :param dff: normalize to the baseline fluorescence changed (dF/F)
     :param correct_neuropil: do the neuropil correction
     :param method: baseline calculation method {'maximin', 'constant', 'constant_prctile'}
-    :return:
-        signal
-        baseline signal
+    :return: tuple with (signal, baseline signal)
     """
     f = s2p.F[n]
     fneu = s2p.FNeu[n]
-    # TODO consider to use vb method to calculate baseline
+
     if signal_type == 'df_f':
 
         if dff:
             s1 = dff_signal(f, fneu, s2p, correct_neuropil, method).dff
-            # back to normal amplitude, since minus .7 itself (dff_signal)
-            # s2 = dff_signal(fneu, fneu, s2p, correct_neuropil, method) / 0.3
-            s2 = np.full_like(s1, 0)
+            s2 = np.full_like(s1, 0, dtype=int)
             if normalize:
                 o, f = normalize_signal_factor(s1)
                 s1 = (s1 - o) / f
 
         else:
             fcorr = f - 0.7 * fneu
             sig_baseline = s2p.signal_baseline
@@ -68,15 +64,15 @@
                 o, f = normalize_signal_factor(s1)
                 s1 = (s1 - o) / f
                 ob, fb = normalize_signal_factor(s2)
                 s2 = (s2 - ob) / fb
 
     elif signal_type == 'spks':
         s1 = s2p.spks[n]
-        s2 = np.full_like(s1, 0, dtype=np.double)  # TODO decovlved from df_f s2?
+        s2 = np.full_like(s1, 0, dtype=int)
 
         if normalize:
             s1 = normalize_signal(s1)
 
     else:
         raise ValueError('specify signal type either in df_f or spks')
 
@@ -101,40 +97,50 @@
 
 
 # ============ #
 # DF/F Compute #
 # ============ #
 
 class DFFSignal(NamedTuple):
-    """Container for dF/F signal processing"""
+    """Container for dF/F signal processing.
+
+    `Dimension parameters`:
+
+        N = number of neurons
+
+        F = number of frame
+
+    For single cell (F,) OR multiple cells (N, F)
+
+    """
 
     s2p: Suite2PResult
     """Suite2PResult"""
     f: np.ndarray
-    """fluorescence"""
+    """fluorescence. (F,) | (N, F)"""
     fneu: np.ndarray
-    """neuropil"""
+    """neuropil. (F,) | (N, F)"""
     fcorr: np.ndarray
-    """f used for dff calculation, could be either corrected by fneu"""
+    """f used for dff calculation, could be either corrected by fneu. (F,) | (N, F)"""
     f0: np.ndarray
-    """f0"""
+    """f0. (F,) | (N, F)"""
     dff: np.ndarray
-    """ dff after f0 normalization"""
+    """dff after f0 normalization. (F,) | (N, F)"""
 
     @property
     def dff_baseline(self) -> np.ndarray:
         """baseline of dff, supposed to be 0"""
         return np.full_like(self.dff, 0)
 
     @property
     def baseline_fluctuation(self) -> np.ndarray:
-        """get the fluctuation of the fneu signal
-        Perhaps not fully corrected and physiological reason
+        """get the fluctuation of the fneu signal (F,) | (N, F).
 
-        ** used to get the baseline std (i.e., trial reliability metric)
+        Perhaps not fully corrected with physiological reason.
+        **used to get the baseline std (i.e., trial reliability metric)**
         """
         fneu_corr = 0.3 * self.fneu
         fneu_bas = calc_signal_baseline(fneu_corr, self.s2p, method='maximin')
         return 100 * ((fneu_corr - fneu_bas) / fneu_bas)
 
     def oasis_dcnv(self) -> np.ndarray:
         """spike deconvolution"""
@@ -147,17 +153,17 @@
 
 def dff_signal(f: np.ndarray,
                fneu: np.ndarray,
                s2p: Suite2PResult,
                correct_neuropil: bool = True,
                method: BASELINE_METHOD = 'maximin') -> DFFSignal:
     """
-    df_f normalization, referred by suite2p, return df_f activity
+    df_f signal normalization container
 
-    :param f: neuron signal
+    :param f: neuron signal (F)
     :param fneu: neuropil signal
     :param s2p: Suite2PResult
     :param correct_neuropil: whether do the subtraction using neuropil
     :param method:
 
     :return:
         DFFSignal
@@ -276,18 +282,18 @@
     return ret
 
 
 def _oasis(fcorr: np.ndarray,
            tau: float,
            fs: float) -> np.ndarray:
     """
-    computes non-negative deconvolution. no sparsity constraints
-    Adpated from suite2p
+    Computes non-negative deconvolution. no sparsity constraints
+
+    .. seealso::
 
-    ..seealso::
         suite2p.extraction.dcnv.preprocess
 
     :param fcorr: neuropil-subtracted, baseline-subtracted fluorescence, aka, fcorr - f0. (N, F)
     :param tau:  timescale of the sensor, used for the deconvolution kernel
     :param fs: sampling rate per plane
     :return:
         (N, T) spks
```

### Comparing `neura_library-0.0.4/src/neuralib/imglib/factory.py` & `neura_library-0.0.5/src/neuralib/imglib/factory.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/imglib/io.py` & `neura_library-0.0.5/src/neuralib/imglib/io.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/imglib/labeller.py` & `neura_library-0.0.5/src/neuralib/imglib/labeller.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/imglib/norm.py` & `neura_library-0.0.5/src/neuralib/imglib/norm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import numpy as np
 
 __all__ = [
     'normalize_sequences',
-    'handle_invalid_value'
+    'handle_invalid_value',
+    'get_percentile_value'
 ]
 
 
 def normalize_sequences(frames: list[np.ndarray] | np.ndarray,
                         handle_invalid: bool = True,
                         gamma_correction: bool = False,
                         gamma_value: float = 0.5,
@@ -43,7 +44,21 @@
 
 
 def handle_invalid_value(frames: list[np.ndarray] | np.ndarray) -> list[np.ndarray]:
     """Handle NaN and negative values and ensure all values are >= 0"""
     frames = [np.nan_to_num(frame, nan=0, posinf=0, neginf=0) for frame in frames]
     frames = [np.clip(frame, 0, None) for frame in frames]
     return frames
+
+
+def get_percentile_value(im: np.ndarray,
+                         perc_interval: tuple[float, float] = (10, 100)) -> tuple[float, float]:
+    """Get the central distribution boundary value for
+    imaging enhancement by changing the scaling of array.
+
+    :param im: image array
+    :param perc_interval: percentile
+    :return: lower_bound and upper_bound based on value distribution
+    """
+    im = im.flatten()
+    lb, up = perc_interval
+    return np.percentile(im, lb), np.percentile(im, up)
```

### Comparing `neura_library-0.0.4/src/neuralib/model/bayes_decoding/position.py` & `neura_library-0.0.5/src/neuralib/model/bayes_decoding/position.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     fr *= spatial_bin_size
     term2 = (-1) * spatial_bin_size * np.sum(rate_map, axis=1)
     term2 -= np.max(term2)  # normalize in log space
     term2 = np.exp(term2)  # (X,)
 
     if np.any(term2 < overflow):
-        raise RuntimeError(f'OVERFLOW: {term2=}')  # TODO neuron number exceed ~1k, might problematic
+        raise RuntimeError(f'OVERFLOW: {term2=}')
 
     outer_multiply = np.vectorize(np.multiply.outer, signature='(t),(s)->(t,s)')
     # outer_multiply((N, T), (N, X)) = (N, T, X)
     u = np.sum(outer_multiply(fr.T, np.log(rate_map.T)), axis=0)
     u -= np.max(u, axis=1, keepdims=True)  # normalize in log space
     u = np.exp(u)  # (T, X)
```

### Comparing `neura_library-0.0.4/src/neuralib/persistence/cli_persistence.py` & `neura_library-0.0.5/src/neuralib/persistence/cli_persistence.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/persistence/persistence.py` & `neura_library-0.0.5/src/neuralib/persistence/persistence.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/plot/animation.py` & `neura_library-0.0.5/src/neuralib/plot/animation.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/plot/colormap.py` & `neura_library-0.0.5/src/neuralib/plot/colormap.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/plot/figure.py` & `neura_library-0.0.5/src/neuralib/plot/figure.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/plot/misc.py` & `neura_library-0.0.5/src/neuralib/plot/misc.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/plot/plot.py` & `neura_library-0.0.5/src/neuralib/plot/plot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/plot/setting.py` & `neura_library-0.0.5/src/neuralib/plot/setting.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/plot/tools.py` & `neura_library-0.0.5/src/neuralib/plot/tools.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/plot/venn.py` & `neura_library-0.0.5/src/neuralib/plot/venn.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/scanner/__init__.py` & `neura_library-0.0.5/src/neuralib/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/scanner/core.py` & `neura_library-0.0.5/src/neuralib/scanner/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/scanner/czi.py` & `neura_library-0.0.5/src/neuralib/scanner/czi.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/scanner/lsm.py` & `neura_library-0.0.5/src/neuralib/scanner/lsm.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/segmentation/base.py` & `neura_library-0.0.5/src/neuralib/segmentation/base.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/segmentation/cellpose/core.py` & `neura_library-0.0.5/src/neuralib/segmentation/cellpose/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/segmentation/cellpose/run_api.py` & `neura_library-0.0.5/src/neuralib/segmentation/cellpose/run_api.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/segmentation/cellpose/run_subproc.py` & `neura_library-0.0.5/src/neuralib/segmentation/cellpose/run_subproc.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/segmentation/stardist/run_2d.py` & `neura_library-0.0.5/src/neuralib/segmentation/stardist/run_2d.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/stimpy/__init__.py` & `neura_library-0.0.5/src/neuralib/stimpy/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/stimpy/baselog.py` & `neura_library-0.0.5/src/neuralib/stimpy/baselog.py`

 * *Files 3% similar despite different names*

```diff
@@ -336,14 +336,33 @@
 
     @property
     @abc.abstractmethod
     def stimulus_segment(self) -> np.ndarray:
         """stimulation time segment (on-off) in sec (N, 2)"""
         pass
 
+    def stim_square_pulse_event(self, sampling_rate: float = 30.) -> RigEvent:
+        """
+        Get the stimulation on-off square pulse 0,1 consecutive event
+
+        :param sampling_rate: sampling rate for the time domain interpolation
+        :return: Stimulus rig event
+        """
+        start_time = self.exp_start_time
+        end_time = self.exp_end_time
+        seg = self.stimulus_segment
+
+        t = np.arange(start_time, end_time, 1 / sampling_rate)
+        ret = np.zeros_like(t)
+        for (on, off) in seg:
+            mask = np.logical_and(on < t, t < off)
+            ret[mask] = 1
+
+        return RigEvent('visual_stim', np.vstack((t, ret)).T)
+
     @abc.abstractmethod
     def session_trials(self) -> dict[Session, SessionInfo]:
         """get the session:SessionInfo dictionary (experimental and user-specific)"""
         pass
 
     @property
     @abc.abstractmethod
```

### Comparing `neura_library-0.0.4/src/neuralib/stimpy/baseprot.py` & `neura_library-0.0.5/src/neuralib/stimpy/baseprot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/stimpy/camlog.py` & `neura_library-0.0.5/src/neuralib/stimpy/camlog.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/stimpy/event.py` & `neura_library-0.0.5/src/neuralib/stimpy/event.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/stimpy/math_eval.py` & `neura_library-0.0.5/src/neuralib/stimpy/math_eval.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/stimpy/preference.py` & `neura_library-0.0.5/src/neuralib/stimpy/preference.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/stimpy/protocol_parser.py` & `neura_library-0.0.5/src/neuralib/stimpy/protocol_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/stimpy/session.py` & `neura_library-0.0.5/src/neuralib/stimpy/session.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/stimpy/stimpy_core.py` & `neura_library-0.0.5/src/neuralib/stimpy/stimpy_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,15 +339,14 @@
         if isinstance(self.time_offset, float):
             return tend + self.time_offset
         elif isinstance(self.time_offset, np.ndarray):
             return tend + self.time_offset[-1]
 
     @property
     def stimulus_segment(self) -> np.ndarray:
-        """sti_period"""
         v_start = self.v_frame_idx == 1
         t1 = self.v_present_time[v_start]
         t2 = self.v_present_time[np.nonzero(np.diff(self.v_frame_idx) < 0)[0] + 1]
 
         if isinstance(self.time_offset, float):
             offset = self.time_offset
         elif isinstance(self.time_offset, np.ndarray):
```

### Comparing `neura_library-0.0.4/src/neuralib/stimpy/stimpy_git.py` & `neura_library-0.0.5/src/neuralib/stimpy/stimpy_git.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/stimpy/stimpy_pyv.py` & `neura_library-0.0.5/src/neuralib/stimpy/stimpy_pyv.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/stimpy/stimulus.py` & `neura_library-0.0.5/src/neuralib/stimpy/stimulus.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/stimpy/util.py` & `neura_library-0.0.5/src/neuralib/stimpy/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/tools/pkl_parq_view/main_app.py` & `neura_library-0.0.5/src/neuralib/tools/pkl_parq_view/main_app.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/tools/slack_bot/bot.py` & `neura_library-0.0.5/src/neuralib/tools/slack_bot/bot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/util/cli_args.py` & `neura_library-0.0.5/src/neuralib/util/cli_args.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/util/color_logging.py` & `neura_library-0.0.5/src/neuralib/util/color_logging.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/util/csv.py` & `neura_library-0.0.5/src/neuralib/util/csv.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/util/func.py` & `neura_library-0.0.5/src/neuralib/util/func.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/util/gpu.py` & `neura_library-0.0.5/src/neuralib/util/gpu.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/util/json.py` & `neura_library-0.0.5/src/neuralib/util/json.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/util/profile_test.py` & `neura_library-0.0.5/src/neuralib/util/profile_test.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/util/segement.py` & `neura_library-0.0.5/src/neuralib/util/segement.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/util/table.py` & `neura_library-0.0.5/src/neuralib/util/table.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/util/util_cv2.py` & `neura_library-0.0.5/src/neuralib/util/util_cv2.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/util/util_type.py` & `neura_library-0.0.5/src/neuralib/util/util_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -44,9 +44,10 @@
 #
 AxesArrayLike = Union[np.ndarray, list[Axes]]
 
 
 # ============ #
 
 def is_iterable(val: Any) -> bool:
+    """check value is iterable"""
     from collections.abc import Iterable
     return isinstance(val, Iterable) and not isinstance(val, str)
```

### Comparing `neura_library-0.0.4/src/neuralib/util/util_verbose.py` & `neura_library-0.0.5/src/neuralib/util/util_verbose.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/util/utils.py` & `neura_library-0.0.5/src/neuralib/util/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,47 +13,50 @@
            'joinn',
            'flat_ls',
            'array2str',
            'deprecated',
            'key_from_value']
 
 
-def uglob(d: PathLike,
+def uglob(directory: PathLike,
           pattern: str,
           sort: bool = True,
           is_dir: bool = False) -> Path:
     """
-    Unique glob
+    Unique glob the pattern in a directory
 
-    :param d: directory
+    :param directory: directory
     :param pattern: pattern string
     :param sort: if sort
     :param is_dir: only return if is a directory
     :return: unique path
     """
-    if not isinstance(d, Path):
-        d = Path(d)
+    if not isinstance(directory, Path):
+        directory = Path(directory)
 
-    if not d.is_dir():
-        raise ValueError(f'{d} is not a directory')
+    if not directory.exists():
+        raise FileNotFoundError(f'{directory} not exit')
 
-    f = list(d.glob(pattern))
+    if not directory.is_dir():
+        raise NotADirectoryError(f'{directory} is not a directory')
+
+    f = list(directory.glob(pattern))
 
     if is_dir:
         f = [ff for ff in f if ff.is_dir()]
 
     if sort:
         f.sort()
 
     if len(f) == 0:
-        raise FileNotFoundError(f'{d} not have pattern: {pattern}')
+        raise FileNotFoundError(f'{directory} not have pattern: {pattern}')
     elif len(f) == 1:
         return f[0]
     else:
-        raise RuntimeError(f'multiple files were found in {d} in pattern {pattern} >>> {f}')
+        raise RuntimeError(f'multiple files were found in {directory} in pattern {pattern} >>> {f}')
 
 
 def glob_re(pattern: str, strings: list[str]) -> list[str]:
     """find list of str element fit for re pattern"""
     return list(filter(re.compile(pattern).match, strings))
 
 
@@ -118,22 +121,23 @@
 
 # ============================== #
 
 KT = TypeVar('KT')
 VT = TypeVar('VT')
 
 
-def key_from_value(d: dict[KT, VT], value: VT) -> KT:
-    """Get dict key from dict value, supporting str, int, list, and tuple types for values."""
+def key_from_value(d: dict[KT, VT], value: VT) -> KT | list[KT]:
+    """Get dict key from dict value, supporting str, int, float, list, and tuple types for values."""
     matching_keys = []
     for key, val in d.items():
-        if isinstance(val, (str, int)) and val == value:
-            matching_keys.append(key)
-        elif isinstance(val, (list, tuple)) and value in val:
-            matching_keys.append(key)
+        if not isinstance(val, (str, int, float, list, tuple)):
+            raise RuntimeError(f'value type: {type(val)} not support')
+        else:
+            if isinstance(val, (str, int, float)) and val == value:
+                matching_keys.append(key)
+            elif isinstance(val, (list, tuple)) and value in val:
+                matching_keys.append(key)
 
     if not matching_keys:
         raise KeyError(f'Value {value} not found in the dictionary')
-    if len(matching_keys) > 1:
-        raise RuntimeError(f'Multiple keys found for the value {value}: {matching_keys}')
-
-    return matching_keys[0]
+    else:
+        return matching_keys[0] if len(matching_keys) == 1 else matching_keys
```

### Comparing `neura_library-0.0.4/src/neuralib/util/version.py` & `neura_library-0.0.5/src/neuralib/util/version.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/wrapper/deeplabcut/core.py` & `neura_library-0.0.5/src/neuralib/wrapper/deeplabcut/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/wrapper/deeplabcut/util.py` & `neura_library-0.0.5/src/neuralib/wrapper/deeplabcut/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/wrapper/facemap/__init__.py` & `neura_library-0.0.5/src/neuralib/wrapper/facemap/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/wrapper/facemap/core.py` & `neura_library-0.0.5/src/neuralib/wrapper/facemap/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/wrapper/facemap/plot.py` & `neura_library-0.0.5/src/neuralib/wrapper/facemap/plot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/wrapper/rastermap/__init__.py` & `neura_library-0.0.5/src/neuralib/wrapper/rastermap/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/src/neuralib/wrapper/rastermap/core.py` & `neura_library-0.0.5/src/neuralib/wrapper/rastermap/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/test/test_argp.py` & `neura_library-0.0.5/test/test_argp.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/test/test_argp_dispatch.py` & `neura_library-0.0.5/test/test_argp_dispatch.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/test/test_csv_context_manager.py` & `neura_library-0.0.5/test/test_csv_context_manager.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/test/test_persistence_autoinc.py` & `neura_library-0.0.5/test/test_persistence_autoinc.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/test/test_protocol_parser.py` & `neura_library-0.0.5/test/test_protocol_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/test/test_pyvstim_parser.py` & `neura_library-0.0.5/test/test_pyvstim_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/test/test_stimpy_bitbucket_parser.py` & `neura_library-0.0.5/test/test_stimpy_bitbucket_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.4/test/test_stimpy_github_parser.py` & `neura_library-0.0.5/test/test_stimpy_github_parser.py`

 * *Files identical despite different names*

