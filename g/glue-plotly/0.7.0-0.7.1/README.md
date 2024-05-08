# Comparing `tmp/glue_plotly-0.7.0.tar.gz` & `tmp/glue_plotly-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_plotly-0.7.0.tar", last modified: Tue May  7 20:46:24 2024, max compression
+gzip compressed data, was "glue_plotly-0.7.1.tar", last modified: Wed May  8 20:04:06 2024, max compression
```

## Comparing `glue_plotly-0.7.0.tar` & `glue_plotly-0.7.1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.698685 glue_plotly-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.678685 glue_plotly-0.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.678685 glue_plotly-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/.github/workflows/update-changelog.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-07 20:46:24.698685 glue_plotly-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.682685 glue_plotly-0.7.0/doc/
--rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/doc/BqplotToolbarHighlighted.png
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/doc/PlotlyViewerExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   151377 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/doc/QtChartStudioExport.gif
--rw-r--r--   0 runner    (1001) docker     (127)   221318 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/doc/QtToolbarExport.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.682685 glue_plotly-0.7.0/glue_plotly/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.686685 glue_plotly-0.7.0/glue_plotly/common/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/dotplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/scatter3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.686685 glue_plotly-0.7.0/glue_plotly/common/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/tests/test_dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/tests/test_dotplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/tests/test_scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/common/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/export_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.686685 glue_plotly-0.7.0/glue_plotly/html_exporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.686685 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/scatter2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.690685 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.690685 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/scatter3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_scatter3d.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/save_hover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/save_hover.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/sort_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/sort_components.ui
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/viewers/common/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/viewers/common/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/common/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/common/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/common/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/common/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/viewers/histogram/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/histogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/histogram/dotplot_layer_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/histogram/layer_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/histogram/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/viewers/scatter/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/scatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/scatter/layer_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/viewers/scatter/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/export_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.694685 glue_plotly-0.7.0/glue_plotly/web/qt/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/qt/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/qt/exporter.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.698685 glue_plotly-0.7.0/glue_plotly/web/qt/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/qt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/qt/tests/test_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/qt/tests/test_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.698685 glue_plotly-0.7.0/glue_plotly/web/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/glue_plotly/web/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:46:24.698685 glue_plotly-0.7.0/glue_plotly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-07 20:46:24.000000 glue_plotly-0.7.0/glue_plotly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-07 20:46:24.000000 glue_plotly-0.7.0/glue_plotly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:46:24.000000 glue_plotly-0.7.0/glue_plotly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 20:46:24.000000 glue_plotly-0.7.0/glue_plotly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:46:24.000000 glue_plotly-0.7.0/glue_plotly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 20:46:24.000000 glue_plotly-0.7.0/glue_plotly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 20:46:24.000000 glue_plotly-0.7.0/glue_plotly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-07 20:46:24.698685 glue_plotly-0.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      432 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-07 20:46:00.000000 glue_plotly-0.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.711464 glue_plotly-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.695464 glue_plotly-0.7.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.695464 glue_plotly-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/.github/workflows/update-changelog.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-08 20:04:06.711464 glue_plotly-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.695464 glue_plotly-0.7.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/doc/BqplotToolbarHighlighted.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17060 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/doc/PlotlyViewerExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   151377 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/doc/QtChartStudioExport.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   221318 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/doc/QtToolbarExport.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.695464 glue_plotly-0.7.1/glue_plotly/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.699464 glue_plotly-0.7.1/glue_plotly/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/dotplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/scatter3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.699464 glue_plotly-0.7.1/glue_plotly/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/tests/test_dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/tests/test_dotplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/tests/test_scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/export_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.699464 glue_plotly-0.7.1/glue_plotly/html_exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.703464 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/scatter2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.703464 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.703464 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/scatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_scatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/save_hover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/save_hover.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/sort_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/sort_components.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/viewers/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/viewers/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/common/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/common/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/common/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/common/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/viewers/histogram/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/histogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/histogram/dotplot_layer_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/histogram/layer_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/histogram/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/viewers/scatter/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/scatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/scatter/layer_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/scatter/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/export_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/web/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/qt/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/qt/exporter.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.711464 glue_plotly-0.7.1/glue_plotly/web/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/qt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/qt/tests/test_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/qt/tests/test_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.711464 glue_plotly-0.7.1/glue_plotly/web/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.711464 glue_plotly-0.7.1/glue_plotly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-08 20:04:06.000000 glue_plotly-0.7.1/glue_plotly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-08 20:04:06.000000 glue_plotly-0.7.1/glue_plotly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:04:06.000000 glue_plotly-0.7.1/glue_plotly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 20:04:06.000000 glue_plotly-0.7.1/glue_plotly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:04:06.000000 glue_plotly-0.7.1/glue_plotly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 20:04:06.000000 glue_plotly-0.7.1/glue_plotly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 20:04:06.000000 glue_plotly-0.7.1/glue_plotly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-08 20:04:06.711464 glue_plotly-0.7.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      432 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/tox.ini
```

### Comparing `glue_plotly-0.7.0/.github/workflows/ci_workflows.yml` & `glue_plotly-0.7.1/.github/workflows/ci_workflows.yml`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/.github/workflows/update-changelog.yaml` & `glue_plotly-0.7.1/.github/workflows/update-changelog.yaml`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/CHANGES.md` & `glue_plotly-0.7.1/CHANGES.md`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/LICENSE` & `glue_plotly-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/PKG-INFO` & `glue_plotly-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-plotly
-Version: 0.7.0
+Version: 0.7.1
 Summary: Experimental plot.ly exporters for glue
 Home-page: https://github.com/glue-viz/glue-plotly
 Author: Thomas Robitaille and Catherine Zucker
 Author-email: glue.viz@gmail.com
 License: BSD 3-Clause License
 Provides: glue_plotly
 Requires-Python: >=3.8
```

