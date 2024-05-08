# Comparing `tmp/alcf-1.9.0.tar.gz` & `tmp/alcf-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alcf-1.9.0.tar", last modified: Fri May  3 16:29:07 2024, max compression
+gzip compressed data, was "alcf-2.0.0.tar", last modified: Wed May  8 13:57:50 2024, max compression
```

## Comparing `alcf-1.9.0.tar` & `alcf-2.0.0.tar`

### file list

```diff
@@ -1,203 +1,207 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.198509 alcf-1.9.0/
--rw-r--r--   0 peter     (1000) peter     (1000)      239 2024-05-03 16:23:18.000000 alcf-1.9.0/.editorconfig
--rw-r--r--   0 peter     (1000) peter     (1000)     1144 2024-05-03 16:23:18.000000 alcf-1.9.0/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)      181 2024-05-03 16:23:18.000000 alcf-1.9.0/MANIFEST.in
--rw-r--r--   0 peter     (1000) peter     (1000)     1275 2024-05-03 16:23:18.000000 alcf-1.9.0/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-05-03 16:29:07.198509 alcf-1.9.0/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      764 2024-05-03 16:23:18.000000 alcf-1.9.0/README.md
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf/
--rw-r--r--   0 peter     (1000) peter     (1000)      109 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf/algorithms/
--rw-r--r--   0 peter     (1000) peter     (1000)       27 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf/algorithms/calibration/
--rw-r--r--   0 peter     (1000) peter     (1000)       62 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/calibration/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      373 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/calibration/default.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf/algorithms/cloud_base_detection/
--rw-r--r--   0 peter     (1000) peter     (1000)       71 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/cloud_base_detection/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      930 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/cloud_base_detection/default.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf/algorithms/cloud_detection/
--rw-r--r--   0 peter     (1000) peter     (1000)       66 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/cloud_detection/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1533 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/cloud_detection/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1871 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/couple.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1018 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/interp.pyx
--rw-r--r--   0 peter     (1000) peter     (1000)      818 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/lidar_ratio.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf/algorithms/noise_removal/
--rw-r--r--   0 peter     (1000) peter     (1000)       64 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/noise_removal/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1366 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/noise_removal/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1808 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/output_sample.py
--rw-r--r--   0 peter     (1000) peter     (1000)    11260 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/stats.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1192 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/tsample.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1365 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/algorithms/zsample.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf/bin/
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/bin/__init__.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)      893 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/bin/alcf.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.178509 alcf-1.9.0/alcf/cmds/
--rw-r--r--   0 peter     (1000) peter     (1000)      458 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4022 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/auto.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.178509 alcf-1.9.0/alcf/cmds/auto_cmds/
--rw-r--r--   0 peter     (1000) peter     (1000)      141 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/auto_cmds/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      843 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/auto_cmds/compare.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2639 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/auto_cmds/lidar.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1086 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/auto_cmds/model.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2804 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/calibrate.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2148 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/compare.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4512 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/convert.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6399 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/download.py
--rw-r--r--   0 peter     (1000) peter     (1000)    12457 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/lidar.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1717 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/main.py
--rw-r--r--   0 peter     (1000) peter     (1000)     7093 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/model.py
--rw-r--r--   0 peter     (1000) peter     (1000)    19067 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/plot.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6987 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/simulate.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4993 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/cmds/stats.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.178509 alcf-1.9.0/alcf/download/
--rw-r--r--   0 peter     (1000) peter     (1000)       88 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/download/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2445 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/download/era5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2444 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/download/merra2.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.178509 alcf-1.9.0/alcf/fonts/
--rw-r--r--   0 peter     (1000) peter     (1000)     6709 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/fonts/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)    56032 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/fonts/PublicSans-Bold.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    60100 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/fonts/PublicSans-BoldItalic.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    60316 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/fonts/PublicSans-Italic.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    56792 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/fonts/PublicSans-Regular.otf
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.182509 alcf-1.9.0/alcf/lidars/
--rw-r--r--   0 peter     (1000) peter     (1000)     1456 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2136 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/blview.py
--rw-r--r--   0 peter     (1000) peter     (1000)      101 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/caliop.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1697 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/chm15k.py
--rw-r--r--   0 peter     (1000) peter     (1000)      410 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/cl31.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2409 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/cl51.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1820 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/cl61.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1018 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3791 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/mpl.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2150 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/lidars/mpl2nc.py
--rw-r--r--   0 peter     (1000) peter     (1000)     7005 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/misc.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.182509 alcf-1.9.0/alcf/models/
--rw-r--r--   0 peter     (1000) peter     (1000)     2265 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4350 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/amps.py
--rw-r--r--   0 peter     (1000) peter     (1000)      359 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/cmip5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2824 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/era5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2834 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/icon.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1814 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/icon_intake_healpix.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2881 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/jra55.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2213 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/merra2.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1885 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/nzcsm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3063 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/nzesm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2443 2024-05-03 16:23:18.000000 alcf-1.9.0/alcf/models/um.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.174509 alcf-1.9.0/alcf.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-05-03 16:29:07.000000 alcf-1.9.0/alcf.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     4676 2024-05-03 16:29:07.000000 alcf-1.9.0/alcf.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-05-03 16:29:07.000000 alcf-1.9.0/alcf.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       52 2024-05-03 16:29:07.000000 alcf-1.9.0/alcf.egg-info/entry_points.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-05-03 16:29:07.000000 alcf-1.9.0/alcf.egg-info/not-zip-safe
--rw-r--r--   0 peter     (1000) peter     (1000)      204 2024-05-03 16:29:07.000000 alcf-1.9.0/alcf.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        5 2024-05-03 16:29:07.000000 alcf-1.9.0/alcf.egg-info/top_level.txt
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1677 2024-05-03 16:23:18.000000 alcf-1.9.0/build_doc
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.186509 alcf-1.9.0/cosp/
--rw-r--r--   0 peter     (1000) peter     (1000)      260 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/.editorconfig
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.186509 alcf-1.9.0/cosp/MISR_simulator/
--rw-r--r--   0 peter     (1000) peter     (1000)    16546 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/MISR_simulator/MISR_simulator.f
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.186509 alcf-1.9.0/cosp/MODIS_simulator/
--rw-r--r--   0 peter     (1000) peter     (1000)    64835 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/MODIS_simulator/modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     7387 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/MODIS_simulator/test_modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5167 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)     7506 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/Makefile.cmor1
--rw-r--r--   0 peter     (1000) peter     (1000)     7515 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/Makefile.ibm
--rw-r--r--   0 peter     (1000) peter     (1000)      936 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/README.md
--rw-r--r--   0 peter     (1000) peter     (1000)    48320 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/README.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      467 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/README_v1.4.1.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.186509 alcf-1.9.0/cosp/actsim/
--rw-r--r--   0 peter     (1000) peter     (1000)    35248 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/actsim/lidar_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    38101 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/actsim/lmd_ipsl_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11672 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/actsim/mie_backscatter_1064.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11571 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/actsim/mie_backscatter_532.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11642 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/actsim/mie_backscatter_910.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.190509 alcf-1.9.0/cosp/cfmip2/
--rw-r--r--   0 peter     (1000) peter     (1000)     2508 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     2487 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     7271 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     7400 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     3320 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     3261 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    31979 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    15220 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_constants.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     1881 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_defs.h
--rw-r--r--   0 peter     (1000) peter     (1000)     2644 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_htfrtc.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     6934 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_input_nl.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    40704 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_io.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     4292 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_isccp_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     4123 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_lidar.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     3561 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_misr_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    25019 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     3646 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_output_nl.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    26091 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_rttov.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5694 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_rttov_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     9657 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    13744 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    70109 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_types.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    13287 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/cosp_utils.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.190509 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/
--rw-r--r--   0 peter     (1000) peter     (1000)     2957 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)    59127 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/README
--rw-r--r--   0 peter     (1000) peter     (1000)      165 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/congvec.expected
--rw-r--r--   0 peter     (1000) peter     (1000)     2545 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/congvec.f
--rw-r--r--   0 peter     (1000) peter     (1000)    43978 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/icarus.f
--rw-r--r--   0 peter     (1000) peter     (1000)      869 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/input.data
--rw-r--r--   0 peter     (1000) peter     (1000)     1042 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/input.data.halved
--rw-r--r--   0 peter     (1000) peter     (1000)    13495 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f
--rw-r--r--   0 peter     (1000) peter     (1000)     1845 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/license
--rwxr-xr-x   0 peter     (1000) peter     (1000)       15 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/rcsid
--rw-r--r--   0 peter     (1000) peter     (1000)    11849 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/scops.f
--rw-r--r--   0 peter     (1000) peter     (1000)     2539 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_congvec.f
--rwxr-xr-x   0 peter     (1000) peter     (1000)     2660 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh
--rw-r--r--   0 peter     (1000) peter     (1000)    13385 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f
--rwxr-xr-x   0 peter     (1000) peter     (1000)     3095 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.190509 alcf-1.9.0/cosp/llnl/
--rw-r--r--   0 peter     (1000) peter     (1000)     7918 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/llnl/cosp_radar.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     6082 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/llnl/llnl_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5703 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/llnl/pf_to_mr.f
--rw-r--r--   0 peter     (1000) peter     (1000)     9585 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/llnl/prec_scops.f
--rw-r--r--   0 peter     (1000) peter     (1000)    75040 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/mac_info.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     1317 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/predict_mom07.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.194509 alcf-1.9.0/cosp/quickbeam/
--rw-r--r--   0 peter     (1000) peter     (1000)     1563 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/README
--rw-r--r--   0 peter     (1000) peter     (1000)     4166 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/array_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     5500 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/atmos_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     7260 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/calc_Re.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    10671 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/dsd.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4282 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/format_input.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     7774 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/gases.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     1665 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/load_hydrometeor_classes.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     1761 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/load_mie_table.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     9299 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/math_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    17248 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/mrgrnk.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    36058 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/optics_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4211 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/predict_psd07.f
--rw-r--r--   0 peter     (1000) peter     (1000)    18284 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/radar_simulator.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4867 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/radar_simulator_init.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     2934 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/radar_simulator_types.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4039 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/scale_LUTs_io.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4852 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/quickbeam/zeff.f90
--rwxr-xr-x   0 peter     (1000) peter     (1000)      143 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/replace_tabs.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)      196 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/tests.sh
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.194509 alcf-1.9.0/cosp/utils/
--rwxr-xr-x   0 peter     (1000) peter     (1000)     8682 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/utils/COSP_plots.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)     3379 2023-04-22 09:28:05.000000 alcf-1.9.0/cosp/utils/append_cf3hr_files.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)      333 2024-05-03 16:23:18.000000 alcf-1.9.0/download_cosp
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.194509 alcf-1.9.0/man/
--rw-r--r--   0 peter     (1000) peter     (1000)     4583 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-auto.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2280 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-calibrate.1
--rw-r--r--   0 peter     (1000) peter     (1000)      811 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-compare.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2308 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-convert.1
--rw-r--r--   0 peter     (1000) peter     (1000)     5120 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-download.1
--rw-r--r--   0 peter     (1000) peter     (1000)     7022 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-lidar.1
--rw-r--r--   0 peter     (1000) peter     (1000)     4811 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-model.1
--rw-r--r--   0 peter     (1000) peter     (1000)     5666 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-plot.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1981 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-simulate.1
--rw-r--r--   0 peter     (1000) peter     (1000)     3944 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf-stats.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1450 2024-05-03 16:23:18.000000 alcf-1.9.0/man/alcf.1
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2024-05-03 16:29:07.198509 alcf-1.9.0/setup.cfg
--rwxr-xr-x   0 peter     (1000) peter     (1000)     2261 2024-05-03 16:23:18.000000 alcf-1.9.0/setup.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-03 16:29:07.198509 alcf-1.9.0/src/
--rw-r--r--   0 peter     (1000) peter     (1000)    12585 2024-05-03 16:23:18.000000 alcf-1.9.0/src/cosp_run.f03
--rw-r--r--   0 peter     (1000) peter     (1000)    11128 2024-05-03 16:23:18.000000 alcf-1.9.0/src/main.f03
--rw-r--r--   0 peter     (1000) peter     (1000)     8501 2024-05-03 16:23:18.000000 alcf-1.9.0/src/nc_utils.f03
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.904014 alcf-2.0.0/
+-rw-r--r--   0 peter     (1000) peter     (1000)      245 2024-05-08 13:55:39.000000 alcf-2.0.0/.editorconfig
+-rw-r--r--   0 peter     (1000) peter     (1000)     1144 2024-05-08 13:55:39.000000 alcf-2.0.0/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)      181 2024-05-08 13:55:39.000000 alcf-2.0.0/MANIFEST.in
+-rw-r--r--   0 peter     (1000) peter     (1000)     1275 2024-05-08 13:55:39.000000 alcf-2.0.0/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-05-08 13:57:50.904014 alcf-2.0.0/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      764 2024-05-08 13:55:39.000000 alcf-2.0.0/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.884014 alcf-2.0.0/alcf/
+-rw-r--r--   0 peter     (1000) peter     (1000)      109 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.888014 alcf-2.0.0/alcf/algorithms/
+-rw-r--r--   0 peter     (1000) peter     (1000)       27 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.888014 alcf-2.0.0/alcf/algorithms/calibration/
+-rw-r--r--   0 peter     (1000) peter     (1000)       62 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/calibration/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      373 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/calibration/default.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.888014 alcf-2.0.0/alcf/algorithms/cloud_base_detection/
+-rw-r--r--   0 peter     (1000) peter     (1000)       71 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/cloud_base_detection/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      907 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/cloud_base_detection/default.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.888014 alcf-2.0.0/alcf/algorithms/cloud_detection/
+-rw-r--r--   0 peter     (1000) peter     (1000)       66 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/cloud_detection/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1578 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/cloud_detection/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2029 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/couple.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.888014 alcf-2.0.0/alcf/algorithms/interp/
+-rw-r--r--   0 peter     (1000) peter     (1000)      447 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/interp/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      980 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/interp/area_block.pyx
+-rw-r--r--   0 peter     (1000) peter     (1000)     1931 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/interp/area_linear.pyx
+-rw-r--r--   0 peter     (1000) peter     (1000)      258 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/interp/linear.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      818 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/lidar_ratio.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.888014 alcf-2.0.0/alcf/algorithms/noise_removal/
+-rw-r--r--   0 peter     (1000) peter     (1000)       64 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/noise_removal/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1366 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/noise_removal/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1808 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/output_sample.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    11674 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/stats.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1192 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/tsample.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1479 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/algorithms/zsample.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.888014 alcf-2.0.0/alcf/bin/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/bin/__init__.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      893 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/bin/alcf.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.888014 alcf-2.0.0/alcf/cmds/
+-rw-r--r--   0 peter     (1000) peter     (1000)      458 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4022 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/auto.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.888014 alcf-2.0.0/alcf/cmds/auto_cmds/
+-rw-r--r--   0 peter     (1000) peter     (1000)      141 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/auto_cmds/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      843 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/auto_cmds/compare.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2639 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/auto_cmds/lidar.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1086 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/auto_cmds/model.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2804 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/calibrate.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2148 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/compare.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4512 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/convert.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6399 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/download.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    12966 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/lidar.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1717 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/main.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7117 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/model.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    19370 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/plot.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6987 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/simulate.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5297 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/cmds/stats.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.892014 alcf-2.0.0/alcf/download/
+-rw-r--r--   0 peter     (1000) peter     (1000)       88 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/download/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2445 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/download/era5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2444 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/download/merra2.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.892014 alcf-2.0.0/alcf/fonts/
+-rw-r--r--   0 peter     (1000) peter     (1000)     6709 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/fonts/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    56032 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/fonts/PublicSans-Bold.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    60100 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/fonts/PublicSans-BoldItalic.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    60316 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/fonts/PublicSans-Italic.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    56792 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/fonts/PublicSans-Regular.otf
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.892014 alcf-2.0.0/alcf/lidars/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1456 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/lidars/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2136 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/lidars/blview.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      101 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/lidars/caliop.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1697 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/lidars/chm15k.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      410 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/lidars/cl31.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2409 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/lidars/cl51.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1820 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/lidars/cl61.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1018 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/lidars/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3791 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/lidars/mpl.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2150 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/lidars/mpl2nc.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7005 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/misc.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.892014 alcf-2.0.0/alcf/models/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2265 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/models/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4350 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/models/amps.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      359 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/models/cmip5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2824 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/models/era5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2834 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/models/icon.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1814 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/models/icon_intake_healpix.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2881 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/models/jra55.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2213 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/models/merra2.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1885 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/models/nzcsm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3063 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/models/nzesm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2443 2024-05-08 13:55:39.000000 alcf-2.0.0/alcf/models/um.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.884014 alcf-2.0.0/alcf.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-05-08 13:57:50.000000 alcf-2.0.0/alcf.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     4794 2024-05-08 13:57:50.000000 alcf-2.0.0/alcf.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-05-08 13:57:50.000000 alcf-2.0.0/alcf.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       52 2024-05-08 13:57:50.000000 alcf-2.0.0/alcf.egg-info/entry_points.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-05-08 13:57:50.000000 alcf-2.0.0/alcf.egg-info/not-zip-safe
+-rw-r--r--   0 peter     (1000) peter     (1000)      204 2024-05-08 13:57:50.000000 alcf-2.0.0/alcf.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        5 2024-05-08 13:57:50.000000 alcf-2.0.0/alcf.egg-info/top_level.txt
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1677 2024-05-08 13:55:39.000000 alcf-2.0.0/build_doc
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.896014 alcf-2.0.0/cosp/
+-rw-r--r--   0 peter     (1000) peter     (1000)      260 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/.editorconfig
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.896014 alcf-2.0.0/cosp/MISR_simulator/
+-rw-r--r--   0 peter     (1000) peter     (1000)    16546 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/MISR_simulator/MISR_simulator.f
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.896014 alcf-2.0.0/cosp/MODIS_simulator/
+-rw-r--r--   0 peter     (1000) peter     (1000)    64835 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/MODIS_simulator/modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7387 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/MODIS_simulator/test_modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5167 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)     7506 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/Makefile.cmor1
+-rw-r--r--   0 peter     (1000) peter     (1000)     7515 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/Makefile.ibm
+-rw-r--r--   0 peter     (1000) peter     (1000)      936 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/README.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    48320 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/README.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      467 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/README_v1.4.1.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.900014 alcf-2.0.0/cosp/actsim/
+-rw-r--r--   0 peter     (1000) peter     (1000)    35248 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/actsim/lidar_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    38101 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/actsim/lmd_ipsl_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11672 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/actsim/mie_backscatter_1064.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11571 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/actsim/mie_backscatter_532.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11642 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/actsim/mie_backscatter_910.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.900014 alcf-2.0.0/cosp/cfmip2/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2508 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     2487 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     7271 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     7400 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     3320 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     3261 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    31979 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    15220 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_constants.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1881 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_defs.h
+-rw-r--r--   0 peter     (1000) peter     (1000)     2644 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_htfrtc.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     6934 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_input_nl.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    40704 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_io.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4292 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_isccp_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4123 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_lidar.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     3561 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_misr_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    25019 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     3646 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_output_nl.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    26091 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_rttov.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5694 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_rttov_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     9657 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    13744 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    70109 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_types.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    13287 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/cosp_utils.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.900014 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2957 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)    59127 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/README
+-rw-r--r--   0 peter     (1000) peter     (1000)      165 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/congvec.expected
+-rw-r--r--   0 peter     (1000) peter     (1000)     2545 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/congvec.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    43978 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/icarus.f
+-rw-r--r--   0 peter     (1000) peter     (1000)      869 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/input.data
+-rw-r--r--   0 peter     (1000) peter     (1000)     1042 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/input.data.halved
+-rw-r--r--   0 peter     (1000) peter     (1000)    13495 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     1845 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/license
+-rwxr-xr-x   0 peter     (1000) peter     (1000)       15 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/rcsid
+-rw-r--r--   0 peter     (1000) peter     (1000)    11849 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/scops.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     2539 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/test_congvec.f
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     2660 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh
+-rw-r--r--   0 peter     (1000) peter     (1000)    13385 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     3095 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.900014 alcf-2.0.0/cosp/llnl/
+-rw-r--r--   0 peter     (1000) peter     (1000)     7918 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/llnl/cosp_radar.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     6082 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/llnl/llnl_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5703 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/llnl/pf_to_mr.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     9585 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/llnl/prec_scops.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    75040 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/mac_info.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     1317 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/predict_mom07.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.904014 alcf-2.0.0/cosp/quickbeam/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1563 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/README
+-rw-r--r--   0 peter     (1000) peter     (1000)     4166 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/array_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5500 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/atmos_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7260 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/calc_Re.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    10671 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/dsd.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4282 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/format_input.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7774 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/gases.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1665 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/load_hydrometeor_classes.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1761 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/load_mie_table.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     9299 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/math_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    17248 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/mrgrnk.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    36058 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/optics_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4211 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/predict_psd07.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    18284 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/radar_simulator.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4867 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/radar_simulator_init.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     2934 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/radar_simulator_types.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4039 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/scale_LUTs_io.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4852 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/quickbeam/zeff.f90
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      143 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/replace_tabs.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      196 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/tests.sh
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.904014 alcf-2.0.0/cosp/utils/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     8682 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/utils/COSP_plots.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     3379 2023-04-22 09:28:05.000000 alcf-2.0.0/cosp/utils/append_cf3hr_files.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      333 2024-05-08 13:55:39.000000 alcf-2.0.0/download_cosp
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.904014 alcf-2.0.0/man/
+-rw-r--r--   0 peter     (1000) peter     (1000)     4581 2024-05-08 13:55:39.000000 alcf-2.0.0/man/alcf-auto.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2278 2024-05-08 13:55:39.000000 alcf-2.0.0/man/alcf-calibrate.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      809 2024-05-08 13:55:39.000000 alcf-2.0.0/man/alcf-compare.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2306 2024-05-08 13:55:39.000000 alcf-2.0.0/man/alcf-convert.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     5118 2024-05-08 13:55:39.000000 alcf-2.0.0/man/alcf-download.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     7283 2024-05-08 13:55:39.000000 alcf-2.0.0/man/alcf-lidar.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     4822 2024-05-08 13:55:39.000000 alcf-2.0.0/man/alcf-model.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     5927 2024-05-08 13:55:39.000000 alcf-2.0.0/man/alcf-plot.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1979 2024-05-08 13:55:39.000000 alcf-2.0.0/man/alcf-simulate.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     4205 2024-05-08 13:55:39.000000 alcf-2.0.0/man/alcf-stats.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1668 2024-05-08 13:55:39.000000 alcf-2.0.0/man/alcf.1
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2024-05-08 13:57:50.904014 alcf-2.0.0/setup.cfg
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     2427 2024-05-08 13:55:39.000000 alcf-2.0.0/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-08 13:57:50.904014 alcf-2.0.0/src/
+-rw-r--r--   0 peter     (1000) peter     (1000)    12585 2024-05-08 13:55:39.000000 alcf-2.0.0/src/cosp_run.f03
+-rw-r--r--   0 peter     (1000) peter     (1000)    11128 2024-05-08 13:55:39.000000 alcf-2.0.0/src/main.f03
+-rw-r--r--   0 peter     (1000) peter     (1000)     8501 2024-05-08 13:55:39.000000 alcf-2.0.0/src/nc_utils.f03
```

### Comparing `alcf-1.9.0/LICENSE.md` & `alcf-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/Makefile` & `alcf-2.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/PKG-INFO` & `alcf-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alcf
-Version: 1.9.0
+Version: 2.0.0
 Summary: Automatic Lidar and Ceilometer Framework (ALCF)
 Home-page: https://alcf.peterkuma.net
 Author: Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn
 Author-email: peter@peterkuma.net
 License: MIT
 Keywords: alc,ceilometer,lidar,atmosphere,model,simulator,nwp,gcm,cosp,actsim,vaisala,cl51,cl31,lufft,chm-15k,minimpl,amps,merra-2,um
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alcf-1.9.0/README.md` & `alcf-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/algorithms/cloud_base_detection/default.py` & `alcf-2.0.0/alcf/algorithms/cloud_base_detection/default.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 		dims = (n,)
 		dimnames = ('time',)
 	cbh = np.zeros(dims, dtype=np.float64)
 	for i in range(n):
 		for j in range(l):
 			x = cloud_mask[i,:,j] if len(dims) == 2 \
 				else cloud_mask[i,:]
