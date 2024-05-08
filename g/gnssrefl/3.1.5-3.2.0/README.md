# Comparing `tmp/gnssrefl-3.1.5.tar.gz` & `tmp/gnssrefl-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-3.1.5.tar", last modified: Mon Apr 15 18:28:21 2024, max compression
+gzip compressed data, was "gnssrefl-3.2.0.tar", last modified: Wed May  8 15:26:45 2024, max compression
```

## Comparing `gnssrefl-3.1.5.tar` & `gnssrefl-3.2.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.784948 gnssrefl-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-15 18:28:21.784948 gnssrefl-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.756948 gnssrefl-3.1.5/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/check_rinex_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25021 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.760948 gnssrefl-3.1.5/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/decipher_argt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14619 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/filesizes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gnssir_cl_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    20577 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gnssir_input.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    41964 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gnssir_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    50903 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (127)    50899 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (127)   199207 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)    40525 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (127)    14913 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    25457 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/make_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/max_resolve_RH_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/mjd.py
--rw-r--r--   0 runner    (1001) docker     (127)    34201 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/nmea2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/nyquist_libs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51554 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18818 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/quickLook_function2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5978 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/quickPhase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/quicklib.py
--rw-r--r--   0 runner    (1001) docker     (127)    19877 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    19450 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    35142 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    57267 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    25224 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rinex_coords.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24490 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    38571 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/sd_libs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/smoosh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/smoosh_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    16533 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    61061 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    45925 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (127)    20834 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/vwc_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    32950 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/xnmeasnr.f
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.760948 gnssrefl-3.1.5/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-15 18:28:21.000000 gnssrefl-3.1.5/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-15 18:28:21.000000 gnssrefl-3.1.5/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:28:21.000000 gnssrefl-3.1.5/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-15 18:28:21.000000 gnssrefl-3.1.5/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-15 18:28:21.000000 gnssrefl-3.1.5/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 18:28:21.000000 gnssrefl-3.1.5/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:28:21.784948 gnssrefl-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.784948 gnssrefl-3.1.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:45.088953 gnssrefl-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 15:26:37.000000 gnssrefl-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 15:26:37.000000 gnssrefl-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-08 15:26:45.088953 gnssrefl-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-08 15:26:37.000000 gnssrefl-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:45.060953 gnssrefl-3.2.0/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/check_rinex_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25021 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:45.060953 gnssrefl-3.2.0/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/decipher_argt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14619 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/filesizes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gnssir_cl_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21055 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gnssir_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44620 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gnssir_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50903 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (127)    50899 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (127)   199307 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40525 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)    14913 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25457 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/make_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/max_resolve_RH_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/mjd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34201 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/nmea2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/nyquist_libs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51554 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18818 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/quickLook_function2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5978 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/quickPhase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/quicklib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19450 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43423 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57267 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25224 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rinex_coords.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24490 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38571 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/sd_libs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/smoosh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/smoosh_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16533 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61269 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45925 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20834 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/vwc_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32950 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/xnmeasnr.f
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:45.060953 gnssrefl-3.2.0/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-08 15:26:45.000000 gnssrefl-3.2.0/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-08 15:26:45.000000 gnssrefl-3.2.0/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:26:45.000000 gnssrefl-3.2.0/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-08 15:26:45.000000 gnssrefl-3.2.0/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 15:26:45.000000 gnssrefl-3.2.0/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 15:26:45.000000 gnssrefl-3.2.0/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:26:45.088953 gnssrefl-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:45.088953 gnssrefl-3.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-08 15:26:38.000000 gnssrefl-3.2.0/test/test_rinex2snr.py
```

### Comparing `gnssrefl-3.1.5/LICENSE` & `gnssrefl-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/PKG-INFO` & `gnssrefl-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 3.1.5
+Version: 3.2.0
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# gnssrefl v3.1.5 
+# gnssrefl v3.2.0 
 
 If you use this code in any presentation or publication, you are expected to cite either 
 this github repository or the gnssrefl DOI, which is given just below.
 
 [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) 
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601494.svg)](http://dx.doi.org/10.5281/zenodo.5601494)
```

### Comparing `gnssrefl-3.1.5/README.md` & `gnssrefl-3.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gnssrefl v3.1.5 
+# gnssrefl v3.2.0 
 
 If you use this code in any presentation or publication, you are expected to cite either 
 this github repository or the gnssrefl DOI, which is given just below.
 
 [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) 
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601494.svg)](http://dx.doi.org/10.5281/zenodo.5601494)
```

### Comparing `gnssrefl-3.1.5/gnssrefl/EGM96.py` & `gnssrefl-3.2.0/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/check_rinex_file.py` & `gnssrefl-3.2.0/gnssrefl/check_rinex_file.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/computemp1mp2.py` & `gnssrefl-3.2.0/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/daily_avg.py` & `gnssrefl-3.2.0/gnssrefl/daily_avg.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/daily_avg_cl.py` & `gnssrefl-3.2.0/gnssrefl/daily_avg_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-3.2.0/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/decipher_argt.py` & `gnssrefl-3.2.0/gnssrefl/decipher_argt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/download_ioc.py` & `gnssrefl-3.2.0/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/download_noaa.py` & `gnssrefl-3.2.0/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/download_orbits.py` & `gnssrefl-3.2.0/gnssrefl/download_orbits.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/download_psmsl.py` & `gnssrefl-3.2.0/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/download_rinex.py` & `gnssrefl-3.2.0/gnssrefl/download_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/download_teqc.py` & `gnssrefl-3.2.0/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/download_tides.py` & `gnssrefl-3.2.0/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/download_unr.py` & `gnssrefl-3.2.0/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/download_wsv.py` & `gnssrefl-3.2.0/gnssrefl/download_wsv.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/filesizes.py` & `gnssrefl-3.2.0/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/gnssir_cl.py` & `gnssrefl-3.2.0/gnssrefl/gnssir_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/gnssir_cl_old.py` & `gnssrefl-3.2.0/gnssrefl/gnssir_cl_old.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/gnssir_input.py` & `gnssrefl-3.2.0/gnssrefl/gnssir_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,16 @@
     parser.add_argument("-extension", default=None,type=str, help="Provide extension name so you can try different strategies")
     parser.add_argument("-ediff", default=None, type=float, help="Allowed min/max elevation diff from obs min/max elev angle (degrees) default is 2")
     parser.add_argument("-delTmax", default=None, type=float, help="max arc length (min) default is 75. Shorten for tides.")
     parser.add_argument("-frlist", nargs="*",type=int,  help="User defined frequencies using our nomenclature")
     parser.add_argument("-azlist2", nargs="*",type=float,  default=None,help="list of azimuth regions, default is 0-360") 
     parser.add_argument("-ellist", nargs="*",type=float,  default=None,help="List of elevation angles, advanced users only!") 
     parser.add_argument("-refr_model", default=1, type=int, help="refraction model. default is 1, zero turns it off)")
-    parser.add_argument("-Hortho", default=None, type=float, help="station orthometric height, meters")
+    parser.add_argument("-apriori_rh", default=None, type=float, help="apriori reflector height (m) used by NITE model")
+    parser.add_argument("-Hortho", default=None, type=float, help="station orthometric height (m)")
     parser.add_argument("-pele", nargs="*", type=float, help="min and max elevation angle in direct signal removal, default is 5-30")
     parser.add_argument("-daily_avg_medfilter", default=None, type=float, help="daily_avg, median filter, meters")
     parser.add_argument("-daily_avg_reqtracks", default=None, type=int, help="daily_avg, ReqTracks parameter ")
     parser.add_argument("-subdaily_alt_sigma", default=None, type=str, help="subdaily, Nievinski sigma")
     parser.add_argument("-subdaily_sigma", default=None, type=str, help="subdaily, sigma for part 1")
     parser.add_argument("-subdaily_ampl", default=None, type=float, help="subdaily, LSP amplitude override")
     parser.add_argument("-subdaily_delta_out", default=None, type=int, help="subdaily, spline output interval (sec)")
@@ -62,16 +63,17 @@
 
 
 def make_gnssir_input(station: str, lat: float=0, lon: float=0, height: float=0, e1: float = 5.0, e2: float = 25.0,
        h1: float = 0.5, h2: float = 8.0, nr1: float = None, nr2: float = None, peak2noise: float = 2.8, 
        ampl: float = 5.0, allfreq: bool = False, l1: bool = False, l2c: bool = False, 
        xyz: bool = False, refraction: bool = True, extension: str = '', ediff: float=2.0, 
        delTmax: float=75.0, frlist: list=[], azlist2: list=[0,360], ellist : list=[], refr_model : int=1, 
-                      Hortho : float = None, pele: list=[5,30], daily_avg_reqtracks: int=None, 
-                      daily_avg_medfilter: float =None, subdaily_alt_sigma : bool=None, subdaily_ampl : float=None, subdaily_delta_out : float=None, 
+                      apriori_rh: float=None, Hortho : float = None, pele: list=[5,30], daily_avg_reqtracks: int=None, 
+                      daily_avg_medfilter: float =None, subdaily_alt_sigma : bool=None, 
+                      subdaily_ampl : float=None, subdaily_delta_out : float=None, 
                       subdaily_knots : int=None, subdaily_sigma: float=None, subdaily_subdir: str=None, 
                       subdaily_spline_outlier1: float=None, subdaily_spline_outlier2: float=None):
 
     """
     This new script sets the Lomb Scargle analysis strategy you will use in gnssir. It saves your inputs 
     to a json file which by default is saved in REFL_CODE/<station>.json. This code replaces make_json_input.
 
@@ -95,15 +97,16 @@
     they are inadvertently mixing files with different strategies. And that is why it is an integer, because
     all results in the LSP results files are numbers.  Going forward, we are adding a time-varying capability.
 
         Model 1: Bennett, static
         Model 2: Bennett and time-varying
         Model 3: Ulich, static
         Model 4: Ulich, time-varying
-        Model 5: NITE, Feng et al. 2023 DOI: 10.1109/TGRS.2023.3332422
+        Model 5: NITE, Feng et al. 2023 DOI: 10.1109/TGRS.2023.3332422, time-varying
+        Model 6: MPF, Williams and Nievinski, 2017,  DOI: 10.1002/2016JB013612, time-varying
 
     gnssir_input will have a new parameter for the json output, refr_model. If it is not set, i.e. you 
     have an old json, it is assumed to be 1. You can change the refraction model by 
     hand editting the file if you like. And you can certainly test out the impact by using -extension option.
 
     Examples
     --------
@@ -216,14 +219,17 @@
 
     refr_model : int
         refraction model. we are keeping this as integer as it is written to a file withonly
         numbers in it.  1 is the default simple refraction (just correct elevation angles
         using standard bending models).  0 is no refraction correction.  As we add more
         models, they will receiver their own number. 
 
+    apriori_rh : float
+        apriori reflector height (meters). only used in NITE model 
+
     Hortho : float
         station orthometric height, in meters. Currently only used in subdaily.  If not provided on the command line, 
         it will use ellipsoidal height and EGM96 to compute.
 
     pele : float
         min and max elevation angles in direct signal removal, i.e. 3 40. Default is 5 30. 
 
@@ -289,23 +295,27 @@
             sys.exit()
 
     # calculate Hortho using EGM96 if none provided
     if Hortho is None:
         geoidC = g.geoidCorrection(lat,lon)
         Hortho = height - geoidC
 
+    if apriori_rh is None:
+        apriori_rh = 5 # completely made up, meters
+
 # start the lsp dictionary
     reqA = ampl
 
     lsp = {}
     lsp['station'] = station.lower()
     lsp['lat'] = lat
     lsp['lon'] = lon
     lsp['ht'] = height
     lsp['Hortho'] = round(Hortho,4) # no point having it be so many decimal points
+    lsp['apriori_rh'] = apriori_rh
     
 
     if h1 > h2:
         print(f'h1 cannot be greater than h2. You have set h1 to {h1} and h2 to {h2}. Exiting.')
         sys.exit()
 
     if ( (h2-h1)  < 5):
```

### Comparing `gnssrefl-3.1.5/gnssrefl/gnssir_v2.py` & `gnssrefl-3.2.0/gnssrefl/gnssir_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import math
 import numpy as np
 import os
 import scipy.interpolate
 import scipy.signal
 import subprocess
 import sys
+import time
 import warnings
 
 import gnssrefl.gps as g
 import gnssrefl.read_snr_files as snr
 import gnssrefl.refraction as refr
 
 def gnssir_guts_v2(station,year,doy, snr_type, extension,lsp):
@@ -61,14 +62,16 @@
             peak to noise value for QC
         ediff : float
             elev angle difference for arc length, QC
         reqAmp : float
             required periodogram amplitude for QC
         ellist: list of floats
             added 23jun16, allow multiple elevation angle regions
+        apriori_rh : float
+            a priori reflector height, used in NITE, meters
         
     """
 
     #   make sure environment variables exist.  set to current directory if not
     g.check_environ_variables()
 
     # make sure REFL_CODE/Files/station directory exists ... 
@@ -78,26 +81,24 @@
         ellist = lsp['ellist']
         if len(ellist) > 0:
             print('Using an augmented elevation angle list', ellist)
     else:
         ellist = [];
         #print('no augmented elevation angle list')
 
-
-
     # this is also checked in the command line - but for people calling the code ...
     if ((lsp['maxH'] - lsp['minH']) < 5):
         print('Requested reflector heights (', lsp['minH'], ',', lsp['maxH'], ') are too close together. Exiting.')
         print('They must be at least 5 meters apart - and preferably further than that.')
         return
 
     e1=lsp['e1']; e2=lsp['e2']; minH = lsp['minH']; maxH = lsp['maxH']
     ediff = lsp['ediff']; NReg = lsp['NReg']  
     PkNoise = lsp['PkNoise']; prec = lsp['desiredP']; delTmax = lsp['delTmax']
-    if 'azval2' in lsp:
+    if 'azval2' in lsp.keys():
         azval2 = lsp['azval2']; 
         naz = int(len(azval2)/2)
     else:
         print('This module requires azval2 to be set in gnssir_input. This record is not present in your json.')
         sys.exit()
 
     pele = lsp['pele'] ; pfitV = lsp['polyV']
@@ -129,30 +130,51 @@
     xdir = os.environ['REFL_CODE']
     ann = g.make_nav_dirs(year) # make sure directories are there for orbits
     g.result_directories(station,year,extension) # make directories for the LSP results
 
    # this defines the minimum number of points in an arc.  This depends entirely on the sampling
    # rate for the receiver, so you should not assume this value is relevant to your case.
     minNumPts = 20
-    p,T,irefr,humidity = set_refraction_params(station, dmjd, lsp)
-    # removing print statement for now.  should add screenstats parameter
-    if screenstats:
-        print('Refraction parameters (press, temp, humidity, ModelNum)',np.round(p,3),np.round(T,3),np.round(humidity,3),irefr)
-
-    if (irefr == 3) or (irefr == 4):
-        TempK = T + 273.15 # T is in celsius ... I think.
-        # N_ant is the refraction index
-        N_ant=refr.refrc_Rueger(p,humidity,TempK)[0]    #
+    p,T,irefr,humidity,Tm, lapse_rate = set_refraction_params(station, dmjd, lsp)
+    TempK = T + 273.15 # T is in celsius ... I think.
+    vapor = humidity
+    pressure = p
+    temperature = TempK
+    # peng used these variables. eventually consolidate
+    lat1=lsp['lat']; lon1=lsp['lon']; height1=lsp['ht'] ; mjd1 = dmjd
+    lat1R = math.radians(lat1); lon1R = math.radians(lon1); 
+
+    # only used by NITE
+    if 'apriori_rh' in lsp.keys():
+        RH_apriori = lsp['apriori_rh']  # a priori reflector height used in NITE
+    else:
+        RH_apriori = 5 # completely made up
 
+    #if screenstats:
+    print('Refraction parameters (pressure, temp, humidity, ModelNum)',np.round(p,3),np.round(T,3),np.round(humidity,3),irefr)
+
+    if (irefr >= 3) & (irefr <= 6):
+        # N_ant is the index of refraction
+        # apparently this is wrong ?
+        #N_ant=refr.refrc_Rueger(p,humidity,TempK)[0]    #
+        N_ant = refr.refrc_Rueger(pressure-vapor, vapor, TempK)[0]   #get antenne refractivity
+        #ztd=2.3                                             #zenith total delay from PPP
+        # hydrostatic delay, Saastamoinen
+        zhd = refr.saastam2(pressure, lat1, height1)             
+        # wet delay 
+        zwd = refr.asknewet(humidity, Tm, lapse_rate)
+        print('Dry and wet zenith delays, meters ', round(zhd,3),round(zwd,3))
+        # if you had estimated total delay, you could get wet delay by 
+        ztd = zhd + zwd 
 
 # only doing one day at a time for now - but have started defining the needed inputs for using it
     twoDays = False
     obsfile2= '' # dummy value for name of file for the day before, when we get to that
     fname, resultExist = g.LSPresult_name(station,year,doy,extension) 
-    #print('Results are written to:', fname)
+    print('Results are written to:', fname)
 
     if (lsp['nooverwrite'] == True) & (resultExist == True):
         allGood = 0
         print('>>>>> The result file already exists for this day and you have selected the do not overwrite option')
         #sys.exit()
     else:
         # uncompress here so you should not have to do it in read_snr_multiday ...
@@ -171,33 +193,59 @@
             snrD = snrD[iss,:]
             # not sure nrows and ncols is being used ... so not redoing it
 
 
         snr.compress_snr_files(lsp['wantCompression'], obsfile, obsfile2,twoDays,gzip) 
     if (allGood == 1):
         print('Reading from: ', obsfile)
-        print('Results will be written to:', fname)
+        #print('Results will be written to:', fname)
         minObsE = min(snrD[:,1])
         print('Min observed elev. angle ', station, year, doy, minObsE, '/requested e1 and e2 ', e1,e2)
         # only apply this test for simple e1 and e2
         if len(ellist) == 0:
             if minObsE > (e1 + ediff):
                 print('You literally have no data above the minimum elevation angle setting')
                 print('which is e1 + ediff: ', e1 + ediff, ' If you do not like')
                 print('this QC constraint, then set ediff to be very large (10 degrees) in the json or use ')
                 print('the minimum elevation angle your receiver used. Exiting.')
                 sys.exit()
 
         if (irefr == 3) or (irefr == 4):
-            # elev refraction, lsp, pres, temp, time, sat
+            # elev refraction, lsp, pressure, temperature- units?, time, sat
             if irefr == 3:
                 print('Ulich refraction correction')
             else:
                 print('Ulich refraction correction, time-varying')
+            # I do not understand why all these extra parameters are sent to this 
+            # function as they are not used. Maybe I was doing some testing.
             ele=refr.Ulich_Bending_Angle(snrD[:,1],N_ant,lsp,p,T,snrD[:,3],snrD[:,0])
+        elif (irefr == 5 ) or (irefr == 6):
+            # NITE MODEL
+            # remove ele < 1.5 cause it blows up
+            i=snrD[:,1] > 1.5
+            snrD = snrD[i,:]
+            N = len(snrD[:,1])
+            # elevation angles, degrees
+            ele=snrD[:,1]
+            # zenith angle in radians
+            zenithA = 0.5*np.pi - np.radians(ele)
+            #get mapping function and derivatives
+            [gmf_h,dgmf_h,gmf_w,dgmf_w]=refr.gmf_deriv(mjd1, lat1R, lon1R,height1,zenithA)
+            [mpf, dmpf]=[refr.mpf_tot(gmf_h,gmf_w,zhd,zwd),refr.mpf_tot(dgmf_h,dgmf_w,zhd,zwd)]
+
+            # inputs apriori RH, elevation angle, refractive index, zenith delay, mpf ?, dmpf?
+            if irefr == 5:
+                print('NITE refraction correction, Peng et al. remove data < 1.5 degrees')
+                dE_NITE=refr.Equivalent_Angle_Corr_NITE(RH_apriori, ele, N_ant, ztd, mpf, dmpf)
+                ele = ele + dE_NITE 
+            else: 
+                print('MPF refraction correction, Wiliams and Nievinski')
+                dE_MPF= refr.Equivalent_Angle_Corr_mpf(ele,mpf,N_ant,RH_apriori)
+                ele = ele + dE_MPF 
+
         elif irefr == 0:
             print('No refraction correction applied ')
             ele = snrD[:,1]
         else :
             if irefr == 1:
                 if screenstats:
                     print('Standard Bennett refraction correction')
@@ -207,14 +255,15 @@
             ele = snrD[:,1]
             ele=apply_refraction_corr(lsp,ele,p,T)
 
         # apply an elevation mask for all the data for the polynomial fit
         i= (ele >= pele[0]) & (ele < pele[1])
         ele = ele[i]
         snrD = snrD[i,:]
+        # why doesn't this have an i index, is it not used?
         sats = snrD[:,0]
         # make sure the snrD array has elevation angles fixed
         snrD[:,1] = ele # ????
 
         # open output file
         fout,frej = g.open_outputfile(station,year,doy,extension) 
 #  main loop a given list of frequencies
@@ -368,15 +417,15 @@
 
 def set_refraction_params(station, dmjd,lsp):
     """
     set values used in refraction correction
 
     Parameters
     ----------
-    station : string
+    station : str
         4 character station name
 
     dmjd : float
         modified julian date
 
     lsp : dictionary with information about the station
         lat : float
@@ -392,14 +441,18 @@
         pressure, hPa
     T : float
         temperature, Celsius
     irefr : int
         refraction model number I believe, which is also sent, so not needed
     e : float
         water vapor pressure, hPa
+    Tm : float
+        temperature in Kelvin
+    la : float
+        lapse rate
 
     """
 
     if 'refr_model' not in lsp.keys():
         # default is always to use refraction model 1
         # if for some reason it is missing ...
         refraction_model = 1
@@ -410,26 +463,28 @@
     xdir = os.environ['REFL_CODE']
     # default values
     p = 0; T = 0; irefr = 0; e=0
     if lsp['refraction']:
         irefr = refraction_model
         refr.readWrite_gpt2_1w(xdir, station, lsp['lat'], lsp['lon'])
         # time varying was originally set to no for now (it = 1)
-        # now allows time varying for models 2 and 4
-        if (refraction_model == 2) or (refraction_model == 4):
+        # now allows time varying for models 2, 4 and now MPF and NITE
+        if refraction_model in [2, 4, 5, 6]:
             it = 0
+            print('Using time-varying refraction parameter inputs')
+        #elif (refraction_model == 5):
         else:
             it = 1
         dlat = lsp['lat']*np.pi/180; dlong = lsp['lon']*np.pi/180; ht = lsp['ht']
         p,T,dT,Tm,e,ah,aw,la,undu = refr.gpt2_1w(station, dmjd,dlat,dlong,ht,it)
         # e is water vapor pressure, so humidity ??
         #print("Pressure {0:8.2f} Temperature {1:6.1f} \n".format(p,T))
 
     #print('refraction model', refraction_model,irefr)
-    return p,T,irefr, e
+    return p,T,irefr, e, Tm, la
 
 def apply_refraction_corr(lsp,ele,p,T):
     """
 
     Parameters
     ----------
     lsp : dictionary
```

### Comparing `gnssrefl-3.1.5/gnssrefl/gnsssnr.f` & `gnssrefl-3.2.0/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/gnsssnrbigger.f` & `gnssrefl-3.2.0/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/gps.py` & `gnssrefl-3.2.0/gnssrefl/gps.py`

 * *Files 0% similar despite different names*

```diff
@@ -2027,17 +2027,17 @@
     #versionNumber = 'working-on-it'
     tem = '% station ' + station + ' https://github.com/kristinemlarson/gnssrefl ' + versionNumber  + '\n'
     try:
         fout=open(filepath1,'w+')
 #       put a header in the output file
         fout.write(tem)
         fout.write("% Phase Center corrections have NOT been applied \n")
-        fout.write("% year, doy, RH, sat,UTCtime, Azim, Amp,  eminO, emaxO,NumbOf,freq,rise,EdotF, PkNoise  DelT     MJD   refr-appl\n")
+        fout.write("% year, doy, RH, sat,UTCtime, Azim, Amp,  eminO, emaxO,NumbOf,freq,rise,EdotF, PkNoise  DelT     MJD   refr-model\n")
         fout.write("% (1)  (2)   (3) (4)  (5)     (6)   (7)    (8)    (9)   (10)  (11) (12) (13)    (14)     (15)    (16)   (17)\n")
-        fout.write("%             m        hrs    deg   v/v    deg    deg  values            hrs               min         1 is yes  \n")
+        fout.write("%             m        hrs    deg   v/v    deg    deg  values            hrs             min           0 is none \n")
     except:
         print('problem on first attempt - so try making results directory')
         f1 = xdir + '/' + str(year) + '/results/'
         subprocess.call(['mkdir',f1])
         # os.system(cm)
         f2 = xdir + '/' + str(year) + '/results/' + station
         subprocess.call(['mkdir',f2])
@@ -5095,16 +5095,18 @@
     if os.path.isfile(fullname):
         subprocess.call(['unxz', fullname])
 
     if os.path.isfile(fdir + '/' + littlename):
         #print(littlename, ' already exists on disk')
         return littlename, fdir, True 
     try:
+        #g.replace_wget(url,littlename + '.gz')
         wget.download(url,littlename + '.gz')
-        subprocess.call(['gunzip', littlename + '.gz'])
+        if os.path.isfile(littlename + '.gz'):
+            subprocess.call(['gunzip', littlename + '.gz'])
     except:
         print('Problems downloading Rapid GFZ orbit')
         print(url)
 
     if os.path.isfile(littlename):
        store_orbitfile(littlename,year,'sp3') ; foundit = True
```

### Comparing `gnssrefl-3.1.5/gnssrefl/gpssnr.f` & `gnssrefl-3.2.0/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/gpsweek.py` & `gnssrefl-3.2.0/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/gpt_1wA.pickle` & `gnssrefl-3.2.0/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/highrate.py` & `gnssrefl-3.2.0/gnssrefl/highrate.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/installexe_cl.py` & `gnssrefl-3.2.0/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/invsnr_cl.py` & `gnssrefl-3.2.0/gnssrefl/invsnr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/invsnr_input.py` & `gnssrefl-3.2.0/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/karnak_libraries.py` & `gnssrefl-3.2.0/gnssrefl/karnak_libraries.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/kelly.py` & `gnssrefl-3.2.0/gnssrefl/kelly.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/llh2xyz.py` & `gnssrefl-3.2.0/gnssrefl/llh2xyz.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/make_meta.py` & `gnssrefl-3.2.0/gnssrefl/make_meta.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/max_resolve_RH_cl.py` & `gnssrefl-3.2.0/gnssrefl/max_resolve_RH_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/nmea2snr.py` & `gnssrefl-3.2.0/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/nmea2snr_cl.py` & `gnssrefl-3.2.0/gnssrefl/nmea2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/nyquist_libs.py` & `gnssrefl-3.2.0/gnssrefl/nyquist_libs.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/phase_functions.py` & `gnssrefl-3.2.0/gnssrefl/phase_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/prn2gps.py` & `gnssrefl-3.2.0/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/query_unr.py` & `gnssrefl-3.2.0/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/quickLook_cl.py` & `gnssrefl-3.2.0/gnssrefl/quickLook_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/quickLook_function2.py` & `gnssrefl-3.2.0/gnssrefl/quickLook_function2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/quickPhase.py` & `gnssrefl-3.2.0/gnssrefl/quickPhase.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/quicklib.py` & `gnssrefl-3.2.0/gnssrefl/quicklib.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/quickplt.py` & `gnssrefl-3.2.0/gnssrefl/quickplt.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     parser.add_argument("-errorcol",   help="column for errors for y-axis values", type=int,default=None)
     parser.add_argument("-mjd", help="True/T for when x-values are MJD ", type=str,default=None)
     parser.add_argument("-reverse", help="reverse the y-axis", type=str,default=None)
     parser.add_argument("-ymd", help="True/T for when columns 1-3 are year month day ", type=str,default=None)
     parser.add_argument("-ymdhm", help="True/T for when columns 1-5 are year month day hour minute", type=str,default=None)
     parser.add_argument("-xlabel", type=str, help="optional x-axis label", default=None)
     parser.add_argument("-ylabel", type=str, help="optional y-axis label", default=None)
-    parser.add_argument("-symbol", help="plot symbol, e.g. * or -", type=str,default=None)
+    parser.add_argument("-symbol", help="plot symbol, e.g. o or -", type=str,default=None)
     parser.add_argument("-title", help="optional title", type=str,default=None)
     parser.add_argument("-outfile", help="optional filename for plot. Must end in png", type=str,default=None)
     parser.add_argument("-xlimits", nargs="*",type=float, help="optional x-axis limits", default=None)
     parser.add_argument("-ylimits", nargs="*",type=float, help="optional y-axis limits", default=None)
     parser.add_argument("-ydoy", help="True/T for when columns 1-2 are year and doy", type=str,default=None)
     parser.add_argument("-filename2", help="second filename", type=str, default=None)
     parser.add_argument("-freq", help="spec freq, column 11 in a LSP file ", type=int,default=None)
@@ -412,29 +412,30 @@
         tval2 = g.ydoy2datetime(tvd2[:,0], tvd2[:,1])
 
     fig,ax=myplt.subplots()
 
     # i.e. using default
     if symbol is None:
         if yerrors:
-            ax.errorbar(tval, yval, yerr=tvd[:,errorcol], fmt='.',color='blue')
+            ax.errorbar(tval, yval, yerr=tvd[:,errorcol], fmt='.')
         else:
             ax.plot(tval, yval, 'b.')
     else:
         if yerrors:
             ax.errorbar(tval, yval, yerr=tvd[:,errorcol],fmt=symbol)
         else:
             ax.plot(tval, yval, symbol)
 
     # is second file currently supported???
     if secondFile:
         if symbol is None:
             ax.plot(tval2, yval2, 'r.')
         else:
-            ax.plot(tval2, yval2, color='red', fmt=symbol)
+            # ??
+            ax.plot(tval2, yval2, symbol )
 
     myplt.grid()
     myplt.ylabel(ylabel)
 
     if xlabel is not None:
         myplt.xlabel(xlabel)
     else:
```

### Comparing `gnssrefl-3.1.5/gnssrefl/read_snr_files.py` & `gnssrefl-3.2.0/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/refl_zones.py` & `gnssrefl-3.2.0/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/refl_zones_cl.py` & `gnssrefl-3.2.0/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/refraction.py` & `gnssrefl-3.2.0/gnssrefl/sd_libs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1070 +1,1145 @@
-"""
-written in python from 
-from original TU Vienna codes for GMF
-"""
+# subdaily libraries
 import datetime
 import math
-import os
-import pickle
-import subprocess
-import sys
-import wget
-
+import matplotlib.pyplot as plt
 import numpy as np
-from scipy.interpolate import interp1d
+from astropy.time import Time
 
+# gnssrefl specific code
 import gnssrefl.gps as g
+import gnssrefl.gnssir_v2 as guts2
 
-
-def read_4by5(station, dlat,dlon,hell):
+def mjd_to_obstimes(mjd):
     """
-    reads existing grid points for a given location
+    takes mjd array and converts to datetime for plotting.
 
     Parameters
     ----------
-    station : string
-        name of station
-    dlat : float
-        latitude in degrees
-    dlon : float
-        longitude in degrees
-    hell : float
-        ellipsoidal height in meters
+    mjd : numpy array of floats
+        mod julian date
 
     Returns
     -------
-    pgrid : 4 by 5 numpy array
-        pressure in hPa
+    dt : numpy array of datetime objects
+
+    """
 
-    Tgrid : 4 by 5 numpy array 
-        temperature in C
+    dt = Time(mjd,format='mjd').utc.datetime; 
 
-    Qgrid : 4 by 5 numpy array 
+    return dt
 
-    dTgrid : 4 by 5 numpy array  
-       temperature lapse rate in degrees per km 
-
-    u : 4 by 1 numpy array
-        geoid undulation in meters
-
-    Hs : 4 by 1 numpy array  
-
-    ahgrid : 4 by 5 numpy array
-        hydrostatic mapping function coefficient at zero height (VMF1) 
-
-    awgrid : 4 by 5 numpy array
-        wet mapping function coefficient (VMF1) 
-
-    lagrid : 4 by 5 numpy array
-
-    Tmgrid : 4 by 5 numpy array
-        mean temperature of the water vapor in degrees Kelvin 
-
-    requires that an environment variable exists for REFL_CODE
-    """
-#
-    xdir = str(os.environ['REFL_CODE'])
-    inputpath = xdir + '/input/'
-#    if not os.path.isdir(inputpath): #if year folder doesn't exist, make it
-#        os.makedirs(inputpath)
-
-    # input file should be written here
-    obsfile = inputpath + station + '_refr.txt'
-    #print('reading from station refraction file: ', obsfile)
-    x = np.genfromtxt(obsfile,comments='%')
-    max_ind = 4
-    pgrid = np.zeros((4,5))
-    Tgrid = np.zeros((4,5))
-    Qgrid = np.zeros((4,5))
-    dTgrid = np.zeros((4,5))
-    u = np.zeros((4,1))
-    Hs = np.zeros((4,1)) 
-    ahgrid = np.zeros((4,5))
-    awgrid = np.zeros((4,5))
-    lagrid = np.zeros((4,5))
-    Tmgrid = np.zeros((4,5))
-
-    for n in [0,1,2,3]:
-        ij = 0
-        u[n]= x[n*5,6]
-        Hs[n]= x[n*5,7]
-        for m in range(n*5, n*5+5):
-            pgrid[n,ij] = x[m,2] 
-            Tgrid[n,ij] = x[m,3] 
-            Qgrid[n,ij] = x[m,4]/1000
-            dTgrid[n,ij] = x[m,5]/1000
-            ahgrid[n,ij] = x[m,8]/1000
-            awgrid[n,ij] = x[m,9]/1000
-            lagrid[n,ij] = x[m,10] 
-            Tmgrid[n,ij] = x[m,11] 
-            ij +=1
-
-    return pgrid, Tgrid, Qgrid, dTgrid, u, Hs, ahgrid, awgrid, lagrid, Tmgrid
-#
-def gpt2_1w (station, dmjd,dlat,dlon,hell,it):
+
+def write_spline_output(iyear, th, spline, delta_out, station, txtdir,Hortho):
     """
+    Writing the output of the spline fit to the final RH time series.
+    No output other than this text file for year 2023 and station name ssss:
+
+    $REFL_CODE/Files/ssss/ssss_2023_spline_out.txt
+
+
+    I do not think this is used anymore. It has been consolidated with the plot code.
+
     Parameters
     ----------
+    iyear : int
+        full year
+    th : numpy array
+        time values of some kind ... maybe fractional day of years?
+    spline: fit, output of interpolate.BSpline
+        needs doc
+    delta_out : int
+        how often you want the splinefit water level written, in seconds
     station : str
         station name
-    dmjd:  float 
-        modified Julian date (scalar, only one epoch per call is possible)
-    dlat : float 
-        ellipsoidal latitude in radians [-pi/2:+pi/2] 
-    dlon : float
-        longitude in radians [-pi:pi] or [0:2pi] 
-    hell : float 
-        ellipsoidal height in m 
-    it: integer
-        case 1: no time variation but static quantities
+    txtdir : str
+        output directory
+    Hortho : float
+        orthometric height used to convert RH to something more sea level like
+        meters
+    """
 
-        case 0: with time variation (annual and semiannual terms)
+    if delta_out == 0:
+        print('No spline values will be written because the interval is set to zero.')
+    else:
+        firstpoint  = float(th[0]); lastpoint = float(th[-1])
+        s1 = math.floor(firstpoint) ; s2 = math.ceil(lastpoint)
+        ndays = s2-s1 # number of days
+        # how many values you want in the linspace world
+        numvals = 1 + int(ndays*86400/delta_out)
+        # this should be evenly defined fractional doy
+        tplot = np.linspace(s1, s2, numvals,endpoint=True)
+        # then fit it
+        spline_even = spline(tplot)
+        N = len(tplot)
+
+        # but you only want those values when we have data ....
+        splinefileout =  txtdir + '/' + station + '_' + str(iyear) + '_spline_out_orig.txt'
+        print('Writing evenly sampled file to: ', splinefileout)
+        vn = ' gnssrefl v' + str(g.version('gnssrefl'))
+        fout = open(splinefileout,'w+')
+        fout.write('{0:1s}  {1:30s}  \n'.format('%','station: ' + station + vn))
+        fout.write('{0:1s}  {1:30s}  \n'.format('%','This is NOT observational data - be careful when interpreting it.'))
+        fout.write('{0:1s}  {1:30s}  \n'.format('%','If the data are not well represented by the spline functions, you will '))
+        fout.write('{0:1s}  {1:30s}  \n'.format('%','have a very poor representation of the data. I am also writing out station '))
+        fout.write('{0:1s}  {1:30s}  {2:8.3f} \n'.format('%','orthometric height minus RH, where Hortho (m) is ', Hortho  ))
+        fout.write('{0:1s}  {1:30s}  \n'.format('%','This assumes RH is measured relative to the L1 phase center.  '))
+        fout.write('{0:1s}  {1:30s}  \n'.format('%','MJD             RH(m) YYYY MM DD  HH  MM  SS   quasi-sea-level(m)'))
+        fout.write('{0:1s}  {1:30s}  \n'.format('%','(1)              (2)  (3) (4) (5) (6) (7) (8)    (9)'))
+
+
+        dtime = False
+        for i in range(0,N):
+            modjul = g.fdoy2mjd(iyear,tplot[i])
+            doy = math.floor(tplot[i])
+            utc= 24*(tplot[i] - doy)
+            bigt,yy,mm,dd,hh,mi,ss = g.ymd_hhmmss(iyear,doy,utc,dtime)
+            if (tplot[i] >= firstpoint) & (tplot[i] <= lastpoint):
+                fout.write('{0:15.7f}  {1:10.3f} {2:4.0f} {3:3.0f} {4:3.0f} {5:3.0f} {6:3.0f} {7:3.0f} {8:10.3f} \n'.format(
+                    modjul, spline_even[i], yy,mm,dd,hh,mi,ss, Hortho-spline_even[i]))
+        fout.close()
 
-    Returns
-    -------
-    p : float
-        pressure in hPa
-    T:  float
-        temperature in degrees Celsius 
-    dT : float
-       temperature lapse rate in degrees per km 
-    Tm : float
-        mean temperature of the water vapor in degrees Kelvin 
-    e : float
-        water vapor pressure in hPa 
-    ah: float
-        hydrostatic mapping function coefficient at zero height (VMF1) 
-    aw: float
-        wet mapping function coefficient (VMF1) 
-    la: float
-        water vapor decrease factor 
-    undu: float
-        geoid undulation in m 
+def testing_nvals(Gval, Rval, Eval, Cval):
+    """
+    writing the number of observations per constellation as a test. not currently used
+
+    Parameters
+    Gval: numpy array
+        GPS RH values
+    Rval : numpy array
+        GLONASS RH values
+    Eval : numpy array
+        Galileo RH values
+    Cval : numpy
+        Beidou RH values
 
+    writes to a file - kristine.txt returns nothing
+
+    """
+    fouting = open('kristine.txt','w+')
+    for i in range(0,len(Gval)):
+        fouting.write(' {0:3.0f} {1:4.0f} {2:4.0f} {3:4.0f} {4:4.0f} \n'.format(i, Gval[i], Rval[i], Eval[i], Cval[i]))
+    fouting.close()
+
+    return
+
+
+def numsats_plot(station,tval,nval,Gval,Rval,Eval,Cval,txtdir,fs,hires_figs,year):
     """
+    makes the plot that summarizes the number of satellites in each
+    constellation per epoch
+
+    Parameters
+    ----------
+    station : str
+        name of the station
+    tval : numpy array
+        datetime objects?
+    nval : numpy array
+        number of total satellites at a given epoch
+    Gval : numpy array
+        number of galileo satellites at an epoch
+    Rval : numpy array
+        number of glonass satellites at an epoch
+    Eval : numpy array
+        number of galileo satellites at an epoch
+    Cval : numpy array
+        number of beidou satellites at an epoch
+    txtdir : str
+        where results are stored
+    fs : int
+        fontsize for the plots
+    hires_figs : bool
+        try to plot high resolution
+    year : int
+        calendar year
+
+    """
+
+    fig,ax=plt.subplots(figsize=(10,5))
+    ax.plot(tval,nval,'ko',label='Total',markersize=3)
+    if (np.sum(Gval) > 0):
+        ax.plot(tval,Gval,'bo',label='GPS',markersize=3)
+    if (np.sum(Rval) > 0):
+        ax.plot(tval,Rval,'ro',label='GLO',markersize=3)
+    if (np.sum(Eval) > 0):
+        ax.plot(tval,Eval,'o',color='orange',label='GAL',markersize=3)
+    if (np.sum(Cval) > 0):
+        ax.plot(tval,Cval,'co',label='BEI',markersize=3)
+
+    plt.legend(loc="best",fontsize=fs)
+    #ax.legend(loc='best')
+    plt.title(station + ': number of RH retrievals each day',fontsize=fs)
+    plt.xticks(rotation =45,fontsize=fs); plt.yticks(fontsize=fs)
+    plt.grid()
+
+    # was trying to do this, but life is short
+    #if hires_figs:
+#        https://stackoverflow.com/questions/4700614/how-to-put-the-legend-outside-the-plot
+    # Shrink current axis's height by 10% on the bottom
+        #box = ax.get_position()
+
+        #ax.set_position([box.x0, box.y0 + box.height * 0.1, box.width, box.height * 0.9])
+        #ax.legend(loc='upper center', bbox_to_anchor=(0.5, -0.05), fancybox=True, shadow=True, ncol=5)
+
+    # Put a legend below current axis
+        #ax.legend(loc='upper center', bbox_to_anchor=(0.5, -0.05), fancybox=True, shadow=True, ncol=4)
+        #ax.set_position([box.x0, box.y0 + box.height * 0.5, box.width, box.height ])
+        #ax.legend(loc='center left', bbox_to_anchor=(1, 0.3))
+
+
+    fig.autofmt_xdate()
+    plotname = txtdir + '/' + station + '_' + str(year) + '_Subnvals.png'
+    if hires_figs:
+        plotname = txtdir + '/' + station + '_' + str(year) +'_Subnvals.eps'
 
-#  need to find diffpod and difflon
-    if (dlon < 0):
-        plon = (dlon + 2*np.pi)*180/np.pi;
+    plt.savefig(plotname,dpi=300)
+    print('Plot file saved as: ', plotname)
+
+
+def rh_plots(otimes,tv,station,txtdir,year,d1,d2,percent99):
+    """
+    overview plots for rh_plot
+
+    Parameters
+    ----------
+    otimes : numpy array of datetime objects
+        observation times
+    tv : numpy array
+        gnssrefl results written into this variable using loadtxt
+    station : str
+        station name, only used for the title
+    txtdir : str
+        directory where the plots will be written to
+    year: int
+        what year is being analyzed
+    d1 : int
+        minimum day of year
+    d2 : int
+        maximum day of year
+    percent99 : bool
+        whether you want only the 1-99 percentile plotted
+
+    """
+    if d1 == 1 and d2 == 366:
+        # these are the defaults
+        setlimits = False
     else:
-        plon = dlon*180/np.pi;
-# transform to polar distance in degrees
-    ppod = (-dlat + np.pi/2)*180/np.pi; 
-
-#       % find the index (line in the grid file) of the nearest point
-#  	  % changed for the 1 degree grid (GP)
-    ipod = np.floor(ppod+1); 
-    ilon = np.floor(plon+1);
+        setlimits = True
+        yyy,mm,dd = g.ydoy2ymd(year, d1)
+        th1 = datetime.datetime(year=year, month=mm, day=dd)
+        yyy,mm,dd = g.ydoy2ymd(year, d2)
+        th2 = datetime.datetime(year=year, month=mm, day=dd)
+    # this is not working, so just setting it to false, cause who cares!
+    setlimits = False
+    fs = 10
+    fig,(ax2,ax3)=plt.subplots(2,1,sharex=True)
+        # put some azimuth information on it
+    colors = tv[:,5]
+        # ax.plot( otimes, tv[:,2], '.')
+        # https://matplotlib.org/stable/gallery/lines_bars_and_markers/scatter_with_legend.html
+    # help from felipe nievinski
+    #tmp = numpy.percentile(tv[:,2], [1 99])
+    #matplotlib.pyplot.ylim(tmp[1], tmp[2])
+
+    scatter = ax2.scatter(otimes,tv[:,2],marker='o', s=10, c=colors)
+    colorbar = fig.colorbar(scatter, ax=ax2)
+    colorbar.set_label('deg', fontsize=fs)
+    ax2.set_ylabel('meters',fontsize=fs)
+    ax2.set_title('Azimuth',fontsize=fs)
+    #ax1.title.set_text('Azimuth')
+    plt.xticks(rotation =45,fontsize=fs); plt.yticks(fontsize=fs)
+    fig.suptitle( station.upper() + ' Reflector Heights', fontsize=fs)
+
+    if setlimits:
+        ax2.set_xlim((th1, th2))
+
+    # now doing 1 and 99%
+    p1 = 0.01; p2 = 0.99
+    #lowv, highv = my_percentile(tv[:,2],p1, p2)
+    # this crashed my docker build - but it turned out to have nothing to do with it
+    yl = np.percentile(tv[:,2] ,[1 ,99])
+    print('percentile values',yl)
+    # I think this is a typo?
+    #lowv = yl[0]; highv = y[1]
+    lowv = yl[0]; highv = yl[1]
     
-#   normalized (to one) differences, can be positive or negative
-#	% changed for the 1 degree grid (GP)
-    diffpod = (ppod - (ipod - 0.5));
-    difflon = (plon - (ilon - 0.5));
-
-
-# change the reference epoch to January 1 2000
-    #print('Modified Julian Day', dmjd)
-    dmjd1 = dmjd-51544.5 
-
-    pi2 = 2*np.pi
-    pi4 = 4*np.pi
-
-# mean gravity in m/s**2
-    gm = 9.80665;
-# molar mass of dry air in kg/mol
-    dMtr = 28.965E-3 
-#    dMtr = 28.965*10^-3 
-# universal gas constant in J/K/mol
-    Rg = 8.3143 
-
-# factors for amplitudes, i.e. whether you want time varying
-    if (it==1):
-        #print('>>>> no refraction time variation ')
-        cosfy = 0; coshy = 0; sinfy = 0; sinhy = 0;
-    else: 
-        cosfy = np.cos(pi2*dmjd1/365.25)
-        coshy = np.cos(pi4*dmjd1/365.25) 
-        sinfy = np.sin(pi2*dmjd1/365.25) 
-        sinhy = np.sin(pi4*dmjd1/365.25) 
-    cossin = np.matrix([1, cosfy, sinfy, coshy, sinhy])
-# initialization of new vectors
-    p =  0; T =  0; dT = 0; Tm = 0; e =  0; ah = 0; aw = 0; la = 0; undu = 0;
-    undul = np.zeros(4)
-    Ql = np.zeros(4)
-    dTl = np.zeros(4)
-    Tl = np.zeros(4)
-    pl = np.zeros(4)
-    ahl = np.zeros(4)
-    awl = np.zeros(4)
-    lal = np.zeros(4)
-    Tml = np.zeros(4)
-    el = np.zeros(4)
-#
-    pgrid, Tgrid, Qgrid, dTgrid, u, Hs, ahgrid, awgrid, lagrid, Tmgrid = read_4by5(station,dlat,dlon,hell)
-#
-    for l in [0,1,2,3]:
-        KL = l   #silly to have this as a variable like this 
-#  transforming ellipsoidal height to orthometric height:
-#  Hortho = -N + Hell
-        undul[l] = u[KL] 
-        hgt = hell-undul[l] 
-#  pressure, temperature at the height of the grid
-        T0 = Tgrid[KL,0] + Tgrid[KL,1]*cosfy + Tgrid[KL,2]*sinfy + Tgrid[KL,3]*coshy + Tgrid[KL,4]*sinhy;
-        tg = float(Tgrid[KL,:] *cossin.T)
-#     print(T0,tg)
-
-        p0 = pgrid[KL,0] + pgrid[KL,1]*cosfy + pgrid[KL,2]*sinfy + pgrid[KL,3]*coshy + pgrid[KL,4]*sinhy;
- 
-#       humidity 
-        Ql[l] = Qgrid[KL,0] + Qgrid[KL,1]*cosfy + Qgrid[KL,2]*sinfy + Qgrid[KL,3]*coshy + Qgrid[KL,4]*sinhy;
- 
-# reduction = stationheight - gridheight
-        Hs1 = Hs[KL]
-        redh = hgt - Hs1;
-
-# lapse rate of the temperature in degree / m
-        dTl[l] = dTgrid[KL,0] + dTgrid[KL,1]*cosfy + dTgrid[KL,2]*sinfy + dTgrid[KL,3]*coshy + dTgrid[KL,4]*sinhy;
-   
-# temperature reduction to station height
-        Tl[l] = T0 + dTl[l]*redh - 273.15;
-
-#  virtual temperature
-        Tv = T0*(1+0.6077*Ql[l])   
-        c = gm*dMtr/(Rg*Tv) 
-        
-# pressure in hPa
-        pl[l] = (p0*np.exp(-c*redh))/100 
-            
-#  hydrostatic coefficient ah
-        ahl[l] = ahgrid[KL,0] + ahgrid[KL,1]*cosfy + ahgrid[KL,2]*sinfy + ahgrid[KL,3]*coshy + ahgrid[KL,4]*sinhy;
-            
-# wet coefficient aw
-        awl[l] = awgrid[KL,0] + awgrid[KL,1]*cosfy + awgrid[KL,2]*sinfy + awgrid[KL,3]*coshy + awgrid[KL,4]*sinhy;
-					 
-# water vapor decrease factor la - added by GP
-        lal[l] = lagrid[KL,0] + lagrid[KL,1]*cosfy + lagrid[KL,2]*sinfy + lagrid[KL,3]*coshy + lagrid[KL,4]*sinhy;
-					 
-# mean temperature of the water vapor Tm - added by GP
-        Tml[l] = Tmgrid[KL,0] +  Tmgrid[KL,1]*cosfy + Tmgrid[KL,2]*sinfy + Tmgrid[KL,3]*coshy + Tmgrid[KL,4]*sinhy;
-					 		 
-# water vapor pressure in hPa - changed by GP
-        e0 = Ql[l]*p0/(0.622+0.378*Ql[l])/100; # % on the grid
-        aa = (100*pl[l]/p0)
-        bb = lal[l]+1
-        el[l] = e0*np.power(aa,bb)  # % on the station height - (14) Askne and Nordius, 1987
-           
-    dnpod1 = np.abs(diffpod); # % distance nearer point
-    dnpod2 = 1 - dnpod1;   # % distance to distant point
-    dnlon1 = np.abs(difflon);
-    dnlon2 = 1 - dnlon1;
-        
-#   pressure
-    R1 = dnpod2*pl[0]+dnpod1*pl[1];
-    R2 = dnpod2*pl[2]+dnpod1*pl[3];
-    p = dnlon2*R1+dnlon1*R2;
-            
-#   temperature
-    R1 = dnpod2*Tl[0]+dnpod1*Tl[1];
-    R2 = dnpod2*Tl[2]+dnpod1*Tl[3];
-    T = dnlon2*R1+dnlon1*R2;
-        
-#   temperature in degree per km
-    R1 = dnpod2*dTl[0]+dnpod1*dTl[1];
-    R2 = dnpod2*dTl[2]+dnpod1*dTl[3];
-    dT = (dnlon2*R1+dnlon1*R2)*1000;
-            
-#   water vapor pressure in hPa - changed by GP
-    R1 = dnpod2*el[0]+dnpod1*el[1];
-    R2 = dnpod2*el[2]+dnpod1*el[3];
-    e = dnlon2*R1+dnlon1*R2;
-            
-#   hydrostatic
-    R1 = dnpod2*ahl[0]+dnpod1*ahl[1];
-    R2 = dnpod2*ahl[2]+dnpod1*ahl[3];
-    ah = dnlon2*R1+dnlon1*R2;
-           
-#   wet
-    R1 = dnpod2*awl[0]+dnpod1*awl[1];
-    R2 = dnpod2*awl[2]+dnpod1*awl[3];
-    aw = dnlon2*R1+dnlon1*R2;
-        
-#  undulation
-    R1 = dnpod2*undul[0]+dnpod1*undul[1];
-    R2 = dnpod2*undul[2]+dnpod1*undul[3];
-    undu = dnlon2*R1+dnlon1*R2;
-
-#   water vapor decrease factor la - added by GP
-    R1 = dnpod2*lal[0]+dnpod1*lal[1];
-    R2 = dnpod2*lal[2]+dnpod1*lal[3];
-    la = dnlon2*R1+dnlon1*R2;
-		
-#   mean temperature of the water vapor Tm - added by GP
-    R1 = dnpod2*Tml[0]+dnpod1*Tml[1];
-    R2 = dnpod2*Tml[2]+dnpod1*Tml[3];
-    Tm = dnlon2*R1+dnlon1*R2; 
+    if percent99:
+        ax2.set_ylim((lowv,highv))
+
+    ax2.invert_yaxis()
+    ax2.grid(True)
 
-    return p, T, dT,Tm,e,ah,aw,la,undu
+    fig.autofmt_xdate()
 
-def readWrite_gpt2_1w(xdir, station, site_lat, site_lon):
+#    put some amplitude information on it
+    # https://matplotlib.org/stable/gallery/lines_bars_and_markers/scatter_with_legend.html
+    colors = tv[:,6]
+
+    scatter = ax3.scatter(otimes,tv[:,2],marker='o', s=10, c=colors)
+    colorbar = fig.colorbar(scatter, ax=ax3)
+    ax3.set_ylabel('meters',fontsize=fs)
+    colorbar.set_label('v/v', fontsize=fs)
+    plt.xticks(rotation =45,fontsize=fs); plt.yticks(fontsize=fs)
+    ax3.set_title('Amplitude',fontsize=fs)
+    ax3.grid(True)
+    if setlimits:
+        ax3.set_xlim((th1, th2))
+
+    if percent99:
+        ax3.set_ylim((lowv, highv ))
+    ax3.invert_yaxis()
+    fig.autofmt_xdate()
+
+    if percent99:
+        plotname = txtdir + '/' + station + '_rh2_99.png'
+    else:
+        plotname = txtdir + '/' + station + '_rh2.png'
+
+
+    print('png file saved as: ', plotname)
+    plt.savefig(plotname,dpi=300)
+
+
+def two_stacked_plots(otimes,tv,station,txtdir,year,d1,d2,hires_figs):
     """
-    makes a grid for refraction correction
+    This actually makes three stacked plots - not two, LOL
+    It gives an overview for quality control
 
     Parameters
     ----------
-    xdir : str
-        directory for output
+    otimes : numpy array of datetime objects
+        observations times
+    tv : numpy array
+        gnssrefl results written into this variable using loadtxt
     station : str
-        station name, 4 ch
-    lat : float
-        latitude in degrees
-    lon : float 
-        longitude in degrees 
-
-    """
-    PROJECT_ROOT = os.path.dirname(os.path.abspath(__file__))
-    BASE_DIR = os.path.dirname(PROJECT_ROOT)
-    try3 = PROJECT_ROOT + '/' + 'gpt_1wA.pickle'
-
-    # check that output path exists.  
-    outpath = xdir + '/input/'
-    if not os.path.isdir(outpath): 
-        os.makedirs(outpath)
-
-    outfile = outpath + station + '_refr.txt'
-    if os.path.isfile(outfile):
-        okokok = 1
-        #print('refraction file for this station already exists')
+        station name, only used for the title
+    txtdir : str
+        where the plots will be written to
+    year: int
+        what year is being analyzed
+    d1 : int
+        minimum day of year
+    d2 : int
+        maximum day of year
+    hires_figs : bool
+        true for eps instead of png
+
+    """
+    if d1 == 1 and d2 == 366:
+        # these are the defaults
+        setlimits = False
     else:
-        print('A station specific refraction output file will be written to ', outfile)
+        setlimits = True
+        yyy,mm,dd = g.ydoy2ymd(year, d1)
+        th1 = datetime.datetime(year=year, month=mm, day=dd)
+        yyy,mm,dd = g.ydoy2ymd(year, d2)
+        th2 = datetime.datetime(year=year, month=mm, day=dd)
+    # this is not working, so just setting it to false, cause who cares!
+    setlimits = False
+    fs = 12
+    fig,(ax1,ax2,ax3)=plt.subplots(3,1,sharex=True,figsize=(10,8))
+    #fig,(ax1,ax2,ax3)=plt.subplots(3,1,sharex=True)
+    i = (tv[:,10] < 100)
+    colors = tv[:,10]
+    scatter = ax1.scatter(otimes,tv[:,2],marker='o', s=10, c=colors)
+    colorbar = fig.colorbar(scatter, ax=ax1)
+    colorbar.set_label('Frequency', fontsize=fs)
+    ax1.set_title('Signals',fontsize=fs)
+    plt.xticks(rotation =45,fontsize=fs); 
+    ax1.set_ylabel('RH (m)',fontsize=fs)
+    plt.yticks(fontsize=fs)
+    ax1.invert_yaxis()
+    ax1.grid(True)
+    #fig.suptitle( station.upper() + ' Reflector Heights', fontsize=fs)
+    if setlimits:
+        ax1.set_xlim((th1, th2))
+    fig.autofmt_xdate()
+
+    #fig,(ax1,ax2)=plt.subplots(2,1,sharex=True)
+        # put some azimuth information on it
+    colors = tv[:,5]
+        # ax.plot( otimes, tv[:,2], '.')
+        # https://matplotlib.org/stable/gallery/lines_bars_and_markers/scatter_with_legend.html
+    scatter = ax2.scatter(otimes,tv[:,2],marker='o', s=10, c=colors)
+    colorbar = fig.colorbar(scatter, ax=ax2)
+    colorbar.set_label('deg', fontsize=fs)
+    ax2.set_ylabel('RH (m)',fontsize=fs)
+    ax2.set_title('Azimuth',fontsize=fs)
+    #ax1.title.set_text('Azimuth')
+    plt.xticks(rotation =45,fontsize=fs); plt.yticks(fontsize=fs)
+    ax2.invert_yaxis()
+    ax2.grid(True)
+    if setlimits:
+        ax2.set_xlim((th1, th2))
+    fig.autofmt_xdate()
+
+# put some amplitude information on it
+    colors = tv[:,6]
+    # ax.plot( otimes, tv[:,2], '.')
+    # https://matplotlib.org/stable/gallery/lines_bars_and_markers/scatter_with_legend.html
+    scatter = ax3.scatter(otimes,tv[:,2],marker='o', s=10, c=colors)
+    colorbar = fig.colorbar(scatter, ax=ax3)
+    ax3.set_ylabel('RH (m)',fontsize=fs)
+    colorbar.set_label('v/v', fontsize=fs)
+    plt.xticks(rotation =45,fontsize=fs); plt.yticks(fontsize=fs)
+    ax3.set_title('Amplitude',fontsize=fs)
+    ax3.invert_yaxis()
+    ax3.grid(True)
+    if setlimits:
+        ax3.set_xlim((th1, th2))
+    fig.autofmt_xdate()
+
+    plotname = txtdir + '/' + station + '_' + str(year) + '_combined.png'
+    if hires_figs:
+        plotname = txtdir + '/' + station + '_' + str(year) + '_combined.eps'
+        plt.savefig(plotname,dpi=300)
+    else:
+        plt.savefig(plotname,dpi=300)
+    print('Plot file saved as: ', plotname)
 
-#   change to radians
-        dlat = site_lat*np.pi/180 
-        dlon = site_lon*np.pi/180 
-
-#   read VMF gridfile in pickle format 
-        pname = xdir + '/input/' + 'gpt_1wA.pickle'
-        foundit, pname = look_for_pickle_file() 
-        if foundit:
-            f = open(pname, 'rb')
-            [All_pgrid, All_Tgrid, All_Qgrid, All_dTgrid, All_U, All_Hs, All_ahgrid, All_awgrid, All_lagrid, All_Tmgrid] = pickle.load(f)
-            f.close()
-        else:
-            print('You will need to download gpt_1wA.pickle MANUALLY from github and store it in REFL_CODE/input')
-            sys.exit()
-
-# really should e zero to four, but whatever
-        indx = np.zeros(4,dtype=int)
-        indx_lat = np.zeros(4,dtype=int)
-        indx_lon = np.zeros(4,dtype=int)
-
-
-#figure out grid index
-# % only positive longitude in degrees
-        if (dlon < 0):
-            plon = (dlon + 2*np.pi)*180/np.pi;
-        else:
-            plon = dlon*180/np.pi 
-#
-#  transform to polar distance in degrees
-        ppod = (-dlat + np.pi/2)*180/np.pi  
-
-#% find the index (line in the grid file) of the nearest point
-# % changed for the 1 degree grid (GP)
-        ipod = np.floor(ppod+1)  
-        ilon = np.floor(plon+1) 
-    
-#    % normalized (to one) differences, can be positive or negative
-# % changed for the 1 degree grid (GP)
-        diffpod = (ppod - (ipod - 0.5)) 
-        difflon = (plon - (ilon - 0.5)) 
-#    % added by HCY
-# % changed for the 1 degree grid (GP)
-        if (ipod == 181):
-            ipod = 180 
-        if (ilon == 361):
-            ilon = 1 
-        if (ilon == 0):
-            ilon = 360
-
-#     get the number of the corresponding line
-#	 changed for the 1 degree grid (GP)
-        indx[0] = (ipod - 1)*360 + ilon 
-#  save the lat lon of the grid points
-        indx_lat[0] = 90-ipod+1  
-        indx_lon[0] = ilon-1   
-# % near the poles: nearest neighbour interpolation, otherwise: bilinear
-# % with the 1 degree grid the limits are lower and upper (GP)
-
-        bilinear = 0 
-        max_ind = 1 
-        if (ppod > 0.5) and (ppod < 179.5):
-            bilinear = 1           
-        if (bilinear == 1):
-            max_ind =4 
-
-#    % bilinear interpolation
-#    % get the other indexes 
- 
-        ipod1 = ipod + np.sign(diffpod) 
-        ilon1 = ilon + np.sign(difflon) 
-# % changed for the 1 degree grid (GP)
-        if (ilon1 == 361):
-            ilon1 = 1 
-        if (ilon1 == 0):
-            ilon1 = 360 
-#         get the number of the line
-# changed for the 1 degree grid (GP)
-# four indices ???
-        indx[1] = (ipod1 - 1)*360 + ilon; # % along same longitude
-        indx[2] = (ipod  - 1)*360 + ilon1;# % along same polar distance
-        indx[3] = (ipod1 - 1)*360 + ilon1;# % diagonal
-#
-# save the lat lon of the grid points  lat between [-90 ;90]  lon [0 360] 
-        indx_lat[1] =   90 - ipod1+np.sign(diffpod)     
-        indx_lon[1] = ilon-1 
-        indx_lat[2] =   90-ipod +1
-        indx_lon[2] =  ilon1 - np.sign(difflon) 
-        indx_lat[3] =   90 -ipod1+np.sign(diffpod)     
-        indx_lon[3] = ilon1- np.sign(difflon);
-
-# extract the new grid
-# will need to do 0-4 instead of 1-5 because stored that way in python
-# which values to use in the bigger array
-# assign the correct values
-        indx = indx - 1
-        indx_list = indx.tolist()
-#    print(indx_list)
-#    print(indx)
-#print(np.shape(indx_lat))
-#print(np.shape(indx_lon))
-        w = 0
-# need to write values for a given station to a plain text file
-#
-        fout = open(outfile, 'w+')
-        for a in indx_list:
-            for k in [0,1,2,3,4]:
-                fout.write(" {0:4.0f} {1:5.0f} {2:13.4f} {3:10.4f} {4:10.6f} {5:10.4f} {6:12.5f} {7:12.5f} {8:10.6f} {9:10.6f} {10:10.6f} {11:10.4f} \n".format( indx_lat[w], indx_lon[w],All_pgrid[a,k],All_Tgrid[a,k],All_Qgrid[a,k]*1000,All_dTgrid[a,k]*1000,All_U[a,0],All_Hs[a,0], All_ahgrid[a,k]*1000, All_awgrid[a,k]*1000, All_lagrid[a,k], All_Tmgrid[a,k] ))
+def stack_two_more(otimes,tv,ii,jj,stats, station, txtdir, sigma,kplt,hires_figs,year):
+    """
+    makes a plot of the reflector heights before and after minimal editing
+
+    Parameters
+    ----------
+    otimes : numpy array of datetime objects 
+        observation times
+    tv : numpy array
+        variable with the gnssrefl LSP results
+    ii : numpy array
+        indices of good data
+    jj : numpy array
+        indices of bad data
+    station : str
+        station name
+    txtdir : str
+        directory where plots will be written
+    sigma : float
+        what kind of standard deviation is used for outliers (3sigma, 2.5 sigma etc)
+    kplt : bool
+        make extra plot for kristine
+    year : int 
+        calendar year
+    """
+    fs = 10
+    otimesarray = np.asarray(otimes)
+    # new plot 
+    plt.figure(figsize=(10,5))
+    plt.plot(tv[:,5],tv[:,2], '.',markersize=4,label='obs')
+    plt.plot(tv[ii,5],tv[ii,2], 'ro',markersize=4,label='outliers')
+    plt.xlabel('Azimuth (degrees)')
+    plt.ylabel('Reflector Height (m)')
+    plt.title('Quick Plot of RH with respect to Azimuth')
+    plt.gca().invert_yaxis()
+    plt.legend(loc="best")
+    plt.grid()
+    plotname_stem = txtdir + '/' + station + '_' + str(year) + '_outliers_wrt_az'
+    if hires_figs:
+        plotname = plotname_stem + '.eps'
+    else:
+        plotname = plotname_stem + '.png'
+
+    plt.savefig(plotname,dpi=300)
+    print('Plot file saved as: ', plotname)
 
-            w+=1
+    #    fig=plt.figure(figsize=(10,6))
+    fig = plt.figure(figsize=(10,6))
+    colors = tv[:,5]
+# put some amplitude information on it
+# ax.plot( otimes, tv[:,2], '.')
+# https://matplotlib.org/stable/gallery/lines_bars_and_markers/scatter_with_legend.html
+
+
+    ax1 = fig.add_subplot(211)
+    plt.plot(otimes,tv[:,2], '.',color='gray',label='arcs')
+    plt.plot(stats[:,0], stats[:,1], '.',markersize=4,color='blue',label='daily avg')
+    slabel = str(sigma) + ' sigma'
+    plt.plot(stats[:,0], stats[:,1]-sigma*stats[:,2], '--',color='black',label=slabel)
+    plt.plot(stats[:,0], stats[:,1]+sigma*stats[:,2], '--',color='black')
+    plt.plot(otimesarray[ii],tv[ii,2], 'r.',markersize=4,label='outliers')
+    #plt.plot(otimesarray[ii],tv[ii,2], '.',color='red',label='outliers',markersize=12)
+    plt.legend(loc="best",bbox_to_anchor=(0.95, 0.9),prop={"size":fs-2})
+    plt.title('Raw ' + station.upper() + ' Reflector Heights', fontsize=fs)
+    plt.ylabel('meters',fontsize=fs)
+    plt.gca().invert_yaxis()
+    plt.xticks(rotation =45,fontsize=fs); plt.yticks(fontsize=fs)
+    plt.grid() ; fig.autofmt_xdate()
+    # get the limits so you can use thme on the next plot
+    #aaa, bbb = plt.ylim()
+    savey1,savey2 = plt.ylim()  
+
+    ax2 = fig.add_subplot(212)
+    plt.plot(otimesarray[jj],tv[jj,2], '.',color='green',label='arcs')
+    plt.gca().invert_yaxis()
+    plt.ylabel('meters',fontsize=fs)
+    plt.xticks(rotation =45,fontsize=fs); plt.yticks(fontsize=fs)
+    plt.title('Edited ' + station.upper() + ' Reflector Heights', fontsize=fs)
+
+    plt.grid() ; fig.autofmt_xdate()
+    plotstem = txtdir + '/' + station + '_' + str(year) + '_outliers'
+    if hires_figs:
+        plotname = plotstem + '.eps'
+        plt.savefig(plotname,dpi=300)
+    else:
+        plotname = plotstem + '.png'
+        plt.savefig(plotname,dpi=300)
+
+    plt.ylim((savey1, savey2))
+    print('Plot file saved as: ', plotname)
+    if kplt:
+        fig = plt.figure()
+        ax1 = fig.add_subplot(211)
+        ddd = - (tv[jj,2] - np.max(tv[jj,2]))
+        plt.plot(otimesarray[jj],ddd, '.',color='blue')
+        plt.title('Relative Sea Level Measured with Reflected GNSS Signals:' + station.upper(), fontsize=fs)
+        plt.ylabel('meters',fontsize=fs)
+        plt.xticks(rotation =45,fontsize=fs-1); plt.yticks(fontsize=fs-1)
+        plt.ylim((-0.1, 1.1*np.max(ddd)))
+        plt.suptitle(f"St Michael, Alaska ", size=12)
+        plt.grid()
+
+def writeout_spline_outliers(tvd_bad,txtdir,residual,filename):
+    """
+
+    Write splinefit outliers to a text file. 
+
+    Parameters
+    ----------
+    tvd_bad : numpy array
+        output of the lomb scargle calculations
+    txtdir : str
+        directory for the output, i.e. $REFL_CODE/FiLes/station
+    residual : numpy array
+        RH outliers in units of meters (!)
+    filename : str
+        name of file being written
+
+    """
+    nr,nc=tvd_bad.shape
+    if nr > 0:
+        f = txtdir + '/' + filename
+        print(nr, ' Outliers written to: ', f)
+        fout = open(f, 'w+')
+        # put in a header
+        fout.write('{0:3s} sat azim deltT-min outlier-m fracDOY MJD  OrigRH meanE PkNoise \n'.format('%'))
+        fout.write('{0:3s} (1) (2)   (3)        (4)      (5)    (6)   (7)    (8)   (9)\n'.format('%'))
+        for w in range(0,nr):
+            fy = tvd_bad[w,1] + tvd_bad[w,4]/24 # fractional day of year
+            deltaT = tvd_bad[w,14]
+            mjd = tvd_bad[w,15]
+            # average elevation angle
+            elAv = 0.5*(tvd_bad[w,8] + tvd_bad[w,7])
+            fout.write('{0:3.0f} {1:7.2f} {2:7.2f} {3:7.2f} {4:9.3f} {5:15.7f} {6:7.2f} {7:7.2f} {8:5.2f}\n'.format( 
+                tvd_bad[w,3], tvd_bad[w,5], deltaT,residual[w],fy,mjd,tvd_bad[w,2],elAv,tvd_bad[w,13]))
         fout.close()
-        print('station specific refraction file written')
 
+    return
 
-def corr_el_angles(el_deg, press, temp):
+def print_badpoints(t,outliersize,txtdir,real_residuals):
     """
-    Corrects elevation angles for refraction using simple angle bending model
+    prints outliers to a file.
 
     Parameters
     ----------
-    el_deg : numpy array of floats
-        elevation angles in degrees
-    press : float
-        pressure in hPa
-    temp : float
-        temperature in degrees C
+    t : numpy array
+        lomb scargle result array of "bad points". Format given below
+    outliersize : float
+        outlier criterion, in meters
+    txtdir : str
+        directory where file is written
+    real_residuals : numpy array of floats
+        assume this is RH residuals in meters
 
     Returns
     -------
-    corr_el_deg : numpy array of floats
-        corrected elevation angles (in degrees)
+    writes to a file called outliers.txt in the Files/station area
 
     """
+# format of t 
 
-#  Formula in python from Strandberg, originally from Astronomy journal
-    corr_el_arc_min = 510/(9/5*temp + 492) * press/1010.16 * 1/np.tan(np.deg2rad(el_deg + 7.31/(el_deg + 4.4)))
-    correction = corr_el_arc_min/60 
-     
-    corr_el_deg = el_deg + correction   
-    return corr_el_deg
-
+# (1)  (2)   (3) (4)  (5)     (6)   (7)    (8)    (9)   (10)  (11) (12) (13)    (14)     (15)    (16) (17) (18,19,20,21,22)
+# year, doy, RH, sat,UTCtime, Azim, Amp,  eminO, emaxO,NumbOf,freq,rise,EdotF, PkNoise  DelT     MJD  refr  MM DD HH MM SS
+# (0)  (1)   (2) (3)  (4)     (5)   6 )    (7)    (8)   (9)  (10) (11) (12)    (13)     (14)    (15)  (16) ... 
+
+    m,n = t.shape
+    f = txtdir + '/outliers.txt'
+    if (m > 0):
+        print(m, ' Outliers written to file: ', f)        
+        fout = open(f, 'w+')
+        for i in range(0,m):
+            fout.write('doy {0:3.0f} sat {1:3.0f} azim {2:6.2f} fr {3:3.0f} pk2noise {4:5.1f} residual {5:5.2f} \n'.format( 
+                t[i,1], t[i,3],t[i,5], t[i,10], t[i,13], real_residuals[i] ))
+        fout.close()
+    else:
+        print('no outlier points to write to a file')
 
-def look_for_pickle_file():
+def writejsonfile(ntv,station, outfile):
     """
-    latest attempt to solve the dilemma of the pickle file needed for
-    the refraction correction
+    subdaily RH values written out in json format
 
-    Returns
-    -------
-    foundit : bool
-        whether pickle file found
-    fullpname : str
-        full path to the pickle file
-    """
-#   read VMF gridfile in pickle format
-
-    pfile = 'gpt_1wA.pickle'
-
-    # at one point i thought this was useful
-    PROJECT_ROOT = os.path.dirname(os.path.abspath(__file__))
-    BASE_DIR = os.path.dirname(PROJECT_ROOT)
-    try3 = PROJECT_ROOT + '/' + pfile
-    # do i need str??
-    xdir = str(os.environ['REFL_CODE'])
-    inputdir = xdir + '/input/'
-    if os.path.isdir(inputdir):
-        print('found ', inputdir)
-    else:
-        print('make directory: ', inputdir)
-        subprocess.call(['mkdir',inputdir])
+    This does not appear to be used
 
-    fdir = xdir + '/Files'
-    if not os.path.isdir(fdir):
-        print('make Files directory: ', fdir)
-        subprocess.call(['mkdir', fdir])
-
-    # where the file should be stored
-    fullpname = inputdir + pfile
-
-    print('The large refraction file should be stored here:', fullpname)
-    foundit = False
-
-    if os.path.isfile(fullpname):
-        print('1st attempt: found in ', fullpname)
-        foundit = True
-    else:
-        print('1st attempt: not found in ', fullpname)
+    Parameters
+    -----------
+    ntv : numpy of floats
+        LSP results
 
-    if not foundit:
-        pname =  'gnssrefl/gpt_1wA.pickle'
-        print('2nd attempt: look in subdirectory of current working directory:', pname)
-        if os.path.isfile(pname):
-            subprocess.call(['cp','-f',pname, fullpname  ])
-            foundit = True
-
-    if not foundit:
-        pname = try3
-        print('3rd attempt try looking here: ',pname)
-        if os.path.isfile(pname):
-            foundit = True
-            print('cp it to ', fullpname)
-            subprocess.call(['cp','-f',pname, fullpname])
-        else:
-            print('that did not work')
-
-    url= 'https://github.com/kristinemlarson/gnssrefl/raw/master/gnssrefl/' + pfile
-    if not foundit:
-        print('4th attempt - download from github', url)
-        try:
-            wget.download(url,fullpname)
-        except:
-            print('download or cp failed')
-        if os.path.isfile(fullpname):
-            foundit = True
-
-    if not foundit:
-        url= 'https://morefunwithgps.com/public_html/' + pfile
-        print('5th attempt - ',url)
-        try:
-            wget.download(url,fullpname)
-        except:
-            print('Failed again.')
-
-        if os.path.isfile(fullpname):
-            foundit = True
-        else:
-            print('File should be stored in ', inputdir, ' but is not')
-
-    return foundit , fullpname
+    station : str
+        4 ch station name
 
+    outfile : str
+        filename for output
 
-def Ulich_Bending_Angle(ele, N0,lsp,p,T,ttime,sat):   #UBA
     """
-    Ulich, B. L. "Millimeter wave radio telescopes: Gain and pointing characteristics." (1981)
+    print('You picked the json output')
+    # dictionary
+    #o = {}
+    N= len(ntv)
+
+    # year is in first column
+    year  =  ntv[:,0].tolist()
+    year =[str(int(year[i])) for i in range(N)];
+
+    # day of year
+    doy =  ntv[:,1].tolist()
+    doy=[str(int(doy[i])) for i in range(N)];
+
+    # UTC hour
+    UTChour = ntv[:,4].tolist()
+    UTChour = [str(UTChour[i]) for i in range(N)];
+
+    # converted to ???
+    timestamp = [quickTr(ntv[i,0], ntv[i,1], ntv[i,4]) for i in range(N)]
+
+    # reflector height (meters)
+    rh = ntv[:,2].tolist()
+    rh=[str(rh[i]) for i in range(N)];
+
+    # satellite number
+    sat  = ntv[:,3].tolist()
+    sat =[int(sat[i]) for i in range(N)];
+
+    # frequency
+    freq  = ntv[:,8].tolist()
+    freq =[int(freq[i]) for i in range(N)];
+
+    # amplitude of main periodogram (LSP)
+    ampl  = ntv[:,6].tolist()
+    ampl =[str(ampl[i]) for i in range(N)];
+
+    # azimuth in degrees
+    azim  = ntv[:,5].tolist()
+    azim =[str(azim[i]) for i in range(N)];
+
+    # edotF in units ??
+    edotf  = ntv[:,9].tolist()
+    edotf =[str(edotf[i]) for i in range(N)];
+
+    # modified julian day
+    #mjd = ntv[:,15].tolist()
+    mjd = ntv[:,14].tolist()
+    mjd=[str(mjd[i]) for i in range(N)];
+
+    #column_names = ['timestamp','rh','sat','freq','ampl','azim','edotf','mjd']
+    # now attempt to zip them
+    l = zip(timestamp,rh,sat,freq,ampl,azim,edotf,mjd)
+    dzip = [dict(zip(column_names, next(l))) for i in range(N)]
+    # make a dictionary with metadata and data
+    o={}
+    # not setting lat and lon for now
+    lat = "0"; lon = "0";
+    firstline = {'name': station, 'latitude': lat, 'longitude': lon}
+    o['metadata'] = firstline
+    o['data'] = dzip
+    outf = outfile
+    with open(outf,'w+') as outf:
+        json.dump(o,outf,indent=4)
 
-    Author: 20220629, fengpeng
-    modified to use numpy so I can do arrays
+    return True
 
-    currently writes out corrections to a file for testing
+def rhdot_plots(th,correction,rhdot_at_th, tvel,yvel,fs,station,txtdir,hires_figs,year):
+    """
+    makes the rhdot correction plots
 
     Parameters
     ----------
-    ele : numpy array of floats
-        true elevation angle, degrees
+    th : numpy array
+        time of obs, day of year
+    correction : numpy array
+        rhcorrections in meters
+    rhdot_at_th : numpy array of floats
+        spline fit for rhdot in meters
+    tvel : numpy array of floats
+        time for surface velocity in days of year
+    yvel : numpy array of floats
+        surface velocity in m/hr
+    fs : integer
+        fontsize 
+    station : str
+        station name
+    txtdir : str
+        file directory for output
+    hires_figs : bool
+        whether you want eps instead of png 
+    year : int
+        calendar year
+
+    """
+    mjd0 = g.fdoy2mjd(year, th[0] ) # MJD of first point
+    # not being used
+    #th_obs = mjd_to_obstimes(th+mjd0)
+
+
+    fig=plt.figure(figsize=(10,6))
+    plt.subplot(2,1,1)
+    plt.plot(th, correction,'b.')
+    plt.ylabel('meters',fontsize=fs);
+    plt.xlim((np.min(th), np.max(th)))
+    plt.grid()
+    plt.title('The RH correction from RHdot effect ')
+    #plt.xlim((th_obs[0], th_obs[-1])) #fig.autofmt_xdate()
+
+    plt.subplot(2,1,2)
+    #mjd1 = g.fdoy2mjd(year, tvel[0] ) # MJD of first point
+    #tvel_obs = mjd_to_obstimes(tvel+mjd1)
+
+    # ???
+    A1 = np.min(th)  ; A2 = np.max(th) 
+    jj = (tvel >= A1) & (tvel <= A2)
+
+    plt.plot(th, rhdot_at_th,'b.',label='at GNSS obs')
+    # disaster - did not work
+    #plt.plot(tvel_obs, yvel,'c-', label='spline fit')
+    plt.plot(tvel[jj], yvel[jj],'c-', label='spline fit')
+    plt.legend(loc="upper left")
+    plt.grid()
+    plt.title('surface velocity')
+    plt.ylabel('meters/hour'); plt.xlabel('days of the year') 
+    plt.xlim((A1,A2))
+    #plt.xlim((th[0], th[-1])) #fig.autofmt_xdate()
+
+    if hires_figs:
+        g.save_plot(txtdir + '/' + station + '_rhdot3.eps')
+    else:
+        g.save_plot(txtdir + '/' + station + '_rhdot3.png')
 
-    N0 : float
-        antenna refractivity in ppm
+
+def find_ortho_height(station,extension):
+    """
+    Find orthometric (sea level) height used in final subdaily spline output 
+    and plots. This value should be defined for the GPS L1 phase center of 
+    the GNSS antenna as this is what is assumed in the subdaily code.
+
+    Parameters
+    ----------
+    station : str
+        4 ch station name
+    extension : str
+        gnssir analysis, extension mode
 
     Returns
     -------
-    De : numpy array of floats
-        corrected elevation angle, deg
-        
-    """
-    e_simple_corr = corr_el_angles(ele, p,T)
-    deg2rad = np.pi/180
-
-    # change to radians
-    ele_rad = deg2rad*(ele)
-    r = N0/1000000.
-    f = np.cos(ele_rad) / (np.sin(ele_rad) + 0.00175 * np.tan(deg2rad*(87.5) - ele_rad))
-    dE = (r * f)/deg2rad
-    fout = open('ulich.txt', 'w+')
-    for i in range(0,len(ele)):
-        fout.write(" {0:8.5f} {1:8.5f} {2:8.5f} {3:10.0f} {4:5.0f} \n ".format( 
-            ele[i], ele[i]+dE[i], e_simple_corr[i], ttime[i], sat[i]))
+    Hortho : float
+        orthometric height from gnssir json analysis file as 
+        defined as Hortho, in meters. If your preferred value 
+        for Hortho is not present, it is calculated from the  
+        ellipsoidal height and EGM96. 
 
-    fout.close()
+    """
 
-    return dE + ele
+    lsp = guts2.read_json_file(station, extension)
 
-def refrc_Rueger(drypress,vpress,temp):
+    if 'Hortho' in lsp:
+        # found in the lsp file
+        Hortho = lsp['Hortho']
+    else:
+        # calculate from EGM96
+        geoidC = g.geoidCorrection(lsp['lat'],lsp['lon'])
+        Hortho = lsp['ht']- geoidC
+
+    return Hortho
+
+def mirror_plot(tnew,ynew,spl_x,spl_y,txtdir,station,beginT,endT):
     """
-    Obtains refractivity index suitable for GNSS-IR
+    Makes a plot of the spline fit to the mirrored RH data
+    Plot is saved to txtdir as  station_rhdot1.png
 
-    Rüeger, Jean M. "Refractive index formulae for radio waves." Proceedings of the 
-    FIG XXII International Congress, Washington, DC, USA. Vol. 113. 2002.
+    Parameters
+    ----------
+    tnew : numpy of floats
+        time in days of year, including the faked data, used for splines
+    ynew : numpy of floats
+        RH in meters 
+    spl_x : numpy of floats
+        time in days of year
+    spl_y : numpy of floats
+        smooth RH, meters
+    txtdir : str
+        directory for plot
+    station : str
+        name of station for title
+    beginT : float
+        first time (day of year) real RH measurement
+    endT : float
+        last time (day of year) for first real RH measurement
+
+    """
+    fig=plt.figure(figsize=(10,4))
+
+    plt.plot(tnew,ynew, 'b.', label='obs+fake obs')
+    i = (spl_x > beginT) & (spl_x < endT) # to avoid wonky points in spline
+    plt.plot(spl_x[i],spl_y[i],'c-', label='spline')
+    plt.title('Mirrored obs and spline fit ')
+    plt.legend(loc="upper left")
+    plt.ylabel('meters')
+    if (beginT > 380):
+        plt.xlabel('MJD')
+    else:
+        plt.xlabel('days of the year')
+    plt.xlim((beginT, endT))
+    plt.grid()
+    g.save_plot(txtdir + '/' + station + '_rhdot1.png')
+    plt.close()
+
+def quickTr(year, doy,frachours):
+    """
+    takes timing from lomb scargle code (year, doy) and UTC hour (fractional)
+    and returns a date string
 
     Parameters
     ----------
-    drypress : float
-        dry pressure hPa
-    vpress : float
-        vapor pressure in hPa
-    temp : float
-        temperature in Kelvin
+    year : int
+        full year
+    doy : int
+        day of year
+    frachours : float
+        real-valued UTC hour 
 
-    Returns 
+    Returns
     -------
-    ref : list of floats
-         [Ntotal, Nhydro, Nwet], which are total, hydrostatic and wet refractivity in ppm
+    datestring : str
+         date ala YYYY-MM-DD HH:MM:SS
+    """
+    year = int(year); doy = int(doy); frachours = float(frachours)
+    # convert doy to get month and day
+    d = datetime.datetime(year, 1, 1) + datetime.timedelta(days=(doy-1))
+    month = int(d.month)
+    day = int(d.day)
+
+    hours = int(np.floor(frachours))
+    leftover = 60*(frachours - hours)
+    minutes = int(np.floor(leftover))
+    leftover_hours  = frachours - (hours + minutes/60)
+    seconds = int(leftover_hours*3600)
+    #print(frachours, hours,minutes,leftover_seconds)
+
+    jd = datetime.datetime(year,month, day,hours,minutes,seconds)
+    datestring = jd.strftime("%Y-%m-%d %H:%M:%S")
+
 
+    return datestring
+
+
+def subdaily_resids_last_stage(station, year, th, biasCor_rh, spline_at_GPS, fs, strsig, hires_figs, 
+                               txtdir, ii, jj, th_even,spline_whole_time):
     """
+    Makes the final residual plot for subdaily (after RHdot and IF correction made).
+    Returns the bad points ...
 
-    # Rüeger's "best average", for 375 ppm CO2, 77.690 for 392 ppm CO2
-    [K1r,K2r,K3r]=[77.689 ,71.2952 ,375463.]     
 
-    # Rueger,IAG recommend, in ppm
-    Nrueger = K1r * drypress / temp + K2r * vpress / temp + K3r * vpress / (temp ** 2)  
+    Allows either the original or multiyear option..
 
-    # gas constant (SI exact), molar masses of dry air and water, kg/mol
-    [Rgas,Md,Mw] = [8.31446261815324,0.0289644,0.01801528]   
 
-    #density in kg/m^3
-    drydensity=(drypress*100.)*Md/(Rgas*temp)    
-    #in PV=nRT, P in Pa, V in m^3, n in g/mol, T in K, R=8.314 Pa*m^3/(k*mol)
-    vdensity=(vpress*100.)*Mw/(Rgas*temp)   
-    totaldensity=drydensity+vdensity
+    Parameters
+    ----------
+    station : str
+        4 character station name
+    year : int
+        calendar year
+    th : numpy array of ??
+        time variable of some kind, fractional day of year ?
+    biasCor_rh : numpy array of floats
+        refl hgts that have been corrected for RHdot and IF
+    spline_at_GPS : numpy array of floats
+        RH derived From the spline fit and calculated at GPS time tags
+    fs : int
+        font size
+    strsig : str
+        sigma string to go on the legend
+    hires_figs : bool
+        whether to save the plots with better resolution
+    txtdir : str
+        directory where the plot will be saved
+    ii : numpy array
+        indices of the outliers?
+    jj : numpy array
+        indices of the values to keep?
+    th_even : numpy array
+        evenly spaced time values, day of year
+    spline_whole_time : numpy array of flots
+        splinefit for ???
 
-    #divide 100 because hPa in Rueger formula, result in ppm
-    Nhydro=(K1r*Rgas*totaldensity/Md)/100.   
-    K2rr=K2r-K1r*(Mw/Md)
-    Nwet=K2rr * vpress / temp + K3r * vpress / (temp ** 2)
-    # in ppm
-    ref=[round(Nrueger,4),round(Nhydro,4),round(Nwet,4)]    
-    return ref
+    Returns
+    -------
+    badpoints2 : numpy array of floats
+         RH residuals
+    """
+    # this means you are already in MJD ... 
+    if (th[0] > 400):
+        th_obs = mjd_to_obstimes(th)
+        th_even_obs = mjd_to_obstimes(th_even)
+    else:
+        # convert obs to mjd and then obstimes
+        mjd0 = g.fdoy2mjd(year, th[0])
+        th_obs = mjd_to_obstimes(mjd0 + th - th[0])
+    # convert the spline to mjd and then obstimes
+        mjd1 = g.fdoy2mjd(year, th_even[0])
+        th_even_obs = mjd_to_obstimes(mjd1 + th_even - th_even[0])
+
+
+    # these are now plotted in datetime via mjd translation
+    fig=plt.figure(figsize=(10,5))
+    plt.plot(th_obs, biasCor_rh, 'b.', label='RH ' + strsig)
+    plt.plot(th_even_obs, spline_whole_time, '-',color='orange',label='spline')
+    plt.plot(th_obs[ii], biasCor_rh[ii], 'rx', label='outliers')
+
+    plt.legend(loc="best",fontsize=fs)
+    plt.grid() ; plt.gca().invert_yaxis()
+    plt.ylabel('meters',fontsize=fs); 
+    plt.title(station.upper() + ' RH with RHdot and InterFrequency Corrections Applied',fontsize=fs)
+    fig.autofmt_xdate()
+
+    # put hires_figs boolean here
+    if hires_figs:
+        g.save_plot(txtdir + '/' + station + '_rhdot4.eps')
+    else:
+        g.save_plot(txtdir + '/' + station + '_rhdot4.png')
+
+    # this figure is not sent to the screen
+    fig=plt.figure(figsize=(10,5))
+    plt.plot(th_obs, biasCor_rh - spline_at_GPS, 'b.',label='all residuals')
+    plt.title('Station:' + station + ' Residuals to new spline fit',fontsize=fs)
+    plt.grid()
+    plt.ylabel('meters',fontsize=fs)
+
+    plt.plot(th_obs[ii], (biasCor_rh -spline_at_GPS)[ii], 'r.',label='outliers')
+    # will write these residauls out to a file
+    badpoints2 =  (biasCor_rh -spline_at_GPS)[ii]
+    plt.legend(loc="upper left",fontsize=fs)
+    fig.autofmt_xdate()
+
+    # print('\n RMS with frequency biases and RHdot taken out (m) ', np.round(newsigma,3) , '\n' )
+    if hires_figs:
+        g.save_plot(txtdir + '/' + station + '_rhdot5.eps')
+    else:
+        g.save_plot(txtdir + '/' + station + '_rhdot5.png')
+
+    plt.close() # 
 
+    return badpoints2
 
-def Equvilent_Angle_Corr_NITE(Hr_apr, e_T, N_ant, ztd_ant, mpf_tot, dmpf_de_tot):
+def RH_ortho_plot2( station, H0, year,  txtdir, fs, time_rh, rh, gap_min_val,th,spline,delta_out,csvfile):
     """
-    NITE formula equvilent angle correction and forward model
-    From Peng et al. 2023
+
+    Makes a plot of the final spline fit to the data. Output time interval controlled by the user.
+
+    It also now writes out the file with the spline fit
 
     Parameters
     ----------
-    Hr_apr : float
-        a priori reflector height, meters
-
-    e_T : float
-        elevation angle - units!!!!!
+    station : str
+        name of station, 4 ch
+    H0 : float
+        datum correction (orthometric height) to convert RH to MSL data, in meters
+    year : int
+        year of the time series (ultimately should not be needed)
+    txtdir : str
+       location of plot
+    fs : int
+        fontsize
+    time_rh : numpy of floats
+        time of rh values, in fractional doy I believe
+    rh : numpy of floats
+        refl hgt in meters
+    gap_min_val : float
+        minimum length gap allowed, in day of year units
+    th : numpy floats
+        time values in day of year units
+    spline : output of interpolate.BSpline
+        used for fitting 
+    delta_out : int
+        how often spline is printed, in seconds
+    csvfile : bool
+        print out csv instead of plain txt
+    """
+
+    firstpoint = float(th[0]); lastpoint = float(th[-1])
+    s1 = math.floor(firstpoint); s2 = math.ceil(lastpoint)
+    ndays = s2-s1 # number of days
+    numvals = 1 + int(ndays*86400/delta_out)
+    tp=np.linspace(s1,s2,numvals,endpoint= True)
+
+    # previous tp definition goes from beginning of the first day to the end of last day - but 
+    # does not recognize that the file could have started well beyond that first point 
+    # and it might end say 8 hours into the last day
+    ii = (tp >= firstpoint) & (tp <= lastpoint)
+    tp = tp[ii]
+
+    # this means it is already in MJD
+
+    if (th[0] > 400): 
+        multiyear = True
+        mjd_new = tp
+        mjd_new_obstimes = mjd_to_obstimes(mjd_new)
+        spline_new = spline(tp)
+    else:
+        multiyear = False
+        mjd1 = g.fdoy2mjd(year, tp[0] ) # 
+        mjd_new = mjd1 + (tp - tp[0])
+        mjd_new_obstimes = mjd_to_obstimes(mjd_new)
+        spline_new = spline(tp)
+    N_new = len(mjd_new_obstimes)
+
+    # looks like I identified the gaps in day of year units - 
+    # but then did the implementation in mjd and then datetime ...
+    #splinefileout =  txtdir + '/' + station + '_' + str(year) + '_spline_out.txt'
+    if csvfile:
+        splinefileout =  txtdir + '/' + station +  '_spline_out.csv'
+    else:
+        splinefileout =  txtdir + '/' + station +  '_spline_out.txt'
 
-    N_ant : float
-        antenna refractivity
 
-    ztd_ant : float
-        total zenith tropo delay, meters
+    print('Writing evenly sampled file to: ', splinefileout)
+    fout = open(splinefileout,'w+')
+    vn = station + ' gnssrefl v' + str(g.version('gnssrefl'))
+    fout.write('{0:1s}  {1:30s}  \n'.format('%','station ' + vn))
+    fout.write('{0:1s}  {1:30s}  \n'.format('%','This is NOT observational data - be careful when interpreting it.'))
+    fout.write('{0:1s}  {1:30s}  \n'.format('%','If the data are not well represented by the spline functions, you will '))
+    fout.write('{0:1s}  {1:30s}  \n'.format('%','have a very poor representation of the data. I am also writing out station '))
+    fout.write('{0:1s}  {1:30s}  {2:8.3f} \n'.format('%','orthometric height minus RH, where Hortho (m) is ', H0  ))
+    #fout.write('{0:1s}  {1:30s}  \n'.format('%','This assumes RH is measured relative to the L1 phase center.  '))
+    #fout.write('{0:1s}  {1:30s}  \n'.format('%','MJD, RH(m), YY,MM,DD,HH,MM,SS, quasi-sea-level(m)'))
+    if csvfile:
+        fout.write('{0:1s}  {1:30s}  \n'.format('%','MJD,             RH(m), YYYY, MM, DD, HH, MM, SS,  quasi-sea-level(m)'))
+        fout.write('{0:1s}  {1:30s}  \n'.format('%','(1),              (2),  (3), (4),(5), (6),(7),(8),   (9)'))
+    else:
+        fout.write('{0:1s}  {1:30s}  \n'.format('%','MJD              RH(m)  YYYY  MM  DD  HH  MM  SS   quasi-sea-level(m)'))
+        fout.write('{0:1s}  {1:30s}  \n'.format('%','(1)               (2)   (3)  (4) (5)  (6) (7) (8)    (9)'))
 
-    mpf_tot : float
 
-    dmpf_de_tot : float
+    # difference function to find time between all rh measurements
+    gdiff = np.diff( time_rh )
+    if multiyear:
+        mjdt = time_rh
+        mjd = mjdt[0:-1]
+    else:
+        mjdx = g.fdoy2mjd(year, time_rh[0] ) # 
+        mjdt = mjdx + (time_rh - time_rh[0])
+        mjd = mjdt[0:-1]
+
+
+    # find indices of gaps  that are larger than a certain value
+    ii = (gdiff > gap_min_val)
+    #print('gap_min_val',gap_min_val, gdiff)
+    N = len(mjd[ii])
+    Ngdiff = len(gdiff)
+
+    dlist = mjd_new_obstimes.tolist()
+
+
+    # i have not figured this one out yet ... the horror
+    #if not multiyear:
+    if True:
+    # get the integer values to write out  to the text file ...
+        theyear = [y.year for y in dlist ]
+        xm = [y.month for y in dlist]; xd = [y.day for y in dlist]
+        xh = [y.hour for y in dlist]; xmin = [y.minute for y in dlist]
+        xs = [y.second for y in dlist]
+
+        if (Ngdiff > 0):
+            for i in range(0,Ngdiff):
+                if ii[i]:
+                    e0 = mjd[i] ; e1 = mjd[i+1] # beginning and ending of the gap
+                    bad_indices = (mjd_new > e0) & (mjd_new < e1 )
+                    spline_new[bad_indices] = np.nan
+                    mjd_new_obstimes[bad_indices] = np.datetime64("NaT")
+
+    # write the spline values to a file, with gaps removed
+        for i in range(0,N_new):
+            if not np.isnan(spline_new[i]):
+                rhout = spline_new[i]
+                if csvfile:
+                    fout.write('{0:15.7f}, {1:10.3f},{2:4.0f},{3:3.0f},{4:3.0f},{5:3.0f},{6:3.0f},{7:3.0f},{8:10.3f} \n'.format( mjd_new[i], rhout, theyear[i], xm[i], xd[i], xh[i], xmin[i], xs[i], H0-rhout))
+                else:
+                    fout.write('{0:15.7f}  {1:10.3f} {2:4.0f} {3:3.0f} {4:3.0f} {5:3.0f} {6:3.0f} {7:3.0f} {8:10.3f} \n'.format(mjd_new[i], rhout, theyear[i], xm[i], xd[i], xh[i], xmin[i], xs[i], H0-rhout))
 
 
-    Returns
-    -------
-    new_elev : float
-        new elevation angle, units?
+    fout.close()
 
-    """
-    e_A = e_T+Ulich_Bending_Angle_original(e_T, N_ant)
-    sita_E = sita_Earth(Hr_apr, e_A)
-    sita_S = sita_Satellite(Hr_apr, e_A)
-    e_A_r = e_A+sita_E +sita_S
-    Hv_ratio = Hv_Hr_ratio(Hr_apr, 6378137., e_A)
-    sin_eqv_geo = 0.5 * Hv_ratio / np.sin(np.radians(e_A_r + sita_E)) * (1. - np.cos(np.radians(e_T + e_A_r + sita_E)))
-    Nl = N_layer(N_ant, Hr_apr)
-    dsin_up = Hv_ratio*(Nl / 1000000.)/np.sin(np.radians(e_A_r + sita_E))
-    ddele_T_dh = np.tan(np.radians(e_A))
-    dsin_down = Nl / 1000000.*mpf_tot-ztd_ant*(dmpf_de_tot*(1. / (6378137. *ddele_T_dh ))+dmpf_dh(e_T, dhgt=1.))
-    dsin = 0.5*(dsin_up + dsin_down)
-    ele_eqv = np.degrees(np.arcsin(sin_eqv_geo + dsin))
-    new_elev = ele_eqv - e_T
-    return new_elev
+    fig=plt.figure(figsize=(10,5))
+    plt.plot(mjd_new_obstimes, H0 -spline_new, 'b-',linewidth=2)
+    plt.grid()
+    plt.ylabel('meters',fontsize=fs)
+    plt.title(station.upper() + ' Water Level from GNSS-IR', fontsize=fs)
+    fig.autofmt_xdate()
+
+    pfile = txtdir + '/' + station + '_H0.png'
+    g.save_plot(pfile)
 
+    return
 
-def gmf_deriv(dmjd,dlat,dlon,dhgt,zd):
+def pickup_subdaily_json_defaults(xdir, station, extension):
     """
-    This subroutine determines the Global Mapping Functions GMF  and derivative.
-    Translated from https://vmf.geo.tuwien.ac.at/codes/gmf_deriv.f by Peng Feng in March, 2023.
-
-    Johannes Boehm, 2005 August 30
-    
-    ref 2006 Aug. 14: derivatives (U. Hugentobler)
-    ref 2006 Aug. 14: recursions for Legendre polynomials (O. Montenbruck)
-    ref 2011 Jul. 21: latitude -> ellipsoidal latitude
+    picks up an existing gnssir analysis json. augments
+    with subdaily parameters if needed. Returns the dictionary.
 
     Parameters
     ----------
-    dmjd: float
-        modified julian date
-    dlat: float
-        ellipsoidal latitude in radians
-    dlon: float
-        longitude in radians
-    dhgt: float
-        height in m
-    zd: float
-        zenith distance in radians ??? ( is this really what you mean??
+    xdir : str
+        REFL_CODE code location
+    station : str
+        name of station
+    extension : str
+        possible extension location
 
     Returns
     -------
-    gmfh(2): floats
-        hydrostatic mapping function and derivative wrt z
-
-    gmfw(2): floats
-        wet mapping function and derivative wrt z
-    
+    lsp : dictionary 
+        contents of gnssir json
     """
 
-    ah_mean=[+1.2517e+02, +8.503e-01, +6.936e-02, -6.760e+00, +1.771e-01,
-             +1.130e-02, +5.963e-01, +1.808e-02, +2.801e-03, -1.414e-03,
-             -1.212e+00, +9.300e-02, +3.683e-03, +1.095e-03, +4.671e-05,
-             +3.959e-01, -3.867e-02, +5.413e-03, -5.289e-04, +3.229e-04,
-             +2.067e-05, +3.000e-01, +2.031e-02, +5.900e-03, +4.573e-04,
-             -7.619e-05, +2.327e-06, +3.845e-06, +1.182e-01, +1.158e-02,
-             +5.445e-03, +6.219e-05, +4.204e-06, -2.093e-06, +1.540e-07,
-             -4.280e-08, -4.751e-01, -3.490e-02, +1.758e-03, +4.019e-04,
-             -2.799e-06, -1.287e-06, +5.468e-07, +7.580e-08, -6.300e-09,
-             -1.160e-01, +8.301e-03, +8.771e-04, +9.955e-05, -1.718e-06,
-             -2.012e-06, +1.170e-08, +1.790e-08, -1.300e-09, +1.000e-10]
-
-    bh_mean=[+0.000e+00, +0.000e+00, +3.249e-02, +0.000e+00, +3.324e-02,
-             +1.850e-02, +0.000e+00, -1.115e-01, +2.519e-02, +4.923e-03,
-             +0.000e+00, +2.737e-02, +1.595e-02, -7.332e-04, +1.933e-04,
-             +0.000e+00, -4.796e-02, +6.381e-03, -1.599e-04, -3.685e-04,
-             +1.815e-05, +0.000e+00, +7.033e-02, +2.426e-03, -1.111e-03,
-             -1.357e-04, -7.828e-06, +2.547e-06, +0.000e+00, +5.779e-03,
-             +3.133e-03, -5.312e-04, -2.028e-05, +2.323e-07, -9.100e-08,
-             -1.650e-08, +0.000e+00, +3.688e-02, -8.638e-04, -8.514e-05,
-             -2.828e-05, +5.403e-07, +4.390e-07, +1.350e-08, +1.800e-09,
-             +0.000e+00, -2.736e-02, -2.977e-04, +8.113e-05, +2.329e-07,
-             +8.451e-07, +4.490e-08, -8.100e-09, -1.500e-09, +2.000e-10]
-
-    ah_amp=[ -2.738e-01, -2.837e+00, +1.298e-02, -3.588e-01, +2.413e-02,
-            +3.427e-02, -7.624e-01, +7.272e-02, +2.160e-02, -3.385e-03,
-            +4.424e-01, +3.722e-02, +2.195e-02, -1.503e-03, +2.426e-04,
-            +3.013e-01, +5.762e-02, +1.019e-02, -4.476e-04, +6.790e-05,
-            +3.227e-05, +3.123e-01, -3.535e-02, +4.840e-03, +3.025e-06,
-            -4.363e-05, +2.854e-07, -1.286e-06, -6.725e-01, -3.730e-02,
-            +8.964e-04, +1.399e-04, -3.990e-06, +7.431e-06, -2.796e-07,
-            -1.601e-07, +4.068e-02, -1.352e-02, +7.282e-04, +9.594e-05,
-            +2.070e-06, -9.620e-08, -2.742e-07, -6.370e-08, -6.300e-09,
-            +8.625e-02, -5.971e-03, +4.705e-04, +2.335e-05, +4.226e-06,
-            +2.475e-07, -8.850e-08, -3.600e-08, -2.900e-09, +0.000e+00]
-
-    bh_amp=[+0.000e+00, +0.000e+00, -1.136e-01, +0.000e+00, -1.868e-01,
-            -1.399e-02, +0.000e+00, -1.043e-01, +1.175e-02, -2.240e-03,
-            +0.000e+00, -3.222e-02, +1.333e-02, -2.647e-03, -2.316e-05,
-            +0.000e+00, +5.339e-02, +1.107e-02, -3.116e-03, -1.079e-04,
-            -1.299e-05, +0.000e+00, +4.861e-03, +8.891e-03, -6.448e-04,
-            -1.279e-05, +6.358e-06, -1.417e-07, +0.000e+00, +3.041e-02,
-            +1.150e-03, -8.743e-04, -2.781e-05, +6.367e-07, -1.140e-08,
-            -4.200e-08, +0.000e+00, -2.982e-02, -3.000e-03, +1.394e-05,
-            -3.290e-05, -1.705e-07, +7.440e-08, +2.720e-08, -6.600e-09,
-            +0.000e+00, +1.236e-02, -9.981e-04, -3.792e-05, -1.355e-05,
-            +1.162e-06, -1.789e-07, +1.470e-08, -2.400e-09, -4.000e-10]
-
-    aw_mean=[+5.640e+01, +1.555e+00, -1.011e+00, -3.975e+00, +3.171e-02,
-             +1.065e-01, +6.175e-01, +1.376e-01, +4.229e-02, +3.028e-03,
-             +1.688e+00, -1.692e-01, +5.478e-02, +2.473e-02, +6.059e-04,
-             +2.278e+00, +6.614e-03, -3.505e-04, -6.697e-03, +8.402e-04,
-             +7.033e-04, -3.236e+00, +2.184e-01, -4.611e-02, -1.613e-02,
-             -1.604e-03, +5.420e-05, +7.922e-05, -2.711e-01, -4.406e-01,
-             -3.376e-02, -2.801e-03, -4.090e-04, -2.056e-05, +6.894e-06,
-             +2.317e-06, +1.941e+00, -2.562e-01, +1.598e-02, +5.449e-03,
-             +3.544e-04, +1.148e-05, +7.503e-06, -5.667e-07, -3.660e-08,
-             +8.683e-01, -5.931e-02, -1.864e-03, -1.277e-04, +2.029e-04,
-             +1.269e-05, +1.629e-06, +9.660e-08, -1.015e-07, -5.000e-10]
-
-    bw_mean=[+0.000e+00, +0.000e+00, +2.592e-01, +0.000e+00, +2.974e-02,
-             -5.471e-01, +0.000e+00, -5.926e-01, -1.030e-01, -1.567e-02,
-             +0.000e+00, +1.710e-01, +9.025e-02, +2.689e-02, +2.243e-03,
-             +0.000e+00, +3.439e-01, +2.402e-02, +5.410e-03, +1.601e-03,
-             +9.669e-05, +0.000e+00, +9.502e-02, -3.063e-02, -1.055e-03,
-             -1.067e-04, -1.130e-04, +2.124e-05, +0.000e+00, -3.129e-01,
-             +8.463e-03, +2.253e-04, +7.413e-05, -9.376e-05, -1.606e-06,
-             +2.060e-06, +0.000e+00, +2.739e-01, +1.167e-03, -2.246e-05,
-             -1.287e-04, -2.438e-05, -7.561e-07, +1.158e-06, +4.950e-08,
-             +0.000e+00, -1.344e-01, +5.342e-03, +3.775e-04, -6.756e-05,
-             -1.686e-06, -1.184e-06, +2.768e-07, +2.730e-08, +5.700e-09]
-
-    aw_amp=[+1.023e-01, -2.695e+00, +3.417e-01, -1.405e-01, +3.175e-01,
-            +2.116e-01, +3.536e+00, -1.505e-01, -1.660e-02, +2.967e-02,
-            +3.819e-01, -1.695e-01, -7.444e-02, +7.409e-03, -6.262e-03,
-            -1.836e+00, -1.759e-02, -6.256e-02, -2.371e-03, +7.947e-04,
-            +1.501e-04, -8.603e-01, -1.360e-01, -3.629e-02, -3.706e-03,
-            -2.976e-04, +1.857e-05, +3.021e-05, +2.248e+00, -1.178e-01,
-            +1.255e-02, +1.134e-03, -2.161e-04, -5.817e-06, +8.836e-07,
-            -1.769e-07, +7.313e-01, -1.188e-01, +1.145e-02, +1.011e-03,
-            +1.083e-04, +2.570e-06, -2.140e-06, -5.710e-08, +2.000e-08,
-            -1.632e+00, -6.948e-03, -3.893e-03, +8.592e-04, +7.577e-05,
-            +4.539e-06, -3.852e-07, -2.213e-07, -1.370e-08, +5.800e-09]
-
-    bw_amp=[+0.000e+00, +0.000e+00, -8.865e-02, +0.000e+00, -4.309e-01,
-            +6.340e-02, +0.000e+00, +1.162e-01, +6.176e-02, -4.234e-03,
-            +0.000e+00, +2.530e-01, +4.017e-02, -6.204e-03, +4.977e-03,
-            +0.000e+00, -1.737e-01, -5.638e-03, +1.488e-04, +4.857e-04,
-            -1.809e-04, +0.000e+00, -1.514e-01, -1.685e-02, +5.333e-03,
-            -7.611e-05, +2.394e-05, +8.195e-06, +0.000e+00, +9.326e-02,
-            -1.275e-02, -3.071e-04, +5.374e-05, -3.391e-05, -7.436e-06,
-            +6.747e-07, +0.000e+00, -8.637e-02, -3.807e-03, -6.833e-04,
-            -3.861e-05, -2.268e-05, +1.454e-06, +3.860e-07, -1.068e-07,
-            +0.000e+00, -2.658e-02, -1.947e-03, +7.131e-04, -3.506e-05,
-            +1.885e-07, +5.792e-07, +3.990e-08, +2.000e-08, -5.700e-09]
-
-
-    pi = 3.141592653590000
-
-#   reference day is 28 January
-#   this is taken from Niell (1996) to be consistent
-    doy = dmjd  - 44239.0 + 1 - 28
-
-#   degree n and order m
-    nmax = 9
-    mmax = 9
-
-#   unit vector
-    x = math.cos(dlat)*math.cos(dlon)
-    y = math.cos(dlat)*math.sin(dlon)
-    z = math.sin(dlat)
-  
-# Legendre polynomials (Cunningham)
-
-    V=[[0. for j in range(nmax+1) ] for i in range(nmax+1)]
-    W = [[0. for j in range(mmax + 1)] for i in range(mmax + 1)]
-
-    V[0][0]=1.0
-    W[0][0]=0.0
-    V[1][0]=z*V[0][0]
-    W[1][0]=0.0
-    # print(z)
-
-
-    for n in range(2,nmax+1):
-        V[n][0]=((2*n-1) * z * V[n-1][0] - (n-1) * V[n-2][0])  / n
-        W[n][0]=0.0
-
-
-    for m in range(1,nmax+1):
-        V[m][m] = (2 * m - 1) * (x * V[m - 1][m - 1] - y * W[m - 1][m - 1])
-        W[m][m] = (2 * m - 1) * (x * W[m - 1][m - 1] + y * V[m - 1][m - 1])
-
-        if m<nmax:
-            V[m + 1][m] = (2 * m + 1) * z * V[m][m]
-            W[m + 1][m] = (2 * m + 1) * z * W[m][m]
-        for n in range(m+2,nmax+1):
-            V[n][m] = ((2 * n - 1) * z * V[n-1][m] - (n + m - 1) * V[n-2][m]) / (n - m)
-            W[n][m] = ((2 * n - 1) * z * W[n-1][m] - (n + m - 1) * W[n-2][m]) / (n - m)
-    # print(V)
-    # print(W)
-
-
-    #hydrostatic
-    bh = 0.0029
-    c0h = 0.062
-    if dlat <0.: # southern hemisphere
-        phh = pi
-        c11h = 0.007
-        c10h = 0.002
-    else: # northern hemisphere
-        phh = 0
-        c11h = 0.005
-        c10h = 0.001
-    ch = c0h + ((math.cos(doy / 365.25 * 2. * pi + phh) + 1) * c11h / 2. + c10h) *(1. - math.cos(dlat))
-
-    ahm = 0.
-    aha = 0.
-    i = 0
-    for n in range(0,nmax+1):
-        for m in range(0,n+1):
-            ahm = ahm + (ah_mean[i] * V[n][m] + bh_mean[i] * W[n][m])
-            # print('ahm',i,n,m,ahm,ah_mean[i] , V[n][m] , bh_mean[i],W[n][m])
-            aha = aha + (ah_amp[i] * V[n][m]+ bh_amp[i] * W[n][m])
-            # print('aha', i, n, m, aha, ah_amp[i], V[n][m], bh_amp[i], W[n][m])
-            i=i+1
-    ah=(ahm + aha*math.cos(doy/365.250*2.0*pi))*1.e-5
-    # print('ah',ah,ahm,aha,i)
-    # print(V)
-    # print(W)
-    # print(ah_mean)
-
-
-    sine = math.sin(pi / 2 - zd)
-    cose = math.cos(pi / 2 - zd)
-    beta = bh / (sine + ch)
-    gamma = ah / (sine + beta)
-    topcon = (1.0 + ah / (1.0 + bh / (1.0 + ch)))
-    gmfh=[0.,0.]
-    gmfh[0] = topcon / (sine + gamma)
-#   derivative
-    gmfh[1] = gmfh[0] ** 2 / topcon * cose * (1 - gamma ** 2 / ah * (1 - beta ** 2 / bh))
-
-#    height correction for hydrostatic mapping function from Niell (1996)
-    a_ht = 2.53e-5
-    b_ht = 5.49e-3
-    c_ht = 1.14e-3
-    hs_km = dhgt / 1000.0
-
-    beta = b_ht / (sine + c_ht)
-    gamma = a_ht / (sine + beta)
-    topcon = (1.0 + a_ht / (1.0 + b_ht / (1.0 + c_ht)))
-    ht_corr_coef = 1 / sine - topcon / (sine + gamma)
-    ht_corr = ht_corr_coef * hs_km
-    gmfh[0] = gmfh[0] + ht_corr
-
-#   derivative
-    gmfh[1]= gmfh[1] + (cose/sine**2 - topcon*cose/(sine+gamma)**2*(1-gamma**2/a_ht*(1-beta**2/b_ht))) * hs_km
-
-
-#   wet
-    bw = 0.00146
-    cw = 0.04391
-    awm = 0.0
-    awa = 0.0
-    i=0
-    for n in range(0,nmax+1):
-        for m in range(0,n+1):
-            awm = awm + (aw_mean[i] * V[n][m] + bw_mean[i] * W[n][m])
-            awa = awa + (aw_amp[i] * V[n][m] + bw_amp[i] * W[n][m])
-            i=i+1
-
-    aw = (awm + awa * math.cos(doy / 365.250 * 2 * pi))*1e-5
-    beta = bw / (sine + cw)
-    gamma = aw / (sine + beta)
-    topcon = (1.0 + aw / (1.0 + bw / (1.0 + cw)))
-
-    gmfw = [0., 0.]
-    gmfw[0] = topcon / (sine + gamma)
-
-#   derivative
-    gmfw[1] = gmfw[0] ** 2 / topcon * cose * (1 - gamma ** 2 / aw * (1 - beta ** 2 / bw))
-    return [gmfh[0],gmfh[1],gmfw[0],gmfw[1]]
-
-
-def sita_Earth(Hr, e_A):                                   
-    """
-    no documentation
-    # in meter, in degree
-
-
-    """
-
-    # earth center angle between the reflection point and the GNSS antenna
-    sita_E = Hr / (6378137. * np.tan(np.radians(e_A)))
-    return round(np.degrees(sita_E), 6)                              # in degree
-
-def sita_Satellite(Hr, e_A):                               
-    """
-    no documentation 
-    # in meter, in degree
-    # satellite angle between the reflection point and the GNSS antenna
-
-    """
-
-    ant2satell = 4.*6378137.    # assume satellite distance 4 times earth radius
-    sita_S = 2 * Hr * np.cos(np.radians(e_A)) / ant2satell
-    return round(np.degrees(sita_S), 6)    # in degree, small for MEO satellites
-
-def dH_curve(Hr, Re, e_A):                       
-    """
-    no documentation provided
-    # in meter, in meter, in degree
-    #vertial displacement of the reflection point vs. a "plane reflection"
-    """
-    dH = Re * (1. - np.cos(Hr / np.tan(np.radians(e_A)) / Re))
-    return round(dH, 6)    # in meters
-
-def Hv_Hr_ratio(Hr, Re, e_A):
-    """
-    no documentation provided
-    # in meter, in meter, in degree
-    """
-    dH = Re * (1. - np.cos(Hr / np.tan(np.radians(e_A)) / Re))
-    return (Hr+dH) /Hr    #ratio, allways bigger than 1
-
-def N_layer(N_antenna, Hr):
-    """
-    no documentation 
-
-    #in ppm, in meter
-    # average refractivity in the layer between GNSS antenna and sea surface
-    """
-    Nl = N_antenna *(1+np.exp(Hr/8000.)) /2
-    return round(Nl, 4)     #in ppm
-
-def saastam2(press, lat, height):
-    """
-    no documentation
-    in hPa,  in degree, in meter
-    Saastamion model with updated refractivity equation from Rüeger (2002)
-
-    as best i understand this it is the dry delay
-    """
-    phi = lat / 180 * 3.14159265359
-    height = height / 1000.
-    f = 1. - 0.0026 * np.cos(2. * phi) - 0.00028 * height
-    # ZHD in meter
-    return round(2.2794 * press / f / 1000., 6)                   
-
-def mpf_tot(gmf_h, gmf_w, zhd, zwd):  
-    """
-    no documentation
-    #convert seperate wet&dry MPF to total MPF
-
-    guessing
-
-    gmf_h : float
-        ?
-    gmf_w : float
-        ?
-    zhd : float
-        zenith hydrostatic delay
-    zwd : float
-        zenith wet delay
-    """
-    mpf_tot1=(gmf_h*zhd+gmf_w*zwd)/(zhd+zwd)
-
-    return mpf_tot1
-
-def dmpf_dh(ele, dhgt):    
-    """
-    no documentation
-    # mapping function height correction by (Niell, 1996)
-    """
-    sine = np.sin(np.radians(ele))
-    [a_ht, b_ht, c_ht] = [0.0000253, 0.00549, 0.00114]
-    hs_km = dhgt / 1000.
-    beta = b_ht / (sine + c_ht)
-    topcon = (1. + a_ht / (1. + b_ht / (1. + c_ht)))
-    ht_corr_coef = 1 / sine - topcon / (sine + a_ht / (sine + beta))
-    return ht_corr_coef * hs_km
-
-
-def Ulich_Bending_Angle_original(ele, N0):   
-    """
-    no documentation
-    # input degree, ppm
-    """
-    ele = np.radians(ele)
-    r = N0/1000000.
-    f = np.cos(ele) / (np.sin(ele) + 0.00175 * np.tan(np.radians(87.5) - ele))
-    return np.degrees(r * f)
+    # changed default in subdaily to None instead of '' So have to check
+    if extension is None:
+        lsp = guts2.read_json_file(station, '',noexit=True)
+    else:
+        lsp = guts2.read_json_file(station, extension,noexit=True)
+
+    # check json for subdaily settings
+    # if values not found, then set them to None
+
+    if 'subdaily_ampl' not in lsp:
+        lsp['subdaily_ampl'] = None
+
+    if 'subdaily_spline_outlier1' not in lsp:
+        lsp['subdaily_spline_outlier1'] = None
+
+    if 'subdaily_spline_outlier2' not in lsp:
+        lsp['subdaily_spline_outlier2'] = None
+
+    if 'subdaily_knots' not in lsp:
+        lsp['subdaily_knots'] = None
+
+    if 'subdaily_delta_out' not in lsp:
+        lsp['subdaily_delta_out'] = None
+
+    if 'subdaily_alt_sigma' not in lsp:
+        lsp['subdaily_alt_sigma'] = None
+
+    if 'subdaily_sigma' not in lsp:
+        lsp['subdaily_sigma'] = None
+
+    if 'subdaily_subdir' not in lsp:
+        lsp['subdaily_subdir'] = None
 
+    return lsp
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gnssrefl-3.1.5/gnssrefl/rh_plot.py` & `gnssrefl-3.2.0/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/rinex2snr.py` & `gnssrefl-3.2.0/gnssrefl/rinex2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/rinex2snr_cl.py` & `gnssrefl-3.2.0/gnssrefl/rinex2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/rinex3_rinex2.py` & `gnssrefl-3.2.0/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/rinex3_snr.py` & `gnssrefl-3.2.0/gnssrefl/rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/rinex_coords.py` & `gnssrefl-3.2.0/gnssrefl/rinex_coords.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/rinpy.py` & `gnssrefl-3.2.0/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-3.2.0/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/smoosh.py` & `gnssrefl-3.2.0/gnssrefl/smoosh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/smoosh_snr.py` & `gnssrefl-3.2.0/gnssrefl/smoosh_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/snow_functions.py` & `gnssrefl-3.2.0/gnssrefl/snow_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/snowdepth_cl.py` & `gnssrefl-3.2.0/gnssrefl/snowdepth_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/spline_functions.py` & `gnssrefl-3.2.0/gnssrefl/spline_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -774,15 +774,15 @@
     #print(doplot, ' doplot setting')
     imodel = 0 # no refraction
     if 'lsp' in kwargs:
         lsp = kwargs.get('lsp')
         if lsp['refraction']:
             imodel = 1 #
         dmjd = 59580 # fake number
-        p,T,irefr,humidity = set_refraction_model(station, dmjd,lsp,imodel)
+        p,T,irefr,humidity, Tm, lapse_rate = set_refraction_model(station, dmjd,lsp,imodel)
         #print('refraction parameters ', p,T,humidity,irefr)
 
     if 'rough_in' in kwargs:
         rough_in  = kwargs.get('rough_in')
 
     risky = False
     if 'risky' in kwargs:
@@ -1721,23 +1721,28 @@
         pressure (units?)
     T : float
         temperature in deg C
     irefr : int
         number value written to output files to keep track of refraction model
     e : float
         water vapor pressure, hPa
+    Tm : float
+        temperature in kelvin
+    lapse_rate : float
+        see source code for details
 
     """
     xdir = os.environ['REFL_CODE']
     p = 0; T = 0; irefr = 0
     #print(lsp['lat'], lsp['lon'])
     if (imodel == 1):
         irefr = 1
         refr.readWrite_gpt2_1w(xdir, station, lsp['lat'], lsp['lon'])
 # time varying is set to no for now (it = 1)
         it = 1
+        # should use sea level, and this is ellipsoidal height.  so it is wrong
         dlat = lsp['lat']*np.pi/180; dlong = lsp['lon']*np.pi/180; ht = lsp['ht']
         p,T,dT,Tm,e,ah,aw,la,undu = refr.gpt2_1w(station, dmjd,dlat,dlong,ht,it)
         #print("Pressure {0:8.2f} Temperature {1:6.1f} \n".format(p,T))
 
-    return p,T,irefr, e
+    return p,T,irefr, e, Tm, la
```

### Comparing `gnssrefl-3.1.5/gnssrefl/subdaily.py` & `gnssrefl-3.2.0/gnssrefl/subdaily.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/subdaily_cl.py` & `gnssrefl-3.2.0/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/utils.py` & `gnssrefl-3.2.0/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/veg_multiyr.py` & `gnssrefl-3.2.0/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/vwc_cl.py` & `gnssrefl-3.2.0/gnssrefl/vwc_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/vwc_input.py` & `gnssrefl-3.2.0/gnssrefl/vwc_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/xnmeasnr.f` & `gnssrefl-3.2.0/gnssrefl/xnmeasnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/xyz2llh.py` & `gnssrefl-3.2.0/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/ydoy.py` & `gnssrefl-3.2.0/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl/ymd.py` & `gnssrefl-3.2.0/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-3.2.0/gnssrefl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 3.1.5
+Version: 3.2.0
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# gnssrefl v3.1.5 
+# gnssrefl v3.2.0 
 
 If you use this code in any presentation or publication, you are expected to cite either 
 this github repository or the gnssrefl DOI, which is given just below.
 
 [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) 
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601494.svg)](http://dx.doi.org/10.5281/zenodo.5601494)
```

### Comparing `gnssrefl-3.1.5/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-3.2.0/gnssrefl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-3.2.0/gnssrefl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/pyproject.toml` & `gnssrefl-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.5/setup.py` & `gnssrefl-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "simplekml",
     "earthscope-sdk",
     "jupyterlab",
     "ipywidgets"
 ]
 setup(
     name="gnssrefl",
-    version="3.1.5",
+    version="3.2.0",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
```

### Comparing `gnssrefl-3.1.5/test/test_gps.py` & `gnssrefl-3.2.0/test/test_gps.py`

 * *Files identical despite different names*

