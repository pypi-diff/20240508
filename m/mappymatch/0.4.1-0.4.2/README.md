# Comparing `tmp/mappymatch-0.4.1.tar.gz` & `tmp/mappymatch-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mappymatch-0.4.1.tar", last modified: Mon Jul 17 20:18:38 2023, max compression
+gzip compressed data, was "mappymatch-0.4.2.tar", last modified: Wed May  8 16:04:06 2024, max compression
```

## Comparing `mappymatch-0.4.1.tar` & `mappymatch-0.4.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.068137 mappymatch-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-17 20:18:22.000000 mappymatch-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 20:18:22.000000 mappymatch-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-17 20:18:38.068137 mappymatch-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-17 20:18:22.000000 mappymatch-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.052136 mappymatch-0.4.1/mappymatch/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.052136 mappymatch-0.4.1/mappymatch/constructs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/constructs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/constructs/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/constructs/geofence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/constructs/match.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/constructs/road.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/constructs/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.052136 mappymatch-0.4.1/mappymatch/maps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.056136 mappymatch-0.4.1/mappymatch/maps/igraph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/igraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13041 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/igraph/igraph_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/map_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.056136 mappymatch-0.4.1/mappymatch/maps/nx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/nx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11890 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/nx/nx_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.056136 mappymatch-0.4.1/mappymatch/maps/nx/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/nx/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/nx/readers/osm_readers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.056136 mappymatch-0.4.1/mappymatch/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.060136 mappymatch-0.4.1/mappymatch/matchers/lcss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/lcss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/lcss/constructs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/lcss/lcss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/lcss/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/lcss/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/line_snap.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/match_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/matcher_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/osrm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/valhalla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.060136 mappymatch-0.4.1/mappymatch/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.060136 mappymatch-0.4.1/mappymatch/resources/traces/
--rw-r--r--   0 runner    (1001) docker     (123)    22920 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/resources/traces/sample_trace_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/resources/traces/sample_trace_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    31962 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/resources/traces/sample_trace_3.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.064137 mappymatch-0.4.1/mappymatch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/utils/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/utils/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/utils/process_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.052136 mappymatch-0.4.1/mappymatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-17 20:18:38.000000 mappymatch-0.4.1/mappymatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-17 20:18:38.000000 mappymatch-0.4.1/mappymatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:18:38.000000 mappymatch-0.4.1/mappymatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-17 20:18:38.000000 mappymatch-0.4.1/mappymatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 20:18:38.000000 mappymatch-0.4.1/mappymatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-17 20:18:22.000000 mappymatch-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:18:38.068137 mappymatch-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:18:22.000000 mappymatch-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.068137 mappymatch-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_geofence.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_add_match_for_stationary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_drop_stationary_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_find_stationary_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_forward_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_reverse_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_same_trajectory_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_match_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_osm.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_process_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.909045 mappymatch-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-08 16:04:00.000000 mappymatch-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 16:04:00.000000 mappymatch-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-08 16:04:06.909045 mappymatch-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-08 16:04:00.000000 mappymatch-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.897045 mappymatch-0.4.2/mappymatch/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.897045 mappymatch-0.4.2/mappymatch/constructs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/constructs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/constructs/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/constructs/geofence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/constructs/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/constructs/road.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/constructs/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.897045 mappymatch-0.4.2/mappymatch/maps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.901045 mappymatch-0.4.2/mappymatch/maps/igraph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/igraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/igraph/igraph_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/map_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.901045 mappymatch-0.4.2/mappymatch/maps/nx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/nx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/nx/nx_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.901045 mappymatch-0.4.2/mappymatch/maps/nx/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/nx/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/maps/nx/readers/osm_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.901045 mappymatch-0.4.2/mappymatch/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.901045 mappymatch-0.4.2/mappymatch/matchers/lcss/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/lcss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/lcss/constructs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/lcss/lcss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/lcss/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/lcss/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/line_snap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/matcher_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/osrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/matchers/valhalla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.901045 mappymatch-0.4.2/mappymatch/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.901045 mappymatch-0.4.2/mappymatch/resources/traces/
+-rw-r--r--   0 runner    (1001) docker     (127)    22920 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/resources/traces/sample_trace_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17321 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/resources/traces/sample_trace_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    31962 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/resources/traces/sample_trace_3.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.905045 mappymatch-0.4.2/mappymatch/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/utils/crs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/utils/geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/utils/process_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-08 16:04:00.000000 mappymatch-0.4.2/mappymatch/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.905045 mappymatch-0.4.2/mappymatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-08 16:04:06.000000 mappymatch-0.4.2/mappymatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-08 16:04:06.000000 mappymatch-0.4.2/mappymatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:04:06.000000 mappymatch-0.4.2/mappymatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-08 16:04:06.000000 mappymatch-0.4.2/mappymatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 16:04:06.000000 mappymatch-0.4.2/mappymatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-08 16:04:00.000000 mappymatch-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:04:06.909045 mappymatch-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:04:00.000000 mappymatch-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:06.905045 mappymatch-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_geofence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_add_match_for_stationary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12069 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_drop_stationary_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_find_stationary_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_forward_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_reverse_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_lcss_same_trajectory_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_match_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_osm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_process_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-08 16:04:00.000000 mappymatch-0.4.2/tests/test_trace.py
```

### Comparing `mappymatch-0.4.1/LICENSE` & `mappymatch-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/PKG-INFO` & `mappymatch-0.4.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,26 @@
-Metadata-Version: 2.1
-Name: mappymatch
-Version: 0.4.1
-Summary: Package for mapmatching.
-Author: National Renewable Energy Laboratory
-License: BSD 3-Clause License Copyright (c) 2022, Alliance for Sustainable Energy, LLC
-Project-URL: Homepage, https://github.com/NREL/mappymatch
-Keywords: GPS,map,match
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: docs
-Provides-Extra: dev
-License-File: LICENSE
-
 # mappymatch
 
 Mappymatch is a pure-python package developed and open sourced by the National Renewable Energy Laboratory. It contains a collection of "Matchers" that enable matching a GPS trace (series of GPS coordinates) to a map.
 