-			kk = np.where(x)[0]
-			if len(kk) > 0:
-				if len(dims) == 2:
-					cbh[i,j] = d['zfull'][kk[0]]
-				else:
-					cbh[i] = d['zfull'][kk[0]]
+			kk = np.where(x == 1)[0]
+			if np.any(np.isnan(x)):
+				v = np.nan
+			elif len(kk) > 0:
+				v = d['zfull'][kk[0]]
 			else:
-				if len(dims) == 2:
-					cbh[i,j] = np.inf
-				else:
-					cbh[i] = np.inf
+				v = np.inf
+			if len(dims) == 2:
+				cbh[i,j] = v
+			else:
+				cbh[i] = v
 	d['cbh'] = cbh
 	d['.']['cbh'] = {
 		'.dims': dimnames,
 		'long_name': 'cloud base height',
 		'units': 'm',
 	}
```

### Comparing `alcf-1.9.0/alcf/algorithms/cloud_detection/default.py` & `alcf-2.0.0/alcf/algorithms/cloud_detection/default.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,29 +38,30 @@
 	if bmol is not None:
 		if len(x.shape) == 3:
 			for i in range(x.shape[2]):
 				x[:,:,i] -= bmol
 		else:
 			x -= bmol
 
-	cloud_mask = np.zeros(x.shape, np.byte)
+	cloud_mask = np.full(x.shape, np.nan, np.float64)
 	if cloud_threshold_exp is not None:
 		ct_x, ct_y, ct_h = cloud_threshold_exp
 		for i in range(n):
 			alt = 0 if np.isnan(d['altitude'][i]) else d['altitude'][i]
 			height = d['zfull'] - alt
 			height[height < 0] = 0
 			ct = ct_y + (ct_x - ct_y)*0.5**(height/ct_h)
 			if x.ndim == 3:
 				for k in range(l):
 					cloud_mask[i,:,k] = x[i,:,k] >= ct
 			else:
 				cloud_mask[i,:] = x[i,:] >= ct
 	else:
 		cloud_mask[::] = x >= cloud_threshold
