# Comparing `tmp/trajectopy_core-3.0.1.tar.gz` & `tmp/trajectopy_core-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trajectopy_core-3.0.1.tar", max compression
+gzip compressed data, was "trajectopy_core-3.1.0.tar", max compression
```

## Comparing `trajectopy_core-3.0.1.tar` & `trajectopy_core-3.1.0.tar`

### file list

```diff
@@ -1,72 +1,78 @@
--rw-r--r--   0        0        0     1091 2023-10-09 11:26:32.282290 trajectopy_core-3.0.1/LICENSE
--rw-r--r--   0        0        0     1049 2024-05-06 07:37:48.711881 trajectopy_core-3.0.1/pyproject.toml
--rw-r--r--   0        0        0    33448 2024-05-06 07:02:04.320372 trajectopy_core-3.0.1/README.md
--rw-r--r--   0        0        0      228 2023-11-29 11:29:09.869840 trajectopy_core-3.0.1/trajectopy_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 15:04:24.294777 trajectopy_core-3.0.1/trajectopy_core/alignment/__init__.py
--rw-r--r--   0        0        0    20272 2024-04-23 15:04:24.295777 trajectopy_core-3.0.1/trajectopy_core/alignment/data.py
--rw-r--r--   0        0        0    10299 2024-04-23 15:04:24.295777 trajectopy_core-3.0.1/trajectopy_core/alignment/direct.py
--rw-r--r--   0        0        0     8526 2024-04-23 15:04:24.296780 trajectopy_core-3.0.1/trajectopy_core/alignment/egrad_interface.py
--rw-r--r--   0        0        0    16133 2024-04-23 15:04:24.296780 trajectopy_core-3.0.1/trajectopy_core/alignment/equations.py
--rw-r--r--   0        0        0    32369 2024-04-23 15:04:24.296780 trajectopy_core-3.0.1/trajectopy_core/alignment/estimation.py
--rw-r--r--   0        0        0    23829 2024-04-23 15:04:24.297810 trajectopy_core-3.0.1/trajectopy_core/alignment/parameters.py
--rw-r--r--   0        0        0     2845 2024-04-23 15:04:24.297810 trajectopy_core-3.0.1/trajectopy_core/alignment/result.py
--rw-r--r--   0        0        0     7421 2023-11-08 14:24:59.349660 trajectopy_core-3.0.1/trajectopy_core/alignment/utils.py
--rw-r--r--   0        0        0        0 2024-04-22 13:30:20.272430 trajectopy_core-3.0.1/trajectopy_core/approximation/__init__.py
--rw-r--r--   0        0        0     9308 2023-11-29 11:29:09.871841 trajectopy_core-3.0.1/trajectopy_core/approximation/cubic_approximation.py
--rw-r--r--   0        0        0     6608 2023-11-29 11:29:09.872840 trajectopy_core-3.0.1/trajectopy_core/approximation/math_utils.py
--rw-r--r--   0        0        0     3880 2023-11-29 11:29:09.872840 trajectopy_core-3.0.1/trajectopy_core/approximation/mls_approximation.py
--rw-r--r--   0        0        0     2151 2023-11-29 11:29:09.873840 trajectopy_core-3.0.1/trajectopy_core/approximation/rot_approximation.py
--rw-r--r--   0        0        0     4888 2023-11-29 11:29:09.873840 trajectopy_core-3.0.1/trajectopy_core/approximation/voxelizer.py
--rw-r--r--   0        0        0     2001 2024-04-18 14:05:54.822747 trajectopy_core-3.0.1/trajectopy_core/definitions.py
--rw-r--r--   0        0        0        0 2024-04-23 15:04:24.298782 trajectopy_core-3.0.1/trajectopy_core/evaluation/__init__.py
--rw-r--r--   0        0        0    15186 2024-04-23 15:04:24.298782 trajectopy_core-3.0.1/trajectopy_core/evaluation/ate_result.py
--rw-r--r--   0        0        0    11114 2023-11-29 11:29:09.875840 trajectopy_core-3.0.1/trajectopy_core/evaluation/comparison.py
--rw-r--r--   0        0        0      834 2023-11-29 11:29:09.875840 trajectopy_core-3.0.1/trajectopy_core/evaluation/deviations.py
--rw-r--r--   0        0        0     2277 2024-04-23 15:04:24.299809 trajectopy_core-3.0.1/trajectopy_core/evaluation/metrics.py
--rw-r--r--   0        0        0     9993 2024-04-23 15:04:24.299809 trajectopy_core-3.0.1/trajectopy_core/evaluation/rpe_result.py
--rw-r--r--   0        0        0     1318 2023-11-08 14:24:59.352660 trajectopy_core-3.0.1/trajectopy_core/evaluation/utils.py
--rw-r--r--   0        0        0        0 2024-04-23 15:04:24.299809 trajectopy_core-3.0.1/trajectopy_core/input_output/__init__.py
--rw-r--r--   0        0        0     5273 2024-04-23 15:04:24.300806 trajectopy_core-3.0.1/trajectopy_core/input_output/header.py
--rw-r--r--   0        0        0     3155 2024-05-06 07:38:42.899583 trajectopy_core-3.0.1/trajectopy_core/input_output/rosbag.py
--rw-r--r--   0        0        0     1197 2024-04-23 15:04:24.300806 trajectopy_core-3.0.1/trajectopy_core/input_output/rosmsg.py
--rw-r--r--   0        0        0    11313 2024-04-23 15:04:24.301809 trajectopy_core-3.0.1/trajectopy_core/input_output/trajectory_io.py
--rw-r--r--   0        0        0     1118 2024-04-23 15:04:24.301809 trajectopy_core-3.0.1/trajectopy_core/input_output/utils.py
--rw-r--r--   0        0        0     1899 2023-11-29 11:29:09.878841 trajectopy_core-3.0.1/trajectopy_core/kml.py
--rw-r--r--   0        0        0     1091 2023-10-09 11:26:32.322607 trajectopy_core-3.0.1/trajectopy_core/LICENSE
--rw-r--r--   0        0        0     9635 2024-04-23 13:24:51.703124 trajectopy_core-3.0.1/trajectopy_core/matching.py
--rw-r--r--   0        0        0     1756 2024-04-23 15:04:24.301809 trajectopy_core-3.0.1/trajectopy_core/merging.py
--rw-r--r--   0        0        0        0 2023-11-08 14:24:59.355663 trajectopy_core-3.0.1/trajectopy_core/plotting/__init__.py
--rw-r--r--   0        0        0     3764 2023-12-06 12:10:06.681755 trajectopy_core-3.0.1/trajectopy_core/plotting/bar_plots.py
--rw-r--r--   0        0        0      956 2023-12-06 12:10:06.681755 trajectopy_core-3.0.1/trajectopy_core/plotting/heatmaps.py
--rw-r--r--   0        0        0     2564 2023-12-06 12:10:06.682752 trajectopy_core-3.0.1/trajectopy_core/plotting/histograms.py
--rw-r--r--   0        0        0    11164 2023-12-04 09:19:20.547164 trajectopy_core-3.0.1/trajectopy_core/plotting/line_plots.py
--rw-r--r--   0        0        0    12764 2024-01-30 08:35:04.316260 trajectopy_core-3.0.1/trajectopy_core/plotting/multi_line_plots.py
--rw-r--r--   0        0        0    10999 2024-01-22 14:08:45.543673 trajectopy_core-3.0.1/trajectopy_core/plotting/scatter_plots.py
--rw-r--r--   0        0        0     1626 2024-04-23 13:05:40.251467 trajectopy_core-3.0.1/trajectopy_core/plotting/tables.py
--rw-r--r--   0        0        0     1660 2024-04-23 15:04:24.302811 trajectopy_core-3.0.1/trajectopy_core/plotting/utils.py
--rw-r--r--   0        0        0        0 2023-11-28 13:16:01.712748 trajectopy_core-3.0.1/trajectopy_core/report/__init__.py
--rw-r--r--   0        0        0     2441 2024-04-23 13:05:41.738081 trajectopy_core-3.0.1/trajectopy_core/report/alignment.py
--rw-r--r--   0        0        0    24491 2023-10-25 12:40:21.678268 trajectopy_core-3.0.1/trajectopy_core/report/assets/icon.png
--rw-r--r--   0        0        0     3251 2023-10-25 12:40:21.679269 trajectopy_core-3.0.1/trajectopy_core/report/assets/style.css
--rw-r--r--   0        0        0     6220 2024-02-02 14:24:47.287810 trajectopy_core-3.0.1/trajectopy_core/report/data.py
--rw-r--r--   0        0        0     3640 2024-02-02 14:24:47.287810 trajectopy_core-3.0.1/trajectopy_core/report/multi.py
--rw-r--r--   0        0        0     5286 2024-02-02 14:24:47.288807 trajectopy_core-3.0.1/trajectopy_core/report/single.py
--rw-r--r--   0        0        0     4660 2024-02-02 14:24:47.288807 trajectopy_core-3.0.1/trajectopy_core/report/templates/generic.html
--rw-r--r--   0        0        0     5616 2024-02-02 14:24:47.288807 trajectopy_core-3.0.1/trajectopy_core/report/templates/multi_template.html
--rw-r--r--   0        0        0     7282 2024-02-02 14:24:47.289808 trajectopy_core-3.0.1/trajectopy_core/report/templates/single_template.html
--rw-r--r--   0        0        0     2010 2024-04-23 15:04:24.302811 trajectopy_core-3.0.1/trajectopy_core/report/trajectory.py
--rw-r--r--   0        0        0     2663 2024-01-22 14:08:45.549678 trajectopy_core-3.0.1/trajectopy_core/report/utils.py
--rw-r--r--   0        0        0     1863 2023-11-23 12:18:37.196406 trajectopy_core-3.0.1/trajectopy_core/rotationset.py
--rw-r--r--   0        0        0        0 2023-11-06 11:51:17.163404 trajectopy_core-3.0.1/trajectopy_core/settings/__init__.py
--rw-r--r--   0        0        0     8782 2024-04-23 15:04:24.303809 trajectopy_core-3.0.1/trajectopy_core/settings/alignment.py
--rw-r--r--   0        0        0      301 2023-11-29 11:29:09.884840 trajectopy_core-3.0.1/trajectopy_core/settings/approximation.py
--rw-r--r--   0        0        0     2556 2023-12-04 09:19:20.550568 trajectopy_core-3.0.1/trajectopy_core/settings/base.py
--rw-r--r--   0        0        0     2286 2023-11-29 11:29:09.885840 trajectopy_core-3.0.1/trajectopy_core/settings/comparison.py
--rw-r--r--   0        0        0     1164 2024-04-18 14:05:54.823745 trajectopy_core-3.0.1/trajectopy_core/settings/matching.py
--rw-r--r--   0        0        0     1337 2023-12-04 09:19:20.550568 trajectopy_core-3.0.1/trajectopy_core/settings/processing.py
--rw-r--r--   0        0        0     6498 2024-05-06 06:05:42.856075 trajectopy_core-3.0.1/trajectopy_core/settings/report.py
--rw-r--r--   0        0        0      370 2023-11-29 11:29:09.886843 trajectopy_core-3.0.1/trajectopy_core/settings/sorting.py
--rw-r--r--   0        0        0    10910 2024-04-23 15:04:24.303809 trajectopy_core-3.0.1/trajectopy_core/sorting.py
--rw-r--r--   0        0        0    30134 2024-04-23 15:04:24.304809 trajectopy_core-3.0.1/trajectopy_core/trajectory.py
--rw-r--r--   0        0        0     6322 2023-11-29 11:29:09.888841 trajectopy_core-3.0.1/trajectopy_core/utils.py
--rw-r--r--   0        0        0    34323 1970-01-01 00:00:00.000000 trajectopy_core-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-10-09 11:26:32.282290 trajectopy_core-3.1.0/LICENSE
+-rw-r--r--   0        0        0     1049 2024-05-08 10:26:03.493705 trajectopy_core-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0    33448 2024-05-06 07:02:04.320372 trajectopy_core-3.1.0/README.md
+-rw-r--r--   0        0        0      228 2023-11-29 11:29:09.869840 trajectopy_core-3.1.0/trajectopy_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 15:04:24.294777 trajectopy_core-3.1.0/trajectopy_core/alignment/__init__.py
+-rw-r--r--   0        0        0    20272 2024-04-23 15:04:24.295777 trajectopy_core-3.1.0/trajectopy_core/alignment/data.py
+-rw-r--r--   0        0        0    10299 2024-04-23 15:04:24.295777 trajectopy_core-3.1.0/trajectopy_core/alignment/direct.py
+-rw-r--r--   0        0        0     8526 2024-04-23 15:04:24.296780 trajectopy_core-3.1.0/trajectopy_core/alignment/egrad_interface.py
+-rw-r--r--   0        0        0    16133 2024-04-23 15:04:24.296780 trajectopy_core-3.1.0/trajectopy_core/alignment/equations.py
+-rw-r--r--   0        0        0    32370 2024-05-08 07:35:31.443623 trajectopy_core-3.1.0/trajectopy_core/alignment/estimation.py
+-rw-r--r--   0        0        0    23829 2024-04-23 15:04:24.297810 trajectopy_core-3.1.0/trajectopy_core/alignment/parameters.py
+-rw-r--r--   0        0        0     2845 2024-04-23 15:04:24.297810 trajectopy_core-3.1.0/trajectopy_core/alignment/result.py
+-rw-r--r--   0        0        0     7421 2023-11-08 14:24:59.349660 trajectopy_core-3.1.0/trajectopy_core/alignment/utils.py
+-rw-r--r--   0        0        0        0 2024-04-22 13:30:20.272430 trajectopy_core-3.1.0/trajectopy_core/approximation/__init__.py
+-rw-r--r--   0        0        0     9318 2024-05-08 06:34:00.204503 trajectopy_core-3.1.0/trajectopy_core/approximation/cubic_approximation.py
+-rw-r--r--   0        0        0     3892 2024-05-08 10:26:46.447862 trajectopy_core-3.1.0/trajectopy_core/approximation/mls_approximation.py
+-rw-r--r--   0        0        0     2159 2024-05-08 10:26:46.449861 trajectopy_core-3.1.0/trajectopy_core/approximation/rot_approximation.py
+-rw-r--r--   0        0        0     4888 2023-11-29 11:29:09.873840 trajectopy_core-3.1.0/trajectopy_core/approximation/voxelizer.py
+-rw-r--r--   0        0        0     2001 2024-04-18 14:05:54.822747 trajectopy_core-3.1.0/trajectopy_core/definitions.py
+-rw-r--r--   0        0        0        0 2024-04-23 15:04:24.298782 trajectopy_core-3.1.0/trajectopy_core/evaluation/__init__.py
+-rw-r--r--   0        0        0    15186 2024-04-23 15:04:24.298782 trajectopy_core-3.1.0/trajectopy_core/evaluation/ate_result.py
+-rw-r--r--   0        0        0    11114 2023-11-29 11:29:09.875840 trajectopy_core-3.1.0/trajectopy_core/evaluation/comparison.py
+-rw-r--r--   0        0        0      834 2023-11-29 11:29:09.875840 trajectopy_core-3.1.0/trajectopy_core/evaluation/deviations.py
+-rw-r--r--   0        0        0     2279 2024-05-08 07:35:28.392215 trajectopy_core-3.1.0/trajectopy_core/evaluation/metrics.py
+-rw-r--r--   0        0        0     9993 2024-04-23 15:04:24.299809 trajectopy_core-3.1.0/trajectopy_core/evaluation/rpe_result.py
+-rw-r--r--   0        0        0     1318 2023-11-08 14:24:59.352660 trajectopy_core-3.1.0/trajectopy_core/evaluation/utils.py
+-rw-r--r--   0        0        0        0 2024-04-23 15:04:24.299809 trajectopy_core-3.1.0/trajectopy_core/input_output/__init__.py
+-rw-r--r--   0        0        0     5273 2024-04-23 15:04:24.300806 trajectopy_core-3.1.0/trajectopy_core/input_output/header.py
+-rw-r--r--   0        0        0     3155 2024-05-06 07:38:42.899583 trajectopy_core-3.1.0/trajectopy_core/input_output/rosbag.py
+-rw-r--r--   0        0        0     1197 2024-04-23 15:04:24.300806 trajectopy_core-3.1.0/trajectopy_core/input_output/rosmsg.py
+-rw-r--r--   0        0        0    11313 2024-04-23 15:04:24.301809 trajectopy_core-3.1.0/trajectopy_core/input_output/trajectory_io.py
+-rw-r--r--   0        0        0     1118 2024-04-23 15:04:24.301809 trajectopy_core-3.1.0/trajectopy_core/input_output/utils.py
+-rw-r--r--   0        0        0     1899 2023-11-29 11:29:09.878841 trajectopy_core-3.1.0/trajectopy_core/kml.py
+-rw-r--r--   0        0        0     1091 2023-10-09 11:26:32.322607 trajectopy_core-3.1.0/trajectopy_core/LICENSE
+-rw-r--r--   0        0        0     9635 2024-04-23 13:24:51.703124 trajectopy_core-3.1.0/trajectopy_core/matching.py
+-rw-r--r--   0        0        0     1756 2024-04-23 15:04:24.301809 trajectopy_core-3.1.0/trajectopy_core/merging.py
+-rw-r--r--   0        0        0        0 2023-11-08 14:24:59.355663 trajectopy_core-3.1.0/trajectopy_core/plotting/__init__.py
+-rw-r--r--   0        0        0      783 2024-05-08 10:26:46.456891 trajectopy_core-3.1.0/trajectopy_core/plotting/mpl/__init__.py
+-rw-r--r--   0        0        0     6495 2024-05-08 07:46:54.807146 trajectopy_core-3.1.0/trajectopy_core/plotting/mpl/alignment_plot.py
+-rw-r--r--   0        0        0      482 2024-05-08 06:23:48.857288 trajectopy_core-3.1.0/trajectopy_core/plotting/mpl/default.mplstyle
+-rw-r--r--   0        0        0    16208 2024-05-08 10:26:46.465860 trajectopy_core-3.1.0/trajectopy_core/plotting/mpl/deviation_plot.py
+-rw-r--r--   0        0        0     4850 2024-05-08 06:49:14.739299 trajectopy_core-3.1.0/trajectopy_core/plotting/mpl/trajectory_plot.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:36:40.472881 trajectopy_core-3.1.0/trajectopy_core/plotting/plotly/__init__.py
+-rw-r--r--   0        0        0     3764 2023-12-06 12:10:06.681755 trajectopy_core-3.1.0/trajectopy_core/plotting/plotly/bar_plots.py
+-rw-r--r--   0        0        0      956 2023-12-06 12:10:06.681755 trajectopy_core-3.1.0/trajectopy_core/plotting/plotly/heatmaps.py
+-rw-r--r--   0        0        0     2564 2023-12-06 12:10:06.682752 trajectopy_core-3.1.0/trajectopy_core/plotting/plotly/histograms.py
+-rw-r--r--   0        0        0    11164 2023-12-04 09:19:20.547164 trajectopy_core-3.1.0/trajectopy_core/plotting/plotly/line_plots.py
+-rw-r--r--   0        0        0    12764 2024-01-30 08:35:04.316260 trajectopy_core-3.1.0/trajectopy_core/plotting/plotly/multi_line_plots.py
+-rw-r--r--   0        0        0    10999 2024-01-22 14:08:45.543673 trajectopy_core-3.1.0/trajectopy_core/plotting/plotly/scatter_plots.py
+-rw-r--r--   0        0        0     1626 2024-04-23 13:05:40.251467 trajectopy_core-3.1.0/trajectopy_core/plotting/plotly/tables.py
+-rw-r--r--   0        0        0     1660 2024-04-23 15:04:24.302811 trajectopy_core-3.1.0/trajectopy_core/plotting/utils.py
+-rw-r--r--   0        0        0        0 2023-11-28 13:16:01.712748 trajectopy_core-3.1.0/trajectopy_core/report/__init__.py
+-rw-r--r--   0        0        0     2448 2024-05-08 06:37:26.681301 trajectopy_core-3.1.0/trajectopy_core/report/alignment.py
+-rw-r--r--   0        0        0    24491 2023-10-25 12:40:21.678268 trajectopy_core-3.1.0/trajectopy_core/report/assets/icon.png
+-rw-r--r--   0        0        0     3251 2023-10-25 12:40:21.679269 trajectopy_core-3.1.0/trajectopy_core/report/assets/style.css
+-rw-r--r--   0        0        0     6220 2024-02-02 14:24:47.287810 trajectopy_core-3.1.0/trajectopy_core/report/data.py
+-rw-r--r--   0        0        0     3647 2024-05-08 06:37:34.696928 trajectopy_core-3.1.0/trajectopy_core/report/multi.py
+-rw-r--r--   0        0        0     5293 2024-05-08 06:37:39.795961 trajectopy_core-3.1.0/trajectopy_core/report/single.py
+-rw-r--r--   0        0        0     4660 2024-02-02 14:24:47.288807 trajectopy_core-3.1.0/trajectopy_core/report/templates/generic.html
+-rw-r--r--   0        0        0     5616 2024-02-02 14:24:47.288807 trajectopy_core-3.1.0/trajectopy_core/report/templates/multi_template.html
+-rw-r--r--   0        0        0     7282 2024-02-02 14:24:47.289808 trajectopy_core-3.1.0/trajectopy_core/report/templates/single_template.html
+-rw-r--r--   0        0        0     2017 2024-05-08 06:37:43.750436 trajectopy_core-3.1.0/trajectopy_core/report/trajectory.py
+-rw-r--r--   0        0        0     2663 2024-01-22 14:08:45.549678 trajectopy_core-3.1.0/trajectopy_core/report/utils.py
+-rw-r--r--   0        0        0     1863 2023-11-23 12:18:37.196406 trajectopy_core-3.1.0/trajectopy_core/rotationset.py
+-rw-r--r--   0        0        0        0 2023-11-06 11:51:17.163404 trajectopy_core-3.1.0/trajectopy_core/settings/__init__.py
+-rw-r--r--   0        0        0     8782 2024-04-23 15:04:24.303809 trajectopy_core-3.1.0/trajectopy_core/settings/alignment.py
+-rw-r--r--   0        0        0      301 2023-11-29 11:29:09.884840 trajectopy_core-3.1.0/trajectopy_core/settings/approximation.py
+-rw-r--r--   0        0        0     2556 2023-12-04 09:19:20.550568 trajectopy_core-3.1.0/trajectopy_core/settings/base.py
+-rw-r--r--   0        0        0     2286 2023-11-29 11:29:09.885840 trajectopy_core-3.1.0/trajectopy_core/settings/comparison.py
+-rw-r--r--   0        0        0     1164 2024-04-18 14:05:54.823745 trajectopy_core-3.1.0/trajectopy_core/settings/matching.py
+-rw-r--r--   0        0        0      814 2024-05-08 08:05:21.454082 trajectopy_core-3.1.0/trajectopy_core/settings/mpl_settings.py
+-rw-r--r--   0        0        0     1337 2023-12-04 09:19:20.550568 trajectopy_core-3.1.0/trajectopy_core/settings/processing.py
+-rw-r--r--   0        0        0     6498 2024-05-06 06:05:42.856075 trajectopy_core-3.1.0/trajectopy_core/settings/report.py
+-rw-r--r--   0        0        0      370 2023-11-29 11:29:09.886843 trajectopy_core-3.1.0/trajectopy_core/settings/sorting.py
+-rw-r--r--   0        0        0    10910 2024-04-23 15:04:24.303809 trajectopy_core-3.1.0/trajectopy_core/sorting.py
+-rw-r--r--   0        0        0    30134 2024-04-23 15:04:24.304809 trajectopy_core-3.1.0/trajectopy_core/trajectory.py
+-rw-r--r--   0        0        0    10437 2024-05-08 06:33:35.681872 trajectopy_core-3.1.0/trajectopy_core/utils.py
+-rw-r--r--   0        0        0    34323 1970-01-01 00:00:00.000000 trajectopy_core-3.1.0/PKG-INFO
```

### Comparing `trajectopy_core-3.0.1/LICENSE` & `trajectopy_core-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/pyproject.toml` & `trajectopy_core-3.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trajectopy-core"
-version = "3.0.1"
+version = "3.1.0"
 description = "Trajectory Evaluation in Python"
 authors = ["Gereon Tombrink <tombrink@igg.uni-bonn.de>"]
 maintainers = ["Gereon Tombrink <tombrink@igg.uni-bonn.de>"]
 license = "MIT"
 keywords = ["trajectory", "evaluation", "alignment", "similarity", "leverarm", "epsg", "robotics"]
 readme = "README.md"
 homepage = "https://github.com/gereon-t/trajectopy-core"