-The current and planned Matchers are:
+![Map Matching Animation](docs/source/images/map-matching.gif?raw=true)
+
+The current matchers are:
 
-- `LCSSMatcher`: A matcher that implements the LCSS algorithm described in this [paper](https://doi.org/10.3141%2F2645-08). Works best with high resolution GPS traces.  
+- `LCSSMatcher`: A matcher that implements the LCSS algorithm described in this [paper](https://doi.org/10.3141%2F2645-08). Works best with high resolution GPS traces.
 - `OsrmMatcher`: A light matcher that pings an OSRM server to request map matching results. See the [official documentation](http://project-osrm.org/) for more info.
 - `ValhallaMatcher`: A matcher to ping a [Valhalla](https://www.interline.io/valhalla/) server for map matching results.
 
 Currently supported map formats are:
 
 - Open Street Maps
 
 ## Installation
 
-```
+```console
 pip install mappymatch
 ```
 
 If you have trouble with that, check out [the docs](https://mappymatch.readthedocs.io/en/latest/general/install.html) for more detailed install instructions.
 
 ## Example Usage
```

### Comparing `mappymatch-0.4.1/mappymatch/constructs/coordinate.py` & `mappymatch-0.4.2/mappymatch/constructs/coordinate.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,30 +5,28 @@
 
 from pyproj import CRS, Transformer
 from pyproj.exceptions import ProjError
 from shapely.geometry import Point
 
 from mappymatch.utils.crs import LATLON_CRS
 
-CoordinateId: Any
-
 
 class Coordinate(NamedTuple):
     """
     Represents a single coordinate with a CRS and a geometry
 
     Attributes:
         coordinate_id: The unique identifier for this coordinate
         geom: The geometry of this coordinate
         crs: The CRS of this coordinate
         x: The x value of this coordinate
         y: The y value of this coordinate
     """
 
-    coordinate_id: CoordinateId
+    coordinate_id: Any
     geom: Point
     crs: CRS
 
     def __repr__(self):
         crs_a = self.crs.to_authority() if self.crs else "Null"
         return f"Coordinate(coordinate_id={self.coordinate_id}, x={self.x}, y={self.y}, crs={crs_a})"
```

### Comparing `mappymatch-0.4.1/mappymatch/constructs/geofence.py` & `mappymatch-0.4.2/mappymatch/constructs/geofence.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         return Geofence(crs=frame.crs, geometry=polygon)
 
     @classmethod
     def from_trace(
         cls,
         trace: Trace,
-        padding: float = 15,
+        padding: float = 1e3,
         crs: CRS = LATLON_CRS,
         buffer_res: int = 2,
     ) -> Geofence:
         """
         Create a new geofence from a trace.
 
         This is done by computing a radial buffer around the
```

### Comparing `mappymatch-0.4.1/mappymatch/constructs/match.py` & `mappymatch-0.4.2/mappymatch/constructs/match.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch/constructs/road.py` & `mappymatch-0.4.2/mappymatch/constructs/road.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Convert the road to a dictionary
         """
         d = self._asdict()
         d["origin_junction_id"] = self.road_id.start
-        d["origin_destination_id"] = self.road_id.end
+        d["destination_junction_id"] = self.road_id.end
         d["road_key"] = self.road_id.key
 
         return d
 
     def to_flat_dict(self) -> Dict[str, Any]:
         """
         Convert the road to a flat dictionary
```

### Comparing `mappymatch-0.4.1/mappymatch/constructs/trace.py` & `mappymatch-0.4.2/mappymatch/constructs/trace.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch/maps/igraph/igraph_map.py` & `mappymatch-0.4.2/mappymatch/maps/igraph/igraph_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,14 @@
             edge_data[self._geom_key],
             metadata=metadata,
         )
 
         return road
 
     def _build_rtree(self):
-
         idx = rt.index.Index()
 
         for e in self.g.es:
             geom = e.attributes()[self._geom_key]
             box = geom.bounds
 
             idx.insert(e.index, box)
```

### Comparing `mappymatch-0.4.1/mappymatch/maps/map_interface.py` & `mappymatch-0.4.2/mappymatch/maps/map_interface.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch/maps/nx/nx_map.py` & `mappymatch-0.4.2/mappymatch/maps/nx/nx_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,21 +195,22 @@
             file: The graph pickle file to load the graph from
 
         Returns:
             A NxMap instance
         """
         p = Path(file)
         if p.suffix == ".pickle":
-            g = nx.readwrite.read_gpickle(file)
-            return NxMap(g)
+            raise ValueError(
+                "NxMap does not support reading from pickle files, please use .json instead"
+            )
         elif p.suffix == ".json":
             with p.open("r") as f:
                 return NxMap.from_dict(json.load(f))
         else:
-            raise TypeError("NxMap only supports pickle and json files")
+            raise TypeError("NxMap only supports reading from json files")
 
     @classmethod
     def from_geofence(
         cls,
         geofence: Geofence,
         xy: bool = True,
         network_type: NetworkType = NetworkType.DRIVE,
@@ -242,32 +243,34 @@
 
         Args:
             outfile: The file to save the graph to
         """
         outfile = Path(outfile)
 
         if outfile.suffix == ".pickle":
-            nx.write_gpickle(self.g, str(outfile))
+            raise ValueError(
+                "NxMap does not support writing to pickle files, please use .json instead"
+            )
         elif outfile.suffix == ".json":
             graph_dict = self.to_dict()
             with open(outfile, "w") as f:
                 json.dump(graph_dict, f)
         else:
-            raise TypeError(
-                "NxMap only supports writing to pickle and json files"
-            )
+            raise TypeError("NxMap only supports writing to json files")
 
     @classmethod
     def from_dict(cls, d: Dict[str, Any]) -> NxMap:
         """
         Build a NxMap instance from a dictionary
         """
+        geom_key = d["graph"].get("geometry_key", DEFAULT_GEOMETRY_KEY)
+
         for link in d["links"]:
-            geom_wkt = link["geom"]
-            link["geom"] = wkt.loads(geom_wkt)
+            geom_wkt = link[geom_key]
+            link[geom_key] = wkt.loads(geom_wkt)
 
         crs_key = d["graph"].get("crs_key", DEFAULT_CRS_KEY)
         crs = CRS.from_wkt(d["graph"][crs_key])
         d["graph"][crs_key] = crs
 
         g = nx.readwrite.json_graph.node_link_graph(d)
 
@@ -277,16 +280,16 @@
         """
         Convert the map to a dictionary
         """
         graph_dict = nx.readwrite.json_graph.node_link_data(self.g)
 
         # convert geometries to well know text
         for link in graph_dict["links"]:
-            geom = link["geom"]
-            link["geom"] = geom.wkt
+            geom = link[self._geom_key]
+            link[self._geom_key] = geom.wkt
 
         # convert crs to well known text
         crs_key = graph_dict["graph"].get("crs_key", DEFAULT_CRS_KEY)
         graph_dict["graph"][crs_key] = self.crs.to_wkt()
 
         return graph_dict
```

### Comparing `mappymatch-0.4.1/mappymatch/maps/nx/readers/osm_readers.py` & `mappymatch-0.4.2/mappymatch/maps/nx/readers/osm_readers.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch/matchers/lcss/constructs.py` & `mappymatch-0.4.2/mappymatch/matchers/lcss/constructs.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch/matchers/lcss/lcss.py` & `mappymatch-0.4.2/mappymatch/matchers/lcss/lcss.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,14 @@
         return MatchResult(matches_w_stationary_points, joined_segment.path)
 
     def match_trace_batch(
         self,
         trace_batch: List[Trace],
         processes: int = 1,
     ) -> List[MatchResult]:
-
         if processes > 1:
             results = [self.match_trace(t) for t in trace_batch]
         else:
             with Pool(processes=processes) as p:
                 results = p.map(self.match_trace, trace_batch)
 
         return results
```

### Comparing `mappymatch-0.4.1/mappymatch/matchers/lcss/ops.py` & `mappymatch-0.4.2/mappymatch/matchers/lcss/ops.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch/matchers/lcss/utils.py` & `mappymatch-0.4.2/mappymatch/matchers/lcss/utils.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch/matchers/line_snap.py` & `mappymatch-0.4.2/mappymatch/matchers/line_snap.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch/matchers/match_result.py` & `mappymatch-0.4.2/mappymatch/matchers/match_result.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,7 +20,23 @@
         Returns:
             A pandas dataframe
         """
         df = pd.DataFrame([m.to_flat_dict() for m in self.matches])
         df = df.fillna(np.NAN)
 
         return df
+
+    def path_to_dataframe(self) -> pd.DataFrame:
+        """
+        Returns a dataframe with the resulting estimated trace path through the road network.
+        The dataframe is empty if there was no path.
+
+        Returns:
+            A pandas dataframe
+        """
+        if self.path is None:
+            return pd.DataFrame()
+
+        df = pd.DataFrame([r.to_flat_dict() for r in self.path])
+        df = df.fillna(np.NAN)
+
+        return df
```

### Comparing `mappymatch-0.4.1/mappymatch/matchers/matcher_interface.py` & `mappymatch-0.4.2/mappymatch/matchers/matcher_interface.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch/matchers/osrm.py` & `mappymatch-0.4.2/mappymatch/matchers/osrm.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch/matchers/valhalla.py` & `mappymatch-0.4.2/mappymatch/matchers/valhalla.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch/resources/traces/sample_trace_1.csv` & `mappymatch-0.4.2/mappymatch/resources/traces/sample_trace_1.csv`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch/resources/traces/sample_trace_2.csv` & `mappymatch-0.4.2/mappymatch/resources/traces/sample_trace_2.csv`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch/resources/traces/sample_trace_3.csv` & `mappymatch-0.4.2/mappymatch/resources/traces/sample_trace_3.csv`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch/utils/geo.py` & `mappymatch-0.4.2/mappymatch/utils/geo.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch/utils/plot.py` & `mappymatch-0.4.2/mappymatch/utils/plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from typing import List
+from typing import List, Optional, Union
 
 import folium
 import geopandas as gpd
 import matplotlib.pyplot as plt
 import pandas as pd
 from pyproj import CRS
 from shapely.geometry import Point
 
+from mappymatch.constructs.geofence import Geofence
 from mappymatch.constructs.match import Match
 from mappymatch.constructs.road import Road
+from mappymatch.constructs.trace import Trace
 from mappymatch.maps.nx.nx_map import NxMap
 from mappymatch.matchers.matcher_interface import MatchResult
 from mappymatch.utils.crs import LATLON_CRS, XY_CRS
 
 
-def plot_geofence(geofence, m=None):
+def plot_geofence(geofence: Geofence, m: Optional[folium.Map] = None):
     """
     Plot geofence.
 
     Args:
         geofence: The geofence to plot
         m: the folium map to plot on
 
@@ -35,58 +37,72 @@
         m = folium.Map(location=[c[1], c[0]], zoom_start=11)
 
     folium.GeoJson(geofence.geometry).add_to(m)
 
     return m
 
 
-def plot_trace(trace, m=None, point_color="yellow", line_color="green"):
+def plot_trace(
+    trace: Trace,
+    m: Optional[folium.Map] = None,
+    point_color: str = "black",
+    line_color: Optional[str] = "green",
+):
     """
     Plot a trace.
 
     Args:
         trace: The trace.
         m: the folium map to plot on
         point_color: The color the points will be plotted in.
-        line_color: The color for lines.
+        line_color: The color for lines. If None, no lines will be plotted.
 
     Returns:
         An updated folium map with a plot of trace.
     """
 
     if not trace.crs == LATLON_CRS:
         trace = trace.to_crs(LATLON_CRS)
 
     if not m:
         mid_coord = trace.coords[int(len(trace) / 2)]
         m = folium.Map(location=[mid_coord.y, mid_coord.x], zoom_start=11)
 
     for i, c in enumerate(trace.coords):
         folium.Circle(
-            location=(c.y, c.x), radius=5, color=point_color, tooltip=i
+            location=(c.y, c.x),
+            radius=5,
+            color=point_color,
+            tooltip=i,
+            fill=True,
+            fill_opacity=0.8,
+            fill_color=point_color,
         ).add_to(m)
 
-    folium.PolyLine(
-        [(p.y, p.x) for p in trace.coords], color=line_color
-    ).add_to(m)
+    if line_color is not None:
+        folium.PolyLine(
+            [(p.y, p.x) for p in trace.coords], color=line_color
+        ).add_to(m)
 
     return m
 
 
-def plot_matches(matches: List[Match], crs=XY_CRS):
+def plot_matches(matches: Union[MatchResult, List[Match]], crs=XY_CRS):
     """
     Plots a trace and the relevant matches on a folium map.
 
     Args:
-    matches: The matches.
-    road_map: The road map.
+    matches: A list of matches or a MatchResult.
+    crs: what crs to plot in. Defaults to XY_CRS.
 
     Returns:
         A folium map with trace and matches plotted.
     """
+    if isinstance(matches, MatchResult):
+        matches = matches.matches
 
     def _match_to_road(m):
         """Private function."""
         d = {"road_id": m.road.road_id, "geom": m.road.geom}
         return d
 
     def _match_to_coord(m):
@@ -131,15 +147,15 @@
             color="red",
             tooltip=road.road_id,
         ).add_to(fmap)
 
     return fmap
 
 
-def plot_map(tmap: NxMap, m=None):
+def plot_map(tmap: NxMap, m: Optional[folium.Map] = None):
     """
     Plot the roads on an NxMap.
 
     Args:
         tmap: The Nxmap to plot.
         m: the folium map to add to
 
@@ -189,32 +205,46 @@
     plt.scatter(x, y)
     plt.title("Distance To Nearest Road")
     plt.ylabel("Meters")
     plt.xlabel("Point Along The Path")
     plt.show()
 
 
-def plot_path(path: List[Road], crs: CRS):
+def plot_path(
+    path: List[Road],
+    crs: CRS,
+    m: Optional[folium.Map] = None,
+    line_color="red",
+    line_weight=10,
+    line_opacity=0.8,
+):
     """
     Plot a list of roads.
 
     Args:
         path: The path to plot.
         crs: The crs of the path.
+        m: The folium map to add to.
+        line_color: The color of the line.
+        line_weight: The weight of the line.
+        line_opacity: The opacity of the line.
     """
     road_df = pd.DataFrame([{"geom": r.geom} for r in path])
     road_gdf = gpd.GeoDataFrame(road_df, geometry=road_df.geom, crs=crs)
     road_gdf = road_gdf.to_crs(LATLON_CRS)
 
-    mid_i = int(len(road_gdf) / 2)
-    mid_coord = road_gdf.iloc[mid_i].geometry.coords[0]
+    if m is None:
+        mid_i = int(len(road_gdf) / 2)
+        mid_coord = road_gdf.iloc[mid_i].geometry.coords[0]
 
-    fmap = folium.Map(location=[mid_coord[1], mid_coord[0]], zoom_start=11)
+        m = folium.Map(location=[mid_coord[1], mid_coord[0]], zoom_start=11)
 
     for i, road in enumerate(road_gdf.itertuples()):
         folium.PolyLine(
             [(lat, lon) for lon, lat in road.geometry.coords],
-            color="red",
+            color=line_color,
             tooltip=i,
-        ).add_to(fmap)
+            weight=line_weight,
+            opacity=line_opacity,
+        ).add_to(m)
 
-    return fmap
+    return m
```

### Comparing `mappymatch-0.4.1/mappymatch/utils/process_trace.py` & `mappymatch-0.4.2/mappymatch/utils/process_trace.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/mappymatch.egg-info/SOURCES.txt` & `mappymatch-0.4.2/mappymatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/pyproject.toml` & `mappymatch-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mappymatch"
-version = "0.4.1"
+version = "0.4.2"
 description = "Package for mapmatching."
 readme = "README.md"
 authors = [{ name = "National Renewable Energy Laboratory" }]
 license = { text = "BSD 3-Clause License Copyright (c) 2022, Alliance for Sustainable Energy, LLC" }
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
@@ -24,15 +24,15 @@
   "shapely",
   "rtree",
   "pyproj",
   "pandas",
   "numpy",
   "matplotlib",
   "osmnx",
-  "networkx<3",
+  "networkx",
   "igraph",
   "folium",
   "requests",
   "polyline",
 ]
 requires-python = ">=3.8"
```

### Comparing `mappymatch-0.4.1/tests/test_coordinate.py` & `mappymatch-0.4.2/tests/test_coordinate.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/tests/test_lcss_add_match_for_stationary.py` & `mappymatch-0.4.2/tests/test_lcss_add_match_for_stationary.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/tests/test_lcss_compress.py` & `mappymatch-0.4.2/tests/test_lcss_compress.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/tests/test_lcss_drop_stationary_points.py` & `mappymatch-0.4.2/tests/test_lcss_drop_stationary_points.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/tests/test_lcss_find_stationary_points.py` & `mappymatch-0.4.2/tests/test_lcss_find_stationary_points.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/tests/test_lcss_forward_merge.py` & `mappymatch-0.4.2/tests/test_lcss_forward_merge.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/tests/test_lcss_merge.py` & `mappymatch-0.4.2/tests/test_lcss_merge.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/tests/test_lcss_reverse_merge.py` & `mappymatch-0.4.2/tests/test_lcss_reverse_merge.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/tests/test_lcss_same_trajectory_scheme.py` & `mappymatch-0.4.2/tests/test_lcss_same_trajectory_scheme.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/tests/test_match_result.py` & `mappymatch-0.4.2/tests/test_match_result.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/tests/test_osm.py` & `mappymatch-0.4.2/tests/test_osm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from unittest import TestCase
 
 import networkx as nx
+import osmnx as ox
 
 from mappymatch.maps.nx.readers.osm_readers import (
     NetworkType,
     parse_osmnx_graph,
 )
 from tests import get_test_dir
 
 
 class TestOSMap(TestCase):
     def test_osm_networkx_graph_drive(self):
-        gfile = get_test_dir() / "test_assets" / "osmnx_drive_graph.pickle"
+        gfile = get_test_dir() / "test_assets" / "osmnx_drive_graph.graphml"
 
-        osmnx_graph = nx.readwrite.read_gpickle(gfile)
+        osmnx_graph = ox.load_graphml(gfile)
 
         cleaned_graph = parse_osmnx_graph(osmnx_graph, NetworkType.DRIVE)
 
         self.assertEqual(
             cleaned_graph.graph["network_type"], NetworkType.DRIVE.value
         )
```

### Comparing `mappymatch-0.4.1/tests/test_process_trace.py` & `mappymatch-0.4.2/tests/test_process_trace.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.1/tests/test_trace.py` & `mappymatch-0.4.2/tests/test_trace.py`

 * *Files identical despite different names*