+		cloud_mask[np.isnan(x)] = np.nan
 
 	d['cloud_mask'] = cloud_mask
 	d['.']['cloud_mask'] = {
 		'.dims': d['.']['backscatter']['.dims'],
 		'long_name': 'cloud mask',
 		'units': '1',
 	}
```

### Comparing `alcf-1.9.0/alcf/algorithms/couple.py` & `alcf-2.0.0/alcf/algorithms/couple.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import copy
 import numpy as np
 import ds_format as ds
 import aquarius_time as aq
-from alcf import misc
-from alcf.algorithms import interp
+from alcf import misc, algorithms
 
 VARIABLES = [
 	'zfull',
 	'backscatter_sd',
 	'backscatter_mol',
 ]
 
-def couple(d, d_idx):
+def couple(d, d_idx, interp=None):
 	dims = d['backscatter'].shape
 	n = dims[0]
 	l = dims[2] if len(dims) == 3 else 0
 	couple_bsd = False
 	couple_bmol = False
 	if 'backscatter_sd' not in d:
 		couple_bsd = True
@@ -43,23 +42,33 @@
 		i1 = d_idx['i'][j]
 		d1 = ds.read(filename, VARIABLES, {'time': i1})
 		zhalf1 = misc.half(d1['zfull'])
 		zhalf = misc.half(d['zfull'][i,:]) \
 			if d['zfull'].ndim == 2 \
 			else misc.half(d['zfull'])
 		if couple_bsd and 'backscatter_sd' in d1:
-			b_sd = interp(zhalf1, d1['backscatter_sd'], zhalf)
+			b_sd = algorithms.interp(
+				interp,
+				d1['zfull'], zhalf1,
+				d1['backscatter_sd'],
+				d['zfull'][i,:], zhalf
+			)
 			if len(dims) == 3:
 				for k in range(l):
 					d['backscatter_sd'][i,:,k] = b_sd
 			else:
 				d['backscatter_sd'][i,:] = b_sd
 		if couple_bmol and 'backscatter_mol' in d1:
-			b_mol = interp(zhalf1, d1['backscatter_mol'], zhalf)
+			b_mol = algorithms.interp(
+				interp,
+				d1['zfull'], zhalf1,
+				d1['backscatter_mol'],
+				d['zfull'][i,:], zhalf
+			)
 			d['backscatter_mol'][i,:] = b_mol
 
-def stream(dd, state, dirname):
+def stream(dd, state, dirname, interp=None):
 	if 'd_idx' not in state:
 		d_idx = ds.readdir(dirname, ['time'], merge='time')
 		state['d_idx'] = d_idx
-	return misc.stream(dd, state, couple, d_idx=state['d_idx'])
+	return misc.stream(dd, state, couple, d_idx=state['d_idx'], interp=interp)
```

### Comparing `alcf-1.9.0/alcf/algorithms/interp.pyx` & `alcf-2.0.0/alcf/algorithms/interp/area_block.pyx`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 cimport cython
 cimport numpy as np
 import numpy as np
+from libc.math cimport isnan
 
 def interp(
+	np.ndarray[double, ndim=1] x not None,
 	np.ndarray[double, ndim=1] xhalf not None,
 	np.ndarray[double, ndim=1] y not None,
+	np.ndarray[double, ndim=1] x2 not None,
 	np.ndarray[double, ndim=1] xhalf2 not None
 ):
-	'''Interpolate y(x) on x2'''
-	cdef long n = len(xhalf)
-	cdef long n2 = len(xhalf2)
-	cdef np.ndarray[double, ndim=1] y2 = np.zeros(n2-1, dtype=np.float64)
+	cdef long n = len(x)
+	cdef long n2 = len(x2)
+	cdef np.ndarray[double, ndim=1] y2 = np.full(n2, np.nan, dtype=np.float64)
 	cdef long i = 0
 	cdef long i2 = 0
 	cdef double dx = 0
-	cdef double dx2 = 0
-	while i < n-1 and xhalf[i] < xhalf2[0]:
+	cdef double dxtot = 0
+	cdef double a = 0
+	cdef double b = 0
+	while i < n and xhalf[i+1] < xhalf2[0]:
 		i += 1
-	if xhalf[i] < xhalf2[0]:
+	if i == n:
 		return y2
-	if i > 0:
-		i -= 1
-	while i2 < n2-1 and xhalf2[i2] < xhalf[-1]:
-		dx2 = 0
-		while i < n-1 and xhalf[i+1] < xhalf2[i2+1]:
-			dx = xhalf[i+1] - max(xhalf2[i2], xhalf[i])
-			if dx < 0:
-				raise ValueError(xhalf[i+1], xhalf2[i2], xhalf[i])
-			y2[i2] += y[i]*dx
-			dx2 += dx
+	while i2 < n2 and xhalf2[i2] < xhalf[-1]:
+		dxtot = 0
+		while i < n and xhalf[i] < xhalf2[i2+1]:
+			a = max(xhalf[i], xhalf2[i2])
+			b = min(xhalf[i+1], xhalf2[i2+1])
+			dx = b - a
+			if dx > 0:
+				if isnan(y2[i2]):
+					y2[i2] = 0
+				y2[i2] += y[i]*dx
+				dxtot += dx
 			i += 1
-		if i < n-1 and xhalf[i] < xhalf2[i2+1]:
-			dx = xhalf2[i2+1] - max(xhalf2[i2], xhalf[i])
-			if dx < 0:
-				raise ValueError(i, i2)
-			y2[i2] += y[i]*dx
-			dx2 += dx
-		if dx2 > 0:
-			y2[i2] /= dx2
+		if i > 0:
+			i -= 1
+		if dxtot > 0:
+			y2[i2] /= dxtot
 		i2 += 1
 	return y2
```