### Comparing `glue_plotly-0.7.0/README.rst` & `glue_plotly-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/doc/BqplotToolbarHighlighted.png` & `glue_plotly-0.7.1/doc/BqplotToolbarHighlighted.png`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/doc/QtChartStudioExport.gif` & `glue_plotly-0.7.1/doc/QtChartStudioExport.gif`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/doc/QtToolbarExport.gif` & `glue_plotly-0.7.1/doc/QtToolbarExport.gif`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/__init__.py` & `glue_plotly-0.7.1/glue_plotly/__init__.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/common/common.py` & `glue_plotly-0.7.1/glue_plotly/common/common.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/common/dendrogram.py` & `glue_plotly-0.7.1/glue_plotly/common/dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/common/dotplot.py` & `glue_plotly-0.7.1/glue_plotly/common/dotplot.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/common/histogram.py` & `glue_plotly-0.7.1/glue_plotly/common/histogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/common/image.py` & `glue_plotly-0.7.1/glue_plotly/common/image.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/common/profile.py` & `glue_plotly-0.7.1/glue_plotly/common/profile.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/common/scatter2d.py` & `glue_plotly-0.7.1/glue_plotly/common/scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/common/scatter3d.py` & `glue_plotly-0.7.1/glue_plotly/common/scatter3d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/common/tests/test_dendrogram.py` & `glue_plotly-0.7.1/glue_plotly/common/tests/test_dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/common/tests/test_dotplot.py` & `glue_plotly-0.7.1/glue_plotly/common/tests/test_dotplot.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/common/tests/test_histogram.py` & `glue_plotly-0.7.1/glue_plotly/common/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/common/tests/test_profile.py` & `glue_plotly-0.7.1/glue_plotly/common/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/common/tests/test_scatter2d.py` & `glue_plotly-0.7.1/glue_plotly/common/tests/test_scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/common/tests/utils.py` & `glue_plotly-0.7.1/glue_plotly/common/tests/utils.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/export_dialog.py` & `glue_plotly-0.7.1/glue_plotly/export_dialog.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/base.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/base.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/histogram.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/histogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/image.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/image.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/profile.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/profile.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/scatter2d.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_base.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_histogram.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_image.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_profile.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/dendrogram.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/histogram.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/histogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/image.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/image.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/profile.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/profile.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/scatter2d.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/scatter3d.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/scatter3d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/table.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/table.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_base.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_dendrogram.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_histogram.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_image.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_profile.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_scatter2d.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_scatter3d.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_scatter3d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/html_exporters/qt/tests/test_table.py` & `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/logo.png` & `glue_plotly-0.7.1/glue_plotly/logo.png`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/logo.svg` & `glue_plotly-0.7.1/glue_plotly/logo.svg`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/save_hover.py` & `glue_plotly-0.7.1/glue_plotly/save_hover.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/save_hover.ui` & `glue_plotly-0.7.1/glue_plotly/save_hover.ui`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/sort_components.py` & `glue_plotly-0.7.1/glue_plotly/sort_components.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/sort_components.ui` & `glue_plotly-0.7.1/glue_plotly/sort_components.ui`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/utils.py` & `glue_plotly-0.7.1/glue_plotly/utils.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/viewers/common/tests/test_tools.py` & `glue_plotly-0.7.1/glue_plotly/viewers/common/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/viewers/common/tests/utils.py` & `glue_plotly-0.7.1/glue_plotly/viewers/common/tests/utils.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/viewers/common/tools.py` & `glue_plotly-0.7.1/glue_plotly/viewers/common/tools.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/viewers/common/viewer.py` & `glue_plotly-0.7.1/glue_plotly/viewers/common/viewer.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/viewers/histogram/dotplot_layer_artist.py` & `glue_plotly-0.7.1/glue_plotly/viewers/histogram/dotplot_layer_artist.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,25 +104,28 @@
 
         with self.view.figure.batch_update():
             self.view.figure.for_each_trace(self._update_visual_attrs_for_trace, dict(meta=self._dots_id))
 
     def _update_visual_attrs_for_trace(self, trace):
         marker = trace.marker
         marker.update(opacity=self.state.alpha, color=fixed_color(self.state), size=dot_radius(self.view, self.state))
