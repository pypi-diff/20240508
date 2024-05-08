# Comparing `tmp/pyaerocom-0.8.0rc3.tar.gz` & `tmp/pyaerocom-0.8.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyaerocom-0.8.0rc3.tar", last modified: Thu Oct 10 15:44:17 2019, max compression
+gzip compressed data, was "dist/pyaerocom-0.8.0rc4.tar", last modified: Fri Oct 11 09:47:00 2019, max compression
```

## Comparing `pyaerocom-0.8.0rc3.tar` & `pyaerocom-0.8.0rc4.tar`

### file list

```diff
@@ -1,147 +1,146 @@
-drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    35141 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc3/LICENSE
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)       99 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc3/MANIFEST.in
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    12129 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/PKG-INFO
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    10342 2019-10-10 09:27:52.000000 pyaerocom-0.8.0rc3/README.rst
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)        9 2019-10-10 15:43:59.000000 pyaerocom-0.8.0rc3/VERSION.md
-drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/pyaerocom/
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     3398 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc3/pyaerocom/__init__.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     7632 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/_lowlevel_helpers.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    35217 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/colocateddata.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    32693 2019-10-10 13:50:55.000000 pyaerocom-0.8.0rc3/pyaerocom/colocation.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    43067 2019-10-10 13:09:48.000000 pyaerocom-0.8.0rc3/pyaerocom/colocation_auto.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    33734 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/config.py
-drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/pyaerocom/data/
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)   196557 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc3/pyaerocom/data/HTAP2_variables.xlsx
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2337 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc3/pyaerocom/data/_create_var_csv_from_htap2_exceltab.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      705 2019-10-09 08:14:30.000000 pyaerocom-0.8.0rc3/pyaerocom/data/aliases.ini
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6562 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/data/coords.ini
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      997 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/data/data_sources.ini
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6930 2019-10-10 09:11:17.000000 pyaerocom-0.8.0rc3/pyaerocom/data/ebas_config.ini
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     9905 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc3/pyaerocom/data/ebas_flags.csv
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      350 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/data/file_conventions.ini
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    30473 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc3/pyaerocom/data/model_ids.txt
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6691 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/data/paths.ini
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     4320 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc3/pyaerocom/data/paths_testdata.ini
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      996 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/data/paths_user_server.ini
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1134 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc3/pyaerocom/data/regions.ini
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      483 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc3/pyaerocom/data/test_files.ini
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)   156028 2019-10-10 09:11:17.000000 pyaerocom-0.8.0rc3/pyaerocom/data/variables.ini
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2816 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/exceptions.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     7117 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/filter.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     9028 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/geodesy.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6847 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/grid_io.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    79635 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/griddeddata.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    37792 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/helpers.py
-drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/pyaerocom/interactive/
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      253 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc3/pyaerocom/interactive/__init__.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      364 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc3/pyaerocom/interactive/ipywidgets.py
-drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/pyaerocom/io/
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     3565 2019-10-09 08:14:30.000000 pyaerocom-0.8.0rc3/pyaerocom/io/__init__.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     9171 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/aerocom_browser.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6160 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/aux_read_cubes.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    11573 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/cachehandler_ungridded.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    12466 2019-06-19 11:21:22.000000 pyaerocom-0.8.0rc3/pyaerocom/io/cachehandler_ungriddedOLD.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    17659 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/ebas_file_index.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    36249 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/ebas_nasa_ames.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    10023 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/ebas_varinfo.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    15400 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/fileconventions.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     8432 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/helpers.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     5551 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/helpers_units.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    25149 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/iris_io.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    14046 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc3/pyaerocom/io/read_aasetal.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)   116101 2019-10-09 08:14:30.000000 pyaerocom-0.8.0rc3/pyaerocom/io/read_aeolus_l2a_data.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    13824 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/read_aeronet_invv2.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    12244 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/read_aeronet_invv3.py
--rwxr-xr-x   0 jonasg   (421188) jonasg   (421188)    14134 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/read_aeronet_sdav2.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    10987 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/read_aeronet_sdav3.py
--rwxr-xr-x   0 jonasg   (421188) jonasg   (421188)     9752 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/read_aeronet_sunv2.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    12118 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/read_aeronet_sunv3.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      876 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/read_airbase.py
--rwxr-xr-x   0 jonasg   (421188) jonasg   (421188)    30156 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/read_earlinet.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    52099 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/read_ebas.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    20629 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc3/pyaerocom/io/read_gaw.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    48756 2019-10-09 08:14:30.000000 pyaerocom-0.8.0rc3/pyaerocom/io/read_sentinel5p_data.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    20052 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/readaeronetbase.py
--rwxr-xr-x   0 jonasg   (421188) jonasg   (421188)    73597 2019-10-09 08:14:30.000000 pyaerocom-0.8.0rc3/pyaerocom/io/readgridded.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    32394 2019-10-09 08:14:30.000000 pyaerocom-0.8.0rc3/pyaerocom/io/readsatellitel2base.py
--rwxr-xr-x   0 jonasg   (421188) jonasg   (421188)    19235 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc3/pyaerocom/io/readungridded.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    24318 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/readungriddedbase.py
-drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/pyaerocom/io/test/
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)       24 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc3/pyaerocom/io/test/__init__.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    20167 2019-10-10 09:11:17.000000 pyaerocom-0.8.0rc3/pyaerocom/io/test/test_aas_et_al.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1202 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/test/test_read_aeronet_invv3.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2672 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/test/test_read_aeronet_sdav2.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1500 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/test/test_read_aeronet_sdav3.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1277 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/test/test_read_aeronet_sunv2.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     4896 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/test/test_read_aeronet_sunv3.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2895 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/test/test_read_earlinet.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2738 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/test/test_readgridded.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2106 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc3/pyaerocom/io/test/test_readungridded.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2103 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc3/pyaerocom/io/testfiles.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2441 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/io/utils.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    19797 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc3/pyaerocom/mathutils.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     5794 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/metastandards.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      503 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc3/pyaerocom/obs_io.py
-drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/pyaerocom/plot/
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1582 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/plot/__init__.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     5677 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/plot/config.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6093 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/plot/heatmaps.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6394 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc3/pyaerocom/plot/helpers.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    18905 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/plot/mapping.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1634 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/plot/plotcoordinates.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    10843 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc3/pyaerocom/plot/plotmaps.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     7638 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/plot/plotscatter.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     8812 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/plot/plotscatter_v0.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     4659 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/plot/plotseries.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     8608 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/plot/plotsitelocation.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    11023 2019-10-09 08:14:30.000000 pyaerocom-0.8.0rc3/pyaerocom/region.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    57423 2019-10-10 09:11:17.000000 pyaerocom-0.8.0rc3/pyaerocom/stationdata.py
-drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/pyaerocom/test/
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)       23 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/test/__init__.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1474 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc3/pyaerocom/test/settings.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2771 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc3/pyaerocom/test/synthetic_data.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      817 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/test/test_colocateddata.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     3072 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc3/pyaerocom/test/test_dms_gaw.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     5306 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/test/test_ebas_sample_stats.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      982 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/test/test_geodesy.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     3733 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/test/test_griddeddata.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     3457 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/test/test_helpers.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      483 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/test/test_mathutils.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1390 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc3/pyaerocom/test/test_obsdata_versions.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1845 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc3/pyaerocom/test/test_stationdata.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      878 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/test/test_tstype.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2026 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/test/test_ungriddeddata.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      293 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/test/test_units_helpers.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     3363 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/time_config.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     9615 2019-10-10 09:11:17.000000 pyaerocom-0.8.0rc3/pyaerocom/time_resampler.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    24177 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/trends_helpers.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     5245 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/tstype.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)   100204 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/ungriddeddata.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6530 2019-10-10 09:11:17.000000 pyaerocom-0.8.0rc3/pyaerocom/units_helpers.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     5458 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/utils.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    25294 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/variable.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    25305 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/vert_coords.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     8150 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/vertical_profile.py
-drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/pyaerocom/web/
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      220 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc3/pyaerocom/web/__init__.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    64672 2019-10-10 15:10:14.000000 pyaerocom-0.8.0rc3/pyaerocom/web/aerocom_evaluation.py
-drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/pyaerocom/web/cli/
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     4273 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/web/cli/main_aerocom_evaluation.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2564 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/web/cli/main_trends_evaluation.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    20224 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/web/helpers.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     3815 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/web/obs_config_default.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    69311 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom/web/trends_evaluation.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      272 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc3/pyaerocom/web/var_groups.py
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1520 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc3/pyaerocom/web/web_naming_conventions.py
-drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/pyaerocom.egg-info/
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)    12129 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/pyaerocom.egg-info/PKG-INFO
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     4033 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/pyaerocom.egg-info/SOURCES.txt
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)        1 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/pyaerocom.egg-info/dependency_links.txt
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      140 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/pyaerocom.egg-info/entry_points.txt
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)        1 2019-05-17 09:43:42.000000 pyaerocom-0.8.0rc3/pyaerocom.egg-info/not-zip-safe
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)       10 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/pyaerocom.egg-info/top_level.txt
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)      273 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pyaerocom_env.yml
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)       49 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc3/pytest.ini
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)       38 2019-10-10 15:44:17.000000 pyaerocom-0.8.0rc3/setup.cfg
--rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1971 2019-10-10 09:11:17.000000 pyaerocom-0.8.0rc3/setup.py
+drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    35141 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc4/LICENSE
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)       99 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc4/MANIFEST.in
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    12129 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/PKG-INFO
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    10342 2019-10-10 09:27:52.000000 pyaerocom-0.8.0rc4/README.rst
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)        9 2019-10-11 09:26:11.000000 pyaerocom-0.8.0rc4/VERSION.md
+drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/pyaerocom/
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     3398 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc4/pyaerocom/__init__.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     7632 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/_lowlevel_helpers.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    35217 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/colocateddata.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    32693 2019-10-10 13:50:55.000000 pyaerocom-0.8.0rc4/pyaerocom/colocation.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    43067 2019-10-10 13:09:48.000000 pyaerocom-0.8.0rc4/pyaerocom/colocation_auto.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    33734 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/config.py
+drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/pyaerocom/data/
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)   196557 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc4/pyaerocom/data/HTAP2_variables.xlsx
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2337 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc4/pyaerocom/data/_create_var_csv_from_htap2_exceltab.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      705 2019-10-09 08:14:30.000000 pyaerocom-0.8.0rc4/pyaerocom/data/aliases.ini
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6562 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/data/coords.ini
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      997 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/data/data_sources.ini
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6930 2019-10-10 09:11:17.000000 pyaerocom-0.8.0rc4/pyaerocom/data/ebas_config.ini
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     9905 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc4/pyaerocom/data/ebas_flags.csv
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      350 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/data/file_conventions.ini
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    30473 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc4/pyaerocom/data/model_ids.txt
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6691 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/data/paths.ini
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     4320 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc4/pyaerocom/data/paths_testdata.ini
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      996 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/data/paths_user_server.ini
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1134 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc4/pyaerocom/data/regions.ini
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      483 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc4/pyaerocom/data/test_files.ini
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)   156028 2019-10-10 09:11:17.000000 pyaerocom-0.8.0rc4/pyaerocom/data/variables.ini
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2816 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/exceptions.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     7117 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/filter.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     9028 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/geodesy.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6488 2019-10-11 09:10:37.000000 pyaerocom-0.8.0rc4/pyaerocom/grid_io.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    79635 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/griddeddata.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    37792 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/helpers.py
+drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/pyaerocom/interactive/
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      253 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc4/pyaerocom/interactive/__init__.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      364 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc4/pyaerocom/interactive/ipywidgets.py
+drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/pyaerocom/io/
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     3565 2019-10-09 08:14:30.000000 pyaerocom-0.8.0rc4/pyaerocom/io/__init__.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     9615 2019-10-11 09:24:21.000000 pyaerocom-0.8.0rc4/pyaerocom/io/aerocom_browser.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6160 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/aux_read_cubes.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    11573 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/cachehandler_ungridded.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    17659 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/ebas_file_index.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    36249 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/ebas_nasa_ames.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    10023 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/ebas_varinfo.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    15400 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/fileconventions.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     8432 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/helpers.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     5551 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/helpers_units.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    25149 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/iris_io.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    14046 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc4/pyaerocom/io/read_aasetal.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)   116101 2019-10-09 08:14:30.000000 pyaerocom-0.8.0rc4/pyaerocom/io/read_aeolus_l2a_data.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    13824 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/read_aeronet_invv2.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    12244 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/read_aeronet_invv3.py
+-rwxr-xr-x   0 jonasg   (421188) jonasg   (421188)    14134 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/read_aeronet_sdav2.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    10987 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/read_aeronet_sdav3.py
+-rwxr-xr-x   0 jonasg   (421188) jonasg   (421188)     9752 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/read_aeronet_sunv2.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    12118 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/read_aeronet_sunv3.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      876 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/read_airbase.py
+-rwxr-xr-x   0 jonasg   (421188) jonasg   (421188)    30156 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/read_earlinet.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    52099 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/read_ebas.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    20629 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc4/pyaerocom/io/read_gaw.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    48756 2019-10-09 08:14:30.000000 pyaerocom-0.8.0rc4/pyaerocom/io/read_sentinel5p_data.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    20052 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/readaeronetbase.py
+-rwxr-xr-x   0 jonasg   (421188) jonasg   (421188)    73597 2019-10-09 08:14:30.000000 pyaerocom-0.8.0rc4/pyaerocom/io/readgridded.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    32394 2019-10-09 08:14:30.000000 pyaerocom-0.8.0rc4/pyaerocom/io/readsatellitel2base.py
+-rwxr-xr-x   0 jonasg   (421188) jonasg   (421188)    19235 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc4/pyaerocom/io/readungridded.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    24318 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/readungriddedbase.py
+drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/pyaerocom/io/test/
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)       24 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc4/pyaerocom/io/test/__init__.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    20167 2019-10-10 09:11:17.000000 pyaerocom-0.8.0rc4/pyaerocom/io/test/test_aas_et_al.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1202 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/test/test_read_aeronet_invv3.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2672 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/test/test_read_aeronet_sdav2.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1500 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/test/test_read_aeronet_sdav3.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1277 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/test/test_read_aeronet_sunv2.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     4896 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/test/test_read_aeronet_sunv3.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2895 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/test/test_read_earlinet.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2738 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/io/test/test_readgridded.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2106 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc4/pyaerocom/io/test/test_readungridded.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2103 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc4/pyaerocom/io/testfiles.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2441 2019-10-11 09:23:06.000000 pyaerocom-0.8.0rc4/pyaerocom/io/utils.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    19797 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc4/pyaerocom/mathutils.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     5794 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/metastandards.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      503 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc4/pyaerocom/obs_io.py
+drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/pyaerocom/plot/
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1582 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/plot/__init__.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     5677 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/plot/config.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6093 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/plot/heatmaps.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6394 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc4/pyaerocom/plot/helpers.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    18905 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/plot/mapping.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1634 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/plot/plotcoordinates.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    10843 2019-05-17 09:23:16.000000 pyaerocom-0.8.0rc4/pyaerocom/plot/plotmaps.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     7638 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/plot/plotscatter.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     8812 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/plot/plotscatter_v0.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     4659 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/plot/plotseries.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     8608 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/plot/plotsitelocation.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    11023 2019-10-09 08:14:30.000000 pyaerocom-0.8.0rc4/pyaerocom/region.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    57423 2019-10-10 09:11:17.000000 pyaerocom-0.8.0rc4/pyaerocom/stationdata.py
+drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/pyaerocom/test/
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)       23 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/test/__init__.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1474 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc4/pyaerocom/test/settings.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2771 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc4/pyaerocom/test/synthetic_data.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      817 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/test/test_colocateddata.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     3072 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc4/pyaerocom/test/test_dms_gaw.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     5306 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/test/test_ebas_sample_stats.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      982 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/test/test_geodesy.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     3733 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/test/test_griddeddata.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     3457 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/test/test_helpers.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      483 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/test/test_mathutils.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1390 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc4/pyaerocom/test/test_obsdata_versions.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1845 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc4/pyaerocom/test/test_stationdata.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      878 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/test/test_tstype.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2026 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/test/test_ungriddeddata.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      293 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/test/test_units_helpers.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     3363 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/time_config.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     9615 2019-10-10 09:11:17.000000 pyaerocom-0.8.0rc4/pyaerocom/time_resampler.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    24177 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/trends_helpers.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     5245 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/tstype.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)   100204 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/ungriddeddata.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     6530 2019-10-10 09:11:17.000000 pyaerocom-0.8.0rc4/pyaerocom/units_helpers.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     5458 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/utils.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    25294 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/variable.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    25305 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/vert_coords.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     8150 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/vertical_profile.py
+drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/pyaerocom/web/
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      220 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc4/pyaerocom/web/__init__.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    64672 2019-10-10 15:10:14.000000 pyaerocom-0.8.0rc4/pyaerocom/web/aerocom_evaluation.py
+drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/pyaerocom/web/cli/
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     4273 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/web/cli/main_aerocom_evaluation.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     2564 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/web/cli/main_trends_evaluation.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    20224 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/web/helpers.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     3815 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/web/obs_config_default.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    69311 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom/web/trends_evaluation.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      272 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc4/pyaerocom/web/var_groups.py
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1520 2019-10-09 08:13:47.000000 pyaerocom-0.8.0rc4/pyaerocom/web/web_naming_conventions.py
+drwxr-xr-x   0 jonasg   (421188) jonasg   (421188)        0 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/pyaerocom.egg-info/
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)    12129 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/pyaerocom.egg-info/PKG-INFO
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     3991 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/pyaerocom.egg-info/SOURCES.txt
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)        1 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/pyaerocom.egg-info/dependency_links.txt
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      140 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/pyaerocom.egg-info/entry_points.txt
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)        1 2019-05-17 09:43:42.000000 pyaerocom-0.8.0rc4/pyaerocom.egg-info/not-zip-safe
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)       10 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/pyaerocom.egg-info/top_level.txt
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)      273 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pyaerocom_env.yml
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)       49 2019-10-04 13:06:03.000000 pyaerocom-0.8.0rc4/pytest.ini
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)       38 2019-10-11 09:47:00.000000 pyaerocom-0.8.0rc4/setup.cfg
+-rw-r--r--   0 jonasg   (421188) jonasg   (421188)     1971 2019-10-10 09:11:17.000000 pyaerocom-0.8.0rc4/setup.py
```

### Comparing `pyaerocom-0.8.0rc3/LICENSE` & `pyaerocom-0.8.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/PKG-INFO` & `pyaerocom-0.8.0rc4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyaerocom
-Version: 0.8.0rc3
+Version: 0.8.0rc4
 Summary: Python tools for the Aerocom project
 Home-page: https://github.com/jgliss/pyaerocom.git
 Author: Jonas Gliss
 Author-email: jonas.gliss@met.no
 License: GPLv3
 Description: NEWS
         ====