### Comparing `alcf-1.9.0/alcf/algorithms/lidar_ratio.py` & `alcf-2.0.0/alcf/algorithms/lidar_ratio.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/algorithms/noise_removal/default.py` & `alcf-2.0.0/alcf/algorithms/noise_removal/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/algorithms/output_sample.py` & `alcf-2.0.0/alcf/algorithms/output_sample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/algorithms/stats.py` & `alcf-2.0.0/alcf/algorithms/stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
-from alcf.algorithms import interp
-from alcf import misc
+from alcf import misc, algorithms
 
 def calc_filter_mask(filters, time, l):
 	n = len(time)
 	if len(filters) == 0:
 		filter_mask = np.zeros(n, dtype=bool)
 	else:
 		filter_mask = np.ones(n, dtype=bool)
@@ -27,14 +26,15 @@
 	bsd_res=None,
 	bsd_z=None,
 	filter=None,
 	filters_exclude=None,
 	filters_include=None,
 	zlim=None,
 	zres=None,
+	interp='area_block',
 	**kwargs
 ):
 	if zlim is not None and zres is not None:
 		state['zfull2'] = state.get('zfull2',
 			np.arange(zlim[0] + 0.5*zres, zlim[1], zres)
 		)
 	else:
@@ -171,24 +171,26 @@
 			state['backscatter_sd_hist'] += np.histogram(
 				d['backscatter_sd'][filter_mask & mask,jsd],
 				bins=state['backscatter_sd_half'])[0]
 
 	for i in range(o):
 		if l > 0:
 			for k in range(l):