```

### Comparing `trajectopy_core-3.0.1/README.md` & `trajectopy_core-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/alignment/data.py` & `trajectopy_core-3.1.0/trajectopy_core/alignment/data.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/alignment/direct.py` & `trajectopy_core-3.1.0/trajectopy_core/alignment/direct.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/alignment/egrad_interface.py` & `trajectopy_core-3.1.0/trajectopy_core/alignment/egrad_interface.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/alignment/equations.py` & `trajectopy_core-3.1.0/trajectopy_core/alignment/equations.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/alignment/estimation.py` & `trajectopy_core-3.1.0/trajectopy_core/alignment/estimation.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from trajectopy_core.settings.alignment import AlignmentSettings
 from trajectopy_core.settings.matching import MatchingSettings
 from trajectopy_core.trajectory import Trajectory
 
 logger = logging.getLogger("root")
 
 
-def compute_alignment(
+def estimate_alignment(
     traj_from: Trajectory,
     traj_to: Trajectory,
     alignment_settings: AlignmentSettings = AlignmentSettings(),
     matching_settings: MatchingSettings = MatchingSettings(),
 ) -> AlignmentResult:
     """Aligns two trajectories
```

### Comparing `trajectopy_core-3.0.1/trajectopy_core/alignment/parameters.py` & `trajectopy_core-3.1.0/trajectopy_core/alignment/parameters.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/alignment/result.py` & `trajectopy_core-3.1.0/trajectopy_core/alignment/result.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/alignment/utils.py` & `trajectopy_core-3.1.0/trajectopy_core/alignment/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/approximation/cubic_approximation.py` & `trajectopy_core-3.1.0/trajectopy_core/approximation/cubic_approximation.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 from typing import List, Tuple, Union
 
 import numpy as np
 import numpy.matlib as npm
 from scipy.sparse import csr_matrix
 
-from .math_utils import sparse_least_squares
+from trajectopy_core.utils import sparse_least_squares
 
 # logger configuration
 logger = logging.getLogger("root")
 
 
 class CubicApproximation:
     """
```

### Comparing `trajectopy_core-3.0.1/trajectopy_core/approximation/mls_approximation.py` & `trajectopy_core-3.1.0/trajectopy_core/approximation/mls_approximation.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 import logging
 from functools import lru_cache
 from typing import FrozenSet, Tuple, Union
 
 import numpy as np
 
-from .math_utils import Line3D
+from trajectopy_core.utils import Line3D
+
 from .voxelizer import Voxelizer
 
 # logger configuration
 logger = logging.getLogger("root")
 
 
 def mls_iterative(
```

### Comparing `trajectopy_core-3.0.1/trajectopy_core/approximation/rot_approximation.py` & `trajectopy_core-3.1.0/trajectopy_core/approximation/rot_approximation.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 """
 
 import logging
 
 import numpy as np
 
 from trajectopy_core.rotationset import RotationSet
-
-from .math_utils import rndodd
+from trajectopy_core.utils import rndodd
 
 # logger configuration
 logger = logging.getLogger("root")
 
 
 def rot_average_window(function_of: np.ndarray, quat: np.ndarray, win_size: float = 0.15) -> np.ndarray:
     """
```

### Comparing `trajectopy_core-3.0.1/trajectopy_core/approximation/voxelizer.py` & `trajectopy_core-3.1.0/trajectopy_core/approximation/voxelizer.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/definitions.py` & `trajectopy_core-3.1.0/trajectopy_core/definitions.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/evaluation/ate_result.py` & `trajectopy_core-3.1.0/trajectopy_core/evaluation/ate_result.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/evaluation/comparison.py` & `trajectopy_core-3.1.0/trajectopy_core/evaluation/comparison.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/evaluation/deviations.py` & `trajectopy_core-3.1.0/trajectopy_core/evaluation/deviations.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/evaluation/metrics.py` & `trajectopy_core-3.1.0/trajectopy_core/evaluation/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Tuple, Union
 
-from trajectopy_core.alignment.estimation import compute_alignment
+from trajectopy_core.alignment.estimation import estimate_alignment
 from trajectopy_core.alignment.result import AlignmentResult
 from trajectopy_core.evaluation.ate_result import ATEResult
 from trajectopy_core.evaluation.comparison import compare_trajectories_absolute, compare_trajectories_relative
 from trajectopy_core.evaluation.rpe_result import RPEResult
 from trajectopy_core.matching import match_trajectories
 from trajectopy_core.settings.processing import ProcessingSettings
 from trajectopy_core.trajectory import Trajectory
@@ -25,15 +25,15 @@
         settings (ProcessingSettings, optional): Processing settings.
 
     Returns:
         ATEResult: Result of the ATE computation.
 
     """
     match_trajectories(traj_from=trajectory_est, traj_to=trajectory_gt, settings=settings.matching)
-    alignment = compute_alignment(
+    alignment = estimate_alignment(
         traj_from=trajectory_est,
         traj_to=trajectory_gt,
         alignment_settings=settings.alignment,
         matching_settings=settings.matching,
     )
     trajectory_est_aligned = trajectory_est.apply_alignment(alignment_result=alignment, inplace=False)
     return (
```

### Comparing `trajectopy_core-3.0.1/trajectopy_core/evaluation/rpe_result.py` & `trajectopy_core-3.1.0/trajectopy_core/evaluation/rpe_result.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/evaluation/utils.py` & `trajectopy_core-3.1.0/trajectopy_core/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/input_output/header.py` & `trajectopy_core-3.1.0/trajectopy_core/input_output/header.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/input_output/rosbag.py` & `trajectopy_core-3.1.0/trajectopy_core/input_output/rosbag.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/input_output/rosmsg.py` & `trajectopy_core-3.1.0/trajectopy_core/input_output/rosmsg.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/input_output/trajectory_io.py` & `trajectopy_core-3.1.0/trajectopy_core/input_output/trajectory_io.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/input_output/utils.py` & `trajectopy_core-3.1.0/trajectopy_core/input_output/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/kml.py` & `trajectopy_core-3.1.0/trajectopy_core/kml.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/LICENSE` & `trajectopy_core-3.1.0/trajectopy_core/LICENSE`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/matching.py` & `trajectopy_core-3.1.0/trajectopy_core/matching.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/merging.py` & `trajectopy_core-3.1.0/trajectopy_core/merging.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/plotting/bar_plots.py` & `trajectopy_core-3.1.0/trajectopy_core/plotting/plotly/bar_plots.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/plotting/heatmaps.py` & `trajectopy_core-3.1.0/trajectopy_core/plotting/plotly/heatmaps.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/plotting/histograms.py` & `trajectopy_core-3.1.0/trajectopy_core/plotting/plotly/histograms.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/plotting/line_plots.py` & `trajectopy_core-3.1.0/trajectopy_core/plotting/plotly/line_plots.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/plotting/multi_line_plots.py` & `trajectopy_core-3.1.0/trajectopy_core/plotting/plotly/multi_line_plots.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/plotting/scatter_plots.py` & `trajectopy_core-3.1.0/trajectopy_core/plotting/plotly/scatter_plots.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/plotting/tables.py` & `trajectopy_core-3.1.0/trajectopy_core/plotting/plotly/tables.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/plotting/utils.py` & `trajectopy_core-3.1.0/trajectopy_core/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/report/alignment.py` & `trajectopy_core-3.1.0/trajectopy_core/report/alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import List
 
 import jinja2
 import numpy as np
 import pandas as pd
 
 from trajectopy_core.alignment.parameters import AlignmentParameters
-from trajectopy_core.plotting import heatmaps, tables
+from trajectopy_core.plotting.plotly import heatmaps, tables
 from trajectopy_core.report.utils import TEMPLATES_PATH, convert_icon_to_base64
 from trajectopy_core.settings.report import ReportSettings
 
 logger = logging.getLogger("root")
 
 
 def build_correlation_dataframe(estimated_parameters: AlignmentParameters, enabled_only: bool = True) -> pd.DataFrame:
```

### Comparing `trajectopy_core-3.0.1/trajectopy_core/report/assets/icon.png` & `trajectopy_core-3.1.0/trajectopy_core/report/assets/icon.png`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/report/assets/style.css` & `trajectopy_core-3.1.0/trajectopy_core/report/assets/style.css`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/report/data.py` & `trajectopy_core-3.1.0/trajectopy_core/report/data.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/report/multi.py` & `trajectopy_core-3.1.0/trajectopy_core/report/multi.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 from typing import List, Optional
 
 import jinja2
 
 from trajectopy_core.evaluation.ate_result import ATEResult
 from trajectopy_core.evaluation.rpe_result import RPEResult
-from trajectopy_core.plotting import bar_plots, multi_line_plots
+from trajectopy_core.plotting.plotly import bar_plots, multi_line_plots
 from trajectopy_core.report.data import ATEReportData, ATEReportDataCollection, RPEReportData, RPEReportDataCollection
 from trajectopy_core.report.utils import TEMPLATES_PATH, convert_icon_to_base64
 from trajectopy_core.settings.report import ReportSettings
 
 logger = logging.getLogger("root")
```

### Comparing `trajectopy_core-3.0.1/trajectopy_core/report/single.py` & `trajectopy_core-3.1.0/trajectopy_core/report/single.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import List, Optional
 
 import jinja2
 import numpy as np
 
 from trajectopy_core.evaluation.ate_result import ATEResult
 from trajectopy_core.evaluation.rpe_result import RPEResult
-from trajectopy_core.plotting import bar_plots, histograms, line_plots, scatter_plots
+from trajectopy_core.plotting.plotly import bar_plots, histograms, line_plots, scatter_plots
 from trajectopy_core.report.data import ATEReportData, RPEReportData
 from trajectopy_core.report.utils import TEMPLATES_PATH, convert_icon_to_base64, number_to_string
 from trajectopy_core.settings.report import ReportSettings
 
 logger = logging.getLogger("root")
```

### Comparing `trajectopy_core-3.0.1/trajectopy_core/report/templates/generic.html` & `trajectopy_core-3.1.0/trajectopy_core/report/templates/generic.html`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/report/templates/multi_template.html` & `trajectopy_core-3.1.0/trajectopy_core/report/templates/multi_template.html`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/report/templates/single_template.html` & `trajectopy_core-3.1.0/trajectopy_core/report/templates/single_template.html`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/report/trajectory.py` & `trajectopy_core-3.1.0/trajectopy_core/report/trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 import logging
 from typing import List
 
 import jinja2
 
-from trajectopy_core.plotting import multi_line_plots, scatter_plots
+from trajectopy_core.plotting.plotly import multi_line_plots, scatter_plots
 from trajectopy_core.report.utils import TEMPLATES_PATH, convert_icon_to_base64
 from trajectopy_core.settings.report import ReportSettings
 from trajectopy_core.trajectory import Trajectory
 
 logger = logging.getLogger("root")
```

### Comparing `trajectopy_core-3.0.1/trajectopy_core/report/utils.py` & `trajectopy_core-3.1.0/trajectopy_core/report/utils.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/rotationset.py` & `trajectopy_core-3.1.0/trajectopy_core/rotationset.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/settings/alignment.py` & `trajectopy_core-3.1.0/trajectopy_core/settings/alignment.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/settings/base.py` & `trajectopy_core-3.1.0/trajectopy_core/settings/base.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/settings/comparison.py` & `trajectopy_core-3.1.0/trajectopy_core/settings/comparison.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/settings/matching.py` & `trajectopy_core-3.1.0/trajectopy_core/settings/matching.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/settings/processing.py` & `trajectopy_core-3.1.0/trajectopy_core/settings/processing.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/settings/report.py` & `trajectopy_core-3.1.0/trajectopy_core/settings/report.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/sorting.py` & `trajectopy_core-3.1.0/trajectopy_core/sorting.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/trajectopy_core/trajectory.py` & `trajectopy_core-3.1.0/trajectopy_core/trajectory.py`

 * *Files identical despite different names*

### Comparing `trajectopy_core-3.0.1/PKG-INFO` & `trajectopy_core-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trajectopy-core
-Version: 3.0.1
+Version: 3.1.0
 Summary: Trajectory Evaluation in Python
 Home-page: https://github.com/gereon-t/trajectopy-core
 License: MIT
 Keywords: trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics
 Author: Gereon Tombrink
 Author-email: tombrink@igg.uni-bonn.de
 Maintainer: Gereon Tombrink
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trajectopy-core Version: 3.0.1 Summary: Trajectory
+Metadata-Version: 2.1 Name: trajectopy-core Version: 3.1.0 Summary: Trajectory
 Evaluation in Python Home-page: https://github.com/gereon-t/trajectopy-core
 License: MIT Keywords:
 trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics Author:
 Gereon Tombrink Author-email: tombrink@igg.uni-bonn.de Maintainer: Gereon
 Tombrink Maintainer-email: tombrink@igg.uni-bonn.de Requires-Python:
 >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