```

### Comparing `pyaerocom-0.8.0rc3/README.rst` & `pyaerocom-0.8.0rc4/README.rst`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/__init__.py` & `pyaerocom-0.8.0rc4/pyaerocom/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/_lowlevel_helpers.py` & `pyaerocom-0.8.0rc4/pyaerocom/_lowlevel_helpers.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/colocateddata.py` & `pyaerocom-0.8.0rc4/pyaerocom/colocateddata.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/colocation.py` & `pyaerocom-0.8.0rc4/pyaerocom/colocation.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/colocation_auto.py` & `pyaerocom-0.8.0rc4/pyaerocom/colocation_auto.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/config.py` & `pyaerocom-0.8.0rc4/pyaerocom/config.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/data/HTAP2_variables.xlsx` & `pyaerocom-0.8.0rc4/pyaerocom/data/HTAP2_variables.xlsx`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/data/_create_var_csv_from_htap2_exceltab.py` & `pyaerocom-0.8.0rc4/pyaerocom/data/_create_var_csv_from_htap2_exceltab.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/data/aliases.ini` & `pyaerocom-0.8.0rc4/pyaerocom/data/aliases.ini`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/data/coords.ini` & `pyaerocom-0.8.0rc4/pyaerocom/data/coords.ini`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/data/data_sources.ini` & `pyaerocom-0.8.0rc4/pyaerocom/data/data_sources.ini`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/data/ebas_config.ini` & `pyaerocom-0.8.0rc4/pyaerocom/data/ebas_config.ini`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/data/ebas_flags.csv` & `pyaerocom-0.8.0rc4/pyaerocom/data/ebas_flags.csv`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/data/model_ids.txt` & `pyaerocom-0.8.0rc4/pyaerocom/data/model_ids.txt`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/data/paths.ini` & `pyaerocom-0.8.0rc4/pyaerocom/data/paths.ini`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/data/paths_testdata.ini` & `pyaerocom-0.8.0rc4/pyaerocom/data/paths_testdata.ini`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/data/paths_user_server.ini` & `pyaerocom-0.8.0rc4/pyaerocom/data/paths_user_server.ini`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/data/regions.ini` & `pyaerocom-0.8.0rc4/pyaerocom/data/regions.ini`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/data/variables.ini` & `pyaerocom-0.8.0rc4/pyaerocom/data/variables.ini`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/exceptions.py` & `pyaerocom-0.8.0rc4/pyaerocom/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/filter.py` & `pyaerocom-0.8.0rc4/pyaerocom/filter.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/geodesy.py` & `pyaerocom-0.8.0rc4/pyaerocom/geodesy.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/grid_io.py` & `pyaerocom-0.8.0rc4/pyaerocom/grid_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,14 @@
         if True (and if metadata varies between different NetCDF files that are
         supposed to be merged in time), the metadata in all loaded objects is 
         unified based on the metadata of the first grid (otherwise, 
         concatenating them in time might not work using the Iris interface).
         This might need to be reviewed and should be used with care if 
         specific metadata aspects of individual files need to be accessed.
         Aerocom default is True
-    USE_RENAMED_DIR : bool
-        if True, data files are searched within a subdirectory named "renamed" 
-        that needs to exist withing the data directory of a certain model or
-        obs data type. Aerocom default is True.
     USE_FILECONVENTION : bool
         if True, file names are strictly required to follow one of the file
         naming conventions that can be specified in the file 
         `file_conventions.ini <https://github.com/metno/pyaerocom/tree/master/
         pyaerocom/data>`__. Aerocom default is True.
     INCLUDE_SUBDIRS : bool
         if True, search for files is expanded to all subdirecories included in
@@ -76,25 +72,24 @@
                 'PERFORM_FMT_CHECKS': True,
                 'DEL_TIME_BOUNDS': True,
                 'SHIFT_LONS': True,
                 'CHECK_TIME_FILENAME': True,
                 'CORRECT_TIME_FILENAME': True,
                 'CHECK_DIM_COORDS': True,
                 'EQUALISE_METADATA': True,
-                'USE_RENAMED_DIR': True,
                 'INCLUDE_SUBDIRS': False}
+    
     _DEFAULT = {'FILE_TYPE': '.nc',
                 'PERFORM_FMT_CHECKS' : False,
                 'DEL_TIME_BOUNDS': True,
                 'SHIFT_LONS': False,
                 'CHECK_TIME_FILENAME': False,
                 'CORRECT_TIME_FILENAME': False,
                 'CHECK_DIM_COORDS': False,
                 'EQUALISE_METADATA': False,
-                'USE_RENAMED_DIR': False,
                 'INCLUDE_SUBDIRS': True}
     
     def __init__(self, **kwargs):
         self.FILE_TYPE = '.nc'
         # it is important to keep them in the order from highest to lowest
         # resolution
         self.TS_TYPES = ['minutely', 'hourly', '3hourly', 'daily', 'weekly', 
@@ -113,20 +108,18 @@
         self.CHECK_DIM_COORDS = False
          # check and update metadata dictionary on Cube load since 
          # iris concatenate of Cubes only works if metadata is equal
         
         
         self.EQUALISE_METADATA = True
         
-        self.USE_RENAMED_DIR = True
-        
         self.INCLUDE_SUBDIRS = False
         
         self.INFER_SURFACE_LEVEL = True
-        
+    
     def load_aerocom_default(self):
         self.from_dict(self._AEROCOM)
     
     def load_default(self):
         self.from_dict(self._DEFAULT)
         
     def to_dict(self):
```

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/griddeddata.py` & `pyaerocom-0.8.0rc4/pyaerocom/griddeddata.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/helpers.py` & `pyaerocom-0.8.0rc4/pyaerocom/helpers.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/__init__.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/aerocom_browser.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/aerocom_browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,43 +97,51 @@
                 for subdir in subdirs:
                     if ignorecase:
                         match = bool(re.search(pattern, subdir,re.IGNORECASE))
                     else:
                         match = bool(re.search(pattern, subdir))
                     if match:
                         _dir = join(search_dir, subdir)