-				state['backscatter_hist'][i,:,k] += interp(
-					zhalf,
+				state['backscatter_hist'][i,:,k] += algorithms.interp(
+					interp,
+					d['zfull'], zhalf,
 					backscatter_hist_tmp[i,:,k],
-					zhalf2
+					state['zfull2'], zhalf2
 				)
 		else:
-			state['backscatter_hist'][i,:] += interp(
-				zhalf,
+			state['backscatter_hist'][i,:] += algorithms.interp(
+				interp,
+				d['zfull'], zhalf,
 				backscatter_hist_tmp[i,:],
-				zhalf2
+				state['zfull2'], zhalf2
 			)
 	for i in range(n):
 		if not mask[i]:
 			continue
 		if l > 0:
 			for k in range(l):
 				if not filter_mask[i,k]:
@@ -216,44 +218,50 @@
 				backscatter_mol_avg_tmp[:] += d['backscatter_mol'][i,:]
 			state['n'] += 1
 			state['time_total'] += \
 				24*60*60*(d['time_bnds'][i,1] - d['time_bnds'][i,0])
 			state['clt'] += np.any(d['cloud_mask'][i,:])
 	if l > 0:
 		for k in range(l):
-			state['cl'][:,k] += interp(
-				zhalf,
+			state['cl'][:,k] += algorithms.interp(
+				interp,
+				d['zfull'], zhalf,
 				cl_tmp[:,k],
-				zhalf2
+				state['zfull2'], zhalf2
 			)
-			state['backscatter_avg'][:,k] += interp(
-				zhalf,
+			state['backscatter_avg'][:,k] += algorithms.interp(
+				interp,
+				d['zfull'], zhalf,
 				backscatter_avg_tmp[:,k],
-				zhalf2
+				state['zfull2'], zhalf2
 			)
-			state['backscatter_mol_avg'][:,k] += interp(
-				zhalf,
+			state['backscatter_mol_avg'][:,k] += algorithms.interp(
+				interp,
+				d['zfull'], zhalf,
 				backscatter_mol_avg_tmp[:,k],
-				zhalf2
+				state['zfull2'], zhalf2
 			)
 	else:
-		state['cl'] += interp(
-			zhalf,
+		state['cl'] += algorithms.interp(
+			interp,
+			d['zfull'], zhalf,
 			cl_tmp,
-			zhalf2
+			state['zfull2'], zhalf2
 		)
-		state['backscatter_avg'] += interp(
-			zhalf,
+		state['backscatter_avg'] += algorithms.interp(
+			interp,
+			d['zfull'], zhalf,
 			backscatter_avg_tmp,
-			zhalf2
+			state['zfull2'], zhalf2
 		)
-		state['backscatter_mol_avg'] += interp(
-			zhalf,
+		state['backscatter_mol_avg'] += algorithms.interp(
+			interp,
+			d['zfull'], zhalf,
 			backscatter_mol_avg_tmp,
-			zhalf2
+			state['zfull2'], zhalf2
 		)
 
 def stats_reduce(state, bsd_z=None, **kwargs):
 	if not 'n' in state:
 		return {}
 	if len(state['cl'].shape) == 2:
 		for k in range(len(state['n'])):
@@ -264,21 +272,21 @@
 				state['cl'][:,k] /= state['n'][k]
 				state['clt'][k] /= state['n'][k]
 				state['backscatter_avg'][:,k] /= state['n'][k]
 				state['backscatter_mol_avg'][:,k] /= state['n'][k]
 	else:
 		if state['clt'] > 0:
 			state['cbh'] /= state['clt']
-		if state['n'] != 0:
+		if state['n'] > 0:
 			state['backscatter_hist'] /= state['n']
 			state['cl'] /= state['n']
 			state['clt'] /= state['n']
 			state['backscatter_avg'] /= state['n']
 			state['backscatter_mol_avg'] /= state['n']
-	state['backscatter_sd_hist'] /= state['n']
+			state['backscatter_sd_hist'] /= state['n']
 	do = {
 		'cl': 100.*state['cl'],
 		'cbh': 100.*state['cbh'],
 		'clt': 100.*state['clt'],
 		'zfull': state['zfull2'],
 		'n': state['n'],
 		'time_total': state['time_total'],
```

### Comparing `alcf-1.9.0/alcf/algorithms/tsample.py` & `alcf-2.0.0/alcf/algorithms/tsample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/algorithms/zsample.py` & `alcf-2.0.0/alcf/algorithms/zsample.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import ds_format as ds
-from alcf import misc
-from alcf.algorithms import interp
+from alcf import misc, algorithms
 
-def zsample(d, zres=None, zlim=None):
+def zsample(d, zres=None, zlim=None, interp=None):
 	n = ds.dim(d, 'time')
 	m = ds.dim(d, 'level')
 	l = ds.dim(d, 'column')
 	if m == 0:
 		return
 
 	zfull = d['zfull']
@@ -34,19 +33,24 @@
 		shape2[1] = m2
 		l = shape2[2]
 		x2 = np.zeros(shape2, dtype=x.dtype)
 		if var == 'backscatter_sd':
 			x = x**2
 		for i2 in range(n):
 			for j2 in range(l):
-				x2[i2,:,j2] = interp(zhalf[i2,:], x[i2,:,j2], zhalf2)
+				x2[i2,:,j2] = algorithms.interp(
+					interp,
+					zfull[i2,:] if zfull.ndim == 2 else zfull, zhalf[i2,:],
+					x[i2,:,j2],
+					zfull2, zhalf2
+				)
 		if var == 'backscatter_sd':
 			x2 = np.sqrt(x2)
 		x2 = x2.reshape([n, m2] + shape[2:])
 		x2 = np.moveaxis(x2, [0, 1], [i, j])
 		ds.var(d, var, x2)
 
 	ds.var(d, 'zfull', zfull2)
 	ds.dims(d, 'zfull', ['level'])
 
-def stream(dd, state, zres=None, zlim=None, **options):
-	return misc.stream(dd, state, zsample, zres=zres, zlim=zlim)
+def stream(dd, state, zres=None, zlim=None, interp=None, **options):
+	return misc.stream(dd, state, zsample, zres=zres, zlim=zlim, interp=interp)
```

### Comparing `alcf-1.9.0/alcf/bin/alcf.py` & `alcf-2.0.0/alcf/bin/alcf.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/cmds/auto.py` & `alcf-2.0.0/alcf/cmds/auto.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/cmds/auto_cmds/compare.py` & `alcf-2.0.0/alcf/cmds/auto_cmds/compare.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/cmds/auto_cmds/lidar.py` & `alcf-2.0.0/alcf/cmds/auto_cmds/lidar.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/cmds/auto_cmds/model.py` & `alcf-2.0.0/alcf/cmds/auto_cmds/model.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/cmds/calibrate.py` & `alcf-2.0.0/alcf/cmds/calibrate.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/cmds/compare.py` & `alcf-2.0.0/alcf/cmds/compare.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/cmds/convert.py` & `alcf-2.0.0/alcf/cmds/convert.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/cmds/download.py` & `alcf-2.0.0/alcf/cmds/download.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/cmds/lidar.py` & `alcf-2.0.0/alcf/cmds/lidar.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,24 @@
 	'time_bnds',
 	'zfull',
 	'altitude',
 	'lon',
 	'lat',
 ]
 
+REQ_VARIABLES = [
+	'backscatter',
+	'time',
+	'time_bnds',
+	'zfull',
+	'altitude',
+	'lon',
+	'lat',
+]
+
 def read_calibration_file(filename):
 	with open(filename, 'rb') as f:
 		return pst.decode(f.read())
 
 def run(type_, input_, output,
 	altitude=None,
 	tres=300,
@@ -50,14 +60,15 @@
 	cl_crit_range=6000,
 	lat=None,
 	lon=None,
 	r=False,
 	keep_vars=[],
 	align_output=True,
 	debug=False,
+	interp='area_block',
 	**options
 ):
 	"""
 alcf-lidar -- Process lidar data.
 ==========
 
 Synopsis
@@ -111,14 +122,15 @@
 - `bsd_z: <value>`: Height at which `bsd` applies (m). Default: `8000`.
 - `calibration: <algorithm>`: Backscatter calibration algorithm. Available algorithms: `default`, `none`. Default: `default`.
 - `couple: <directory>`: Couple to other lidar data. Default: `none`.
 - `cl_crit_range: <range>`: Critical range for the `fix_cl_range` option (m). Default: 6000.
 - `cloud_detection: <algorithm>`: Cloud detection algorithm. Available algorithms: `default`, `none`. Default: `default`.
 - `cloud_base_detection: <algorithm>`: Cloud base detection algorithm. Available algorithms: `default`, `none`. Default: `default`.
 - `--fix_cl_range`: Fix CL31/CL51 range correction (if `noise_h2` firmware option if off). The critical range is taken from `cl_crit_range`.
+- `interp: <value>`: Vertical interpolation method. `area_block` for area-weighting with block interpolation, `area_linear` for area-weighting with linear interpolation or `linear` for simple linear interpolation. Default: `area_block`.
 - `keep_vars: { <var>... }`: Keep the listed input variables. The variable must be numerical and have a time dimension. The variable is resampled in the same way as backscatter along their time and level dimensions, its name is prefixed with `input_`, and its type is changed to float64. Default: `{ }`.
 - `lat: <lat>`: Latitude of the instrument (degrees North). Default: Taken from lidar data or `none` if not available.
 - `lon: <lon>`: Longitude of the instrument (degrees East). Default: Taken from lidar data or `none` if not available.
 - `noise_removal: <algorithm>`: Noise removal algorithm. Available algorithms: `default`, `none`.  Default: `default`.
 - `output_sampling: <period>`: Output sampling period (seconds). Default: `86400` (24 hours).
 - `-r`: Process the input directory recursively.
 - `time: { <low> <high> }`: Time limits (see Time format below). Default: `none`.
@@ -237,14 +249,18 @@
 		print('-> %s' % filename)
 		return []
 
 	def output_stream(dd, state, output_sampling=None, **options):
 		return misc.stream(dd, state, write, output=output)
 
 	def preprocess(d, tshift=None):
+		misc.require_vars(d, REQ_VARIABLES)
+		for var in VARIABLES:
+			if var in d:
+				d[var] = d[var].astype(np.float64)
 		if tshift is not None:
 			d['time'] += tshift/86400.
 			d['time_bnds'] += tshift/86400.
 		return d
 
 	def process(dd, state, **options):
 		state['preprocess'] = state.get('preprocess', {})
@@ -257,24 +273,25 @@
 		state['cloud_detection'] = state.get('cloud_detection', {})
 		state['cloud_base_detection'] = state.get('cloud_base_detection', {})
 		state['lidar_ratio'] = state.get('lidar_ratio', {})
 		state['output'] = state.get('output', {})
 		state['couple'] = state.get('couple', {})
 		dd = misc.stream(dd, state['preprocess'], preprocess, tshift=tshift)
 		if couple is not None:
-			dd = couple_mod.stream(dd, state['couple'], couple)
+			dd = couple_mod.stream(dd, state['couple'], couple, interp=interp)
 		if noise_removal_mod is not None:
 			dd = noise_removal_mod.stream(dd, state['noise_removal'],
 				align=align_output,
 				**options
 			)
 		if calibration_mod is not None:
 			dd = calibration_mod.stream(dd, state['calibration'], **options)
 		if zres is not None or zlim is not None:
-			dd = zsample.stream(dd, state['zsample'], zres=zres, zlim=zlim)
+			dd = zsample.stream(dd, state['zsample'],
+				zres=zres, zlim=zlim, interp=interp)
 		if tres is not None or time is not None:
 			dd = tsample.stream(dd, state['tsample'],
 				tres=tres/86400.,
 				align=align_output
 			)
 		if output_sampling is not None:
 			dd = output_sample.stream(dd, state['output_sample'],
```

### Comparing `alcf-1.9.0/alcf/cmds/main.py` & `alcf-2.0.0/alcf/cmds/main.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/cmds/model.py` & `alcf-2.0.0/alcf/cmds/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 - `end`: End time (see Time format below).
 - `track: <file>`, `track: { <file>... }`: One or more track NetCDF files (see Files below). If multiple files are supplied and `time_bnds` is not present in the files, they are assumed to be multiple segments of a discontinous track unless the last and first time of adjacent tracks are the same.
 - `options`: See Options below.
 
 Options
 -------
 
-- `njobs: <n>`: Number of parallel jobs. Default: number of CPU cores.
+- `njobs: <n>`: Number of parallel jobs. Default: number of CPU cores capped to 16.
 - `-r`: Process the input directory recursively.
 - `--track_lon_180`: Expect track longitude between -180 and 180 degrees. This option is no longer needed as the conversion is automatically. [deprecated]
 - `override_year: <year>`: Override year in the track. Use if comparing observations with a model statistically and the model output does not have a corresponding year available. The observation time is converted to the same time relative to the start of the year in the specified year. Note that if the original year is a leap year and the override year is not, as a consequence of the above 31 December is mapped to 1 January. The output retains the original year as in the track, even though the model data come from the override year. Default: `none`.
 - `track_gap: <interval>`: If the interval is not 0, a track file is supplied, the `time_bnds` variable is not defined in the file and any two adjacent points are separated by more than the specified time interval (seconds), then a gap is assumed to be present between the two data points, instead of interpolating location between the two points. Default: `21600` (6 hours).
 
 Types
 -----
@@ -169,15 +169,16 @@
 	time_start = max(d_track['time_bnds'][0,0], time_lim[0])
 	time_end = min(d_track['time_bnds'][-1,1], time_lim[1])
 
 	model = MODELS.get(type_)
 	if model is None:
 		raise ValueError('Invalid type: %s' % type_)
 
-	if njobs is None: njobs = os.cpu_count()
+	if njobs is None:
+		njobs = min(16, os.cpu_count())
 
 	warnings = []
 	index = None
 	if hasattr(model, 'index'):
 		index = model.index(input_, warnings=warnings, recursive=r, njobs=njobs)
 
 	with ProcessPoolExecutor(max_workers=njobs) as ex:
```

### Comparing `alcf-1.9.0/alcf/cmds/plot.py` & `alcf-2.0.0/alcf/cmds/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 	sigma=5,
 	remove_bmol=True,
 	vlim=None,
 	vlog=None,
 	zres=50,
 	zlim=None,
 	render='antialiased',
+	interp='area_block',
 	**opts
 ):
 	if plot_type == 'backscatter':
 		misc.require_vars(d, ['time', 'zfull', 'backscatter', 'cloud_mask'])
 		cmap = copy.copy(mpl.colormaps.get_cmap('viridis'))
 		under = '#222222'
 		label = 'Att. vol. backscattering coef. (×10$^{-6}$ m$^{-1}$sr$^{-1}$)'
@@ -146,15 +147,18 @@
 			zlim = [np.min(d['zfull']), np.max(d['zfull'])]
 		zhalf = np.arange(zlim[0], zlim[1] + zres, zres)
 		zfull = 0.5*(zhalf[1:] + zhalf[:-1])
 		xp = np.full((x.shape[0], len(zfull)), np.nan, np.float64)
 		for i in range(xp.shape[0]):
 			zhalfi = misc.half(d['zfull'][i,:])
 			xp[i,:] = algorithms.interp(
-				zhalfi, x[i,:], zhalf
+				interp,
+				d['zfull'][i,:], zhalfi,
+				x[i,:],
+				zfull, zhalf
 			)
 		x = xp
 	else:
 		raise ValueError('Invalid plot type "%s"' % plot_type)
 
 	if vlog:
 		norm = LogNorm(vlim[0], vlim[1])
@@ -526,24 +530,25 @@
 
 General options
 ---------------
 
 - `dpi: <value>`: Resolution in dots per inch (DPI). Default: `300`.
 - `--grid`: Plot grid.
 - `height: <value>`: Plot height (inches). Default: `5` if `plot_type` is `cloud_occurrence` or `backscatter_hist` else `4`.
+- `interp: <value>`: Vertical interpolation method. `area_block` for area-weighting with block interpolation, `area_linear` for area-weighting with linear interpolation or `linear` for simple linear interpolation. Default: `area_block`.
+- `render: <value>`: Render profiles anti-aliased (`antialiased`) or standard (`standard`). Standard is more suitable for short time intervals. Default: `antialiased`.
 - `subcolumn: <value>`: Model subcolumn to plot. Default: `0`.
 - `title: <value>`: Plot title.
 - `width: <value>`: Plot width (inches). Default: `5` if `plot_type` is `cloud_occurrence` or `backscatter_hist` else `10`.
-- `render: <value>`: Render profiles anti-aliased (`antialiased`) or standard (`standard`). Standard is more suitable for short time intervals. Default: `antialiased`.
 
 backscatter options
 -------------------
 
-- `lr: <value>`: Plot effective lidar ratio. Default: `true`.
 - `cloud_mask: <value>`: Plot cloud mask. Default: `true`.
+- `lr: <value>`: Plot effective lidar ratio. Default: `true`.
 - `remove_bmol: <value>`: Remove molecular backscatter (observed data have to be coupled with model data via the `couple` option of `alcf lidar`). Default: `true`.
 - `sigma: <value>`: Remove of number of standard deviations of backscatter from the mean backscatter (real). Default: `5`.
 - `vlim: { <min> <max }`: Value limits (10^-6 m-1.sr-1). Default: `{ 0.1 200 }`.
 - `vlog: <value>`: Plot values on logarithmic scale: `true` of `false`. Default: `true`.
 
 backscatter_hist options
 ------------------------
@@ -573,16 +578,16 @@
 - `vlog: <value>`: Plot values on logarithmic scale: `true` of `false`. Default: `true`.
 - `zres: <zres>`: Height resolution (m). Default: `50`.
 
 cbh and cloud_occurrence options
 --------------------------------
 
 - `colors: { <value>... }`: Line colors. Default: `{ #0084c8 #dc0000 #009100 #ffc022 #ba00ff }`
-- `linestyle: { <value> ... }`: Line style (`solid`, `dashed`, `dotted`). Default: `solid`.
 - `labels: { <value>... }`: Line labels. Default: `none`.
+- `linestyle: { <value> ... }`: Line style (`solid`, `dashed`, `dotted`). Default: `solid`.
 - `lw: <value>`: Line width. Default: `1`.
 - `xlim: { <min> <max> }`: x axis limits (%). Default: `{ 0 100 }`.
 - `zlim: { <min> <max> }`: z axis limits (m). Default: `{ 0 15 }`.
 
 Examples
 --------
```

### Comparing `alcf-1.9.0/alcf/cmds/simulate.py` & `alcf-2.0.0/alcf/cmds/simulate.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/cmds/stats.py` & `alcf-2.0.0/alcf/cmds/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import sys
 import numpy as np
 import ds_format as ds
 import alcf
-from alcf.algorithms import interp
 from alcf.algorithms import stats
-from alcf.misc import parse_time
+from alcf import misc
 
 VARIABLES = [
 	'cloud_mask',
 	'cbh',
 	'zfull',
 	'time',
 	'time_bnds',
@@ -35,14 +34,15 @@
 	bsd_res=0.001,
 	bsd_z=8000.,
 	filter=None,
 	filter_exclude=None,
 	filter_include=None,
 	zlim=[0., 15000.],
 	zres=100.,
+	interp='area_block',
 	**kwargs
 ):
 	'''
 alcf-stats -- Calculate cloud occurrence statistics.
 ==========
 
 Synopsis
@@ -69,14 +69,15 @@
 - `bsd_lim: { <low> <high> }`: Backscatter standard deviation histogram limits (10^-6 m-1.sr-1). Default: `{ 0.001 10 }`.
 - `bsd_log: <value>`: Enable/disable logarithmic scale of the backscatter standard deviation histogram (`true` or `false`). Default: `true`.
 - `bsd_res: <value>`: Backscatter standard deviation histogram resolution (10^-6 m-1.sr-1). Default: `0.001`.
 - `bsd_z: <value>`: Backscatter standard deviation histogram height (m). Default: `8000`.
 - `filter: <value> | { <value> ... }`: Filter profiles by condition: `cloudy` for cloudy profiles only, `clear` for clear sky profiles only, `night` for nighttime profiles, `day` for daytime profiles, `none` for all profiles. If an array of values is supplied, all conditions must be true. For `night` and `day`, lidar profiles must contain valid longitude and latitude fields set via the `lon` and `lat` arguments of `alcf lidar` or read implicitly from raw lidar data files if available (mpl, mpl2nc). Default: `none`.
 - `filter_exclude: <value> | { <value>... }`: Filter by a mask defined in a NetCDF file, described below under Filter file. If multiple files are supplied, they must all apply for a profile to be excluded.
 - `filter_include: <value> | { <value>... }`: The same as `filter_exclude`, but with time intervals to be included in the result. If both are defined, `filter_include` takes precedence. If multiple files are supplied, they must all apply for a profile to be included.
+- `interp: <value>`: Vertical interpolation method. `area_block` for area-weighting with block interpolation, `area_linear` for area-weighting with linear interpolation or `linear` for simple linear interpolation. Default: `area_block`.
 - `tlim: { <start> <end> }`: Time limits (see Time format below). Default: `none`.
 - `zlim: { <low> <high> }`: Height limits (m). Default: `{ 0 15000 }`.
 - `zres: <value>`: Height resolution (m). Default: `50`.
 
 Time format
 -----------
 
@@ -90,27 +91,28 @@
 Examples
 --------
 
 Calculate statistics from processed lidar data in `alcf_cl51_lidar` and store the output in `alcf_cl51_stats.nc`.
 
     alcf stats alcf_cl51_lidar alcf_cl51_stats.nc
 	'''
-	tlim_jd = parse_time(tlim) if tlim is not None else None
+	tlim_jd = misc.parse_time(tlim) if tlim is not None else None
 	state = {}
 	options = {
 		'tlim': tlim_jd,
 		'blim': np.array(blim, dtype=np.float64)*1e-6,
 		'bres': bres*1e-6,
 		'bsd_lim': np.array(bsd_lim, dtype=np.float64)*1e-6,
 		'bsd_log': bsd_log,
 		'bsd_res': bsd_res*1e-6,
 		'bsd_z': bsd_z,
 		'filter': filter if type(filter) is list else [filter],
 		'zlim': zlim,
 		'zres': zres,
+		'interp': interp,
 	}
 
 	if filter_exclude is not None:
 		dd = read_filters(filter_exclude)
 		options['filters_exclude'] = [d['time_bnds'] for d in dd]
 
 	if filter_include is not None:
@@ -127,10 +129,13 @@
 			print('<- %s' % filename)
 			dd = stats.stream([d], state, **options)
 	else:
 		d = ds.read(input_, VARIABLES)
 		print('<- %s' % input_)
 		dd = stats.stream([d], state, **options)
 	dd = stats.stream([None], state, **options)
-	print('-> %s' % output)
-	ds.attrs(dd[0], None, alcf.META)
-	ds.write(output, dd[0])
+	if dd[0] == {}:
+		raise RuntimeError('No input files')
+	else:
+		print('-> %s' % output)
+		ds.attrs(dd[0], None, alcf.META)
+		ds.write(output, dd[0])
```

### Comparing `alcf-1.9.0/alcf/download/era5.py` & `alcf-2.0.0/alcf/download/era5.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/download/merra2.py` & `alcf-2.0.0/alcf/download/merra2.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/fonts/LICENSE.md` & `alcf-2.0.0/alcf/fonts/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/fonts/PublicSans-Bold.otf` & `alcf-2.0.0/alcf/fonts/PublicSans-Bold.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/fonts/PublicSans-BoldItalic.otf` & `alcf-2.0.0/alcf/fonts/PublicSans-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/fonts/PublicSans-Italic.otf` & `alcf-2.0.0/alcf/fonts/PublicSans-Italic.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/fonts/PublicSans-Regular.otf` & `alcf-2.0.0/alcf/fonts/PublicSans-Regular.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/lidars/__init__.py` & `alcf-2.0.0/alcf/lidars/__init__.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/lidars/blview.py` & `alcf-2.0.0/alcf/lidars/blview.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/lidars/chm15k.py` & `alcf-2.0.0/alcf/lidars/chm15k.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/lidars/cl51.py` & `alcf-2.0.0/alcf/lidars/cl51.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/lidars/cl61.py` & `alcf-2.0.0/alcf/lidars/cl61.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/lidars/default.py` & `alcf-2.0.0/alcf/lidars/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/lidars/mpl.py` & `alcf-2.0.0/alcf/lidars/mpl.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/lidars/mpl2nc.py` & `alcf-2.0.0/alcf/lidars/mpl2nc.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/misc.py` & `alcf-2.0.0/alcf/misc.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/models/__init__.py` & `alcf-2.0.0/alcf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/models/amps.py` & `alcf-2.0.0/alcf/models/amps.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/models/era5.py` & `alcf-2.0.0/alcf/models/era5.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/models/icon.py` & `alcf-2.0.0/alcf/models/icon.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/models/icon_intake_healpix.py` & `alcf-2.0.0/alcf/models/icon_intake_healpix.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/models/jra55.py` & `alcf-2.0.0/alcf/models/jra55.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/models/merra2.py` & `alcf-2.0.0/alcf/models/merra2.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/models/nzcsm.py` & `alcf-2.0.0/alcf/models/nzcsm.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/models/nzesm.py` & `alcf-2.0.0/alcf/models/nzesm.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf/models/um.py` & `alcf-2.0.0/alcf/models/um.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/alcf.egg-info/PKG-INFO` & `alcf-2.0.0/alcf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alcf
-Version: 1.9.0
+Version: 2.0.0
 Summary: Automatic Lidar and Ceilometer Framework (ALCF)
 Home-page: https://alcf.peterkuma.net
 Author: Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn
 Author-email: peter@peterkuma.net
 License: MIT
 Keywords: alc,ceilometer,lidar,atmosphere,model,simulator,nwp,gcm,cosp,actsim,vaisala,cl51,cl31,lufft,chm-15k,minimpl,amps,merra-2,um
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alcf-1.9.0/alcf.egg-info/SOURCES.txt` & `alcf-2.0.0/alcf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,29 @@
 alcf.egg-info/dependency_links.txt
 alcf.egg-info/entry_points.txt
 alcf.egg-info/not-zip-safe
 alcf.egg-info/requires.txt
 alcf.egg-info/top_level.txt
 alcf/algorithms/__init__.py
 alcf/algorithms/couple.py
-alcf/algorithms/interp.pyx
 alcf/algorithms/lidar_ratio.py
 alcf/algorithms/output_sample.py
 alcf/algorithms/stats.py
 alcf/algorithms/tsample.py
 alcf/algorithms/zsample.py
 alcf/algorithms/calibration/__init__.py
 alcf/algorithms/calibration/default.py
 alcf/algorithms/cloud_base_detection/__init__.py
 alcf/algorithms/cloud_base_detection/default.py
 alcf/algorithms/cloud_detection/__init__.py
 alcf/algorithms/cloud_detection/default.py
+alcf/algorithms/interp/__init__.py
+alcf/algorithms/interp/area_block.pyx
+alcf/algorithms/interp/area_linear.pyx
+alcf/algorithms/interp/linear.py
 alcf/algorithms/noise_removal/__init__.py
 alcf/algorithms/noise_removal/default.py
 alcf/bin/__init__.py
 alcf/bin/alcf.py
 alcf/cmds/__init__.py
 alcf/cmds/auto.py
 alcf/cmds/calibrate.py
```

### Comparing `alcf-1.9.0/build_doc` & `alcf-2.0.0/build_doc`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/MISR_simulator/MISR_simulator.f` & `alcf-2.0.0/cosp/MISR_simulator/MISR_simulator.f`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/MODIS_simulator/modis_simulator.F90` & `alcf-2.0.0/cosp/MODIS_simulator/modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/MODIS_simulator/test_modis_simulator.F90` & `alcf-2.0.0/cosp/MODIS_simulator/test_modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/Makefile` & `alcf-2.0.0/cosp/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/Makefile.cmor1` & `alcf-2.0.0/cosp/Makefile.cmor1`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/Makefile.ibm` & `alcf-2.0.0/cosp/Makefile.ibm`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/README.md` & `alcf-2.0.0/cosp/README.md`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/README.txt` & `alcf-2.0.0/cosp/README.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/actsim/lidar_simulator.F90` & `alcf-2.0.0/cosp/actsim/lidar_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/actsim/lmd_ipsl_stats.F90` & `alcf-2.0.0/cosp/actsim/lmd_ipsl_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/actsim/mie_backscatter_1064.F90` & `alcf-2.0.0/cosp/actsim/mie_backscatter_1064.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/actsim/mie_backscatter_532.F90` & `alcf-2.0.0/cosp/actsim/mie_backscatter_532.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/actsim/mie_backscatter_910.F90` & `alcf-2.0.0/cosp/actsim/mie_backscatter_910.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt` & `alcf-2.0.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt` & `alcf-2.0.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt` & `alcf-2.0.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt` & `alcf-2.0.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt` & `alcf-2.0.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt` & `alcf-2.0.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp.F90` & `alcf-2.0.0/cosp/cosp.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_constants.F90` & `alcf-2.0.0/cosp/cosp_constants.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_defs.h` & `alcf-2.0.0/cosp/cosp_defs.h`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_htfrtc.F90` & `alcf-2.0.0/cosp/cosp_htfrtc.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_input_nl.txt` & `alcf-2.0.0/cosp/cosp_input_nl.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_io.F90` & `alcf-2.0.0/cosp/cosp_io.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_isccp_simulator.F90` & `alcf-2.0.0/cosp/cosp_isccp_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_lidar.F90` & `alcf-2.0.0/cosp/cosp_lidar.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_misr_simulator.F90` & `alcf-2.0.0/cosp/cosp_misr_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_modis_simulator.F90` & `alcf-2.0.0/cosp/cosp_modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_output_nl.txt` & `alcf-2.0.0/cosp/cosp_output_nl.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_rttov.F90` & `alcf-2.0.0/cosp/cosp_rttov.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_rttov_simulator.F90` & `alcf-2.0.0/cosp/cosp_rttov_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_simulator.F90` & `alcf-2.0.0/cosp/cosp_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_stats.F90` & `alcf-2.0.0/cosp/cosp_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_types.F90` & `alcf-2.0.0/cosp/cosp_types.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/cosp_utils.F90` & `alcf-2.0.0/cosp/cosp_utils.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/Makefile` & `alcf-2.0.0/cosp/icarus-scops-4.1-bsd/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/README` & `alcf-2.0.0/cosp/icarus-scops-4.1-bsd/README`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/congvec.f` & `alcf-2.0.0/cosp/icarus-scops-4.1-bsd/congvec.f`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/icarus.f` & `alcf-2.0.0/cosp/icarus-scops-4.1-bsd/icarus.f`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/input.data` & `alcf-2.0.0/cosp/icarus-scops-4.1-bsd/input.data`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/input.data.halved` & `alcf-2.0.0/cosp/icarus-scops-4.1-bsd/input.data.halved`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f` & `alcf-2.0.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/license` & `alcf-2.0.0/cosp/icarus-scops-4.1-bsd/license`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/scops.f` & `alcf-2.0.0/cosp/icarus-scops-4.1-bsd/scops.f`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_congvec.f` & `alcf-2.0.0/cosp/icarus-scops-4.1-bsd/test_congvec.f`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh` & `alcf-2.0.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f` & `alcf-2.0.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh` & `alcf-2.0.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/llnl/cosp_radar.F90` & `alcf-2.0.0/cosp/llnl/cosp_radar.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/llnl/llnl_stats.F90` & `alcf-2.0.0/cosp/llnl/llnl_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/llnl/pf_to_mr.f` & `alcf-2.0.0/cosp/llnl/pf_to_mr.f`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/llnl/prec_scops.f` & `alcf-2.0.0/cosp/llnl/prec_scops.f`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/mac_info.txt` & `alcf-2.0.0/cosp/mac_info.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/predict_mom07.F90` & `alcf-2.0.0/cosp/predict_mom07.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/README` & `alcf-2.0.0/cosp/quickbeam/README`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/array_lib.f90` & `alcf-2.0.0/cosp/quickbeam/array_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/atmos_lib.f90` & `alcf-2.0.0/cosp/quickbeam/atmos_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/calc_Re.f90` & `alcf-2.0.0/cosp/quickbeam/calc_Re.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/dsd.f90` & `alcf-2.0.0/cosp/quickbeam/dsd.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/format_input.f90` & `alcf-2.0.0/cosp/quickbeam/format_input.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/gases.f90` & `alcf-2.0.0/cosp/quickbeam/gases.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/load_hydrometeor_classes.f90` & `alcf-2.0.0/cosp/quickbeam/load_hydrometeor_classes.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/load_mie_table.f90` & `alcf-2.0.0/cosp/quickbeam/load_mie_table.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/math_lib.f90` & `alcf-2.0.0/cosp/quickbeam/math_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/mrgrnk.f90` & `alcf-2.0.0/cosp/quickbeam/mrgrnk.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/optics_lib.f90` & `alcf-2.0.0/cosp/quickbeam/optics_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/predict_psd07.f` & `alcf-2.0.0/cosp/quickbeam/predict_psd07.f`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/radar_simulator.f90` & `alcf-2.0.0/cosp/quickbeam/radar_simulator.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/radar_simulator_init.f90` & `alcf-2.0.0/cosp/quickbeam/radar_simulator_init.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/radar_simulator_types.f90` & `alcf-2.0.0/cosp/quickbeam/radar_simulator_types.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/scale_LUTs_io.f90` & `alcf-2.0.0/cosp/quickbeam/scale_LUTs_io.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/quickbeam/zeff.f90` & `alcf-2.0.0/cosp/quickbeam/zeff.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/utils/COSP_plots.py` & `alcf-2.0.0/cosp/utils/COSP_plots.py`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/cosp/utils/append_cf3hr_files.sh` & `alcf-2.0.0/cosp/utils/append_cf3hr_files.sh`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/man/alcf-auto.1` & `alcf-2.0.0/man/alcf-auto.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-AUTO" "1" "April 2024" ""
+.TH "ALCF\-AUTO" "1" "May 2024" ""
 .SH "NAME"
 \fBalcf\-auto\fR \- Peform automatic processing of model or lidar data\.
 .SH "SYNOPSIS"
 .nf
 alcf auto model <model_type> <lidar_type> point: { <lon> <lat> } time: { <start> <end> } [<options>] [<model_options>] [<lidar_options>] [\-\-] <input> <output>
 
 alcf auto model <model_type> <lidar_type> track: <track> [<options>] [<model_options>] [<lidar_options>] [\-\-] <input> <output>
```

### Comparing `alcf-1.9.0/man/alcf-calibrate.1` & `alcf-2.0.0/man/alcf-calibrate.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-CALIBRATE" "1" "April 2024" ""
+.TH "ALCF\-CALIBRATE" "1" "May 2024" ""
 .SH "NAME"
 \fBalcf\-calibrate\fR \- Calibrate ALC backscatter\.
 .SH "SYNOPSIS"
 .nf
 alcf calibrate <type> [\-\-] <time_periods> <input> <output>
 .fi
 .SH "DESCRIPTION"
```

### Comparing `alcf-1.9.0/man/alcf-compare.1` & `alcf-2.0.0/man/alcf-compare.1`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-COMPARE" "1" "April 2024" ""
+.TH "ALCF\-COMPARE" "1" "May 2024" ""
 .SH "NAME"
 \fBalcf\-compare\fR \- Calculate comparison statistics from multiple lidar time series\.
 .SH "SYNOPSIS"
 .nf
 alcf compare <input_1> <input_2> [<input_n>\|\.\|\.\|\.] <output>
 .fi
 .SH "ARGUMENTS"
```

### Comparing `alcf-1.9.0/man/alcf-convert.1` & `alcf-2.0.0/man/alcf-convert.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-CONVERT" "1" "April 2024" ""
+.TH "ALCF\-CONVERT" "1" "May 2024" ""
 .SH "NAME"
 \fBalcf\-convert\fR \- Convert input instrument or model data to NetCDF\.
 .SH "SYNOPSIS"
 .nf
 alcf convert [options] <type> [\-\-] <input> <output>
 .fi
 .SH "DESCRIPTION"
```

### Comparing `alcf-1.9.0/man/alcf-download.1` & `alcf-2.0.0/man/alcf-download.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-DOWNLOAD" "1" "April 2024" ""
+.TH "ALCF\-DOWNLOAD" "1" "May 2024" ""
 .SH "NAME"
 \fBalcf\-download\fR \- Download model data\.
 .SH "SYNOPSIS"
 .nf
 alcf download <type> [login_options] \-\-login
 alcf download <type> point: { <lon> <lat> } time: { <start> <end> } [<options>] [\-\-] <output>
 alcf download <type> track: <track> [<options>] [\-\-] <output>
```

### Comparing `alcf-1.9.0/man/alcf-lidar.1` & `alcf-2.0.0/man/alcf-lidar.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-LIDAR" "1" "April 2024" ""
+.TH "ALCF\-LIDAR" "1" "May 2024" ""
 .SH "NAME"
 \fBalcf\-lidar\fR \- Process lidar data\.
 .SH "SYNOPSIS"
 .nf
 alcf lidar <type> [<options>] [<algorithm_options>] [\-\-] <lidar> <output>
 .fi
 .SH "DESCRIPTION"
@@ -99,14 +99,17 @@
 .TP
 \fBcloud_base_detection: <algorithm>\fR
 Cloud base detection algorithm\. Available algorithms: \fBdefault\fR, \fBnone\fR\. Default: \fBdefault\fR\.
 .TP
 \fB\-\-fix_cl_range\fR
 Fix CL31/CL51 range correction (if \fBnoise_h2\fR firmware option if off)\. The critical range is taken from \fBcl_crit_range\fR\.
 .TP
+\fBinterp: <value>\fR
+Vertical interpolation method\. \fBarea_block\fR for area\-weighting with block interpolation, \fBarea_linear\fR for area\-weighting with linear interpolation or \fBlinear\fR for simple linear interpolation\. Default: \fBarea_block\fR\.
+.TP
 \fBkeep_vars: { <\|\.\|\.\|\. }\fR
 Keep the listed input variables\. The variable must be numerical and have a time dimension\. The variable is resampled in the same way as backscatter along their time and level dimensions, its name is prefixed with \fBinput_\fR, and its type is changed to float64\. Default: \fB{ }\fR\.
 .TP
 \fBlat: <lat>\fR
 Latitude of the instrument (degrees North)\. Default: Taken from lidar data or \fBnone\fR if not available\.
 .TP
 \fBlon: <lon>\fR
```

### Comparing `alcf-1.9.0/man/alcf-model.1` & `alcf-2.0.0/man/alcf-model.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-MODEL" "1" "April 2024" ""
+.TH "ALCF\-MODEL" "1" "May 2024" ""
 .SH "NAME"
 \fBalcf\-model\fR \- Extract model data at a point or along a track\.
 .SH "SYNOPSIS"
 .nf
 alcf model <type> point: { <lon> <lat> } time: { <start> <end> } [options] [\-\-] <input> <output>
 
 alcf model <type> track: <track> [options] [\-\-] <input> <output>
@@ -30,15 +30,15 @@
 \fBtrack: <file>\fR, \fBtrack: { <file>\|\.\|\.\|\. }\fR: One or more track NetCDF files (see Files below)\. If multiple files are supplied and \fBtime_bnds\fR is not present in the files, they are assumed to be multiple segments of a discontinous track unless the last and first time of adjacent tracks are the same\.
 .IP "\[ci]" 4
 \fBoptions\fR: See Options below\.
 .IP "" 0
 .SH "OPTIONS"
 .TP
 \fBnjobs: <n>\fR
-Number of parallel jobs\. Default: number of CPU cores\.
+Number of parallel jobs\. Default: number of CPU cores capped to 16\.
 .TP
 \fB\-r\fR
 Process the input directory recursively\.
 .TP
 \fB\-\-track_lon_180\fR
 Expect track longitude between \-180 and 180 degrees\. This option is no longer needed as the conversion is automatically\. [deprecated]
 .TP
```

### Comparing `alcf-1.9.0/man/alcf-plot.1` & `alcf-2.0.0/man/alcf-plot.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-PLOT" "1" "April 2024" ""
+.TH "ALCF\-PLOT" "1" "May 2024" ""
 .SH "NAME"
 \fBalcf\-plot\fR \- Plot lidar data\.
 .SH "SYNOPSIS"
 .nf
 alcf plot <plot_type> [<options>] [<plot_options>] [\-\-] <input> <output>
 .fi
 .SH "DESCRIPTION"
@@ -60,33 +60,36 @@
 .TP
 \fB\-\-grid\fR
 Plot grid\.
 .TP
 \fBheight: <value>\fR
 Plot height (inches)\. Default: \fB5\fR if \fBplot_type\fR is \fBcloud_occurrence\fR or \fBbackscatter_hist\fR else \fB4\fR\.
 .TP
+\fBinterp: <value>\fR
+Vertical interpolation method\. \fBarea_block\fR for area\-weighting with block interpolation, \fBarea_linear\fR for area\-weighting with linear interpolation or \fBlinear\fR for simple linear interpolation\. Default: \fBarea_block\fR\.
+.TP
+\fBrender: <value>\fR
+Render profiles anti\-aliased (\fBantialiased\fR) or standard (\fBstandard\fR)\. Standard is more suitable for short time intervals\. Default: \fBantialiased\fR\.
+.TP
 \fBsubcolumn: <value>\fR
 Model subcolumn to plot\. Default: \fB0\fR\.
 .TP
 \fBtitle: <value>\fR
 Plot title\.
 .TP
 \fBwidth: <value>\fR
 Plot width (inches)\. Default: \fB5\fR if \fBplot_type\fR is \fBcloud_occurrence\fR or \fBbackscatter_hist\fR else \fB10\fR\.
-.TP
-\fBrender: <value>\fR
-Render profiles anti\-aliased (\fBantialiased\fR) or standard (\fBstandard\fR)\. Standard is more suitable for short time intervals\. Default: \fBantialiased\fR\.
 .SH "BACKSCATTER OPTIONS"
 .TP
-\fBlr: <value>\fR
-Plot effective lidar ratio\. Default: \fBtrue\fR\.
-.TP
 \fBcloud_mask: <value>\fR
 Plot cloud mask\. Default: \fBtrue\fR\.
 .TP
+\fBlr: <value>\fR
+Plot effective lidar ratio\. Default: \fBtrue\fR\.
+.TP
 \fBremove_bmol: <value>\fR
 Remove molecular backscatter (observed data have to be coupled with model data via the \fBcouple\fR option of \fBalcf lidar\fR)\. Default: \fBtrue\fR\.
 .TP
 \fBsigma: <value>\fR
 Remove of number of standard deviations of backscatter from the mean backscatter (real)\. Default: \fB5\fR\.
 .TP
 \fBvlim: { <min> <max }\fR
@@ -135,20 +138,20 @@
 \fBzres: <zres>\fR
 Height resolution (m)\. Default: \fB50\fR\.
 .SH "CBH AND CLOUD_OCCURRENCE OPTIONS"
 .TP
 \fBcolors: { <value>\|\.\|\.\|\. }\fR
 Line colors\. Default: \fB{ #0084c8 #dc0000 #009100 #ffc022 #ba00ff }\fR
 .TP
-\fBlinestyle: { <value> \|\.\|\.\|\. }\fR
-Line style (\fBsolid\fR, \fBdashed\fR, \fBdotted\fR)\. Default: \fBsolid\fR\.
-.TP
 \fBlabels: { <value>\|\.\|\.\|\. }\fR
 Line labels\. Default: \fBnone\fR\.
 .TP
+\fBlinestyle: { <value> \|\.\|\.\|\. }\fR
+Line style (\fBsolid\fR, \fBdashed\fR, \fBdotted\fR)\. Default: \fBsolid\fR\.
+.TP
 \fBlw: <value>\fR
 Line width\. Default: \fB1\fR\.
 .TP
 \fBxlim: { <min> <max> }\fR
 x axis limits (%)\. Default: \fB{ 0 100 }\fR\.
 .TP
 \fBzlim: { <min> <max> }\fR
```

### Comparing `alcf-1.9.0/man/alcf-simulate.1` & `alcf-2.0.0/man/alcf-simulate.1`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-SIMULATE" "1" "April 2024" ""
+.TH "ALCF\-SIMULATE" "1" "May 2024" ""
 .SH "NAME"
 \fBalcf\-simulate\fR \- Simulate lidar measurements from model data using COSP\.
 .SH "SYNOPSIS"
 .nf
 alcf simulate <type> [<options>] [\-\-] <input> <output>
 .fi
 .SH "DESCRIPTION"
```

### Comparing `alcf-1.9.0/man/alcf-stats.1` & `alcf-2.0.0/man/alcf-stats.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-STATS" "1" "April 2024" ""
+.TH "ALCF\-STATS" "1" "May 2024" ""
 .SH "NAME"
 \fBalcf\-stats\fR \- Calculate cloud occurrence statistics\.
 .SH "SYNOPSIS"
 .nf
 alcf stats [<options>] [\-\-] <input> <output>
 .fi
 .SH "DESCRIPTION"
@@ -41,14 +41,17 @@
 .TP
 \fBfilter_exclude: <value> | { <value>\|\.\|\.\|\. }\fR
 Filter by a mask defined in a NetCDF file, described below under Filter file\. If multiple files are supplied, they must all apply for a profile to be excluded\.
 .TP
 \fBfilter_include: <value> | { <value>\|\.\|\.\|\. }\fR
 The same as \fBfilter_exclude\fR, but with time intervals to be included in the result\. If both are defined, \fBfilter_include\fR takes precedence\. If multiple files are supplied, they must all apply for a profile to be included\.
 .TP
+\fBinterp: <value>\fR
+Vertical interpolation method\. \fBarea_block\fR for area\-weighting with block interpolation, \fBarea_linear\fR for area\-weighting with linear interpolation or \fBlinear\fR for simple linear interpolation\. Default: \fBarea_block\fR\.
+.TP
 \fBtlim: { <start> <end> }\fR
 Time limits (see Time format below)\. Default: \fBnone\fR\.
 .TP
 \fBzlim: { <low> <high> }\fR
 Height limits (m)\. Default: \fB{ 0 15000 }\fR\.
 .TP
 \fBzres: <value>\fR
```

### Comparing `alcf-1.9.0/man/alcf.1` & `alcf-2.0.0/man/alcf.1`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF" "1" "April 2024" ""
+.TH "ALCF" "1" "May 2024" ""
 .SH "NAME"
 \fBalcf\fR \- Tool for processing of automatic lidar and ceilometer (ALC) data and intercomparison with atmospheric models\.
 .SH "SYNOPSIS"
 .nf
-alcf <cmd> [<options>]
-alcf <cmd> \-\-help
+alcf <cmd> [<options>] [<arguments>]
+alcf [<cmd>] \-\-help
+alcf \-\-version
 .fi
 .SH "ARGUMENTS"
 .TP
 \fBcmd\fR
 See Commands below\.
 .TP
+\fBarguments\fR
+Command arguments\. Use \fBalcf <cmd> \-\-help\fR for more information\.
+.TP
 \fBoptions\fR
-Command options\.
+Command options (see Options below)\.
 .SH "COMMANDS"
 .TP
 \fBauto\fR
 Peform automatic processing of model or lidar data\.
 .TP
 \fBcalibrate\fR
 Calibrate lidar backscatter\.
@@ -41,18 +45,21 @@
 \fBsimulate\fR
 Simulate lidar measurements from model data using COSP\.
 .TP
 \fBstats\fR
 Calculate cloud occurrence statistics\.
 .SH "OPTIONS"
 .TP
-\fB\-\-help\fR
-Print help for command\.
-.TP
 \fB\-\-debug\fR
 Enable debugging information\.
+.TP
+\fB\-\-help\fR
+Print general help or help for a command and exit\.
+.TP
+\fB\-\-version\fR
+Print version and exit\.
 .SH "COPYRIGHT"
 Copyright \(co 2019–2024 Peter Kuma, Adrian J\. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber and Connor J\. Flynn\.
 .SH "BUG REPORTING"
 Report bugs to Peter Kuma (\fIpeter@peterkuma\.net\fR)\.
 .SH "SEE ALSO"
 alcf\-auto(1), alcf\-calibrate(1), alcf\-compare(1), alcf\-convert(1), alcf\-download(1), alcf\-lidar(1), alcf\-model(1), alcf\-plot(1), alcf\-simulate(1), alcf\-stats(1)
```

### Comparing `alcf-1.9.0/setup.py` & `alcf-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,27 +16,32 @@
 	def run(self):
 		subprocess.run('make', cwd='cosp', check=True)
 		subprocess.run('make', check=True)
 		build_py.run(self)
 
 setup(
 	name='alcf',
-	version='1.9.0',
+	version='2.0.0',
 	description='Automatic Lidar and Ceilometer Framework (ALCF)',
 	author='Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn',
 	author_email='peter@peterkuma.net',
 	license='MIT',
 	entry_points={
 		'console_scripts': 'alcf = alcf.bin.alcf:main_wrapper',
 	},
 	packages=find_packages(),
 	ext_modules=[
 		Extension(
-			'alcf.algorithms.interp',
-			['alcf/algorithms/interp.pyx'],
+			'alcf.algorithms.interp.area_block',
+			['alcf/algorithms/interp/area_block.pyx'],
+			include_dirs = numpy_include_dirs,
+		),
+		Extension(
+			'alcf.algorithms.interp.area_linear',
+			['alcf/algorithms/interp/area_linear.pyx'],
 			include_dirs = numpy_include_dirs,
 		),
 	],
 	zip_safe=False,
 	package_data={'alcf': ['cosp_alcf'] + \
 		[os.path.join('fonts', x) for x in os.listdir('alcf/fonts')]},
 	data_files=[('share/man/man1',
```

### Comparing `alcf-1.9.0/src/cosp_run.f03` & `alcf-2.0.0/src/cosp_run.f03`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/src/main.f03` & `alcf-2.0.0/src/main.f03`

 * *Files identical despite different names*

### Comparing `alcf-1.9.0/src/nc_utils.f03` & `alcf-2.0.0/src/nc_utils.f03`

 * *Files identical despite different names*