-        print(marker)
         trace.update(marker=marker,
                      visible=self.state.visible,
                      unselected=dict(marker=dict(opacity=self.state.alpha)))
 
     def _update_data(self):
         old_dots = self._get_dots()
         if old_dots:
-            self.view._remove_traces(old_dots)
+            with self.view.figure.batch_update():
+                for trace in old_dots:
+                    self.view._remove_trace_index(trace)
 
         dots = traces_for_layer(self.view, self.state, add_data_label=True)
+        for trace in dots:
+            trace.update(hoverinfo='all', unselected=dict(marker=dict(opacity=self.state.alpha)))
         self._dots_id = dots[0].meta if dots else None
         self.view.figure.add_traces(dots)
 
     def _update_zorder(self):
         traces = [self.view.selection_layer]
         for layer in self.view.layers:
             traces += list(layer.traces())
```

### Comparing `glue_plotly-0.7.0/glue_plotly/viewers/histogram/layer_artist.py` & `glue_plotly-0.7.1/glue_plotly/viewers/histogram/layer_artist.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/viewers/histogram/viewer.py` & `glue_plotly-0.7.1/glue_plotly/viewers/histogram/viewer.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/viewers/scatter/layer_artist.py` & `glue_plotly-0.7.1/glue_plotly/viewers/scatter/layer_artist.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/viewers/scatter/viewer.py` & `glue_plotly-0.7.1/glue_plotly/viewers/scatter/viewer.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/web/export_plotly.py` & `glue_plotly-0.7.1/glue_plotly/web/export_plotly.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/web/qt/__init__.py` & `glue_plotly-0.7.1/glue_plotly/web/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/web/qt/exporter.py` & `glue_plotly-0.7.1/glue_plotly/web/qt/exporter.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/web/qt/exporter.ui` & `glue_plotly-0.7.1/glue_plotly/web/qt/exporter.ui`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/web/qt/tests/test_exporter.py` & `glue_plotly-0.7.1/glue_plotly/web/qt/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly/web/qt/tests/test_plotly.py` & `glue_plotly-0.7.1/glue_plotly/web/qt/tests/test_plotly.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/glue_plotly.egg-info/PKG-INFO` & `glue_plotly-0.7.1/glue_plotly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-plotly
-Version: 0.7.0
+Version: 0.7.1
 Summary: Experimental plot.ly exporters for glue
 Home-page: https://github.com/glue-viz/glue-plotly
 Author: Thomas Robitaille and Catherine Zucker
 Author-email: glue.viz@gmail.com
 License: BSD 3-Clause License
 Provides: glue_plotly
 Requires-Python: >=3.8
```

### Comparing `glue_plotly-0.7.0/glue_plotly.egg-info/SOURCES.txt` & `glue_plotly-0.7.1/glue_plotly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/setup.cfg` & `glue_plotly-0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.0/tox.ini` & `glue_plotly-0.7.1/tox.ini`

 * *Files identical despite different names*