-                        ok = True 
-                        if const.GRID_IO.USE_RENAMED_DIR:
-                            logger.info("Checking if renamed directory exists")
-                            _dir = join(_dir, "renamed")
-                            if not isdir(_dir):
-                                ok = False
-                                _warnings.append("Renamed folder does not exist "
-                                                 "in {}".format(join(search_dir, 
-                                                     subdir)))
-                        # directory exists and is candidate since it matches 
-                        # the pattern
-                        if ok:
-                            # append name of candidate ...
-                            _candidates.append(subdir)
-                            # ... and the corresponding data directory
-                            self[subdir] = _dir
-                            
-                            # now check if it is actually an exact match, if 
-                            # applicable
-                            if return_if_match:
-                            
-                                if ignorecase:
-                                    match = name_or_pattern.lower() == subdir.lower()
-                                else:
-                                    match = name_or_pattern == subdir
-                                if match:
-                                    logger.info("Found match for ID {}".format(name_or_pattern))
-                                    if return_if_match:
-                                        return _dir
+                        _rnsubdir = join(_dir, "renamed")
+                        if isdir(_rnsubdir):
+                            logger.info("{} has subdir renamed. Using that one"
+                                        .format(_dir))
+                            _dir = _rnsubdir
+# =============================================================================
+#                         ok = True 
+#                         if const.GRID_IO.USE_RENAMED_DIR:
+#                             logger.info("Checking if renamed directory exists")
+#                             _dir = join(_dir, "renamed")
+#                             if not isdir(_dir):
+#                                 ok = False
+#                                 _warnings.append("Renamed folder does not exist "
+#                                                  "in {}".format(join(search_dir, 
+#                                                      subdir)))
+#                         # directory exists and is candidate since it matches 
+#                         # the pattern
+#                         if ok:
+# =============================================================================
+                        # append name of candidate ...
+                        _candidates.append(subdir)
+                        # ... and the corresponding data directory
+                        self[subdir] = _dir
+                        
+                        # now check if it is actually an exact match, if 
+                        # applicable
+                        if return_if_match:
+                        
+                            if ignorecase:
+                                match = name_or_pattern.lower() == subdir.lower()
+                            else:
+                                match = name_or_pattern == subdir
+                            if match:
+                                logger.info("Found match for ID {}"
+                                            .format(name_or_pattern))
+                                if return_if_match:
+                                    return _dir
                                 
                                 
                         
             else:
                 _msgs.append('directory %s does not exist\n'
                                  %search_dir)
         for msg in _msgs:
```

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/aux_read_cubes.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/aux_read_cubes.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/cachehandler_ungridded.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/cachehandler_ungridded.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/ebas_file_index.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/ebas_file_index.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/ebas_nasa_ames.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/ebas_nasa_ames.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/ebas_varinfo.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/ebas_varinfo.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/fileconventions.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/fileconventions.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/helpers.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/helpers.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/helpers_units.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/helpers_units.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/iris_io.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/iris_io.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/read_aasetal.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/read_aasetal.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/read_aeolus_l2a_data.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/read_aeolus_l2a_data.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/read_aeronet_invv2.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/read_aeronet_invv2.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/read_aeronet_invv3.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/read_aeronet_invv3.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/read_aeronet_sdav2.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/read_aeronet_sdav2.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/read_aeronet_sdav3.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/read_aeronet_sdav3.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/read_aeronet_sunv2.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/read_aeronet_sunv2.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/read_aeronet_sunv3.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/read_aeronet_sunv3.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/read_airbase.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/read_airbase.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/read_earlinet.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/read_earlinet.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/read_ebas.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/read_ebas.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/read_gaw.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/read_gaw.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/read_sentinel5p_data.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/read_sentinel5p_data.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/readaeronetbase.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/readaeronetbase.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/readgridded.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/readgridded.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/readsatellitel2base.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/readsatellitel2base.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/readungridded.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/readungridded.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/readungriddedbase.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/readungriddedbase.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/test/test_aas_et_al.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/test/test_aas_et_al.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/test/test_read_aeronet_invv3.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/test/test_read_aeronet_invv3.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/test/test_read_aeronet_sdav2.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/test/test_read_aeronet_sdav2.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/test/test_read_aeronet_sdav3.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/test/test_read_aeronet_sdav3.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/test/test_read_aeronet_sunv2.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/test/test_read_aeronet_sunv2.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/test/test_read_aeronet_sunv3.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/test/test_read_aeronet_sunv3.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/test/test_read_earlinet.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/test/test_read_earlinet.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/test/test_readgridded.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/test/test_readgridded.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/test/test_readungridded.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/test/test_readungridded.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/testfiles.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/testfiles.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/io/utils.py` & `pyaerocom-0.8.0rc4/pyaerocom/io/utils.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/mathutils.py` & `pyaerocom-0.8.0rc4/pyaerocom/mathutils.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/metastandards.py` & `pyaerocom-0.8.0rc4/pyaerocom/metastandards.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/plot/__init__.py` & `pyaerocom-0.8.0rc4/pyaerocom/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/plot/config.py` & `pyaerocom-0.8.0rc4/pyaerocom/plot/config.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/plot/heatmaps.py` & `pyaerocom-0.8.0rc4/pyaerocom/plot/heatmaps.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/plot/helpers.py` & `pyaerocom-0.8.0rc4/pyaerocom/plot/helpers.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/plot/mapping.py` & `pyaerocom-0.8.0rc4/pyaerocom/plot/mapping.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/plot/plotcoordinates.py` & `pyaerocom-0.8.0rc4/pyaerocom/plot/plotcoordinates.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/plot/plotmaps.py` & `pyaerocom-0.8.0rc4/pyaerocom/plot/plotmaps.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/plot/plotscatter.py` & `pyaerocom-0.8.0rc4/pyaerocom/plot/plotscatter.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/plot/plotscatter_v0.py` & `pyaerocom-0.8.0rc4/pyaerocom/plot/plotscatter_v0.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/plot/plotseries.py` & `pyaerocom-0.8.0rc4/pyaerocom/plot/plotseries.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/plot/plotsitelocation.py` & `pyaerocom-0.8.0rc4/pyaerocom/plot/plotsitelocation.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/region.py` & `pyaerocom-0.8.0rc4/pyaerocom/region.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/stationdata.py` & `pyaerocom-0.8.0rc4/pyaerocom/stationdata.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/test/settings.py` & `pyaerocom-0.8.0rc4/pyaerocom/test/settings.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/test/synthetic_data.py` & `pyaerocom-0.8.0rc4/pyaerocom/test/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/test/test_colocateddata.py` & `pyaerocom-0.8.0rc4/pyaerocom/test/test_colocateddata.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/test/test_dms_gaw.py` & `pyaerocom-0.8.0rc4/pyaerocom/test/test_dms_gaw.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/test/test_ebas_sample_stats.py` & `pyaerocom-0.8.0rc4/pyaerocom/test/test_ebas_sample_stats.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/test/test_geodesy.py` & `pyaerocom-0.8.0rc4/pyaerocom/test/test_geodesy.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/test/test_griddeddata.py` & `pyaerocom-0.8.0rc4/pyaerocom/test/test_griddeddata.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/test/test_helpers.py` & `pyaerocom-0.8.0rc4/pyaerocom/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/test/test_obsdata_versions.py` & `pyaerocom-0.8.0rc4/pyaerocom/test/test_obsdata_versions.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/test/test_stationdata.py` & `pyaerocom-0.8.0rc4/pyaerocom/test/test_stationdata.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/test/test_tstype.py` & `pyaerocom-0.8.0rc4/pyaerocom/test/test_tstype.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/test/test_ungriddeddata.py` & `pyaerocom-0.8.0rc4/pyaerocom/test/test_ungriddeddata.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/time_config.py` & `pyaerocom-0.8.0rc4/pyaerocom/time_config.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/time_resampler.py` & `pyaerocom-0.8.0rc4/pyaerocom/time_resampler.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/trends_helpers.py` & `pyaerocom-0.8.0rc4/pyaerocom/trends_helpers.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/tstype.py` & `pyaerocom-0.8.0rc4/pyaerocom/tstype.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/ungriddeddata.py` & `pyaerocom-0.8.0rc4/pyaerocom/ungriddeddata.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/units_helpers.py` & `pyaerocom-0.8.0rc4/pyaerocom/units_helpers.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/utils.py` & `pyaerocom-0.8.0rc4/pyaerocom/utils.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/variable.py` & `pyaerocom-0.8.0rc4/pyaerocom/variable.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/vert_coords.py` & `pyaerocom-0.8.0rc4/pyaerocom/vert_coords.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/vertical_profile.py` & `pyaerocom-0.8.0rc4/pyaerocom/vertical_profile.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/web/aerocom_evaluation.py` & `pyaerocom-0.8.0rc4/pyaerocom/web/aerocom_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/web/cli/main_aerocom_evaluation.py` & `pyaerocom-0.8.0rc4/pyaerocom/web/cli/main_aerocom_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/web/cli/main_trends_evaluation.py` & `pyaerocom-0.8.0rc4/pyaerocom/web/cli/main_trends_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/web/helpers.py` & `pyaerocom-0.8.0rc4/pyaerocom/web/helpers.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/web/obs_config_default.py` & `pyaerocom-0.8.0rc4/pyaerocom/web/obs_config_default.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/web/trends_evaluation.py` & `pyaerocom-0.8.0rc4/pyaerocom/web/trends_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom/web/web_naming_conventions.py` & `pyaerocom-0.8.0rc4/pyaerocom/web/web_naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyaerocom-0.8.0rc3/pyaerocom.egg-info/PKG-INFO` & `pyaerocom-0.8.0rc4/pyaerocom.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyaerocom
-Version: 0.8.0rc3
+Version: 0.8.0rc4
 Summary: Python tools for the Aerocom project
 Home-page: https://github.com/jgliss/pyaerocom.git
 Author: Jonas Gliss
 Author-email: jonas.gliss@met.no
 License: GPLv3
 Description: NEWS
         ====
```

### Comparing `pyaerocom-0.8.0rc3/pyaerocom.egg-info/SOURCES.txt` & `pyaerocom-0.8.0rc4/pyaerocom.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 pyaerocom/data/variables.ini
 pyaerocom/interactive/__init__.py
 pyaerocom/interactive/ipywidgets.py
 pyaerocom/io/__init__.py
 pyaerocom/io/aerocom_browser.py
 pyaerocom/io/aux_read_cubes.py
 pyaerocom/io/cachehandler_ungridded.py
-pyaerocom/io/cachehandler_ungriddedOLD.py
 pyaerocom/io/ebas_file_index.py
 pyaerocom/io/ebas_nasa_ames.py
 pyaerocom/io/ebas_varinfo.py
 pyaerocom/io/fileconventions.py
 pyaerocom/io/helpers.py
 pyaerocom/io/helpers_units.py
 pyaerocom/io/iris_io.py
```

### Comparing `pyaerocom-0.8.0rc3/setup.py` & `pyaerocom-0.8.0rc4/setup.py`

 * *Files identical despite different names*

