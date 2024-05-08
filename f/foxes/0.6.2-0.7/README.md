# Comparing `tmp/foxes-0.6.2.tar.gz` & `tmp/foxes-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxes-0.6.2.tar", last modified: Thu Mar 14 09:42:54 2024, max compression
+gzip compressed data, was "foxes-0.7.tar", last modified: Wed May  8 15:48:07 2024, max compression
```

## Comparing `foxes-0.6.2.tar` & `foxes-0.7.tar`

### file list

```diff
@@ -1,314 +1,314 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.226564 foxes-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-14 09:42:49.000000 foxes-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40774 2024-03-14 09:42:49.000000 foxes-0.6.2/Logo_FOXES.svg
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-14 09:42:49.000000 foxes-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-03-14 09:42:54.226564 foxes-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-03-14 09:42:49.000000 foxes-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.182563 foxes-0.6.2/foxes/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.182563 foxes-0.6.2/foxes/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.182563 foxes-0.6.2/foxes/algorithms/downwind/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/downwind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/downwind/downwind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.182563 foxes-0.6.2/foxes/algorithms/downwind/models/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/downwind/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/downwind/models/calc_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/downwind/models/farm_wakes_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/downwind/models/point_wakes_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/downwind/models/set_amb_farm_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/downwind/models/set_amb_point_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.186564 foxes-0.6.2/foxes/algorithms/iterative/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/iterative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/iterative/iterative.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.186564 foxes-0.6.2/foxes/algorithms/iterative/models/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/iterative/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/iterative/models/convergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/iterative/models/farm_wakes_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/iterative/models/urelax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.186564 foxes-0.6.2/foxes/algorithms/sequential/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/sequential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.186564 foxes-0.6.2/foxes/algorithms/sequential/models/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/sequential/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/sequential/models/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/sequential/models/seq_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    15357 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/algorithms/sequential/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.190564 foxes-0.6.2/foxes/core/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/axial_induction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/data_calc_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/farm_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/farm_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/farm_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14997 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/partial_wakes_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/point_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13680 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/rotor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/turbine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/turbine_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/turbine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/vertical_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/wake_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/wake_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/wake_superposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/core/wind_farm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.190564 foxes-0.6.2/foxes/data/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.190564 foxes-0.6.2/foxes/data/farms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/farms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/farms/test_farm_67.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.190564 foxes-0.6.2/foxes/data/power_ct_curves/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/power_ct_curves/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.194563 foxes-0.6.2/foxes/data/states/
--rw-r--r--   0 runner    (1001) docker     (127)   427815 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/states/WRF-Timeseries-4464.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   126124 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/states/abl_states_6000.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/states/timeseries_100.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)    29085 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/states/timeseries_3000.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)    78694 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/states/timeseries_8000.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/states/wind_rose_bremen.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/states/wind_rotation.nc
--rwxr-xr-x   0 runner    (1001) docker     (127)     3061 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/states/winds100.tab
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/data/static_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.194563 foxes-0.6.2/foxes/input/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.194563 foxes-0.6.2/foxes/input/farm_layout/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/farm_layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/farm_layout/from_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/farm_layout/from_df.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/farm_layout/from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/farm_layout/from_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/farm_layout/from_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/farm_layout/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/farm_layout/row.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.198564 foxes-0.6.2/foxes/input/states/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.198564 foxes-0.6.2/foxes/input/states/create/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/states/create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/states/create/random_abl_states.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/states/create/random_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/states/field_data_nc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/states/multi_height.py
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/states/scan_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/states/single.py
--rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/states/states_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.198564 foxes-0.6.2/foxes/input/windio/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/windio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/input/windio/windio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.198564 foxes-0.6.2/foxes/models/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.198564 foxes-0.6.2/foxes/models/axial_induction_models/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/axial_induction_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/axial_induction_models/betz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/axial_induction_models/madsen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.198564 foxes-0.6.2/foxes/models/farm_controllers/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/farm_controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/farm_controllers/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.198564 foxes-0.6.2/foxes/models/farm_models/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/farm_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/farm_models/turbine2farm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20540 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/model_book.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.202564 foxes-0.6.2/foxes/models/partial_wakes/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/partial_wakes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/partial_wakes/axiwake.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/partial_wakes/centre.py
--rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/partial_wakes/distsliced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/partial_wakes/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/partial_wakes/mapped.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/partial_wakes/rotor_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/partial_wakes/top_hat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.202564 foxes-0.6.2/foxes/models/point_models/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/point_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/point_models/set_uniform_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/point_models/tke2ti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/point_models/wake_deltas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.202564 foxes-0.6.2/foxes/models/rotor_models/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/rotor_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/rotor_models/centre.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/rotor_models/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/rotor_models/levels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.202564 foxes-0.6.2/foxes/models/turbine_models/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_models/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_models/kTI_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_models/lookup_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_models/power_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_models/rotor_centre_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_models/sector_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_models/set_XYHD.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_models/set_farm_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_models/table_factors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_models/thrust2ct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_models/yaw2yawm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_models/yawm2yaw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.206564 foxes-0.6.2/foxes/models/turbine_types/
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_types/CpCt_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_types/CpCt_from_two.py
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_types/PCt_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_types/PCt_from_two.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_types/null_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_types/wsrho2PCt_from_two.py
--rw-r--r--   0 runner    (1001) docker     (127)    12113 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/turbine_types/wsti2PCt_from_two.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.206564 foxes-0.6.2/foxes/models/vertical_profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/vertical_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/vertical_profiles/abl_log_neutral_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/vertical_profiles/abl_log_stable_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/vertical_profiles/abl_log_unstable_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/vertical_profiles/abl_log_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/vertical_profiles/data_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/vertical_profiles/sheared_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/vertical_profiles/uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.206564 foxes-0.6.2/foxes/models/wake_frames/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_frames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_frames/farm_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_frames/rotor_wd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_frames/seq_dynamic_wakes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8894 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_frames/streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_frames/timelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_frames/yawed_wakes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.210564 foxes-0.6.2/foxes/models/wake_models/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/axisymmetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/dist_sliced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.210564 foxes-0.6.2/foxes/models/wake_models/induction/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/induction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/induction/rankine_half_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/induction/rathmann.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/induction/self_similar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/induction/self_similar2020.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.210564 foxes-0.6.2/foxes/models/wake_models/ti/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/ti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/ti/crespo_hernandez.py
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/ti/iec_ti.py
--rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/top_hat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/wake_mirror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.210564 foxes-0.6.2/foxes/models/wake_models/wind/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/wind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/wind/bastankhah14.py
--rw-r--r--   0 runner    (1001) docker     (127)    18709 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/wind/bastankhah16.py
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/wind/jensen.py
--rw-r--r--   0 runner    (1001) docker     (127)    15275 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_models/wind/turbopark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.214564 foxes-0.6.2/foxes/models/wake_superpositions/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_superpositions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_superpositions/ti_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_superpositions/ti_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_superpositions/ti_pow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_superpositions/ti_quadratic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_superpositions/ws_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_superpositions/ws_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_superpositions/ws_pow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_superpositions/ws_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/models/wake_superpositions/ws_quadratic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.214564 foxes-0.6.2/foxes/opt/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.214564 foxes-0.6.2/foxes/opt/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/constraints/area_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/constraints/min_dist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.214564 foxes-0.6.2/foxes/opt/core/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/core/farm_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/core/farm_objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/core/farm_opt_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/core/farm_vars_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/core/pop_states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.214564 foxes-0.6.2/foxes/opt/objectives/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/objectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/objectives/farm_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/objectives/max_n_turbines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.214564 foxes-0.6.2/foxes/opt/problems/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/problems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.214564 foxes-0.6.2/foxes/opt/problems/layout/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/problems/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/problems/layout/farm_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.218564 foxes-0.6.2/foxes/opt/problems/layout/geom_layouts/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/problems/layout/geom_layouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/problems/layout/geom_layouts/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/problems/layout/geom_layouts/geom_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
--rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
--rw-r--r--   0 runner    (1001) docker     (127)    17834 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/problems/layout/geom_layouts/objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/problems/layout/reggrids_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/problems/layout/regular_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    19425 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/opt/problems/opt_farm_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.218564 foxes-0.6.2/foxes/output/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/calc_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    10981 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/farm_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    17663 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/farm_results_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.222564 foxes-0.6.2/foxes/output/flow_plots_2d/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/flow_plots_2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28135 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/flow_plots_2d/flow_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/flow_plots_2d/get_fig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/flow_plots_2d/seq_flow_ani_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/flow_plots_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/results_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11067 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/rose_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/round.py
--rw-r--r--   0 runner    (1001) docker     (127)    31519 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/slice_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/state_turbine_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/output/turbine_type_curves.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.222564 foxes-0.6.2/foxes/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.226564 foxes-0.6.2/foxes/utils/abl/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/abl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/abl/neutral.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/abl/sheared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/abl/stable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/abl/unstable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/cubic_roots.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/data_book.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/exec_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.226564 foxes-0.6.2/foxes/utils/geom2d/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/geom2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19120 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/geom2d/area_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/geom2d/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/geom2d/example_intersection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/geom2d/example_union.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/geom2d/half_plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/geom2d/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/geopandas_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/geopandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/pandas_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/plotly_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/random_xy.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/regularize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.226564 foxes-0.6.2/foxes/utils/runners/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/runners/runners.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/subclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/tab_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/two_circles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/wind_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/windrose_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/utils/xarray_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-03-14 09:42:49.000000 foxes-0.6.2/foxes/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:42:54.226564 foxes-0.6.2/foxes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-03-14 09:42:54.000000 foxes-0.6.2/foxes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-03-14 09:42:54.000000 foxes-0.6.2/foxes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 09:42:54.000000 foxes-0.6.2/foxes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-14 09:42:54.000000 foxes-0.6.2/foxes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-14 09:42:54.000000 foxes-0.6.2/foxes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 09:42:53.000000 foxes-0.6.2/foxes.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-14 09:42:49.000000 foxes-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-14 09:42:54.230564 foxes-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-14 09:42:49.000000 foxes-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.733879 foxes-0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-08 15:47:59.000000 foxes-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40774 2024-05-08 15:47:59.000000 foxes-0.7/Logo_FOXES.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-08 15:47:59.000000 foxes-0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-05-08 15:48:07.733879 foxes-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-08 15:47:59.000000 foxes-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.685878 foxes-0.7/foxes/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 15:47:59.000000 foxes-0.7/foxes/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-08 15:47:59.000000 foxes-0.7/foxes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.685878 foxes-0.7/foxes/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.685878 foxes-0.7/foxes/algorithms/downwind/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/downwind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21612 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/downwind/downwind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.689878 foxes-0.7/foxes/algorithms/downwind/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/downwind/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/downwind/models/farm_wakes_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/downwind/models/init_farm_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/downwind/models/point_wakes_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/downwind/models/reorder_farm_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/downwind/models/set_amb_farm_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/downwind/models/set_amb_point_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.689878 foxes-0.7/foxes/algorithms/iterative/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/iterative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/iterative/iterative.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.689878 foxes-0.7/foxes/algorithms/iterative/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/iterative/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/iterative/models/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/iterative/models/farm_wakes_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/iterative/models/urelax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.689878 foxes-0.7/foxes/algorithms/sequential/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/sequential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.689878 foxes-0.7/foxes/algorithms/sequential/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/sequential/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/sequential/models/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/sequential/models/seq_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16242 2024-05-08 15:47:59.000000 foxes-0.7/foxes/algorithms/sequential/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-08 15:47:59.000000 foxes-0.7/foxes/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.693879 foxes-0.7/foxes/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15169 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/axial_induction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14581 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/data_calc_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/farm_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/farm_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/farm_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17275 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/partial_wakes_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/point_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/rotor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/turbine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/turbine_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/turbine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/vertical_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/wake_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/wake_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/wake_superposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-08 15:47:59.000000 foxes-0.7/foxes/core/wind_farm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.693879 foxes-0.7/foxes/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.693879 foxes-0.7/foxes/data/farms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/farms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/farms/test_farm_67.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.697878 foxes-0.7/foxes/data/power_ct_curves/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/power_ct_curves/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.697878 foxes-0.7/foxes/data/states/
+-rw-r--r--   0 runner    (1001) docker     (127)   427815 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/states/WRF-Timeseries-4464.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126124 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/states/abl_states_6000.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/states/timeseries_100.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    29085 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/states/timeseries_3000.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    78694 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/states/timeseries_8000.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/states/wind_rose_bremen.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/states/wind_rotation.nc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3061 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/states/winds100.tab
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-08 15:47:59.000000 foxes-0.7/foxes/data/static_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.697878 foxes-0.7/foxes/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.701878 foxes-0.7/foxes/input/farm_layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/farm_layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/farm_layout/from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/farm_layout/from_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/farm_layout/from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/farm_layout/from_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/farm_layout/from_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/farm_layout/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/farm_layout/row.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.701878 foxes-0.7/foxes/input/states/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.701878 foxes-0.7/foxes/input/states/create/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/states/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/states/create/random_abl_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/states/create/random_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18693 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/states/field_data_nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/states/multi_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/states/scan_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/states/single.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/states/states_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.701878 foxes-0.7/foxes/input/windio/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/windio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-08 15:47:59.000000 foxes-0.7/foxes/input/windio/windio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.701878 foxes-0.7/foxes/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.705879 foxes-0.7/foxes/models/axial_induction_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/axial_induction_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/axial_induction_models/betz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/axial_induction_models/madsen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.705879 foxes-0.7/foxes/models/farm_controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/farm_controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/farm_controllers/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.705879 foxes-0.7/foxes/models/farm_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/farm_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/farm_models/turbine2farm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21372 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/model_book.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.705879 foxes-0.7/foxes/models/partial_wakes/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/partial_wakes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/partial_wakes/axiwake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/partial_wakes/centre.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/partial_wakes/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/partial_wakes/rotor_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/partial_wakes/segregated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/partial_wakes/top_hat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.705879 foxes-0.7/foxes/models/point_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/point_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/point_models/set_uniform_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/point_models/tke2ti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/point_models/wake_deltas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.705879 foxes-0.7/foxes/models/rotor_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/rotor_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/rotor_models/centre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/rotor_models/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/rotor_models/levels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.709879 foxes-0.7/foxes/models/turbine_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_models/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_models/kTI_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_models/lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_models/power_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_models/rotor_centre_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_models/sector_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_models/set_farm_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_models/table_factors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_models/thrust2ct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_models/yaw2yawm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_models/yawm2yaw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.709879 foxes-0.7/foxes/models/turbine_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_types/CpCt_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_types/CpCt_from_two.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_types/PCt_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_types/PCt_from_two.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_types/null_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11143 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_types/wsrho2PCt_from_two.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/turbine_types/wsti2PCt_from_two.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.713879 foxes-0.7/foxes/models/vertical_profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/vertical_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/vertical_profiles/abl_log_neutral_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/vertical_profiles/abl_log_stable_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/vertical_profiles/abl_log_unstable_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/vertical_profiles/abl_log_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/vertical_profiles/data_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/vertical_profiles/sheared_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/vertical_profiles/uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.713879 foxes-0.7/foxes/models/wake_frames/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_frames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_frames/farm_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_frames/rotor_wd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_frames/seq_dynamic_wakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_frames/streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_frames/timelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_frames/yawed_wakes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.713879 foxes-0.7/foxes/models/wake_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/axisymmetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/dist_sliced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.713879 foxes-0.7/foxes/models/wake_models/induction/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/induction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/induction/rankine_half_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/induction/rathmann.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/induction/self_similar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/induction/self_similar2020.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.717879 foxes-0.7/foxes/models/wake_models/ti/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/ti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/ti/crespo_hernandez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/ti/iec_ti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/top_hat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/wake_mirror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.717879 foxes-0.7/foxes/models/wake_models/wind/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/wind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/wind/bastankhah14.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17629 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/wind/bastankhah16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/wind/jensen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_models/wind/turbopark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.717879 foxes-0.7/foxes/models/wake_superpositions/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_superpositions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_superpositions/ti_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_superpositions/ti_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_superpositions/ti_pow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_superpositions/ti_quadratic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_superpositions/ws_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_superpositions/ws_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_superpositions/ws_pow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_superpositions/ws_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-08 15:47:59.000000 foxes-0.7/foxes/models/wake_superpositions/ws_quadratic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.717879 foxes-0.7/foxes/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.717879 foxes-0.7/foxes/opt/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/constraints/area_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/constraints/min_dist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.721879 foxes-0.7/foxes/opt/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/core/farm_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/core/farm_objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/core/farm_opt_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/core/farm_vars_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/core/pop_states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.721879 foxes-0.7/foxes/opt/objectives/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/objectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/objectives/farm_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/objectives/max_n_turbines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.721879 foxes-0.7/foxes/opt/problems/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/problems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.721879 foxes-0.7/foxes/opt/problems/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/problems/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/problems/layout/farm_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.721879 foxes-0.7/foxes/opt/problems/layout/geom_layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/problems/layout/geom_layouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/problems/layout/geom_layouts/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/problems/layout/geom_layouts/geom_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17834 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/problems/layout/geom_layouts/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/problems/layout/reggrids_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/problems/layout/regular_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19425 2024-05-08 15:47:59.000000 foxes-0.7/foxes/opt/problems/opt_farm_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.725879 foxes-0.7/foxes/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/calc_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10981 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/farm_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17663 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/farm_results_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.725879 foxes-0.7/foxes/output/flow_plots_2d/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/flow_plots_2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28209 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/flow_plots_2d/flow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/flow_plots_2d/get_fig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/flow_plots_2d/seq_flow_ani_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/flow_plots_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/results_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11090 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/rose_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/rotor_point_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/round.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31519 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/slice_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/state_turbine_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-08 15:47:59.000000 foxes-0.7/foxes/output/turbine_type_curves.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.729879 foxes-0.7/foxes/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.729879 foxes-0.7/foxes/utils/abl/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/abl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/abl/neutral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/abl/sheared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/abl/stable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/abl/unstable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/cubic_roots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/data_book.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/exec_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.733879 foxes-0.7/foxes/utils/geom2d/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/geom2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19120 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/geom2d/area_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/geom2d/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/geom2d/example_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/geom2d/example_union.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/geom2d/half_plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/geom2d/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/geopandas_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/geopandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/pandas_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/plotly_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/random_xy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/regularize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.733879 foxes-0.7/foxes/utils/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/runners/runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/tab_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/two_circles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/wind_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/windrose_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-08 15:47:59.000000 foxes-0.7/foxes/utils/xarray_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-08 15:47:59.000000 foxes-0.7/foxes/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:48:07.733879 foxes-0.7/foxes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-05-08 15:48:07.000000 foxes-0.7/foxes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-05-08 15:48:07.000000 foxes-0.7/foxes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:48:07.000000 foxes-0.7/foxes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-08 15:48:07.000000 foxes-0.7/foxes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 15:48:07.000000 foxes-0.7/foxes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:48:07.000000 foxes-0.7/foxes.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-08 15:47:59.000000 foxes-0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-08 15:48:07.733879 foxes-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 15:47:59.000000 foxes-0.7/setup.py
```

### Comparing `foxes-0.6.2/LICENSE` & `foxes-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/Logo_FOXES.svg` & `foxes-0.7/Logo_FOXES.svg`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/PKG-INFO` & `foxes-0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxes
-Version: 0.6.2
+Version: 0.7
 Summary: Farm Optimization and eXtended yield Evaluation Software
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
 Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
@@ -34,14 +34,15 @@
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx-immaterial; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
 Requires-Dist: ipykernel; extra == "doc"
 Requires-Dist: ipywidgets; extra == "doc"
 Requires-Dist: m2r2; extra == "doc"
+Requires-Dist: lxml_html_clean; extra == "doc"
 Provides-Extra: all
 Requires-Dist: windio>=1.0; extra == "all"
 Requires-Dist: flake8; extra == "all"
 Requires-Dist: pytest; extra == "all"
 Requires-Dist: pymoo>=0.6; extra == "all"
 Requires-Dist: sphinx; extra == "all"
 Requires-Dist: sphinx-immaterial; extra == "all"
@@ -98,24 +99,23 @@
     volume = {8}, 
     number = {86}, 
     pages = {5464}, 
     journal = {Journal of Open Source Software} 
 }
  ```
 
-## Requirements
+## Installation via pip
 
 The supported Python versions are: 
 
 - `Python 3.8`
 - `Python 3.9`
 - `Python 3.10`
 - `Python 3.11`
-
-## Installation via pip
+- `Python 3.12`
 
 ### Virtual Python environment
 
 First create a new `venv` environment, for example called `foxes` and located at `~/venv/foxes` (choose any other convenient name and location in your file system if you prefer), by
 
 ```console
 python3 -m venv ~/venv/foxes
@@ -158,14 +158,22 @@
 cd foxes
 pip install -e .
 ```
 The last line makes sure that all your code changes are included whenever importing `foxes`. Concerning the `git clone` line, we actually recommend that you fork `foxes` on GitHub and then replace that command by cloning your fork instead.
 
 ## Installation via conda
 
+The supported Python versions are: 
+
+- `Python 3.8`
+- `Python 3.9`
+- `Python 3.10`
+- `Python 3.11`
+- `Python 3.12`
+
 ### Preparation
 
 It is strongly recommend to use the `libmamba` dependency solver instead of the default solver. Install it once by
 
 ```console
 conda install conda-libmamba-solver -n base -c conda-forge
 ```
@@ -229,20 +237,18 @@
 For detailed examples of how to run _foxes_, check the `examples` and `notebooks` folders in this repository. A minimal running example is the following, based on provided static `csv` data files:
 
 ```python
 import foxes
 
 states = foxes.input.states.Timeseries("timeseries_3000.csv.gz", ["WS", "WD","TI","RHO"])
 
-mbook = foxes.ModelBook()
-
 farm = foxes.WindFarm()
 foxes.input.farm_layout.add_from_file(farm, "test_farm_67.csv", turbine_models=["NREL5MW"])
 
-algo = foxes.algorithms.Downwind(mbook, farm, states, ["Jensen_linear_k007"])
+algo = foxes.algorithms.Downwind(farm, states, ["Jensen_linear_k007"])
 farm_results = algo.calc_farm()
 
 print(farm_results)
 ```
 
 ## Testing
```

### Comparing `foxes-0.6.2/README.md` & `foxes-0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,24 +45,23 @@
     volume = {8}, 
     number = {86}, 
     pages = {5464}, 
     journal = {Journal of Open Source Software} 
 }
  ```
 
-## Requirements
+## Installation via pip
 
 The supported Python versions are: 
 
 - `Python 3.8`
 - `Python 3.9`
 - `Python 3.10`
 - `Python 3.11`
-
-## Installation via pip
+- `Python 3.12`
 
 ### Virtual Python environment
 
 First create a new `venv` environment, for example called `foxes` and located at `~/venv/foxes` (choose any other convenient name and location in your file system if you prefer), by
 
 ```console
 python3 -m venv ~/venv/foxes
@@ -105,14 +104,22 @@
 cd foxes
 pip install -e .
 ```
 The last line makes sure that all your code changes are included whenever importing `foxes`. Concerning the `git clone` line, we actually recommend that you fork `foxes` on GitHub and then replace that command by cloning your fork instead.
 
 ## Installation via conda
 
+The supported Python versions are: 
+
+- `Python 3.8`
+- `Python 3.9`
+- `Python 3.10`
+- `Python 3.11`
+- `Python 3.12`
+
 ### Preparation
 
 It is strongly recommend to use the `libmamba` dependency solver instead of the default solver. Install it once by
 
 ```console
 conda install conda-libmamba-solver -n base -c conda-forge
 ```
@@ -176,20 +183,18 @@
 For detailed examples of how to run _foxes_, check the `examples` and `notebooks` folders in this repository. A minimal running example is the following, based on provided static `csv` data files:
 
 ```python
 import foxes
 
 states = foxes.input.states.Timeseries("timeseries_3000.csv.gz", ["WS", "WD","TI","RHO"])
 
-mbook = foxes.ModelBook()
-
 farm = foxes.WindFarm()
 foxes.input.farm_layout.add_from_file(farm, "test_farm_67.csv", turbine_models=["NREL5MW"])
 
-algo = foxes.algorithms.Downwind(mbook, farm, states, ["Jensen_linear_k007"])
+algo = foxes.algorithms.Downwind(farm, states, ["Jensen_linear_k007"])
 farm_results = algo.calc_farm()
 
 print(farm_results)
 ```
 
 ## Testing
```

### Comparing `foxes-0.6.2/foxes/__init__.py` & `foxes-0.7/foxes/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/algorithms/downwind/downwind.py` & `foxes-0.7/foxes/algorithms/downwind/downwind.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,139 +14,192 @@
     that is calculated by the provided `TurbineOrder`
     object.
 
     Attributes
     ----------
     states: foxes.core.States
         The ambient states
-    wake_models: list of foxes.core.WakeModel
-        The wake models, applied to all turbines
+    wake_models: dict
+        The wake models. Key: wake model name,
+        value: foxes.core.WakeModel
     rotor_model: foxes.core.RotorModel
         The rotor model, for all turbines
     wake_frame: foxes.core.WakeFrame
         The wake frame
-    partial_wakes_model: foxes.core.PartialWakesModel
-        The partial wakes model
+    partial_wakes: dict
+        The partial wakes mapping. Key: wake model name,
+        value: foxes.core.PartialWakesModel
     farm_controller: foxes.core.FarmController
         The farm controller
     n_states: int
         The number of states
 
     :group: algorithms.downwind
 
     """
 
-    @classmethod
-    def get_model(cls, name):
-        """
-        Get the algorithm specific model
-
-        Parameters
-        ----------
-        name: str
-            The model name
-
-        Returns
-        -------
-        model: foxes.core.model
-            The model
-
-        """
-        return getattr(mdls, name)
+    DEFAULT_FARM_OUTPUTS = [
+        FV.X,
+        FV.Y,
+        FV.H,
+        FV.D,
+        FV.AMB_WD,
+        FV.AMB_REWS,
+        FV.AMB_TI,
+        FV.AMB_RHO,
+        FV.AMB_P,
+        FV.WD,
+        FV.REWS,
+        FV.YAW,
+        FV.TI,
+        FV.CT,
+        FV.P,
+        FV.ORDER,
+        FV.WEIGHT,
+    ]
 
     def __init__(
         self,
-        mbook,
         farm,
         states,
         wake_models,
         rotor_model="centre",
         wake_frame="rotor_wd",
-        partial_wakes_model="auto",
+        partial_wakes=None,
         farm_controller="basic_ctrl",
-        chunks={FC.STATE: 1000, FC.POINT: 10000},
+        chunks={FC.STATE: 1000, FC.POINT: 4000},
         wake_mirrors={},
+        mbook=None,
         dbook=None,
         verbosity=1,
     ):
         """
         Constructor.
 
         Parameters
         ----------
-        mbook: foxes.ModelBook
-            The model book
         farm: foxes.WindFarm
             The wind farm
         states: foxes.core.States
             The ambient states
         wake_models: list of str
             The wake models, applied to all turbines.
             Will be looked up in the model book
         rotor_model: str
             The rotor model, for all turbines. Will be
             looked up in the model book
         wake_frame: str
             The wake frame. Will be looked up in the
             model book
-        partial_wakes_model: str
-            The partial wakes model. Will be
-            looked up in the model book
+        partial_wakes: dict, list or str, optional
+            The partial wakes mapping. Key: wake model name,
+            value: partial wake model name
         farm_controller: str
             The farm controller. Will be
             looked up in the model book
         chunks: dict
             The chunks choice for running in parallel with dask,
             e.g. `{"state": 1000}` for chunks of 1000 states
         wake_mirrors: dict
             Switch on wake mirrors for wake models.
             Key: wake model name, value: list of heights
+        mbook: foxes.ModelBook, optional
+            The model book
         dbook: foxes.DataBook, optional
             The data book, or None for default
         verbosity: int
             The verbosity level, 0 means silent
 
         """
+        if mbook is None:
+            mbook = fm.ModelBook()
+
         super().__init__(mbook, farm, chunks, verbosity, dbook)
 
         self.states = states
         self.n_states = None
         self.states_data = None
 
         self.rotor_model = self.mbook.rotor_models[rotor_model]
         self.rotor_model.name = rotor_model
 
-        self.partial_wakes_model = self.mbook.partial_wakes[partial_wakes_model]
-        self.partial_wakes_model.name = partial_wakes_model
-
         self.wake_frame = self.mbook.wake_frames[wake_frame]
         self.wake_frame.name = wake_frame
 
-        self.wake_models = []
+        self.wake_models = {}
         for w in wake_models:
             m = self.mbook.wake_models[w]
             m.name = w
 
             # optionally add wake mirrors:
             if w in wake_mirrors:
                 hts = wake_mirrors[w]
                 if isinstance(m, fm.wake_models.WakeMirror):
                     if list(m.heights) != list(hts):
                         raise ValueError(
                             f"Wake model '{w}' is mirrored with heights {m.heights}, cannot apply WakeMirror with heights {hts}"
                         )
                 else:
-                    self.wake_models.append(fm.wake_models.WakeMirror(m, heights=hts))
+                    self.wake_models[w] = fm.wake_models.WakeMirror(m, heights=hts)
 
             else:
-                self.wake_models.append(m)
+                self.wake_models[w] = m
+
+        self.partial_wakes = {}
+        if partial_wakes is None:
+            partial_wakes = {}
+        if isinstance(partial_wakes, list) and len(partial_wakes) == 1:
+            partial_wakes = partial_wakes[0]
+        if isinstance(partial_wakes, str):
+            for w in wake_models:
+                try:
+                    pw = partial_wakes
+                except TypeError:
+                    pw = mbook.default_partial_wakes(self.wake_models[w])
+                self.partial_wakes[w] = self.mbook.partial_wakes[pw]
+                self.partial_wakes[w].name = pw
+        elif isinstance(partial_wakes, list):
+            for i, w in enumerate(wake_models):
+                if i >= len(partial_wakes):
+                    raise IndexError(
+                        f"Not enough partial wakes in list {partial_wakes}, expecting {len(wake_models)}"
+                    )
+                pw = partial_wakes[i]
+                self.partial_wakes[w] = self.mbook.partial_wakes[pw]
+                self.partial_wakes[w].name = pw
+        else:
+            for w in wake_models:
+                if w in partial_wakes:
+                    pw = partial_wakes[w]
+                else:
+                    pw = mbook.default_partial_wakes(self.wake_models[w])
+                self.partial_wakes[w] = self.mbook.partial_wakes[pw]
+                self.partial_wakes[w].name = pw
 
         self.farm_controller = self.mbook.farm_controllers[farm_controller]
         self.farm_controller.name = farm_controller
 
+    @classmethod
+    def get_model(cls, name):
+        """
+        Get the algorithm specific model
+
+        Parameters
+        ----------
+        name: str
+            The model name
+
+        Returns
+        -------
+        model: foxes.core.model
+            The model
+
+        """
+        return getattr(mdls, name)
+
     def _print_deco(self, func_name, n_points=None):
         """
         Helper function for printing model names
         """
         if self.verbosity > 0:
             deco = "-" * 50
             print(f"\n{deco}")
@@ -156,21 +209,24 @@
             print(f"  n_turbines: {self.n_turbines}")
             if n_points is not None:
                 print(f"  n_points : {n_points}")
             print(deco)
             print(f"  states   : {self.states}")
             print(f"  rotor    : {self.rotor_model}")
             print(f"  controller: {self.farm_controller}")
-            print(f"  partialwks: {self.partial_wakes_model}")
             print(f"  wake frame: {self.wake_frame}")
             print(deco)
             print(f"  wakes:")
-            for i, w in enumerate(self.wake_models):
+            for i, w in enumerate(self.wake_models.values()):
                 print(f"    {i}) {w}")
             print(deco)
+            print(f"  partial wakes:")
+            for i, (w, p) in enumerate(self.partial_wakes.items()):
+                print(f"    {i}) {w}: {p}")
+            print(deco)
             print(f"  turbine models:")
             for i, m in enumerate(self.farm_controller.pre_rotor_models.models):
                 print(f"    {i}) {m} [pre-rotor]")
             for i, m in enumerate(self.farm_controller.post_rotor_models.models):
                 print(f"    {i+len(self.farm_controller.pre_rotor_models.models)}) {m}")
             print(deco)
             print()
@@ -222,16 +278,17 @@
 
         """
         mdls = [self.states] if with_states else []
         mdls += [
             self.rotor_model,
             self.farm_controller,
             self.wake_frame,
-            self.partial_wakes_model,
-        ] + self.wake_models
+        ]
+        mdls += list(self.wake_models.values())
+        mdls += list(self.partial_wakes.values())
 
         return mdls
 
     def initialize(self):
         """
         Initializes the algorithm.
         """
@@ -241,89 +298,85 @@
         self.init_states()
 
         for m in self.all_models(with_states=False):
             m.initialize(self, self.verbosity)
 
     def _collect_farm_models(
         self,
+        outputs,
         calc_parameters,
         ambient,
     ):
         """
         Helper function that creates model list
         """
         # prepare:
         calc_pars = []
-        t2f = fm.farm_models.Turbine2FarmModel
         mlist = FarmDataModelList(models=[])
         mlist.name = f"{self.name}_calc"
 
-        # 0) set XHYD:
-        m = fm.turbine_models.SetXYHD()
-        mlist.models.append(t2f(m))
-        calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
-
-        # 1) run pre-rotor turbine models via farm controller:
+        # 0) run pre-rotor turbine models via farm controller:
         mlist.models.append(self.farm_controller)
         calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
         calc_pars[-1]["pre_rotor"] = True
 
-        # 2) calculate yaw from wind direction at rotor centre:
-        mlist.models.append(fm.rotor_models.CentreRotor(calc_vars=[FV.WD, FV.YAW]))
-        mlist.models[-1].name = "calc_yaw_" + mlist.models[-1].name
+        # 1) set initial data:
+        mlist.models.append(self.get_model("InitFarmData")())
         calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
 
-        # 3) calculate ambient rotor results:
+        # 2) calculate ambient rotor results:
         mlist.models.append(self.rotor_model)
         calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
         calc_pars[-1].update(
             {"store_rpoints": True, "store_rweights": True, "store_amb_res": True}
         )
 
-        # 4) calculate turbine order:
-        mlist.models.append(self.get_model("CalcOrder")())
-        calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
-
-        # 5) run post-rotor turbine models via farm controller:
+        # 3) run post-rotor turbine models via farm controller:
         mlist.models.append(self.farm_controller)
         calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
         calc_pars[-1]["pre_rotor"] = False
 
-        # 6) copy results to ambient, requires self.farm_vars:
+        # 4) copy results to ambient, requires self.farm_vars:
         self.farm_vars = mlist.output_farm_vars(self)
         mlist.models.append(self.get_model("SetAmbFarmResults")())
         calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
 
-        # 7) calculate wake effects:
+        # 5) calculate wake effects:
         if not ambient:
             mlist.models.append(self.get_model("FarmWakesCalculation")())
             calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
 
+        # 6) reorder back to state-turbine dimensions:
+        if outputs != False:
+            mlist.models.append(self.get_model("ReorderFarmOutput")(outputs))
+            calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
+
         return mlist, calc_pars
 
     def _calc_farm_vars(self, mlist):
         """Helper function that gathers the farm variables"""
         self.farm_vars = sorted(list(set([FV.WEIGHT] + mlist.output_farm_vars(self))))
 
-    def _run_farm_calc(self, mlist, *data, **kwargs):
+    def _run_farm_calc(self, mlist, *data, outputs=None, **kwargs):
         """Helper function for running the main farm calculation"""
         self.print(
             f"\nCalculating {self.n_states} states for {self.n_turbines} turbines"
         )
-        farm_results = mlist.run_calculation(
-            self, *data, out_vars=self.farm_vars, **kwargs
-        )
+        out_vars = self.farm_vars if outputs is None else outputs
+        farm_results = mlist.run_calculation(self, *data, out_vars=out_vars, **kwargs)
         farm_results[FC.TNAME] = ((FC.TURBINE,), self.farm.turbine_names)
-        if FV.ORDER in farm_results:
-            farm_results[FV.ORDER] = farm_results[FV.ORDER].astype(FC.ITYPE)
+        for v in [FV.ORDER, FV.ORDER_SSEL, FV.ORDER_INV]:
+            if v in farm_results:
+                farm_results[v] = farm_results[v].astype(FC.ITYPE)
 
         return farm_results
 
     def calc_farm(
         self,
+        outputs=None,
         calc_parameters={},
         persist=True,
         finalize=True,
         ambient=False,
         chunked_results=False,
         **kwargs,
     ):
@@ -331,14 +384,16 @@
         Calculate farm data.
 
         Parameters
         ----------
         calc_parameters: dict
             Parameters for model calculation.
             Key: model name str, value: parameter dict
+        outputs: list of str, optional
+            The output variables, or None for defaults
         persist: bool
             Switch for forcing dask to load all model data
             into memory
         finalize: bool
             Flag for finalization after calculation
         ambient: bool
             Flag for ambient instead of waked calculation
@@ -358,35 +413,45 @@
         if not self.initialized:
             self.initialize()
 
         # welcome:
         self._print_deco("calc_farm")
 
         # collect models:
-        mlist, calc_pars = self._collect_farm_models(calc_parameters, ambient)
+        if outputs == "default":
+            outputs = self.DEFAULT_FARM_OUTPUTS
+        mlist, calc_pars = self._collect_farm_models(outputs, calc_parameters, ambient)
 
         # initialize models:
         if not mlist.initialized:
             mlist.initialize(self, self.verbosity)
             self._calc_farm_vars(mlist)
         self._print_model_oder(mlist, calc_pars)
 
+        # update outputs:
+        if outputs is None:
+            outputs = self.farm_vars
+        else:
+            outputs = sorted(list(set(outputs).intersection(self.farm_vars)))
+
         # get input model data:
         models_data = self.get_models_data()
         if persist:
             models_data = models_data.persist()
         self.print("\nInput data:\n\n", models_data, "\n")
-        self.print(f"\nOutput farm variables:", ", ".join(self.farm_vars))
+        self.print(f"\nFarm variables:", ", ".join(self.farm_vars))
+        self.print(f"\nOutput variables:", ", ".join(outputs))
         self.print(f"\nChunks: {self.chunks}\n")
 
         # run main calculation:
         farm_results = self._run_farm_calc(
             mlist,
             models_data,
             parameters=calc_pars,
+            outputs=outputs,
             **kwargs,
         )
         del models_data
 
         # finalize models:
         if finalize:
             self.print("\n")
@@ -555,14 +620,15 @@
         self.print(f"\nOutput point variables:", ", ".join(ovars))
         self.print(f"\nChunks: {self.chunks}\n")
 
         # calculate:
         self.print(
             f"Calculating {len(ovars)} variables at {points.shape[1]} points in {self.n_states} states"
         )
+
         point_results = mlist.run_calculation(
             self,
             models_data,
             farm_results,
             point_data,
             out_vars=ovars,
             parameters=calc_pars,
```

### Comparing `foxes-0.6.2/foxes/algorithms/downwind/models/calc_order.py` & `foxes-0.7/foxes/algorithms/downwind/models/set_amb_point_results.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,88 @@
 import foxes.variables as FV
-from foxes.core import FarmDataModel
+from foxes.core import PointDataModel
 
 
-class CalcOrder(FarmDataModel):
+class SetAmbPointResults(PointDataModel):
     """
-    This model calculates the turbine evaluation
-    order, via wake frames.
+    This model copies point results to ambient results.
+
+    Attributes
+    ----------
+    pvars: list of str
+        The point variables to be treated
+    vars: list of str
+        The variables to be copied to output
 
     :group: algorithms.downwind.models
 
     """
 
-    def sub_models(self):
+    def __init__(self):
         """
-        List of all sub-models
-
-        Returns
-        -------
-        smdls: list of foxes.core.Model
-            Names of all sub models
-
+        Constructor.
         """
-        return [self._wframe]
+        super().__init__()
+        self.pvars = None
+        self.vars = None
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         verbosity: int
             The verbosity level, 0 = silent
 
         """
-        self._wframe = algo.wake_frame
+        self.pvars = algo.states.output_point_vars(algo)
+        self.vars = [v for v in self.pvars if v in FV.var2amb]
         super().initialize(algo, verbosity)
 
-    def output_farm_vars(self, algo):
+    def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
         output_vars: list of str
             The output variable names
 
         """
-        return [FV.ORDER]
+        return [FV.var2amb[v] for v in self.vars]
 
-    def calculate(self, algo, mdata, fdata):
+    def calculate(self, algo, mdata, fdata, pdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The point data
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_turbines)
+            Values: numpy.ndarray with shape (n_states, n_points)
 
         """
-        return {FV.ORDER: self._wframe.calc_order(algo, mdata, fdata)}
+        for v in self.vars:
+            pdata[FV.var2amb[v]] = pdata[v].copy()
+        return {v: pdata[v] for v in self.output_point_vars(algo)}
```

### Comparing `foxes-0.6.2/foxes/algorithms/downwind/models/farm_wakes_calc.py` & `foxes-0.7/foxes/models/turbine_models/thrust2ct.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,47 @@
 import numpy as np
 
+from foxes.core import TurbineModel
 import foxes.variables as FV
-from foxes.core import FarmDataModel
 
 
-class FarmWakesCalculation(FarmDataModel):
+class Thrust2Ct(TurbineModel):
     """
-    This model calculates wakes effects on farm data.
+    Calculates ct from thrust force data.
 
-    :group: algorithms.downwind.models
+    Attributes
+    ----------
+    thrust_var: str
+        Name of the thrust variable
+    WSCT: str
+        The wind speed variable for ct lookup
+
+    :group: models.turbine_models
 
     """
 
-    def __init__(self):
+    def __init__(self, thrust_var=FV.T, var_ws_ct=FV.REWS2):
         """
         Constructor.
+
+        Parameters
+        ----------
+        thrust_var: str
+            Name of the thrust variable
+        var_ws_ct: str
+            The wind speed variable for ct lookup
+
         """
         super().__init__()
+        self.thrust_var = thrust_var
+        self.WSCT = var_ws_ct
+
+    def __repr__(self):
+        a = f"thrust_var={self.thrust_var}, var_ws_ct={self.WSCT}"
+        return f"{type(self).__name__}({a})"
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
@@ -29,92 +50,45 @@
 
         Returns
         -------
         output_vars: list of str
             The output variable names
 
         """
-        ovars = algo.rotor_model.output_farm_vars(
-            algo
-        ) + algo.farm_controller.output_farm_vars(algo)
-        return list(dict.fromkeys(ovars))
+        return [FV.CT]
 
-    def sub_models(self):
+    def calculate(self, algo, mdata, fdata, st_sel):
         """
-        List of all sub-models
-
-        Returns
-        -------
-        smdls: list of foxes.core.Model
-            Names of all sub models
-
-        """
-        return [self.pwakes]
-
-    def initialize(self, algo, verbosity=0):
-        """
-        Initializes the model.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
-
-        """
-        self.pwakes = algo.partial_wakes_model
-        super().initialize(algo, verbosity)
-
-    def calculate(self, algo, mdata, fdata):
-        """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
+        st_sel: slice or numpy.ndarray of bool
+            The state-turbine selection,
+            for shape: (n_states, n_turbines)
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
-        torder = fdata[FV.ORDER]
-        n_order = torder.shape[1]
-        n_states = mdata.n_states
-
-        def _evaluate(algo, mdata, fdata, pdata, wdeltas, o):
-            self.pwakes.evaluate_results(
-                algo, mdata, fdata, pdata, wdeltas, states_turbine=o
-            )
-
-            trbs = np.zeros((n_states, algo.n_turbines), dtype=bool)
-            np.put_along_axis(trbs, o[:, None], True, axis=1)
-
-            res = algo.farm_controller.calculate(
-                algo, mdata, fdata, pre_rotor=False, st_sel=trbs
-            )
-            fdata.update(res)
-
-        wdeltas, pdata = self.pwakes.new_wake_deltas(algo, mdata, fdata)
-        for oi in range(n_order):
-            o = torder[:, oi]
-
-            if oi > 0:
-                _evaluate(algo, mdata, fdata, pdata, wdeltas, o)
-
-            if oi < n_order - 1:
-                self.pwakes.contribute_to_wake_deltas(
-                    algo, mdata, fdata, pdata, o, wdeltas
-                )
+        ct = fdata[FV.CT]
+
+        T = fdata[self.thrust_var][st_sel]
+        rho = fdata[FV.RHO][st_sel]
+        A = np.pi * (fdata[FV.D][st_sel] / 2) ** 2
+        ws = fdata[self.WSCT][st_sel]
+
+        ct[st_sel] = 2 * T / (rho * A * ws**2)
 
-        return {v: fdata[v] for v in self.output_farm_vars(algo)}
+        return {FV.CT: ct}
```

### Comparing `foxes-0.6.2/foxes/algorithms/downwind/models/point_wakes_calc.py` & `foxes-0.7/foxes/opt/core/pop_states.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,140 +1,168 @@
-import foxes.variables as FV
+import numpy as np
+
+from foxes.core import States, Data
 import foxes.constants as FC
-from foxes.core import PointDataModel
+import foxes.variables as FV
 
 
-class PointWakesCalculation(PointDataModel):
+class PopStates(States):
     """
-    This model calculates wake effects at points of interest.
+    Helper class for vectorized opt population
+    calculation, via artificial states of length
+    n_pop times n_states.
 
     Attributes
     ----------
-    pvars: list of str
-        The variables of interest
-    emodels: foxes.core.PointDataModelList
-        The extra evaluation models
-    emodels_cpars: list of dict
-        The calculation parameters for extra models
-    wake_models: list of foxes.core.WakeModel
-        The wake models, default: from algo
+    states: foxes.core.States
+        The original states
+    n_pop: int
+        The population size
 
-    :group: algorithms.downwind.models
+    :group: opt.core
 
     """
 
-    def __init__(self, emodels=None, emodels_cpars=None, wake_models=None):
+    def __init__(self, states, n_pop):
         """
         Constructor.
 
         Parameters
         ----------
-        emodels: foxes.core.PointDataModelList, optional
-            The extra evaluation models
-        emodels_cpars: list of dict, optional
-            The calculation parameters for extra models
-        wake_models: list of foxes.core.WakeModel, optional
-            The wake models, default: from algo
+        states: foxes.core.States
+            The original states
+        n_pop: int
+            The population size
 
         """
         super().__init__()
-        self.pvars = None
-        self.emodels = emodels
-        self.emodels_cpars = emodels_cpars
-        self.wake_models = wake_models
+        self.states = states
+        self.n_pop = n_pop
 
-    def sub_models(self):
+    def load_data(self, algo, verbosity=0):
         """
-        List of all sub-models
+        Load and/or create all model data that is subject to chunking.
+
+        Such data should not be stored under self, for memory reasons. The
+        data returned here will automatically be chunked and then provided
+        as part of the mdata object during calculations.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        verbosity: int
+            The verbosity level, 0 = silent
 
         Returns
         -------
-        smdls: list of foxes.core.Model
-            Names of all sub models
+        idata: dict
+            The dict has exactly two entries: `data_vars`,
+            a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
+            and `coords`, a dict with entries `dim_name_str -> dim_array`
+
+        """
+        self.STATE0 = self.var(FC.STATE + "0")
+        self.SMAP = self.var("SMAP")
+
+        idata = super().load_data(algo, verbosity)
+        idata0 = algo.get_model_data(self.states)
+        for cname, coord in idata0["coords"].items():
+            if cname != FC.STATE:
+                idata["coords"][cname] = coord
+            else:
+                idata["coords"][self.STATE0] = coord
+
+        for dname, (dims0, data0) in idata0["data_vars"].items():
+            if dname != FV.WEIGHT:
+                hdims = tuple([d if d != FC.STATE else self.STATE0 for d in dims0])
+                idata["data_vars"][dname] = (hdims, data0)
+
+        smap = np.zeros((self.n_pop, self.states.size()), dtype=np.int32)
+        smap[:] = np.arange(self.states.size())[None, :]
+        smap = smap.reshape(self.size())
+        idata["data_vars"][self.SMAP] = ((FC.STATE,), smap)
+
+        found = False
+        for dname, (dims0, data0) in idata["data_vars"].items():
+            if self.STATE0 in dims0:
+                found = True
+                break
+        if not found:
+            del idata["coords"][self.STATE0]
 
-        """
-        return [self.emodels] if self.emodels is not None else []
+        return idata
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         verbosity: int
             The verbosity level, 0 = silent
 
         """
+        if not self.states.initialized:
+            self.states.initialize(algo, verbosity)
         super().initialize(algo, verbosity)
-        self.pvars = algo.states.output_point_vars(algo)
 
-    def output_point_vars(self, algo):
+    def size(self):
         """
-        The variables which are being modified by the model.
+        The total number of states.
+
+        Returns
+        -------
+        int:
+            The total number of states
+
+        """
+        return self.states.size() * self.n_pop
+
+    def weights(self, algo):
+        """
+        The statistical weights of all states.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars: list of str
-            The output variable names
+        weights: numpy.ndarray
+            The weights, shape: (n_states, n_turbines)
 
         """
-        return self.pvars
+        weights = np.zeros(
+            (self.n_pop, self.states.size(), algo.n_turbines), dtype=FC.DTYPE
+        )
+        weights[:] = self.states.weights(algo)[None, :, :] / self.n_pop
+        return weights.reshape(self.size(), algo.n_turbines)
 
-    def contribute_to_wake_deltas(
-        self,
-        algo,
-        mdata,
-        fdata,
-        pdata,
-        states_source_turbine,
-        wmodels,
-        wdeltas,
-    ):
+    def output_point_vars(self, algo):
         """
-        Contribute to wake deltas from source turbines
+        The variables which are being modified by the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        pdata: foxes.core.Data
-            The point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        wmodels: list of foxes.core.WakeModel
-            The wake models
-        wdeltas: dict
-            The wake deltas, are being modified ob the fly.
-            Key: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
 
-        """
-        wcoos = algo.wake_frame.get_wake_coos(
-            algo, mdata, fdata, pdata, states_source_turbine
-        )
+        Returns
+        -------
+        output_vars: list of str
+            The output variable names
 
-        for w in wmodels:
-            w.contribute_to_wake_deltas(
-                algo, mdata, fdata, pdata, states_source_turbine, wcoos, wdeltas
-            )
+        """
+        return self.states.output_point_vars(algo)
 
-    def calculate(self, algo, mdata, fdata, pdata, states_source_turbine=None):
+    def calculate(self, algo, mdata, fdata, pdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
@@ -143,57 +171,36 @@
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
         pdata: foxes.core.Data
             The point data
-        states_source_turbine: numpy.ndarray, optional
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,).
-            Default: include all turbines
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
 
-        torder = fdata[FV.ORDER].astype(FC.ITYPE)
-        n_order = torder.shape[1]
-        wake_models = algo.wake_models if self.wake_models is None else self.wake_models
-
-        wdeltas = {}
-        wmodels = []
-        for w in wake_models:
-            hdeltas = {}
-            w.init_wake_deltas(algo, mdata, fdata, pdata, hdeltas)
-            if len(set(self.pvars).intersection(hdeltas.keys())):
-                wdeltas.update(hdeltas)
-                wmodels.append(w)
-            del hdeltas
-
-        if states_source_turbine is None:
-            for oi in range(n_order):
-                o = torder[:, oi]
-                self.contribute_to_wake_deltas(
-                    algo, mdata, fdata, pdata, o, wmodels, wdeltas
+        hdata = {}
+        hdims = {}
+        smap = mdata[self.SMAP]
+        for dname, data in mdata.items():
+            dms = mdata.dims[dname]
+            if dname == self.SMAP or dname == self.STATE0:
+                pass
+            elif dms[0] == self.STATE0:
+                hdata[dname] = data[smap]
+                hdims[dname] = tuple([FC.STATE] + list(dms)[1:])
+            elif self.STATE0 in dms:
+                raise ValueError(
+                    f"States '{self.name}': Found states variable not at dimension 0 for mdata entry '{dname}': {dms}"
                 )
-        else:
-            self.contribute_to_wake_deltas(
-                algo, mdata, fdata, pdata, states_source_turbine, wmodels, wdeltas
-            )
-
-        amb_res = {v: pdata[FV.var2amb[v]] for v in wdeltas if v in FV.var2amb}
-        for w in wmodels:
-            w.finalize_wake_deltas(algo, mdata, fdata, pdata, amb_res, wdeltas)
-
-        for v in self.pvars:
-            if v in wdeltas:
-                pdata[v] = amb_res[v] + wdeltas[v]
-
-        if self.emodels is not None:
-            self.emodels.calculate(algo, mdata, fdata, pdata, self.emodels_cpars)
+            else:
+                hdata[dname] = data
+                hdims[dname] = dms
+        hmdata = Data(hdata, hdims, mdata.loop_dims)
 
-        return {v: pdata[v] for v in self.pvars}
+        return self.states.calculate(algo, hmdata, fdata, pdata)
```

### Comparing `foxes-0.6.2/foxes/algorithms/downwind/models/set_amb_farm_results.py` & `foxes-0.7/foxes/algorithms/downwind/models/set_amb_farm_results.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/algorithms/downwind/models/set_amb_point_results.py` & `foxes-0.7/foxes/models/point_models/wake_deltas.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,42 @@
-import foxes.variables as FV
 from foxes.core import PointDataModel
+import foxes.variables as FV
 
 
-class SetAmbPointResults(PointDataModel):
+class WakeDeltas(PointDataModel):
     """
-    This model copies point results to ambient results.
+    This point model simply subtracts ambient results
+    from waked results.
 
     Attributes
     ----------
-    pvars: list of str
-        The point variables to be treated
     vars: list of str
-        The variables to be copied to output
+        The variables
+    normalize: bool
+        Divide resulting deltas by ambient values
 
-    :group: algorithms.downwind.models
+    :group: models.point_models
 
     """
 
-    def __init__(self):
+    def __init__(self, vars, normalize=False):
         """
         Constructor.
-        """
-        super().__init__()
-        self.pvars = None
-        self.vars = None
-
-    def initialize(self, algo, verbosity=0):
-        """
-        Initializes the model.
 
         Parameters
         ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
+        vars: list of str
+            The variables
+        normalize: bool
+            Divide resulting deltas by ambient values
 
         """
-        self.pvars = algo.states.output_point_vars(algo)
-        self.vars = [v for v in self.pvars if v in FV.var2amb]
-        super().initialize(algo, verbosity)
+        super().__init__()
+        self.vars = vars
+        self.normalize = normalize
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
@@ -52,37 +45,42 @@
 
         Returns
         -------
         output_vars: list of str
             The output variable names
 
         """
-        return [FV.var2amb[v] for v in self.vars]
+        return [f"DELTA_{v}" for v in self.vars]
 
     def calculate(self, algo, mdata, fdata, pdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The point data
+        tdata: foxes.core.TData
+            The target point data
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
-        for v in self.vars:
-            pdata[FV.var2amb[v]] = pdata[v].copy()
-        return {v: pdata[v] for v in self.output_point_vars(algo)}
+
+        out = {f"DELTA_{v}": pdata[v] - pdata[FV.var2amb[v]] for v in self.vars}
+
+        if self.normalize:
+            for v in self.vars:
+                out[v] /= pdata[FV.var2amb[v]]
+
+        return out
```

### Comparing `foxes-0.6.2/foxes/algorithms/iterative/iterative.py` & `foxes-0.7/foxes/algorithms/iterative/iterative.py`

 * *Files 22% similar despite different names*

```diff
@@ -40,43 +40,46 @@
 
         """
         try:
             return getattr(mdls, name)
         except AttributeError:
             return super().get_model(name)
 
-    def __init__(self, *args, max_it=None, conv_crit=None, **kwargs):
+    def __init__(self, *args, max_it=None, conv_crit="default", mod_cutin={}, **kwargs):
         """
         Constructor.
 
         Parameters
         ----------
         args: tuple, optional
             Arguments for Downwind
         max_it: int, optional
             The maximal number of iterations
         conv_crit: foxes.algorithms.iterative.ConvCrit, optional
             The convergence criteria
+        mod_cutin: dict, optional
+            Parameters for cutin modification
         kwargs: dict, optional
             Keyword arguments for Downwind
 
         """
         super().__init__(*args, **kwargs)
 
         self.max_it = 2 * self.farm.n_turbines if max_it is None else max_it
         self.conv_crit = (
-            self.get_model("DefaultConv")() if conv_crit is None else conv_crit
+            self.get_model("DefaultConv")() if conv_crit == "default" else conv_crit
         )
         self.prev_farm_results = None
         self._it = None
         self._mlist = None
         self._reamb = False
-        self._urelax = Dict(
-            first={}, pre_rotor={}, post_rotor={}, pre_wake={FV.CT: 0.5}, last={}
-        )
+        self._urelax = None
+
+        self._mod_cutin = dict(modify_ct=True, modify_P=False)
+        self._mod_cutin.update(mod_cutin)
 
     def set_urelax(self, entry_point, **urel):
         """
         Sets under-relaxation parameters.
 
         Parameters
         ----------
@@ -85,16 +88,33 @@
             pre_wake, last
         urel: dict
             The variables and their under-relaxation values
 
         """
         if self.initialized:
             raise ValueError(f"Attempt to set_urelax after initialization")
+        if self._urelax is None:
+            self._urelax = Dict(
+                first={},
+                pre_rotor={},
+                post_rotor={},
+                pre_wake={},
+                last={},
+            )
         self._urelax[entry_point].update(urel)
 
+    def initialize(self):
+        """
+        Initializes the algorithm.
+        """
+        super().initialize()
+        if len(self._mod_cutin):
+            for t in self.farm_controller.turbine_types:
+                t.modify_cutin(**self._mod_cutin)
+
     @property
     def urelax(self):
         """
         Returns the under-relaxation parameters
 
         Returns
         -------
@@ -115,78 +135,97 @@
             The current iteration number
 
         """
         return self._it
 
     def _collect_farm_models(
         self,
+        outputs,
         calc_parameters,
         ambient,
     ):
         """
         Helper function that creates model list
         """
-
         if self._it == 0:
             self._mlist0, self._calc_pars0 = super()._collect_farm_models(
-                calc_parameters,
+                outputs=False,
+                calc_parameters=calc_parameters,
                 ambient=ambient,
             )
 
             n = 0
-            if len(self._urelax["first"]):
-                self._mlist0.insert(0, mdls.URelax(**self._urelax["first"]))
-                self._calc_pars0.insert(0, {})
-                self._reamb = True
-                n += 1
-
-            if len(self._urelax["pre_rotor"]):
-                self._mlist0.insert(2 + n, mdls.URelax(**self._urelax["pre_rotor"]))
-                self._calc_pars0.insert(2 + n, {})
-                self._reamb = True
-                n += 1
-
-            if len(self._urelax["post_rotor"]):
-                self._mlist0.insert(4 + n, mdls.URelax(**self._urelax["post_rotor"]))
-                self._calc_pars0.insert(4 + n, {})
-                self._reamb = True
-                n += 1
-
-            if len(self._urelax["pre_wake"]):
-                self._mlist0.models[7 + n].urelax = mdls.URelax(
-                    **self._urelax["pre_wake"]
-                )
-
-            if len(self._urelax["last"]):
-                self._mlist0.append(mdls.URelax(**self._urelax["last"]))
-                self._calc_pars0.append({})
+            if self._urelax is not None:
+                if len(self._urelax["first"]):
+                    self._mlist0.insert(0, mdls.URelax(**self._urelax["first"]))
+                    self._calc_pars0.insert(0, {})
+                    self._reamb = True
+                    n += 1
+
+                if len(self._urelax["pre_rotor"]):
+                    self._mlist0.insert(2 + n, mdls.URelax(**self._urelax["pre_rotor"]))
+                    self._calc_pars0.insert(2 + n, {})
+                    self._reamb = True
+                    n += 1
+
+                if len(self._urelax["post_rotor"]):
+                    self._mlist0.insert(
+                        4 + n, mdls.URelax(**self._urelax["post_rotor"])
+                    )
+                    self._calc_pars0.insert(4 + n, {})
+                    self._reamb = True
+                    n += 1
+
+                if len(self._urelax["pre_wake"]):
+                    self._mlist0.models[5 + n].urelax = mdls.URelax(
+                        **self._urelax["pre_wake"]
+                    )
+
+                if len(self._urelax["last"]):
+                    self._mlist0.append(mdls.URelax(**self._urelax["last"]))
+                    self._calc_pars0.append({})
 
             return self._mlist0, self._calc_pars0
 
         elif ambient or self._reamb:
             return self._mlist0, self._calc_pars0
 
         else:
             # prepare:
             calc_pars = []
             mlist = FarmDataModelList(models=[])
 
-            # add under-relaxation during wake calculation:
-            urelax = None
-            if len(self._urelax["pre_wake"]):
-                urelax = mdls.URelax(**self._urelax["pre_wake"])
-
-            # add model that calculates wake effects:
-            mlist.models.append(self.get_model("FarmWakesCalculation")(urelax=urelax))
-            calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
-
-            # add under-relaxation:
-            if len(self._urelax["last"]):
-                mlist.append(mdls.URelax(**self._urelax["last"]))
-                calc_pars.append({})
+            # do not rotate back from downwind order:
+            if not self._final_run:
+
+                # add under-relaxation during wake calculation:
+                urelax = None
+                if self._urelax is not None and len(self._urelax["pre_wake"]):
+                    urelax = mdls.URelax(**self._urelax["pre_wake"])
+
+                # add model that calculates wake effects:
+                mlist.models.append(
+                    self.get_model("FarmWakesCalculation")(urelax=urelax)
+                )
+                calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
+
+                # add under-relaxation:
+                if self._urelax is not None and len(self._urelax["last"]):
+                    mlist.append(mdls.URelax(**self._urelax["last"]))
+                    calc_pars.append({})
+
+            # rotate back from downwind order:
+            else:
+
+                # add model that calculates wake effects:
+                # mlist.models.append(self.get_model("FarmWakesCalculation")(urelax=None))
+                # calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
+
+                mlist.models.append(self.get_model("ReorderFarmOutput")(outputs))
+                calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
 
             return mlist, calc_pars
 
     def _calc_farm_vars(self, mlist):
         """Helper function that gathers the farm variables"""
         if self._it == 0:
             super()._calc_farm_vars(mlist)
@@ -214,31 +253,41 @@
         Returns
         -------
         farm_results: xarray.Dataset
             The farm results. The calculated variables have
             dimensions (state, turbine)
 
         """
+        outputs = kwargs.pop("outputs", self.DEFAULT_FARM_OUTPUTS)
+        outputs = list(set(outputs + [FV.ORDER_SSEL, FV.ORDER_INV, FV.WEIGHT]))
+
         fres = None
         self._it = -1
+        self._final_run = False
         while self._it < self.max_it:
             self._it += 1
 
             self.print(f"\nAlgorithm {self.name}: Iteration {self._it}\n", vlim=0)
 
             self.prev_farm_results = fres
-            fres = super().calc_farm(finalize=False, **kwargs)
+            fres = super().calc_farm(outputs=None, finalize=False, **kwargs)
 
-            conv = self.conv_crit.check_converged(
-                self, self.prev_farm_results, fres, verbosity=self.verbosity + 1
-            )
+            if self.conv_crit is not None:
+                conv = self.conv_crit.check_converged(
+                    self, self.prev_farm_results, fres, verbosity=self.verbosity + 1
+                )
 
-            if conv:
-                self.print(f"\nAlgorithm {self.name}: Convergence reached.\n", vlim=0)
-                break
+                if conv:
+                    self.print(
+                        f"\nAlgorithm {self.name}: Convergence reached.\n", vlim=0
+                    )
+                    self.print("Starting final run")
+                    self._final_run = True
+                    fres = super().calc_farm(outputs=outputs, finalize=False, **kwargs)
+                    break
 
             if self._it == 0:
                 self.verbosity -= 1
 
         # finalize models:
         if finalize:
             self.print("\n")
```

### Comparing `foxes-0.6.2/foxes/algorithms/iterative/models/convergence.py` & `foxes-0.7/foxes/algorithms/iterative/models/convergence.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,12 +269,12 @@
 
     def __init__(self):
         """
         Constructor.
         """
         super().__init__(
             {
-                FV.REWS: 1e-5,
-                FV.TI: 1e-6,
-                FV.CT: 1e-6,
+                FV.REWS: 1e-6,
+                FV.TI: 1e-7,
+                FV.CT: 1e-7,
             }
         )
```

### Comparing `foxes-0.6.2/foxes/algorithms/iterative/models/farm_wakes_calc.py` & `foxes-0.7/foxes/models/turbine_models/rotor_centre_calc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,136 @@
 import numpy as np
 
+from foxes.core import TurbineModel, Data
 import foxes.variables as FV
-from foxes.core import FarmDataModel
+import foxes.constants as FC
 
 
-class FarmWakesCalculation(FarmDataModel):
+class RotorCentreCalc(TurbineModel):
     """
-    This model calculates wakes effects on farm data.
+    Calculates data at the rotor centre
 
     Attributes
     ----------
-    urelax: foxes.algorithms.iterative.models.URelax
-        The under-relaxation model
+    calc_vars: dict
+        The variables that are calculated by the model,
+        keys: var names, values: rotor var names
 
-    :group: algorithms.iterative.models
+    :group: models.turbine_models
 
     """
 
-    def __init__(self, urelax=None):
+    def __init__(self, calc_vars):
         """
         Constructor.
 
         Parameters
         ----------
-        urelax: foxes.algorithms.iterative.models.URelax, optional
-            The under-relaxation model
+        calc_vars: dict
+            The variables that are calculated by the model,
+            keys: var names, values: rotor var names
 
         """
         super().__init__()
-        self.urelax = urelax
 
-    def output_farm_vars(self, algo):
+        if isinstance(calc_vars, dict):
+            self.calc_vars = calc_vars
+        else:
+            self.calc_vars = {v: v for v in calc_vars}
+
+    def initialize(self, algo, verbosity=0):
         """
-        The variables which are being modified by the model.
+        Initializes the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-
-        Returns
-        -------
-        output_vars: list of str
-            The output variable names
+        verbosity: int
+            The verbosity level, 0 = silent
 
         """
-        ovars = algo.rotor_model.output_farm_vars(
-            algo
-        ) + algo.farm_controller.output_farm_vars(algo)
-        return list(dict.fromkeys(ovars))
+        self._wcalc = algo.get_model("PointWakesCalculation")()
+        super().initialize(algo, verbosity)
 
     def sub_models(self):
         """
         List of all sub-models
 
         Returns
         -------
         smdls: list of foxes.core.Model
-            All sub models
+            Names of all sub models
 
         """
-        return [self.pwakes] if self.urelax is None else [self.urelax, self.pwakes]
+        return [self._wcalc]
 
-    def initialize(self, algo, verbosity=0):
+    def output_farm_vars(self, algo):
         """
-        Initializes the model.
+        The variables which are being modified by the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
+
+        Returns
+        -------
+        output_vars: list of str
+            The output variable names
 
         """
-        self.pwakes = algo.partial_wakes_model
-        super().initialize(algo, verbosity)
+        return list(self.calc_vars.keys())
 
-    def calculate(self, algo, mdata, fdata):
-        """ "
+    def calculate(self, algo, mdata, fdata, st_sel):
+        """
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
+        st_sel: slice or numpy.ndarray of bool
+            The state-turbine selection,
+            for shape: (n_states, n_turbines)
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
+        # prepare target point data:
+        tdata = Data.from_points(
+            fdata[FV.TXYH],
+            data={
+                v: np.zeros_like(fdata[FV.X][:, :, None])
+                for v in self.calc_vars.values()
+            },
+            dims={v: (FC.STATE, FC.TARGET, FC.TPOINT) for v in self.calc_vars.values()},
+            name=f"{self.name}_tdata",
+        )
+
+        # run ambient calculation:
+        res = algo.states.calculate(algo, mdata, fdata, tdata)
+        for v, a in FV.var2amb.items():
+            if v in res:
+                res[a] = res[v].copy()
+        tdata.update(res)
+
+        # run wake calculation:
+        res = self._wcalc.calculate(algo, mdata, fdata, tdata)
+
+        # extract results:
+        out = {v: fdata[v] for v in self.calc_vars.keys()}
+        for v in out.keys():
+            out[v][st_sel] = res[self.calc_vars[v]][st_sel]
 
-        torder = fdata[FV.ORDER]
-        n_order = torder.shape[1]
-        n_states = mdata.n_states
-
-        def _evaluate(algo, mdata, fdata, pdata, wdeltas, o):
-            self.pwakes.evaluate_results(
-                algo, mdata, fdata, pdata, wdeltas, states_turbine=o
-            )
-
-            trbs = np.zeros((n_states, algo.n_turbines), dtype=bool)
-            np.put_along_axis(trbs, o[:, None], True, axis=1)
-
-            res = algo.farm_controller.calculate(
-                algo, mdata, fdata, pre_rotor=False, st_sel=trbs
-            )
-            fdata.update(res)
-
-            if self.urelax is not None:
-                res = self.urelax.calculate(algo, mdata, fdata)
-                for v, d in res.items():
-                    fdata[v][trbs] = d[trbs]
-
-        wdeltas, pdata = self.pwakes.new_wake_deltas(algo, mdata, fdata)
-        for oi in range(n_order):
-            o = torder[:, oi]
-            self.pwakes.contribute_to_wake_deltas(algo, mdata, fdata, pdata, o, wdeltas)
-
-        for oi in range(n_order):
-            _evaluate(algo, mdata, fdata, pdata, wdeltas, torder[:, oi])
-
-        return {v: fdata[v] for v in self.output_farm_vars(algo)}
+        return out
```

### Comparing `foxes-0.6.2/foxes/algorithms/iterative/models/urelax.py` & `foxes-0.7/foxes/algorithms/iterative/models/urelax.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/algorithms/sequential/models/plugin.py` & `foxes-0.7/foxes/algorithms/sequential/models/plugin.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/algorithms/sequential/models/seq_state.py` & `foxes-0.7/foxes/algorithms/sequential/models/seq_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,33 +130,34 @@
         -------
         output_vars: list of str
             The output variable names
 
         """
         return self.states.output_point_vars(algo)
 
-    def calculate(self, algo, mdata, fdata, pdata):
-        """
+    def calculate(self, algo, mdata, fdata, tdata):
+        """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
-        pdata: foxes.core.Data
-            The point data
+        tdata: foxes.core.Data
+            The target point data
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_points)
+            Values: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints)
 
         """
-        return self.states.calculate(algo, mdata, fdata, pdata)
+        return self.states.calculate(algo, mdata, fdata, tdata)
```

### Comparing `foxes-0.6.2/foxes/algorithms/sequential/sequential.py` & `foxes-0.7/foxes/algorithms/sequential/sequential.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 from xarray import Dataset
 
 from foxes.algorithms.downwind.downwind import Downwind
 import foxes.constants as FC
 import foxes.variables as FV
-from foxes.core.data import Data
+from foxes.core.data import MData, FData, TData
 
 from . import models as mdls
 
 
 class Sequential(Downwind):
     """
     A sequential calculation of states without chunking.
@@ -26,15 +26,16 @@
         Key: model name str, value: parameter dict
     states0: foxes.core.States
         The original states
     points: numpy.ndarray
         The points of interest, shape: (n_states, n_points, 3)
     plugins: list of foxes.algorithm.sequential.SequentialIterPlugin
         The plugins, updated with every iteration
-
+    outputs: list of str
+        The output variables
     :group: algorithms.sequential
 
     """
 
     @classmethod
     def get_model(cls, name):
         """
@@ -54,32 +55,30 @@
         try:
             return getattr(mdls, name)
         except AttributeError:
             return super().get_model(name)
 
     def __init__(
         self,
-        mbook,
         farm,
         states,
         *args,
         points=None,
         ambient=False,
         calc_pars={},
-        chunks={FC.STATE: None, FC.POINT: 10000},
+        chunks={FC.STATE: None, FC.POINT: 4000},
         plugins=[],
+        outputs=None,
         **kwargs,
     ):
         """
         Constructor.
 
         Parameters
         ----------
-        mbook: foxes.ModelBook
-            The model book
         farm: foxes.WindFarm
             The wind farm
         states: foxes.core.States
             The ambient states
         args: tuple, optional
             Additional arguments for Downwind
         points: numpy.ndarray, optional
@@ -89,26 +88,27 @@
         calc_pars: dict
             Parameters for model calculation.
             Key: model name str, value: parameter dict
         chunks: dict
             The xarray.Dataset chunk parameters
         plugins: list of foxes.algorithm.sequential.SequentialIterPlugin
             The plugins, updated with every iteration
+        outputs: list of str, optional
+            The output variables
         kwargs: dict, optional
             Additional arguments for Downwind
 
         """
-        super().__init__(
-            mbook, farm, mdls.SeqState(states), *args, chunks=chunks, **kwargs
-        )
+        super().__init__(farm, mdls.SeqState(states), *args, chunks=chunks, **kwargs)
         self.ambient = ambient
         self.calc_pars = calc_pars
         self.states0 = self.states.states
         self.points = points
         self.plugins = plugins
+        self.outputs = outputs if outputs is not None else self.DEFAULT_FARM_OUTPUTS
 
         self._i = None
 
     @property
     def iterating(self):
         """
         Flag for running iteration
@@ -131,15 +131,15 @@
 
             self._inds = self.states0.index()
             self._weights = self.states0.weights(self)
             self._i = 0
             self._counter = 0
 
             self._mlist, self._calc_pars = self._collect_farm_models(
-                self.calc_pars, self.ambient
+                self.outputs, self.calc_pars, self.ambient
             )
             if not self._mlist.initialized:
                 self._mlist.initialize(self, self.verbosity)
                 self._calc_farm_vars(self._mlist)
             self._print_model_oder(self._mlist, self._calc_pars)
 
             self._mdata = self.get_models_idata()
@@ -151,22 +151,22 @@
                     ]
                 )
                 print("\nInput data:\n")
                 print(s, "\n")
                 print(f"Output farm variables:", ", ".join(self.farm_vars))
                 print()
 
-            self._mdata = Data(
+            self._mdata = MData(
                 data={v: d[1] for v, d in self._mdata["data_vars"].items()},
                 dims={v: d[0] for v, d in self._mdata["data_vars"].items()},
                 loop_dims=[FC.STATE],
                 name="mdata",
             )
 
-            self._fdata = Data(
+            self._fdata = FData(
                 data={
                     v: np.zeros((self.n_states, self.n_turbines), dtype=FC.DTYPE)
                     for v in self.farm_vars
                 },
                 dims={v: (FC.STATE, FC.TURBINE) for v in self.farm_vars},
                 loop_dims=[FC.STATE],
                 name="fdata",
@@ -178,22 +178,21 @@
                 )
                 if not self._plist.initialized:
                     self._plist.initialize(self, self.verbosity)
                 self._pvars = self._plist.output_point_vars(self)
                 self.print(f"\nOutput point variables:", ", ".join(self._pvars), "\n")
 
                 n_points = self.points.shape[1]
-                self._pdata = Data.from_points(
+                self._tdata = TData.from_points(
                     self.points,
                     data={
-                        v: np.zeros((self.n_states, n_points), dtype=FC.DTYPE)
+                        v: np.zeros((self.n_states, n_points, 1), dtype=FC.DTYPE)
                         for v in self._pvars
                     },
-                    dims={v: (FC.STATE, FC.POINT) for v in self._pvars},
-                    name="pdata",
+                    dims={v: (FC.STATE, FC.TARGET, FC.TPOINT) for v in self._pvars},
                 )
 
             for p in self.plugins:
                 p.initialize(self)
 
         return self
 
@@ -203,25 +202,25 @@
         if self._i < len(self._inds):
             self._counter = self._i
             self.states._counter = self._i
             self.states._size = 1
             self.states._indx = self._inds[self._i]
             self.states._weight = self._weights[self._i]
 
-            mdata = Data(
+            mdata = MData(
                 data={
                     v: d[self._i, None] if self._mdata.dims[v][0] == FC.STATE else d
                     for v, d in self._mdata.items()
                 },
                 dims={v: d for v, d in self._mdata.dims.items()},
                 loop_dims=[FC.STATE],
                 name="mdata",
             )
 
-            fdata = Data(
+            fdata = FData(
                 data={
                     v: np.zeros((1, self.n_turbines), dtype=FC.DTYPE)
                     for v in self.farm_vars
                 },
                 dims={v: (FC.STATE, FC.TURBINE) for v in self.farm_vars},
                 loop_dims=[FC.STATE],
                 name="fdata",
@@ -230,15 +229,15 @@
             fres = self._mlist.calculate(self, mdata, fdata, parameters=self._calc_pars)
             fres[FV.WEIGHT] = self.weight[None, :]
 
             for v, d in fres.items():
                 self._fdata[v][self._i] = d[0]
 
             fres = Dataset(
-                coords={FC.STATE: [self.index], FC.TURBINE: np.arange(self.n_turbines)},
+                coords={FC.STATE: [self.index]},
                 data_vars={v: ((FC.STATE, FC.TURBINE), d) for v, d in fres.items()},
             )
             fres[FC.TNAME] = ((FC.TURBINE,), self.farm.turbine_names)
             if FV.ORDER in fres:
                 fres[FV.ORDER] = fres[FV.ORDER].astype(FC.ITYPE)
 
             if self.points is None:
@@ -246,33 +245,36 @@
                     p.update(self, fres)
 
                 self._i += 1
                 return fres
 
             else:
                 n_points = self.points.shape[1]
-                pdata = Data.from_points(
+                tdata = TData.from_points(
                     self.points[self.counter, None],
                     data={
-                        v: np.zeros((1, n_points), dtype=FC.DTYPE) for v in self._pvars
+                        v: np.zeros((1, n_points, 1), dtype=FC.DTYPE)
+                        for v in self._pvars
                     },
-                    dims={v: (FC.STATE, FC.POINT) for v in self._pvars},
-                    name="pdata",
+                    dims={v: (FC.STATE, FC.TARGET, FC.TPOINT) for v in self._pvars},
                 )
 
                 pres = self._plist.calculate(
-                    self, mdata, fdata, pdata, parameters=self._calc_pars_p
+                    self, mdata, fdata, tdata, parameters=self._calc_pars_p
                 )
 
                 for v, d in pres.items():
-                    self._pdata[v][self._i] = d[0]
+                    self._tdata[v][self._i] = d[0]
 
                 pres = Dataset(
-                    coords={FC.STATE: [self.index], FC.POINT: np.arange(n_points)},
-                    data_vars={v: ((FC.STATE, FC.POINT), d) for v, d in pres.items()},
+                    coords={FC.STATE: [self.index]},
+                    data_vars={
+                        v: ((FC.STATE, FC.TARGET, FC.TPOINT), d)
+                        for v, d in pres.items()
+                    },
                 )
 
                 for p in self.plugins:
                     p.update(self, fres, pres)
 
                 self._i += 1
                 return fres, pres
@@ -326,14 +328,34 @@
         -------
         indx: int
             The current index
 
         """
         return self.states._indx if self.iterating else None
 
+    def states_i0(self, counter, algo=None):
+        """
+        Returns counter or index
+
+        Parameters
+        ----------
+        counter: bool
+            Flag for counter
+        algo: object, optional
+            Dummy argument, due to consistency with
+            foxes.core.Data.states_i0
+
+        Returns
+        -------
+        i0: int
+            The counter or index
+
+        """
+        return self.counter if counter else self.index
+
     @property
     def weight(self):
         """
         The current weight array
 
         Returns
         -------
@@ -346,45 +368,45 @@
     @property
     def mdata(self):
         """
         Get the current model data
 
         Returns
         -------
-        d: foxes.core.Data
+        d: foxes.core.MData
             The current model data
 
         """
         return self._mdata if self.iterating else None
 
     @property
     def fdata(self):
         """
         Get the current farm data
 
         Returns
         -------
-        d: foxes.core.Data
+        d: foxes.core.FData
             The current farm data
 
         """
         return self._fdata
 
     @property
-    def pdata(self):
+    def tdata(self):
         """
         Get the current point data
 
         Returns
         -------
-        d: foxes.core.Data
+        d: foxes.core.TData
             The current point data
 
         """
-        return self._pdata if self.points is not None and self.iterating else None
+        return self._tdata if self.points is not None and self.iterating else None
 
     @property
     def farm_results(self):
         """
         The overall farm results
 
         Returns
@@ -401,14 +423,27 @@
         results[FC.TNAME] = ((FC.TURBINE,), self.farm.turbine_names)
         if FV.ORDER in results:
             results[FV.ORDER] = results[FV.ORDER].astype(FC.ITYPE)
 
         return results
 
     @property
+    def prev_farm_results(self):
+        """
+        Alias for farm_results
+
+        Returns
+        -------
+        results: xarray.Dataset
+            The overall farm results
+
+        """
+        return self.farm_results
+
+    @property
     def cur_farm_results(self):
         """
         The current farm results
 
         Returns
         -------
         results: xarray.Dataset
@@ -445,15 +480,15 @@
         results = Dataset(
             coords={
                 FC.STATE: self._inds,
                 FC.TURBINE: np.arange(self.n_turbines),
                 FC.POINT: np.arange(n_points),
                 FC.XYH: np.arange(3),
             },
-            data_vars={v: (self._pdata.dims[v], d) for v, d in self._pdata.items()},
+            data_vars={v: (self._tdata.dims[v], d) for v, d in self._tdata.items()},
         )
 
         return results
 
     @property
     def cur_point_results(self):
         """
@@ -473,15 +508,15 @@
             coords={
                 FC.STATE: [self.index],
                 FC.TURBINE: np.arange(self.n_turbines),
                 FC.POINT: np.arange(n_points),
                 FC.XYH: np.arange(3),
             },
             data_vars={
-                v: (self._pdata.dims[v], d[i, None]) for v, d in self._pdata.items()
+                v: (self._tdata.dims[v], d[i, None]) for v, d in self._tdata.items()
             },
         )
 
         return results
 
     def calc_farm(self, *args, **kwargs):
         if not self.iterating:
@@ -497,46 +532,48 @@
 
         plist, calc_pars = self._collect_point_models(ambient=self.ambient)
         if not plist.initialized:
             plist.initialize(self, self.verbosity)
         pvars = plist.output_point_vars(self)
 
         mdata = self.get_models_idata()
-        mdata = Data(
+        mdata = MData(
             data={v: d[1] for v, d in mdata["data_vars"].items()},
             dims={v: d[0] for v, d in mdata["data_vars"].items()},
             loop_dims=[FC.STATE],
             name="mdata",
         )
-        mdata = Data(
+        mdata = MData(
             data={
                 v: d[self.states.counter, None] if mdata.dims[v][0] == FC.STATE else d
                 for v, d in mdata.items()
             },
             dims={v: d for v, d in mdata.dims.items()},
             loop_dims=[FC.STATE],
             name="mdata",
         )
 
-        fdata = Data(
+        fdata = FData(
             data={v: farm_results[v].to_numpy() for v in self.farm_vars},
             dims={v: (FC.STATE, FC.TURBINE) for v in self.farm_vars},
             loop_dims=[FC.STATE],
             name="fdata",
         )
 
-        pdata = Data.from_points(
+        tdata = TData.from_points(
             points[0, None],
-            data={v: np.zeros((1, n_points), dtype=FC.DTYPE) for v in pvars},
-            dims={v: (FC.STATE, FC.POINT) for v in pvars},
-            name="pdata",
+            data={v: np.zeros((1, n_points, 1), dtype=FC.DTYPE) for v in pvars},
+            dims={v: (FC.STATE, FC.TARGET, FC.TPOINT) for v in pvars},
+            name="tdata",
         )
 
-        pres = plist.calculate(self, mdata, fdata, pdata, parameters=calc_pars)
+        pres = plist.calculate(self, mdata, fdata, tdata, parameters=calc_pars)
         pres = Dataset(
-            coords={FC.STATE: self.states.index(), FC.POINT: np.arange(n_points)},
-            data_vars={v: ((FC.STATE, FC.POINT), d) for v, d in pres.items()},
+            coords={FC.STATE: self.states.index()},
+            data_vars={
+                v: ((FC.STATE, FC.TARGET, FC.TPOINT), d) for v, d in pres.items()
+            },
         )
 
         # plist.finalize(self, self.verbosity)
 
         return pres
```

### Comparing `foxes-0.6.2/foxes/constants.py` & `foxes-0.7/foxes/constants.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,41 +21,51 @@
 """
 
 TNAME = "tname"
 """ Wind turbine name identifier
 :group: foxes.constants
 """
 
-POINT = "point"
-""" Point identifier
+TARGET = "target"
+""" Target identifier
 :group: foxes.constants
 """
 
-POINTS = "points"
-""" Points identifier
+TARGETS = "targets"
+""" Targets identifier
 :group: foxes.constants
 """
 
-RPOINT = "rotor_point"
-""" Rotor point identifier
+TPOINT = "target_point"
+""" Target point identifier
 :group: foxes.constants
 """
 
-RPOINTS = "rotor_points"
-""" Rotor points identifier
+TPOINTS = "target_points"
+""" Points per target identifier
 :group: foxes.constants
 """
 
-RWEIGHTS = "rotor_weights"
-""" Rotor point weights identifier
+TWEIGHTS = "tpoint_weights"
+""" Target point weights identifier
 :group: foxes.constants
 """
 
-AMB_RPOINT_RESULTS = "amb_rpoint_res"
-""" Identified for ambient rotor point results
+POINT = "point"
+""" Point identifier
+:group: foxes.constants
+"""
+
+POINTS = "points"
+""" Points identifier
+:group: foxes.constants
+"""
+
+AMB_TARGET_RESULTS = "amb_target_res"
+""" Identified for ambient target results
 :group: foxes.constants
 """
 
 
 VARS = "vars"
 """ Variables identifier
 :group: foxes.constants
@@ -77,26 +87,31 @@
 """
 
 STATES_SEL = "states_sel"
 """Identifier for states selection
 :group: foxes.constants
 """
 
-STATE_SOURCE_TURBINE = "state_source_turbine"
-"""Identifier for the source turbines per state
+STATE_TURBINE = "state-turbine"
+"""Identifier for state-turbine dimensions
+:group: foxes.constants
+"""
+
+STATE_TARGET = "state-target"
+"""Identifier for state-target dimensions
 :group: foxes.constants
 """
 
-STATE_TURBINE = "state-turbine"
-"""Identifier for state-turbine dimensions
+STATE_TARGET_TPOINT = "state-target-tpoint"
+"""Identifier for state-target-tpoints dimensions
 :group: foxes.constants
 """
 
-STATE_POINT = "state-point"
-"""Identifier for state-point dimensions
+STATE_SOURCE_ORDERI = "state-source-orderi"
+"""Identifier for order index of wake causing turbines
 :group: foxes.constants
 """
 
 DTYPE = np.float64
 """ Default data type for floats
 :group: foxes.constants
 """
```

### Comparing `foxes-0.6.2/foxes/core/__init__.py` & `foxes-0.7/foxes/core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Abstract classes and core functionality.
 """
 
-from .data import Data
+from .data import Data, MData, FData, TData
 from .model import Model
 from .data_calc_model import DataCalcModel
 from .states import States, ExtendedStates
 from .wind_farm import WindFarm
 from .algorithm import Algorithm
 from .farm_data_model import FarmDataModel, FarmDataModelList
 from .point_data_model import PointDataModel, PointDataModelList
@@ -14,11 +14,11 @@
 from .farm_model import FarmModel
 from .turbine_model import TurbineModel
 from .turbine_type import TurbineType
 from .farm_controller import FarmController
 from .turbine import Turbine
 from .partial_wakes_model import PartialWakesModel
 from .wake_frame import WakeFrame
-from .wake_model import WakeModel
+from .wake_model import WakeModel, TurbineInductionModel
 from .wake_superposition import WakeSuperposition
 from .vertical_profile import VerticalProfile
 from .axial_induction_model import AxialInductionModel
```

### Comparing `foxes-0.6.2/foxes/core/algorithm.py` & `foxes-0.7/foxes/core/algorithm.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,17 @@
         self.farm = farm
         self.chunks = chunks
         self.verbosity = verbosity
         self.n_states = None
         self.n_turbines = farm.n_turbines
         self.dbook = StaticData() if dbook is None else dbook
 
+        if chunks is not None and FC.TARGET not in chunks:
+            self.chunks[FC.TARGET] = chunks.get(FC.POINT, None)
+
         self._idata_mem = Dict()
 
     def print(self, *args, vlim=1, **kwargs):
         """
         Print function, based on verbosity.
 
         Parameters
@@ -111,23 +114,32 @@
                     f"Input {mtype} data entry '{v}': Wrong data shape, expecting {len(t[0])} dimensions, got {t[1].shape}"
                 )
             if FC.STATE in t[0]:
                 if t[0][0] != FC.STATE:
                     raise ValueError(
                         f"Input {mtype} data entry '{v}': Dimension '{FC.STATE}' not at first position, got {t[0]}"
                     )
-                if FC.POINT in t[0] and t[0][1] != FC.POINT:
-                    raise ValueError(
-                        f"Input {mtype} data entry '{v}': Dimension '{FC.POINT}' not at second position, got {t[0]}"
-                    )
-            elif FC.POINT in t[0]:
-                if t[0][0] != FC.POINT:
-                    raise ValueError(
-                        f"Input {mtype} data entry '{v}': Dimension '{FC.POINT}' not at first position, got {t[0]}"
-                    )
+                if FC.TURBINE in t[0]:
+                    if t[0][1] != FC.TURBINE:
+                        raise ValueError(
+                            f"Input {mtype} data entry '{v}': Dimension '{FC.TURBINE}' not at second position, got {t[0]}"
+                        )
+                if FC.TARGET in t[0]:
+                    if t[0][1] != FC.TARGET:
+                        raise ValueError(
+                            f"Input {mtype} data entry '{v}': Dimension '{FC.TARGET}' not at second position, got {t[0]}"
+                        )
+                    if len(t[0]) < 3 or t[0][2] != FC.TPOINT:
+                        raise KeyError(
+                            f"Input {mtype} data entry '{v}': Expecting dimension '{FC.TPOINT}' as third entry. Got {t[0]}"
+                        )
+            elif FC.TURBINE in t[0]:
+                raise ValueError(
+                    f"Input {mtype} data entry '{v}': Dimension '{FC.TURBINE}' requires combination with dimension '{FC.STATE}'"
+                )
             for d, s in zip(t[0], t[1].shape):
                 if d not in sizes:
                     sizes[d] = s
                 elif sizes[d] != s:
                     raise ValueError(
                         f"Input {mtype} data entry '{v}': Dimension '{d}' has wrong size, expecting {sizes[d]}, got {s}"
                     )
@@ -149,17 +161,17 @@
         """
         xrdata = xr.Dataset(**idata)
         if self.chunks is not None:
             if FC.TURBINE in self.chunks.keys():
                 raise ValueError(
                     f"Dimension '{FC.TURBINE}' cannot be chunked, got chunks {self.chunks}"
                 )
-            if FC.RPOINT in self.chunks.keys():
+            if FC.TPOINT in self.chunks.keys():
                 raise ValueError(
-                    f"Dimension '{FC.RPOINT}' cannot be chunked, got chunks {self.chunks}"
+                    f"Dimension '{FC.TPOINT}' cannot be chunked, got chunks {self.chunks}"
                 )
             xrdata = xrdata.chunk(
                 chunks={c: v for c, v in self.chunks.items() if c in sizes}
             )
         return xrdata
 
     def chunked(self, ds):
@@ -372,15 +384,22 @@
             len(points.shape) != 3
             or points.shape[0] != self.n_states
             or points.shape[2] != 3
         ):
             raise ValueError(
                 f"points have wrong dimensions, expecting ({self.n_states}, {points.shape[1]}, 3), got {points.shape}"
             )
-        idata["data_vars"][FC.POINTS] = ((FC.STATE, FC.POINT, FC.XYH), points)
+        idata["data_vars"][FC.TARGETS] = (
+            (FC.STATE, FC.TARGET, FC.TPOINT, FC.XYH),
+            points[:, :, None, :],
+        )
+        idata["data_vars"][FC.TWEIGHTS] = (
+            (FC.TPOINT,),
+            np.array([1.0], dtype=FC.DTYPE),
+        )
 
         sizes = self.__get_sizes(idata, "point")
         return self.__get_xrdata(idata, sizes)
 
     def finalize(self, clear_mem=False):
         """
         Finalizes the algorithm.
```

### Comparing `foxes-0.6.2/foxes/core/data.py` & `foxes-0.7/foxes/models/turbine_models/set_farm_vars.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,223 +1,194 @@
 import numpy as np
 
-from foxes.utils import Dict
-import foxes.variables as FV
+from foxes.core import TurbineModel
 import foxes.constants as FC
+import foxes.variables as FV
 
 
-class Data(Dict):
+class SetFarmVars(TurbineModel):
     """
-    Container for data and meta data.
-
-    Used during the calculation of single chunks,
-    usually for numpy data (not xarray data).
+    Set farm data variables to given data.
 
     Attributes
     ----------
-    dims: dict
-        The dimensions tuples, same or subset
-        of data keys
-    loop_dims: array_like of str
-        List of the loop dimensions during xarray's
-        `apply_ufunc` calculations
-    sizes: dict
-        The dimension sizes
+    vars: list of str
+        The variables to be set
 
-    :group: core
+    :group: models.turbine_models
 
     """
 
-    def __init__(self, data, dims, loop_dims, name="data"):
+    def __init__(self, pre_rotor=False):
         """
         Constructor.
 
         Parameters
         ----------
-        data: dict
-            The initial data to be stored
-        dims: dict
-            The dimensions tuples, same or subset
-            of data keys
-        loop_dims: array_like of str
-            List of the loop dimensions during xarray's
-            `apply_ufunc` calculations
-        name: str
-            The data container name
-
-        """
-        super().__init__(name=name)
-
-        self.update(data)
-        self.dims = dims
-        self.loop_dims = loop_dims
-
-        self.sizes = {}
-        for v, d in data.items():
-            self.__run_entry_checks(v, d, dims[v])
+        pre_rotor: bool
+            Flag for running this model before
+            running the rotor model.
 
-        self.__auto_update()
+        """
+        super().__init__(pre_rotor=pre_rotor)
+        self.reset()
 
-    @property
-    def n_states(self):
+    def add_var(self, var, data):
         """
-        The number of states
+        Add data for a variable.
 
-        Returns
-        -------
-        int:
-            The number of states
+        Parameters
+        ----------
+        var: str
+            The variable name
+        data: numpy.ndarray
+            The data, shape: (n_states, n_turbines)
 
         """
-        return self.sizes[FC.STATE] if FC.STATE in self.sizes else None
+        self.vars.append(var)
+        self._vdata.append(np.asarray(data, dtype=FC.DTYPE))
 
-    @property
-    def n_turbines(self):
+    def reset(self):
         """
-        The number of turbines
-
-        Returns
-        -------
-        int:
-            The number of turbines
-
+        Remove all variables.
         """
-        return self.sizes[FC.TURBINE] if FC.TURBINE in self.sizes else None
+        self.vars = []
+        self._vdata = []
 
-    @property
-    def n_points(self):
+    def output_farm_vars(self, algo):
         """
-        The number of points
+        The variables which are being modified by the model.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
 
         Returns
         -------
-        int:
-            The number of points
+        output_vars: list of str
+            The output variable names
 
         """
-        return self.sizes[FC.POINT] if FC.POINT in self.sizes else None
+        return self.vars
 
-    def states_i0(self, counter=False, algo=None):
+    def load_data(self, algo, verbosity=0):
         """
-        Get the state counter for first state in chunk
+        Load and/or create all model data that is subject to chunking.
+
+        Such data should not be stored under self, for memory reasons. The
+        data returned here will automatically be chunked and then provided
+        as part of the mdata object during calculations.
 
         Parameters
         ----------
-        counter: bool
-            Return the state counter instead of the index
-        algo: foxes.core.Algorithm, optional
-            The algorithm, required for state counter
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        verbosity: int
+            The verbosity level, 0 = silent
 
         Returns
         -------
-        int:
-            The state counter for first state in chunk
-            or the corresponding index
+        idata: dict
+            The dict has exactly two entries: `data_vars`,
+            a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
+            and `coords`, a dict with entries `dim_name_str -> dim_array`
+
+        """
+        idata = super().load_data(algo, verbosity)
+
+        for i, v in enumerate(self.vars):
+            data = np.full((algo.n_states, algo.n_turbines), np.nan, dtype=FC.DTYPE)
+            vdata = self._vdata[i]
+
+            # handle special case of call during vectorized optimization:
+            if (
+                np.ndim(vdata)
+                and vdata.shape[0] != algo.n_states
+                and hasattr(algo.states, "n_pop")
+            ):
+                n_pop = algo.states.n_pop
+                n_ost = algo.states.states.size()
+                n_trb = algo.n_turbines
+                vdata = np.zeros((n_pop, n_ost, n_trb), dtype=FC.DTYPE)
+                vdata[:] = self._vdata[i][None, :]
+                vdata = vdata.reshape(n_pop * n_ost, n_trb)
+
+            data[:] = vdata
+            idata["data_vars"][self.var(v)] = ((FC.STATE, FC.TURBINE), data)
 
-        """
-        if FC.STATE not in self:
-            return None
-        elif counter:
-            if algo is None:
-                raise KeyError(f"{self.name}: Missing algo for deducing state counter")
-            return np.argwhere(algo.states.index() == self[FC.STATE][0])[0][0]
-        else:
-            return self[FC.STATE][0]
+        return idata
 
-    def __auto_update(self):
-        data = self
-        dims = self.dims
-
-        if (
-            FV.TXYH not in data
-            and FV.X in data
-            and FV.Y in data
-            and FV.H in data
-            and dims[FV.X] == (FC.STATE, FC.TURBINE)
-            and dims[FV.Y] == (FC.STATE, FC.TURBINE)
-            and dims[FV.H] == (FC.STATE, FC.TURBINE)
-        ):
-            self[FV.TXYH] = np.zeros(
-                (self.n_states, self.n_turbines, 3), dtype=FC.DTYPE
-            )
-
-            self[FV.TXYH][:, :, 0] = self[FV.X]
-            self[FV.TXYH][:, :, 1] = self[FV.Y]
-            self[FV.TXYH][:, :, 2] = self[FV.H]
-
-            self[FV.X] = self[FV.TXYH][:, :, 0]
-            self[FV.Y] = self[FV.TXYH][:, :, 1]
-            self[FV.H] = self[FV.TXYH][:, :, 2]
-
-            self.dims[FV.TXYH] = (FC.STATE, FC.TURBINE, FC.XYH)
-
-    def __run_entry_checks(self, name, data, dims):
-        # remove axes of size 1, added by dask for extra loop dimensions:
-        if dims is not None:
-            if len(dims) != len(data.shape):
-                for li, l in enumerate(self.loop_dims):
-                    if data.shape[li] == 1 and (len(dims) < li + 1 or dims[li] != l):
-                        self[name] = np.squeeze(data, axis=li)
-
-            for ci, c in enumerate(dims):
-                if c not in self.sizes:
-                    self.sizes[c] = self[name].shape[ci]
-                elif self.sizes[c] != self[name].shape[ci]:
-                    raise ValueError(
-                        f"Inconsistent size for data entry '{name}', dimension '{c}': Expecting {self.sizes[c]}, found {self[name].shape[ci]} in shape {self[name].shape}"
-                    )
-
-    def add(self, name, data, dims):
+    def calculate(self, algo, mdata, fdata, st_sel):
         """
-        Add data entry
+        The main model calculation.
 
-        Parameters
-        ----------
-        name: str
-            The data name
-        data: np.ndarray
-            The data
-        dims: tuple of str
-            The dimensions
-
-        """
-        self[name] = data
-        self.dims[name] = dims
-        self.__run_entry_checks(name, data, dims)
-        self.__auto_update()
-
-    @classmethod
-    def from_points(
-        cls,
-        points,
-        data={},
-        dims={},
-        name="pdata",
-    ):
-        """
-        Create from points
+        This function is executed on a single chunk of data,
+        all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        points: np.ndarray
-            The points, shape: (n_states, n_points, 3)
-        data: dict
-            The initial data to be stored
-        dims: dict
-            The dimensions tuples, same or subset
-            of data keys
-        name: str
-            The data container name
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.MData
+            The model data
+        fdata: foxes.core.FData
+            The farm data
+        st_sel: slice or numpy.ndarray of bool
+            The state-turbine selection,
+            for shape: (n_states, n_turbines)
 
         Returns
         -------
-        pdata: Data
-            The data object
+        results: dict
+            The resulting data, keys: output variable str.
+            Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
-        if len(points.shape) != 3 or points.shape[2] != 3:
-            raise ValueError(
-                f"Expecting points shape (n_states, n_points, 3), got {points.shape}"
-            )
-        data[FC.POINTS] = points
-        dims[FC.POINTS] = (FC.STATE, FC.POINT, FC.XYH)
-        return Data(data, dims, [FC.STATE, FC.POINT], name)
+        if self.pre_rotor:
+            order = np.s_[:]
+            ssel = np.s_[:]
+        else:
+            order = fdata[FV.ORDER]
+            ssel = fdata[FV.ORDER_SSEL]
+
+        bsel = np.zeros((fdata.n_states, fdata.n_turbines), dtype=bool)
+        bsel[st_sel] = True
+
+        for v in self.vars:
+            data = mdata[self.var(v)][ssel, order]
+            hsel = ~np.isnan(data)
+            tsel = bsel & hsel
+
+            # special case of turbine positions:
+            if v in [FV.X, FV.Y]:
+                i = [FV.X, FV.Y].index(v)
+                for ti in np.where(tsel)[1]:
+                    t = algo.farm.turbines[ti]
+                    if len(t.xy.shape) == 1:
+                        xy = np.zeros((algo.n_states, 2), dtype=FC.DTYPE)
+                        xy[:] = t.xy[None, :]
+                        t.xy = xy
+                    i0 = fdata.states_i0()
+                    hsel = tsel[:, ti]
+                    ssel = i0 + np.where(hsel)[0]
+                    t.xy[ssel, i] = data[hsel, ti]
+
+            # special case of rotor diameter and hub height:
+            if v in [FV.D, FV.H]:
+                for ti in np.where(tsel)[1]:
+                    t = algo.farm.turbines[ti]
+                    x = np.zeros(algo.n_states, dtype=FC.DTYPE)
+                    if v == FV.D:
+                        x[:] = t.D
+                        t.D = x
+                    else:
+                        x[:] = t.H
+                        t.H = x
+                    i0 = fdata.states_i0()
+                    hsel = tsel[:, ti]
+                    ssel = i0 + np.where(hsel)[0]
+                    x[ssel] = data[hsel, ti]
+
+            fdata[v][tsel] = data[tsel]
+
+        return {v: fdata[v] for v in self.vars}
```

### Comparing `foxes-0.6.2/foxes/core/data_calc_model.py` & `foxes-0.7/foxes/core/data_calc_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import xarray as xr
 from abc import abstractmethod
 from dask.distributed import progress
 from dask.diagnostics import ProgressBar
 
 from .model import Model
-from .data import Data
+from .data import MData, FData, TData
 from foxes.utils.runners import DaskRunner
 import foxes.constants as FC
 import foxes.variables as FV
 
 
 class DataCalcModel(Model):
     """
@@ -69,82 +69,86 @@
         out_dims,
         calc_pars,
         init_vars,
     ):
         """
         Wrapper that mitigates between apply_ufunc and `calculate`.
         """
-
         n_prev = len(init_vars)
         if n_prev:
             prev = ldata[:n_prev]
             ldata = ldata[n_prev:]
 
         # reconstruct original data:
         data = []
-        for hvars in dvars:
+        for i, hvars in enumerate(dvars):
             v2l = {v: lvars.index(v) for v in hvars if v in lvars}
             v2e = {v: evars.index(v) for v in hvars if v in evars}
 
             hdata = {v: ldata[v2l[v]] if v in v2l else edata[v2e[v]] for v in hvars}
             hdims = {v: ldims[v2l[v]] if v in v2l else edims[v2e[v]] for v in hvars}
-            data.append(Data(hdata, hdims, loop_dims))
+
+            if i == 0:
+                data.append(MData(data=hdata, dims=hdims, loop_dims=loop_dims))
+            elif i == 1:
+                data.append(FData(data=hdata, dims=hdims, loop_dims=loop_dims))
+            elif i == 2:
+                data.append(TData(data=hdata, dims=hdims, loop_dims=loop_dims))
+            else:
+                raise NotImplementedError(
+                    f"Not more than 3 data sets implemented, found {len(dvars)}"
+                )
 
             del hdata, hdims, v2l, v2e
 
         # deduce output shape:
         oshape = []
         for li, l in enumerate(out_dims):
             for i, dims in enumerate(ldims):
                 if l in dims:
                     oshape.append(ldata[i].shape[dims.index(l)])
                     break
             if len(oshape) != li + 1:
                 raise ValueError(f"Model '{self.name}': Failed to find loop dimension")
 
         # add zero output data arrays:
-        odims = {v: out_dims for v in out_vars}
+        odims = {v: tuple(out_dims) for v in out_vars}
         odata = {
             v: (
                 np.full(oshape, np.nan, dtype=FC.DTYPE)
                 if v not in init_vars
                 else prev[init_vars.index(v)].copy()
             )
             for v in out_vars
             if v not in data[-1]
         }
-        if (
-            n_prev
-            and FV.TXYH not in odata
-            and FV.X in odata
-            and FV.X in odata
-            and FV.Y in odata
-            and FV.H in odata
-        ):
-            txyh = np.zeros((data[0].n_states, data[0].n_turbines, 3), dtype=FC.DTYPE)
-            txyh[..., 0] = odata[FV.X]
-            txyh[..., 1] = odata[FV.Y]
-            txyh[..., 2] = odata[FV.H]
-            odata[FV.TXYH] = txyh
-            odims[FV.TXYH] = (FC.STATE, FC.TURBINE, FC.XYH)
-            del txyh
+
         if len(data) == 1:
-            data.append(Data(odata, odims, loop_dims))
+            data.append(FData(odata, odims, loop_dims))
         else:
             odata.update(data[-1])
             odims.update(data[-1].dims)
-            data[-1] = Data(odata, odims, loop_dims)
+            if len(data) == 2:
+                data[-1] = FData(odata, odims, loop_dims)
+            else:
+                data[-1] = TData(odata, odims, loop_dims)
         del odims, odata
 
-        # link chunk state indices from mdata to fdata and pdata:
+        # link chunk state indices from mdata to fdata and tdata:
         if FC.STATE in data[0]:
             for d in data[1:]:
                 d[FC.STATE] = data[0][FC.STATE]
 
+        # link weights from mdata to fdata:
+        if FV.WEIGHT in data[0]:
+            data[1][FV.WEIGHT] = data[0][FV.WEIGHT]
+            data[1].dims[FV.WEIGHT] = data[0].dims[FV.WEIGHT]
+
         # run model calculation:
+        self.ensure_variables(algo, *data)
         results = self.calculate(algo, *data, **calc_pars)
 
         # replace missing results by first input data with matching shape:
         missing = set(out_vars).difference(results.keys())
         if len(missing):
             found = set()
             for v in missing:
```

### Comparing `foxes-0.6.2/foxes/core/farm_controller.py` & `foxes-0.7/foxes/core/farm_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,17 +12,14 @@
 
     Attributes
     ----------
     turbine_types: list of foxes.core.TurbineType
         The turbine type of each turbine
     turbine_model_names: list of str
         Names of all turbine models found in the farm
-    turbine_model_sels: numpy.ndarray of bool
-        Selection flags for all turbine models,
-        shape: (n_states, n_turbines, n_models)
     pre_rotor_models: foxes.core.FarmDataModelList
         The turbine models with pre-rotor flag
     post_rotor_models: foxes.core.FarmDataModelList
         The turbine models without pre-rotor flag
     pars: dict
         Parameters for the turbine models, stored
         under their respecitve name
@@ -42,15 +39,14 @@
             under their respective name
 
         """
         super().__init__()
 
         self.turbine_types = None
         self.turbine_model_names = None
-        self.turbine_model_sels = None
         self.pre_rotor_models = None
         self.post_rotor_models = None
 
         self.pars = pars
 
     def sub_models(self):
         """
@@ -219,37 +215,40 @@
         mnames_pre, tmsels_pre = self._analyze_models(
             algo, pre_rotor=True, models=prer_models
         )
         mnames_post, tmsels_post = self._analyze_models(
             algo, pre_rotor=False, models=postr_models
         )
         tmsels = tmsels_pre + tmsels_post
+        self._tmall = [np.all(t) for t in tmsels]
         self.turbine_model_names = mnames_pre + mnames_post
         if len(self.turbine_model_names):
-            self.turbine_model_sels = np.stack(tmsels, axis=2)
+            self._tmsels = np.stack(tmsels, axis=2)
         else:
             raise ValueError(f"Controller '{self.name}': No turbine model found.")
 
-    def __get_pars(self, algo, models, ptype, mdata=None, st_sel=None, from_data=True):
+    def __get_pars(self, algo, models, ptype, mdata=None, downwind_index=None):
         """
         Private helper function for gathering model parameters.
         """
-        if from_data:
-            s = mdata[FC.TMODEL_SELS]
-        else:
-            s = self.turbine_model_sels
-        if st_sel is not None:
-            s = s & st_sel[:, :, None]
-
-        pars = [
-            {"st_sel": s[:, :, self.turbine_model_names.index(m.name)]} for m in models
-        ]
-        for mi, m in enumerate(models):
+        pars = []
+        for m in models:
+            mi = self.turbine_model_names.index(m.name)
+            if self._tmall[mi]:
+                s = np.s_[:, :] if downwind_index is None else np.s_[:, downwind_index]
+            else:
+                if downwind_index is None:
+                    s = mdata[FC.TMODEL_SELS][:, :, mi]
+                else:
+                    s = np.s_[
+                        mdata[FC.TMODEL_SELS][:, downwind_index, mi], downwind_index
+                    ]
+            pars.append({"st_sel": s})
             if m.name in self.pars:
-                pars[mi].update(self.pars[m.name][ptype])
+                pars[-1].update(self.pars[m.name][ptype])
 
         return pars
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
@@ -284,19 +283,22 @@
         idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().load_data(algo, verbosity)
+
         idata["coords"][FC.TMODELS] = self.turbine_model_names
         idata["data_vars"][FC.TMODEL_SELS] = (
             (FC.STATE, FC.TURBINE, FC.TMODELS),
-            self.turbine_model_sels,
+            self._tmsels,
         )
+        self._tmsels = None
+
         return idata
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
@@ -313,47 +315,45 @@
         return list(
             dict.fromkeys(
                 self.pre_rotor_models.output_farm_vars(algo)
                 + self.post_rotor_models.output_farm_vars(algo)
             )
         )
 
-    def calculate(self, algo, mdata, fdata, pre_rotor, st_sel=None):
+    def calculate(self, algo, mdata, fdata, pre_rotor, downwind_index=None):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
         pre_rotor: bool
             Flag for running pre-rotor or post-rotor
             models
-        st_sel: numpy.ndarray of bool, optional
-            Selection of states and turbines, shape:
-            (n_states, n_turbines). None for all.
+        downwind_index: int, optional
+            The index in the downwind order
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         s = self.pre_rotor_models if pre_rotor else self.post_rotor_models
-        pars = self.__get_pars(algo, s.models, "calc", mdata, st_sel, from_data=True)
+        pars = self.__get_pars(algo, s.models, "calc", mdata, downwind_index)
         res = s.calculate(algo, mdata, fdata, parameters=pars)
-        self.turbine_model_sels = mdata[FC.TMODEL_SELS]
         return res
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
@@ -362,8 +362,7 @@
             The calculation algorithm
         verbosity: int
             The verbosity level, 0 means silent
 
         """
         super().finalize(algo, verbosity)
         self.turbine_model_names = None
-        self.turbine_model_sels = None
```

### Comparing `foxes-0.6.2/foxes/core/farm_data_model.py` & `foxes-0.7/foxes/core/farm_data_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import abstractmethod
+import numpy as np
 
 from .data_calc_model import DataCalcModel
 import foxes.constants as FC
 
 
 class FarmDataModel(DataCalcModel):
     """
@@ -47,29 +48,50 @@
         -------
         output_vars: list of str
             The output variable names
 
         """
         return []
 
+    def ensure_variables(self, algo, mdata, fdata):
+        """
+        Add variables to fdata, initialized with NaN
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.Data
+            The model data
+        fdata: foxes.core.Data
+            The farm data
+
+        """
+        n_states = fdata.n_states
+        n_turbines = fdata.n_turbines
+        for v in self.output_farm_vars(algo):
+            if v not in fdata:
+                fdata[v] = np.full((n_states, n_turbines), np.nan, dtype=FC.DTYPE)
+                fdata.dims[v] = (FC.STATE, FC.TURBINE)
+
     @abstractmethod
     def calculate(self, algo, mdata, fdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
@@ -214,17 +236,17 @@
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
         parameters: list of dict, optional
             A list of parameter dicts, one for each model
 
         Returns
         -------
         results: dict
```

### Comparing `foxes-0.6.2/foxes/core/model.py` & `foxes-0.7/foxes/core/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from abc import ABC
 from itertools import count
+from copy import deepcopy
 
 import foxes.constants as FC
 from .data import Data
 
 
 class Model(ABC):
     """
@@ -33,16 +34,15 @@
         ext = "" if self._id == 0 else f"{self._id}"
         self.name = f"{type(self).__name__}{ext}"
 
         self._store = {}
         self.__initialized = False
 
     def __repr__(self):
-        t = type(self).__name__
-        return f"{self.name} ({t})"
+        return f"{type(self).__name__}()"
 
     @property
     def model_id(self):
         """
         Unique id based on the model type.
 
         Returns
@@ -183,198 +183,285 @@
     def get_data(
         self,
         variable,
         target,
         lookup="smfp",
         mdata=None,
         fdata=None,
-        pdata=None,
-        states_source_turbine=None,
-        upcast=False,
+        tdata=None,
+        downwind_index=None,
         accept_none=False,
         accept_nan=True,
         algo=None,
+        upcast=False,
     ):
         """
         Getter for a data entry in the model object
         or provided data sources
 
         Parameters
         ----------
         variable: str
             The variable, serves as data key
         target: str, optional
-            The dimensions identifier for the output, e.g
-            FC.STATE_TURBINE, FC.STATE_POINT
+            The dimensions identifier for the output,
+            FC.STATE_TURBINE, FC.STATE_TARGET or
+            FC.STATE_TARGET_TPOINT
         lookup: str
             The order of data sources. Combination of:
             's' for self,
             'm' for mdata,
             'f' for fdata,
-            'p' for pdata,
+            't' for tdata,
             'w' for wake modelling data
         mdata: foxes.core.Data, optional
             The model data
         fdata: foxes.core.Data, optional
             The farm data
-        pdata: foxes.core.Data, optional
-            The evaluation point data
-        states_source_turbine: numpy.ndarray, optional
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        upcast: bool, optional
-            Upcast array to dims if data is scalar
+        tdata: foxes.core.Data, optional
+            The target point data
+        downwind_index: int, optional
+            The index in the downwind order
         data_prio: bool
             First search the data source, then the object
         accept_none: bool
             Do not throw an error if data entry is None
         accept_nan: bool
             Do not throw an error if data entry is np.nan
         algo: foxes.core.Algorithm, optional
             The algorithm, needed for data from previous iteration
+        upcast: bool
+            Flag for ensuring targets dimension,
+            otherwise dimension 1 is entered
 
         """
 
         def _geta(a):
-            sources = [s for s in [mdata, fdata, pdata, algo, self] if s is not None]
+            sources = [s for s in [mdata, fdata, tdata, algo, self] if s is not None]
             for s in sources:
-                if a == "states_i0":
-                    out = s.states_i0(counter=True, algo=algo)
-                    if out is not None:
-                        return out
-                else:
-                    try:
+                try:
+                    if a == "states_i0":
+                        out = s.states_i0(counter=True, algo=algo)
+                        if out is not None:
+                            return out
+                    else:
                         out = getattr(s, a)
                         if out is not None:
                             return out
-                    except AttributeError:
-                        pass
+                except AttributeError:
+                    pass
             raise KeyError(
-                f"Model '{self.name}': Failed to determine '{a}'. Maybe add to arguments of get_data: mdata, fdata, pdata, algo?"
+                f"Model '{self.name}': Failed to determine '{a}'. Maybe add to arguments of get_data: mdata, fdata, tdata, algo?"
             )
 
         n_states = _geta("n_states")
         if target == FC.STATE_TURBINE:
             n_turbines = _geta("n_turbines")
             dims = (FC.STATE, FC.TURBINE)
-        elif target == FC.STATE_POINT:
-            n_points = _geta("n_points")
-            dims = (FC.STATE, FC.POINT)
+            shp = (n_states, n_turbines)
+        elif target == FC.STATE_TARGET:
+            n_targets = _geta("n_targets")
+            dims = (FC.STATE, FC.TARGET)
+            shp = (n_states, n_targets)
+        elif target == FC.STATE_TARGET_TPOINT:
+            n_targets = _geta("n_targets")
+            n_tpoints = _geta("n_tpoints")
+            dims = (FC.STATE, FC.TARGET, FC.TPOINT)
+            shp = (n_states, n_targets, n_tpoints)
         else:
             raise KeyError(
-                f"Model '{self.name}': Wrong parameter 'target = {target}'. Choices: {FC.STATE_TURBINE}, {FC.STATE_POINT}"
+                f"Model '{self.name}': Wrong parameter 'target = {target}'. Choices: {FC.STATE_TURBINE}, {FC.STATE_TARGET}, {FC.STATE_TARGET_TPOINT}"
             )
 
         out = None
+        out_dims = None
         for s in lookup:
             # lookup self:
             if s == "s" and hasattr(self, variable):
                 a = getattr(self, variable)
-
-                if a is not None and upcast:
-                    if target == FC.STATE_TURBINE:
+                if a is not None:
+                    if not upcast:
+                        out = a
+                        out_dims = None
+                    elif target == FC.STATE_TURBINE:
                         out = np.full((n_states, n_turbines), np.nan, dtype=FC.DTYPE)
                         out[:] = a
-                    elif target == FC.STATE_POINT:
-                        out = np.full((n_states, n_points), np.nan, dtype=FC.DTYPE)
+                        out_dims = (FC.STATE, FC.TURBINE)
+                    elif target == FC.STATE_TARGET:
+                        out = np.full((n_states, n_targets), np.nan, dtype=FC.DTYPE)
                         out[:] = a
-                    else:
-                        raise KeyError(
-                            f"Model '{self.name}': Wrong parameter 'target = {target}' for 'upcast = True' in get_data. Choose: FC.STATE_TURBINE, FC.STATE_POINT"
+                        out_dims = (FC.STATE, FC.TARGET)
+                    elif target == FC.STATE_TARGET_TPOINT:
+                        out = np.full(
+                            (n_states, n_targets, n_tpoints), np.nan, dtype=FC.DTYPE
                         )
-
-                else:
-                    out = a
+                        out[:] = a
+                        out_dims = (FC.STATE, FC.TARGET, FC.TPOINT)
+                    else:
+                        raise NotImplementedError
 
             # lookup mdata:
             elif (
                 s == "m"
                 and mdata is not None
                 and variable in mdata
-                and len(mdata.dims[variable]) > 1
-                and tuple(mdata.dims[variable][:2]) == dims
+                and tuple(mdata.dims[variable]) == dims
             ):
                 out = mdata[variable]
+                out_dims = dims
 
             # lookup fdata:
             elif (
                 s == "f"
                 and fdata is not None
                 and variable in fdata
-                and len(fdata.dims[variable]) > 1
-                and tuple(fdata.dims[variable][:2]) == (FC.STATE, FC.TURBINE)
+                and tuple(fdata.dims[variable]) == (FC.STATE, FC.TURBINE)
             ):
-                # direct fdata:
-                if target == FC.STATE_TURBINE:
-                    out = fdata[variable]
-
-                # translate state-turbine to state-point data:
-                elif target == FC.STATE_POINT and states_source_turbine is not None:
-                    # from fdata, uniform for points:
-                    st_sel = (np.arange(n_states), states_source_turbine)
-                    out = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-                    out[:] = fdata[variable][st_sel][:, None]
-
-                    # from previous iteration, if requested:
-                    if pdata is not None and FC.STATES_SEL in pdata:
-                        if not np.all(
-                            states_source_turbine == pdata[FC.STATE_SOURCE_TURBINE]
-                        ):
-                            raise ValueError(
-                                f"Model '{self.name}': Mismatch of 'states_source_turbine'. Expected {list(pdata[FC.STATE_SOURCE_TURBINE])}, got {list(states_source_turbine)}"
-                            )
-
-                        i0 = _geta("states_i0")
-                        sp = pdata[FC.STATES_SEL]
-                        sel = sp < i0
-                        if np.any(sel):
-                            if algo is None or not hasattr(algo, "prev_farm_results"):
-                                raise KeyError(
-                                    f"Model '{self.name}': Argument algo is either not given, or not an iterative algorithm"
-                                )
-
-                            prev_fdata = getattr(algo, "prev_farm_results")
-                            if prev_fdata is None:
-                                out[sel] = 0
-                            else:
-                                st = np.zeros_like(sp)
-                                st[:] = states_source_turbine[:, None]
-                                out[sel] = prev_fdata[variable].to_numpy()[
-                                    sp[sel], st[sel]
-                                ]
+                out = fdata[variable]
+                out_dims = (FC.STATE, FC.TURBINE)
 
             # lookup pdata:
             elif (
-                s == "p"
-                and pdata is not None
-                and variable in pdata
-                and len(pdata.dims[variable]) > 1
-                and tuple(pdata.dims[variable][:2]) == dims
+                s == "t"
+                and tdata is not None
+                and variable in tdata
+                and tuple(tdata.dims[variable]) == (FC.STATE, FC.TARGET, FC.TPOINT)
             ):
-                out = pdata[variable]
+                out = tdata[variable]
+                out_dims = (FC.STATE, FC.TARGET, FC.TPOINT)
 
             # lookup wake modelling data:
             elif (
                 s == "w"
-                and target == FC.STATE_POINT
                 and fdata is not None
-                and pdata is not None
+                and tdata is not None
                 and variable in fdata
-                and len(fdata.dims[variable]) > 1
-                and tuple(fdata.dims[variable][:2]) == (FC.STATE, FC.TURBINE)
-                and states_source_turbine is not None
+                and tuple(fdata.dims[variable]) == (FC.STATE, FC.TURBINE)
+                and downwind_index is not None
                 and algo is not None
             ):
-                out = algo.wake_frame.get_wake_modelling_data(
-                    algo, variable, states_source_turbine, fdata, pdata
+                out, out_dims = algo.wake_frame.get_wake_modelling_data(
+                    algo,
+                    variable,
+                    downwind_index,
+                    fdata,
+                    tdata=tdata,
+                    target=target,
+                    upcast=upcast,
                 )
 
             if out is not None:
                 break
 
+        # cast dimensions:
+        if out_dims != dims:
+            if out_dims is None:
+                if upcast:
+                    out0 = out
+                    out = np.zeros(shp, dtype=FC.DTYPE)
+                    out[:] = out0
+                    out_dims = dims
+                    del out0
+                else:
+                    out_dims = tuple([1 for _ in dims])
+
+            elif out_dims == (FC.STATE, FC.TURBINE):
+                if downwind_index is None:
+                    raise KeyError(
+                        f"Require downwind_index for target {target} and out dims {out_dims}"
+                    )
+                out0 = out[:, downwind_index, None]
+                if len(dims) == 3:
+                    out0 = out0[:, :, None]
+                if upcast:
+                    out = np.zeros(shp, dtype=FC.DTYPE)
+                    out[:] = out0
+                    out_dims = dims
+                else:
+                    out = out0
+                    out_dims = (FC.STATE, 1) if len(dims) == 2 else (FC.STATE, 1, 1)
+                del out0
+
+            elif out_dims == (FC.STATE, 1):
+                out0 = out
+                if len(dims) == 3:
+                    out0 = out0[:, :, None]
+                    out_dims = (FC.STATE, 1, 1)
+                if upcast:
+                    out = np.zeros(shp, dtype=FC.DTYPE)
+                    out[:] = out0
+                    out_dims = dims
+                else:
+                    out = out0
+                del out0
+
+            elif out_dims == (FC.STATE, 1, 1):
+                out0 = out
+                if len(dims) == 2:
+                    out0 = out0[:, :, 0]
+                    out_dims = (FC.STATE, 1)
+                if upcast:
+                    out = np.zeros(shp, dtype=FC.DTYPE)
+                    out[:] = out0
+                    out_dims = dims
+                else:
+                    out = out0
+                del out0
+
+            else:
+                raise NotImplementedError(
+                    f"No casting implemented for target {target} and out dims {out_dims} fo upcast {upcast}"
+                )
+
+        # data from other chunks, only with iterations:
+        if (
+            target in [FC.STATE_TARGET, FC.STATE_TARGET_TPOINT]
+            and fdata is not None
+            and variable in fdata
+            and tdata is not None
+            and FC.STATES_SEL in tdata
+        ):
+            if out_dims != dims:
+                raise ValueError(
+                    f"Model '{self.name}': Iteration data found for variable '{variable}', but missing upcast: out_dims = {out_dims}, expecting {dims}"
+                )
+            if downwind_index is None:
+                raise KeyError(
+                    f"Model '{self.name}': Require downwind_index for obtaining results from previous iteration"
+                )
+            if tdata[FC.STATE_SOURCE_ORDERI] != downwind_index:
+                raise ValueError(
+                    f"Model '{self.name}': Expecting downwind_index {tdata[FC.STATE_SOURCE_ORDERI]}, got {downwind_index}"
+                )
+            if algo is None:
+                raise ValueError(
+                    f"Model '{self.name}': Iteration data found for variable '{variable}', requiring algo"
+                )
+
+            i0 = _geta("states_i0")
+            sts = tdata[FC.STATES_SEL]
+            if target == FC.STATE_TARGET and tdata.n_tpoints != 1:
+                # find the mean index and round it to nearest integer:
+                sts = tdata.tpoint_mean(FC.STATES_SEL)[:, :, None]
+                sts = (sts + 0.5).astype(FC.ITYPE)
+            sel = sts < i0
+            if np.any(sel):
+                if not hasattr(algo, "prev_farm_results"):
+                    raise KeyError(
+                        f"Model '{self.name}': Iteration data found for variable '{variable}', requiring iterative algorithm"
+                    )
+                prev_fres = getattr(algo, "prev_farm_results")
+                if prev_fres is not None:
+                    prev_data = prev_fres[variable].to_numpy()[sts[sel], downwind_index]
+                    if target == FC.STATE_TARGET:
+                        out[sel[:, :, 0]] = prev_data
+                    else:
+                        out[sel] = prev_data
+                    del prev_fres, prev_data
+
         # check for None:
         if not accept_none and out is None:
             raise ValueError(
                 f"Model '{self.name}': Variable '{variable}' is requested but not found."
             )
 
         # check for nan:
@@ -406,16 +493,18 @@
         """
         i0 = data.states_i0(counter=True, algo=algo)
         if i0 not in self._store:
             self._store[i0] = Data(
                 data={}, dims={}, loop_dims=data.loop_dims, name=f"{self.name}_{i0}"
             )
 
-        self._store[i0][name] = data[name]
-        self._store[i0].dims[name] = data.dims[name] if name in data.dims else None
+        self._store[i0][name] = deepcopy(data[name])
+        self._store[i0].dims[name] = (
+            deepcopy(data.dims[name]) if name in data.dims else None
+        )
 
     def from_data_or_store(self, name, algo, data, ret_dims=False, safe=False):
         """
         Get data from mdata or local store
 
         Parameters
         ----------
@@ -446,39 +535,7 @@
         if not safe or (i0 in self._store and name in self._store[i0]):
             if ret_dims:
                 return self._store[i0][name], self._store[i0].dims[name]
             else:
                 return self._store[i0][name]
         else:
             return (None, None) if ret_dims else None
-
-    '''
-    @classmethod
-    def reduce_states(cls, sel_states, objs):
-        """
-        Modifies the given objects by selecting a
-        subset of states.
-
-        Parameters
-        ----------
-        sel_states: list of int
-            The states selection
-        objs: list of foxes.core.Data
-            The objects, e.g. [mdata, fdata, pdata]
-
-        Returns
-        -------
-        mobjs: list of foxes.core.Data
-            The modified objects with reduced
-            states dimension
-
-        """
-        out = []
-        for o in objs:
-            data = {
-                v: d[sel_states] if o.dims[v][0] == FC.STATE else d
-                for v, d in o.items()
-            }
-            out.append(Data(data, o.dims, loop_dims=o.loop_dims, name=o.name))
-
-        return out
-        '''
```

### Comparing `foxes-0.6.2/foxes/core/partial_wakes_model.py` & `foxes-0.7/foxes/models/wake_superpositions/ws_linear.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,199 +1,180 @@
-from abc import abstractmethod
+import numpy as np
 
-from foxes.utils import all_subclasses
+from foxes.core import WakeSuperposition
+import foxes.variables as FV
+import foxes.constants as FC
 
-from .model import Model
 
-
-class PartialWakesModel(Model):
+class WSLinear(WakeSuperposition):
     """
-    Abstract base class for partial wakes models.
-
-    Partial wakes models compute wake effects
-    for rotor effective quantities.
+    Linear supersposition of wind deficit results
 
     Attributes
     ----------
-    wake_models: list of foxes.core.WakeModel
-        The wake model selection
-    wake_frame: foxes.core.WakeFrame, optional
-        The wake frame
+    scale_amb: bool
+        Flag for scaling wind deficit with ambient wind speed
+        instead of waked wind speed
+    lim_low: float
+        Lower limit of the final waked wind speed
+    lim_high: float
+        Upper limit of the final waked wind speed
 
-    :group: core
+    :group: models.wake_superpositions
 
     """
 
-    def __init__(self, wake_models=None, wake_frame=None):
+    def __init__(self, scale_amb=False, lim_low=None, lim_high=None):
         """
         Constructor.
 
         Parameters
         ----------
-        wake_models: list of foxes.core.WakeModel
-            The wake model selection, None for all
-            from algorithm.
-        wake_frame: foxes.core.WakeFrame, optional
-            The wake frame, None takes from algorithm
+        scale_amb: bool
+            Flag for scaling wind deficit with ambient wind speed
+            instead of waked wind speed
+        lim_low: float
+            Lower limit of the final waked wind speed
+        lim_high: float
+            Upper limit of the final waked wind speed
 
         """
         super().__init__()
 
-        self._wmodels = wake_models
-        self._wframe = wake_frame
-
-    def sub_models(self):
-        """
-        List of all sub-models
-
-        Returns
-        -------
-        smdls: list of foxes.core.Model
-            Names of all sub models
-
-        """
-        return self.wake_models + [self.wake_frame]
-
-    def initialize(self, algo, verbosity=0):
-        """
-        Initializes the model.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
-
-        """
-        self.wake_models = algo.wake_models if self._wmodels is None else self._wmodels
-        self.wake_frame = algo.wake_frame if self._wframe is None else self._wframe
-        super().initialize(algo, verbosity)
+        self.scale_amb = scale_amb
+        self.lim_low = lim_low
+        self.lim_high = lim_high
+
+    def __repr__(self):
+        a = f"scale_amb={self.scale_amb}, lim_low={self.lim_low}, lim_high={self.lim_high}"
+        return f"{type(self).__name__}({a})"
 
-    @abstractmethod
-    def new_wake_deltas(self, algo, mdata, fdata):
+    def input_farm_vars(self, algo):
         """
-        Creates new initial wake deltas, filled
-        with zeros.
+        The variables which are needed for running
+        the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
 
         Returns
         -------
-        wake_deltas: dict
-            Keys: Variable name str, values: any
-        pdata: foxes.core.Data
-            The evaluation point data
+        input_vars: list of str
+            The input variable names
 
         """
-        pass
+        return [FV.AMB_REWS] if self.scale_amb else [FV.REWS]
 
-    @abstractmethod
-    def contribute_to_wake_deltas(
+    def add_wake(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        wake_deltas,
+        tdata,
+        downwind_index,
+        st_sel,
+        variable,
+        wake_delta,
+        wake_model_result,
     ):
         """
-        Modifies wake deltas by contributions from the
-        specified wake source turbines.
+        Add a wake delta to previous wake deltas,
+        at rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray of int
-            For each state, one turbine index corresponding
-            to the wake causing turbine. Shape: (n_states,)
-        wake_deltas: Any
-            The wake deltas object created by the
-            `new_wake_deltas` function
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        st_sel: numpy.ndarray of bool
+            The selection of targets, shape: (n_states, n_targets)
+        variable: str
+            The variable name for which the wake deltas applies
+        wake_delta: numpy.ndarray
+            The original wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
+        wake_model_result: numpy.ndarray
+            The new wake deltas of the selected rotors,
+            shape: (n_st_sel, n_tpoints, ...)
+
+        Returns
+        -------
+        wdelta: numpy.ndarray
+            The updated wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
 
         """
-        pass
+        if variable not in [FV.REWS, FV.REWS2, FV.REWS3, FV.WS]:
+            raise ValueError(
+                f"Superposition '{self.name}': Expecting wind speed variable, got {variable}"
+            )
+
+        if np.any(st_sel):
+            scale = self.get_data(
+                FV.AMB_REWS if self.scale_amb else FV.REWS,
+                FC.STATE_TARGET,
+                lookup="w",
+                algo=algo,
+                fdata=fdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
+                upcast=True,
+            )[st_sel, None]
 
-    @abstractmethod
-    def evaluate_results(
+            wake_delta[st_sel] += scale * wake_model_result
+
+        return wake_delta
+
+    def calc_final_wake_delta(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        wake_deltas,
-        states_turbine,
-        amb_res=None,
+        variable,
+        amb_results,
+        wake_delta,
     ):
         """
-        Updates the farm data according to the wake
-        deltas.
+        Calculate the final wake delta after adding all
+        contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-            Modified in-place by this function
-        pdata: foxes.core.Data
-            The evaluation point data
-        wake_deltas: Any
-            The wake deltas object, created by the
-            `new_wake_deltas` function and filled
-            by `contribute_to_wake_deltas`
-        states_turbine: numpy.ndarray of int
-            For each state, the index of one turbine
-            for which to evaluate the wake deltas.
-            Shape: (n_states,)
-        amb_res: dict, optional
-            Ambient states results. Keys: var str, values:
-            numpy.ndarray of shape (n_states, n_points)
-
-        """
-        pass
-
-    @classmethod
-    def new(cls, pwake_type, **kwargs):
-        """
-        Run-time partial wakes factory.
+        variable: str
+            The variable name for which the wake deltas applies
+        amb_results: numpy.ndarray
+            The ambient results at targets,
+            shape: (n_states, n_targets, n_tpoints)
+        wake_delta: numpy.ndarray
+            The wake deltas at targets, shape:
+            (n_states, n_targets, n_tpoints)
 
-        Parameters
-        ----------
-        pwake_type: str
-            The selected derived class name
+        Returns
+        -------
+        final_wake_delta: numpy.ndarray
+            The final wake delta, which will be added to the ambient
+            results by simple plus operation. Shape:
+            (n_states, n_targets, n_tpoints)
 
         """
-
-        if pwake_type is None:
-            return None
-
-        allc = all_subclasses(cls)
-        found = pwake_type in [scls.__name__ for scls in allc]
-
-        if found:
-            for scls in allc:
-                if scls.__name__ == pwake_type:
-                    return scls(**kwargs)
-
-        else:
-            estr = "Partial wakes model type '{}' is not defined, available types are \n {}".format(
-                pwake_type, sorted([i.__name__ for i in allc])
-            )
-            raise KeyError(estr)
+        w = wake_delta
+        if self.lim_low is not None:
+            w = np.maximum(w, self.lim_low - amb_results)
+        if self.lim_high is not None:
+            w = np.minimum(w, self.lim_high - amb_results)
+        return w
```

### Comparing `foxes-0.6.2/foxes/core/point_data_model.py` & `foxes-0.7/foxes/core/point_data_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 from abc import abstractmethod
 
 from .data_calc_model import DataCalcModel
 import foxes.constants as FC
 
 
 class PointDataModel(DataCalcModel):
@@ -22,38 +23,64 @@
         -------
         output_vars: list of str
             The output variable names
 
         """
         return []
 
+    def ensure_variables(self, algo, mdata, fdata, tdata):
+        """
+        Add variables to tdata, initialized with NaN
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.Data
+            The model data
+        fdata: foxes.core.Data
+            The farm data
+        tdata: foxes.core.Data
+            The target point data
+
+        """
+        for v in self.output_point_vars(algo):
+            if v not in tdata:
+                tdata[v] = np.full(
+                    (tdata.n_states, tdata.n_targets, tdata.n_tpoints),
+                    np.nan,
+                    dtype=FC.DTYPE,
+                )
+                tdata.dims[v] = (FC.STATE, FC.TARGET, FC.TPOINT)
+
     @abstractmethod
-    def calculate(self, algo, mdata, fdata, pdata):
+    def calculate(self, algo, mdata, fdata, tdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The point data
+        tdata: foxes.core.TData
+            The target point data
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_points)
+            Values: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints)
 
         """
         pass
 
     def run_calculation(self, algo, *data, out_vars, **calc_pars):
         """
         Starts the model calculation in parallel, via
@@ -74,22 +101,27 @@
 
         Returns
         -------
         results: xarray.Dataset
             The calculation results
 
         """
-        return super().run_calculation(
+        results = super().run_calculation(
             algo,
             *data,
             out_vars=out_vars,
-            loop_dims=[FC.STATE, FC.POINT],
-            out_core_vars=[FC.VARS],
+            loop_dims=[FC.STATE, FC.TARGET],
+            out_core_vars=[FC.TPOINT, FC.VARS],
             **calc_pars,
         )
+        if results.sizes[FC.TPOINT] != 1:
+            raise ValueError(
+                f"PointDataModel '{self.name}': Expecting dimension '{FC.TPOINT}' of size 1, found {results.sizes[FC.TPOINT]}"
+            )
+        return results.sel({FC.TPOINT: 0}).rename({FC.TARGET: FC.POINT})
 
     def __add__(self, m):
         if isinstance(m, list):
             return PointDataModelList([self] + m)
         elif isinstance(m, PointDataModelList):
             return PointDataModelList([self] + m.models)
         else:
@@ -166,50 +198,51 @@
 
         """
         ovars = []
         for m in self.models:
             ovars += m.output_point_vars(algo)
         return list(dict.fromkeys(ovars))
 
-    def calculate(self, algo, mdata, fdata, pdata, parameters=None):
+    def calculate(self, algo, mdata, fdata, tdata, parameters=None):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The point data
+        tdata: foxes.core.TData
+            The target point data
         parameters: list of dict, optional
             A list of parameter dicts, one for each model
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_points)
+            Values: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints)
 
         """
         if parameters is None:
             parameters = [{}] * len(self.models)
         elif not isinstance(parameters, list):
             raise ValueError(
                 f"{self.name}: Wrong parameters type, expecting list, got {type(parameters).__name__}"
             )
         elif len(parameters) != len(self.models):
             raise ValueError(
                 f"{self.name}: Wrong parameters length, expecting list with {len(self.models)} entries, got {len(parameters)}"
             )
 
         for mi, m in enumerate(self.models):
-            res = m.calculate(algo, mdata, fdata, pdata, **parameters[mi])
-            pdata.update(res)
+            res = m.calculate(algo, mdata, fdata, tdata, **parameters[mi])
+            tdata.update(res)
 
-        return {v: pdata[v] for v in self.output_point_vars(algo)}
+        return {v: tdata[v] for v in self.output_point_vars(algo)}
```

### Comparing `foxes-0.6.2/foxes/core/rotor_model.py` & `foxes-0.7/foxes/core/rotor_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from abc import abstractmethod
 
 import foxes.variables as FV
 import foxes.constants as FC
 from .farm_data_model import FarmDataModel
 from foxes.utils import wd2uv, uv2wd, all_subclasses
 
-from .data import Data
+from .data import TData
 
 
 class RotorModel(FarmDataModel):
     """
     Abstract base class of rotor models.
 
     Rotor models calculate ambient farm data from
@@ -37,14 +37,18 @@
             The variables that are calculated by the model
             (Their ambients are added automatically)
 
         """
         super().__init__()
         self.calc_vars = calc_vars
 
+        self.RPOINTS = self.var("rpoints")
+        self.RWEIGHTS = self.var("rweights")
+        self.AMBRES = self.var("amb_res")
+
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
@@ -114,17 +118,17 @@
         """
         Calculates rotor points from design points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
 
         Returns
         -------
         points: numpy.ndarray
             The rotor points, shape:
             (n_states, n_turbines, n_rpoints, 3)
@@ -148,35 +152,35 @@
         points[:] = fdata[FV.TXYH][:, :, None, :]
         points[:] += (
             0.5 * D[:, :, None, None] * np.einsum("stad,pa->stpd", rax, dpoints)
         )
 
         return points
 
-    def _set_res(self, fdata, v, res, stsel):
+    def _set_res(self, fdata, v, res, downwind_index):
         """
         Helper function for results setting
         """
-        if stsel is None:
+        if downwind_index is None:
             fdata[v] = res.copy()
         elif res.shape[1] == 1:
-            fdata[v][stsel] = res[:, 0]
+            fdata[v][:, downwind_index] = res[:, 0]
         else:
             raise ValueError(
-                f"Rotor model '{self.name}': states_turbine is not None, but results shape for '{v}' has more than one turbine, {res.shape}"
+                f"Rotor model '{self.name}': downwind_index is not None, but results shape for '{v}' has more than one turbine, {res.shape}"
             )
 
     def eval_rpoint_results(
         self,
         algo,
         mdata,
         fdata,
-        rpoint_results,
+        tdata,
         weights,
-        states_turbine=None,
+        downwind_index=None,
         copy_to_ambient=False,
     ):
         """
         Evaluate rotor point results.
 
         This function modifies `fdata`, either
         for all turbines or one turbine per state,
@@ -184,87 +188,76 @@
         the latter case, the turbine dimension of the
         `rpoint_results` is expected to have size one.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        rpoint_results: dict
-            The results at rotor points. Keys: variable str.
-            Values: numpy.ndarray, shape if `states_turbine`
-            is None: (n_states, n_turbines, n_rpoints).
-            Else: (n_states, 1, n_rpoints)
+        tdata: foxes.core.TData
+            The target point data
         weights: numpy.ndarray
             The rotor point weights, shape: (n_rpoints,)
-        states_turbine: numpy.ndarray of int, optional
-            The turbine indices, one per state. Shape: (n_states,)
-        copy_to_ambient: bool, optional
+        downwind_index: int, optional
+            The index in the downwind order
+        copy_to_ambient: bool
             If `True`, the fdata results are copied to ambient
             variables after calculation
 
         """
-
-        n_states = mdata.n_states
-        n_turbines = algo.n_turbines
-        if states_turbine is not None:
-            stsel = (np.arange(n_states), states_turbine)
-        else:
-            stsel = None
-
         uvp = None
         uv = None
         if (
             FV.WS in self.calc_vars
             or FV.WD in self.calc_vars
             or FV.YAW in self.calc_vars
             or FV.REWS in self.calc_vars
             or FV.REWS2 in self.calc_vars
             or FV.REWS3 in self.calc_vars
         ):
-            wd = rpoint_results[FV.WD]
-            ws = rpoint_results[FV.WS]
+            wd = tdata[FV.WD]
+            ws = tdata[FV.WS]
             uvp = wd2uv(wd, ws, axis=-1)
             uv = np.einsum("stpd,p->std", uvp, weights)
 
         wd = None
         vdone = []
         for v in self.calc_vars:
             if v == FV.WD or v == FV.YAW:
                 if wd is None:
                     wd = uv2wd(uv, axis=-1)
-                self._set_res(fdata, v, wd, stsel)
+                self._set_res(fdata, v, wd, downwind_index)
                 vdone.append(v)
 
             elif v == FV.WS:
                 ws = np.linalg.norm(uv, axis=-1)
-                self._set_res(fdata, v, ws, stsel)
+                self._set_res(fdata, v, ws, downwind_index)
                 del ws
                 vdone.append(v)
         del uv, wd
 
         if (
             FV.REWS in self.calc_vars
             or FV.REWS2 in self.calc_vars
             or FV.REWS3 in self.calc_vars
         ):
-            if stsel is None:
+            if downwind_index is None:
                 yaw = fdata[FV.YAW].copy()
             else:
-                yaw = fdata[FV.YAW][stsel][:, None]
+                yaw = fdata[FV.YAW][:, downwind_index, None]
             nax = wd2uv(yaw, axis=-1)
             wsp = np.einsum("stpd,std->stp", uvp, nax)
 
             for v in self.calc_vars:
                 if v == FV.REWS:
                     rews = np.maximum(np.einsum("stp,p->st", wsp, weights), 0.0)
-                    self._set_res(fdata, v, rews, stsel)
+                    self._set_res(fdata, v, rews, downwind_index)
                     del rews
                     vdone.append(v)
 
                 elif v == FV.REWS2:
                     # For highly inhomogeneous wind fields
                     # and multiple rotor points some of the uv
                     # vectors may have negative projections onto the
@@ -274,141 +267,130 @@
                             np.maximum(
                                 np.einsum("stp,p->st", np.sign(wsp) * wsp**2, weights),
                                 0.0,
                             )
                         )
                     else:
                         rews2 = np.sqrt(np.einsum("stp,p->st", wsp**2, weights))
-                    self._set_res(fdata, v, rews2, stsel)
+                    self._set_res(fdata, v, rews2, downwind_index)
                     del rews2
                     vdone.append(v)
 
                 elif v == FV.REWS3:
                     # For highly inhomogeneous wind fields
                     # and multiple rotor points some of the uv
                     # vectors may have negative projections onto the
                     # turbine axis direction:
                     if uvp.shape[2] > 1:
                         rews3 = np.maximum(
                             np.einsum("stp,p->st", wsp**3, weights), 0.0
                         ) ** (1.0 / 3.0)
                     else:
                         rews3 = (np.einsum("stp,p->st", wsp**3, weights)) ** (1.0 / 3.0)
-                    self._set_res(fdata, v, rews3, stsel)
+                    self._set_res(fdata, v, rews3, downwind_index)
                     del rews3
                     vdone.append(v)
 
             del wsp
         del uvp
 
         for v in self.calc_vars:
             if v not in vdone:
-                res = np.einsum("stp,p->st", rpoint_results[v], weights)
-                self._set_res(fdata, v, res, stsel)
+                res = np.einsum("stp,p->st", tdata[v], weights)
+                self._set_res(fdata, v, res, downwind_index)
             if copy_to_ambient and v in FV.var2amb:
                 fdata[FV.var2amb[v]] = fdata[v].copy()
 
     def calculate(
         self,
         algo,
         mdata,
         fdata,
         rpoints=None,
         weights=None,
         store_rpoints=False,
         store_rweights=False,
         store_amb_res=False,
-        states_turbine=None,
+        downwind_index=None,
     ):
         """
         Calculate ambient rotor effective results.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
         rpoints: numpy.ndarray, optional
             The rotor points, or None for automatic for
             this rotor. Shape: (n_states, n_turbines, n_rpoints, 3)
         weights: numpy.ndarray, optional
             The rotor point weights, or None for automatic
             for this rotor. Shape: (n_rpoints,)
         store_rpoints: bool, optional
             Switch for storing rotor points to mdata
         store_rweights: bool, optional
             Switch for storing rotor point weights to mdata
         store_amb_res: bool, optional
             Switch for storing ambient rotor point reults as they
             come from the states to mdata
-        states_turbine: numpy.ndarray of int, optional
-            The turbine indices, one per state. Shape: (n_states,)
+        downwind_index: int, optional
+            Only compute for index in the downwind order
 
         Returns
         -------
         results: dict
             results dict. Keys: Variable name str. Values:
             numpy.ndarray with results, shape: (n_states, n_turbines)
 
         """
 
         if rpoints is None:
-            rpoints = mdata.get(FC.RPOINTS, self.get_rotor_points(algo, mdata, fdata))
+            rpoints = mdata.get(self.RPOINTS, self.get_rotor_points(algo, mdata, fdata))
         if store_rpoints:
-            mdata[FC.RPOINTS] = rpoints
-            mdata.dims[FC.RPOINTS] = (FC.STATE, FC.TURBINE, FC.RPOINT, FC.XYH)
-            self.data_to_store(FC.RPOINTS, algo, mdata)
-
-        if states_turbine is not None:
-            n_states = mdata.n_states
-            stsel = (np.arange(n_states), states_turbine)
-            rpoints = rpoints[stsel][:, None]
-        n_states, n_turbines, n_rpoints, __ = rpoints.shape
-        n_points = n_turbines * n_rpoints
+            mdata[self.RPOINTS] = rpoints
+            mdata.dims[self.RPOINTS] = (FC.STATE, FC.TURBINE, FC.TPOINT, FC.XYH)
+            self.data_to_store(self.RPOINTS, algo, mdata)
+
+        if downwind_index is not None:
+            rpoints = rpoints[:, downwind_index, None]
 
         if weights is None:
-            weights = mdata.get(FC.RWEIGHTS, self.rotor_point_weights())
+            weights = mdata.get(FC.TWEIGHTS, self.rotor_point_weights())
         if store_rweights:
-            mdata[FC.RWEIGHTS] = weights
-            mdata.dims[FC.RWEIGHTS] = (FC.RPOINT,)
-            self.data_to_store(FC.RWEIGHTS, algo, mdata)
+            mdata[self.RWEIGHTS] = weights
+            mdata.dims[self.RWEIGHTS] = (FC.TPOINT,)
+            self.data_to_store(self.RWEIGHTS, algo, mdata)
 
+        tdata = TData.from_tpoints(rpoints, weights)
         svars = algo.states.output_point_vars(algo)
-        points = rpoints.reshape(n_states, n_points, 3)
-        pdata = {FC.POINTS: points}
-        pdims = {FC.POINTS: (FC.STATE, FC.POINT, FC.XYH)}
-        pdata.update(
-            {v: np.full((n_states, n_points), np.nan, dtype=FC.DTYPE) for v in svars}
-        )
-        pdims.update({v: (FC.STATE, FC.POINT) for v in svars})
-        pdata = Data(pdata, pdims, loop_dims=[FC.STATE, FC.POINT])
-        del pdims, points
-
-        sres = algo.states.calculate(algo, mdata, fdata, pdata)
-        pdata.update(sres)
-        del sres
-
-        rpoint_results = {}
         for v in svars:
-            rpoint_results[v] = pdata[v].reshape(n_states, n_turbines, n_rpoints)
+            tdata.add(
+                v,
+                data=np.full_like(rpoints[..., 0], np.nan),
+                dims=(FC.STATE, FC.TARGET, FC.TPOINT),
+            )
+
+        sres = algo.states.calculate(algo, mdata, fdata, tdata)
+        tdata.update(sres)
 
         if store_amb_res:
-            mdata[FC.AMB_RPOINT_RESULTS] = rpoint_results
-            self.data_to_store(FC.AMB_RPOINT_RESULTS, algo, mdata)
+            mdata[self.AMBRES] = sres.copy()
+            self.data_to_store(self.AMBRES, algo, mdata)
 
         self.eval_rpoint_results(
             algo,
             mdata,
             fdata,
-            rpoint_results,
+            tdata,
             weights,
-            states_turbine,
+            downwind_index,
             copy_to_ambient=True,
         )
 
         return {v: fdata[v] for v in self.output_farm_vars(algo)}
 
     @classmethod
     def new(cls, rmodel_type, *args, **kwargs):
```

### Comparing `foxes-0.6.2/foxes/core/states.py` & `foxes-0.7/foxes/core/states.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,40 +241,40 @@
         -------
         output_vars: list of str
             The output variable names
 
         """
         return self.states.output_point_vars(algo)
 
-    def calculate(self, algo, mdata, fdata, pdata):
+    def calculate(self, algo, mdata, fdata, tdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The point data
+        tdata: foxes.core.TData
+            The target point data
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
-        return self.pmodels.calculate(algo, mdata, fdata, pdata)
+        return self.pmodels.calculate(algo, mdata, fdata, tdata)
 
     def __add__(self, m):
         models = self.pmodels.models[1:]
         if isinstance(m, list):
             return ExtendedStates(self.states, models + m)
         elif isinstance(m, ExtendedStates):
             if m.states is not self.states:
```

### Comparing `foxes-0.6.2/foxes/core/turbine.py` & `foxes-0.7/foxes/core/turbine.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/core/turbine_model.py` & `foxes-0.7/foxes/core/turbine_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,21 +24,21 @@
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        st_sel: numpy.ndarray of bool
+        st_sel: slice or numpy.ndarray of bool
             The state-turbine selection,
-            shape: (n_states, n_turbines)
+            for shape: (n_states, n_turbines)
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
```

### Comparing `foxes-0.6.2/foxes/core/turbine_type.py` & `foxes-0.7/foxes/core/turbine_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,14 +56,38 @@
         self.P_unit = P_unit
 
         if P_unit not in FC.P_UNITS:
             raise KeyError(
                 f"Turbine type '{self.name}': Unkown P_unit '{P_unit}', expecting {list(FC.P_UNITS.keys())}"
             )
 
+    def __repr__(self):
+        a = f"D={self.D}, H={self.H}, P_nominal={self.P_nominal}, P_unit={self.P_unit}"
+        return f"{type(self).__name__}({a})"
+
+    def modify_cutin(self, modify_ct, modify_P):
+        """
+        Modify the data such that a discontinuity
+        at cutin wind speed is avoided
+
+        Parameters
+        ----------
+        variable: str
+            The target variable
+        modify_ct: bool
+            Flag for modification of the ct curve
+        modify_P: bool
+            Flag for modification of the power curve
+
+        """
+        if modify_ct or modify_P:
+            raise NotImplementedError(
+                f"Turbine type '{self.name}': Continuous cutin not implemented for modify_ct = {modify_ct}, modify_P = {modify_P}"
+            )
+
     @classmethod
     def new(cls, ttype_type, *args, **kwargs):
         """
         Run-time turbine type factory.
 
         Parameters
         ----------
```

### Comparing `foxes-0.6.2/foxes/core/vertical_profile.py` & `foxes-0.7/foxes/core/vertical_profile.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,22 +23,22 @@
         vars: list of str
             The variable names
 
         """
         return []
 
     @abstractmethod
-    def calculate(self, data, heights):
+    def calculate(self, tdata, heights):
         """
         Run the profile calculation.
 
         Parameters
         ----------
-        data: dict
-            The input data
+        tdata: dict
+            The target point data
         heights: numpy.ndarray
             The evaluation heights
 
         Returns
         -------
         results: numpy.ndarray
             The profile results, same
```

### Comparing `foxes-0.6.2/foxes/core/wake_frame.py` & `foxes-0.7/foxes/models/wake_models/induction/rankine_half_body.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,300 +1,273 @@
-from abc import abstractmethod
 import numpy as np
-from scipy.interpolate import interpn
 
-from foxes.utils import all_subclasses
-import foxes.constants as FC
+from foxes.core import TurbineInductionModel
+from foxes.utils import uv2wd, wd2uv
 import foxes.variables as FV
-
-from .data import Data
-from .model import Model
+import foxes.constants as FC
 
 
-class WakeFrame(Model):
+class RankineHalfBody(TurbineInductionModel):
     """
-    Abstract base class for wake frames.
+    The Rankine half body induction wake model
 
-    Wake frames translate global coordinates into
-    wake frame coordinates, which are then evaluated
-    by wake models.
+    The individual wake effects are superposed linearly,
+    without invoking a wake superposition model.
 
-    They are also responsible for the calculation of
-    the turbine evaluation order.
+    Notes
+    -----
+    Reference:
+    B Gribben and G Hawkes
+    "A potential flow model for wind turbine induction and wind farm blockage"
+    Techincal Paper, Frazer-Nash Consultancy, 2019
+    https://www.fnc.co.uk/media/o5eosxas/a-potential-flow-model-for-wind-turbine-induction-and-wind-farm-blockage.pdf
+
+    Attributes
+    ----------
+    induction: foxes.core.AxialInductionModel or str
+        The induction model
 
-    :group: core
+    :group: models.wake_models.induction
 
     """
 
-    @abstractmethod
-    def calc_order(self, algo, mdata, fdata):
-        """ "
-        Calculates the order of turbine evaluation.
-
-        This function is executed on a single chunk of data,
-        all computations should be based on numpy arrays.
+    def __init__(self, induction="Madsen"):
+        """
+        Constructor.
 
         Parameters
         ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-
-        Returns
-        -------
-        order: numpy.ndarray
-            The turbine order, shape: (n_states, n_turbines)
+        induction: foxes.core.AxialInductionModel or str
+            The induction model
 
         """
-        pass
+        super().__init__()
+        self.induction = induction
 
-    @abstractmethod
-    def get_wake_coos(self, algo, mdata, fdata, pdata, states_source_turbine):
-        """
-        Calculate wake coordinates.
+    def __repr__(self):
+        iname = (
+            self.induction if isinstance(self.induction, str) else self.induction.name
+        )
+        return f"{type(self).__name__}(induction={iname})"
 
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+    def sub_models(self):
+        """
+        List of all sub-models
 
         Returns
         -------
-        wake_coos: numpy.ndarray
-            The wake frame coordinates of the evaluation
-            points, shape: (n_states, n_points, 3)
+        smdls: list of foxes.core.Model
+            All sub models
 
         """
-        pass
+        return [self.induction]
 
-    def get_wake_modelling_data(
-        self,
-        algo,
-        variable,
-        states_source_turbine,
-        fdata,
-        pdata,
-        states0=None,
-    ):
+    def initialize(self, algo, verbosity=0, force=False):
         """
-        Return data that is required for computing the
-        wake from source turbines to evaluation points.
+        Initializes the model.
 
         Parameters
         ----------
-        algo: foxes.core.Algorithm, optional
-            The algorithm, needed for data from previous iteration
-        variable: str
-            The variable, serves as data key
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        fdata: foxes.core.Data
-            The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states0: numpy.ndarray, optional
-            The states of wake creation
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        verbosity: int
+            The verbosity level, 0 = silent
+        force: bool
+            Overwrite existing data
 
         """
-        n_states = fdata.n_states
-        n_points = pdata.n_points
-        s = np.arange(n_states) if states0 is None else states0
-
-        out = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        out[:] = fdata[variable][s, states_source_turbine][:, None]
-
-        return out
+        if isinstance(self.induction, str):
+            self.induction = algo.mbook.axial_induction[self.induction]
+        super().initialize(algo, verbosity, force)
 
-    def get_centreline_points(self, algo, mdata, fdata, states_source_turbine, x):
+    def new_wake_deltas(self, algo, mdata, fdata, tdata):
         """
-        Gets the points along the centreline for given
-        values of x.
+        Creates new empty wake delta arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        x: numpy.ndarray
-            The wake frame x coordinates, shape: (n_states, n_points)
+        tdata: foxes.core.TData
+            The target point data
 
         Returns
         -------
-        points: numpy.ndarray
-            The centreline points, shape: (n_states, n_points, 3)
+        wake_deltas: dict
+            Key: variable name, value: The zero filled
+            wake deltas, shape: (n_states, n_turbines, n_rpoints, ...)
 
         """
-        raise NotImplementedError(
-            f"Wake frame '{self.name}': Centreline points requested but not implemented."
-        )
+        return {
+            FV.WS: np.zeros_like(tdata[FC.TARGETS][..., 0]),
+            FV.WD: np.zeros_like(tdata[FC.TARGETS][..., 0]),
+            "U": np.zeros_like(tdata[FC.TARGETS][..., 0]),
+            "V": np.zeros_like(tdata[FC.TARGETS][..., 0]),
+        }
 
-    def calc_centreline_integral(
+    def contribute(
         self,
         algo,
         mdata,
         fdata,
-        states_source_turbine,
-        variables,
-        x,
-        dx,
-        wake_models=None,
-        self_wake=True,
-        **ipars,
+        tdata,
+        downwind_index,
+        wake_coos,
+        wake_deltas,
     ):
         """
-        Integrates variables along the centreline.
+        Modifies wake deltas at target points by
+        contributions from the specified wake source turbines.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        variables: list of str
-            The variables to be integrated
-        x: numpy.ndarray
-            The wake frame x coordinates of the upper integral bounds,
-            shape: (n_states, n_points)
-        dx: float
-            The step size of the integral
-        wake_models: list of foxes.core.WakeModels
-            The wake models to consider, default: from algo
-        self_wake: bool
-            Flag for considering only wake from states_source_turbine
-        ipars: dict, optional
-            Additional interpolation parameters
-
-        Returns
-        -------
-        results: numpy.ndarray
-            The integration results, shape: (n_states, n_points, n_vars)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        wake_coos: numpy.ndarray
+            The wake frame coordinates of the evaluation
+            points, shape: (n_states, n_targets, n_tpoints, 3)
+        wake_deltas: dict
+            The wake deltas. Key: variable name,
+            value: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints, ...)
+
+        """
+        # get ct:
+        ct = self.get_data(
+            FV.CT,
+            FC.STATE_TARGET_TPOINT,
+            lookup="w",
+            algo=algo,
+            fdata=fdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
+            upcast=False,
+        )
 
-        """
-        # prepare:
-        n_states, n_points = x.shape
-        vrs = [FV.amb2var.get(v, v) for v in variables]
-        n_vars = len(vrs)
-
-        # calc evaluation points:
-        xmin = 0.0
-        xmax = np.nanmax(x)
-        n_steps = int((xmax - xmin) / dx)
-        if xmin + n_steps * dx < xmax:
-            n_steps += 1
-        n_ix = n_steps + 1
-        xs = np.arange(xmin, xmin + n_ix * dx, dx)
-        xpts = np.zeros((n_states, n_steps), dtype=FC.DTYPE)
-        xpts[:] = xs[None, 1:]
-        pts = self.get_centreline_points(
-            algo, mdata, fdata, states_source_turbine, xpts
+        # get ws:
+        ws = self.get_data(
+            FV.REWS,
+            FC.STATE_TARGET_TPOINT,
+            lookup="w",
+            algo=algo,
+            fdata=fdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
+            upcast=False,
         )
 
-        # run ambient calculation:
-        pdata = Data.from_points(
-            pts,
-            data={v: np.full((n_states, n_steps), np.nan, dtype=FC.DTYPE) for v in vrs},
-            dims={v: (FC.STATE, FC.POINT) for v in vrs},
+        # get D
+        D = self.get_data(
+            FV.D,
+            FC.STATE_TARGET_TPOINT,
+            lookup="w",
+            algo=algo,
+            fdata=fdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
+            upcast=True,
         )
-        res = algo.states.calculate(algo, mdata, fdata, pdata)
-        pdata.update(res)
-        amb2var = algo.get_model("SetAmbPointResults")()
-        amb2var.initialize(algo, verbosity=0)
-        res = amb2var.calculate(algo, mdata, fdata, pdata)
-        pdata.update(res)
-        del res, amb2var
-
-        # find out if all vars ambient:
-        ambient = True
-        for v in variables:
-            if v not in FV.amb2var:
-                ambient = False
-                break
-
-        # calc wakes:
-        if not ambient:
-            wcalc = algo.get_model("PointWakesCalculation")(wake_models=wake_models)
-            wcalc.initialize(algo, verbosity=0)
-            wsrc = states_source_turbine if self_wake else None
-            res = wcalc.calculate(algo, mdata, fdata, pdata, states_source_turbine=wsrc)
-            pdata.update(res)
-            del wcalc, res
-
-        # collect integration results:
-        iresults = np.zeros((n_states, n_ix, n_vars), dtype=FC.DTYPE)
-        for vi, v in enumerate(variables):
-            for i in range(n_steps):
-                iresults[:, i + 1, vi] = iresults[:, i, vi] + pdata[v][:, i] * dx
-
-        # interpolate to x of interest:
-        qts = np.zeros((n_states, n_points, 2), dtype=FC.DTYPE)
-        qts[:, :, 0] = np.arange(n_states)[:, None]
-        qts[:, :, 1] = x
-        qts = qts.reshape(n_states * n_points, 2)
-        results = interpn(
-            (np.arange(n_states), xs),
-            iresults,
-            qts,
-            bounds_error=False,
-            fill_value=0.0,
-            **ipars,
+
+        # calc m (page 7, skipping pi everywhere)
+        m = 2 * ws * self.induction.ct2a(ct) * (D / 2) ** 2
+
+        # get r and theta
+        x = np.round(wake_coos[..., 0], 12)
+        r = np.linalg.norm(wake_coos[..., 1:], axis=-1)
+        r_sph = np.sqrt(r**2 + x**2)
+        theta = np.arctan2(r, x)
+
+        # define rankine half body shape (page 3)
+        RHB_shape = (
+            np.cos(theta) - (2 / (m + 1e-15)) * ws * (r_sph * np.sin(theta)) ** 2
         )
 
-        return results.reshape(n_states, n_points, n_vars)
+        # stagnation point condition
+        xs = -np.sqrt(m / (4 * ws))
 
-    @classmethod
-    def new(cls, wframe_type, *args, **kwargs):
+        # set values out of body shape
+        st_sel = (ct > 0) & ((RHB_shape < -1) | (x < xs))
+        if np.any(st_sel):
+            # apply selection
+            xyz = wake_coos[st_sel]
+
+            # calc velocity components
+            vel_factor = m[st_sel] / (4 * np.linalg.norm(xyz, axis=-1) ** 3)
+            wake_deltas["U"][st_sel] += vel_factor * xyz[:, 0]
+            wake_deltas["V"][st_sel] += vel_factor * xyz[:, 1]
+
+        # set values inside body shape
+        st_sel = (ct > 0) & (RHB_shape >= -1) & (x >= xs) & (x <= 0)
+        if np.any(st_sel):
+            # apply selection
+            xyz = np.zeros_like(wake_coos[st_sel])
+            xyz[:, 0] = xs[st_sel]
+
+            # calc velocity components
+            vel_factor = m[st_sel] / (4 * np.linalg.norm(xyz, axis=-1) ** 3)
+            wake_deltas["U"][st_sel] += vel_factor * xyz[:, 0]
+
+    def finalize_wake_deltas(
+        self,
+        algo,
+        mdata,
+        fdata,
+        amb_results,
+        wake_deltas,
+    ):
         """
-        Run-time wake frame factory.
+        Finalize the wake calculation.
+
+        Modifies wake_deltas on the fly.
 
         Parameters
         ----------
-        wframe_type: str
-            The selected derived class name
-        args: tuple, optional
-            Additional parameters for constructor
-        kwargs: dict, optional
-            Additional parameters for constructor
-
-        """
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.MData
+            The model data
+        fdata: foxes.core.FData
+            The farm data
+        amb_results: dict
+            The ambient results, key: variable name str,
+            values: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints)
+        wake_deltas: dict
+            The wake deltas object at the selected target
+            turbines. Key: variable str, value: numpy.ndarray
+            with shape (n_states, n_targets, n_tpoints)
+
+        """
+        # calc ambient wind vector:
+        ws0 = amb_results[FV.WS]
+        nx = wd2uv(amb_results[FV.WD])
+        wind_vec = nx * ws0[:, :, :, None]
+
+        # wake deltas are in wake frame, rotate back to global frame:
+        ny = np.stack((-nx[..., 1], nx[..., 0]), axis=-1)
+        delta_uv = (
+            wake_deltas["U"][:, :, :, None] * nx + wake_deltas["V"][:, :, :, None] * ny
+        )
+        del ws0, nx, ny
 
-        if wframe_type is None:
-            return None
-
-        allc = all_subclasses(cls)
-        found = wframe_type in [scls.__name__ for scls in allc]
-
-        if found:
-            for scls in allc:
-                if scls.__name__ == wframe_type:
-                    return scls(*args, **kwargs)
-
-        else:
-            estr = (
-                "Wake frame type '{}' is not defined, available types are \n {}".format(
-                    wframe_type, sorted([i.__name__ for i in allc])
-                )
-            )
-            raise KeyError(estr)
+        # add ambient result to wake deltas:
+        wind_vec += delta_uv
+        del delta_uv
+
+        # deduce WS and WD deltas:
+        new_wd = uv2wd(wind_vec)
+        new_ws = np.linalg.norm(wind_vec, axis=-1)
+        wake_deltas[FV.WS] += new_ws - amb_results[FV.WS]
+        wake_deltas[FV.WD] += new_wd - amb_results[FV.WD]
```

### Comparing `foxes-0.6.2/foxes/core/wake_model.py` & `foxes-0.7/foxes/core/wake_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,131 @@
 from abc import abstractmethod
+import numpy as np
 
 from foxes.utils import all_subclasses
+import foxes.variables as FV
+import foxes.constants as FC
 
 from .model import Model
 
 
 class WakeModel(Model):
     """
     Abstract base class for wake models.
 
     :group: core
 
     """
 
-    @abstractmethod
-    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
+    @property
+    def affects_downwind(self):
+        """
+        Flag for downwind or upwind effects
+        on other turbines
+
+        Returns
+        -------
+        dwnd: bool
+            Flag for downwind effects by this model
+
         """
-        Initialize wake delta storage.
+        return True
 
-        They are added on the fly to the wake_deltas dict.
+    def new_wake_deltas(self, algo, mdata, fdata, tdata):
+        """
+        Creates new empty wake delta arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
+        tdata: foxes.core.TData
+            The target point data
+
+        Returns
+        -------
         wake_deltas: dict
-            The wake deltas storage, add wake deltas
-            on the fly. Keys: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
+            Key: variable name, value: The zero filled
+            wake deltas, shape: (n_states, n_turbines, n_rpoints, ...)
 
         """
-        pass
+        return {FV.WS: np.zeros_like(tdata[FC.TARGETS][..., 0])}
 
     @abstractmethod
-    def contribute_to_wake_deltas(
+    def contribute(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
+        tdata,
+        downwind_index,
         wake_coos,
         wake_deltas,
     ):
         """
-        Calculate the contribution to the wake deltas
-        by this wake model.
-
-        Modifies wake_deltas on the fly.
+        Modifies wake deltas at target points by
+        contributions from the specified wake source turbines.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
         wake_coos: numpy.ndarray
             The wake frame coordinates of the evaluation
-            points, shape: (n_states, n_points, 3)
+            points, shape: (n_states, n_targets, n_tpoints, 3)
         wake_deltas: dict
-            The wake deltas, are being modified ob the fly.
-            Key: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
+            The wake deltas. Key: variable name,
+            value: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints, ...)
 
         """
         pass
 
     def finalize_wake_deltas(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
         amb_results,
         wake_deltas,
     ):
         """
         Finalize the wake calculation.
 
         Modifies wake_deltas on the fly.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
         amb_results: dict
             The ambient results, key: variable name str,
-            values: numpy.ndarray with shape (n_states, n_points)
+            values: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints)
         wake_deltas: dict
-            The wake deltas, are being modified ob the fly.
-            Key: Variable name str, for which the wake delta
-            applies, values: numpy.ndarray with shape
-            (n_states, n_points, ...) before evaluation,
-            numpy.ndarray with shape (n_states, n_points) afterwards
+            The wake deltas object at the selected target
+            turbines. Key: variable str, value: numpy.ndarray
+            with shape (n_states, n_targets, n_tpoints)
 
         """
         pass
 
     @classmethod
     def new(cls, wmodel_type, *args, **kwargs):
         """
@@ -148,7 +156,30 @@
         else:
             estr = (
                 "Wake model type '{}' is not defined, available types are \n {}".format(
                     wmodel_type, sorted([i.__name__ for i in allc])
                 )
             )
             raise KeyError(estr)
+
+
+class TurbineInductionModel(WakeModel):
+    """
+    Abstract base class for turbine induction models.
+
+    :group: core
+
+    """
+
+    @property
+    def affects_downwind(self):
+        """
+        Flag for downwind or upwind effects
+        on other turbines
+
+        Returns
+        -------
+        dwnd: bool
+            Flag for downwind effects by this model
+
+        """
+        return False
```

### Comparing `foxes-0.6.2/foxes/core/wake_superposition.py` & `foxes-0.7/foxes/core/wake_superposition.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,93 +13,96 @@
     other means.
 
     :group: core
 
     """
 
     @abstractmethod
-    def calc_wakes_plus_wake(
+    def add_wake(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        sel_sp,
+        tdata,
+        downwind_index,
+        st_sel,
         variable,
         wake_delta,
         wake_model_result,
     ):
         """
-        Add a wake delta to previous wake deltas.
+        Add a wake delta to previous wake deltas,
+        at rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        sel_sp: numpy.ndarray of bool
-            The selection of points, shape: (n_states, n_points)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        st_sel: numpy.ndarray of bool
+            The selection of targets, shape: (n_states, n_targets)
         variable: str
             The variable name for which the wake deltas applies
         wake_delta: numpy.ndarray
-            The original wake deltas, shape: (n_states, n_points)
+            The original wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
         wake_model_result: numpy.ndarray
-            The new wake deltas of the selected points,
-            shape: (n_sel_sp,)
+            The new wake deltas of the selected rotors,
+            shape: (n_st_sel, n_tpoints, ...)
 
         Returns
         -------
         wdelta: numpy.ndarray
-            The updated wake deltas, shape: (n_states, n_points)
+            The updated wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
 
         """
         pass
 
     @abstractmethod
     def calc_final_wake_delta(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
         variable,
         amb_results,
         wake_delta,
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
         variable: str
             The variable name for which the wake deltas applies
         amb_results: numpy.ndarray
-            The ambient results, shape: (n_states, n_points)
+            The ambient results at targets,
+            shape: (n_states, n_targets, n_tpoints)
         wake_delta: numpy.ndarray
-            The wake deltas, shape: (n_states, n_points)
+            The wake deltas at targets, shape:
+            (n_states, n_targets, n_tpoints)
 
         Returns
         -------
         final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
-            results by simple plus operation. Shape: (n_states, n_points)
+            results by simple plus operation. Shape:
+            (n_states, n_targets, n_tpoints)
 
         """
         pass
```

### Comparing `foxes-0.6.2/foxes/core/wind_farm.py` & `foxes-0.7/foxes/core/wind_farm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/data/farms/test_farm_67.csv` & `foxes-0.7/foxes/data/farms/test_farm_67.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/data/parse.py` & `foxes-0.7/foxes/data/parse.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv` & `foxes-0.7/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/data/states/WRF-Timeseries-4464.csv.gz` & `foxes-0.7/foxes/data/states/WRF-Timeseries-4464.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/data/states/abl_states_6000.csv.gz` & `foxes-0.7/foxes/data/states/abl_states_6000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/data/states/timeseries_3000.csv.gz` & `foxes-0.7/foxes/data/states/timeseries_3000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/data/states/timeseries_8000.csv.gz` & `foxes-0.7/foxes/data/states/timeseries_8000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/data/states/wind_rose_bremen.csv` & `foxes-0.7/foxes/data/states/wind_rose_bremen.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/data/states/wind_rotation.nc` & `foxes-0.7/foxes/data/states/wind_rotation.nc`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/data/states/winds100.tab` & `foxes-0.7/foxes/data/states/winds100.tab`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/data/static_data.py` & `foxes-0.7/foxes/data/static_data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/input/farm_layout/from_csv.py` & `foxes-0.7/foxes/input/farm_layout/from_csv.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/input/farm_layout/from_df.py` & `foxes-0.7/foxes/input/farm_layout/from_df.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/input/farm_layout/from_file.py` & `foxes-0.7/foxes/input/farm_layout/from_file.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/input/farm_layout/from_json.py` & `foxes-0.7/foxes/input/farm_layout/from_json.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/input/farm_layout/from_random.py` & `foxes-0.7/foxes/input/farm_layout/from_random.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import numpy as np
 
 from foxes.utils import random_xy_square
 from foxes.core import Turbine
 
+
 def add_random(
-        farm, 
-        n_turbines, 
-        min_dist, 
-        centre=[0, 0], 
-        seed=None,
-        verbosity=1, 
-        **turbine_parameters,
-    ):
+    farm,
+    n_turbines,
+    min_dist,
+    centre=[0, 0],
+    seed=None,
+    verbosity=1,
+    **turbine_parameters,
+):
     """
     Add turbines that lie randomly within a square
-    
+
     Parameters
     ----------
     farm: foxes.WindFarm
         The wind farm
     n_turbines: int
         The number of turbines
     min_dist: float
```

### Comparing `foxes-0.6.2/foxes/input/farm_layout/grid.py` & `foxes-0.7/foxes/input/farm_layout/grid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/input/farm_layout/row.py` & `foxes-0.7/foxes/input/farm_layout/row.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/input/states/create/random_abl_states.py` & `foxes-0.7/foxes/input/states/create/random_abl_states.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/input/states/create/random_timeseries.py` & `foxes-0.7/foxes/input/states/create/random_timeseries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import numpy as np
 import pandas as pd
 
 import foxes.variables as FV
 
+
 def random_timseries_data(
-        n_times, 
-        data_ranges=None,
-        start_time="2000-01-01 00:00:00",
-        freq='h',
-        seed=None,
-        iname="Time",
-    ):
-    """ 
+    n_times,
+    data_ranges=None,
+    start_time="2000-01-01 00:00:00",
+    freq="h",
+    seed=None,
+    iname="Time",
+):
+    """
     Creates random uniform timeseries data
 
     Parameters
     ----------
     n_times: int
         The number of time steps
     data_ranges: dict, optional
@@ -25,34 +26,31 @@
         The first time stamp in the series
     freq: str
         The time period range frequency
     seed: int, optional
         The random seed
     iname: str
         The index name
-    
+
     Returns
     -------
     sdata: pandas.DataFrame
         The timeseries data
-    
+
     :group: input.states.create
 
     """
     if seed:
         np.random.seed(seed)
-    
-    dranges = {
-        FV.WS: (0., 30.),
-        FV.WD: (0., 360.)
-    }
+
+    dranges = {FV.WS: (0.0, 30.0), FV.WD: (0.0, 360.0)}
     if data_ranges:
         dranges.update(data_ranges)
 
     times = pd.period_range(start=start_time, periods=n_times, freq=freq)
     times = times.astype(str).astype("datetime64[ns]")
-    sdata = pd.DataFrame(index=times, data={
-        v: np.random.uniform(d[0], d[1], n_times)
-        for v, d in dranges.items()
-    })
+    sdata = pd.DataFrame(
+        index=times,
+        data={v: np.random.uniform(d[0], d[1], n_times) for v, d in dranges.items()},
+    )
     sdata.index.name = iname
     return sdata
```

### Comparing `foxes-0.6.2/foxes/input/states/field_data_nc.py` & `foxes-0.7/foxes/input/states/field_data_nc.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,41 +417,45 @@
         -------
         weights: numpy.ndarray
             The weights, shape: (n_states, n_turbines)
 
         """
         return self._weights
 
-    def calculate(self, algo, mdata, fdata, pdata):
+    def calculate(self, algo, mdata, fdata, tdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The point data
+        tdata: foxes.core.TData
+            The target point data
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_points)
+            Values: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints)
 
         """
         # prepare:
-        points = pdata[FC.POINTS]
+        n_states = tdata.n_states
+        n_targets = tdata.n_targets
+        n_tpoints = tdata.n_tpoints
+        points = tdata[FC.TARGETS].reshape(n_states, n_targets * n_tpoints, 3)
         n_pts = points.shape[1]
         n_states = fdata.n_states
 
         # pick pre-loaded data:
         if self.pre_load:
             x = mdata[self.X]
             y = mdata[self.Y]
@@ -567,8 +571,8 @@
                 if v in self._dkys:
                     out[v] = data[..., self._dkys[v]]
                 else:
                     out[v] = np.full(
                         (n_states, n_pts), self.fixed_vars[v], dtype=FC.DTYPE
                     )
 
-        return out
+        return {v: d.reshape(n_states, n_targets, n_tpoints) for v, d in out.items()}
```

### Comparing `foxes-0.6.2/foxes/input/states/multi_height.py` & `foxes-0.7/foxes/input/states/multi_height.py`

 * *Files 9% similar despite different names*

```diff
@@ -188,21 +188,21 @@
             elif verbosity:
                 print(f"States '{self.name}': Reading file {self.data_source}")
             rpars = dict(self.RDICT, **self.rpars)
             data = PandasFileHelper().read_file(self.data_source, **rpars)
             isorg = False
         else:
             isorg = True
+            data = self.data_source
 
         if self.states_sel is not None:
             data = data.iloc[self.states_sel]
         elif self.states_loc is not None:
             data = data.loc[self.states_loc]
-        else:
-            data = data
+
         self._N = len(data.index)
         self._inds = data.index.to_numpy()
 
         col_w = self.var2col.get(FV.WEIGHT, FV.WEIGHT)
         self._weights = np.zeros((self._N, algo.n_turbines), dtype=FC.DTYPE)
         if col_w in data:
             self._weights[:] = data[col_w].to_numpy()[:, None]
@@ -304,43 +304,48 @@
         -------
         weights: numpy.ndarray
             The weights, shape: (n_states, n_turbines)
 
         """
         return self._weights
 
-    def calculate(self, algo, mdata, fdata, pdata):
+    def calculate(self, algo, mdata, fdata, tdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The point data
+        tdata: foxes.core.TData
+            The target point data
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_points)
+            Values: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints)
 
         """
+        n_states = tdata.n_states
+        n_targets = tdata.n_targets
+        n_tpoints = tdata.n_tpoints
         h = mdata[self.H]
-        z = pdata[FC.POINTS][:, :, 2]
+        z = tdata[FC.TARGETS][..., 2].reshape(n_states, n_targets * n_tpoints)
         n_h = len(h)
         vrs = list(mdata[self.VARS])
+        n_vars = len(vrs)
 
         coeffs = np.zeros((n_h, n_h), dtype=FC.DTYPE)
         np.fill_diagonal(coeffs, 1.0)
         ipars = dict(assume_sorted=True, bounds_error=True)
         ipars.update(self.ipars)
         intp = interp1d(h, coeffs, axis=0, **ipars)
         ires = intp(z)
@@ -360,32 +365,37 @@
                 uvh = wd2uv(
                     mdata[self.DATA][:, i_wd], mdata[self.var(FV.WS)][:, None], axis=-1
                 )
             else:
                 raise KeyError(
                     f"States '{self.name}': Found variable '{FV.WD}', but missing variable '{FV.WS}'"
                 )
-            uv = np.einsum("shd,sph->spd", uvh, ires)
+            uv = np.einsum("shd,sph->spd", uvh, ires).reshape(
+                n_states, n_targets, n_tpoints, 2
+            )
             del uvh
 
-        ires = np.einsum("svh,sph->svp", mdata[self.DATA], ires)
+        ires = np.einsum("svh,sph->vsp", mdata[self.DATA], ires).reshape(
+            n_vars, n_states, n_targets, n_tpoints
+        )
 
         results = {}
         for v in self.ovars:
-            results[v] = pdata[v]
             if has_wd and v == FV.WD:
                 results[v] = uv2wd(uv, axis=-1)
             elif has_wd and v == FV.WS:
                 results[v] = np.linalg.norm(uv, axis=-1)
             elif v in self.fixed_vars:
+                results[v] = np.zeros((n_states, n_targets, n_tpoints), dtype=FC.DTYPE)
                 results[v][:] = self.fixed_vars[v]
             elif v in self._solo.keys():
-                results[v][:] = mdata[self.var(v)][:, None]
+                results[v] = np.zeros((n_states, n_targets, n_tpoints), dtype=FC.DTYPE)
+                results[v][:] = mdata[self.var(v)][:, None, None]
             else:
-                results[v] = ires[:, vrs.index(v)]
+                results[v] = ires[vrs.index(v)]
 
         return results
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
```

### Comparing `foxes-0.6.2/foxes/input/states/scan_ws.py` & `foxes-0.7/foxes/models/wake_superpositions/ws_product.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,172 +1,173 @@
 import numpy as np
 
-from foxes.core import States
+from foxes.core import WakeSuperposition
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class ScanWS(States):
+class WSProduct(WakeSuperposition):
     """
-    A given list of wind speeds, all other variables are fixed.
+    Product supersposition of wind deficit results
 
-    Parameters
+    This is based on the idea that the dimensionless
+    wind deficit should be rescaled with the wake
+    corrected wind field, rather than the rotor
+    equivalent wind speed.
+
+    Source: https://arxiv.org/pdf/2010.03873.pdf
+            Equation (8)
+
+    Attributes
     ----------
-    wd: float
-        The wind direction
-    ti: float
-        The TI value
-    rho: float
-        The air density
+    lim_low: float
+        Lower limit of the final waked wind speed
+    lim_high: float
+        Upper limit of the final waked wind speed
 
-    :group: input.states
+    :group: models.wake_superpositions
 
     """
 
-    def __init__(self, ws_list, wd, ti=None, rho=None):
+    def __init__(self, lim_low=None, lim_high=None):
         """
         Constructor.
 
         Parameters
         ----------
-        ws_list: array_like
-            The wind speed values
-        wd: float
-            The wind direction
-        ti: float, optional
-            The TI value
-        rho: float, optional
-            The air density
+        lim_low: float
+            Lower limit of the final waked wind speed
+        lim_high: float
+            Upper limit of the final waked wind speed
 
         """
         super().__init__()
 
-        self._wsl = np.array(ws_list)
-        self.N = len(ws_list)
-        self.wd = wd
-        self.ti = ti
-        self.rho = rho
-
-    def load_data(self, algo, verbosity=0):
-        """
-        Load and/or create all model data that is subject to chunking.
-
-        Such data should not be stored under self, for memory reasons. The
-        data returned here will automatically be chunked and then provided
-        as part of the mdata object during calculations.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
-
-        Returns
-        -------
-        idata: dict
-            The dict has exactly two entries: `data_vars`,
-            a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
-            and `coords`, a dict with entries `dim_name_str -> dim_array`
-
-        """
-        self.WS = self.var(FV.WS)
-
-        idata = super().load_data(algo, verbosity)
-        idata["data_vars"][self.WS] = ((FC.STATE,), self._wsl)
-
-        return idata
-
-    def size(self):
-        """
-        The total number of states.
-
-        Returns
-        -------
-        int:
-            The total number of states
+        self.lim_low = lim_low
+        self.lim_high = lim_high
 
-        """
-        return self.N
+    def __repr__(self):
+        a = f"lim_low={self.lim_low}, lim_high={self.lim_high}"
+        return f"{type(self).__name__}({a})"
 
-    def output_point_vars(self, algo):
+    def input_farm_vars(self, algo):
         """
-        The variables which are being modified by the model.
+        The variables which are needed for running
+        the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars: list of str
-            The output variable names
+        input_vars: list of str
+            The input variable names
 
         """
-        pvars = [FV.WS]
-        if self.wd is not None:
-            pvars.append(FV.WD)
-        if self.ti is not None:
-            pvars.append(FV.TI)
-        if self.rho is not None:
-            pvars.append(FV.RHO)
-        return pvars
+        return [FV.AMB_REWS] if self.scale_amb else [FV.REWS]
 
-    def weights(self, algo):
+    def add_wake(
+        self,
+        algo,
+        mdata,
+        fdata,
+        tdata,
+        downwind_index,
+        st_sel,
+        variable,
+        wake_delta,
+        wake_model_result,
+    ):
         """
-        The statistical weights of all states.
+        Add a wake delta to previous wake deltas,
+        at rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
+        mdata: foxes.core.MData
+            The model data
+        fdata: foxes.core.FData
+            The farm data
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        st_sel: numpy.ndarray of bool
+            The selection of targets, shape: (n_states, n_targets)
+        variable: str
+            The variable name for which the wake deltas applies
+        wake_delta: numpy.ndarray
+            The original wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
+        wake_model_result: numpy.ndarray
+            The new wake deltas of the selected rotors,
+            shape: (n_st_sel, n_tpoints, ...)
 
         Returns
         -------
-        weights: numpy.ndarray
-            The weights, shape: (n_states, n_turbines)
+        wdelta: numpy.ndarray
+            The updated wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
 
         """
-        return np.full((self.N, algo.n_turbines), 1.0 / self.N, dtype=FC.DTYPE)
-
-    def calculate(self, algo, mdata, fdata, pdata):
-        """ "
-        The main model calculation.
+        if variable not in [FV.REWS, FV.REWS2, FV.REWS3, FV.WS]:
+            raise ValueError(
+                f"Superposition '{self.name}': Expecting wind speed variable, got {variable}"
+            )
 
-        This function is executed on a single chunk of data,
-        all computations should be based on numpy arrays.
+        if np.any(st_sel):
+            if np.max(np.abs(wake_delta)) < 1e-14:
+                wake_delta[:] = 1
+
+            wake_delta[st_sel] *= 1 + wake_model_result
+
+        return wake_delta
+
+    def calc_final_wake_delta(
+        self,
+        algo,
+        mdata,
+        fdata,
+        variable,
+        amb_results,
+        wake_delta,
+    ):
+        """
+        Calculate the final wake delta after adding all
+        contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The point data
+        variable: str
+            The variable name for which the wake deltas applies
+        amb_results: numpy.ndarray
+            The ambient results at targets,
+            shape: (n_states, n_targets, n_tpoints)
+        wake_delta: numpy.ndarray
+            The wake deltas at targets, shape:
+            (n_states, n_targets, n_tpoints)
 
         Returns
         -------
-        results: dict
-            The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_points)
+        final_wake_delta: numpy.ndarray
+            The final wake delta, which will be added to the ambient
+            results by simple plus operation. Shape:
+            (n_states, n_targets, n_tpoints)
 
         """
-        pdata[FV.WS][:] = mdata[self.WS][:, None]
-
-        if self.wd is not None:
-            pdata[FV.WD] = np.full(
-                (pdata.n_states, pdata.n_points), self.wd, dtype=FC.DTYPE
-            )
-        if self.ti is not None:
-            pdata[FV.TI] = np.full(
-                (pdata.n_states, pdata.n_points), self.ti, dtype=FC.DTYPE
-            )
-        if self.rho is not None:
-            pdata[FV.RHO] = np.full(
-                (pdata.n_states, pdata.n_points), self.rho, dtype=FC.DTYPE
-            )
-
-        return {v: pdata[v] for v in self.output_point_vars(algo)}
+        w = amb_results * (wake_delta - 1)
+        if self.lim_low is not None:
+            w = np.maximum(w, self.lim_low - amb_results)
+        if self.lim_high is not None:
+            w = np.minimum(w, self.lim_high - amb_results)
+        return w
```

### Comparing `foxes-0.6.2/foxes/input/states/single.py` & `foxes-0.7/foxes/models/turbine_models/power_mask.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,219 +1,202 @@
 import numpy as np
 
-from foxes.core import States, VerticalProfile
+from foxes.core import TurbineModel
 import foxes.variables as FV
 import foxes.constants as FC
+from foxes.utils import cubic_roots
 
 
-class SingleStateStates(States):
+class PowerMask(TurbineModel):
     """
-    A single uniform state.
+    Invokes a maximal power value.
+
+    This may correspond to turbine derating, if
+    the maximal power value is below rated power.
+    For higher values, a boost is introduced.
+
+    The model updates the P and CT variables,
+    so it is wise to use it after calling the
+    turbine type model.
 
     Attributes
     ----------
-    ws: float
-        The wind speed
-    wd: float
-        The wind direction
-    ti: float
-        The TI value
-    rho: float
-        The air density
-    profdicts: dict
-        Key: output variable name str, Value: str or dict
-        or `foxes.core.VerticalProfile`
-    profdata: dict,
-        Additional data for profiles
+    var_ws_P: str
+        The wind speed variable for power lookup
+    factor_P: float
+        The power unit factor, e.g. 1000 for kW
+    P_lim: float
+        Threshold power delta for boosts
+    induction: foxes.core.AxialInductionModel
+        The induction model
 
-    :group: input.states
+    :group: models.turbine_models
 
     """
 
-    def __init__(self, ws=None, wd=None, ti=None, rho=None, profiles={}, **profdata):
+    def __init__(self, var_ws_P=FV.REWS3, factor_P=1.0e3, P_lim=100, induction="Betz"):
         """
         Constructor.
 
         Parameters
         ----------
-        ws: float, optional
-            The wind speed
-        wd: float, optional
-            The wind direction
-        ti: float, optional
-            The TI value
-        rho: float, optional
-            The air density
-        profiles: dict, optional
-            Key: output variable name str, Value: str or dict
-            or `foxes.core.VerticalProfile`
-        profdata: dict, optional
-            Additional data for profiles
+        var_ws_P: str
+            The wind speed variable for power lookup
+        factor_P: float
+            The power unit factor, e.g. 1000 for kW
+        P_lim: float
+            Threshold power delta for boosts
+        induction: foxes.core.AxialInductionModel or str
+            The induction model
 
         """
         super().__init__()
-        self.ws = ws
-        self.wd = wd
-        self.ti = ti
-        self.rho = rho
-        self.profdicts = profiles
-        self.profdata = profdata
-
-        if (
-            ws is None
-            and wd is None
-            and ti is None
-            and rho is None
-            and not len(profiles)
-        ):
-            raise KeyError(
-                f"Expecting at least one parameter: ws, wd, ti, rho, profiles"
-            )
 
-    def sub_models(self):
-        """
-        List of all sub-models
+        self.var_ws_P = var_ws_P
+        self.factor_P = factor_P
+        self.P_lim = P_lim
+        self.induction = induction
+
+    def __repr__(self):
+        iname = (
+            self.induction if isinstance(self.induction, str) else self.induction.name
+        )
+        a = f"var_ws_P={self.var_ws_P}, P_lim={self.P_lim}, induction={iname}"
+        return f"{type(self).__name__}({a})"
 
-        Returns
-        -------
-        smdls: list of foxes.core.Model
-            Names of all sub models
-
-        """
-        return list(self._profiles.values())
-
-    def initialize(self, algo, verbosity=0):
+    def output_farm_vars(self, algo):
         """
-        Initializes the model.
+        The variables which are being modified by the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
-
-        """
-        self._profiles = {}
-        for v, d in self.profdicts.items():
-            if isinstance(d, str):
-                self._profiles[v] = VerticalProfile.new(d)
-            elif isinstance(d, VerticalProfile):
-                self._profiles[v] = d
-            elif isinstance(d, dict):
-                t = d.pop("type")
-                self._profiles[v] = VerticalProfile.new(t, **d)
-            else:
-                raise TypeError(
-                    f"States '{self.name}': Wrong profile type '{type(d).__name__}' for variable '{v}'. Expecting VerticalProfile, str or dict"
-                )
-        super().initialize(algo, verbosity)
-
-    def size(self):
-        """
-        The total number of states.
 
         Returns
         -------
-        int:
-            The total number of states
+        output_vars: list of str
+            The output variable names
 
         """
-        return 1
+        return [FV.P, FV.CT]
 
-    def output_point_vars(self, algo):
+    def sub_models(self):
         """
-        The variables which are being modified by the model.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
+        List of all sub-models
 
         Returns
         -------
-        output_vars: list of str
-            The output variable names
+        smdls: list of foxes.core.Model
+            All sub models
 
         """
-        out = set()
-        if self.ws is not None:
-            out.add(FV.WS)
-        if self.wd is not None:
-            out.add(FV.WD)
-        if self.ti is not None:
-            out.add(FV.TI)
-        if self.rho is not None:
-            out.add(FV.RHO)
-        out.update(list(self._profiles.keys()))
-
-        return list(out)
+        return [self.induction]
 
-    def weights(self, algo):
+    def initialize(self, algo, verbosity=0):
         """
-        The statistical weights of all states.
+        Initializes the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-
-        Returns
-        -------
-        weights: numpy.ndarray
-            The weights, shape: (n_states, n_turbines)
+        verbosity: int
+            The verbosity level, 0 = silent
 
         """
-        return np.ones((1, algo.n_turbines), dtype=FC.DTYPE)
+        if isinstance(self.induction, str):
+            self.induction = algo.mbook.axial_induction[self.induction]
+        super().initialize(algo, verbosity)
+
+        self._P_rated = []
+        for t in algo.farm_controller.turbine_types:
+            Pnom = FC.DTYPE(t.P_nominal)
+            if np.isnan(Pnom):
+                raise ValueError(
+                    f"Model '{self.name}': P_nominal is NaN for turbine type '{t.name}'"
+                )
+            self._P_rated.append(Pnom)
+        self._P_rated = np.array(self._P_rated, dtype=FC.DTYPE)
 
-    def calculate(self, algo, mdata, fdata, pdata):
-        """ "
+    def calculate(self, algo, mdata, fdata, st_sel):
+        """
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The point data
+        st_sel: slice or numpy.ndarray of bool
+            The state-turbine selection,
+            for shape: (n_states, n_turbines)
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_points)
+            Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
-
-        if self.ws is not None:
-            pdata[FV.WS] = np.full(
-                (pdata.n_states, pdata.n_points), self.ws, dtype=FC.DTYPE
-            )
-        if self.wd is not None:
-            pdata[FV.WD] = np.full(
-                (pdata.n_states, pdata.n_points), self.wd, dtype=FC.DTYPE
+        # prepare:
+        P = fdata[FV.P]
+        max_P = fdata[FV.MAX_P]
+        P_rated = self._P_rated[None, :]
+
+        # select power entries for which this is active:
+        sel = np.zeros((fdata.n_states, fdata.n_turbines), dtype=bool)
+        sel[st_sel] = True
+        sel = (
+            sel
+            & ~np.isnan(max_P)
+            & (
+                ((max_P < P_rated) & (P > max_P))
+                | ((max_P > P_rated) & (P > P_rated - self.P_lim))
             )
-        if self.ti is not None:
-            pdata[FV.TI] = np.full(
-                (pdata.n_states, pdata.n_points), self.ti, dtype=FC.DTYPE
-            )
-        if self.rho is not None:
-            pdata[FV.RHO] = np.full(
-                (pdata.n_states, pdata.n_points), self.rho, dtype=FC.DTYPE
-            )
-
-        if len(self._profiles):
-            z = pdata[FC.POINTS][:, :, 2]
-            for k, v in self.profdata.items():
-                pdata[k] = v
-            for v, p in self._profiles.items():
-                pres = p.calculate(pdata, z)
-                pdata[v] = pres
+        )
+        if np.any(sel):
+            # apply selection:
+            max_P = max_P[sel]
+            ws = fdata[self.var_ws_P][sel]
+            rho = fdata[FV.RHO][sel]
+            r = fdata[FV.D][sel] / 2
+            P = P[sel]
+            ct = fdata[FV.CT][sel]
+
+            # calculate power efficiency e of turbine
+            # e is the ratio of the cp derived from the power curve
+            # and the theoretical cp from the turbine induction
+            cp = P / (0.5 * ws**3 * rho * np.pi * r**2) * self.factor_P
+            a = self.induction.ct2a(ct)
+            cp_a = 4 * a**3 - 8 * a**2 + 4 * a
+            e = cp / cp_a
+            del cp, a, cp_a, ct, P
+
+            # calculating new cp for changed power
+            cp = max_P / (0.5 * ws**3 * rho * np.pi * r**2) * self.factor_P
+
+            # find roots:
+            N = len(cp)
+            a3 = np.full(N, 4.0, dtype=FC.DTYPE)
+            a2 = np.full(N, -8.0, dtype=FC.DTYPE)
+            a1 = np.full(N, 4.0, dtype=FC.DTYPE)
+            a0 = -cp / e
+            rts = cubic_roots(a0, a1, a2, a3)
+            rts[np.isnan(rts)] = np.inf
+            rts[rts <= 0.0] = np.inf
+            a = np.min(rts, axis=1)
+            del a0, a1, a2, a3, rts
+
+            # set results:
+            P = fdata[FV.P]
+            ct = fdata[FV.CT]
+            P[sel] = max_P
+            ct[sel] = 4 * a * (1 - a)
 
-        return {v: pdata[v] for v in self.output_point_vars(algo)}
+        return {FV.P: fdata[FV.P], FV.CT: fdata[FV.CT]}
```

### Comparing `foxes-0.6.2/foxes/input/states/states_table.py` & `foxes-0.7/foxes/input/states/states_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -305,56 +305,60 @@
         -------
         weights: numpy.ndarray
             The weights, shape: (n_states, n_turbines)
 
         """
         return self._weights
 
-    def calculate(self, algo, mdata, fdata, pdata):
+    def calculate(self, algo, mdata, fdata, tdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The point data
+        tdata: foxes.core.TData
+            The target point data
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_points)
+            Values: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints)
 
         """
-        z = pdata[FC.POINTS][:, :, 2]
-
         for i, v in enumerate(self._tvars):
-            if v in pdata:
-                pdata[v][:] = mdata[self.DATA][:, i, None]
+            if v in tdata:
+                tdata[v][:] = mdata[self.DATA][:, i, None, None]
             else:
-                pdata[v] = mdata[self.DATA][:, i, None]
-                pdata.dims[v] = (FC.STATE, FC.POINT)
+                tdata[v] = np.zeros(
+                    (tdata.n_states, tdata.n_targets, tdata.n_tpoints), dtype=FC.DTYPE
+                )
+                tdata[v][:] = mdata[self.DATA][:, i, None, None]
+                tdata.dims[v] = (FC.STATE, FC.TARGET, FC.TPOINT)
 
         for v, f in self.fixed_vars.items():
-            pdata[v] = np.full((pdata.n_states, pdata.n_points), f, dtype=FC.DTYPE)
+            tdata[v] = np.full(
+                (tdata.n_states, tdata.n_targets, tdata.n_tpoints), f, dtype=FC.DTYPE
+            )
 
+        z = tdata[FC.TARGETS][..., 2]
         for v, p in self._profiles.items():
-            pres = p.calculate(pdata, z)
-            pdata[v] = pres
+            tdata[v] = p.calculate(tdata, z)
 
-        return {v: pdata[v] for v in self.output_point_vars(algo)}
+        return {v: tdata[v] for v in self.output_point_vars(algo)}
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
@@ -468,16 +472,16 @@
 
             wd0 = self._tab_data["wd"].to_numpy()
             ws0 = a * np.append(
                 np.array([0], dtype=FC.DTYPE), self._tab_data["ws"].to_numpy()
             )
             ws0 = 0.5 * (ws0[:-1] + ws0[1:])
 
-            n_ws = self._tab_data.dims["ws"]
-            n_wd = self._tab_data.dims["wd"]
+            n_ws = self._tab_data.sizes["ws"]
+            n_wd = self._tab_data.sizes["wd"]
             ws = np.zeros((n_ws, n_wd), dtype=FC.DTYPE)
             wd = np.zeros((n_ws, n_wd), dtype=FC.DTYPE)
             ws[:] = ws0[:, None]
             wd[:] = wd0[None, :]
 
             wd_freq = self._tab_data["wd_freq"].to_numpy() / 100
             weights = self._tab_data["ws_freq"].to_numpy() * wd_freq[None, :] / 1000
```

### Comparing `foxes-0.6.2/foxes/input/windio/windio.py` & `foxes-0.7/foxes/input/windio/windio.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/models/axial_induction_models/betz.py` & `foxes-0.7/foxes/models/axial_induction_models/betz.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     ct_max: float
         The maximal ct value
 
     :group: models.axial_induction
 
     """
 
-    def __init__(self, ct_max=1):
+    def __init__(self, ct_max=0.99999):
         """
         Constructor.
 
         Parameters
         ----------
         ct_max: float
             The maximal ct value
```

### Comparing `foxes-0.6.2/foxes/models/axial_induction_models/madsen.py` & `foxes-0.7/foxes/models/axial_induction_models/madsen.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/models/farm_models/turbine2farm.py` & `foxes-0.7/foxes/models/farm_models/turbine2farm.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,17 +71,17 @@
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
         **parameters: dict, optional
             Init parameters forwarded to the turbine model
 
         Returns
         -------
         results: dict
```

### Comparing `foxes-0.6.2/foxes/models/model_book.py` & `foxes-0.7/foxes/models/model_book.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     TurbineType,
     TurbineModel,
     PartialWakesModel,
     WakeFrame,
     WakeSuperposition,
     WakeModel,
     AxialInductionModel,
+    TurbineInductionModel,
 )
 
 
 class ModelBook:
     """
     Container for all kinds of models.
 
@@ -89,24 +90,24 @@
             self.rotor_models[f"level{n}"] = fm.rotor_models.LevelRotor(
                 calc_vars=rvars, n=n, reduce=True
             )
 
         self.turbine_types = Dict(name="turbine_types")
         self.turbine_types["null_type"] = fm.turbine_types.NullType()
         self.turbine_types["NREL5MW"] = fm.turbine_types.PCtFile(
-            "NREL-5MW-D126-H90.csv"
+            "NREL-5MW-D126-H90.csv", rho=1.225
         )
         self.turbine_types["DTU10MW"] = fm.turbine_types.PCtFile(
-            "DTU-10MW-D178d3-H119.csv"
+            "DTU-10MW-D178d3-H119.csv", rho=1.225
         )
         self.turbine_types["IEA15MW"] = fm.turbine_types.PCtFile(
-            "IEA-15MW-D240-H150.csv"
+            "IEA-15MW-D240-H150.csv", rho=1.225
         )
         self.turbine_types["IWT7.5MW"] = fm.turbine_types.PCtFile(
-            "IWT-7d5MW-D164-H100.csv"
+            "IWT-7d5MW-D164-H100.csv", rho=1.225
         )
         if Pct_file is not None:
             self.turbine_types["Pct"] = fm.turbine_types.PCtFile(Pct_file)
 
         self.turbine_models = Dict(
             name="turbine_models",
             kTI=fm.turbine_models.kTI(),
@@ -144,33 +145,29 @@
             basic_ctrl=fm.farm_controllers.BasicFarmController(),
         )
 
         self.partial_wakes = Dict(
             name="partial_wakes",
             rotor_points=fm.partial_wakes.RotorPoints(),
             top_hat=fm.partial_wakes.PartialTopHat(),
-            distsliced=fm.partial_wakes.PartialDistSlicedWake(),
             centre=fm.partial_wakes.PartialCentre(),
-            auto=fm.partial_wakes.Mapped(),
         )
         nlst = list(range(2, 11)) + [20]
         for n in nlst:
             self.partial_wakes[f"axiwake{n}"] = fm.partial_wakes.PartialAxiwake(n)
         for n in nlist:
-            self.partial_wakes[f"distsliced{n**2}"] = (
-                fm.partial_wakes.PartialDistSlicedWake(n)
-            )
-        for n in nlist:
-            self.partial_wakes[f"grid{n**2}"] = fm.partial_wakes.PartialGrid(n)
+            self.partial_wakes[f"grid{n**2}"] = fm.partial_wakes.PartialGrid(n=n)
 
         self.wake_frames = Dict(
             name="wake_frames",
             rotor_wd=fm.wake_frames.RotorWD(var_wd=FV.WD),
             rotor_wd_farmo=fm.wake_frames.FarmOrder(),
             yawed=fm.wake_frames.YawedWakes(),
+            yawed_k002=fm.wake_frames.YawedWakes(k=0.02),
+            yawed_k004=fm.wake_frames.YawedWakes(k=0.04),
         )
         stps = [1.0, 5.0, 10.0, 50.0, 100.0, 500.0]
         for s in stps:
             self.wake_frames[f"streamlines_{int(s)}"] = fm.wake_frames.Streamlines2D(
                 step=s
             )
         for s in stps:
@@ -243,15 +240,15 @@
         self.wake_models = Dict(name="wake_models")
         slist = [
             "linear",
             "linear_lim",
             "linear_amb",
             "linear_amb_lim",
             "quadratic",
-            "wquadratic_lim",
+            "quadratic_lim",
             "quadratic_amb",
             "quadratic_amb_lim",
             "cubic",
             "cubic_amb",
             "quartic",
             "quartic_amb",
             "wmax",
@@ -413,21 +410,20 @@
             )
 
             self.wake_models[f"IECTI2019_{s}"] = fm.wake_models.ti.IECTIWake(
                 superposition=f"ti_{s}", iec_type="2019"
             )
 
         self.wake_models[f"RHB"] = fm.wake_models.induction.RankineHalfBody()
+        self.wake_models[f"Rathmann"] = fm.wake_models.induction.Rathmann()
         self.wake_models[f"SelfSimilar"] = fm.wake_models.induction.SelfSimilar()
         self.wake_models[f"SelfSimilar2020"] = (
             fm.wake_models.induction.SelfSimilar2020()
         )
 
-        self.wake_models[f"Rathmann"] = fm.wake_models.induction.Rathmann()
-
         self.sources = Dict(
             name="sources",
             point_models=self.point_models,
             rotor_models=self.rotor_models,
             turbine_types=self.turbine_types,
             turbine_models=self.turbine_models,
             farm_models=self.farm_models,
@@ -515,14 +511,43 @@
                 raise KeyError(
                     f"Model '{name}' of type '{model_type}' not found in model book. Available: {sorted(list(self.sources[model_type].keys()))}"
                 )
             bclass = self.base_classes[model_type]
             self.sources[model_type][name] = bclass.new(class_name, *args, **kwargs)
         return self.sources[model_type][name]
 
+    def default_partial_wakes(self, wake_model):
+        """
+        Gets a default partial wakes model name
+        for a given wake model
+
+        Parameters
+        ----------
+        wake_model: foxes.core.WakeModel
+            The wake model
+
+        Returns
+        -------
+        pwake: str
+            The partial wake model name
+
+        """
+        if isinstance(wake_model, TurbineInductionModel):
+            return "grid9"
+        elif isinstance(wake_model, fm.wake_models.TopHatWakeModel):
+            return "top_hat"
+        elif isinstance(wake_model, fm.wake_models.AxisymmetricWakeModel):
+            return "axiwake6"
+        elif isinstance(wake_model, fm.wake_models.DistSlicedWakeModel):
+            return "grid9"
+        else:
+            raise TypeError(
+                f"No default partial wakes model defined for wake model type '{type(wake_model).__name__}'"
+            )
+
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
```

### Comparing `foxes-0.6.2/foxes/models/partial_wakes/axiwake.py` & `foxes-0.7/foxes/models/wake_frames/timelines.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,325 +1,304 @@
 import numpy as np
 
-from foxes.core import PartialWakesModel, Data
-from foxes.models.wake_models.axisymmetric import AxisymmetricWakeModel
-from foxes.utils.two_circles import calc_area
+from foxes.core import WakeFrame
+from foxes.utils import wd2uv
+from foxes.core.data import MData, FData, TData
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class PartialAxiwake(PartialWakesModel):
+class Timelines(WakeFrame):
     """
-    Partial wake calculation for axial wake models.
-
-    The basic idea is that the x-dependent part of
-    the wake model is evaluated only once, and the radial
-    part then for `n` radii that cover the target rotor discs.
-
-    The latter results are then weighted according to the overlap
-    of radial wake circle area deltas and the target rotor disc area.
+    Dynamic wakes for spatially uniform timeseries states.
 
     Attributes
     ----------
-    n: int
-        The number of radial evaluation points
-    rotor_model: foxes.core.RotorModel
-        The rotor model, default is the one from the algorithm
+    max_wake_length: float
+        The maximal wake length
+    cl_ipars: dict
+        Interpolation parameters for centre line
+        point interpolation
+    dt_min: float, optional
+        The delta t value in minutes,
+        if not from timeseries data
 
-    :group: models.partial_wakes
+    :group: models.wake_frames
 
     """
 
-    def __init__(self, n, wake_models=None, wake_frame=None, rotor_model=None):
+    def __init__(self, max_wake_length=2e4, cl_ipars={}, dt_min=None):
         """
         Constructor.
 
         Parameters
         ----------
-        n: int
-            The number of radial evaluation points
-        wake_models: list of foxes.core.WakeModel, optional
-            The wake models, default are the ones from the algorithm
-        wake_frame: foxes.core.WakeFrame, optional
-            The wake frame, default is the one from the algorithm
-        rotor_model: foxes.core.RotorModel, optional
-            The rotor model, default is the one from the algorithm
+        max_wake_length: float
+            The maximal wake length
+        cl_ipars: dict
+            Interpolation parameters for centre line
+            point interpolation
+        dt_min: float, optional
+            The delta t value in minutes,
+            if not from timeseries data
 
         """
-        super().__init__(wake_models, wake_frame)
-
-        self.n = n
-        self.rotor_model = rotor_model
+        super().__init__()
+        self.max_wake_length = max_wake_length
+        self.cl_ipars = cl_ipars
+        self.dt_min = dt_min
 
     def __repr__(self):
-        return super().__repr__() + f"(n={self.n})"
+        return f"{type(self).__name__}(dt_min={self.dt_min})"
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         verbosity: int
             The verbosity level, 0 = silent
 
         """
-        if self.rotor_model is None:
-            self.rotor_model = algo.rotor_model
         super().initialize(algo, verbosity)
 
-        for w in self.wake_models:
-            if not isinstance(w, AxisymmetricWakeModel):
+        if verbosity > 0:
+            print(f"{self.name}: Pre-calculating ambient wind vectors")
+
+        # get and check times:
+        times = np.asarray(algo.states.index())
+        if self.dt_min is None:
+            if not np.issubdtype(times.dtype, np.datetime64):
                 raise TypeError(
-                    f"Partial wakes '{self.name}': Cannot be applied to wake model '{w.name}', since not an AxisymmetricWakeModel"
+                    f"{self.name}: Expecting state index of type np.datetime64, found {times.dtype}"
                 )
+            elif len(times) == 1:
+                raise KeyError(
+                    f"{self.name}: Expecting 'dt_min' for single step timeseries"
+                )
+            dt = (times[1:] - times[:-1]).astype("timedelta64[s]").astype(FC.ITYPE)
+        else:
+            n = max(len(times) - 1, 1)
+            dt = np.full(n, self.dt_min * 60, dtype="timedelta64[s]").astype(FC.ITYPE)
+
+        # calculate horizontal wind vector in all states:
+        self._uv = np.zeros((algo.n_states, 1, 3), dtype=FC.DTYPE)
+
+        # prepare mdata:
+        mdata = algo.get_model_data(algo.states)["data_vars"]
+        mdict = {v: d[1] for v, d in mdata.items()}
+        mdims = {v: d[0] for v, d in mdata.items()}
+        mdata = MData(mdict, mdims, loop_dims=[FC.STATE])
+        del mdict, mdims
+
+        # prepare fdata:
+        fdata = FData({}, {}, loop_dims=[FC.STATE])
+
+        # prepare tdata:
+        tdata = {
+            v: np.zeros((algo.n_states, 1, 1), dtype=FC.DTYPE)
+            for v in algo.states.output_point_vars(algo)
+        }
+        pdims = {v: (FC.STATE, FC.TARGET, FC.TPOINT) for v in tdata.keys()}
+        tdata = TData.from_points(
+            points=np.zeros((algo.n_states, 1, 3), dtype=FC.DTYPE),
+            data=tdata,
+            dims=pdims,
+        )
 
-    def sub_models(self):
-        """
-        List of all sub-models
-
-        Returns
-        -------
-        smdls: list of foxes.core.Model
-            All sub models
-
-        """
-        return super().sub_models() + [self.rotor_model]
+        # calculate:
+        res = algo.states.calculate(algo, mdata, fdata, tdata)
+        if len(dt) == 1:
+            self._dxy = wd2uv(res[FV.WD], res[FV.WS])[:, 0, 0, :2] * dt[:, None]
+        else:
+            self._dxy = wd2uv(res[FV.WD], res[FV.WS])[:-1, 0, 0, :2] * dt[:, None]
+            self._dxy = np.insert(self._dxy, 0, self._dxy[0], axis=0)
+
+        """ DEBUG
+        import matplotlib.pyplot as plt
+        xy = np.array([np.sum(self._dxy[:n], axis=0) for n in range(len(self._dxy))])
+        print(xy)
+        plt.plot(xy[:, 0], xy[:, 1])
+        plt.show()
+        quit()
+        """
+
+    def calc_order(self, algo, mdata, fdata):
+        """ "
+        Calculates the order of turbine evaluation.
 
-    def new_wake_deltas(self, algo, mdata, fdata):
-        """
-        Creates new initial wake deltas, filled
-        with zeros.
+        This function is executed on a single chunk of data,
+        all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
 
         Returns
         -------
-        wake_deltas: dict
-            Keys: Variable name str, values: any
-        pdata: foxes.core.Data
-            The evaluation point data
+        order: numpy.ndarray
+            The turbine order, shape: (n_states, n_turbines)
 
         """
-        pdata = Data.from_points(points=fdata[FV.TXYH])
+        # prepare:
+        n_states = fdata.n_states
+        n_turbines = algo.n_turbines
+        tdata = TData.from_points(points=fdata[FV.TXYH])
 
-        wake_deltas = {}
-        for w in self.wake_models:
-            w.init_wake_deltas(algo, mdata, fdata, pdata, wake_deltas)
+        # calculate streamline x coordinates for turbines rotor centre points:
+        # n_states, n_turbines_source, n_turbines_target
+        coosx = np.zeros((n_states, n_turbines, n_turbines), dtype=FC.DTYPE)
+        for ti in range(n_turbines):
+            coosx[:, ti, :] = self.get_wake_coos(algo, mdata, fdata, tdata, ti)[
+                :, :, 0, 0
+            ]
+
+        # derive turbine order:
+        # TODO: Remove loop over states
+        order = np.zeros((n_states, n_turbines), dtype=FC.ITYPE)
+        for si in range(n_states):
+            order[si] = np.lexsort(keys=coosx[si])
 
-        return wake_deltas, pdata
+        return order
 
-    def contribute_to_wake_deltas(
+    def get_wake_coos(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        wake_deltas,
+        tdata,
+        downwind_index,
     ):
         """
-        Modifies wake deltas by contributions from the
-        specified wake source turbines.
+        Calculate wake coordinates of rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray of int
-            For each state, one turbine index corresponding
-            to the wake causing turbine. Shape: (n_states,)
-        wake_deltas: Any
-            The wake deltas object created by the
-            `new_wake_deltas` function
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+
+        Returns
+        -------
+        wake_coos: numpy.ndarray
+            The wake frame coordinates of the evaluation
+            points, shape: (n_states, n_targets, n_tpoints, 3)
 
         """
         # prepare:
-        n_states = mdata.n_states
-        n_turbines = algo.n_turbines
-        D = fdata[FV.D]
+        targets = tdata[FC.TARGETS]
+        n_states, n_targets, n_tpoints = targets.shape[:3]
+        n_points = n_targets * n_tpoints
+        points = targets.reshape(n_states, n_points, 3)
+        rxyz = fdata[FV.TXYH][:, downwind_index]
+
+        D = np.zeros((n_states, n_points), dtype=FC.DTYPE)
+        D[:] = fdata[FV.D][:, downwind_index, None]
+
+        i0 = mdata.states_i0(counter=True, algo=algo)
+        i1 = i0 + mdata.n_states
+        dxy = self._dxy[:i1]
+
+        trace_p = np.zeros((n_states, n_points, 2), dtype=FC.DTYPE)
+        trace_p[:] = points[:, :, :2] - rxyz[:, None, :2]
+        trace_l = np.zeros((n_states, n_points), dtype=FC.DTYPE)
+        trace_d = np.full((n_states, n_points), np.inf, dtype=FC.DTYPE)
+        trace_si = np.zeros((n_states, n_points), dtype=FC.ITYPE)
+        trace_si[:] = i0 + np.arange(n_states)[:, None] + 1
+
+        wcoos = np.full((n_states, n_points, 3), 1e20, dtype=FC.DTYPE)
+        wcoosx = wcoos[:, :, 0]
+        wcoosy = wcoos[:, :, 1]
+        wcoos[:, :, 2] = points[:, :, 2] - rxyz[:, None, 2]
+        del rxyz
+
+        while True:
+            sel = (trace_si > 0) & (trace_l < self.max_wake_length)
+            if np.any(sel):
+                trace_si[sel] -= 1
+
+                delta = dxy[trace_si[sel]]
+                dmag = np.linalg.norm(delta, axis=-1)
+
+                trace_p[sel] -= delta
+                trace_l[sel] += dmag
+
+                trp = trace_p[sel]
+                d0 = trace_d[sel]
+                d = np.linalg.norm(trp, axis=-1)
+                trace_d[sel] = d
+
+                seln = d <= np.minimum(d0, 2 * dmag)
+                if np.any(seln):
+                    htrp = trp[seln]
+                    raxis = delta[seln]
+                    raxis = raxis / np.linalg.norm(raxis, axis=-1)[:, None]
+                    saxis = np.concatenate(
+                        [-raxis[:, 1, None], raxis[:, 0, None]], axis=1
+                    )
 
-        # calc coordinates to rotor centres:
-        wcoos = self.wake_frame.get_wake_coos(
-            algo, mdata, fdata, pdata, states_source_turbine
+                    wcx = wcoosx[sel]
+                    wcx[seln] = np.einsum("sd,sd->s", htrp, raxis) + trace_l[sel][seln]
+                    wcoosx[sel] = wcx
+                    del wcx, raxis
+
+                    wcy = wcoosy[sel]
+                    wcy[seln] = np.einsum("sd,sd->s", htrp, saxis)
+                    wcoosy[sel] = wcy
+                    del wcy, saxis, htrp
+
+            else:
+                break
+
+        # turbines that cause wake:
+        tdata[FC.STATE_SOURCE_ORDERI] = downwind_index
+
+        # states that cause wake for each target point:
+        tdata.add(
+            FC.STATES_SEL,
+            trace_si.reshape(n_states, n_targets, n_tpoints),
+            (FC.STATE, FC.TARGET, FC.TPOINT),
         )
 
-        # prepare x and r coordinates:
-        x = wcoos[:, :, 0]
-        n = wcoos[:, :, 1:3]
-        R = np.linalg.norm(n, axis=-1)
-        r = np.zeros((n_states, n_turbines, self.n), dtype=FC.DTYPE)
-        del wcoos
-
-        # prepare circle section area calculation:
-        A = np.zeros((n_states, n_turbines, self.n), dtype=FC.DTYPE)
-        weights = np.zeros_like(A)
-
-        # get normalized 2D vector between rotor and wake centres:
-        sel = R > 0.0
-        if np.any(sel):
-            n[sel] /= R[sel][:, None]
-        if np.any(~sel):
-            n[:, :, 0][~sel] = 1
-
-        # case wake centre outside rotor disk:
-        sel = (x > 1e-5) & (R > D / 2)
-        if np.any(sel):
-            n_sel = np.sum(sel)
-            Rsel = np.zeros((n_sel, self.n + 1), dtype=FC.DTYPE)
-            Rsel[:] = R[sel][:, None]
-            Dsel = D[sel][:, None]
-
-            # equal delta R2:
-            R1 = np.zeros((n_sel, self.n + 1), dtype=FC.DTYPE)
-            R1[:] = Dsel / 2
-            steps = np.linspace(0.0, 1.0, self.n + 1, endpoint=True) - 0.5
-            R2 = np.zeros_like(R1)
-            R2[:] = Rsel + Dsel * steps[None, :]
-            r[sel] = 0.5 * (R2[:, 1:] + R2[:, :-1])
-
-            hA = calc_area(R1, R2, Rsel)
-            hA = hA[:, 1:] - hA[:, :-1] + 1e-15
-
-            weights[sel] = hA / np.sum(hA, axis=-1)[:, None]
-            del hA, Rsel, Dsel, R1, R2
-
-        # case wake centre inside rotor disk:
-        sel = (x > 1e-5) & (R < D / 2)
-        if np.any(sel):
-            n_sel = np.sum(sel)
-            Rsel = np.zeros((n_sel, self.n + 1), dtype=FC.DTYPE)
-            Rsel[:] = R[sel][:, None]
-            Dsel = D[sel][:, None]
-
-            # equal delta R2:
-            R1 = np.zeros((n_sel, self.n + 1), dtype=FC.DTYPE)
-            R1[:, 1:] = Dsel / 2
-            R2 = np.zeros_like(R1)
-            # R2[:, 1:] = Rsel[:, :-1] + Dsel/2
-            # R2[:]    *= np.linspace(0., 1, self.n + 1, endpoint=True)[None, :]
-            R2[:, 1:] = (Rsel[:, :-1] + Dsel / 2) / (self.n - 0.5)
-            R2[:, 1:] *= (
-                0.5 + np.linspace(0.0, self.n - 1, self.n, endpoint=True)[None, :]
-            )
-            hr = 0.5 * (R2[:, 1:] + R2[:, :-1])
-            hr[:, 0] = 0.0
-            r[sel] = hr
-
-            hA = calc_area(R1, R2, Rsel)
-            hA = hA[:, 1:] - hA[:, :-1]
-            weights[sel] = hA / np.sum(hA, axis=-1)[:, None]
-            del hA, hr, Rsel, Dsel, R1, R2
-
-        # evaluate wake models:
-        for w in self.wake_models:
-            wdeltas, sp_sel = w.calc_wakes_spsel_x_r(
-                algo, mdata, fdata, pdata, states_source_turbine, x, r
-            )
-
-            for v, wdel in wdeltas.items():
-                d = np.einsum("ps,ps->p", wdel, weights[sp_sel])
-
-                try:
-                    superp = w.superp[v]
-                except KeyError:
-                    raise KeyError(
-                        f"Model '{self.name}': Missing wake superposition entry for variable '{v}' in wake model '{w.name}', found {sorted(list(w.superp.keys()))}"
-                    )
+        return wcoos.reshape(n_states, n_targets, n_tpoints, 3)
 
-                wake_deltas[v] = superp.calc_wakes_plus_wake(
-                    algo,
-                    mdata,
-                    fdata,
-                    pdata,
-                    states_source_turbine,
-                    sp_sel,
-                    v,
-                    wake_deltas[v],
-                    d,
-                )
-
-    def evaluate_results(
-        self,
-        algo,
-        mdata,
-        fdata,
-        pdata,
-        wake_deltas,
-        states_turbine,
-        amb_res=None,
-    ):
+    def get_centreline_points(self, algo, mdata, fdata, downwind_index, x):
         """
-        Updates the farm data according to the wake
-        deltas.
+        Gets the points along the centreline for given
+        values of x.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-            Modified in-place by this function
-        pdata: foxes.core.Data
-            The evaluation point data
-        wake_deltas: Any
-            The wake deltas object, created by the
-            `new_wake_deltas` function and filled
-            by `contribute_to_wake_deltas`
-        states_turbine: numpy.ndarray of int
-            For each state, the index of one turbine
-            for which to evaluate the wake deltas.
-            Shape: (n_states,)
-        amb_res: dict, optional
-            Ambient states results. Keys: var str, values:
-            numpy.ndarray of shape (n_states, n_points)
-
-        """
+        downwind_index: int
+            The index in the downwind order
+        x: numpy.ndarray
+            The wake frame x coordinates, shape: (n_states, n_points)
 
-        weights = algo.rotor_model.from_data_or_store(FC.RWEIGHTS, algo, mdata)
-        rpoints = algo.rotor_model.from_data_or_store(FC.RPOINTS, algo, mdata)
-        n_states, n_turbines, n_rpoints, __ = rpoints.shape
-
-        amb_res_in = amb_res is not None
-        if not amb_res_in:
-            amb_res = algo.rotor_model.from_data_or_store(
-                FC.AMB_RPOINT_RESULTS, algo, mdata
-            )
-
-        wres = {}
-        st_sel = (np.arange(n_states), states_turbine)
-        for v, ares in amb_res.items():
-            wres[v] = ares.reshape(n_states, n_turbines, n_rpoints)[st_sel]
-
-        wdel = {}
-        for v, d in wake_deltas.items():
-            wdel[v] = d.reshape(n_states, n_turbines, 1)[st_sel]
-        for w in self.wake_models:
-            w.finalize_wake_deltas(algo, mdata, fdata, pdata, wres, wdel)
-
-        for v in wres.keys():
-            if v in wake_deltas:
-                wres[v] += wdel[v]
-                if amb_res_in:
-                    amb_res[v][st_sel] = wres[v]
-            wres[v] = wres[v][:, None]
+        Returns
+        -------
+        points: numpy.ndarray
+            The centreline points, shape: (n_states, n_points, 3)
 
-        self.rotor_model.eval_rpoint_results(
-            algo, mdata, fdata, wres, weights, states_turbine=states_turbine
-        )
+        """
+        raise NotImplementedError
```

### Comparing `foxes-0.6.2/foxes/models/partial_wakes/centre.py` & `foxes-0.7/foxes/models/partial_wakes/rotor_points.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,98 @@
-import numpy as np
+from foxes.core import PartialWakesModel
 
-import foxes.constants as FC
-import foxes.variables as FV
 
-from .rotor_points import RotorPoints
-
-
-class PartialCentre(RotorPoints):
+class RotorPoints(PartialWakesModel):
     """
-    Partial wakes calculated only at the 
-    rotor centre point.
+    Partial wakes calculation directly by the
+    rotor model.
 
     :group: models.partial_wakes
 
     """
 
     def get_wake_points(self, algo, mdata, fdata):
         """
-        Get the wake calculation points.
+        Get the wake calculation points, and their
+        weights.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
 
         Returns
         -------
         rpoints: numpy.ndarray
-            All rotor points, shape: (n_states, n_points, 3)
+            The wake calculation points, shape:
+            (n_states, n_turbines, n_tpoints, 3)
+        rweights: numpy.ndarray
+            The target point weights, shape: (n_tpoints,)
 
         """
-        return fdata[FV.TXYH]
-
+        rotor = algo.rotor_model
+        return (
+            rotor.from_data_or_store(rotor.RPOINTS, algo, mdata),
+            rotor.from_data_or_store(rotor.RWEIGHTS, algo, mdata),
+        )
 
-    def evaluate_results(
+    def finalize_wakes(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
+        tdata,
+        amb_res,
+        rpoint_weights,
         wake_deltas,
-        states_turbine,
-        amb_res=None,
+        wmodel,
+        downwind_index,
     ):
         """
-        Updates the farm data according to the wake
-        deltas.
+        Updates the wake_deltas at the selected target
+        downwind index.
+
+        Modifies wake_deltas on the fly.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-            Modified in-place by this function
-        pdata: foxes.core.Data
-            The evaluation point data
-        wake_deltas: Any
-            The wake deltas object, created by the
-            `new_wake_deltas` function and filled
-            by `contribute_to_wake_deltas`
-        states_turbine: numpy.ndarray of int
-            For each state, the index of one turbine
-            for which to evaluate the wake deltas.
-            Shape: (n_states,)
-        amb_res: dict, optional
-            Ambient states results. Keys: var str, values:
-            numpy.ndarray of shape (n_states, n_points)
+        tdata: foxes.core.Data
+            The target point data
+        amb_res: dict
+            The ambient results at the target points
+            of all rotors. Key: variable name, value
+            np.ndarray of shape:
+            (n_states, n_turbines, n_rotor_points)
+        rpoint_weights: numpy.ndarray
+            The rotor point weights, shape: (n_rotor_points,)
+        wake_deltas: dict
+            The wake deltas. Key: variable name,
+            value: np.ndarray of shape
+            (n_states, n_turbines, n_tpoints)
+        wmodel: foxes.core.WakeModel
+            The wake model
+        downwind_index: int
+            The index in the downwind order
+
+        Returns
+        -------
+        final_wake_deltas: dict
+            The final wake deltas at the selected downwind
+            turbines. Key: variable name, value: np.ndarray
+            of shape (n_states, n_rotor_points)
 
         """
-        weights = algo.rotor_model.from_data_or_store(FC.RWEIGHTS, algo, mdata)
-        rpoints = algo.rotor_model.from_data_or_store(FC.RPOINTS, algo, mdata)
-        n_states, n_turbines, n_rpoints, __ = rpoints.shape
-
-        amb_res_in = amb_res is not None
-        if not amb_res_in:
-            amb_res = algo.rotor_model.from_data_or_store(
-                FC.AMB_RPOINT_RESULTS, algo, mdata
-            )
-
-        wres = {}
-        st_sel = (np.arange(n_states), states_turbine)
-        for v, ares in amb_res.items():
-            wres[v] = ares.reshape(n_states, n_turbines, n_rpoints)[st_sel]
-
-        wdel = {}
-        for v, d in wake_deltas.items():
-            wdel[v] = d.reshape(n_states, n_turbines, 1)[st_sel]
-        for w in self.wake_models:
-            w.finalize_wake_deltas(algo, mdata, fdata, pdata, wres, wdel)
-
-        for v in wres.keys():
-            if v in wake_deltas:
-                wres[v] += wdel[v]
-                if amb_res_in:
-                    amb_res[v][st_sel] = wres[v]
-            wres[v] = wres[v][:, None]
+        ares = {v: d[:, downwind_index, None] for v, d in amb_res.items()}
+        wdel = {v: d[:, downwind_index, None].copy() for v, d in wake_deltas.items()}
+        wmodel.finalize_wake_deltas(algo, mdata, fdata, ares, wdel)
 
-        algo.rotor_model.eval_rpoint_results(
-            algo, mdata, fdata, wres, weights, states_turbine=states_turbine
-        )
+        return {v: d[:, 0] for v, d in wdel.items()}
```

### Comparing `foxes-0.6.2/foxes/models/partial_wakes/grid.py` & `foxes-0.7/foxes/models/wake_models/gaussian.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,106 @@
-from foxes.models.partial_wakes.distsliced import PartialDistSlicedWake
-from foxes.models.rotor_models.grid import GridRotor
+import numpy as np
+from abc import abstractmethod
 
+from foxes.models.wake_models.axisymmetric import AxisymmetricWakeModel
 
-class PartialGrid(PartialDistSlicedWake):
+
+class GaussianWakeModel(AxisymmetricWakeModel):
     """
-    Partial wakes on a grid rotor that may
-    differ from the one in the algorithm.
+    Abstract base class for Gaussian wake models.
 
-    :group: models.partial_wakes
+    :group: models.wake_models
 
     """
 
-    def __init__(
-        self, n, wake_models=None, wake_frame=None, rotor_model=None, **kwargs
+    @abstractmethod
+    def calc_amplitude_sigma(
+        self,
+        algo,
+        mdata,
+        fdata,
+        tdata,
+        downwind_index,
+        x,
     ):
         """
-        Constructor.
+        Calculate the amplitude and the sigma,
+        both depend only on x (not on r).
 
         Parameters
         ----------
-        n: int, optional
-            The `GridRotor`'s `n` parameter
-        wake_models: list of foxes.core.WakeModel, optional
-            The wake models, default are the ones from the algorithm
-        wake_frame: foxes.core.WakeFrame, optional
-            The wake frame, default is the one from the algorithm
-        rotor_model: foxes.core.RotorModel, optional
-            The rotor model, default is the one from the algorithm
-        kwargs: dict, optional
-            Additional parameters for the `GridRotor`
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.MData
+            The model data
+        fdata: foxes.core.FData
+            The farm data
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
+        x: numpy.ndarray
+            The x values, shape: (n_states, n_targets)
+
+        Returns
+        -------
+        amsi: tuple
+            The amplitude and sigma, both numpy.ndarray
+            with shape (n_st_sel,)
+        st_sel: numpy.ndarray of bool
+            The state-target selection, for which the wake
+            is non-zero, shape: (n_states, n_targets)
 
         """
-        super().__init__(n, wake_models, wake_frame, rotor_model, **kwargs)
+        pass
 
-        if not isinstance(self.grotor, GridRotor):
-            raise ValueError(
-                f"Wrong grotor type, expecting {GridRotor.__name__}, got {type(self.grotor).__name__}"
-            )
-
-    def contribute_to_wake_deltas(
+    def calc_wakes_x_r(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        wake_deltas,
+        tdata,
+        downwind_index,
+        x,
+        r,
     ):
         """
-        Modifies wake deltas by contributions from the
-        specified wake source turbines.
+        Calculate wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray of int
-            For each state, one turbine index corresponding
-            to the wake causing turbine. Shape: (n_states,)
-        wake_deltas: Any
-            The wake deltas object created by the
-            `new_wake_deltas` function
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
+        x: numpy.ndarray
+            The x values, shape: (n_states, n_targets)
+        r: numpy.ndarray
+            The radial values for each x value, shape:
+            (n_states, n_targets, n_yz_per_target)
+
+        Returns
+        -------
+        wdeltas: dict
+            The wake deltas. Key: variable name str,
+            value: numpy.ndarray, shape: (n_st_sel, n_r_per_x)
+        st_sel: numpy.ndarray of bool
+            The state-target selection, for which the wake
+            is non-zero, shape: (n_states, n_targets)
 
         """
-
-        # evaluate grid rotor:
-        wcoos = self.wake_frame.get_wake_coos(
-            algo, mdata, fdata, pdata, states_source_turbine
+        amsi, st_sel = self.calc_amplitude_sigma(
+            algo, mdata, fdata, tdata, downwind_index, x
         )
+        wdeltas = {}
+        rsel = r[st_sel]
+        for v in amsi.keys():
+            ampld, sigma = amsi[v]
+            wdeltas[v] = ampld[:, None] * np.exp(-0.5 * (rsel / sigma[:, None]) ** 2)
 
-        # evaluate wake models:
-        for w in self.wake_models:
-            w.contribute_to_wake_deltas(
-                algo, mdata, fdata, pdata, states_source_turbine, wcoos, wake_deltas
-            )
+        return wdeltas, st_sel
```

### Comparing `foxes-0.6.2/foxes/models/partial_wakes/mapped.py` & `foxes-0.7/foxes/models/wake_models/ti/crespo_hernandez.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,252 +1,333 @@
-from copy import deepcopy
+import numpy as np
 
-from foxes.core import PartialWakesModel
-from foxes.models.partial_wakes.rotor_points import RotorPoints
-from foxes.models.partial_wakes.top_hat import PartialTopHat
-from foxes.models.partial_wakes.axiwake import PartialAxiwake
-from foxes.models.partial_wakes.distsliced import PartialDistSlicedWake
 from foxes.models.wake_models.top_hat import TopHatWakeModel
-from foxes.models.wake_models.dist_sliced import DistSlicedWakeModel
-from foxes.models.wake_models.axisymmetric import AxisymmetricWakeModel
+import foxes.variables as FV
 import foxes.constants as FC
 
 
-class Mapped(PartialWakesModel):
+class CrespoHernandezTIWake(TopHatWakeModel):
     """
-    Partial wake models depending on the wake model (type).
+    The Crespo and Hernandez TI empirical correlation
 
-    This is required if more than one wake models are
-    used and different partial wake models should be invoked.
+    Notes
+    -----
+    Reference:
+    "Turbulence characteristics in wind-turbine wakes"
+    A. Crespo, J. Hernandez
+    https://doi.org/10.1016/0167-6105(95)00033-X
+
+    For the wake diameter we use Eqns. (17), (15), (4), (5) from
+            doi:10.1088/1742-6596/625/1/012039
 
     Attributes
     ----------
-    wname2pwake: dict
-        Mapping from wake model name to partial wakes.
-        Key: model name str, value: Tuple of length 2,
-        (Partial wake class name, parameter dict)
-    wtype2pwake: dict
-        Mapping from wake model class name to partial wakes.
-        Key: wake model class name str, value: Tuple of length 2,
-        (Partial wake class name, parameter dict)
+    k: float
+        The wake growth parameter k. If not given here
+        it will be searched in the farm data.
+    a_near: float
+        Model parameter
+    a_far: float
+        Model parameter
+    e1: float
+        Model parameter
+    e2: float
+        Model parameter
+    e3: float
+        Model parameter
+    use_ambti: bool
+        Flag for using ambient TI instead of local
+        wake corrected TI
+    sbeta_factor: float
+        Factor multiplying sbeta
+    near_wake_D: float
+        The near wake distance in units of D,
+        calculated from TI and ct if None
+    k_var: str
+        The variable name for k
 
-    :group: models.partial_wakes
+    :group: models.wake_models.ti
 
     """
 
     def __init__(
-        self, wname2pwake={}, wtype2pwake=None, wake_models=None, wake_frame=None
+        self,
+        superposition,
+        k=None,
+        use_ambti=False,
+        sbeta_factor=0.25,
+        near_wake_D=None,
+        a_near=0.362,
+        a_far=0.73,
+        e1=0.83,
+        e2=-0.0325,
+        e3=-0.32,
+        k_var=FV.K,
+        **kwargs,
     ):
         """
         Constructor.
 
         Parameters
         ----------
-        wname2pwake: dict, optional
-            Mapping from wake model name to partial wakes.
-            Key: model name str, value: Tuple of length 2,
-            (Partial wake class name, parameter dict)
-        wtype2pwake: dict, optional
-            Mapping from wake model class name to partial wakes.
-            Key: wake model class name str, value: Tuple of length 2,
-            (Partial wake class name, parameter dict)
-        wake_models: list of foxes.core.WakeModel, optional
-            The wake models, default are the ones from the algorithm
-        wake_frame: foxes.core.WakeFrame, optional
-            The wake frame, default is the one from the algorithm
-
-        """
-        super().__init__(wake_models, wake_frame)
-
-        self.wname2pwake = wname2pwake
-
-        if wtype2pwake is None:
-            self.wtype2pwake = {
-                TopHatWakeModel: (PartialTopHat.__name__, {}),
-                AxisymmetricWakeModel: (PartialAxiwake.__name__, {"n": 6}),
-                DistSlicedWakeModel: (PartialDistSlicedWake.__name__, {"n": 9}),
-            }
+        superposition: str
+            The TI wake superposition.
+        k: float, optional
+            The wake growth parameter k. If not given here
+            it will be searched in the farm data.
+        use_ambti: bool
+            Flag for using ambient TI instead of local
+            wake corrected TI
+        sbeta_factor: float
+            Factor multiplying sbeta
+        near_wake_D: float, optional
+            The near wake distance in units of D,
+            calculated from TI and ct if not given here
+        a_near: float
+            Model parameter
+        a_far: float
+            Model parameter
+        e1: float
+            Model parameter
+        e2: float
+            Model parameter
+        e3: float
+            Model parameter
+        k_var: str
+            The variable name for k
+        kwargs: dict, optional
+            Additional parameters for the base class
+
+        """
+        super().__init__(superpositions={FV.TI: superposition}, **kwargs)
+
+        self.a_near = a_near
+        self.a_far = a_far
+        self.e1 = e1
+        self.e2 = e2
+        self.e3 = e3
+        self.use_ambti = use_ambti
+        self.sbeta_factor = sbeta_factor
+        self.near_wake_D = near_wake_D
+        self.k_var = k_var
+
+        setattr(self, k_var, k)
+
+    def __repr__(self):
+        k = getattr(self, self.k_var)
+        iname = (
+            self.induction if isinstance(self.induction, str) else self.induction.name
+        )
+        s = f"{type(self).__name__}"
+        s += f"({self.superpositions[FV.TI]}, induction={iname}"
+        if k is None:
+            s += f", k_var={self.k_var}"
         else:
-            self.wtype2pwake = wtype2pwake
-
-        self._pwakes = None
+            s += f", {self.k_var}={k}"
+        s += ")"
+        return s
 
-    def initialize(self, algo, verbosity=0):
+    def new_wake_deltas(self, algo, mdata, fdata, tdata):
         """
-        Initializes the model.
+        Creates new empty wake delta arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
-
-        """
-        self.wake_models = algo.wake_models if self._wmodels is None else self._wmodels
-        self.wake_frame = algo.wake_frame if self._wframe is None else self._wframe
-
-        pws = {}
-        for w in self.wake_models:
-            pdat = None
-            if w.name in self.wname2pwake:
-                pdat = deepcopy(self.wname2pwake[w.name])
-
-            if pdat is None:
-                for pwcls, tdat in self.wtype2pwake.items():
-                    if isinstance(w, pwcls):
-                        pdat = deepcopy(tdat)
-                        break
-
-            if pdat is None:
-                pdat = (RotorPoints.__name__, {})
-
-            pname = pdat[0]
-            if pname not in pws:
-                pws[pname] = pdat[1]
-                pws[pname]["wake_models"] = []
-                pws[pname]["wake_frame"] = self.wake_frame
-            pws[pname]["wake_models"].append(w)
-
-        self._pwakes = []
-        for pname, pars in pws.items():
-            if verbosity:
-                print(
-                    f"Partial wakes '{self.name}': Applying {pname} to {[w.name for w in pars['wake_models']]}"
-                )
-            self._pwakes.append(PartialWakesModel.new(pname, **pars))
-
-        super().initialize(algo, verbosity)
-
-    def sub_models(self):
-        """
-        List of all sub-models
-
-        Returns
-        -------
-        smdls: list of foxes.core.Model
-            Names of all sub models
-
-        """
-        return super().sub_models() + self._pwakes
-
-    def new_wake_deltas(self, algo, mdata, fdata):
-        """
-        Creates new initial wake deltas, filled
-        with zeros.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
+        tdata: foxes.core.TData
+            The target point data
 
         Returns
         -------
         wake_deltas: dict
-            Keys: Variable name str, values: any
-        pdata: foxes.core.Data
-            The evaluation point data
+            Key: variable name, value: The zero filled
+            wake deltas, shape: (n_states, n_turbines, n_rpoints, ...)
 
         """
-        wdeltas = []
-        pdatas = []
-        for pw in self._pwakes:
-            w, p = pw.new_wake_deltas(algo, mdata, fdata)
-            wdeltas.append(w)
-            pdatas.append(p)
+        return {FV.TI: np.zeros_like(tdata[FC.TARGETS][..., 0])}
 
-        return wdeltas, pdatas
-
-    def contribute_to_wake_deltas(
+    def calc_wake_radius(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        wake_deltas,
+        tdata,
+        downwind_index,
+        x,
+        ct,
     ):
         """
-        Modifies wake deltas by contributions from the
-        specified wake source turbines.
+        Calculate the wake radius, depending on x only (not r).
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray of int
-            For each state, one turbine index corresponding
-            to the wake causing turbine. Shape: (n_states,)
-        wake_deltas: Any
-            The wake deltas object created by the
-            `new_wake_deltas` function
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
+        x: numpy.ndarray
+            The x values, shape: (n_states, n_targets)
+        ct: numpy.ndarray
+            The ct values of the wake-causing turbines,
+            shape: (n_states, n_targets)
+
+        Returns
+        -------
+        wake_r: numpy.ndarray
+            The wake radii, shape: (n_states, n_targets)
 
         """
-        for pwi, pw in enumerate(self._pwakes):
-            pw.contribute_to_wake_deltas(
-                algo, mdata, fdata, pdata[pwi], states_source_turbine, wake_deltas[pwi]
-            )
+        # get D:
+        D = self.get_data(
+            FV.D,
+            FC.STATE_TARGET,
+            lookup="w",
+            algo=algo,
+            fdata=fdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
+            upcast=False,
+        )
+
+        # get k:
+        k = self.get_data(
+            self.k_var,
+            FC.STATE_TARGET,
+            lookup="sw",
+            algo=algo,
+            fdata=fdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
+            upcast=False,
+        )
+
+        # calculate:
+        a = self.induction.ct2a(ct)
+        beta = (1 - a) / (1 - 2 * a)
+        radius = 2 * (k * x + self.sbeta_factor * np.sqrt(beta) * D)
+
+        return radius
 
-    def evaluate_results(
+    def calc_centreline(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        wake_deltas,
-        states_turbine,
-        amb_res=None,
+        tdata,
+        downwind_index,
+        st_sel,
+        x,
+        wake_r,
+        ct,
     ):
         """
-        Updates the farm data according to the wake
-        deltas.
+        Calculate centre line results of wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-            Modified in-place by this function
-        pdata: foxes.core.Data
-            The evaluation point data
-        wake_deltas: Any
-            The wake deltas object, created by the
-            `new_wake_deltas` function and filled
-            by `contribute_to_wake_deltas`
-        states_turbine: numpy.ndarray of int
-            For each state, the index of one turbine
-            for which to evaluate the wake deltas.
-            Shape: (n_states,)
-        amb_res: dict, optional
-            Ambient states results. Keys: var str, values:
-            numpy.ndarray of shape (n_states, n_points)
-
-        """
-        if amb_res is None:
-            ares = algo.rotor_model.from_data_or_store(
-                FC.AMB_RPOINT_RESULTS, algo, mdata
-            ).copy()
-            amb_res = {v: d.copy() for v, d in ares.items()}
-
-        for pwi, pw in enumerate(self._pwakes):
-            pw.evaluate_results(
-                algo,
-                mdata,
-                fdata,
-                pdata[pwi],
-                wake_deltas[pwi],
-                states_turbine,
-                amb_res=amb_res,
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
+        st_sel: numpy.ndarray of bool
+            The state-target selection, for which the wake
+            is non-zero, shape: (n_states, n_targets)
+        x: numpy.ndarray
+            The x values, shape: (n_st_sel,)
+        wake_r: numpy.ndarray
+            The wake radii, shape: (n_st_sel,)
+        ct: numpy.ndarray
+            The ct values of the wake-causing turbines,
+            shape: (n_st_sel,)
+
+        Returns
+        -------
+        cl_del: dict
+            The centre line wake deltas. Key: variable name str,
+            varlue: numpy.ndarray, shape: (n_st_sel,)
+
+        """
+        # prepare:
+        n_targts = np.sum(st_sel)
+        TI = FV.AMB_TI if self.use_ambti else FV.TI
+
+        # get D:
+        D = self.get_data(
+            FV.D,
+            FC.STATE_TARGET,
+            lookup="w",
+            algo=algo,
+            fdata=fdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
+            upcast=True,
+        )[st_sel]
+
+        # get TI:
+        ti = self.get_data(
+            TI,
+            FC.STATE_TARGET,
+            lookup="w",
+            algo=algo,
+            fdata=fdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
+            upcast=True,
+        )[st_sel]
+
+        # calculate induction factor:
+        twoa = 2 * self.induction.ct2a(ct)
+
+        # prepare output:
+        wake_deltas = np.zeros(n_targts, dtype=FC.DTYPE)
+
+        # calc near wake length, if not given
+        if self.near_wake_D is None:
+            near_wake_D = (
+                2**self.e1
+                * self.a_near
+                / (self.a_far * ti**self.e2)
+                * twoa ** (1 - self.e1)
+            ) ** (1 / self.e3)
+        else:
+            near_wake_D = self.near_wake_D
+
+        # calc near wake:
+        sel = x < near_wake_D * D
+        if np.any(sel):
+            wake_deltas[sel] = self.a_near * twoa[sel]
+
+        # calc far wake:
+        if np.any(~sel):
+            # calculate delta:
+            #
+            # Note the sign flip of the exponent ti[~sel]**(-0.0325)
+            # compared to the original paper. This was found in
+            # https://doi.org/10.1016/j.jweia.2018.04.010, Eq. (46)
+            # Without this flip the near and far wake areas are not
+            # smoothly connected.
+            #
+            wake_deltas[~sel] = (
+                self.a_far
+                * (twoa[~sel] / 2) ** self.e1
+                * ti[~sel] ** self.e2
+                * (x[~sel] / D[~sel]) ** self.e3
             )
+
+        return {FV.TI: wake_deltas}
```

### Comparing `foxes-0.6.2/foxes/models/partial_wakes/rotor_points.py` & `foxes-0.7/foxes/models/wake_models/dist_sliced.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,192 +1,218 @@
+from abc import abstractmethod
 import numpy as np
 
-from foxes.core import PartialWakesModel, Data
-import foxes.constants as FC
+from foxes.core import WakeModel
 
 
-class RotorPoints(PartialWakesModel):
+class DistSlicedWakeModel(WakeModel):
     """
-    Partial wakes calculation directly by the
-    rotor model.
+    Abstract base class for wake models for which
+    the x-denpendency can be separated from the
+    yz-dependency.
+
+    The multi-yz ability is used by the `PartialDistSlicedWake`
+    partial wakes model.
+
+    Attributes
+    ----------
+    superpositions: dict
+        The superpositions. Key: variable name str,
+        value: The wake superposition model name,
+        will be looked up in model book
+    superp: dict
+        The superposition dict, key: variable name str,
+        value: `foxes.core.WakeSuperposition`
 
-    :group: models.partial_wakes
+    :group: models.wake_models
 
     """
 
-    def __init__(self, wake_models=None, wake_frame=None):
+    def __init__(self, superpositions):
         """
         Constructor.
 
         Parameters
         ----------
-        wake_models: list of foxes.core.WakeModel, optional
-            The wake models, default are the ones from the algorithm
-        wake_frame: foxes.core.WakeFrame, optional
-            The wake frame, default is the one from the algorithm
+        superpositions: dict
+            The superpositions. Key: variable name str,
+            value: The wake superposition model name,
+            will be looked up in model book
 
         """
-        super().__init__(wake_models, wake_frame)
+        super().__init__()
+        self.superpositions = superpositions
 
-    def get_wake_points(self, algo, mdata, fdata):
+    def sub_models(self):
         """
-        Get the wake calculation points.
+        List of all sub-models
+
+        Returns
+        -------
+        smdls: list of foxes.core.Model
+            Names of all sub models
+
+        """
+        return list(self.superp.values())
+
+    def initialize(self, algo, verbosity=0, force=False):
+        """
+        Initializes the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-
-        Returns
-        -------
-        rpoints: numpy.ndarray
-            All rotor points, shape: (n_states, n_points, 3)
+        verbosity: int
+            The verbosity level, 0 = silent
+        force: bool
+            Overwrite existing data
 
         """
-        rpoints = algo.rotor_model.from_data_or_store(FC.RPOINTS, algo, mdata)
-        n_states, n_turbines, n_rpoints, __ = rpoints.shape
-        return rpoints.reshape(n_states, n_turbines * n_rpoints, 3)
+        self.superp = {
+            v: algo.mbook.wake_superpositions[s] for v, s in self.superpositions.items()
+        }
+        super().initialize(algo, verbosity, force)
 
-    def new_wake_deltas(self, algo, mdata, fdata):
+    @abstractmethod
+    def calc_wakes_x_yz(
+        self,
+        algo,
+        mdata,
+        fdata,
+        tdata,
+        downwind_index,
+        x,
+        yz,
+    ):
         """
-        Creates new initial wake deltas, filled
-        with zeros.
+        Calculate wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
+        x: numpy.ndarray
+            The x values, shape: (n_states, n_targets)
+        yz: numpy.ndarray
+            The yz values for each x value, shape:
+            (n_states, n_targets, n_yz_per_target, 2)
 
         Returns
         -------
-        wake_deltas: dict
-            Keys: Variable name str, values: any
-        pdata: foxes.core.Data
-            The evaluation point data
+        wdeltas: dict
+            The wake deltas. Key: variable name str,
+            value: numpy.ndarray, shape: (n_st_sel, n_yz_per_target)
+        st_sel: numpy.ndarray of bool
+            The state-target selection, for which the wake
+            is non-zero, shape: (n_states, n_targets)
 
         """
-        points = self.get_wake_points(algo, mdata, fdata)
-        pdata = Data.from_points(points=points)
-
-        wake_deltas = {}
-        for w in self.wake_models:
-            w.init_wake_deltas(algo, mdata, fdata, pdata, wake_deltas)
+        pass
 
-        return wake_deltas, pdata
-
-    def contribute_to_wake_deltas(
+    def contribute(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
+        tdata,
+        downwind_index,
+        wake_coos,
         wake_deltas,
     ):
         """
-        Modifies wake deltas by contributions from the
-        specified wake source turbines.
+        Modifies wake deltas at target points by
+        contributions from the specified wake source turbines.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray of int
-            For each state, one turbine index corresponding
-            to the wake causing turbine. Shape: (n_states,)
-        wake_deltas: Any
-            The wake deltas object created by the
-            `new_wake_deltas` function
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        wake_coos: numpy.ndarray
+            The wake frame coordinates of the evaluation
+            points, shape: (n_states, n_targets, n_tpoints, 3)
+        wake_deltas: dict
+            The wake deltas. Key: variable name,
+            value: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints, ...)
 
         """
-        wcoos = self.wake_frame.get_wake_coos(
-            algo, mdata, fdata, pdata, states_source_turbine
+        # rounding for safe x > 0 conditions
+        x = np.round(wake_coos[:, :, 0, 0], 12)
+        yz = wake_coos[..., 1:3]
+
+        wdeltas, st_sel = self.calc_wakes_x_yz(
+            algo, mdata, fdata, tdata, downwind_index, x, yz
         )
 
-        for w in self.wake_models:
-            w.contribute_to_wake_deltas(
-                algo, mdata, fdata, pdata, states_source_turbine, wcoos, wake_deltas
+        for v, hdel in wdeltas.items():
+            try:
+                superp = self.superp[v]
+            except KeyError:
+                raise KeyError(
+                    f"Model '{self.name}': Missing wake superposition entry for variable '{v}', found {sorted(list(self.superp.keys()))}"
+                )
+
+            wake_deltas[v] = superp.add_wake(
+                algo,
+                mdata,
+                fdata,
+                tdata,
+                downwind_index,
+                st_sel,
+                v,
+                wake_deltas[v],
+                hdel,
             )
 
-    def evaluate_results(
+    def finalize_wake_deltas(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
+        amb_results,
         wake_deltas,
-        states_turbine,
-        amb_res=None,
     ):
         """
-        Updates the farm data according to the wake
-        deltas.
+        Finalize the wake calculation.
+
+        Modifies wake_deltas on the fly.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-            Modified in-place by this function
-        pdata: foxes.core.Data
-            The evaluation point data
-        wake_deltas: Any
-            The wake deltas object, created by the
-            `new_wake_deltas` function and filled
-            by `contribute_to_wake_deltas`
-        states_turbine: numpy.ndarray of int
-            For each state, the index of one turbine
-            for which to evaluate the wake deltas.
-            Shape: (n_states,)
-        amb_res: dict, optional
-            Ambient states results. Keys: var str, values:
-            numpy.ndarray of shape (n_states, n_points)
-
-        """
-        weights = algo.rotor_model.from_data_or_store(FC.RWEIGHTS, algo, mdata)
-        rpoints = algo.rotor_model.from_data_or_store(FC.RPOINTS, algo, mdata)
-        n_states, n_turbines, n_rpoints, __ = rpoints.shape
-
-        amb_res_in = amb_res is not None
-        if not amb_res_in:
-            amb_res = algo.rotor_model.from_data_or_store(
-                FC.AMB_RPOINT_RESULTS, algo, mdata
-            )
-
-        wres = {}
-        st_sel = (np.arange(n_states), states_turbine)
-        for v, ares in amb_res.items():
-            wres[v] = ares.reshape(n_states, n_turbines, n_rpoints)[st_sel]
-
-        wdel = {}
-        for v, d in wake_deltas.items():
-            wdel[v] = d.reshape(n_states, n_turbines, n_rpoints)[st_sel]
-        for w in self.wake_models:
-            w.finalize_wake_deltas(algo, mdata, fdata, pdata, wres, wdel)
-
-        for v in wres.keys():
-            if v in wake_deltas:
-                wres[v] += wdel[v]
-                if amb_res_in:
-                    amb_res[v][st_sel] = wres[v]
-            wres[v] = wres[v][:, None]
+        amb_results: dict
+            The ambient results, key: variable name str,
+            values: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints)
+        wake_deltas: dict
+            The wake deltas object at the selected target
+            turbines. Key: variable str, value: numpy.ndarray
+            with shape (n_states, n_targets, n_tpoints)
 
-        algo.rotor_model.eval_rpoint_results(
-            algo, mdata, fdata, wres, weights, states_turbine=states_turbine
-        )
+        """
+        for v, s in self.superp.items():
+            wake_deltas[v] = s.calc_final_wake_delta(
+                algo, mdata, fdata, v, amb_results[v], wake_deltas[v]
+            )
```

### Comparing `foxes-0.6.2/foxes/models/partial_wakes/top_hat.py` & `foxes-0.7/foxes/models/wake_frames/yawed_wakes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,289 +1,321 @@
 import numpy as np
 
-from foxes.core import PartialWakesModel, Data
-from foxes.models.wake_models.top_hat import TopHatWakeModel
-from foxes.utils.two_circles import calc_area
+from foxes.core import WakeFrame
+from foxes.models.wake_models.wind.bastankhah16 import (
+    Bastankhah2016Model,
+    Bastankhah2016,
+)
 import foxes.variables as FV
 import foxes.constants as FC
+from .rotor_wd import RotorWD
 
 
-class PartialTopHat(PartialWakesModel):
+class YawedWakes(WakeFrame):
     """
-    Partial wakes for top-hat models.
+    Bend the wakes for yawed turbines, based on the
+    Bastankhah 2016 wake model
 
-    The wake effect is weighted by the overlap of
-    the wake circle and the rotor disc circle.
+    Notes
+    -----
+    Reference:
+    "Experimental and theoretical study of wind turbine wakes in yawed conditions"
+    Majid Bastankhah, Fernando Porté-Agel
+    https://doi.org/10.1017/jfm.2016.595
 
     Attributes
     ----------
-    rotor_model: foxes.core.RotorModel
-        The rotor model, default is the one from the algorithm
+    model: Bastankhah2016Model
+        The model for computing common data
+    model_pars: dict
+        Model parameters
+    K: float
+        The wake growth parameter k. If not given here
+        it will be searched in the farm data.
+    YAWM: float
+        The yaw misalignment YAWM. If not given here
+        it will be searched in the farm data.
+    base_frame: foxes.core.WakeFrame
+        The wake frame from which to start
+    k_var: str
+        The variable name for k
 
-    :group: models.partial_wakes
+    :group: models.wake_frames
 
     """
 
-    def __init__(self, wake_models=None, wake_frame=None, rotor_model=None):
+    def __init__(
+        self,
+        k=None,
+        base_frame=RotorWD(),
+        k_var=FV.K,
+        **kwargs,
+    ):
         """
         Constructor.
 
         Parameters
         ----------
-        wake_models: list of foxes.core.WakeModel, optional
-            The wake models, default are the ones from the algorithm
-        wake_frame: foxes.core.WakeFrame, optional
-            The wake frame, default is the one from the algorithm
-        rotor_model: foxes.core.RotorModel, optional
-            The rotor model, default is the one from the algorithm
+        k: float, optional
+            The wake growth parameter k. If not given here
+            it will be searched in the farm data, by default None
+        base_frame: foxes.core.WakeFrame
+            The wake frame from which to start
+        k_var: str
+            The variable name for k
+        kwargs: dict, optional
+            Additional parameters for the Bastankhah2016Model,
+            if not found in wake model
+
+        """
+        super().__init__()
+
+        self.base_frame = base_frame
+        self.model = None
+        self.model_pars = kwargs
+        self.k_var = k_var
+
+        setattr(self, k_var, k)
+        setattr(self, FV.YAWM, 0.0)
+
+    def __repr__(self):
+        k = getattr(self, self.k_var)
+        s = f"{type(self).__name__}("
+        if k is None:
+            s += f"k_var={self.k_var}"
+        else:
+            s += f"{self.k_var}={k}"
+        s += ")"
+        return s
 
+    def sub_models(self):
         """
-        super().__init__(wake_models, wake_frame)
-        self.rotor_model = rotor_model
+        List of all sub-models
 
-    def initialize(self, algo, verbosity=0):
+        Returns
+        -------
+        smdls: list of foxes.core.Model
+            Names of all sub models
+
+        """
+        return [self.base_frame, self.model]
+
+    def initialize(self, algo, verbosity=0, force=False):
         """
         Initializes the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         verbosity: int
             The verbosity level, 0 = silent
+        force: bool
+            Overwrite existing data
 
         """
-        if self.rotor_model is None:
-            self.rotor_model = algo.rotor_model
-
-        super().initialize(algo, verbosity)
-
-        for w in self.wake_models:
-            if not isinstance(w, TopHatWakeModel):
-                raise TypeError(
-                    f"Partial wakes '{self.name}': Cannot be applied to wake model '{w.name}', since not a TopHatWakeModel"
-                )
-
-        self.WCOOS_ID = self.var("WCOOS_ID")
-        self.WCOOS_X = self.var("WCOOS_X")
-        self.WCOOS_R = self.var("WCOOS_R")
-
-    def sub_models(self):
-        """
-        List of all sub-models
+        if not self.initialized:
+            for w in algo.wake_models:
+                if isinstance(w, Bastankhah2016):
+                    if not w.initialized:
+                        w.initialize(algo, verbosity, force)
+                    self.model = w.model
+                    if w.k_var == self.k_var:
+                        setattr(self, self.k_var, getattr(w, self.k_var))
+            if self.model is None:
+                self.model = Bastankhah2016Model(**self.model_pars)
+            if self.k is None:
+                for w in algo.wake_models:
+                    if hasattr(w, "k_var") and w.k_var == self.k_var:
+                        setattr(self, self.k_var, getattr(w, self.k_var))
+                        break
+
+        super().initialize(algo, verbosity, force)
+
+    def calc_order(self, algo, mdata, fdata):
+        """ "
+        Calculates the order of turbine evaluation.
 
-        Returns
-        -------
-        smdls: list of foxes.core.Model
-            Names of all sub models
-
-        """
-        return super().sub_models() + [self.rotor_model]
-
-    def new_wake_deltas(self, algo, mdata, fdata):
-        """
-        Creates new initial wake deltas, filled
-        with zeros.
+        This function is executed on a single chunk of data,
+        all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
 
         Returns
         -------
-        wake_deltas: dict
-            Keys: Variable name str, values: any
-        pdata: foxes.core.Data
-            The evaluation point data
+        order: numpy.ndarray
+            The turbine order, shape: (n_states, n_turbines)
 
         """
-        pdata = Data.from_points(points=fdata[FV.TXYH])
+        return self.base_frame.calc_order(algo, mdata, fdata)
 
-        wake_deltas = {}
-        for w in self.wake_models:
-            w.init_wake_deltas(algo, mdata, fdata, pdata, wake_deltas)
+    def _update_y(self, algo, mdata, fdata, tdata, downwind_index, x, y):
+        """
+        Helper function for y deflection
+        """
 
-        return wake_deltas, pdata
+        # get gamma:
+        gamma = self.get_data(
+            FV.YAWM,
+            FC.STATE_TARGET,
+            lookup="wfs",
+            algo=algo,
+            fdata=fdata,
+            tdata=tdata,
+            upcast=True,
+            downwind_index=downwind_index,
+            accept_nan=False,
+        )
+        gamma *= np.pi / 180
 
-    def contribute_to_wake_deltas(
+        # get k:
+        k = self.get_data(
+            self.k_var,
+            FC.STATE_TARGET,
+            lookup="sf",
+            algo=algo,
+            fdata=fdata,
+            tdata=tdata,
+            upcast=True,
+            downwind_index=downwind_index,
+            accept_nan=False,
+        )
+
+        # run model calculation:
+        self.model.calc_data(algo, mdata, fdata, tdata, downwind_index, x, gamma, k)
+
+        # select targets:
+        st_sel = self.model.get_data(Bastankhah2016Model.ST_SEL, mdata)
+        if np.any(st_sel):
+            # prepare:
+            n_st_sel = np.sum(st_sel)
+            ydef = np.zeros((n_st_sel,), dtype=FC.DTYPE)
+
+            # collect data:
+            near = self.model.get_data(Bastankhah2016Model.NEAR, mdata)
+            far = ~near
+
+            # near wake:
+            if np.any(near):
+                # collect data:
+                delta = self.model.get_data(Bastankhah2016Model.DELTA_NEAR, mdata)
+
+                # set deflection:
+                ydef[near] = delta
+
+            # far wake:
+            if np.any(far):
+                # collect data:
+                delta = self.model.get_data(Bastankhah2016Model.DELTA_FAR, mdata)
+
+                # set deflection:
+                ydef[far] = delta
+
+            # apply deflection:
+            y[st_sel] -= ydef
+
+    def get_wake_coos(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        wake_deltas,
+        tdata,
+        downwind_index,
     ):
         """
-        Modifies wake deltas by contributions from the
-        specified wake source turbines.
+        Calculate wake coordinates of rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray of int
-            For each state, one turbine index corresponding
-            to the wake causing turbine. Shape: (n_states,)
-        wake_deltas: Any
-            The wake deltas object created by the
-            `new_wake_deltas` function
-
-        """
-        n_states = mdata.n_states
-        n_points = fdata.n_turbines
-        stsel = (np.arange(n_states), states_source_turbine)
-
-        if (
-            self.WCOOS_ID not in mdata
-            or mdata[self.WCOOS_ID] != states_source_turbine[0]
-        ):
-            wcoos = self.wake_frame.get_wake_coos(
-                algo, mdata, fdata, pdata, states_source_turbine
-            )
-            mdata[self.WCOOS_ID] = states_source_turbine[0]
-            mdata[self.WCOOS_X] = wcoos[:, :, 0]
-            mdata[self.WCOOS_R] = np.linalg.norm(wcoos[:, :, 1:3], axis=-1)
-            wcoos[:, :, 1:3] = 0
-        else:
-            wcoos = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-            wcoos[:, :, 0] = mdata[self.WCOOS_X]
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
 
-        ct = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        ct[:] = fdata[FV.CT][stsel][:, None]
-        x = mdata[self.WCOOS_X]
-
-        sel0 = (ct > 0.0) & (x > 0.0)
-        if np.any(sel0):
-            R = mdata[self.WCOOS_R]
-            r = np.zeros_like(R)
-            D = fdata[FV.D]
-
-            for w in self.wake_models:
-                wr = w.calc_wake_radius(
-                    algo, mdata, fdata, pdata, states_source_turbine, x, ct
-                )
-
-                sel_sp = sel0 & (wr > R - D / 2)
-                if np.any(sel_sp):
-                    hx = x[sel_sp]
-                    hct = ct[sel_sp]
-                    hwr = wr[sel_sp]
-
-                    clw = w.calc_centreline_wake_deltas(
-                        algo,
-                        mdata,
-                        fdata,
-                        pdata,
-                        states_source_turbine,
-                        sel_sp,
-                        hx,
-                        hwr,
-                        hct,
-                    )
-                    del hx, hct
-
-                    hR = R[sel_sp]
-                    hD = D[sel_sp]
-                    weights = calc_area(hD / 2, hwr, hR) / (np.pi * (hD / 2) ** 2)
-                    del hD, hwr, hR
-
-                    for v, d in clw.items():
-                        try:
-                            superp = w.superp[v]
-                        except KeyError:
-                            raise KeyError(
-                                f"Model '{self.name}': Missing wake superposition entry for variable '{v}' in wake model '{w.name}', found {sorted(list(w.superp.keys()))}"
-                            )
-
-                        wake_deltas[v] = superp.calc_wakes_plus_wake(
-                            algo,
-                            mdata,
-                            fdata,
-                            pdata,
-                            states_source_turbine,
-                            sel_sp,
-                            v,
-                            wake_deltas[v],
-                            weights * d,
-                        )
+        Returns
+        -------
+        wake_coos: numpy.ndarray
+            The wake frame coordinates of the evaluation
+            points, shape: (n_states, n_targets, n_tpoints, 3)
 
-    def evaluate_results(
-        self,
-        algo,
-        mdata,
-        fdata,
-        pdata,
-        wake_deltas,
-        states_turbine,
-        amb_res=None,
-    ):
         """
-        Updates the farm data according to the wake
-        deltas.
+        # get unyawed results:
+        xyz = self.base_frame.get_wake_coos(
+            algo,
+            mdata,
+            fdata,
+            tdata,
+            downwind_index,
+        )
+
+        # take rotor average:
+        xy = np.einsum("stpd,p->std", xyz[..., :2], tdata[FC.TWEIGHTS])
+        x = xy[:, :, 0]
+        y = xy[:, :, 1]
+
+        # apply deflection:
+        self._update_y(algo, mdata, fdata, tdata, downwind_index, x, y)
+        xyz[..., 1] = y[:, :, None]
+
+        return xyz
+
+    def get_centreline_points(self, algo, mdata, fdata, downwind_index, x):
+        """
+        Gets the points along the centreline for given
+        values of x.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-            Modified in-place by this function
-        pdata: foxes.core.Data
-            The evaluation point data
-        wake_deltas: Any
-            The wake deltas object, created by the
-            `new_wake_deltas` function and filled
-            by `contribute_to_wake_deltas`
-        states_turbine: numpy.ndarray of int
-            For each state, the index of one turbine
-            for which to evaluate the wake deltas.
-            Shape: (n_states,)
-        amb_res: dict, optional
-            Ambient states results. Keys: var str, values:
-            numpy.ndarray of shape (n_states, n_points)
-
-        """
-        weights = algo.rotor_model.from_data_or_store(FC.RWEIGHTS, algo, mdata)
-        rpoints = algo.rotor_model.from_data_or_store(FC.RPOINTS, algo, mdata)
-        n_states, n_turbines, n_rpoints, __ = rpoints.shape
-
-        amb_res_in = amb_res is not None
-        if not amb_res_in:
-            amb_res = algo.rotor_model.from_data_or_store(
-                FC.AMB_RPOINT_RESULTS, algo, mdata
-            )
-
-        wres = {}
-        st_sel = (np.arange(n_states), states_turbine)
-        for v, ares in amb_res.items():
-            wres[v] = ares.reshape(n_states, n_turbines, n_rpoints)[st_sel]
-
-        wdel = {}
-        for v, d in wake_deltas.items():
-            wdel[v] = d.reshape(n_states, n_turbines, 1)[st_sel]
-        for w in self.wake_models:
-            w.finalize_wake_deltas(algo, mdata, fdata, pdata, wres, wdel)
-
-        for v in wres.keys():
-            if v in wake_deltas:
-                wres[v] += wdel[v]
-                if amb_res_in:
-                    amb_res[v][st_sel] = wres[v]
-            wres[v] = wres[v][:, None]
+        downwind_index: int
+            The index in the downwind order
+        x: numpy.ndarray
+            The wake frame x coordinates, shape: (n_states, n_points)
+
+        Returns
+        -------
+        points: numpy.ndarray
+            The centreline points, shape: (n_states, n_points, 3)
 
-        self.rotor_model.eval_rpoint_results(
-            algo, mdata, fdata, wres, weights, states_turbine=states_turbine
+        """
+        points = self.base_frame.get_centreline_points(
+            algo, mdata, fdata, downwind_index, x
+        )
+
+        nx = np.zeros_like(points)
+        nx[:, 0] = points[:, 1] - points[:, 0]
+        nx[:, -1] = points[:, -1] - points[:, -2]
+        nx[:, 1:-1] = 0.5 * (points[:, 1:-1] - points[:, :-2]) + 0.5 * (
+            points[:, 2:] - points[:, 1:-1]
         )
+        nx /= np.linalg.norm(nx, axis=-1)[:, :, None]
+
+        nz = np.zeros_like(nx)
+        nz[:, :, 2] = 1
+        ny = np.cross(nz, nx, axis=-1)
+        del nx, nz
+
+        y = np.zeros_like(x)
+        self._update_y(algo, mdata, fdata, None, downwind_index, x, y)
+
+        points += y[:, :, None] * ny
+
+        return points
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `foxes-0.6.2/foxes/models/point_models/set_uniform_data.py` & `foxes-0.7/foxes/models/point_models/set_uniform_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,20 +125,20 @@
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The point data
+        tdata: foxes.core.TData
+            The target point data
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
```

### Comparing `foxes-0.6.2/foxes/models/point_models/tke2ti.py` & `foxes-0.7/foxes/models/point_models/tke2ti.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,20 +36,20 @@
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The point data
+        tdata: foxes.core.TData
+            The target point data
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
```

### Comparing `foxes-0.6.2/foxes/models/point_models/wake_deltas.py` & `foxes-0.7/foxes/models/turbine_models/yaw2yawm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,65 @@
-from foxes.core import PointDataModel
+from foxes.core import TurbineModel
 import foxes.variables as FV
+import foxes.constants as FC
+from foxes.utils import delta_wd
 
 
-class WakeDeltas(PointDataModel):
+class YAW2YAWM(TurbineModel):
     """
-    This point model simply subtracts ambient results
-    from waked results.
+    Calculates delta yaw (i.e. YAWM) from absolute
+    yaw (i.e. YAW)
 
-    Attributes
-    ----------
-    vars: list of str
-        The variables
-    normalize: bool
-        Divide resulting deltas by ambient values
-
-    :group: models.point_models
+    :group: models.turbine_models
 
     """
 
-    def __init__(self, vars, normalize=False):
-        """
-        Constructor.
-
-        Parameters
-        ----------
-        vars: list of str
-            The variables
-        normalize: bool
-            Divide resulting deltas by ambient values
-
-        """
-        super().__init__()
-        self.vars = vars
-        self.normalize = normalize
-
-    def output_point_vars(self, algo):
+    def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
         output_vars: list of str
             The output variable names
 
         """
-        return [f"DELTA_{v}" for v in self.vars]
+        return [FV.YAWM]
 
-    def calculate(self, algo, mdata, fdata, pdata):
-        """ "
+    def calculate(self, algo, mdata, fdata, st_sel):
+        """
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The point data
+        st_sel: slice or numpy.ndarray of bool
+            The state-turbine selection,
+            for shape: (n_states, n_turbines)
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_points)
+            Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
+        yaw = fdata[FV.YAW][st_sel]
+        wd = fdata[FV.WD][st_sel]
 
-        out = {f"DELTA_{v}": pdata[v] - pdata[FV.var2amb[v]] for v in self.vars}
-
-        if self.normalize:
-            for v in self.vars:
-                out[v] /= pdata[FV.var2amb[v]]
+        yawm = fdata[FV.YAWM]
+        yawm[st_sel] = delta_wd(wd, yaw)
 
-        return out
+        return {FV.YAWM: yawm}
```

### Comparing `foxes-0.6.2/foxes/models/rotor_models/centre.py` & `foxes-0.7/foxes/models/rotor_models/centre.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,17 +65,17 @@
         """
         Calculates rotor points from design points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
 
         Returns
         -------
         points: numpy.ndarray
             The rotor points, shape:
             (n_states, n_turbines, n_rpoints, 3)
@@ -86,15 +86,15 @@
     def eval_rpoint_results(
         self,
         algo,
         mdata,
         fdata,
         rpoint_results,
         weights,
-        states_turbine=None,
+        downwind_index=None,
         copy_to_ambient=False,
     ):
         """
         Evaluate rotor point results.
 
         This function modifies `fdata`, either
         for all turbines or one turbine per state,
@@ -102,44 +102,40 @@
         the latter case, the turbine dimension of the
         `rpoint_results` is expected to have size one.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
         rpoint_results: dict
             The results at rotor points. Keys: variable str.
             Values: numpy.ndarray, shape if `states_turbine`
             is None: (n_states, n_turbines, n_rpoints).
             Else: (n_states, 1, n_rpoints)
         weights: numpy.ndarray
             The rotor point weights, shape: (n_rpoints,)
-        states_turbine: numpy.ndarray of int, optional
-            The turbine indices, one per state. Shape: (n_states,)
-        copy_to_ambient: bool, optional
+        downwind_index: int, optional
+            The index in the downwind order
+        copy_to_ambient: bool
             If `True`, the fdata results are copied to ambient
             variables after calculation
 
         """
         if len(weights) > 1:
             return super().eval_rpoint_results(
-                algo, mdata, fdata, rpoint_results, weights, states_turbine
+                algo, mdata, fdata, rpoint_results, weights, downwind_index
             )
 
         n_states = mdata.n_states
         n_turbines = algo.n_turbines
 
-        stsel = None
-        if states_turbine is not None:
-            stsel = (np.arange(n_states), states_turbine)
-
         uvp = None
         uv = None
         if (
             FV.WS in self.calc_vars
             or FV.WD in self.calc_vars
             or FV.YAW in self.calc_vars
             or FV.REWS in self.calc_vars
@@ -156,45 +152,45 @@
         for v in self.calc_vars:
             if v not in fdata:
                 fdata[v] = np.zeros((n_states, n_turbines), dtype=FC.DTYPE)
 
             if v == FV.WD or v == FV.YAW:
                 if wd is None:
                     wd = uv2wd(uv, axis=-1)
-                self._set_res(fdata, v, wd, stsel)
+                self._set_res(fdata, v, wd, downwind_index)
                 vdone.append(v)
 
             elif v == FV.WS:
-                self._set_res(fdata, v, ws[:, :, 0], stsel)
+                self._set_res(fdata, v, ws[:, :, 0], downwind_index)
                 del ws
                 vdone.append(v)
         del uv, wd
 
         if (
             FV.REWS in self.calc_vars
             or FV.REWS2 in self.calc_vars
             or FV.REWS3 in self.calc_vars
         ):
-            if stsel is None:
+            if downwind_index is None:
                 yaw = fdata[FV.YAW]
             else:
-                yaw = fdata[FV.YAW][stsel][:, None]
+                yaw = fdata[FV.YAW][:, downwind_index, None]
             nax = wd2uv(yaw, axis=-1)
             wsp = np.einsum("stpd,std->stp", uvp, nax)
 
             for v in self.calc_vars:
                 if v == FV.REWS or v == FV.REWS2 or v == FV.REWS3:
                     rews = wsp[:, :, 0]
-                    self._set_res(fdata, v, rews, stsel)
+                    self._set_res(fdata, v, rews, downwind_index)
                     del rews
                     vdone.append(v)
 
             del wsp
         del uvp
 
         for v in self.calc_vars:
             if v not in vdone:
                 res = rpoint_results[v][:, :, 0]
-                self._set_res(fdata, v, res, stsel)
+                self._set_res(fdata, v, res, downwind_index)
                 del res
             if copy_to_ambient and v in FV.var2amb:
                 fdata[FV.var2amb[v]] = fdata[v].copy()
```

### Comparing `foxes-0.6.2/foxes/models/rotor_models/grid.py` & `foxes-0.7/foxes/models/rotor_models/grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,16 @@
         super().__init__(calc_vars)
 
         self.n = n
         self.reduce = reduce
         self.nint = nint
 
     def __repr__(self):
-        return super().__repr__() + f"(n={self.n})"
+        r = "" if self.reduce else ", reduce=False"
+        return f"{type(self).__name__}(n={self.n}){r}"
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         Parameters
         ----------
```

### Comparing `foxes-0.6.2/foxes/models/rotor_models/levels.py` & `foxes-0.7/foxes/models/rotor_models/levels.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,16 @@
         super().__init__(calc_vars)
 
         self.n = n
         self.reduce = reduce
         self.nint = nint
 
     def __repr__(self):
-        return super().__repr__() + f"(n={self.n})"
+        r = "" if self.reduce else ", reduce=False"
+        return f"{type(self).__name__}(n={self.n}){r}"
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         Parameters
         ----------
```

### Comparing `foxes-0.6.2/foxes/models/turbine_models/calculator.py` & `foxes-0.7/foxes/models/turbine_models/calculator.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     in_vars: list of str
         The input farm vairables
     out_vars: list of str
         The output variables
     func: Function
         The function: f(in0, in1, ..., stsel) -> (out0, ou1, ...)
         where inX and outY are numpy.ndarrays and
-        st_sel is the boolean state-turbine selection.
+        st_sel is the state-turbine selection slice or array.
         All arrays have shape (n_states, n_turbines).
 
     :group: models.turbine_models
 
     """
 
     def __init__(self, in_vars, out_vars, func, **kwargs):
@@ -32,25 +32,29 @@
         in_vars: list of str
             The input farm vairables
         out_vars: list of str
             The output variables
         func: Function
             The function: f(in0, in1, ..., stsel) -> (out0, ou1, ...)
             where inX and outY are numpy.ndarrays and
-            st_sel is the boolean state-turbine selection.
+            st_sel is the state-turbine selection slice or array.
             All arrays have shape (n_states, n_turbines).
         kwargs: dict, optional
             Additional arguments for TurbineModel
 
         """
         super().__init__(**kwargs)
         self.in_vars = in_vars
         self.out_vars = out_vars
         self.func = func
 
+    def __repr__(self):
+        a = f"{self.in_vars}, {self.out_vars}"
+        return f"{type(self).__name__}({a})"
+
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
@@ -61,31 +65,31 @@
         output_vars: list of str
             The output variable names
 
         """
         return self.out_vars
 
     def calculate(self, algo, mdata, fdata, st_sel):
-        """ "
+        """
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        st_sel: numpy.ndarray of bool
+        st_sel: slice or numpy.ndarray of bool
             The state-turbine selection,
-            shape: (n_states, n_turbines)
+            for shape: (n_states, n_turbines)
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
```

### Comparing `foxes-0.6.2/foxes/models/turbine_models/kTI_model.py` & `foxes-0.7/foxes/models/turbine_models/kTI_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,18 +47,20 @@
         self.ti_var = ti_var
         self.k_var = k_var
         setattr(self, ti_var, ti_val)
         setattr(self, FV.KTI, kTI)
         setattr(self, FV.KB, 0 if kb is None else kb)
 
     def __repr__(self):
-        return (
-            super().__repr__()
-            + f"({self.k_var}, kTI={getattr(self, FV.KTI)}, ti={self.ti_var})"
-        )
+        kti = getattr(self, FV.KTI)
+        kb = getattr(self, FV.KB)
+        ti = getattr(self, self.ti_var)
+        tiv = f", ti_val={ti}" if ti is not None else ""
+        a = f"kTI={kti}, kb={kb}, ti_var={self.ti_var}{tiv}, k_var={self.k_var}"
+        return f"{type(self).__name__}({a})"
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
@@ -70,49 +72,49 @@
         output_vars: list of str
             The output variable names
 
         """
         return [self.k_var]
 
     def calculate(self, algo, mdata, fdata, st_sel):
-        """ "
+        """
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        st_sel: numpy.ndarray of bool
+        st_sel: slice or numpy.ndarray of bool
             The state-turbine selection,
-            shape: (n_states, n_turbines)
+            for shape: (n_states, n_turbines)
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
-        kTI = self.get_data(
+        kti = self.get_data(
             FV.KTI, FC.STATE_TURBINE, lookup="sf", fdata=fdata, upcast=True
         )[st_sel]
         kb = self.get_data(
             FV.KB, FC.STATE_TURBINE, lookup="sf", fdata=fdata, upcast=True
         )[st_sel]
         ti = self.get_data(
             self.ti_var, FC.STATE_TURBINE, lookup="sf", fdata=fdata, upcast=True
         )[st_sel]
 
         k = fdata.get(
             self.k_var, np.zeros((fdata.n_states, fdata.n_turbines), dtype=FC.DTYPE)
         )
 
-        k[st_sel] = kTI * ti + kb
+        k[st_sel] = kti * ti + kb
 
         return {self.k_var: k}
```

### Comparing `foxes-0.6.2/foxes/models/turbine_models/lookup_table.py` & `foxes-0.7/foxes/models/turbine_models/lookup_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,48 +153,61 @@
                 print()
                 print(self._data)
                 print()
 
         return super().load_data(algo, verbosity)
 
     def calculate(self, algo, mdata, fdata, st_sel):
-        """ "
+        """
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        st_sel: numpy.ndarray of bool
+        st_sel: slice or numpy.ndarray of bool
             The state-turbine selection,
-            shape: (n_states, n_turbines)
+            for shape: (n_states, n_turbines)
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
+        data = {
+            v: self.get_data(
+                self.input_vars[0],
+                FC.STATE_TURBINE,
+                lookup="fs",
+                fdata=fdata,
+                upcast=True,
+            )[st_sel]
+            for v in self.input_vars
+        }
+        dims = {
+            v: ("_z") if len(data[v].shape) == 1 else ("_z", "_u")
+            for v in self.input_vars
+        }
         indata = {
             v: xr.DataArray(
-                self.get_data(
-                    v, FC.STATE_TURBINE, lookup="fs", fdata=fdata, upcast=True
-                )[st_sel],
-                dims=["_z"],
+                data[v],
+                dims=dims[v],
             )
             for v in self.input_vars
         }
+        del data, dims
 
         odata = self._data.interp(**indata, **self._xargs)
 
         out = {}
         for v in self.output_vars:
             out[v] = fdata[v]
             out[v][st_sel] = odata[v]
```

### Comparing `foxes-0.6.2/foxes/models/turbine_models/power_mask.py` & `foxes-0.7/foxes/models/turbine_models/table_factors.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,80 @@
 import numpy as np
+import pandas as pd
+from scipy.interpolate import interpn
 
 from foxes.core import TurbineModel
-import foxes.variables as FV
+from foxes.utils import PandasFileHelper
 import foxes.constants as FC
-from foxes.utils import cubic_roots
 
 
-class PowerMask(TurbineModel):
+class TableFactors(TurbineModel):
     """
-    Invokes a maximal power value.
+    Multiplies variables by factors from a
+    two dimensional table.
 
-    This may correspond to turbine derating, if
-    the maximal power value is below rated power.
-    For higher values, a boost is introduced.
-
-    The model updates the P and CT variables,
-    so it is wise to use it after calling the
-    turbine type model.
+    The column names are expected to be numbers
+    that represent the col_var variable.
 
     Attributes
     ----------
-    var_ws_P: str
-        The wind speed variable for power lookup
-    factor_P: float
-        The power unit factor, e.g. 1000 for kW
+    data_source: str or pandas.DataFrame
+        Either path to a file or data
+    row_var: str
+        The row-wise variable
+    col_var: str
+        The column-wise variable
+    ovars: list of str
+        The variables onto which the factors
+        are multiplied
 
     :group: models.turbine_models
 
     """
 
-    def __init__(self, var_ws_P=FV.REWS3, factor_P=1.0e3):
+    def __init__(
+        self,
+        data_source,
+        row_var,
+        col_var,
+        output_vars,
+        pd_file_read_pars={},
+        **ipars,
+    ):
         """
         Constructor.
 
         Parameters
         ----------
-        var_ws_P: str
-            The wind speed variable for power lookup
-        factor_P: float
-            The power unit factor, e.g. 1000 for kW
+        data_source: str or pandas.DataFrame
+            Either path to a file or data
+        row_var: str
+            The row-wise variable
+        col_var: str
+            The column-wise variable
+        output_vars: list of str
+            The variables onto which the factors
+            are multiplied
+        pd_file_read_pars: dict
+            Parameters for pandas file reading
+        ipars: dict, optional
+            Parameters for scipy.interpolate.interpn
 
         """
         super().__init__()
 
-        self.var_ws_P = var_ws_P
-        self.factor_P = factor_P
+        self.data_source = data_source
+        self.row_var = row_var
+        self.col_var = col_var
+        self.ovars = output_vars
+        self._rpars = pd_file_read_pars
+        self._ipars = ipars
+
+        self._cvals = None
+        self._data = None
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
@@ -57,15 +83,15 @@
 
         Returns
         -------
         output_vars: list of str
             The output variable names
 
         """
-        return [FV.P, FV.CT]
+        return self.ovars
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         Parameters
         ----------
@@ -73,100 +99,69 @@
             The calculation algorithm
         verbosity: int
             The verbosity level, 0 = silent
 
         """
         super().initialize(algo, verbosity)
 
-        self._P_rated = []
-        for t in algo.farm_controller.turbine_types:
-            Pnom = FC.DTYPE(t.P_nominal)
-            if np.isnan(Pnom):
-                raise ValueError(
-                    f"Model '{self.name}': P_nominal is NaN for turbine type '{t.name}'"
-                )
-            self._P_rated.append(Pnom)
-        self._P_rated = np.array(self._P_rated, dtype=FC.DTYPE)
-
-    @classmethod
-    def update_P_ct(cls, data, max_P, rated_P, factor_P, var_ws=FV.REWS3, P_lim=100):
-        # select power entries for which this is active:
-        P = data[FV.P]
-        sel = ~np.isnan(max_P) & (
-            ((max_P < rated_P) & (P > max_P))
-            | ((max_P > rated_P) & (P > rated_P - P_lim))
-        )
-        if np.any(sel):
-            # apply selection:
-            max_P = max_P[sel]
-            ws = data[var_ws][sel]
-            rho = data[FV.RHO][sel]
-            r = data[FV.D][sel] / 2
-            P = P[sel]
-            ct = data[FV.CT][sel]
-            ct[ct > 1.0] = 1.0
-
-            # calculate power efficiency e of turbine
-            # e is the ratio of the cp derived from the power curve
-            # and the theoretical cp from the turbine induction
-            cp = P / (0.5 * ws**3 * rho * np.pi * r**2) * factor_P
-            a = 0.5 * (1 - np.sqrt(1 - ct))
-            cp_a = 4 * a**3 - 8 * a**2 + 4 * a
-            e = cp / cp_a
-            del cp, a, cp_a, ct, P
-
-            # calculating new cp for changed power
-            cp = max_P / (0.5 * ws**3 * rho * np.pi * r**2) * factor_P
-
-            # find roots:
-            N = len(cp)
-            a3 = np.full(N, 4.0, dtype=FC.DTYPE)
-            a2 = np.full(N, -8.0, dtype=FC.DTYPE)
-            a1 = np.full(N, 4.0, dtype=FC.DTYPE)
-            a0 = -cp / e
-            rts = cubic_roots(a0, a1, a2, a3)
-            rts[np.isnan(rts)] = np.inf
-            rts[rts <= 0.0] = np.inf
-            a = np.min(rts, axis=1)
-            del a0, a1, a2, a3, rts
-
-            # set results:
-            P = data[FV.P]
-            ct = data[FV.CT]
-            P[sel] = max_P
-            ct[sel] = 4 * a * (1 - a)
+        if isinstance(self.data_source, pd.DataFrame):
+            self._data = self.data_source
+        else:
+            if verbosity > 0:
+                print(f"{self.name}: Reading file {self.data_source}")
+            rpars = dict(index_col=0)
+            rpars.update(self._rpars)
+            self._data = PandasFileHelper.read_file(self.data_source, **rpars)
+
+        self._rvals = self._data.index.to_numpy(FC.DTYPE)
+        self._cvals = self._data.columns.to_numpy(FC.DTYPE)
+        self._data = self._data.to_numpy(FC.DTYPE)
 
     def calculate(self, algo, mdata, fdata, st_sel):
-        """ "
+        """
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        st_sel: numpy.ndarray of bool
+        st_sel: slice or numpy.ndarray of bool
             The state-turbine selection,
-            shape: (n_states, n_turbines)
+            for shape: (n_states, n_turbines)
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
+        n_sel = np.sum(st_sel)
+        qts = np.zeros((n_sel, 2), dtype=FC.DTYPE)
+        qts[:, 0] = fdata[self.row_var][st_sel]
+        qts[:, 1] = fdata[self.col_var][st_sel]
+
+        try:
+            factors = interpn(
+                (self._rvals, self._cvals), self._data, qts, **self._ipars
+            )
+        except ValueError as e:
+            print(f"\nDATA       : ({self.row_var}, {self.col_var})")
+            print(
+                f"DATA BOUNDS: ({np.min(self._rvals)}, {np.min(self._cvals)}) -- ({np.max(self._rvals)}, {np.max(self._cvals)})"
+            )
+            print(
+                f"VALUE BOUNDS: ({np.min(qts[:, 0]):.4f}, {np.min(qts[:, 1]):.4f}) -- ({np.max(qts[:, 0]):.4f}, {np.max(qts[:, 1]):.4f})\n"
+            )
+            raise e
 
-        # prepare:
-        max_P = fdata[FV.MAX_P]
-        rated_P = self._P_rated[None, :]
-
-        # calculate:
-        self.update_P_ct(fdata, max_P, rated_P, self.factor_P, var_ws=self.var_ws_P)
+        for v in self.output_farm_vars(algo):
+            fdata[v][st_sel] *= factors
 
-        return {FV.P: fdata[FV.P], FV.CT: fdata[FV.CT]}
+        return {v: fdata[v] for v in self.output_farm_vars(algo)}
```

### Comparing `foxes-0.6.2/foxes/models/turbine_models/rotor_centre_calc.py` & `foxes-0.7/foxes/opt/objectives/max_n_turbines.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,139 +1,142 @@
 import numpy as np
 
-from foxes.core import TurbineModel, Data
-import foxes.variables as FV
+from foxes.opt.core.farm_objective import FarmObjective
 import foxes.constants as FC
 
 
-class RotorCentreCalc(TurbineModel):
+class MaxNTurbines(FarmObjective):
     """
-    Calculates data at the rotor centre
+    Maximizes the number of turrbines.
 
     Attributes
     ----------
-    calc_vars: dict
-        The variables that are calculated by the model,
-        keys: var names, values: rotor var names
+    check_valid: bool
+        Check FC.VALID variable before counting
 
-    :group: models.turbine_models
+    :group: opt.objectives
 
     """
 
-    def __init__(self, calc_vars):
+    def __init__(
+        self,
+        problem,
+        name="max_n_turbines",
+        check_valid=True,
+        **kwargs,
+    ):
         """
         Constructor.
 
         Parameters
         ----------
-        calc_vars: dict
-            The variables that are calculated by the model,
-            keys: var names, values: rotor var names
+        problem: foxes.opt.FarmOptProblem
+            The underlying optimization problem
+        name: str
+            The name of the objective function
+        check_valid: bool
+            Check FC.VALID variable before counting
+        kwargs: dict, optional
+            Additional parameters for `FarmObjective`
 
         """
-        super().__init__()
+        super().__init__(problem, name, **kwargs)
+        self.check_valid = check_valid
 
-        if isinstance(calc_vars, dict):
-            self.calc_vars = calc_vars
-        else:
-            self.calc_vars = {v: v for v in calc_vars}
-
-    def initialize(self, algo, verbosity=0):
+    def n_components(self):
         """
-        Initializes the model.
+        Returns the number of components of the
+        function.
 
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
+        Returns
+        -------
+        int:
+            The number of components.
 
         """
-        self._wcalc = algo.get_model("PointWakesCalculation")()
-        super().initialize(algo, verbosity)
+        return 1
 
-    def sub_models(self):
+    def maximize(self):
         """
-        List of all sub-models
+        Returns flag for maximization of each component.
 
         Returns
         -------
-        smdls: list of foxes.core.Model
-            Names of all sub models
+        flags: np.array
+            Bool array for component maximization,
+            shape: (n_components,)
 
         """
-        return [self._wcalc]
+        return [True]
 
-    def output_farm_vars(self, algo):
+    def calc_individual(self, vars_int, vars_float, problem_results, components=None):
         """
-        The variables which are being modified by the model.
+        Calculate values for a single individual of the
+        underlying problem.
 
         Parameters
         ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
+        vars_int: np.array
+            The integer variable values, shape: (n_vars_int,)
+        vars_float: np.array
+            The float variable values, shape: (n_vars_float,)
+        problem_results: Any
+            The results of the variable application
+            to the problem
+        components: list of int, optional
+            The selected components or None for all
 
         Returns
         -------
-        output_vars: list of str
-            The output variable names
+        values: np.array
+            The component values, shape: (n_sel_components,)
 
         """
-        return list(self.calc_vars.keys())
-
-    def calculate(self, algo, mdata, fdata, st_sel):
-        """ "
-        The main model calculation.
+        if FC.VALID in problem_results and self.check_valid:
+            vld = np.sum(problem_results[FC.VALID].to_numpy(), axis=1)
+            if np.min(vld) != np.max(vld):
+                raise ValueError(
+                    f"Objective '{self.name}': Number of valid turbines is state dependend, counting impossible"
+                )
+            return np.array([vld[0]], dtype=np.float64)
+        else:
+            return np.array([self.farm.n_turbines], dtype=np.float64)
 
-        This function is executed on a single chunk of data,
-        all computations should be based on numpy arrays.
+    def calc_population(self, vars_int, vars_float, problem_results, components=None):
+        """
+        Calculate values for all individuals of a population.
 
         Parameters
         ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        st_sel: numpy.ndarray of bool
-            The state-turbine selection,
-            shape: (n_states, n_turbines)
+        vars_int: np.array
+            The integer variable values, shape: (n_pop, n_vars_int)
+        vars_float: np.array
+            The float variable values, shape: (n_pop, n_vars_float)
+        problem_results: Any
+            The results of the variable application
+            to the problem
+        components: list of int, optional
+            The selected components or None for all
 
         Returns
         -------
-        results: dict
-            The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_turbines)
-
-        """
-        # prepare point data:
-        pdata = {FC.POINTS: fdata[FV.TXYH]}
-        dims = {FC.POINTS: (FC.STATE, FC.POINT, FC.XYH)}
-        for v in self.calc_vars.values():
-            pdata[v] = np.zeros_like(pdata[FC.POINTS][:, :, 0])
-            dims[v] = (FC.STATE, FC.POINT)
-        pdata = Data(
-            name=f"{self.name}_pdata",
-            data=pdata,
-            dims=dims,
-            loop_dims=[FC.STATE, FC.POINT],
-        )
-        del dims
-
-        # run ambient calculation:
-        res = algo.states.calculate(algo, mdata, fdata, pdata)
-        for v, a in FV.var2amb.items():
-            if v in res:
-                res[a] = res[v].copy()
-        pdata.update(res)
-
-        # run wake calculation:
-        res = self._wcalc.calculate(algo, mdata, fdata, pdata)
-
-        # extract results:
-        out = {v: fdata[v] for v in self.calc_vars.keys()}
-        for v in out.keys():
-            out[v][st_sel] = res[self.calc_vars[v]][st_sel]
+        values: np.array
+            The component values, shape: (n_pop, n_sel_components)
 
-        return out
+        """
+        n_pop = problem_results["n_pop"].to_numpy()
+        if self.check_valid:
+            n_states = problem_results["n_org_states"].to_numpy()
+            n_turbines = self.farm.n_turbines
+            vld = (
+                problem_results[FC.VALID]
+                .to_numpy()
+                .reshape(n_pop, n_states, n_turbines)
+            )
+            vld = np.sum(vld, axis=2)
+            if np.any(np.min(vld, axis=1) != np.max(vld, axis=1)):
+                raise ValueError(
+                    f"Objective '{self.name}': Number of valid turbines is state dependend, counting impossible"
+                )
+            return vld[:, 0, None]
+        else:
+            return np.full((n_pop, 1), self.farm.n_turbines, dtype=vars_float.dtype)
```

### Comparing `foxes-0.6.2/foxes/models/turbine_models/sector_management.py` & `foxes-0.7/foxes/models/turbine_models/sector_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,40 +158,39 @@
         output_vars: list of str
             The output variable names
 
         """
         return self._tvars
 
     def calculate(self, algo, mdata, fdata, st_sel):
-        """ "
+        """
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        st_sel: numpy.ndarray of bool
+        st_sel: slice or numpy.ndarray of bool
             The state-turbine selection,
-            shape: (n_states, n_turbines)
+            for shape: (n_states, n_turbines)
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
-
         # prepare:
         n_trbs = len(self._trbs)
         if n_trbs == fdata.n_turbines and np.all(
             self._trbs == np.arange(fdata.n_turbines)
         ):
             tsel = np.s_[:]
         else:
```

### Comparing `foxes-0.6.2/foxes/models/turbine_models/set_XYHD.py` & `foxes-0.7/foxes/models/wake_superpositions/ti_quadratic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,143 @@
 import numpy as np
 
-from foxes.core import TurbineModel
+from foxes.core import WakeSuperposition
 import foxes.variables as FV
-import foxes.constants as FC
 
 
-class SetXYHD(TurbineModel):
+class TIQuadratic(WakeSuperposition):
     """
-    Sets basic turbine data, from
-    turbine object to farm data.
+    Quadratic wake superposition for TI.
 
     Attributes
     ----------
-    set_XY: bool
-        Flag for (x,y) data
-    set_H: bool
-        Flag for height data
-    set_D: bool
-        Flag for rotor diameter data
+    superp_to_amb: str
+        The method for combining ambient with wake deltas:
+        linear or quadratic
 
-    :group: models.turbine_models
+    :group: models.wake_superpositions
 
     """
 
-    def __init__(self, set_XY=True, set_H=True, set_D=True):
+    def __init__(self, superp_to_amb="quadratic"):
         """
         Constructor.
 
         Parameters
         ----------
-        set_XY: bool
-            Flag for (x,y) data
-        set_H: bool
-            Flag for height data
-        set_D: bool
-            Flag for rotor diameter data
+        superp_to_amb: str
+            The method for combining ambient with wake deltas:
+            linear or quadratic
 
         """
         super().__init__()
+        self.superp_to_amb = superp_to_amb
 
-        self.set_XY = set_XY
-        self.set_H = set_H
-        self.set_D = set_D
+    def __repr__(self):
+        return f"{type(self).__name__}(superp_to_amb={self.superp_to_amb})"
 
-    def output_farm_vars(self, algo):
+    def add_wake(
+        self,
+        algo,
+        mdata,
+        fdata,
+        tdata,
+        downwind_index,
+        st_sel,
+        variable,
+        wake_delta,
+        wake_model_result,
+    ):
         """
-        The variables which are being modified by the model.
+        Add a wake delta to previous wake deltas,
+        at rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
+        mdata: foxes.core.MData
+            The model data
+        fdata: foxes.core.FData
+            The farm data
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        st_sel: numpy.ndarray of bool
+            The selection of targets, shape: (n_states, n_targets)
+        variable: str
+            The variable name for which the wake deltas applies
+        wake_delta: numpy.ndarray
+            The original wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
+        wake_model_result: numpy.ndarray
+            The new wake deltas of the selected rotors,
+            shape: (n_st_sel, n_tpoints, ...)
 
         Returns
         -------
-        output_vars: list of str
-            The output variable names
+        wdelta: numpy.ndarray
+            The updated wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
 
         """
-        ovars = []
-        if self.set_XY:
-            ovars.append(FV.X)
-            ovars.append(FV.Y)
-        if self.set_H:
-            ovars.append(FV.H)
-        if self.set_D:
-            ovars.append(FV.D)
-        return ovars
-
-    def calculate(self, algo, mdata, fdata, st_sel):
-        """ "
-        The main model calculation.
-
-        This function is executed on a single chunk of data,
-        all computations should be based on numpy arrays.
+        if variable != FV.TI:
+            raise ValueError(
+                f"Superposition '{self.name}': Expecting wake variable {FV.TI}, got {variable}"
+            )
+
+        wake_delta[st_sel] += wake_model_result**2
+        return wake_delta
+
+    def calc_final_wake_delta(
+        self,
+        algo,
+        mdata,
+        fdata,
+        variable,
+        amb_results,
+        wake_delta,
+    ):
+        """
+        Calculate the final wake delta after adding all
+        contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        st_sel: numpy.ndarray of bool
-            The state-turbine selection,
-            shape: (n_states, n_turbines)
+        variable: str
+            The variable name for which the wake deltas applies
+        amb_results: numpy.ndarray
+            The ambient results at targets,
+            shape: (n_states, n_targets, n_tpoints)
+        wake_delta: numpy.ndarray
+            The wake deltas at targets, shape:
+            (n_states, n_targets, n_tpoints)
 
         Returns
         -------
-        results: dict
-            The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_turbines)
-
-        """
-        n_states = mdata.n_states
-        n_turbines = algo.n_turbines
-
-        if self.set_XY or self.set_H:
-            fdata[FV.TXYH] = np.full((n_states, n_turbines, 3), np.nan, dtype=FC.DTYPE)
-            if self.set_XY:
-                fdata[FV.X] = fdata[FV.TXYH][..., 0]
-                fdata[FV.Y] = fdata[FV.TXYH][..., 1]
-            if self.set_H:
-                fdata[FV.H] = fdata[FV.TXYH][..., 2]
-
-        for ti in range(n_turbines):
-            ssel = st_sel[:, ti]
-            if np.any(ssel):
-                if np.all(ssel):
-                    ssel = np.s_[:]
-
-                if self.set_XY:
-                    fdata[FV.X][ssel, ti] = algo.farm.turbines[ti].xy[0]
-                    fdata[FV.Y][ssel, ti] = algo.farm.turbines[ti].xy[1]
-
-                if self.set_H:
-                    H = algo.farm.turbines[ti].H
-                    if H is None:
-                        H = algo.farm_controller.turbine_types[ti].H
-                    fdata[FV.H][ssel, ti] = H
-
-                if self.set_D:
-                    D = algo.farm.turbines[ti].D
-                    if D is None:
-                        D = algo.farm_controller.turbine_types[ti].D
-                    fdata[FV.D][ssel, ti] = D
+        final_wake_delta: numpy.ndarray
+            The final wake delta, which will be added to the ambient
+            results by simple plus operation. Shape:
+            (n_states, n_targets, n_tpoints)
 
-        return {v: fdata[v] for v in self.output_farm_vars(algo)}
+        """
+        # linear superposition to ambient:
+        if self.superp_to_amb == "linear":
+            return np.sqrt(wake_delta)
+
+        # quadratic superposition to ambient:
+        elif self.superp_to_amb == "quadratic":
+            return np.sqrt(wake_delta + amb_results**2) - amb_results
+
+        # unknown ti delta:
+        else:
+            raise ValueError(
+                f"Unknown superp_to_amb = '{self.superp_to_amb}', valid choices: linear, quadratic"
+            )
```

### Comparing `foxes-0.6.2/foxes/models/turbine_models/set_farm_vars.py` & `foxes-0.7/foxes/input/states/scan_ws.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,165 +1,168 @@
 import numpy as np
 
-from foxes.core import TurbineModel
+from foxes.core import States
+import foxes.variables as FV
 import foxes.constants as FC
 
 
-class SetFarmVars(TurbineModel):
+class ScanWS(States):
     """
-    Set farm data variables to given data.
+    A given list of wind speeds, all other variables are fixed.
 
-    Attributes
+    Parameters
     ----------
-    vars: list of str
-        The variables to be set
+    wd: float
+        The wind direction
+    ti: float
+        The TI value
+    rho: float
+        The air density
 
-    :group: models.turbine_models
+    :group: input.states
 
     """
 
-    def __init__(self, pre_rotor=False):
+    def __init__(self, ws_list, wd, ti=None, rho=None):
         """
         Constructor.
 
         Parameters
         ----------
-        pre_rotor: bool
-            Flag for running this model before
-            running the rotor model.
+        ws_list: array_like
+            The wind speed values
+        wd: float
+            The wind direction
+        ti: float, optional
+            The TI value
+        rho: float, optional
+            The air density
+
+        """
+        super().__init__()
+
+        self._wsl = np.array(ws_list)
+        self.N = len(ws_list)
+        self.wd = wd
+        self.ti = ti
+        self.rho = rho
 
+    def load_data(self, algo, verbosity=0):
         """
-        super().__init__(pre_rotor=pre_rotor)
-        self.reset()
+        Load and/or create all model data that is subject to chunking.
 
-    def add_var(self, var, data):
-        """
-        Add data for a variable.
+        Such data should not be stored under self, for memory reasons. The
+        data returned here will automatically be chunked and then provided
+        as part of the mdata object during calculations.
 
         Parameters
         ----------
-        var: str
-            The variable name
-        data: numpy.ndarray
-            The data, shape: (n_states, n_turbines)
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        verbosity: int
+            The verbosity level, 0 = silent
+
+        Returns
+        -------
+        idata: dict
+            The dict has exactly two entries: `data_vars`,
+            a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
+            and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
-        self.vars.append(var)
-        self._vdata.append(np.asarray(data, dtype=FC.DTYPE))
+        self.WS = self.var(FV.WS)
 
-    def reset(self):
+        idata = super().load_data(algo, verbosity)
+        idata["data_vars"][self.WS] = ((FC.STATE,), self._wsl)
+
+        return idata
+
+    def size(self):
         """
-        Remove all variables.
+        The total number of states.
+
+        Returns
+        -------
+        int:
+            The total number of states
+
         """
-        self.vars = []
-        self._vdata = []
+        return self.N
 
-    def output_farm_vars(self, algo):
+    def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
         output_vars: list of str
             The output variable names
 
         """
-        return self.vars
+        pvars = [FV.WS]
+        if self.wd is not None:
+            pvars.append(FV.WD)
+        if self.ti is not None:
+            pvars.append(FV.TI)
+        if self.rho is not None:
+            pvars.append(FV.RHO)
+        return pvars
 
-    def load_data(self, algo, verbosity=0):
+    def weights(self, algo):
         """
-        Load and/or create all model data that is subject to chunking.
-
-        Such data should not be stored under self, for memory reasons. The
-        data returned here will automatically be chunked and then provided
-        as part of the mdata object during calculations.
+        The statistical weights of all states.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
 
         Returns
         -------
-        idata: dict
-            The dict has exactly two entries: `data_vars`,
-            a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
-            and `coords`, a dict with entries `dim_name_str -> dim_array`
+        weights: numpy.ndarray
+            The weights, shape: (n_states, n_turbines)
 
         """
-        idata = super().load_data(algo, verbosity)
-
-        for i, v in enumerate(self.vars):
-            data = np.full((algo.n_states, algo.n_turbines), np.nan, dtype=FC.DTYPE)
-            vdata = self._vdata[i]
-
-            # handle special case of call during vectorized optimization:
-            if (
-                np.ndim(vdata)
-                and vdata.shape[0] != algo.n_states
-                and hasattr(algo.states, "n_pop")
-            ):
-                n_pop = algo.states.n_pop
-                n_ost = algo.states.states.size()
-                n_trb = algo.n_turbines
-                vdata = np.zeros((n_pop, n_ost, n_trb), dtype=FC.DTYPE)
-                vdata[:] = self._vdata[i][None, :]
-                vdata = vdata.reshape(n_pop * n_ost, n_trb)
-
-            data[:] = vdata
-            idata["data_vars"][self.var(v)] = ((FC.STATE, FC.TURBINE), data)
+        return np.full((self.N, algo.n_turbines), 1.0 / self.N, dtype=FC.DTYPE)
 
-        return idata
-
-    def calculate(self, algo, mdata, fdata, st_sel):
+    def calculate(self, algo, mdata, fdata, tdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        st_sel: numpy.ndarray of bool
-            The state-turbine selection,
-            shape: (n_states, n_turbines)
+        tdata: foxes.core.TData
+            The target point data
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_turbines)
+            Values: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints)
 
         """
-        n_states = fdata.n_states
-        n_turbines = fdata.n_turbines
-        allt = np.all(st_sel)
-
-        for v in self.vars:
-            data = mdata[self.var(v)]
-            hsel = ~np.isnan(data)
-            hallt = np.all(hsel)
-
-            if allt and hallt:
-                fdata[v][:] = data
-
-            else:
-                if v not in fdata:
-                    fdata[v] = np.full((n_states, n_turbines), np.nan, dtype=FC.DTYPE)
+        tdata[FV.WS] = np.zeros_like(tdata[FC.TARGETS][..., 0])
+        tdata[FV.WS][:] = mdata[self.WS][:, None, None]
 
-                tsel = st_sel & hsel
-                fdata[v][tsel] = data[tsel]
+        if self.wd is not None:
+            tdata[FV.WD] = np.full_like(tdata[FV.WS], self.wd)
+        if self.ti is not None:
+            tdata[FV.TI] = np.full_like(tdata[FV.WS], self.ti)
+        if self.rho is not None:
+            tdata[FV.RHO] = np.full_like(tdata[FV.WS], self.rho)
 
-        return {v: fdata[v] for v in self.vars}
+        return {v: tdata[v] for v in self.output_point_vars(algo)}
```

### Comparing `foxes-0.6.2/foxes/models/turbine_models/table_factors.py` & `foxes-0.7/foxes/output/calc_points.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,167 +1,144 @@
 import numpy as np
-import pandas as pd
-from scipy.interpolate import interpn
+from xarray import Dataset
 
-from foxes.core import TurbineModel
-from foxes.utils import PandasFileHelper
 import foxes.constants as FC
+import foxes.variables as FV
+from foxes.utils import write_nc
 
+from .output import Output
 
-class TableFactors(TurbineModel):
-    """
-    Multiplies variables by factors from a
-    two dimensional table.
 
-    The column names are expected to be numbers
-    that represent the col_var variable.
+class PointCalculator(Output):
+    """
+    Computes results at given points
 
     Attributes
     ----------
-    data_source: str or pandas.DataFrame
-        Either path to a file or data
-    row_var: str
-        The row-wise variable
-    col_var: str
-        The column-wise variable
-    ovars: list of str
-        The variables onto which the factors
-        are multiplied
+    algo: foxes.Algorithm
+        The algorithm for point calculation
+    farm_results: xarray.Dataset
+        The farm results
 
-    :group: models.turbine_models
+    :group: output
 
     """
 
-    def __init__(
-        self,
-        data_source,
-        row_var,
-        col_var,
-        output_vars,
-        pd_file_read_pars={},
-        **ipars,
-    ):
+    def __init__(self, algo, farm_results, **kwargs):
         """
         Constructor.
 
         Parameters
         ----------
-        data_source: str or pandas.DataFrame
-            Either path to a file or data
-        row_var: str
-            The row-wise variable
-        col_var: str
-            The column-wise variable
-        output_vars: list of str
-            The variables onto which the factors
-            are multiplied
-        pd_file_read_pars: dict
-            Parameters for pandas file reading
-        ipars: dict, optional
-            Parameters for scipy.interpolate.interpn
+        algo: foxes.Algorithm
+            The algorithm for point calculation
+        farm_results: xarray.Dataset
+            The farm results
+        kwargs: dict, optional
+            Additional parameters for the base class
 
         """
-        super().__init__()
+        super().__init__(**kwargs)
+        self.algo = algo
+        self.farm_results = farm_results
 
-        self.data_source = data_source
-        self.row_var = row_var
-        self.col_var = col_var
-        self.ovars = output_vars
-        self._rpars = pd_file_read_pars
-        self._ipars = ipars
-
-        self._cvals = None
-        self._data = None
-
-    def output_farm_vars(self, algo):
+    def calculate(
+        self,
+        points,
+        *args,
+        states_mean=False,
+        weight_turbine=0,
+        to_file=None,
+        write_vars=None,
+        write_pars={},
+        **kwargs,
+    ):
         """
-        The variables which are being modified by the model.
+        Calculate point results
 
         Parameters
         ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
+        points: numpy.ndarray
+            The points, shape: (n_points, 3)
+            or (n_states, n_points, 3)
+        args: tuple, optional
+            Additional arguments for algo.calc_points
+        states_mean: bool
+            Flag for taking the mean over states
+        weight_turbine: int, optional
+            Index of the turbine from which to take the weight
+        to_file: str, optional
+            Path to the output netCDF file
+        write_vars: list of str
+            The variables to be written to file, or None
+            for all
+        write_pars: dict, optional
+            Additional parameters for write_nc
+        kwargs: tuple, optional
+            Additional arguments for algo.calc_points
 
         Returns
         -------
-        output_vars: list of str
-            The output variable names
-
-        """
-        return self.ovars
+        point_results: xarray.Dataset
+            The point results. The calculated variables have
+            dimensions (state, point)
 
-    def initialize(self, algo, verbosity=0):
         """
-        Initializes the model.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
-
-        """
-        super().initialize(algo, verbosity)
-
-        if isinstance(self.data_source, pd.DataFrame):
-            self._data = self.data_source
+        if points.shape[-1] == 3 and len(points.shape) == 3:
+            pts = points
+            p_has_s = True
+        elif points.shape[-1] == 3 and len(points.shape) == 2:
+            pts = np.zeros([self.algo.n_states] + list(points.shape), dtype=FC.DTYPE)
+            pts[:] = points[None, :]
+            p_has_s = False
         else:
-            if verbosity > 0:
-                print(f"{self.name}: Reading file {self.data_source}")
-            rpars = dict(index_col=0)
-            rpars.update(self._rpars)
-            self._data = PandasFileHelper.read_file(self.data_source, **rpars)
-
-        self._rvals = self._data.index.to_numpy(FC.DTYPE)
-        self._cvals = self._data.columns.to_numpy(FC.DTYPE)
-        self._data = self._data.to_numpy(FC.DTYPE)
-
-    def calculate(self, algo, mdata, fdata, st_sel):
-        """ "
-        The main model calculation.
+            raise ValueError(
+                f"Expecting point shape (n_states, n_points, 3) or (n_points, 3), got {points.shape}"
+            )
 
-        This function is executed on a single chunk of data,
-        all computations should be based on numpy arrays.
+        pres = self.algo.calc_points(self.farm_results, pts, *args, **kwargs)
 
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        st_sel: numpy.ndarray of bool
-            The state-turbine selection,
-            shape: (n_states, n_turbines)
-
-        Returns
-        -------
-        results: dict
-            The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_turbines)
-
-        """
-        n_sel = np.sum(st_sel)
-        qts = np.zeros((n_sel, 2), dtype=FC.DTYPE)
-        qts[:, 0] = fdata[self.row_var][st_sel]
-        qts[:, 1] = fdata[self.col_var][st_sel]
-
-        try:
-            factors = interpn(
-                (self._rvals, self._cvals), self._data, qts, **self._ipars
+        if states_mean:
+            weights = self.farm_results[FV.WEIGHT].to_numpy()[:, weight_turbine]
+            pres = Dataset(
+                data_vars={
+                    v: np.einsum("s,sp->p", weights, pres[v].to_numpy())
+                    for v in pres.data_vars.keys()
+                }
             )
-        except ValueError as e:
-            print(f"\nDATA       : ({self.row_var}, {self.col_var})")
-            print(
-                f"DATA BOUNDS: ({np.min(self._rvals)}, {np.min(self._cvals)}) -- ({np.max(self._rvals)}, {np.max(self._cvals)})"
-            )
-            print(
-                f"VALUE BOUNDS: ({np.min(qts[:, 0]):.4f}, {np.min(qts[:, 1]):.4f}) -- ({np.max(qts[:, 0]):.4f}, {np.max(qts[:, 1]):.4f})\n"
-            )
-            raise e
 
-        for v in self.output_farm_vars(algo):
-            fdata[v][st_sel] *= factors
+        vrs = list(pres.data_vars.keys()) if write_vars is None else write_vars
+        if to_file is not None:
+            if states_mean:
+                if p_has_s:
+                    points = np.einsum("s,spd->pd", weights, points)
+                dvars = {
+                    "x": ((FC.POINT,), points[..., 0]),
+                    "y": ((FC.POINT,), points[..., 1]),
+                    "z": ((FC.POINT,), points[..., 2]),
+                }
+                dvars.update({v: ((FC.POINT,), pres[v].to_numpy()) for v in vrs})
+                ds = Dataset(data_vars=dvars)
+            else:
+                if p_has_s:
+                    dvars = {
+                        "x": ((FC.STATE, FC.POINT), points[..., 0]),
+                        "y": ((FC.STATE, FC.POINT), points[..., 1]),
+                        "z": ((FC.STATE, FC.POINT), points[..., 2]),
+                    }
+                else:
+                    dvars = {
+                        "x": ((FC.POINT,), points[..., 0]),
+                        "y": ((FC.POINT,), points[..., 1]),
+                        "z": ((FC.POINT,), points[..., 2]),
+                    }
+                dvars.update(
+                    {v: ((FC.STATE, FC.POINT), pres[v].to_numpy()) for v in vrs}
+                )
+                ds = Dataset(
+                    coords={FC.STATE: pres[FC.STATE].to_numpy()}, data_vars=dvars
+                )
+
+            fpath = self.get_fpath(to_file)
+            write_nc(ds, fpath, **write_pars)
 
-        return {v: fdata[v] for v in self.output_farm_vars(algo)}
+        return pres
```

### Comparing `foxes-0.6.2/foxes/models/turbine_models/thrust2ct.py` & `foxes-0.7/foxes/models/turbine_models/yawm2yaw.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,23 @@
 import numpy as np
 
 from foxes.core import TurbineModel
 import foxes.variables as FV
+import foxes.constants as FC
 
 
-class Thrust2Ct(TurbineModel):
+class YAWM2YAW(TurbineModel):
     """
-    Calculates ct from thrust force data.
-
-    Attributes
-    ----------
-    thrust_var: str
-        Name of the thrust variable
-    WSCT: str
-        The wind speed variable for ct lookup
+    Calculates absolute yaw (i.e. YAWM) from delta
+    yaw (i.e. YAWM)
 
     :group: models.turbine_models
 
     """
 
-    def __init__(self, thrust_var=FV.T, var_ws_ct=FV.REWS2):
-        """
-        Constructor.
-
-        Parameters
-        ----------
-        thrust_var: str
-            Name of the thrust variable
-        var_ws_ct: str
-            The wind speed variable for ct lookup
-
-        """
-        super().__init__()
-        self.thrust_var = thrust_var
-        self.WSCT = var_ws_ct
-
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
@@ -46,45 +25,42 @@
 
         Returns
         -------
         output_vars: list of str
             The output variable names
 
         """
-        return [FV.CT]
+        return [FV.YAW]
 
     def calculate(self, algo, mdata, fdata, st_sel):
-        """ "
+        """
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        st_sel: numpy.ndarray of bool
+        st_sel: slice or numpy.ndarray of bool
             The state-turbine selection,
-            shape: (n_states, n_turbines)
+            for shape: (n_states, n_turbines)
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
-        ct = fdata[FV.CT]
-
-        T = fdata[self.thrust_var][st_sel]
-        rho = fdata[FV.RHO][st_sel]
-        A = np.pi * (fdata[FV.D][st_sel] / 2) ** 2
-        ws = fdata[self.WSCT][st_sel]
+        yawm = fdata[FV.YAWM][st_sel]
+        wd = fdata[FV.WD][st_sel]
 
-        ct[st_sel] = 2 * T / (rho * A * ws**2)
+        yaw = fdata[FV.YAW]
+        yaw[st_sel] = np.mod(wd + yawm, 360.0)
 
-        return {FV.CT: ct}
+        return {FV.YAW: yaw}
```

### Comparing `foxes-0.6.2/foxes/models/turbine_types/CpCt_file.py` & `foxes-0.7/foxes/models/turbine_types/CpCt_file.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/models/turbine_types/CpCt_from_two.py` & `foxes-0.7/foxes/models/turbine_types/CpCt_from_two.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/models/turbine_types/PCt_file.py` & `foxes-0.7/foxes/models/turbine_types/PCt_from_two.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,80 @@
 import numpy as np
 import pandas as pd
-from pathlib import Path
 
 from foxes.core import TurbineType
 from foxes.utils import PandasFileHelper
-from foxes.data import PCTCURVE, parse_Pct_file_name
+from foxes.data import PCTCURVE, parse_Pct_two_files
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class PCtFile(TurbineType):
+class PCtFromTwo(TurbineType):
     """
     Calculate power and ct by interpolating
-    from power-ct-curve data file (or pandas DataFrame).
+    from power curve and ct curve data files.
 
     Attributes
     ----------
-    source: str or pandas.DataFrame
-        The file path, static name, or data
+    source_P: str or pandas.DataFrame
+        The file path for the power curve, static name, or data
+    source_ct: str or pandas.DataFrame
+        The file path for the ct curve, static name, or data
     col_ws: str
         The wind speed column
     col_P: str
         The power column
     col_ct: str
         The ct column
     rho: float
         The air densitiy for which the data is valid
         or None for no correction
     WSCT: str
         The wind speed variable for ct lookup
     WSP: str
         The wind speed variable for power lookup
-    rpars: dict, optional
-        Parameters for pandas file reading
+    rpars_P: dict, optional
+        Parameters for pandas power file reading
+    rpars_ct: dict, optional
+        Parameters for pandas ct file reading
 
     :group: models.turbine_types
 
     """
 
     def __init__(
         self,
-        data_source,
-        col_ws="ws",
+        data_source_P,
+        data_source_ct,
+        col_ws_P_file="ws",
+        col_ws_ct_file="ws",
         col_P="P",
         col_ct="ct",
         rho=None,
         p_ct=1.0,
         p_P=1.88,
         var_ws_ct=FV.REWS2,
         var_ws_P=FV.REWS3,
-        pd_file_read_pars={},
+        pd_file_read_pars_P={},
+        pd_file_read_pars_ct={},
         **parameters,
     ):
         """
         Constructor.
 
         Parameters
         ----------
-        data_source: str or pandas.DataFrame
-            The file path, static name, or data
-        col_ws: str
-            The wind speed column
+        data_source_P: str or pandas.DataFrame
+            The file path for the power curve, static name, or data
+        data_source_ct: str or pandas.DataFrame
+            The file path for the ct curve, static name, or data
+        col_ws_P_file: str
+            The wind speed column in the file of the power curve
+        col_ws_ct_file: str
+            The wind speed column in the file of the ct curve
         col_P: str
             The power column
         col_ct: str
             The ct column
         rho: float, optional
             The air densitiy for which the data is valid
             or None for no correction
@@ -72,38 +82,52 @@
             The exponent for yaw dependency of ct
         p_P: float
             The exponent for yaw dependency of P
         var_ws_ct: str
             The wind speed variable for ct lookup
         var_ws_P: str
             The wind speed variable for power lookup
-        pd_file_read_pars: dict
-            Parameters for pandas file reading
+        pd_file_read_pars_P:  dict
+            Parameters for pandas power file reading
+        pd_file_read_pars_ct:  dict
+            Parameters for pandas ct file reading
         parameters: dict, optional
             Additional parameters for TurbineType class
 
         """
-        if not isinstance(data_source, pd.DataFrame):
-            pars = parse_Pct_file_name(data_source)
-            pars.update(parameters)
+        if not isinstance(data_source_P, pd.DataFrame) or not isinstance(
+            data_source_ct, pd.DataFrame
+        ):
+            pars = parse_Pct_two_files(data_source_P, data_source_ct)
         else:
             pars = parameters
-
         super().__init__(**pars)
 
-        self.source = data_source
-        self.col_ws = col_ws
+        self.source_P = data_source_P
+        self.source_ct = data_source_ct
+        self.col_ws_P_file = col_ws_P_file
+        self.col_ws_ct_file = col_ws_ct_file
         self.col_P = col_P
         self.col_ct = col_ct
         self.rho = rho
         self.p_ct = p_ct
         self.p_P = p_P
         self.WSCT = var_ws_ct
         self.WSP = var_ws_P
-        self.rpars = pd_file_read_pars
+        self.rpars_P = pd_file_read_pars_P
+        self.rpars_ct = pd_file_read_pars_ct
+
+        self._data_P = None
+        self._data_ct = None
+        self._data_ws_P = None
+        self._data_ws_ct = None
+
+    def __repr__(self):
+        a = f"D={self.D}, H={self.H}, P_nominal={self.P_nominal}, P_unit={self.P_unit}, rho={self.rho}"
+        return f"{type(self).__name__}({a})"
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
@@ -137,35 +161,38 @@
         -------
         idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
-        if isinstance(self.source, pd.DataFrame):
-            data = self.source
+        # read power curve:
+        if isinstance(self.source_P, pd.DataFrame):
+            self._data_P = self.source_P
         else:
-            fpath = algo.dbook.get_file_path(PCTCURVE, self.source, check_raw=True)
-            if verbosity > 0:
-                if not Path(self.source).is_file():
-                    print(
-                        f"Turbine type '{self.name}': Reading static data from context '{PCTCURVE}'"
-                    )
-                    print(f"Path: {fpath}")
-                else:
-                    print(f"Turbine type '{self.name}': Reading file", self.source)
-            data = PandasFileHelper.read_file(fpath, **self.rpars)
-
-        data = data.set_index(self.col_ws).sort_index()
-        self.data_ws = data.index.to_numpy()
-        self.data_P = data[self.col_P].to_numpy()
-        self.data_ct = data[self.col_ct].to_numpy()
+            fpath = algo.dbook.get_file_path(PCTCURVE, self.source_P, check_raw=True)
+            self._data_P = PandasFileHelper.read_file(fpath, **self.rpars_P)
+
+        self._data_P = self._data_P.set_index(self.col_ws_P_file).sort_index()
+        self._data_ws_P = self._data_P.index.to_numpy()
+        self._data_P = self._data_P[self.col_P].to_numpy()
+
+        # read ct curve:
+        if isinstance(self.source_ct, pd.DataFrame):
+            self._data_ct = self.source_ct
+        else:
+            fpath = algo.dbook.get_file_path(PCTCURVE, self.source_ct, check_raw=True)
+            self._data_ct = PandasFileHelper.read_file(fpath, **self.rpars_ct)
+
+        self._data_ct = self._data_ct.set_index(self.col_ws_ct_file).sort_index()
+        self._data_ws_ct = self._data_ct.index.to_numpy()
+        self._data_ct = self._data_ct[self.col_ct].to_numpy()
 
         if self.P_nominal is None:
-            self.P_nominal = np.max(self.data_P) / FC.P_UNITS[self.P_unit]
+            self.P_nominal = np.max(self._data_P) / FC.P_UNITS[self.P_unit]
             if verbosity > 0:
                 print(
                     f"Turbine type '{self.name}': Setting P_nominal = {self.P_nominal:.2f} {self.P_unit}"
                 )
 
         return super().load_data(algo, verbosity)
 
@@ -176,17 +203,17 @@
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
         st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
@@ -200,15 +227,15 @@
 
         # apply air density correction:
         if self.rho is not None:
             # correct wind speed by air density, such
             # that in the partial load region the
             # correct value is reconstructed:
             rho = fdata[FV.RHO][st_sel]
-            rews2 *= (self.rho / rho) ** 0.5
+            # rews2 *= (self.rho / rho) ** 0.5
             rews3 *= (self.rho / rho) ** (1.0 / 3.0)
             del rho
 
         # in yawed case, calc yaw corrected wind speed:
         if FV.YAWM in fdata and (self.p_P is not None or self.p_ct is not None):
             # calculate corrected wind speed wsc,
             # gives ws**3 * cos**p_P in partial load region
@@ -225,20 +252,19 @@
                 rews3 *= (cosm**self.p_P) ** (1.0 / 3.0)
             del yawm, cosm
 
         out = {
             FV.P: fdata[FV.P],
             FV.CT: fdata[FV.CT],
         }
-
         out[FV.P][st_sel] = np.interp(
-            rews3, self.data_ws, self.data_P, left=0.0, right=0.0
+            rews3, self._data_ws_P, self._data_P, left=0.0, right=0.0
         )
         out[FV.CT][st_sel] = np.interp(
-            rews2, self.data_ws, self.data_ct, left=0.0, right=0.0
+            rews2, self._data_ws_ct, self._data_ct, left=0.0, right=0.0
         )
 
         return out
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
@@ -248,8 +274,8 @@
         algo: foxes.core.Algorithm
             The calculation algorithm
         verbosity: int
             The verbosity level
 
         """
         super().finalize(algo, verbosity)
-        del self.data_ws, self.data_P, self.data_ct
+        del self._data_ws_P, self._data_ws_ct, self._data_P, self._data_ct
```

### Comparing `foxes-0.6.2/foxes/models/turbine_types/PCt_from_two.py` & `foxes-0.7/foxes/models/turbine_types/PCt_file.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,70 @@
 import numpy as np
 import pandas as pd
+from pathlib import Path
 
 from foxes.core import TurbineType
 from foxes.utils import PandasFileHelper
-from foxes.data import PCTCURVE, parse_Pct_two_files
+from foxes.data import PCTCURVE, parse_Pct_file_name
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class PCtFromTwo(TurbineType):
+class PCtFile(TurbineType):
     """
     Calculate power and ct by interpolating
-    from power curve and ct curve data files.
+    from power-ct-curve data file (or pandas DataFrame).
 
     Attributes
     ----------
-    source_P: str or pandas.DataFrame
-        The file path for the power curve, static name, or data
-    source_ct: str or pandas.DataFrame
-        The file path for the ct curve, static name, or data
+    source: str or pandas.DataFrame
+        The file path, static name, or data
     col_ws: str
         The wind speed column
     col_P: str
         The power column
     col_ct: str
         The ct column
     rho: float
         The air densitiy for which the data is valid
         or None for no correction
     WSCT: str
         The wind speed variable for ct lookup
     WSP: str
         The wind speed variable for power lookup
-    rpars_P: dict, optional
-        Parameters for pandas power file reading
-    rpars_ct: dict, optional
-        Parameters for pandas ct file reading
+    rpars: dict, optional
+        Parameters for pandas file reading
 
     :group: models.turbine_types
 
     """
 
     def __init__(
         self,
-        data_source_P,
-        data_source_ct,
-        col_ws_P_file="ws",
-        col_ws_ct_file="ws",
+        data_source,
+        col_ws="ws",
         col_P="P",
         col_ct="ct",
         rho=None,
         p_ct=1.0,
         p_P=1.88,
         var_ws_ct=FV.REWS2,
         var_ws_P=FV.REWS3,
-        pd_file_read_pars_P={},
-        pd_file_read_pars_ct={},
+        pd_file_read_pars={},
         **parameters,
     ):
         """
         Constructor.
 
         Parameters
         ----------
-        data_source_P: str or pandas.DataFrame
-            The file path for the power curve, static name, or data
-        data_source_ct: str or pandas.DataFrame
-            The file path for the ct curve, static name, or data
-        col_ws_P_file: str
-            The wind speed column in the file of the power curve
-        col_ws_ct_file: str
-            The wind speed column in the file of the ct curve
+        data_source: str or pandas.DataFrame
+            The file path, static name, or data
+        col_ws: str
+            The wind speed column
         col_P: str
             The power column
         col_ct: str
             The ct column
         rho: float, optional
             The air densitiy for which the data is valid
             or None for no correction
@@ -82,48 +72,42 @@
             The exponent for yaw dependency of ct
         p_P: float
             The exponent for yaw dependency of P
         var_ws_ct: str
             The wind speed variable for ct lookup
         var_ws_P: str
             The wind speed variable for power lookup
-        pd_file_read_pars_P:  dict
-            Parameters for pandas power file reading
-        pd_file_read_pars_ct:  dict
-            Parameters for pandas ct file reading
+        pd_file_read_pars: dict
+            Parameters for pandas file reading
         parameters: dict, optional
             Additional parameters for TurbineType class
 
         """
-        if not isinstance(data_source_P, pd.DataFrame) or not isinstance(
-            data_source_ct, pd.DataFrame
-        ):
-            pars = parse_Pct_two_files(data_source_P, data_source_ct)
+        if not isinstance(data_source, pd.DataFrame):
+            pars = parse_Pct_file_name(data_source)
+            pars.update(parameters)
         else:
             pars = parameters
+
         super().__init__(**pars)
 
-        self.source_P = data_source_P
-        self.source_ct = data_source_ct
-        self.col_ws_P_file = col_ws_P_file
-        self.col_ws_ct_file = col_ws_ct_file
+        self.source = data_source
+        self.col_ws = col_ws
         self.col_P = col_P
         self.col_ct = col_ct
         self.rho = rho
         self.p_ct = p_ct
         self.p_P = p_P
         self.WSCT = var_ws_ct
         self.WSP = var_ws_P
-        self.rpars_P = pd_file_read_pars_P
-        self.rpars_ct = pd_file_read_pars_ct
+        self.rpars = pd_file_read_pars
 
-        self._data_P = None
-        self._data_ct = None
-        self._data_ws_P = None
-        self._data_ws_ct = None
+    def __repr__(self):
+        a = f"D={self.D}, H={self.H}, P_nominal={self.P_nominal}, P_unit={self.P_unit}, rho={self.rho}"
+        return f"{type(self).__name__}({a})"
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
@@ -157,59 +141,133 @@
         -------
         idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
-        # read power curve:
-        if isinstance(self.source_P, pd.DataFrame):
-            self._data_P = self.source_P
-        else:
-            fpath = algo.dbook.get_file_path(PCTCURVE, self.source_P, check_raw=True)
-            self._data_P = PandasFileHelper.read_file(fpath, **self.rpars_P)
-
-        self._data_P = self._data_P.set_index(self.col_ws_P_file).sort_index()
-        self._data_ws_P = self._data_P.index.to_numpy()
-        self._data_P = self._data_P[self.col_P].to_numpy()
-
-        # read ct curve:
-        if isinstance(self.source_ct, pd.DataFrame):
-            self._data_ct = self.source_ct
+        if isinstance(self.source, pd.DataFrame):
+            data = self.source
         else:
-            fpath = algo.dbook.get_file_path(PCTCURVE, self.source_ct, check_raw=True)
-            self._data_ct = PandasFileHelper.read_file(fpath, **self.rpars_ct)
-
-        self._data_ct = self._data_ct.set_index(self.col_ws_ct_file).sort_index()
-        self._data_ws_ct = self._data_ct.index.to_numpy()
-        self._data_ct = self._data_ct[self.col_ct].to_numpy()
+            fpath = algo.dbook.get_file_path(PCTCURVE, self.source, check_raw=True)
+            if verbosity > 0:
+                if not Path(self.source).is_file():
+                    print(
+                        f"Turbine type '{self.name}': Reading static data from context '{PCTCURVE}'"
+                    )
+                    print(f"Path: {fpath}")
+                else:
+                    print(f"Turbine type '{self.name}': Reading file", self.source)
+            data = PandasFileHelper.read_file(fpath, **self.rpars)
+
+        data = data.set_index(self.col_ws).sort_index()
+        self.data_ws = data.index.to_numpy()
+        self.data_P = data[self.col_P].to_numpy()
+        self.data_ct = data[self.col_ct].to_numpy()
 
         if self.P_nominal is None:
-            self.P_nominal = np.max(self._data_P) / FC.P_UNITS[self.P_unit]
+            self.P_nominal = np.max(self.data_P) / FC.P_UNITS[self.P_unit]
             if verbosity > 0:
                 print(
                     f"Turbine type '{self.name}': Setting P_nominal = {self.P_nominal:.2f} {self.P_unit}"
                 )
 
         return super().load_data(algo, verbosity)
 
+    def modify_cutin(
+        self,
+        modify_ct,
+        modify_P,
+        steps=20,
+        iterations=100,
+        a=0.55,
+        b=0.55,
+    ):
+        """
+        Modify the data such that a discontinuity
+        at cutin wind speed is avoided
+
+        Parameters
+        ----------
+        variable: str
+            The target variable
+        modify_ct: bool
+            Flag for modification of the ct curve
+        modify_P: bool
+            Flag for modification of the power curve
+        steps: int
+            The number of wind speed steps between 0 and
+            the cutin wind speed
+        iterations: int
+            The number of iterations
+        a: float
+            Coefficient for iterative mixing
+        b: float
+            Coefficient for iterative mixing
+
+        """
+        if modify_ct or modify_P:
+
+            ws = self.data_ws
+            ct = self.data_ct
+            P = self.data_P
+
+            i = 0
+            try:
+                while (
+                    i < len(ws)
+                    and (not modify_ct or ct[i] < 1e-5)
+                    and (not modify_P or P[i] < 0.1)
+                ):
+                    i += 1
+            except IndexError:
+                raise IndexError(
+                    f"Turbine type '{self.name}': Failed not determine cutin wind speed. ws = {ws}, ct = {ct}, P = {P}"
+                )
+
+            if ws[i] > 0:
+                ws = ws[i:]
+                ct = ct[i:]
+                P = P[i:]
+
+                new_ws = np.linspace(0.0, ws[0], steps + 1, dtype=ws.dtype)
+                new_ct = np.zeros_like(new_ws)
+                new_P = np.zeros_like(new_ws)
+
+                if modify_ct:
+                    new_ct[-1] = ct[0]
+                    for it in range(iterations):
+                        new_ct[1:-1] = a * new_ct[:-2] + (1 - a) * new_ct[2:]
+
+                if modify_P:
+                    new_P[-1] = P[0]
+                    for it in range(iterations):
+                        new_P[1:-1] = b * new_P[:-2] + (1 - b) * new_P[2:]
+
+                self.data_ws = np.concatenate([new_ws[:-1], ws], axis=0)
+                self.data_ct = np.concatenate([new_ct[:-1], ct], axis=0)
+                self.data_P = np.concatenate([new_P[:-1], P], axis=0)
+
+        else:
+            super().modify_cutin(modify_ct, modify_P)
+
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
         st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
@@ -223,15 +281,15 @@
 
         # apply air density correction:
         if self.rho is not None:
             # correct wind speed by air density, such
             # that in the partial load region the
             # correct value is reconstructed:
             rho = fdata[FV.RHO][st_sel]
-            rews2 *= (self.rho / rho) ** 0.5
+            # rews2 *= (self.rho / rho) ** 0.5
             rews3 *= (self.rho / rho) ** (1.0 / 3.0)
             del rho
 
         # in yawed case, calc yaw corrected wind speed:
         if FV.YAWM in fdata and (self.p_P is not None or self.p_ct is not None):
             # calculate corrected wind speed wsc,
             # gives ws**3 * cos**p_P in partial load region
@@ -248,19 +306,20 @@
                 rews3 *= (cosm**self.p_P) ** (1.0 / 3.0)
             del yawm, cosm
 
         out = {
             FV.P: fdata[FV.P],
             FV.CT: fdata[FV.CT],
         }
+
         out[FV.P][st_sel] = np.interp(
-            rews3, self._data_ws_P, self._data_P, left=0.0, right=0.0
+            rews3, self.data_ws, self.data_P, left=0.0, right=0.0
         )
         out[FV.CT][st_sel] = np.interp(
-            rews2, self._data_ws_ct, self._data_ct, left=0.0, right=0.0
+            rews2, self.data_ws, self.data_ct, left=0.0, right=0.0
         )
 
         return out
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
@@ -270,8 +329,8 @@
         algo: foxes.core.Algorithm
             The calculation algorithm
         verbosity: int
             The verbosity level
 
         """
         super().finalize(algo, verbosity)
-        del self._data_ws_P, self._data_ws_ct, self._data_P, self._data_ct
+        del self.data_ws, self.data_P, self.data_ct
```

### Comparing `foxes-0.6.2/foxes/models/turbine_types/null_type.py` & `foxes-0.7/foxes/models/turbine_types/null_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,17 @@
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
         st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
```

### Comparing `foxes-0.6.2/foxes/models/turbine_types/wsrho2PCt_from_two.py` & `foxes-0.7/foxes/models/turbine_types/wsrho2PCt_from_two.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,17 +211,17 @@
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
         st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
```

### Comparing `foxes-0.6.2/foxes/models/turbine_types/wsti2PCt_from_two.py` & `foxes-0.7/foxes/models/turbine_types/wsti2PCt_from_two.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,18 @@
             self.ipars_P = dict(method="linear", bounds_error=True, fill_value=0.0)
         if self.ipars_ct is None:
             self.ipars_ct = dict(method="linear", bounds_error=True, fill_value=0.0)
 
         self._P = None
         self._ct = None
 
+    def __repr__(self):
+        a = f"D={self.D}, H={self.H}, P_nominal={self.P_nominal}, P_unit={self.P_unit}, rho={self.rho}"
+        return f"{type(self).__name__}({a})"
+
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
@@ -219,17 +223,17 @@
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
         st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
```

### Comparing `foxes-0.6.2/foxes/models/vertical_profiles/abl_log_neutral_ws.py` & `foxes-0.7/foxes/models/vertical_profiles/abl_log_neutral_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/models/vertical_profiles/abl_log_stable_ws.py` & `foxes-0.7/foxes/models/vertical_profiles/abl_log_stable_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/models/vertical_profiles/abl_log_unstable_ws.py` & `foxes-0.7/foxes/models/vertical_profiles/abl_log_unstable_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/models/vertical_profiles/abl_log_ws.py` & `foxes-0.7/foxes/models/vertical_profiles/abl_log_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/models/vertical_profiles/data_profile.py` & `foxes-0.7/foxes/models/vertical_profiles/data_profile.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/models/vertical_profiles/sheared_ws.py` & `foxes-0.7/foxes/models/vertical_profiles/sheared_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/models/vertical_profiles/uniform.py` & `foxes-0.7/foxes/models/vertical_profiles/uniform.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/models/wake_frames/farm_order.py` & `foxes-0.7/foxes/models/wake_frames/farm_order.py`

 * *Files 20% similar despite different names*

```diff
@@ -55,80 +55,84 @@
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
 
         Returns
         -------
         order: numpy.ndarray
             The turbine order, shape: (n_states, n_turbines)
 
         """
         order = np.zeros((fdata.n_states, fdata.n_turbines), dtype=FC.ITYPE)
         order[:] = np.arange(fdata.n_turbines)[None, :]
 
         return order
 
-    def get_wake_coos(self, algo, mdata, fdata, pdata, states_source_turbine):
+    def get_wake_coos(
+        self,
+        algo,
+        mdata,
+        fdata,
+        tdata,
+        downwind_index,
+    ):
         """
-        Calculate wake coordinates.
+        Calculate wake coordinates of rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
 
         Returns
         -------
         wake_coos: numpy.ndarray
             The wake frame coordinates of the evaluation
-            points, shape: (n_states, n_points, 3)
+            points, shape: (n_states, n_targets, n_tpoints, 3)
 
         """
-        return self.base_frame.get_wake_coos(
-            algo, mdata, fdata, pdata, states_source_turbine
-        )
+        return self.base_frame.get_wake_coos(algo, mdata, fdata, tdata, downwind_index)
 
-    def get_centreline_points(self, algo, mdata, fdata, states_source_turbine, x):
+    def get_centreline_points(self, algo, mdata, fdata, downwind_index, x):
         """
         Gets the points along the centreline for given
         values of x.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        downwind_index: int
+            The index in the downwind order
         x: numpy.ndarray
             The wake frame x coordinates, shape: (n_states, n_points)
 
         Returns
         -------
         points: numpy.ndarray
             The centreline points, shape: (n_states, n_points, 3)
 
         """
         return self.base_frame.get_centreline_points(
-            algo, mdata, fdata, states_source_turbine, x
+            algo, mdata, fdata, downwind_index, x
         )
```

### Comparing `foxes-0.6.2/foxes/models/wake_frames/rotor_wd.py` & `foxes-0.7/foxes/models/wake_frames/rotor_wd.py`

 * *Files 19% similar despite different names*

```diff
@@ -40,105 +40,106 @@
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
 
         Returns
         -------
         order: numpy.ndarray
             The turbine order, shape: (n_states, n_turbines)
 
         """
         n = np.mean(wd2uv(fdata[self.var_wd], axis=1), axis=-1)
         xy = fdata[FV.TXYH][:, :, :2]
-
         order = np.argsort(np.einsum("std,sd->st", xy, n), axis=-1)
 
         return order
 
-    def get_wake_coos(self, algo, mdata, fdata, pdata, states_source_turbine):
+    def get_wake_coos(
+        self,
+        algo,
+        mdata,
+        fdata,
+        tdata,
+        downwind_index,
+    ):
         """
-        Calculate wake coordinates.
+        Calculate wake coordinates of rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
 
         Returns
         -------
         wake_coos: numpy.ndarray
             The wake frame coordinates of the evaluation
-            points, shape: (n_states, n_points, 3)
+            points, shape: (n_states, n_targets, n_tpoints, 3)
 
         """
-        points = pdata[FC.POINTS]
-        n_states = mdata.n_states
-        stsel = (np.arange(n_states), states_source_turbine)
+        n_states = tdata.n_states
+        targets = tdata[FC.TARGETS]
 
-        xyz = fdata[FV.TXYH][stsel]
-        delta = points - xyz[:, None, :]
+        xyz = fdata[FV.TXYH][:, downwind_index]
+        delta = targets - xyz[:, None, None, :]
         del xyz
 
-        wd = fdata[self.var_wd][stsel]
+        wd = fdata[self.var_wd][:, downwind_index]
 
         nax = np.zeros((n_states, 3, 3), dtype=FC.DTYPE)
         n = nax[:, 0, :2]
         n[:] = wd2uv(wd, axis=-1)
         m = nax[:, 1, :2]
         m[:] = np.stack([-n[:, 1], n[:, 0]], axis=-1)
         nax[:, 2, 2] = 1
         del wd
 
-        coos = np.einsum("spd,sad->spa", delta, nax)
+        coos = np.einsum("stpd,sad->stpa", delta, nax)
 
         return coos
 
-    def get_centreline_points(self, algo, mdata, fdata, states_source_turbine, x):
+    def get_centreline_points(self, algo, mdata, fdata, downwind_index, x):
         """
         Gets the points along the centreline for given
         values of x.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        downwind_index: int
+            The index in the downwind order
         x: numpy.ndarray
             The wake frame x coordinates, shape: (n_states, n_points)
 
         Returns
         -------
         points: numpy.ndarray
             The centreline points, shape: (n_states, n_points, 3)
 
         """
-        n_states = mdata.n_states
-        stsel = (np.arange(n_states), states_source_turbine)
-
-        wd = fdata[self.var_wd][stsel]
+        wd = fdata[self.var_wd][:, downwind_index]
         n = np.append(wd2uv(wd, axis=-1), np.zeros_like(wd)[:, None], axis=-1)
 
-        xyz = fdata[FV.TXYH][stsel]
+        xyz = fdata[FV.TXYH][:, downwind_index]
         return xyz[:, None, :] + x[:, :, None] * n[:, None, :]
```

### Comparing `foxes-0.6.2/foxes/models/wake_frames/seq_dynamic_wakes.py` & `foxes-0.7/foxes/core/wake_frame.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,35 @@
+from abc import abstractmethod
 import numpy as np
-from scipy.spatial.distance import cdist
+from scipy.interpolate import interpn
 
-from foxes.core import WakeFrame
-from foxes.utils import wd2uv
-from foxes.core.data import Data
-import foxes.variables as FV
+from foxes.utils import all_subclasses
 import foxes.constants as FC
-from foxes.algorithms import Sequential
-
-
-class SeqDynamicWakes(WakeFrame):
-    """
-    Dynamic wakes for the sequential algorithm.
+import foxes.variables as FV
 
-    Attributes
-    ----------
-    cl_ipars: dict
-        Interpolation parameters for centre line
-        point interpolation
-    dt_min: float, optional
-        The delta t value in minutes,
-        if not from timeseries data
+from .data import Data
+from .model import Model
 
-    :group: models.wake_frames.sequential
 
+class WakeFrame(Model):
     """
+    Abstract base class for wake frames.
 
-    def __init__(self, cl_ipars={}, dt_min=None):
-        """
-        Constructor.
-
-        Parameters
-        ----------
-        cl_ipars: dict
-            Interpolation parameters for centre line
-            point interpolation
-        dt_min: float, optional
-            The delta t value in minutes,
-            if not from timeseries data
-
-        """
-        super().__init__()
-        self.cl_ipars = cl_ipars
-        self.dt_min = dt_min
-
-    def initialize(self, algo, verbosity=0):
-        """
-        Initializes the model.
+    Wake frames translate global coordinates into
+    wake frame coordinates, which are then evaluated
+    by wake models.
 
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
+    They are also responsible for the calculation of
+    the turbine evaluation order.
 
-        """
-        super().initialize(algo, verbosity)
-        if not isinstance(algo, Sequential):
-            raise TypeError(
-                f"Incompatible algorithm type {type(algo).__name__}, expecting {Sequential.__name__}"
-            )
-
-        # determine time step:
-        times = np.asarray(algo.states.index())
-        if self.dt_min is None:
-            if not np.issubdtype(times.dtype, np.datetime64):
-                raise TypeError(
-                    f"{self.name}: Expecting state index of type np.datetime64, found {times.dtype}"
-                )
-            elif len(times) == 1:
-                raise KeyError(
-                    f"{self.name}: Expecting 'dt_min' for single step timeseries"
-                )
-            self._dt = (
-                (times[1:] - times[:-1]).astype("timedelta64[s]").astype(FC.ITYPE)
-            )
-        else:
-            n = max(len(times) - 1, 1)
-            self._dt = np.full(n, self.dt_min * 60, dtype="timedelta64[s]").astype(
-                FC.ITYPE
-            )
+    :group: core
 
-        # init wake traces data:
-        self._traces_p = np.zeros((algo.n_states, algo.n_turbines, 3), dtype=FC.DTYPE)
-        self._traces_v = np.zeros((algo.n_states, algo.n_turbines, 3), dtype=FC.DTYPE)
-        self._traces_l = np.zeros((algo.n_states, algo.n_turbines), dtype=FC.DTYPE)
+    """
 
+    @abstractmethod
     def calc_order(self, algo, mdata, fdata):
         """ "
         Calculates the order of turbine evaluation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
@@ -105,183 +44,298 @@
 
         Returns
         -------
         order: numpy.ndarray
             The turbine order, shape: (n_states, n_turbines)
 
         """
+        pass
 
-        # prepare:
-        n_states = fdata.n_states
-        n_turbines = algo.n_turbines
-        pdata = Data.from_points(points=fdata[FV.TXYH])
-
-        # calculate streamline x coordinates for turbines rotor centre points:
-        # n_states, n_turbines_source, n_turbines_target
-        coosx = np.zeros((n_states, n_turbines, n_turbines), dtype=FC.DTYPE)
-        for ti in range(n_turbines):
-            coosx[:, ti, :] = self.get_wake_coos(
-                algo, mdata, fdata, pdata, np.full(n_states, ti)
-            )[..., 0]
-
-        # derive turbine order:
-        # TODO: Remove loop over states
-        order = np.zeros((n_states, n_turbines), dtype=FC.ITYPE)
-        for si in range(n_states):
-            order[si] = np.lexsort(keys=coosx[si])
-
-        return order
-
-    def get_wake_coos(self, algo, mdata, fdata, pdata, states_source_turbine):
+    @abstractmethod
+    def get_wake_coos(
+        self,
+        algo,
+        mdata,
+        fdata,
+        tdata,
+        downwind_index,
+    ):
         """
-        Calculate wake coordinates.
+        Calculate wake coordinates of rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
 
         Returns
         -------
         wake_coos: numpy.ndarray
             The wake frame coordinates of the evaluation
-            points, shape: (n_states, n_points, 3)
+            points, shape: (n_states, n_targets, n_tpoints, 3)
 
         """
-
-        # prepare:
-        n_states = 1
-        n_points = pdata.n_points
-        points = pdata[FC.POINTS]
-        stsel = (np.arange(n_states), states_source_turbine)
-        tindx = states_source_turbine[0]
-        counter = algo.states.counter
-        N = counter + 1
-
-        # new wake starts at turbine:
-        self._traces_p[counter, tindx] = fdata[FV.TXYH][0, tindx]
-        self._traces_l[counter, tindx] = 0
-
-        # transport wakes that originate from previous time steps:
-        if counter > 0:
-            dxyz = self._traces_v[:counter, tindx] * self._dt[:counter, None]
-            self._traces_p[:counter, tindx] += dxyz
-            self._traces_l[:counter, tindx] += np.linalg.norm(dxyz, axis=-1)
-
-        # compute wind vectors at wake traces:
-        # TODO: dz from U_z is missing here
-        hpdata = {
-            v: np.zeros((1, N), dtype=FC.DTYPE)
-            for v in algo.states.output_point_vars(algo)
-        }
-        hpdata[FC.POINTS] = self._traces_p[None, :N, tindx]
-        hpdims = {FC.POINTS: (FC.STATE, FC.POINT, FC.XYH)}
-        hpdims.update({v: (FC.STATE, FC.POINT) for v in hpdata.keys()})
-        hpdata = Data(hpdata, hpdims, loop_dims=[FC.STATE, FC.POINT])
-        res = algo.states.calculate(algo, mdata, fdata, hpdata)
-        self._traces_v[:N, tindx, :2] = wd2uv(res[FV.WD][0], res[FV.WS][0])
-        del hpdata, hpdims, res
-
-        # project:
-        dists = cdist(points[0], self._traces_p[:N, tindx])
-        tri = np.argmin(dists, axis=1)
-        del dists
-        wcoos = np.full((n_states, n_points, 3), 1e20, dtype=FC.DTYPE)
-        wcoos[0, :, 2] = points[0, :, 2] - fdata[FV.TXYH][stsel][0, None, 2]
-        delp = points[0, :, :2] - self._traces_p[tri, tindx, :2]
-        nx = self._traces_v[tri, tindx, :2]
-        nx /= np.linalg.norm(nx, axis=1)[:, None]
-        ny = np.concatenate([-nx[:, 1, None], nx[:, 0, None]], axis=1)
-        wcoos[0, :, 0] = np.einsum("pd,pd->p", delp, nx) + self._traces_l[tri, tindx]
-        wcoos[0, :, 1] = np.einsum("pd,pd->p", delp, ny)
-
-        # turbines that cause wake:
-        pdata.add(FC.STATE_SOURCE_TURBINE, states_source_turbine, (FC.STATE,))
-
-        # states that cause wake for each target point:
-        pdata.add(FC.STATES_SEL, tri[None, :], (FC.STATE, FC.POINT))
-
-        return wcoos
+        pass
 
     def get_wake_modelling_data(
         self,
         algo,
         variable,
-        states_source_turbine,
+        downwind_index,
         fdata,
-        pdata,
+        tdata,
+        target,
         states0=None,
+        upcast=False,
     ):
         """
         Return data that is required for computing the
         wake from source turbines to evaluation points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm, optional
             The algorithm, needed for data from previous iteration
         variable: str
             The variable, serves as data key
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        fdata: foxes.core.Data
+        downwind_index: int, optional
+            The index in the downwind order
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
+        tdata: foxes.core.TData
+            The target point data
+        target: str, optional
+            The dimensions identifier for the output,
+            FC.STATE_TURBINE, FC.STATE_TARGET,
+            FC.STATE_TARGET_TPOINT
         states0: numpy.ndarray, optional
             The states of wake creation
+        upcast: bool
+            Flag for ensuring targets dimension,
+            otherwise dimension 1 is entered
 
-        """
-        if states0 is None:
-            # from previous iteration:
-            if not np.all(states_source_turbine == pdata[FC.STATE_SOURCE_TURBINE]):
-                raise ValueError(
-                    f"Model '{self.name}': Mismatch of 'states_source_turbine'. Expected {list(pdata[FC.STATE_SOURCE_TURBINE])}, got {list(states_source_turbine)}"
-                )
-
-            s = pdata[FC.STATES_SEL]
-            data = algo.farm_results[variable].to_numpy()
+        Returns
+        -------
+        data: numpy.ndarray
+            Data for wake modelling, shape:
+            (n_states, n_turbines) or (n_states, n_target)
+        dims: tuple
+            The data dimensions
 
-            return data[s, states_source_turbine]
+        """
+        n_states = fdata.n_states
+        s = np.s_[:] if states0 is None else states0
 
+        if not upcast:
+            if target == FC.STATE_TARGET_TPOINT:
+                out = fdata[variable][s, downwind_index, None, None]
+                dims = (FC.STATE, 1, 1)
+            else:
+                out = fdata[variable][s, downwind_index, None]
+                dims = (FC.STATE, 1)
+        elif target == FC.STATE_TURBINE:
+            out = np.zeros((n_states, fdata.n_turbines), dtype=FC.DTYPE)
+            out[:] = fdata[variable][s, downwind_index, None]
+            dims = (FC.STATE, FC.TURBINE)
+        elif target == FC.STATE_TARGET:
+            out = np.zeros((n_states, tdata.n_targets), dtype=FC.DTYPE)
+            out[:] = fdata[variable][s, downwind_index, None]
+            dims = (FC.STATE, FC.TARGET)
+        elif target == FC.STATE_TARGET_TPOINT:
+            out = np.zeros((n_states, tdata.n_targets, tdata.n_tpoints), dtype=FC.DTYPE)
+            out[:] = fdata[variable][s, downwind_index, None, None]
+            dims = (FC.STATE, FC.TARGET, FC.TPOINT)
         else:
-            return super().get_wake_modelling_data(
-                algo, variable, states_source_turbine, fdata, pdata, states0
+            raise ValueError(
+                f"Unsupported target '{target}', expcting '{FC.STATE_TURBINE}', '{FC.STATE_TARGET}', {FC.STATE_TARGET_TPOINT}"
             )
 
-    def get_centreline_points(self, algo, mdata, fdata, states_source_turbine, x):
+        return out, dims
+
+    def get_centreline_points(self, algo, mdata, fdata, downwind_index, x):
         """
         Gets the points along the centreline for given
         values of x.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        downwind_index: int
+            The index in the downwind order
         x: numpy.ndarray
             The wake frame x coordinates, shape: (n_states, n_points)
 
         Returns
         -------
         points: numpy.ndarray
             The centreline points, shape: (n_states, n_points, 3)
 
         """
+        raise NotImplementedError(
+            f"Wake frame '{self.name}': Centreline points requested but not implemented."
+        )
+
+    def calc_centreline_integral(
+        self,
+        algo,
+        mdata,
+        fdata,
+        downwind_index,
+        variables,
+        x,
+        dx,
+        wake_models=None,
+        self_wake=True,
+        **ipars,
+    ):
+        """
+        Integrates variables along the centreline.
 
-        raise NotImplementedError
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.MData
+            The model data
+        fdata: foxes.core.FData
+            The farm data
+        downwind_index: int
+            The index in the downwind order
+        variables: list of str
+            The variables to be integrated
+        x: numpy.ndarray
+            The wake frame x coordinates of the upper integral bounds,
+            shape: (n_states, n_points)
+        dx: float
+            The step size of the integral
+        wake_models: list of foxes.core.WakeModels
+            The wake models to consider, default: from algo
+        self_wake: bool
+            Flag for considering only wake from states_source_turbine
+        ipars: dict, optional
+            Additional interpolation parameters
+
+        Returns
+        -------
+        results: numpy.ndarray
+            The integration results, shape: (n_states, n_points, n_vars)
+
+        """
+        # prepare:
+        n_states, n_points = x.shape
+        vrs = [FV.amb2var.get(v, v) for v in variables]
+        n_vars = len(vrs)
+
+        # calc evaluation points:
+        xmin = 0.0
+        xmax = np.nanmax(x)
+        n_steps = int((xmax - xmin) / dx)
+        if xmin + n_steps * dx < xmax:
+            n_steps += 1
+        n_ix = n_steps + 1
+        xs = np.arange(xmin, xmin + n_ix * dx, dx)
+        xpts = np.zeros((n_states, n_steps), dtype=FC.DTYPE)
+        xpts[:] = xs[None, 1:]
+        pts = self.get_centreline_points(algo, mdata, fdata, downwind_index, xpts)
+
+        # run ambient calculation:
+        tdata = Data.from_points(
+            pts,
+            data={
+                v: np.full((n_states, n_steps, 1), np.nan, dtype=FC.DTYPE) for v in vrs
+            },
+            dims={v: (FC.STATE, FC.TARGET, FC.TPOINT) for v in vrs},
+        )
+        res = algo.states.calculate(algo, mdata, fdata, tdata)
+        tdata.update(res)
+        amb2var = algo.get_model("SetAmbPointResults")()
+        amb2var.initialize(algo, verbosity=0)
+        res = amb2var.calculate(algo, mdata, fdata, tdata)
+        tdata.update(res)
+        del res, amb2var
+
+        # find out if all vars ambient:
+        ambient = True
+        for v in variables:
+            if v not in FV.amb2var:
+                ambient = False
+                break
+
+        # calc wakes:
+        if not ambient:
+            wcalc = algo.get_model("PointWakesCalculation")(wake_models=wake_models)
+            wcalc.initialize(algo, verbosity=0)
+            wsrc = downwind_index if self_wake else None
+            res = wcalc.calculate(algo, mdata, fdata, tdata, downwind_index=wsrc)
+            tdata.update(res)
+            del wcalc, res
+
+        # collect integration results:
+        iresults = np.zeros((n_states, n_ix, n_vars), dtype=FC.DTYPE)
+        for vi, v in enumerate(variables):
+            for i in range(n_steps):
+                iresults[:, i + 1, vi] = iresults[:, i, vi] + tdata[v][:, i, 0] * dx
+
+        # interpolate to x of interest:
+        qts = np.zeros((n_states, n_points, 2), dtype=FC.DTYPE)
+        qts[:, :, 0] = np.arange(n_states)[:, None]
+        qts[:, :, 1] = x
+        qts = qts.reshape(n_states * n_points, 2)
+        results = interpn(
+            (np.arange(n_states), xs),
+            iresults,
+            qts,
+            bounds_error=False,
+            fill_value=0.0,
+            **ipars,
+        )
+
+        return results.reshape(n_states, n_points, n_vars)
+
+    @classmethod
+    def new(cls, wframe_type, *args, **kwargs):
+        """
+        Run-time wake frame factory.
+
+        Parameters
+        ----------
+        wframe_type: str
+            The selected derived class name
+        args: tuple, optional
+            Additional parameters for constructor
+        kwargs: dict, optional
+            Additional parameters for constructor
+
+        """
+
+        if wframe_type is None:
+            return None
+
+        allc = all_subclasses(cls)
+        found = wframe_type in [scls.__name__ for scls in allc]
+
+        if found:
+            for scls in allc:
+                if scls.__name__ == wframe_type:
+                    return scls(*args, **kwargs)
+
+        else:
+            estr = (
+                "Wake frame type '{}' is not defined, available types are \n {}".format(
+                    wframe_type, sorted([i.__name__ for i in allc])
+                )
+            )
+            raise KeyError(estr)
```

### Comparing `foxes-0.6.2/foxes/models/wake_frames/streamlines.py` & `foxes-0.7/foxes/models/wake_frames/streamlines.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from scipy.interpolate import interpn
 
 from foxes.core import WakeFrame
 from foxes.utils import wd2uv
-from foxes.core.data import Data
+from foxes.core.data import TData
 import foxes.variables as FV
 import foxes.constants as FC
 
 
 class Streamlines2D(WakeFrame):
     """
     Streamline following wakes
@@ -43,17 +43,19 @@
         """
         super().__init__()
         self.step = step
         self.max_length = max_length
         self.cl_ipars = cl_ipars
 
         self.DATA = self.var("DATA")
+        self.STEPS = self.var("STEPS")
+        self.SDAT = self.var("SDAT")
 
     def __repr__(self):
-        return super().__repr__() + f"(step={self.step})"
+        return f"{type(self).__name__}(step={self.step})"
 
     def _calc_streamlines(self, algo, mdata, fdata):
         """
         Helper function that computes all streamline data
         """
         # prepare:
         n_states = mdata.n_states
@@ -76,27 +78,25 @@
                 xyz = data[:, :, i - 1, :3]
                 n = wd2uv(data[:, :, i - 1, 3])
                 data[:, :, i, :2] = xyz[:, :, :2] + self.step * n
                 data[:, :, i, 2] = xyz[:, :, 2]
 
                 # calculate next tangential vector:
                 svars = algo.states.output_point_vars(algo)
-                pdata = {FC.POINTS: data[:, :, i, :3]}
-                pdims = {FC.POINTS: (FC.STATE, FC.POINT, FC.XYH)}
-                pdata.update(
-                    {
-                        v: np.full((n_states, n_turbines), np.nan, dtype=FC.DTYPE)
+                tdata = TData.from_points(
+                    data[:, :, i, :3],
+                    data={
+                        v: np.full((n_states, n_turbines, 1), np.nan, dtype=FC.DTYPE)
                         for v in svars
-                    }
+                    },
+                    dims={v: (FC.STATE, FC.TARGET, FC.TPOINT) for v in svars},
                 )
-                pdims.update({v: (FC.STATE, FC.POINT) for v in svars})
-                pdata = Data(pdata, pdims, loop_dims=[FC.STATE, FC.POINT])
-                data[:, :, i, 3] = algo.states.calculate(algo, mdata, fdata, pdata)[
+                data[:, :, i, 3] = algo.states.calculate(algo, mdata, fdata, tdata)[
                     FV.WD
-                ]
+                ][:, :, 0]
 
                 sel = np.isnan(data[:, :, i, 3])
                 if np.any(sel):
                     data[sel, i, 3] = data[sel, i - 1, 3]
 
         return data
 
@@ -104,47 +104,48 @@
         """
         Gets streamline data, generating it on the fly
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
 
         Returns
         -------
         data: numpy.ndarray
             The streamline data, shape:
             (n_states, n_turbines, n_steps, 4)
             with data x, y, z, wd
 
         """
         if self.DATA not in mdata or not np.all(
             mdata[self.DATA][:, :, 0, :3] == fdata[FV.TXYH]
         ):
             mdata[self.DATA] = self._calc_streamlines(algo, mdata, fdata)
+            mdata.dims[self.DATA] = (FC.STATE, FC.TURBINE, self.STEPS, self.SDAT)
 
         return mdata[self.DATA]
 
-    def _calc_coos(self, algo, mdata, fdata, points, states_source_turbine):
+    def _calc_coos(self, algo, mdata, fdata, targets, downwind_index):
         """
         Helper function, calculates streamline coordinates
         for given points and given turbine
         """
 
         # prepare:
-        n_states = mdata.n_states
-        n_points = points.shape[1]
-        st_sel = (np.arange(n_states), states_source_turbine)
+        n_states, n_targets, n_tpoints = targets.shape[:3]
+        n_points = n_targets * n_tpoints
+        points = targets.reshape(n_states, n_points, 3)
 
         # find nearest streamline points:
-        data = self.get_streamline_data(algo, mdata, fdata)[st_sel]
+        data = self.get_streamline_data(algo, mdata, fdata)[:, downwind_index]
         dists = np.linalg.norm(points[:, :, None, :2] - data[:, None, :, :2], axis=-1)
         selp = np.argmin(dists, axis=2)
         data = np.take_along_axis(data[:, None], selp[:, :, None, None], axis=2)[
             :, :, 0
         ]
         slen = self.step * selp
         del dists, selp
@@ -154,104 +155,108 @@
         nx = wd2uv(data[:, :, 3])
         ny = np.stack([-nx[:, :, 1], nx[:, :, 0]], axis=2)
         delta = points[:, :, :2] - data[:, :, :2]
         coos[:, :, 0] = slen + np.einsum("spd,spd->sp", delta, nx)
         coos[:, :, 1] = np.einsum("spd,spd->sp", delta, ny)
         coos[:, :, 2] = points[:, :, 2] - data[:, :, 2]
 
-        return coos
+        return coos.reshape(n_states, n_targets, n_tpoints, 3)
 
     def calc_order(self, algo, mdata, fdata):
         """ "
         Calculates the order of turbine evaluation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
 
         Returns
         -------
         order: numpy.ndarray
             The turbine order, shape: (n_states, n_turbines)
 
         """
         # prepare:
         n_states = fdata.n_states
         n_turbines = algo.n_turbines
-        pdata = Data.from_points(points=fdata[FV.TXYH])
+        tdata = TData.from_points(points=fdata[FV.TXYH])
 
         # calculate streamline x coordinates for turbines rotor centre points:
         # n_states, n_turbines_source, n_turbines_target
         coosx = np.zeros((n_states, n_turbines, n_turbines), dtype=FC.DTYPE)
         for ti in range(n_turbines):
-            coosx[:, ti, :] = self.get_wake_coos(
-                algo, mdata, fdata, pdata, np.full(n_states, ti)
-            )[..., 0]
+            coosx[:, ti, :] = self.get_wake_coos(algo, mdata, fdata, tdata, ti)[
+                :, :, 0, 0
+            ]
 
         # derive turbine order:
         # TODO: Remove loop over states
         order = np.zeros((n_states, n_turbines), dtype=FC.ITYPE)
         for si in range(n_states):
             order[si] = np.lexsort(keys=coosx[si])
 
         return order
 
-    def get_wake_coos(self, algo, mdata, fdata, pdata, states_source_turbine):
+    def get_wake_coos(
+        self,
+        algo,
+        mdata,
+        fdata,
+        tdata,
+        downwind_index,
+    ):
         """
-        Calculate wake coordinates.
+        Calculate wake coordinates of rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
 
         Returns
         -------
         wake_coos: numpy.ndarray
             The wake frame coordinates of the evaluation
-            points, shape: (n_states, n_points, 3)
+            points, shape: (n_states, n_targets, n_tpoints, 3)
 
         """
-        return self._calc_coos(
-            algo, mdata, fdata, pdata[FC.POINTS], states_source_turbine
-        )
+        return self._calc_coos(algo, mdata, fdata, tdata[FC.TARGETS], downwind_index)
 
-    def get_centreline_points(self, algo, mdata, fdata, states_source_turbine, x):
+    def get_centreline_points(self, algo, mdata, fdata, downwind_index, x):
         """
         Gets the points along the centreline for given
         values of x.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        downwind_index: int
+            The index in the downwind order
         x: numpy.ndarray
             The wake frame x coordinates, shape: (n_states, n_points)
 
         Returns
         -------
         points: numpy.ndarray
             The centreline points, shape: (n_states, n_points, 3)
@@ -259,16 +264,15 @@
         """
         # calculate long enough streamlines:
         xmax = np.max(x)
         self._ensure_min_length(algo, mdata, fdata, xmax)
 
         # get streamline points:
         n_states, n_points = x.shape
-        st_sel = (np.arange(n_states), states_source_turbine)
-        data = self.get_streamline_data(algo, mdata, fdata)[st_sel]
+        data = self.get_streamline_data(algo, mdata, fdata)[:, downwind_index]
         spts = data[:, :, :3]
         n_spts = spts.shape[1]
         xs = self.step * np.arange(n_spts)
 
         # interpolate to x of interest:
         qts = np.zeros((n_states, n_points, 2), dtype=FC.DTYPE)
         qts[:, :, 0] = np.arange(n_states)[:, None]
```

### Comparing `foxes-0.6.2/foxes/models/wake_models/dist_sliced.py` & `foxes-0.7/foxes/models/wake_models/ti/iec_ti.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,224 +1,232 @@
-from abc import abstractmethod
+import numpy as np
 
-from foxes.core import WakeModel
+from foxes.models.wake_models.top_hat import TopHatWakeModel
+import foxes.variables as FV
+import foxes.constants as FC
 
 
-class DistSlicedWakeModel(WakeModel):
+class IECTIWake(TopHatWakeModel):
     """
-    Abstract base class for wake models for which
-    the x-denpendency can be separated from the
-    yz-dependency.
+    The TI wake model from IEC-64100-1-2005-8 (2005):
 
-    The multi-yz ability is used by the `PartialDistSlicedWake`
-    partial wakes model.
+    Notes
+    -----
+    Reference:
+    http://orbit.dtu.dk/files/3750291/2009_31.pdf
+    v2: VolLuk: corrected implementation following: IEC-64100-1-2005-8
+    (Appearently an error in the document by DTU)
+
+    and the Frandsen wake TI model, from IEC-64100 (2019):
+    http://orbit.dtu.dk/files/3750291/2009_31.pdf
 
     Attributes
     ----------
-    superpositions: dict
-        The superpositions. Key: variable name str,
-        value: The wake superposition model name,
-        will be looked up in model book
-    superp: dict
-        The superposition dict, key: variable name str,
-        value: `foxes.core.WakeSuperposition`
+    opening_angle: float
+        The wake opening angle. The wake growth parameter k is calculated
+        based on the wake opening angle.
+    k_var: str
+        The variable name for k
 
-    :group: models.wake_models
+    :group: models.wake_models.ti
 
     """
 
-    def __init__(self, superpositions):
+    def __init__(
+        self,
+        superposition,
+        opening_angle=21.6,
+        iec_type="2019",
+        k_var=FV.K,
+        **kwargs,
+    ):
         """
         Constructor.
 
         Parameters
         ----------
-        superpositions: dict
-            The superpositions. Key: variable name str,
-            value: The wake superposition model name,
-            will be looked up in model book
-
-        """
-        super().__init__()
-        self.superpositions = superpositions
-
-    def sub_models(self):
-        """
-        List of all sub-models
-
-        Returns
-        -------
-        smdls: list of foxes.core.Model
-            Names of all sub models
-
-        """
-        return list(self.superp.values())
-
-    def initialize(self, algo, verbosity=0, force=False):
-        """
-        Initializes the model.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
-        force: bool
-            Overwrite existing data
-
-        """
-        self.superp = {
-            v: algo.mbook.wake_superpositions[s] for v, s in self.superpositions.items()
-        }
-        super().initialize(algo, verbosity, force)
+        superposition: str
+            The TI wake superposition.
+        opening_angle: float
+            The wake opening angle. The wake growth parameter k is calculated
+            based on the wake opening angle.
+        k_var: str
+            The variable name for k
+        kwargs: dict, optional
+            Additional parameters for the base class
+
+        """
+        super().__init__(superpositions={FV.TI: superposition}, **kwargs)
+
+        k = float(np.tan(np.deg2rad(opening_angle / 2.0)))
+
+        self.iec_type = iec_type
+        self.k_var = k_var
+        setattr(self, k_var, k)
+
+    def __repr__(self):
+        k = getattr(self, self.k_var)
+        iname = (
+            self.induction if isinstance(self.induction, str) else self.induction.name
+        )
+        s = f"{type(self).__name__}"
+        s += f"({self.superpositions[FV.TI]}, induction={iname}"
+        if k is None:
+            s += f", k_var={self.k_var}"
+        else:
+            s += f", {self.k_var}={k}"
+        s += ")"
+        return s
 
-    @abstractmethod
-    def calc_wakes_spsel_x_yz(
-        self,
-        algo,
-        mdata,
-        fdata,
-        pdata,
-        states_source_turbine,
-        x,
-        yz,
-    ):
+    def new_wake_deltas(self, algo, mdata, fdata, tdata):
         """
-        Calculate wake deltas.
+        Creates new empty wake delta arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        x: numpy.ndarray
-            The x values, shape: (n_states, n_points)
-        yz: numpy.ndarray
-            The yz values for each x value, shape:
-            (n_states, n_points, n_yz_per_x, 2)
+        tdata: foxes.core.TData
+            The target point data
 
         Returns
         -------
-        wdeltas: dict
-            The wake deltas. Key: variable name str,
-            value: numpy.ndarray, shape: (n_sp_sel, n_yz_per_x)
-        sp_sel: numpy.ndarray of bool
-            The state-point selection, for which the wake
-            is non-zero, shape: (n_states, n_points)
+        wake_deltas: dict
+            Key: variable name, value: The zero filled
+            wake deltas, shape: (n_states, n_turbines, n_rpoints, ...)
 
         """
-        pass
+        return {FV.TI: np.zeros_like(tdata[FC.TARGETS][..., 0])}
 
-    def contribute_to_wake_deltas(
+    def calc_wake_radius(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        wake_coos,
-        wake_deltas,
+        tdata,
+        downwind_index,
+        x,
+        ct,
     ):
         """
-        Calculate the contribution to the wake deltas
-        by this wake model.
-
-        Modifies wake_deltas on the fly.
+        Calculate the wake radius, depending on x only (not r).
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        wake_coos: numpy.ndarray
-            The wake frame coordinates of the evaluation
-            points, shape: (n_states, n_points, 3)
-        wake_deltas: dict
-            The wake deltas, are being modified ob the fly.
-            Key: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
+        x: numpy.ndarray
+            The x values, shape: (n_states, n_targets)
+        ct: numpy.ndarray
+            The ct values of the wake-causing turbines,
+            shape: (n_states, n_targets)
 
-        """
-        x = wake_coos[:, :, 0]
-        yz = wake_coos[:, :, None, 1:3]
+        Returns
+        -------
+        wake_r: numpy.ndarray
+            The wake radii, shape: (n_states, n_targets)
 
-        wdeltas, sp_sel = self.calc_wakes_spsel_x_yz(
-            algo, mdata, fdata, pdata, states_source_turbine, x, yz
+        """
+        k = self.get_data(
+            self.k_var,
+            FC.STATE_TARGET,
+            lookup="sw",
+            algo=algo,
+            fdata=fdata,
+            tdata=tdata,
+            upcast=False,
+            downwind_index=downwind_index,
         )
+        return k * x
 
-        for v, hdel in wdeltas.items():
-            try:
-                superp = self.superp[v]
-            except KeyError:
-                raise KeyError(
-                    f"Model '{self.name}': Missing wake superposition entry for variable '{v}', found {sorted(list(self.superp.keys()))}"
-                )
-
-            wake_deltas[v] = superp.calc_wakes_plus_wake(
-                algo,
-                mdata,
-                fdata,
-                pdata,
-                states_source_turbine,
-                sp_sel,
-                v,
-                wake_deltas[v],
-                hdel[:, 0],
-            )
-
-    def finalize_wake_deltas(
+    def calc_centreline(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        amb_results,
-        wake_deltas,
+        tdata,
+        downwind_index,
+        st_sel,
+        x,
+        wake_r,
+        ct,
     ):
         """
-        Finalize the wake calculation.
-
-        Modifies wake_deltas on the fly.
+        Calculate centre line results of wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        amb_results: dict
-            The ambient results, key: variable name str,
-            values: numpy.ndarray with shape (n_states, n_points)
-        wake_deltas: dict
-            The wake deltas, are being modified ob the fly.
-            Key: Variable name str, for which the wake delta
-            applies, values: numpy.ndarray with shape
-            (n_states, n_points, ...) before evaluation,
-            numpy.ndarray with shape (n_states, n_points) afterwards
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
+        st_sel: numpy.ndarray of bool
+            The state-target selection, for which the wake
+            is non-zero, shape: (n_states, n_targets)
+        x: numpy.ndarray
+            The x values, shape: (n_st_sel,)
+        wake_r: numpy.ndarray
+            The wake radii, shape: (n_st_sel,)
+        ct: numpy.ndarray
+            The ct values of the wake-causing turbines,
+            shape: (n_st_sel,)
 
-        """
-        for v, s in self.superp.items():
-            wake_deltas[v] = s.calc_final_wake_delta(
-                algo, mdata, fdata, pdata, v, amb_results[v], wake_deltas[v]
+        Returns
+        -------
+        cl_del: dict
+            The centre line wake deltas. Key: variable name str,
+            varlue: numpy.ndarray, shape: (n_st_sel,)
+
+        """
+        # read D from extra data:
+        D = self.get_data(
+            FV.D,
+            FC.STATE_TARGET,
+            lookup="w",
+            algo=algo,
+            fdata=fdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
+            upcast=True,
+        )[st_sel]
+
+        # get ws:
+        ws = self.get_data(
+            FV.REWS,
+            FC.STATE_TARGET,
+            lookup="w",
+            algo=algo,
+            fdata=fdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
+            upcast=True,
+        )[st_sel]
+
+        # calculate wind deficit:
+        if self.iec_type == "2005":
+            cl_deltas = np.sqrt(0.9) / (1.5 + 0.3 * x / D * np.sqrt(ws))
+        elif self.iec_type == "2019" or self.iec_type == "Frandsen":
+            cl_deltas = 1.0 / (1.5 + 0.8 * x / D / np.sqrt(ct))
+        else:
+            raise TypeError(
+                f"Type of IEC {self.iec_type} not found. Select '2015' or '2019'/'Frandsen'."
             )
+
+        return {FV.TI: cl_deltas}
```

### Comparing `foxes-0.6.2/foxes/models/wake_models/induction/rankine_half_body.py` & `foxes-0.7/foxes/models/wake_models/induction/self_similar.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,71 @@
 import numpy as np
 
-from foxes.core import WakeModel
-from foxes.utils import uv2wd, wd2uv
+from foxes.core import TurbineInductionModel
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class RankineHalfBody(WakeModel):
+class SelfSimilar(TurbineInductionModel):
     """
-    The Rankine half body induction wake model
+    The self-similar induction wake model
+    from Troldborg and Meyer Forsting
 
     The individual wake effects are superposed linearly,
     without invoking a wake superposition model.
 
     Notes
     -----
-    Reference:
-    B Gribben and G Hawkes
-    "A potential flow model for wind turbine induction and wind farm blockage"
-    Techincal Paper, Frazer-Nash Consultancy, 2019
-    https://www.fnc.co.uk/media/o5eosxas/a-potential-flow-model-for-wind-turbine-induction-and-wind-farm-blockage.pdf
+    References:
+    [1] Troldborg, Niels, and Alexander Raul Meyer Forsting.
+    "A simple model of the wind turbine induction zone derived
+    from numerical simulations."
+    Wind Energy 20.12 (2017): 2011-2020.
+    https://onlinelibrary.wiley.com/doi/full/10.1002/we.2137
+
+    [2] Forsting, Alexander R. Meyer, et al.
+    "On the accuracy of predicting wind-farm blockage."
+    Renewable Energy (2023).
+    https://www.sciencedirect.com/science/article/pii/S0960148123007620
 
     Attributes
     ----------
+    pre_rotor_only: bool
+        Calculate only the pre-rotor region
     induction: foxes.core.AxialInductionModel or str
         The induction model
 
     :group: models.wake_models.induction
 
     """
 
-    def __init__(self, induction="Madsen"):
+    def __init__(self, pre_rotor_only=False, induction="Madsen", gamma=1.1):
         """
         Constructor.
 
         Parameters
         ----------
+        pre_rotor_only: bool
+            Calculate only the pre-rotor region
         induction: foxes.core.AxialInductionModel or str
             The induction model
+        gamma: float, default=1.1
+            The parameter that multiplies Ct in the ct2a calculation
 
         """
         super().__init__()
         self.induction = induction
+        self.pre_rotor_only = pre_rotor_only
+        self.gamma = gamma
+
+    def __repr__(self):
+        iname = (
+            self.induction if isinstance(self.induction, str) else self.induction.name
+        )
+        return f"{type(self).__name__}(gamma={self.gamma}, induction={iname})"
 
     def sub_models(self):
         """
         List of all sub-models
 
         Returns
         -------
@@ -69,213 +89,151 @@
             Overwrite existing data
 
         """
         if isinstance(self.induction, str):
             self.induction = algo.mbook.axial_induction[self.induction]
         super().initialize(algo, verbosity, force)
 
-    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
+    def new_wake_deltas(self, algo, mdata, fdata, tdata):
         """
-        Initialize wake delta storage.
-
-        They are added on the fly to the wake_deltas dict.
+        Creates new empty wake delta arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
+        tdata: foxes.core.TData
+            The target point data
+
+        Returns
+        -------
         wake_deltas: dict
-            The wake deltas storage, add wake deltas
-            on the fly. Keys: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
+            Key: variable name, value: The zero filled
+            wake deltas, shape: (n_states, n_turbines, n_rpoints, ...)
 
         """
-        n_states = mdata.n_states
-        n_points = pdata.n_points
-        wake_deltas["U"] = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        wake_deltas["V"] = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        wake_deltas[FV.WS] = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        wake_deltas[FV.WD] = np.zeros((n_states, n_points), dtype=FC.DTYPE)
+        return {FV.WS: np.zeros_like(tdata[FC.TARGETS][..., 0])}
+
+    def _mu(self, x_R):
+        """Helper function: define mu (eqn 11 from [1])"""
+        return 1 + (x_R / np.sqrt(1 + x_R**2))
+
+    def _a0(self, ct, x_R):
+        """Helper function: define a0 with gamma factor, eqn 8 from [2]"""
+        return self.induction.ct2a(self.gamma * ct)
+
+    def _a(self, ct, x_R):
+        """Helper function: define axial shape function (eqn 11 from [1])"""
+        return self._a0(ct, x_R) * self._mu(x_R)
+
+    def _r_half(self, x_R):
+        """Helper function: using eqn 13 from [2]"""
+        return np.sqrt(0.587 * (1.32 + x_R**2))
+
+    def _rad_fn(self, x_R, r_R, beta=np.sqrt(2), alpha=8 / 9):
+        """Helper function: define radial shape function (eqn 12 from [1])"""
+        return (1 / np.cosh(beta * (r_R) / self._r_half(x_R))) ** alpha  # * (x_R < 0)
 
-    def contribute_to_wake_deltas(
+    def contribute(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
+        tdata,
+        downwind_index,
         wake_coos,
         wake_deltas,
     ):
         """
-        Calculate the contribution to the wake deltas
-        by this wake model.
-
-        Modifies wake_deltas on the fly.
+        Modifies wake deltas at target points by
+        contributions from the specified wake source turbines.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
         wake_coos: numpy.ndarray
             The wake frame coordinates of the evaluation
-            points, shape: (n_states, n_points, 3)
+            points, shape: (n_states, n_targets, n_tpoints, 3)
         wake_deltas: dict
-            The wake deltas, are being modified ob the fly.
-            Key: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
+            The wake deltas. Key: variable name,
+            value: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints, ...)
 
         """
-
-        # get x, y and z
-        x = wake_coos[:, :, 0]
-        y = wake_coos[:, :, 1]
-        z = wake_coos[:, :, 2]
-
-        # get ct:
+        # get ct
         ct = self.get_data(
             FV.CT,
-            FC.STATE_POINT,
+            FC.STATE_TARGET_TPOINT,
             lookup="w",
             algo=algo,
             fdata=fdata,
-            pdata=pdata,
+            tdata=tdata,
             upcast=True,
-            states_source_turbine=states_source_turbine,
+            downwind_index=downwind_index,
         )
 
-        # get ws:
+        # get ws
         ws = self.get_data(
             FV.REWS,
-            FC.STATE_POINT,
+            FC.STATE_TARGET_TPOINT,
             lookup="w",
             algo=algo,
             fdata=fdata,
-            pdata=pdata,
+            tdata=tdata,
             upcast=True,
-            states_source_turbine=states_source_turbine,
+            downwind_index=downwind_index,
         )
 
-        # get D
-        D = self.get_data(
+        # get R
+        R = 0.5 * self.get_data(
             FV.D,
-            FC.STATE_POINT,
+            FC.STATE_TARGET_TPOINT,
             lookup="w",
             algo=algo,
             fdata=fdata,
-            pdata=pdata,
-            upcast=True,
-            states_source_turbine=states_source_turbine,
-        )
-
-        # calc m (page 7, skipping pi everywhere)
-        m = 2 * ws * self.induction.ct2a(ct) * (D / 2) ** 2
-
-        # get r and theta
-        r = np.sqrt(y**2 + z**2)
-        r_sph = np.sqrt(r**2 + x**2)
-        theta = np.arctan2(r, x)
-
-        # define rankine half body shape (page 3)
-        RHB_shape = (
-            np.cos(theta) - (2 / (m + 1e-15)) * ws * (r_sph * np.sin(theta)) ** 2
+            tdata=tdata,
+            upcast=False,
+            downwind_index=downwind_index,
         )
 
-        # stagnation point condition
-        xs = -np.sqrt(m / (4 * ws))
-
-        # set values out of body shape
-        sp_sel = (ct > 0) & ((RHB_shape < -1) | (x < xs))
-        if np.any(sp_sel):
-            # apply selection
-            xyz = wake_coos[sp_sel]
-
-            # calc velocity components
-            vel_factor = m[sp_sel] / (4 * np.linalg.norm(xyz, axis=-1) ** 3)
-            wake_deltas["U"][sp_sel] += vel_factor * xyz[:, 0]
-            wake_deltas["V"][sp_sel] += vel_factor * xyz[:, 1]
+        # get x, r and R etc. Rounding for safe x < 0 condition below
+        x_R = np.round(wake_coos[..., 0] / R, 12)
+        r_R = np.linalg.norm(wake_coos[..., 1:3], axis=-1) / R
 
-        # set values inside body shape
-        sp_sel = (ct > 0) & (RHB_shape >= -1) & (x >= xs) & (x < 0)
+        # select values
+        sp_sel = (ct > 0) & (x_R <= 0)  # upstream
         if np.any(sp_sel):
-            # apply selection
-            xyz = np.zeros_like(wake_coos[sp_sel])
-            xyz[:, 0] = xs[sp_sel]
-
-            # calc velocity components
-            vel_factor = m[sp_sel] / (4 * np.linalg.norm(xyz, axis=-1) ** 3)
-            wake_deltas["U"][sp_sel] += vel_factor * xyz[:, 0]
+            # velocity eqn 10 from [1]
+            xr = x_R[sp_sel]
+            blockage = (
+                ws[sp_sel] * self._a(ct[sp_sel], xr) * self._rad_fn(xr, r_R[sp_sel])
+            )
+            wake_deltas[FV.WS][sp_sel] -= blockage
+
+        # set area behind to mirrored value EXCEPT for area behind turbine
+        if not self.pre_rotor_only:
+            sp_sel = (ct > 0) & (x_R > 0) & (r_R > 1)
+            if np.any(sp_sel):
+                # velocity eqn 10 from [1]
+                xr = x_R[sp_sel]
+                blockage = (
+                    ws[sp_sel]
+                    * self._a(ct[sp_sel], -xr)
+                    * self._rad_fn(-xr, r_R[sp_sel])
+                )
+                wake_deltas[FV.WS][sp_sel] += blockage
 
         return wake_deltas
-
-    def finalize_wake_deltas(
-        self,
-        algo,
-        mdata,
-        fdata,
-        pdata,
-        amb_results,
-        wake_deltas,
-    ):
-        """
-        Finalize the wake calculation.
-
-        Modifies wake_deltas on the fly.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        amb_results: dict
-            The ambient results, key: variable name str,
-            values: numpy.ndarray with shape (n_states, n_points)
-        wake_deltas: dict
-            The wake deltas, are being modified ob the fly.
-            Key: Variable name str, for which the wake delta
-            applies, values: numpy.ndarray with shape
-            (n_states, n_points, ...) before evaluation,
-            numpy.ndarray with shape (n_states, n_points) afterwards
-
-        """
-
-        # calc ambient wind vector:
-        ws0 = amb_results[FV.WS]
-        nx = wd2uv(amb_results[FV.WD])
-        wind_vec = nx * ws0[:, :, None]
-
-        # wake deltas are in wake frame, rotate back to global frame:
-        ny = np.stack((-nx[:, :, 1], nx[:, :, 0]), axis=2)
-        delta_uv = wake_deltas["U"][:, :, None] * nx + wake_deltas["V"][:, :, None] * ny
-        del ws0, nx, ny
-
-        # add ambient result to wake deltas:
-        wind_vec += delta_uv
-        del delta_uv
-
-        # deduce WS and WD deltas:
-        new_wd = uv2wd(wind_vec)
-        new_ws = np.linalg.norm(wind_vec, axis=-1)
-        wake_deltas[FV.WS] += new_ws - amb_results[FV.WS]
-        wake_deltas[FV.WD] += new_wd - amb_results[FV.WD]
```

### Comparing `foxes-0.6.2/foxes/models/wake_models/induction/rathmann.py` & `foxes-0.7/foxes/models/wake_models/induction/rathmann.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
-from foxes.core import WakeModel
+from foxes.core import TurbineInductionModel
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class Rathmann(WakeModel):
+class Rathmann(TurbineInductionModel):
     """
     The Rathmann induction wake model
 
     The individual wake effects are superposed linearly,
     without invoking a wake superposition model.
 
     Notes
@@ -43,14 +43,20 @@
             The induction model
 
         """
         super().__init__()
         self.induction = induction
         self.pre_rotor_only = pre_rotor_only
 
+    def __repr__(self):
+        iname = (
+            self.induction if isinstance(self.induction, str) else self.induction.name
+        )
+        return f"{type(self).__name__}(induction={iname})"
+
     def sub_models(self):
         """
         List of all sub-models
 
         Returns
         -------
         smdls: list of foxes.core.Model
@@ -73,124 +79,113 @@
             Overwrite existing data
 
         """
         if isinstance(self.induction, str):
             self.induction = algo.mbook.axial_induction[self.induction]
         super().initialize(algo, verbosity, force)
 
-    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
+    def new_wake_deltas(self, algo, mdata, fdata, tdata):
         """
-        Initialize wake delta storage.
-
-        They are added on the fly to the wake_deltas dict.
+        Creates new empty wake delta arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
+        tdata: foxes.core.TData
+            The target point data
+
+        Returns
+        -------
         wake_deltas: dict
-            The wake deltas storage, add wake deltas
-            on the fly. Keys: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
+            Key: variable name, value: The zero filled
+            wake deltas, shape: (n_states, n_turbines, n_rpoints, ...)
 
         """
-        n_states = mdata.n_states
-        n_points = pdata.n_points
-        wake_deltas[FV.WS] = np.zeros((n_states, n_points), dtype=FC.DTYPE)
+        return {FV.WS: np.zeros_like(tdata[FC.TARGETS][..., 0])}
 
-    def contribute_to_wake_deltas(
+    def contribute(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
+        tdata,
+        downwind_index,
         wake_coos,
         wake_deltas,
     ):
         """
-        Calculate the contribution to the wake deltas
-        by this wake model.
-
-        Modifies wake_deltas on the fly.
+        Modifies wake deltas at target points by
+        contributions from the specified wake source turbines.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
         wake_coos: numpy.ndarray
             The wake frame coordinates of the evaluation
-            points, shape: (n_states, n_points, 3)
+            points, shape: (n_states, n_targets, n_tpoints, 3)
         wake_deltas: dict
-            The wake deltas, are being modified ob the fly.
-            Key: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
+            The wake deltas. Key: variable name,
+            value: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints, ...)
 
         """
-
-        # get x, y and z
-        x = wake_coos[:, :, 0]
-        y = wake_coos[:, :, 1]
-        z = wake_coos[:, :, 2]
-
         # get ct:
         ct = self.get_data(
             FV.CT,
-            FC.STATE_POINT,
+            FC.STATE_TARGET_TPOINT,
             lookup="w",
             algo=algo,
             fdata=fdata,
-            pdata=pdata,
+            tdata=tdata,
             upcast=True,
-            states_source_turbine=states_source_turbine,
+            downwind_index=downwind_index,
         )
 
         # get ws:
         ws = self.get_data(
             FV.REWS,
-            FC.STATE_POINT,
+            FC.STATE_TARGET_TPOINT,
             lookup="w",
             algo=algo,
             fdata=fdata,
-            pdata=pdata,
+            tdata=tdata,
             upcast=True,
-            states_source_turbine=states_source_turbine,
+            downwind_index=downwind_index,
         )
 
         # get D
-        D = self.get_data(
+        R = 0.5 * self.get_data(
             FV.D,
-            FC.STATE_POINT,
+            FC.STATE_TARGET_TPOINT,
             lookup="w",
             algo=algo,
             fdata=fdata,
-            pdata=pdata,
-            upcast=True,
-            states_source_turbine=states_source_turbine,
+            tdata=tdata,
+            upcast=False,
+            downwind_index=downwind_index,
         )
 
-        x_R = x / (D / 2)
-        r_R = np.sqrt(y**2 + z**2) / (D / 2)
+        # get x, r and R etc. Rounding for safe x < 0 condition below
+        x_R = np.round(wake_coos[..., 0] / R, 12)
+        r_R = np.linalg.norm(wake_coos[..., 1:3], axis=-1) / R
 
         def mu(x_R):
             """axial shape function at r=0 from vortex cylinder model (eqn 11)"""
             return 1 + x_R / (np.sqrt(1 + x_R**2))
 
         def G(x_R, r_R):
             """radial shape function eqn 20"""
@@ -200,27 +195,25 @@
             sin_alpha = np.sqrt(
                 0.5 * (1 - np.sqrt(1 - sin_2_alpha**2))
             )  # derived from cos(2a)**2 + sin(2a)**2 = 1
             sin_beta = 1 / np.sqrt(x_R**2 + r_R**2 + 1)  # eqn 19
             return sin_alpha * sin_beta * (1 + x_R**2)
 
         # ws delta in front of rotor
-        sp_sel = (ct > 0) & (x < 0)
+        sp_sel = (ct > 0) & (x_R <= 0)
         if np.any(sp_sel):
+            xr = x_R[sp_sel]
             a = self.induction.ct2a(ct[sp_sel])
-            blockage = (
-                ws[sp_sel] * a * mu(x_R[sp_sel]) * G(x_R[sp_sel], r_R[sp_sel])
-            )  # eqn 10
+            blockage = ws[sp_sel] * a * mu(xr) * G(xr, r_R[sp_sel])  # eqn 10
             wake_deltas[FV.WS][sp_sel] += -blockage
 
         # ws delta behind rotor
         if not self.pre_rotor_only:
             # mirror -blockage in rotor plane
-            sp_sel = (ct > 0) & (x > 0) & (r_R > 1)
+            sp_sel = (ct > 0) & (x_R > 0) & (r_R > 1)
             if np.any(sp_sel):
+                xr = x_R[sp_sel]
                 a = self.induction.ct2a(ct[sp_sel])
-                blockage = (
-                    ws[sp_sel] * a * mu(-x_R[sp_sel]) * G(-x_R[sp_sel], r_R[sp_sel])
-                )  # eqn 10
+                blockage = ws[sp_sel] * a * mu(-xr) * G(-xr, r_R[sp_sel])  # eqn 10
                 wake_deltas[FV.WS][sp_sel] += blockage
 
         return wake_deltas
```

### Comparing `foxes-0.6.2/foxes/models/wake_models/induction/self_similar2020.py` & `foxes-0.7/foxes/models/wake_models/induction/self_similar2020.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/models/wake_models/ti/iec_ti.py` & `foxes-0.7/foxes/models/wake_models/wind/bastankhah14.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,242 +1,212 @@
 import numpy as np
 
-from foxes.models.wake_models.top_hat import TopHatWakeModel
+from foxes.models.wake_models.gaussian import GaussianWakeModel
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class IECTIWake(TopHatWakeModel):
+class Bastankhah2014(GaussianWakeModel):
     """
-    The TI wake model from IEC-64100-1-2005-8 (2005):
+    The Bastankhah 2014 wake model
 
     Notes
     -----
     Reference:
-    http://orbit.dtu.dk/files/3750291/2009_31.pdf
-    v2: VolLuk: corrected implementation following: IEC-64100-1-2005-8
-    (Appearently an error in the document by DTU)
-
-    and the Frandsen wake TI model, from IEC-64100 (2019):
-    http://orbit.dtu.dk/files/3750291/2009_31.pdf
+    "A new analytical model for wind-turbine wakes"
+    Majid Bastankhah, Fernando Porté-Agel
+    https://doi.org/10.1016/j.renene.2014.01.002
 
     Attributes
     ----------
-    opening_angle: float
-        The wake opening angle. The wake growth parameter k is calculated
-        based on the wake opening angle.
+    k: float, optional
+        The wake growth parameter k. If not given here
+        it will be searched in the farm data.
+    sbeta_factor: float
+        Factor multiplying sbeta
     k_var: str
         The variable name for k
+    induction: foxes.core.AxialInductionModel or str
+        The induction model
 
-    :group: models.wake_models.ti
+    :group: models.wake_models.wind
 
     """
 
     def __init__(
         self,
         superposition,
-        opening_angle=21.6,
-        iec_type="2019",
+        k=None,
+        sbeta_factor=0.2,
         k_var=FV.K,
-        **kwargs,
+        induction="Madsen",
     ):
         """
         Constructor.
 
         Parameters
         ----------
-        superpositions: dict
-            The superpositions. Key: variable name str,
-            value: The wake superposition model name,
-            will be looked up in model book
-        opening_angle: float
-            The wake opening angle. The wake growth parameter k is calculated
-            based on the wake opening angle.
+        superposition: str
+            The wind speed deficit superposition.
+        k: float, optional
+            The wake growth parameter k. If not given here
+            it will be searched in the farm data.
+        sbeta_factor: float
+            Factor multiplying sbeta
         k_var: str
             The variable name for k
-        kwargs: dict, optional
-            Additional parameters for the base class
+        induction: foxes.core.AxialInductionModel or str
+            The induction model
 
         """
-        super().__init__(superpositions={FV.TI: superposition}, **kwargs)
-
-        k = float(np.tan(np.deg2rad(opening_angle / 2.0)))
+        super().__init__(superpositions={FV.WS: superposition})
 
-        self.iec_type = iec_type
+        self.sbeta_factor = sbeta_factor
         self.k_var = k_var
+        self.induction = induction
+
         setattr(self, k_var, k)
 
     def __repr__(self):
         k = getattr(self, self.k_var)
-        s = super().__repr__()
-        s += f"({self.k_var}={k}, sp={self.superpositions[FV.TI]})"
+        iname = (
+            self.induction if isinstance(self.induction, str) else self.induction.name
+        )
+        s = f"{type(self).__name__}"
+        s += f"({self.superpositions[FV.WS]}, induction={iname}"
+        if k is None:
+            s += f", k_var={self.k_var}"
+        else:
+            s += f", {self.k_var}={k}"
+        s += ")"
         return s
 
-    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
+    def sub_models(self):
         """
-        Initialize wake delta storage.
+        List of all sub-models
 
-        They are added on the fly to the wake_deltas dict.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        wake_deltas: dict
-            The wake deltas storage, add wake deltas
-            on the fly. Keys: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
+        Returns
+        -------
+        smdls: list of foxes.core.Model
+            All sub models
 
         """
-        n_states = mdata.n_states
-        wake_deltas[FV.TI] = np.zeros((n_states, pdata.n_points), dtype=FC.DTYPE)
+        return [self.induction]
 
-    def calc_wake_radius(
-        self,
-        algo,
-        mdata,
-        fdata,
-        pdata,
-        states_source_turbine,
-        x,
-        ct,
-    ):
+    def initialize(self, algo, verbosity=0, force=False):
         """
-        Calculate the wake radius, depending on x only (not r).
+        Initializes the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        x: numpy.ndarray
-            The x values, shape: (n_states, n_points)
-        r: numpy.ndarray
-            The radial values for each x value, shape:
-            (n_states, n_points, n_r_per_x, 2)
-        ct: numpy.ndarray
-            The ct values of the wake-causing turbines,
-            shape: (n_states, n_points)
-
-        Returns
-        -------
-        wake_r: numpy.ndarray
-            The wake radii, shape: (n_states, n_points)
+        verbosity: int
+            The verbosity level, 0 = silent
+        force: bool
+            Overwrite existing data
 
         """
+        if isinstance(self.induction, str):
+            self.induction = algo.mbook.axial_induction[self.induction]
+        super().initialize(algo, verbosity, force)
 
-        # get k:
-        k = self.get_data(
-            self.k_var,
-            FC.STATE_POINT,
-            lookup="sw",
-            algo=algo,
-            fdata=fdata,
-            pdata=pdata,
-            upcast=True,
-            states_source_turbine=states_source_turbine,
-        )
-
-        # calculate:
-        radius = k * x
-
-        return radius
-
-    def calc_centreline_wake_deltas(
+    def calc_amplitude_sigma(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        sp_sel,
+        tdata,
+        downwind_index,
         x,
-        wake_r,
-        ct,
     ):
         """
-        Calculate centre line results of wake deltas.
+        Calculate the amplitude and the sigma,
+        both depend only on x (not on r).
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        sp_sel: numpy.ndarray of bool
-            The state-point selection, for which the wake
-            is non-zero, shape: (n_states, n_points)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
         x: numpy.ndarray
-            The x values, shape: (n_sp_sel,)
-        wake_r: numpy.ndarray
-            The wake radii, shape: (n_sp_sel,)
-        ct: numpy.ndarray
-            The ct values of the wake-causing turbines,
-            shape: (n_sp_sel,)
+            The x values, shape: (n_states, n_targets)
 
         Returns
         -------
-        cl_del: dict
-            The centre line wake deltas. Key: variable name str,
-            varlue: numpy.ndarray, shape: (n_sp_sel,)
+        amsi: tuple
+            The amplitude and sigma, both numpy.ndarray
+            with shape (n_st_sel,)
+        st_sel: numpy.ndarray of bool
+            The state-target selection, for which the wake
+            is non-zero, shape: (n_states, n_targets)
 
         """
-
-        # read D from extra data:
-        D = self.get_data(
-            FV.D,
-            FC.STATE_POINT,
+        # get ct:
+        ct = self.get_data(
+            FV.CT,
+            FC.STATE_TARGET,
             lookup="w",
             algo=algo,
             fdata=fdata,
-            pdata=pdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
             upcast=True,
-            states_source_turbine=states_source_turbine,
         )
-        D = D[sp_sel]
 
-        # get ws:
-        ws = self.get_data(
-            FV.REWS,
-            FC.STATE_POINT,
-            lookup="w",
-            algo=algo,
-            fdata=fdata,
-            pdata=pdata,
-            upcast=True,
-            states_source_turbine=states_source_turbine,
-        )
-        ws = ws[sp_sel]
+        # select targets:
+        st_sel = (x > 0) & (ct > 0)
+        if np.any(st_sel):
+            # apply selection:
+            x = x[st_sel]
+            ct = ct[st_sel]
+
+            # get D:
+            D = self.get_data(
+                FV.D,
+                FC.STATE_TARGET,
+                lookup="w",
+                algo=algo,
+                fdata=fdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
+                upcast=True,
+            )[st_sel]
+
+            # get k:
+            k = self.get_data(
+                self.k_var,
+                FC.STATE_TARGET,
+                lookup="sw",
+                algo=algo,
+                fdata=fdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
+                upcast=True,
+            )[st_sel]
+
+            # calculate sigma:
+            # beta = 0.5 * (1 + np.sqrt(1.0 - ct)) / np.sqrt(1.0 - ct)
+            a = self.induction.ct2a(ct)
+            beta = (1 - a) / (1 - 2 * a)
+            sigma = k * x + self.sbeta_factor * np.sqrt(beta) * D
+            del beta, a
+
+            # calculate amplitude:
+            ct_eff = ct / (8 * (sigma / D) ** 2)
+            ampld = np.maximum(-2 * self.induction.ct2a(ct_eff), -1)
 
-        # calculate wind deficit:
-        if self.iec_type == "2005":
-            cl_deltas = np.sqrt(0.9) / (1.5 + 0.3 * x / D * np.sqrt(ws))
-        elif self.iec_type == "2019" or self.iec_type == "Frandsen":
-            cl_deltas = 1.0 / (1.5 + 0.8 * x / D / np.sqrt(ct))
+        # case no targets:
         else:
-            raise TypeError(
-                f"Type of IEC {self.iec_type} not found. Select '2015' or '2019'/'Frandsen'."
-            )
+            st_sel = np.zeros_like(x, dtype=bool)
+            n_sp = np.sum(st_sel)
+            ampld = np.zeros(n_sp, dtype=FC.DTYPE)
+            sigma = np.zeros(n_sp, dtype=FC.DTYPE)
 
-        return {FV.TI: cl_deltas}
+        return {FV.WS: (ampld, sigma)}, st_sel
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `foxes-0.6.2/foxes/models/wake_models/top_hat.py` & `foxes-0.7/foxes/models/wake_models/top_hat.py`

 * *Files 20% similar despite different names*

```diff
@@ -68,169 +68,160 @@
 
     @abstractmethod
     def calc_wake_radius(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
+        tdata,
+        downwind_index,
         x,
         ct,
     ):
         """
         Calculate the wake radius, depending on x only (not r).
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
         x: numpy.ndarray
-            The x values, shape: (n_states, n_points)
-        r: numpy.ndarray
-            The radial values for each x value, shape:
-            (n_states, n_points, n_r_per_x, 2)
+            The x values, shape: (n_states, n_targets)
         ct: numpy.ndarray
             The ct values of the wake-causing turbines,
-            shape: (n_states, n_points)
+            shape: (n_states, n_targets)
 
         Returns
         -------
         wake_r: numpy.ndarray
-            The wake radii, shape: (n_states, n_points)
+            The wake radii, shape: (n_states, n_targets)
 
         """
         pass
 
     @abstractmethod
-    def calc_centreline_wake_deltas(
+    def calc_centreline(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        sp_sel,
+        tdata,
+        downwind_index,
+        st_sel,
         x,
         wake_r,
         ct,
     ):
         """
         Calculate centre line results of wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        sp_sel: numpy.ndarray of bool
-            The state-point selection, for which the wake
-            is non-zero, shape: (n_states, n_points)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
+        st_sel: numpy.ndarray of bool
+            The state-target selection, for which the wake
+            is non-zero, shape: (n_states, n_targets)
         x: numpy.ndarray
-            The x values, shape: (n_sp_sel,)
+            The x values, shape: (n_st_sel,)
         wake_r: numpy.ndarray
-            The wake radii, shape: (n_sp_sel,)
+            The wake radii, shape: (n_st_sel,)
         ct: numpy.ndarray
             The ct values of the wake-causing turbines,
-            shape: (n_sp_sel,)
+            shape: (n_st_sel,)
 
         Returns
         -------
         cl_del: dict
             The centre line wake deltas. Key: variable name str,
-            varlue: numpy.ndarray, shape: (n_sp_sel,)
+            varlue: numpy.ndarray, shape: (n_st_sel,)
 
         """
         pass
 
-    def calc_wakes_spsel_x_r(
+    def calc_wakes_x_r(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
+        tdata,
+        downwind_index,
         x,
         r,
     ):
         """
         Calculate wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
         x: numpy.ndarray
-            The x values, shape: (n_states, n_points)
+            The x values, shape: (n_states, n_targets)
         r: numpy.ndarray
             The radial values for each x value, shape:
-            (n_states, n_points, n_r_per_x, 2)
+            (n_states, n_targets, n_yz_per_target)
 
         Returns
         -------
         wdeltas: dict
             The wake deltas. Key: variable name str,
-            value: numpy.ndarray, shape: (n_sp_sel, n_r_per_x)
-        sp_sel: numpy.ndarray of bool
-            The state-point selection, for which the wake
-            is non-zero, shape: (n_states, n_points)
+            value: numpy.ndarray, shape: (n_st_sel, n_r_per_x)
+        st_sel: numpy.ndarray of bool
+            The state-target selection, for which the wake
+            is non-zero, shape: (n_states, n_targets)
 
         """
         ct = self.get_data(
             FV.CT,
-            FC.STATE_POINT,
+            FC.STATE_TARGET,
             lookup="w",
             fdata=fdata,
-            pdata=pdata,
-            states_source_turbine=states_source_turbine,
+            tdata=tdata,
+            downwind_index=downwind_index,
             algo=algo,
+            upcast=True,
         )
 
-        wake_r = self.calc_wake_radius(
-            algo, mdata, fdata, pdata, states_source_turbine, x, ct
-        )
+        wake_r = self.calc_wake_radius(algo, mdata, fdata, tdata, downwind_index, x, ct)
 
         wdeltas = {}
-        sp_sel = (ct > 0.0) & (x > 1e-5) & np.any(r < wake_r[:, :, None], axis=2)
-        if np.any(sp_sel):
-            x = x[sp_sel]
-            r = r[sp_sel]
-            ct = ct[sp_sel]
-            wake_r = wake_r[sp_sel]
+        st_sel = (ct > 0) & (x > 0) & np.any(r < wake_r[:, :, None], axis=2)
+        if np.any(st_sel):
+            x = x[st_sel]
+            r = r[st_sel]
+            ct = ct[st_sel]
+            wake_r = wake_r[st_sel]
 
-            cl_del = self.calc_centreline_wake_deltas(
-                algo, mdata, fdata, pdata, states_source_turbine, sp_sel, x, wake_r, ct
+            cl_del = self.calc_centreline(
+                algo, mdata, fdata, tdata, downwind_index, st_sel, x, wake_r, ct
             )
 
-            nsel = r >= wake_r[:, None]
+            isin = r < wake_r[:, None]
             for v, wdel in cl_del.items():
-                wdeltas[v] = np.zeros_like(r)
-                wdeltas[v][:] = wdel[:, None]
-                wdeltas[v][nsel] = 0.0
+                wdeltas[v] = np.where(isin, wdel[:, None], 0.0)
 
-        return wdeltas, sp_sel
+        return wdeltas, st_sel
```

### Comparing `foxes-0.6.2/foxes/models/wake_models/wake_mirror.py` & `foxes-0.7/foxes/models/wake_models/wake_mirror.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,137 +47,132 @@
         -------
         smdls: list of foxes.core.Model
             All sub models
 
         """
         return [self.wmodel]
 
-    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
+    def new_wake_deltas(self, algo, mdata, fdata, tdata):
         """
-        Initialize wake delta storage.
-
-        They are added on the fly to the wake_deltas dict.
+        Creates new empty wake delta arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
+        tdata: foxes.core.TData
+            The target point data
+
+        Returns
+        -------
         wake_deltas: dict
-            The wake deltas storage, add wake deltas
-            on the fly. Keys: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
+            Key: variable name, value: The zero filled
+            wake deltas, shape: (n_states, n_turbines, n_rpoints, ...)
 
         """
-        self.wmodel.init_wake_deltas(algo, mdata, fdata, pdata, wake_deltas)
+        return self.wmodel.new_wake_deltas(algo, mdata, fdata, tdata)
 
-    def contribute_to_wake_deltas(
+    def contribute(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
+        tdata,
+        downwind_index,
         wake_coos,
         wake_deltas,
     ):
         """
-        Calculate the contribution to the wake deltas
-        by this wake model.
-
-        Modifies wake_deltas on the fly.
+        Modifies wake deltas at target points by
+        contributions from the specified wake source turbines.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
         wake_coos: numpy.ndarray
             The wake frame coordinates of the evaluation
-            points, shape: (n_states, n_points, 3)
+            points, shape: (n_states, n_targets, n_tpoints, 3)
         wake_deltas: dict
-            The wake deltas, are being modified ob the fly.
-            Key: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
+            The wake deltas. Key: variable name,
+            value: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints, ...)
 
         """
-        stsel = (np.arange(algo.n_states), states_source_turbine)
-        hh = fdata[FV.H][stsel]
-        self.wmodel.contribute_to_wake_deltas(
-            algo, mdata, fdata, pdata, states_source_turbine, wake_coos, wake_deltas
+        hh = fdata[FV.H][:, downwind_index].copy()
+        self.wmodel.contribute(
+            algo, mdata, fdata, tdata, downwind_index, wake_coos, wake_deltas
         )
 
-        pdata[FC.POINTS] = pdata[FC.POINTS].copy()  # making sure this is no ref
+        tdata[FC.TARGETS] = tdata[FC.TARGETS].copy()  # making sure this is no ref
 
         for h in self.heights:
 
-            fdata[FV.H][stsel] = hh + 2 * (h - hh)
+            fdata[FV.H][:, downwind_index] = hh + 2 * (h - hh)
 
             nwcoos = algo.wake_frame.get_wake_coos(
-                algo, mdata, fdata, pdata, states_source_turbine
+                algo, mdata, fdata, tdata, downwind_index
             )
 
-            self.wmodel.contribute_to_wake_deltas(
-                algo, mdata, fdata, pdata, states_source_turbine, nwcoos, wake_deltas
+            self.wmodel.contribute(
+                algo, mdata, fdata, tdata, downwind_index, nwcoos, wake_deltas
             )
 
-        fdata[FV.H][stsel] = hh
+        fdata[FV.H][:, downwind_index] = hh
 
     def finalize_wake_deltas(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
         amb_results,
         wake_deltas,
     ):
         """
         Finalize the wake calculation.
 
         Modifies wake_deltas on the fly.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
         amb_results: dict
             The ambient results, key: variable name str,
-            values: numpy.ndarray with shape (n_states, n_points)
+            values: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints)
         wake_deltas: dict
-            The wake deltas, are being modified ob the fly.
-            Key: Variable name str, for which the wake delta
-            applies, values: numpy.ndarray with shape
-            (n_states, n_points, ...) before evaluation,
-            numpy.ndarray with shape (n_states, n_points) afterwards
+            The wake deltas object at the selected target
+            turbines. Key: variable str, value: numpy.ndarray
+            with shape (n_states, n_targets, n_tpoints)
 
         """
         self.wmodel.finalize_wake_deltas(
-            algo, mdata, fdata, pdata, amb_results, wake_deltas
+            algo,
+            mdata,
+            fdata,
+            amb_results,
+            wake_deltas,
         )
 
 
 class GroundMirror(WakeMirror):
     """
     A wake model wrapper that adds mirror turbines
     that model wake reflection from the ground
```

### Comparing `foxes-0.6.2/foxes/models/wake_models/wind/bastankhah14.py` & `foxes-0.7/foxes/models/wake_models/wind/jensen.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,234 +1,182 @@
 import numpy as np
 
-from foxes.models.wake_models.gaussian import GaussianWakeModel
+from foxes.models.wake_models.top_hat import TopHatWakeModel
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class Bastankhah2014(GaussianWakeModel):
+class JensenWake(TopHatWakeModel):
     """
-    The Bastankhah 2014 wake model
-
-    Notes
-    -----
-    Reference:
-    "A new analytical model for wind-turbine wakes"
-    Majid Bastankhah, Fernando Porté-Agel
-    https://doi.org/10.1016/j.renene.2014.01.002
+    The Jensen wake model.
 
     Attributes
     ----------
     k: float, optional
         The wake growth parameter k. If not given here
         it will be searched in the farm data.
-    sbeta_factor: float
-        Factor multiplying sbeta
     k_var: str
         The variable name for k
-    induction: foxes.core.AxialInductionModel or str
-        The induction model
 
     :group: models.wake_models.wind
 
     """
 
-    def __init__(
-        self,
-        superposition,
-        k=None,
-        sbeta_factor=0.2,
-        k_var=FV.K,
-        induction="Madsen",
-    ):
+    def __init__(self, superposition, k=None, k_var=FV.K, **kwargs):
         """
         Constructor.
 
         Parameters
         ----------
-        superpositions: dict
-            The superpositions. Key: variable name str,
-            value: The wake superposition model name,
-            will be looked up in model book
+        superposition: str
+            The wind deficit superposition
         k: float, optional
             The wake growth parameter k. If not given here
             it will be searched in the farm data.
-        sbeta_factor: float
-            Factor multiplying sbeta
         k_var: str
             The variable name for k
-        induction: foxes.core.AxialInductionModel or str
-            The induction model
+        kwargs: dict, optional
+            Additional parameters for the base class
 
         """
-        super().__init__(superpositions={FV.WS: superposition})
+        super().__init__(superpositions={FV.WS: superposition}, **kwargs)
 
-        self.sbeta_factor = sbeta_factor
         self.k_var = k_var
-        self.induction = induction
-
         setattr(self, k_var, k)
 
     def __repr__(self):
         k = getattr(self, self.k_var)
-        s = super().__repr__()
-        s += f"({self.k_var}={k}, sp={self.superpositions[FV.WS]})"
+        iname = (
+            self.induction if isinstance(self.induction, str) else self.induction.name
+        )
+        s = f"{type(self).__name__}"
+        s += f"({self.superpositions[FV.WS]}, induction={iname}"
+        if k is None:
+            s += f", k_var={self.k_var}"
+        else:
+            s += f", {self.k_var}={k}"
+        s += ")"
         return s
 
-    def sub_models(self):
-        """
-        List of all sub-models
-
-        Returns
-        -------
-        smdls: list of foxes.core.Model
-            All sub models
-
-        """
-        return [self.induction]
-
-    def initialize(self, algo, verbosity=0, force=False):
+    def calc_wake_radius(
+        self,
+        algo,
+        mdata,
+        fdata,
+        tdata,
+        downwind_index,
+        x,
+        ct,
+    ):
         """
-        Initializes the model.
+        Calculate the wake radius, depending on x only (not r).
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
-        force: bool
-            Overwrite existing data
+        mdata: foxes.core.MData
+            The model data
+        fdata: foxes.core.FData
+            The farm data
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
+        x: numpy.ndarray
+            The x values, shape: (n_states, n_targets)
+        ct: numpy.ndarray
+            The ct values of the wake-causing turbines,
+            shape: (n_states, n_targets)
 
-        """
-        if isinstance(self.induction, str):
-            self.induction = algo.mbook.axial_induction[self.induction]
-        super().initialize(algo, verbosity, force)
+        Returns
+        -------
+        wake_r: numpy.ndarray
+            The wake radii, shape: (n_states, n_targets)
 
-    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
         """
-        Initialize wake delta storage.
-
-        They are added on the fly to the wake_deltas dict.
+        D = self.get_data(
+            FV.D,
+            FC.STATE_TARGET,
+            lookup="w",
+            algo=algo,
+            fdata=fdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
+            upcast=False,
+        )
 
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        wake_deltas: dict
-            The wake deltas storage, add wake deltas
-            on the fly. Keys: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
+        k = self.get_data(
+            self.k_var,
+            FC.STATE_TARGET,
+            lookup="sw",
+            algo=algo,
+            fdata=fdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
+            upcast=False,
+        )
 
-        """
-        wake_deltas[FV.WS] = np.zeros((mdata.n_states, pdata.n_points), dtype=FC.DTYPE)
+        return D / 2 + k * x
 
-    def calc_amplitude_sigma_spsel(
+    def calc_centreline(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
+        tdata,
+        downwind_index,
+        st_sel,
         x,
+        wake_r,
+        ct,
     ):
         """
-        Calculate the amplitude and the sigma,
-        both depend only on x (not on r).
+        Calculate centre line results of wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
+        st_sel: numpy.ndarray of bool
+            The state-target selection, for which the wake
+            is non-zero, shape: (n_states, n_targets)
         x: numpy.ndarray
-            The x values, shape: (n_states, n_points)
+            The x values, shape: (n_st_sel,)
+        wake_r: numpy.ndarray
+            The wake radii, shape: (n_st_sel,)
+        ct: numpy.ndarray
+            The ct values of the wake-causing turbines,
+            shape: (n_st_sel,)
 
         Returns
         -------
-        amsi: tuple
-            The amplitude and sigma, both numpy.ndarray
-            with shape (n_sp_sel,)
-        sp_sel: numpy.ndarray of bool
-            The state-point selection, for which the wake
-            is non-zero, shape: (n_states, n_points)
+        cl_del: dict
+            The centre line wake deltas. Key: variable name str,
+            varlue: numpy.ndarray, shape: (n_st_sel,)
 
         """
-        # get ct:
-        ct = self.get_data(
-            FV.CT,
-            FC.STATE_POINT,
-            lookup="w",
-            algo=algo,
-            fdata=fdata,
-            pdata=pdata,
-            upcast=True,
-            states_source_turbine=states_source_turbine,
-        )
-
-        # select targets:
-        sp_sel = (x > 1e-5) & (ct > 0.0)
-        if np.any(sp_sel):
-            # apply selection:
-            x = x[sp_sel]
-            ct = ct[sp_sel]
-
-            # get D:
-            D = self.get_data(
+        R = (
+            self.get_data(
                 FV.D,
-                FC.STATE_POINT,
+                FC.STATE_TARGET,
                 lookup="w",
                 algo=algo,
                 fdata=fdata,
-                pdata=pdata,
-                upcast=True,
-                states_source_turbine=states_source_turbine,
-            )
-            D = D[sp_sel]
-
-            # get k:
-            k = self.get_data(
-                self.k_var,
-                FC.STATE_POINT,
-                lookup="sw",
-                algo=algo,
-                fdata=fdata,
-                pdata=pdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
                 upcast=True,
-                states_source_turbine=states_source_turbine,
-            )
-            k = k[sp_sel]
-
-            # calculate sigma:
-            # beta = 0.5 * (1 + np.sqrt(1.0 - ct)) / np.sqrt(1.0 - ct)
-            a = self.induction.ct2a(ct)
-            beta = (1 - a) / (1 - 2 * a)
-            sigma = k * x + self.sbeta_factor * np.sqrt(beta) * D
-            del beta, a
-
-            # calculate amplitude:
-            ct_eff = ct / (8 * (sigma / D) ** 2)
-            ampld = np.maximum(-2 * self.induction.ct2a(ct_eff), -1)
+            )[st_sel]
+            / 2
+        )
 
-        # case no targets:
-        else:
-            sp_sel = np.zeros_like(x, dtype=bool)
-            n_sp = np.sum(sp_sel)
-            ampld = np.zeros(n_sp, dtype=FC.DTYPE)
-            sigma = np.zeros(n_sp, dtype=FC.DTYPE)
+        twoa = 2 * self.induction.ct2a(ct)
 
-        return {FV.WS: (ampld, sigma)}, sp_sel
+        return {FV.WS: -((R / wake_r) ** 2) * twoa}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `foxes-0.6.2/foxes/models/wake_models/wind/bastankhah16.py` & `foxes-0.7/foxes/models/wake_models/wind/bastankhah16.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     :group: models.wake_models.wind
 
     """
 
     MDATA_KEY = "Bastankhah2016Model"
     PARS = "pars"
     CHECK = "check"
-    SP_SEL = "sp_sel"
+    ST_SEL = "st_sel"
     X0 = "x0"
 
     NEAR = "near"
     R_PC = "r_pc"
     R_PC_S = "r_pc_s"
     AMPL_NEAR = "ampl_near"
     DELTA_NEAR = "delta_near"
@@ -113,138 +113,137 @@
         return dict(alpha=alpha, beta=beta, induction=self.induction.name)
 
     def calc_data(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
+        tdata,
+        downwind_index,
         x,
         gamma,
         k,
     ):
         """
         Calculate common model data, store it in mdata.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
         x: numpy.ndarray
-            The x values, shape: (n_states, n_points)
+            The x values, shape: (n_states, n_targets)
         gamma: numpy.ndarray
-            The YAWM angles in radiants, shape: (n_states, n_points)
+            The YAWM angles in radiants, shape: (n_states, n_targets)
         k: numpy.ndarray
-            The k parameter values, shape: (n_states, n_points)
+            The k parameter values, shape: (n_states, n_targets)
 
         """
 
         # store parameters:
         out = {self.PARS: self.pars}
         out[self.CHECK] = (
             mdata[FC.STATE][0],
-            states_source_turbine[0],
+            downwind_index,
             x.shape,
         )
 
         # get D:
         D = super().get_data(
             FV.D,
-            FC.STATE_POINT,
+            target=FC.STATE_TARGET,
             lookup="w",
             algo=algo,
             fdata=fdata,
-            pdata=pdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
             upcast=True,
-            states_source_turbine=states_source_turbine,
         )
 
         # get ct:
         ct = super().get_data(
             FV.CT,
-            FC.STATE_POINT,
+            target=FC.STATE_TARGET,
             lookup="w",
             algo=algo,
             fdata=fdata,
-            pdata=pdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
             upcast=True,
-            states_source_turbine=states_source_turbine,
         )
 
         # select targets:
-        sp_sel = (x > 1e-5) & (ct > 0.0)
-        if np.any(sp_sel):
+        st_sel = (x > 0) & (ct > 0.0)
+        if np.any(st_sel):
             # get ws:
             ws = super().get_data(
                 FV.REWS,
-                FC.STATE_POINT,
+                target=FC.STATE_TARGET,
                 lookup="w",
                 algo=algo,
                 fdata=fdata,
-                pdata=pdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
                 upcast=True,
-                states_source_turbine=states_source_turbine,
             )
 
             # get TI:
             ti = super().get_data(
                 FV.TI,
-                FC.STATE_POINT,
+                target=FC.STATE_TARGET,
                 lookup="w",
                 algo=algo,
                 fdata=fdata,
-                pdata=pdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
                 upcast=True,
-                states_source_turbine=states_source_turbine,
             )
 
             # get alpha:
             alpha = super().get_data(
                 FV.PA_ALPHA,
-                FC.STATE_POINT,
+                target=FC.STATE_TARGET,
                 lookup="ws",
                 algo=algo,
                 fdata=fdata,
-                pdata=pdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
                 upcast=True,
-                states_source_turbine=states_source_turbine,
             )
 
             # get beta:
             beta = super().get_data(
                 FV.PA_BETA,
-                FC.STATE_POINT,
+                target=FC.STATE_TARGET,
                 lookup="ws",
                 algo=algo,
                 fdata=fdata,
-                pdata=pdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
                 upcast=True,
-                states_source_turbine=states_source_turbine,
             )
 
             # apply filter:
-            x = x[sp_sel]
-            D = D[sp_sel]
-            ct = ct[sp_sel]
-            ws = ws[sp_sel]
-            ti = ti[sp_sel]
-            k = k[sp_sel]
-            gamma = gamma[sp_sel]
-            alpha = alpha[sp_sel]
-            beta = beta[sp_sel]
+            x = x[st_sel]
+            D = D[st_sel]
+            ct = ct[st_sel]
+            ws = ws[st_sel]
+            ti = ti[st_sel]
+            k = k[st_sel]
+            gamma = gamma[st_sel]
+            alpha = alpha[st_sel]
+            beta = beta[st_sel]
 
             # calc theta_c0, Eq. (6.12):
             cosg = np.cos(gamma)
             twoac = 2 * self.induction.ct2a(ct * cosg)
             theta = 0.3 * gamma / cosg * twoac
 
             # calculate x0, Eq. (7.3):
@@ -325,40 +324,40 @@
                 # memorize far wake data:
                 out[self.AMPL_FAR] = ampl
                 out[self.DELTA_FAR] = delta
                 out[self.SIGMA_Y_FAR] = sigma_y
                 out[self.SIGMA_Z_FAR] = sigma_z
 
         # update mdata:
-        out[self.SP_SEL] = sp_sel
+        out[self.ST_SEL] = st_sel
         mdata[self.MDATA_KEY] = out
 
-    def has_data(self, mdata, states_source_turbine, x):
+    def has_data(self, mdata, downwind_index, x):
         """
         Check if data exists
 
         Parameters
         ----------
         mdata: foxes.core.Data
             The model data
-        states_source_turbine: numpy.ndarray
+        downwind_index: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x: numpy.ndarray
             The x values, shape: (n_states, n_points)
 
         Returns
         -------
         check: bool
             True if data exists
 
         """
         check = (
             mdata[FC.STATE][0],
-            states_source_turbine[0],
+            downwind_index,
             x.shape,
         )
         return self.MDATA_KEY in mdata and mdata[self.MDATA_KEY][self.CHECK] == check
 
     def get_data(self, key, mdata):
         """
         Return data entry
@@ -423,18 +422,16 @@
         **kwargs,
     ):
         """
         Constructor.
 
         Parameters
         ----------
-        superposition: dict
-            The superpositions. Key: variable name str,
-            value: The wake superposition model name,
-            will be looked up in model book
+        superposition: str
+            The wind deficit superposition
         k: float
             The wake growth parameter k. If not given here
             it will be searched in the farm data, by default None
         ct_max: float
             The maximal value for ct, values beyond will be limited
             to this number, by default 0.9999
         alpha: float
@@ -455,16 +452,22 @@
         self.k_var = k_var
 
         setattr(self, k_var, k)
         setattr(self, FV.YAWM, 0.0)
 
     def __repr__(self):
         k = getattr(self, self.k_var)
-        s = super().__repr__()
-        s += f"({self.k_var}={k}, sp={self.superpositions[FV.WS]})"
+        iname = self.model_pars.get("induction", "Madsen")
+        s = f"{type(self).__name__}"
+        s += f"({self.superpositions[FV.WS]}, induction={iname}"
+        if k is None:
+            s += f", k_var={self.k_var}"
+        else:
+            s += f", {self.k_var}={k}"
+        s += ")"
         return s
 
     def sub_models(self):
         """
         List of all sub-models
 
         Returns
@@ -489,125 +492,95 @@
             Overwrite existing data
 
         """
         if not self.initialized:
             self.model = Bastankhah2016Model(**self.model_pars)
         super().initialize(algo, verbosity, force)
 
-    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
-        """
-        Initialize wake delta storage.
-
-        They are added on the fly to the wake_deltas dict.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        wake_deltas: dict
-            The wake deltas storage, add wake deltas
-            on the fly. Keys: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
-
-        """
-        n_states = mdata.n_states
-        wake_deltas[FV.WS] = np.zeros((n_states, pdata.n_points), dtype=FC.DTYPE)
-
-    def calc_wakes_spsel_x_yz(
+    def calc_wakes_x_yz(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
+        tdata,
+        downwind_index,
         x,
         yz,
     ):
         """
         Calculate wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
         x: numpy.ndarray
-            The x values, shape: (n_states, n_points)
+            The x values, shape: (n_states, n_targets)
         yz: numpy.ndarray
             The yz values for each x value, shape:
-            (n_states, n_points, n_yz_per_x, 2)
+            (n_states, n_targets, n_yz_per_target, 2)
 
         Returns
         -------
         wdeltas: dict
             The wake deltas. Key: variable name str,
-            value: numpy.ndarray, shape: (n_sp_sel, n_yz_per_x)
-        sp_sel: numpy.ndarray of bool
-            The state-point selection, for which the wake
-            is non-zero, shape: (n_states, n_points)
+            value: numpy.ndarray, shape: (n_st_sel, n_yz_per_target)
+        st_sel: numpy.ndarray of bool
+            The state-target selection, for which the wake
+            is non-zero, shape: (n_states, n_targets)
 
         """
-
         # prepare:
         n_y_per_z = yz.shape[2]
 
         # calculate model data:
-        if not self.model.has_data(mdata, states_source_turbine, x):
+        if not self.model.has_data(mdata, downwind_index, x):
             # get gamma:
             gamma = self.get_data(
                 FV.YAWM,
-                FC.STATE_POINT,
+                FC.STATE_TARGET,
                 lookup="ws",
                 algo=algo,
                 fdata=fdata,
-                pdata=pdata,
+                tdata=tdata,
                 upcast=True,
-                states_source_turbine=states_source_turbine,
+                downwind_index=downwind_index,
             )
             gamma *= np.pi / 180
 
             # get k:
             k = self.get_data(
                 self.k_var,
-                FC.STATE_POINT,
+                FC.STATE_TARGET,
                 lookup="sw",
                 algo=algo,
                 fdata=fdata,
-                pdata=pdata,
+                tdata=tdata,
                 upcast=True,
-                states_source_turbine=states_source_turbine,
+                downwind_index=downwind_index,
             )
 
             # run calculation:
-            self.model.calc_data(
-                algo, mdata, fdata, pdata, states_source_turbine, x, gamma, k
-            )
+            self.model.calc_data(algo, mdata, fdata, tdata, downwind_index, x, gamma, k)
 
         # select targets:
-        sp_sel = self.model.get_data(Bastankhah2016Model.SP_SEL, mdata)
-        n_sp_sel = np.sum(sp_sel)
+        st_sel = self.model.get_data(Bastankhah2016Model.ST_SEL, mdata)
+        n_sp_sel = np.sum(st_sel)
         wdeltas = {FV.WS: np.zeros((n_sp_sel, n_y_per_z), dtype=FC.DTYPE)}
-        if np.any(sp_sel):
+        if np.any(st_sel):
             # apply filter:
-            yz = yz[sp_sel]
+            yz = yz[st_sel]
 
             # collect data:
             near = self.model.get_data(Bastankhah2016Model.NEAR, mdata)
             far = ~near
 
             # near wake:
             if np.any(near):
@@ -646,8 +619,8 @@
                 y = yz[..., 0]
                 z = yz[..., 1]
                 wdeltas[FV.WS][far] = ampl * (
                     np.exp(-0.5 * (y / sigma_y) ** 2)
                     * np.exp(-0.5 * (z / sigma_z) ** 2)
                 )
 
-        return wdeltas, sp_sel
+        return wdeltas, st_sel
```

### Comparing `foxes-0.6.2/foxes/models/wake_models/wind/jensen.py` & `foxes-0.7/foxes/models/wake_superpositions/ws_max.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,204 +1,183 @@
 import numpy as np
 
-from foxes.models.wake_models.top_hat import TopHatWakeModel
+from foxes.core import WakeSuperposition
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class JensenWake(TopHatWakeModel):
+class WSMax(WakeSuperposition):
     """
-    The Jensen wake model.
+    Max supersposition of wind deficit results
 
     Attributes
     ----------
-    k: float, optional
-        The wake growth parameter k. If not given here
-        it will be searched in the farm data.
-    k_var: str
-        The variable name for k
+    scale_amb: bool
+        Flag for scaling wind deficit with ambient wind speed
+        instead of waked wind speed
+    lim_low: float
+        Lower limit of the final waked wind speed
+    lim_high: float
+        Upper limit of the final waked wind speed
 
-    :group: models.wake_models.wind
+    :group: models.wake_superpositions
 
     """
 
-    def __init__(self, superposition, k=None, k_var=FV.K, **kwargs):
+    def __init__(self, scale_amb=False, lim_low=None, lim_high=None):
         """
         Constructor.
 
         Parameters
         ----------
-        superpositions: dict
-            The superpositions. Key: variable name str,
-            value: The wake superposition model name,
-            will be looked up in model book
-        k: float, optional
-            The wake growth parameter k. If not given here
-            it will be searched in the farm data.
-        k_var: str
-            The variable name for k
-        kwargs: dict, optional
-            Additional parameters for the base class
+        scale_amb: bool
+            Flag for scaling wind deficit with ambient wind speed
+            instead of waked wind speed
+        lim_low: float
+            Lower limit of the final waked wind speed
+        lim_high: float
+            Upper limit of the final waked wind speed
 
         """
-        super().__init__(superpositions={FV.WS: superposition}, **kwargs)
-
-        self.k_var = k_var
-        setattr(self, k_var, k)
+        super().__init__()
+
+        self.scale_amb = scale_amb
+        self.lim_low = lim_low
+        self.lim_high = lim_high
 
     def __repr__(self):
-        k = getattr(self, self.k_var)
-        s = super().__repr__()
-        s += f"({self.k_var}={k}, sp={self.superpositions[FV.WS]})"
-        return s
+        a = f"scale_amb={self.scale_amb}, lim_low={self.lim_low}, lim_high={self.lim_high}"
+        return f"{type(self).__name__}({a})"
 
-    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
+    def input_farm_vars(self, algo):
         """
-        Initialize wake delta storage.
-
-        They are added on the fly to the wake_deltas dict.
+        The variables which are needed for running
+        the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        wake_deltas: dict
-            The wake deltas storage, add wake deltas
-            on the fly. Keys: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
+
+        Returns
+        -------
+        input_vars: list of str
+            The input variable names
 
         """
-        n_states = mdata.n_states
-        wake_deltas[FV.WS] = np.zeros((n_states, pdata.n_points), dtype=FC.DTYPE)
+        return [FV.AMB_REWS] if self.scale_amb else [FV.REWS]
 
-    def calc_wake_radius(
+    def add_wake(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        x,
-        ct,
+        tdata,
+        downwind_index,
+        st_sel,
+        variable,
+        wake_delta,
+        wake_model_result,
     ):
         """
-        Calculate the wake radius, depending on x only (not r).
+        Add a wake delta to previous wake deltas,
+        at rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        x: numpy.ndarray
-            The x values, shape: (n_states, n_points)
-        r: numpy.ndarray
-            The radial values for each x value, shape:
-            (n_states, n_points, n_r_per_x, 2)
-        ct: numpy.ndarray
-            The ct values of the wake-causing turbines,
-            shape: (n_states, n_points)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        st_sel: numpy.ndarray of bool
+            The selection of targets, shape: (n_states, n_targets)
+        variable: str
+            The variable name for which the wake deltas applies
+        wake_delta: numpy.ndarray
+            The original wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
+        wake_model_result: numpy.ndarray
+            The new wake deltas of the selected rotors,
+            shape: (n_st_sel, n_tpoints, ...)
 
         Returns
         -------
-        wake_r: numpy.ndarray
-            The wake radii, shape: (n_states, n_points)
+        wdelta: numpy.ndarray
+            The updated wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
 
         """
+        if variable not in [FV.REWS, FV.REWS2, FV.REWS3, FV.WS]:
+            raise ValueError(
+                f"Superposition '{self.name}': Expecting wind speed variable, got {variable}"
+            )
 
-        R = (
-            self.get_data(
-                FV.D,
-                FC.STATE_POINT,
+        if np.any(st_sel):
+            scale = self.get_data(
+                FV.AMB_REWS if self.scale_amb else FV.REWS,
+                FC.STATE_TARGET,
                 lookup="w",
                 algo=algo,
                 fdata=fdata,
-                pdata=pdata,
-                states_source_turbine=states_source_turbine,
-            )
-            / 2
-        )
+                tdata=tdata,
+                downwind_index=downwind_index,
+                upcast=True,
+            )[st_sel, None]
+
+            wake_model_result = np.abs(scale * wake_model_result)
+            odelta = wake_delta[st_sel]
 
-        k = self.get_data(
-            self.k_var,
-            FC.STATE_POINT,
-            lookup="sw",
-            algo=algo,
-            fdata=fdata,
-            pdata=pdata,
-            upcast=True,
-            states_source_turbine=states_source_turbine,
-        )
+            wake_delta[st_sel] = np.maximum(odelta, wake_model_result)
 
-        return R + k * x
+        return wake_delta
 
-    def calc_centreline_wake_deltas(
+    def calc_final_wake_delta(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        sp_sel,
-        x,
-        wake_r,
-        ct,
+        variable,
+        amb_results,
+        wake_delta,
     ):
         """
-        Calculate centre line results of wake deltas.
+        Calculate the final wake delta after adding all
+        contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        sp_sel: numpy.ndarray of bool
-            The state-point selection, for which the wake
-            is non-zero, shape: (n_states, n_points)
-        x: numpy.ndarray
-            The x values, shape: (n_sp_sel,)
-        wake_r: numpy.ndarray
-            The wake radii, shape: (n_sp_sel,)
-        ct: numpy.ndarray
-            The ct values of the wake-causing turbines,
-            shape: (n_sp_sel,)
+        variable: str
+            The variable name for which the wake deltas applies
+        amb_results: numpy.ndarray
+            The ambient results at targets,
+            shape: (n_states, n_targets, n_tpoints)
+        wake_delta: numpy.ndarray
+            The wake deltas at targets, shape:
+            (n_states, n_targets, n_tpoints)
 
         Returns
         -------
-        cl_del: dict
-            The centre line wake deltas. Key: variable name str,
-            varlue: numpy.ndarray, shape: (n_sp_sel,)
+        final_wake_delta: numpy.ndarray
+            The final wake delta, which will be added to the ambient
+            results by simple plus operation. Shape:
+            (n_states, n_targets, n_tpoints)
 
         """
-        n_states = mdata.n_states
-        n_points = sp_sel.shape[1]
-        st_sel = (np.arange(n_states), states_source_turbine)
-
-        R = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        R[:] = fdata[FV.D][st_sel][:, None] / 2
-        R = R[sp_sel]
-
-        twoa = 2 * self.induction.ct2a(ct)
-
-        return {FV.WS: -((R / wake_r) ** 2) * twoa}
+        w = -wake_delta
+        if self.lim_low is not None:
+            w = np.maximum(w, self.lim_low - amb_results)
+        if self.lim_high is not None:
+            w = np.minimum(w, self.lim_high - amb_results)
+        return w
```

### Comparing `foxes-0.6.2/foxes/models/wake_models/wind/turbopark.py` & `foxes-0.7/foxes/models/wake_models/wind/turbopark.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 
 from foxes.models.wake_models.gaussian import GaussianWakeModel
-from foxes.utils import sqrt_reg
 import foxes.variables as FV
 import foxes.constants as FC
 
 
 class TurbOParkWake(GaussianWakeModel):
     """
     The TurbOPark wake model
@@ -44,18 +43,16 @@
         induction="Madsen",
     ):
         """
         Constructor.
 
         Parameters
         ----------
-        superpositions: dict
-            The superpositions. Key: variable name str,
-            value: The wake superposition model name,
-            will be looked up in model book
+        superposition: str
+            The wind deficit superposition
         A: float
             The wake growth parameter A.
         sbeta_factor: float
             Factor multiplying sbeta
         c1: float
             Factor from Frandsen turbulence model
         c2: float
@@ -69,16 +66,19 @@
         self.A = A
         self.sbeta_factor = sbeta_factor
         self.c1 = c1
         self.c2 = c2
         self.induction = induction
 
     def __repr__(self):
-        s = super().__repr__()
-        s += f"(A={self.A}, sp={self.superpositions[FV.WS]})"
+        iname = (
+            self.induction if isinstance(self.induction, str) else self.induction.name
+        )
+        s = f"{type(self).__name__}"
+        s += f"({self.superpositions[FV.WS]}, A={self.A}, induction={iname})"
         return s
 
     def sub_models(self):
         """
         List of all sub-models
 
         Returns
@@ -103,124 +103,94 @@
             Overwrite existing data
 
         """
         if isinstance(self.induction, str):
             self.induction = algo.mbook.axial_induction[self.induction]
         super().initialize(algo, verbosity, force)
 
-    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
-        """
-        Initialize wake delta storage.
-
-        They are added on the fly to the wake_deltas dict.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        wake_deltas: dict
-            The wake deltas storage, add wake deltas
-            on the fly. Keys: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
-
-        """
-        n_states = mdata.n_states
-        wake_deltas[FV.WS] = np.zeros((n_states, pdata.n_points), dtype=FC.DTYPE)
-
-    def calc_amplitude_sigma_spsel(
+    def calc_amplitude_sigma(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
+        tdata,
+        downwind_index,
         x,
     ):
         """
         Calculate the amplitude and the sigma,
         both depend only on x (not on r).
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
         x: numpy.ndarray
-            The x values, shape: (n_states, n_points)
+            The x values, shape: (n_states, n_targets)
 
         Returns
         -------
         amsi: tuple
             The amplitude and sigma, both numpy.ndarray
-            with shape (n_sp_sel,)
-        sp_sel: numpy.ndarray of bool
-            The state-point selection, for which the wake
-            is non-zero, shape: (n_states, n_points)
+            with shape (n_st_sel,)
+        st_sel: numpy.ndarray of bool
+            The state-target selection, for which the wake
+            is non-zero, shape: (n_states, n_targets)
 
         """
-
         # get ct:
         ct = self.get_data(
             FV.CT,
-            FC.STATE_POINT,
+            FC.STATE_TARGET,
             lookup="w",
             algo=algo,
             fdata=fdata,
-            pdata=pdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
             upcast=True,
-            states_source_turbine=states_source_turbine,
         )
 
         # select targets:
-        sp_sel = (x > 1e-5) & (ct > 0.0)
-        if np.any(sp_sel):
+        st_sel = (x > 1e-5) & (ct > 0.0)
+        if np.any(st_sel):
             # apply selection:
-            x = x[sp_sel]
-            ct = ct[sp_sel]
+            x = x[st_sel]
+            ct = ct[st_sel]
 
             # get D:
             D = self.get_data(
                 FV.D,
-                FC.STATE_POINT,
+                FC.STATE_TARGET,
                 lookup="w",
                 algo=algo,
                 fdata=fdata,
-                pdata=pdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
                 upcast=True,
-                states_source_turbine=states_source_turbine,
-            )
-            D = D[sp_sel]
+            )[st_sel]
 
             # get TI:
             ati = self.get_data(
                 FV.AMB_TI,
-                FC.STATE_POINT,
+                FC.STATE_TARGET,
                 lookup="w",
                 algo=algo,
                 fdata=fdata,
-                pdata=pdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
                 upcast=True,
-                states_source_turbine=states_source_turbine,
-            )
-            ati = ati[sp_sel]
+            )[st_sel]
 
             # calculate sigma:
             # beta = np.sqrt(0.5 * (1 + np.sqrt(1.0 - ct)) / np.sqrt(1.0 - ct))
             a = self.induction.ct2a(ct)
             beta = (1 - a) / (1 - 2 * a)
             epsilon = self.sbeta_factor * np.sqrt(beta)
             del a, beta
@@ -254,20 +224,20 @@
 
             # calculate amplitude, same as in Bastankhah model (eqn 7)
             ct_eff = ct / (8 * (sigma / D) ** 2)
             ampld = np.maximum(-2 * self.induction.ct2a(ct_eff), -1)
 
         # case no targets:
         else:
-            sp_sel = np.zeros_like(x, dtype=bool)
-            n_sp = np.sum(sp_sel)
+            st_sel = np.zeros_like(x, dtype=bool)
+            n_sp = np.sum(st_sel)
             ampld = np.zeros(n_sp, dtype=FC.DTYPE)
             sigma = np.zeros(n_sp, dtype=FC.DTYPE)
 
-        return {FV.WS: (ampld, sigma)}, sp_sel
+        return {FV.WS: (ampld, sigma)}, st_sel
 
 
 class TurbOParkWakeIX(GaussianWakeModel):
     """
     The generalized TurbOPark wake model, integrating TI over the streamline.
 
     https://iopscience.iop.org/article/10.1088/1742-6596/2265/2/022063/pdf
@@ -305,18 +275,16 @@
         **ipars,
     ):
         """
         Constructor.
 
         Parameters
         ----------
-        superpositions: dict
-            The superpositions. Key: variable name str,
-            value: The wake superposition model name,
-            will be looked up in model book
+        superposition: str
+            The wind deficit superposition
         dx: float
             The step size of the integral
         A: float, optional
             The wake growth parameter A.
         sbeta_factor: float
             Factor multiplying sbeta
         ti_var:  str
@@ -337,16 +305,19 @@
         self.ti_var = ti_var
         self.ipars = ipars
         self._tiwakes = None
         self.self_wake = self_wake
         self.induction = induction
 
     def __repr__(self):
-        s = super().__repr__()
-        s += f"(ti={self.ti_var}, dx={self.dx}, A={self.A}, sp={self.superpositions[FV.WS]})"
+        iname = (
+            self.induction if isinstance(self.induction, str) else self.induction.name
+        )
+        s = f"{type(self).__name__}({self.superpositions[FV.WS]}"
+        s += f", ti={self.ti_var}, dx={self.dx}, A={self.A}, induction={iname})"
         return s
 
     def sub_models(self):
         """
         List of all sub-models
 
         Returns
@@ -371,167 +342,156 @@
             Overwrite existing data
 
         """
         if isinstance(self.induction, str):
             self.induction = algo.mbook.axial_induction[self.induction]
         super().initialize(algo, verbosity, force)
 
-    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
+    def new_wake_deltas(self, algo, mdata, fdata, tdata):
         """
-        Initialize wake delta storage.
-
-        They are added on the fly to the wake_deltas dict.
+        Creates new empty wake delta arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
+        tdata: foxes.core.TData
+            The target point data
+
+        Returns
+        -------
         wake_deltas: dict
-            The wake deltas storage, add wake deltas
-            on the fly. Keys: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
+            Key: variable name, value: The zero filled
+            wake deltas, shape: (n_states, n_turbines, n_rpoints, ...)
 
         """
-        n_states = mdata.n_states
-        wake_deltas[FV.WS] = np.zeros((n_states, pdata.n_points), dtype=FC.DTYPE)
-
-        # find TI wake models:
+        # find TI wake model:
         self._tiwakes = []
-        for w in algo.wake_models:
+        for w in algo.wake_models.values():
             if w is not self:
-                wdel = {}
-                w.init_wake_deltas(algo, mdata, fdata, pdata, wdel)
+                wdel = w.new_wake_deltas(algo, mdata, fdata, tdata)
                 if self.ti_var in wdel:
                     self._tiwakes.append(w)
         if self.ti_var not in FV.amb2var and len(self._tiwakes) == 0:
             raise KeyError(
                 f"Model '{self.name}': Missing wake model that computes wake delta for variable {self.ti_var}"
             )
 
-    def calc_amplitude_sigma_spsel(
+        return super().new_wake_deltas(algo, mdata, fdata, tdata)
+
+    def calc_amplitude_sigma(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
+        tdata,
+        downwind_index,
         x,
     ):
         """
         Calculate the amplitude and the sigma,
         both depend only on x (not on r).
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index in the downwind order
         x: numpy.ndarray
-            The x values, shape: (n_states, n_points)
+            The x values, shape: (n_states, n_targets)
 
         Returns
         -------
         amsi: tuple
             The amplitude and sigma, both numpy.ndarray
-            with shape (n_sp_sel,)
-        sp_sel: numpy.ndarray of bool
-            The state-point selection, for which the wake
-            is non-zero, shape: (n_states, n_points)
+            with shape (n_st_sel,)
+        st_sel: numpy.ndarray of bool
+            The state-target selection, for which the wake
+            is non-zero, shape: (n_states, n_targets)
 
         """
-
         # get ct:
         ct = self.get_data(
             FV.CT,
-            FC.STATE_POINT,
+            FC.STATE_TARGET,
             lookup="w",
             algo=algo,
             fdata=fdata,
-            pdata=pdata,
+            tdata=tdata,
+            downwind_index=downwind_index,
             upcast=True,
-            states_source_turbine=states_source_turbine,
         )
 
         # select targets:
-        sp_sel = (x > 1e-5) & (ct > 0.0)
-        if np.any(sp_sel):
+        st_sel = (x > 1e-5) & (ct > 0.0)
+        if np.any(st_sel):
             # apply selection:
-            # x = x[sp_sel]
-            ct = ct[sp_sel]
+            # x = x[st_sel]
+            ct = ct[st_sel]
 
             # get D:
             D = self.get_data(
                 FV.D,
-                FC.STATE_POINT,
+                FC.STATE_TARGET,
                 lookup="w",
                 algo=algo,
                 fdata=fdata,
-                pdata=pdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
                 upcast=True,
-                states_source_turbine=states_source_turbine,
-            )
-            D = D[sp_sel]
+            )[st_sel]
 
             # calculate sigma:
             # beta = np.sqrt(0.5 * (1 + np.sqrt(1.0 - ct)) / np.sqrt(1.0 - ct))
             a = self.induction.ct2a(ct)
             beta = (1 - a) / (1 - 2 * a)
             epsilon = self.sbeta_factor * np.sqrt(beta)
             del a, beta
 
             # get TI by integration along centre line:
             ti_ix = algo.wake_frame.calc_centreline_integral(
                 algo,
                 mdata,
                 fdata,
-                states_source_turbine,
+                downwind_index,
                 [self.ti_var],
                 x,
                 dx=self.dx,
                 wake_models=self._tiwakes,
                 self_wake=self.self_wake,
                 **self.ipars,
             )[:, :, 0]
 
             # calculate sigma (eqn 1, plus epsilon from eqn 4 for x = 0)
-            sigma = D * epsilon + self.A * ti_ix[sp_sel]
-
-            del (
-                x,
-                sbeta,
-                epsilon,
-            )
+            sigma = D * epsilon + self.A * ti_ix[st_sel]
+            del x, epsilon
 
             # calculate amplitude, same as in Bastankhah model (eqn 7)
             ct_eff = ct / (8 * (sigma / D) ** 2)
             ampld = np.maximum(-2 * self.induction.ct2a(ct_eff), -1)
 
         # case no targets:
         else:
-            sp_sel = np.zeros_like(x, dtype=bool)
-            n_sp = np.sum(sp_sel)
+            st_sel = np.zeros_like(x, dtype=bool)
+            n_sp = np.sum(st_sel)
             ampld = np.zeros(n_sp, dtype=FC.DTYPE)
             sigma = np.zeros(n_sp, dtype=FC.DTYPE)
 
-        return {FV.WS: (ampld, sigma)}, sp_sel
+        return {FV.WS: (ampld, sigma)}, st_sel
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
```

### Comparing `foxes-0.6.2/foxes/models/wake_superpositions/ti_linear.py` & `foxes-0.7/foxes/models/wake_superpositions/ti_pow.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,137 +1,150 @@
 import numpy as np
 
 from foxes.core import WakeSuperposition
 import foxes.variables as FV
 
 
-class TILinear(WakeSuperposition):
+class TIPow(WakeSuperposition):
     """
-    Linear wake superposition for TI.
+    Power wake superposition for TI.
 
     Attributes
     ----------
+    pow: float
+        The power to which to take the wake results
     superp_to_amb: str
         The method for combining ambient with wake deltas:
         linear or quadratic
 
     :group: models.wake_superpositions
 
     """
 
-    def __init__(self, superp_to_amb="quadratic"):
+    def __init__(self, pow, superp_to_amb="quadratic"):
         """
         Constructor.
 
         Parameters
         ----------
+        pow: float
+            The power to which to take the wake results
         superp_to_amb: str
             The method for combining ambient with wake deltas:
             linear or quadratic
 
         """
         super().__init__()
+        self.pow = pow
         self.superp_to_amb = superp_to_amb
 
-    def calc_wakes_plus_wake(
+    def __repr__(self):
+        return (
+            f"{type(self).__name__}(pow={self.pow}, superp_to_amb={self.superp_to_amb})"
+        )
+
+    def add_wake(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        sel_sp,
+        tdata,
+        downwind_index,
+        st_sel,
         variable,
         wake_delta,
         wake_model_result,
     ):
         """
-        Add a wake delta to previous wake deltas.
+        Add a wake delta to previous wake deltas,
+        at rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        sel_sp: numpy.ndarray of bool
-            The selection of points, shape: (n_states, n_points)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        st_sel: numpy.ndarray of bool
+            The selection of targets, shape: (n_states, n_targets)
         variable: str
             The variable name for which the wake deltas applies
         wake_delta: numpy.ndarray
-            The original wake deltas, shape: (n_states, n_points)
+            The original wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
         wake_model_result: numpy.ndarray
-            The new wake deltas of the selected points,
-            shape: (n_sel_sp,)
+            The new wake deltas of the selected rotors,
+            shape: (n_st_sel, n_tpoints, ...)
 
         Returns
         -------
         wdelta: numpy.ndarray
-            The updated wake deltas, shape: (n_states, n_points)
+            The updated wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
 
         """
         if variable != FV.TI:
             raise ValueError(
                 f"Superposition '{self.name}': Expecting wake variable {FV.TI}, got {variable}"
             )
 
-        wake_delta[sel_sp] += wake_model_result
+        wake_delta[st_sel] += wake_model_result**self.pow
         return wake_delta
 
     def calc_final_wake_delta(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
         variable,
         amb_results,
         wake_delta,
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
         variable: str
             The variable name for which the wake deltas applies
         amb_results: numpy.ndarray
-            The ambient results, shape: (n_states, n_points)
+            The ambient results at targets,
+            shape: (n_states, n_targets, n_tpoints)
         wake_delta: numpy.ndarray
-            The wake deltas, shape: (n_states, n_points)
+            The wake deltas at targets, shape:
+            (n_states, n_targets, n_tpoints)
 
         Returns
         -------
         final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
-            results by simple plus operation. Shape: (n_states, n_points)
+            results by simple plus operation. Shape:
+            (n_states, n_targets, n_tpoints)
 
         """
         # linear superposition to ambient:
         if self.superp_to_amb == "linear":
-            return wake_delta
+            return wake_delta ** (1 / self.pow)
 
         # quadratic superposition to ambient:
         elif self.superp_to_amb == "quadratic":
-            return np.sqrt(wake_delta**2 + amb_results**2) - amb_results
+            return np.sqrt(wake_delta ** (2 / self.pow) + amb_results**2) - amb_results
 
         # unknown ti delta:
         else:
             raise ValueError(
                 f"Unknown superp_to_amb = '{self.superp_to_amb}', valid choices: linear, quadratic"
             )
```

### Comparing `foxes-0.6.2/foxes/models/wake_superpositions/ti_max.py` & `foxes-0.7/foxes/models/wake_superpositions/ti_linear.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 
 from foxes.core import WakeSuperposition
 import foxes.variables as FV
 
 
-class TIMax(WakeSuperposition):
+class TILinear(WakeSuperposition):
     """
-    Max wake superposition for TI.
+    Linear wake superposition for TI.
 
     Attributes
     ----------
     superp_to_amb: str
         The method for combining ambient with wake deltas:
         linear or quadratic
 
@@ -28,102 +28,108 @@
             The method for combining ambient with wake deltas:
             linear or quadratic
 
         """
         super().__init__()
         self.superp_to_amb = superp_to_amb
 
-    def calc_wakes_plus_wake(
+    def __repr__(self):
+        return f"{type(self).__name__}(superp_to_amb={self.superp_to_amb})"
+
+    def add_wake(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        sel_sp,
+        tdata,
+        downwind_index,
+        st_sel,
         variable,
         wake_delta,
         wake_model_result,
     ):
         """
-        Add a wake delta to previous wake deltas.
+        Add a wake delta to previous wake deltas,
+        at rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        sel_sp: numpy.ndarray of bool
-            The selection of points, shape: (n_states, n_points)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        st_sel: numpy.ndarray of bool
+            The selection of targets, shape: (n_states, n_targets)
         variable: str
             The variable name for which the wake deltas applies
         wake_delta: numpy.ndarray
-            The original wake deltas, shape: (n_states, n_points)
+            The original wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
         wake_model_result: numpy.ndarray
-            The new wake deltas of the selected points,
-            shape: (n_sel_sp,)
+            The new wake deltas of the selected rotors,
+            shape: (n_st_sel, n_tpoints, ...)
 
         Returns
         -------
         wdelta: numpy.ndarray
-            The updated wake deltas, shape: (n_states, n_points)
+            The updated wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
 
         """
         if variable != FV.TI:
             raise ValueError(
                 f"Superposition '{self.name}': Expecting wake variable {FV.TI}, got {variable}"
             )
 
-        wake_delta[sel_sp] = np.maximum(wake_model_result, wake_delta[sel_sp])
+        wake_delta[st_sel] += wake_model_result
         return wake_delta
 
     def calc_final_wake_delta(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
         variable,
         amb_results,
         wake_delta,
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
         variable: str
             The variable name for which the wake deltas applies
         amb_results: numpy.ndarray
-            The ambient results, shape: (n_states, n_points)
+            The ambient results at targets,
+            shape: (n_states, n_targets, n_tpoints)
         wake_delta: numpy.ndarray
-            The wake deltas, shape: (n_states, n_points)
+            The wake deltas at targets, shape:
+            (n_states, n_targets, n_tpoints)
 
         Returns
         -------
         final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
-            results by simple plus operation. Shape: (n_states, n_points)
+            results by simple plus operation. Shape:
+            (n_states, n_targets, n_tpoints)
 
         """
         # linear superposition to ambient:
         if self.superp_to_amb == "linear":
             return wake_delta
 
         # quadratic superposition to ambient:
```

### Comparing `foxes-0.6.2/foxes/models/wake_superpositions/ti_pow.py` & `foxes-0.7/foxes/models/wake_superpositions/ti_max.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,142 +1,143 @@
 import numpy as np
 
 from foxes.core import WakeSuperposition
 import foxes.variables as FV
 
 
-class TIPow(WakeSuperposition):
+class TIMax(WakeSuperposition):
     """
-    Power wake superposition for TI.
+    Max wake superposition for TI.
 
     Attributes
     ----------
-    pow: float
-        The power to which to take the wake results
     superp_to_amb: str
         The method for combining ambient with wake deltas:
         linear or quadratic
 
     :group: models.wake_superpositions
 
     """
 
-    def __init__(self, pow, superp_to_amb="quadratic"):
+    def __init__(self, superp_to_amb="quadratic"):
         """
         Constructor.
 
         Parameters
         ----------
-        pow: float
-            The power to which to take the wake results
         superp_to_amb: str
             The method for combining ambient with wake deltas:
             linear or quadratic
 
         """
         super().__init__()
-        self.pow = pow
         self.superp_to_amb = superp_to_amb
 
-    def calc_wakes_plus_wake(
+    def __repr__(self):
+        return f"{type(self).__name__}(superp_to_amb={self.superp_to_amb})"
+
+    def add_wake(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        sel_sp,
+        tdata,
+        downwind_index,
+        st_sel,
         variable,
         wake_delta,
         wake_model_result,
     ):
         """
-        Add a wake delta to previous wake deltas.
+        Add a wake delta to previous wake deltas,
+        at rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        sel_sp: numpy.ndarray of bool
-            The selection of points, shape: (n_states, n_points)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        st_sel: numpy.ndarray of bool
+            The selection of targets, shape: (n_states, n_targets)
         variable: str
             The variable name for which the wake deltas applies
         wake_delta: numpy.ndarray
-            The original wake deltas, shape: (n_states, n_points)
+            The original wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
         wake_model_result: numpy.ndarray
-            The new wake deltas of the selected points,
-            shape: (n_sel_sp,)
+            The new wake deltas of the selected rotors,
+            shape: (n_st_sel, n_tpoints, ...)
 
         Returns
         -------
         wdelta: numpy.ndarray
-            The updated wake deltas, shape: (n_states, n_points)
+            The updated wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
 
         """
         if variable != FV.TI:
             raise ValueError(
                 f"Superposition '{self.name}': Expecting wake variable {FV.TI}, got {variable}"
             )
 
-        wake_delta[sel_sp] += wake_model_result**self.pow
+        wake_delta[st_sel] = np.maximum(wake_model_result, wake_delta[st_sel])
         return wake_delta
 
     def calc_final_wake_delta(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
         variable,
         amb_results,
         wake_delta,
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
         variable: str
             The variable name for which the wake deltas applies
         amb_results: numpy.ndarray
-            The ambient results, shape: (n_states, n_points)
+            The ambient results at targets,
+            shape: (n_states, n_targets, n_tpoints)
         wake_delta: numpy.ndarray
-            The wake deltas, shape: (n_states, n_points)
+            The wake deltas at targets, shape:
+            (n_states, n_targets, n_tpoints)
 
         Returns
         -------
         final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
-            results by simple plus operation. Shape: (n_states, n_points)
+            results by simple plus operation. Shape:
+            (n_states, n_targets, n_tpoints)
 
         """
         # linear superposition to ambient:
         if self.superp_to_amb == "linear":
-            return wake_delta ** (1 / self.pow)
+            return wake_delta
 
         # quadratic superposition to ambient:
         elif self.superp_to_amb == "quadratic":
-            return np.sqrt(wake_delta ** (2 / self.pow) + amb_results**2) - amb_results
+            return np.sqrt(wake_delta**2 + amb_results**2) - amb_results
 
         # unknown ti delta:
         else:
             raise ValueError(
                 f"Unknown superp_to_amb = '{self.superp_to_amb}', valid choices: linear, quadratic"
             )
```

### Comparing `foxes-0.6.2/foxes/models/wake_superpositions/ws_linear.py` & `foxes-0.7/foxes/models/wake_superpositions/ws_pow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,62 @@
 import numpy as np
 
 from foxes.core import WakeSuperposition
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class WSLinear(WakeSuperposition):
+class WSPow(WakeSuperposition):
     """
-    Linear supersposition of wind deficit results
+    Power supersposition of wind deficit results
 
     Attributes
     ----------
+    pow: float
+        The power to which to take the wake results
     scale_amb: bool
         Flag for scaling wind deficit with ambient wind speed
         instead of waked wind speed
     lim_low: float
         Lower limit of the final waked wind speed
     lim_high: float
         Upper limit of the final waked wind speed
 
     :group: models.wake_superpositions
 
     """
 
-    def __init__(self, scale_amb=False, lim_low=None, lim_high=None):
+    def __init__(self, pow, scale_amb=False, lim_low=None, lim_high=None):
         """
         Constructor.
 
         Parameters
         ----------
+        pow: float
+            The power to which to take the wake results
         scale_amb: bool
             Flag for scaling wind deficit with ambient wind speed
             instead of waked wind speed
         lim_low: float
             Lower limit of the final waked wind speed
         lim_high: float
             Upper limit of the final waked wind speed
 
         """
         super().__init__()
 
+        self.pow = pow
         self.scale_amb = scale_amb
         self.lim_low = lim_low
         self.lim_high = lim_high
 
+    def __repr__(self):
+        a = f"pow={self.pow}, scale_amb={self.scale_amb}, lim_low={self.lim_low}, lim_high={self.lim_high}"
+        return f"{type(self).__name__}({a})"
+
     def input_farm_vars(self, algo):
         """
         The variables which are needed for running
         the model.
 
         Parameters
         ----------
@@ -58,116 +67,119 @@
         -------
         input_vars: list of str
             The input variable names
 
         """
         return [FV.AMB_REWS] if self.scale_amb else [FV.REWS]
 
-    def calc_wakes_plus_wake(
+    def add_wake(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        sel_sp,
+        tdata,
+        downwind_index,
+        st_sel,
         variable,
         wake_delta,
         wake_model_result,
     ):
         """
-        Add a wake delta to previous wake deltas.
+        Add a wake delta to previous wake deltas,
+        at rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        sel_sp: numpy.ndarray of bool
-            The selection of points, shape: (n_states, n_points)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        st_sel: numpy.ndarray of bool
+            The selection of targets, shape: (n_states, n_targets)
         variable: str
             The variable name for which the wake deltas applies
         wake_delta: numpy.ndarray
-            The original wake deltas, shape: (n_states, n_points)
+            The original wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
         wake_model_result: numpy.ndarray
-            The new wake deltas of the selected points,
-            shape: (n_sel_sp,)
+            The new wake deltas of the selected rotors,
+            shape: (n_st_sel, n_tpoints, ...)
 
         Returns
         -------
         wdelta: numpy.ndarray
-            The updated wake deltas, shape: (n_states, n_points)
+            The updated wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
 
         """
         if variable not in [FV.REWS, FV.REWS2, FV.REWS3, FV.WS]:
             raise ValueError(
                 f"Superposition '{self.name}': Expecting wind speed variable, got {variable}"
             )
 
-        if np.any(sel_sp):
+        if np.any(st_sel):
             scale = self.get_data(
                 FV.AMB_REWS if self.scale_amb else FV.REWS,
-                FC.STATE_POINT,
+                FC.STATE_TARGET,
                 lookup="w",
                 algo=algo,
                 fdata=fdata,
-                pdata=pdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
                 upcast=True,
-                states_source_turbine=states_source_turbine,
-            )[sel_sp]
+            )[st_sel, None]
 
-            wake_delta[sel_sp] += scale * wake_model_result
+            wake_delta[st_sel] += np.abs(scale * wake_model_result) ** self.pow
 
         return wake_delta
 
     def calc_final_wake_delta(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
         variable,
         amb_results,
         wake_delta,
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
         variable: str
             The variable name for which the wake deltas applies
         amb_results: numpy.ndarray
-            The ambient results, shape: (n_states, n_points)
+            The ambient results at targets,
+            shape: (n_states, n_targets, n_tpoints)
         wake_delta: numpy.ndarray
-            The wake deltas, shape: (n_states, n_points)
+            The wake deltas at targets, shape:
+            (n_states, n_targets, n_tpoints)
 
         Returns
         -------
         final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
-            results by simple plus operation. Shape: (n_states, n_points)
+            results by simple plus operation. Shape:
+            (n_states, n_targets, n_tpoints)
 
         """
-        w = wake_delta
+        w = -(wake_delta ** (1 / self.pow))
         if self.lim_low is not None:
             w = np.maximum(w, self.lim_low - amb_results)
         if self.lim_high is not None:
             w = np.minimum(w, self.lim_high - amb_results)
         return w
```

### Comparing `foxes-0.6.2/foxes/models/wake_superpositions/ws_max.py` & `foxes-0.7/foxes/models/wake_superpositions/ws_quadratic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 
 from foxes.core import WakeSuperposition
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class WSMax(WakeSuperposition):
+class WSQuadratic(WakeSuperposition):
     """
-    Max supersposition of wind deficit results
+    Quadratic supersposition of wind deficit results
 
     Attributes
     ----------
     scale_amb: bool
         Flag for scaling wind deficit with ambient wind speed
         instead of waked wind speed
     lim_low: float
@@ -40,14 +40,18 @@
         """
         super().__init__()
 
         self.scale_amb = scale_amb
         self.lim_low = lim_low
         self.lim_high = lim_high
 
+    def __repr__(self):
+        a = f"scale_amb={self.scale_amb}, lim_low={self.lim_low}, lim_high={self.lim_high}"
+        return f"{type(self).__name__}({a})"
+
     def input_farm_vars(self, algo):
         """
         The variables which are needed for running
         the model.
 
         Parameters
         ----------
@@ -58,119 +62,119 @@
         -------
         input_vars: list of str
             The input variable names
 
         """
         return [FV.AMB_REWS] if self.scale_amb else [FV.REWS]
 
-    def calc_wakes_plus_wake(
+    def add_wake(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        sel_sp,
+        tdata,
+        downwind_index,
+        st_sel,
         variable,
         wake_delta,
         wake_model_result,
     ):
         """
-        Add a wake delta to previous wake deltas.
+        Add a wake delta to previous wake deltas,
+        at rotor points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        sel_sp: numpy.ndarray of bool
-            The selection of points, shape: (n_states, n_points)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        st_sel: numpy.ndarray of bool
+            The selection of targets, shape: (n_states, n_targets)
         variable: str
             The variable name for which the wake deltas applies
         wake_delta: numpy.ndarray
-            The original wake deltas, shape: (n_states, n_points)
+            The original wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
         wake_model_result: numpy.ndarray
-            The new wake deltas of the selected points,
-            shape: (n_sel_sp,)
+            The new wake deltas of the selected rotors,
+            shape: (n_st_sel, n_tpoints, ...)
 
         Returns
         -------
         wdelta: numpy.ndarray
-            The updated wake deltas, shape: (n_states, n_points)
+            The updated wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
 
         """
         if variable not in [FV.REWS, FV.REWS2, FV.REWS3, FV.WS]:
             raise ValueError(
                 f"Superposition '{self.name}': Expecting wind speed variable, got {variable}"
             )
 
-        if np.any(sel_sp):
+        if np.any(st_sel):
             scale = self.get_data(
                 FV.AMB_REWS if self.scale_amb else FV.REWS,
-                FC.STATE_POINT,
+                FC.STATE_TARGET,
                 lookup="w",
                 algo=algo,
                 fdata=fdata,
-                pdata=pdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
                 upcast=True,
-                states_source_turbine=states_source_turbine,
-            )[sel_sp]
-
-            wake_model_result = np.abs(scale * wake_model_result)
-            odelta = wake_delta[sel_sp]
+            )[st_sel, None]
 
-            wake_delta[sel_sp] = np.maximum(odelta, wake_model_result)
+            wake_delta[st_sel] += (scale * wake_model_result) ** 2
 
         return wake_delta
 
     def calc_final_wake_delta(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
         variable,
         amb_results,
         wake_delta,
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
         variable: str
             The variable name for which the wake deltas applies
         amb_results: numpy.ndarray
-            The ambient results, shape: (n_states, n_points)
+            The ambient results at targets,
+            shape: (n_states, n_targets, n_tpoints)
         wake_delta: numpy.ndarray
-            The wake deltas, shape: (n_states, n_points)
+            The wake deltas at targets, shape:
+            (n_states, n_targets, n_tpoints)
 
         Returns
         -------
         final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
-            results by simple plus operation. Shape: (n_states, n_points)
+            results by simple plus operation. Shape:
+            (n_states, n_targets, n_tpoints)
 
         """
-        w = -wake_delta
+        w = -np.sqrt(wake_delta)
         if self.lim_low is not None:
             w = np.maximum(w, self.lim_low - amb_results)
         if self.lim_high is not None:
             w = np.minimum(w, self.lim_high - amb_results)
         return w
```

### Comparing `foxes-0.6.2/foxes/models/wake_superpositions/ws_pow.py` & `foxes-0.7/foxes/models/partial_wakes/segregated.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,178 +1,158 @@
 import numpy as np
 
-from foxes.core import WakeSuperposition
+from foxes.core import PartialWakesModel
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class WSPow(WakeSuperposition):
+class PartialSegregated(PartialWakesModel):
     """
-    Power supersposition of wind deficit results
+    Add the averaged wake effects to the separately
+    averaged ambient rotor results
 
     Attributes
     ----------
-    pow: float
-        The power to which to take the wake results
-    scale_amb: bool
-        Flag for scaling wind deficit with ambient wind speed
-        instead of waked wind speed
-    lim_low: float
-        Lower limit of the final waked wind speed
-    lim_high: float
-        Upper limit of the final waked wind speed
+    rotor_model: foxes.core.RotorModel
+        The rotor model, default is the one from the algorithm
+    grotor: foxes.models.rotor_models.GridRotor
+        The grid rotor model
 
-    :group: models.wake_superpositions
+    :group: models.partial_wakes
 
     """
 
-    def __init__(self, pow, scale_amb=False, lim_low=None, lim_high=None):
+    def __init__(self, rotor_model):
         """
         Constructor.
 
         Parameters
         ----------
-        pow: float
-            The power to which to take the wake results
-        scale_amb: bool
-            Flag for scaling wind deficit with ambient wind speed
-            instead of waked wind speed
-        lim_low: float
-            Lower limit of the final waked wind speed
-        lim_high: float
-            Upper limit of the final waked wind speed
+        rotor_model: foxes.core.RotorModel
+            The rotor model for wake averaging
 
         """
         super().__init__()
 
-        self.pow = pow
-        self.scale_amb = scale_amb
-        self.lim_low = lim_low
-        self.lim_high = lim_high
+        self.rotor = rotor_model
+        self.YZ = self.var("YZ")
+        self.W = self.var(FV.WEIGHT)
 
-    def input_farm_vars(self, algo):
-        """
-        The variables which are needed for running
-        the model.
+    def __repr__(self):
+        return f"{type(self).__name__}(rotor_model={self.rotor.name})"
 
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
+    def sub_models(self):
+        """
+        List of all sub-models
 
         Returns
         -------
-        input_vars: list of str
-            The input variable names
+        smdls: list of foxes.core.Model
+            Names of all sub models
 
         """
-        return [FV.AMB_REWS] if self.scale_amb else [FV.REWS]
+        return super().sub_models() + [self.rotor]
 
-    def calc_wakes_plus_wake(
-        self,
-        algo,
-        mdata,
-        fdata,
-        pdata,
-        states_source_turbine,
-        sel_sp,
-        variable,
-        wake_delta,
-        wake_model_result,
-    ):
+    def get_wake_points(self, algo, mdata, fdata):
         """
-        Add a wake delta to previous wake deltas.
+        Get the wake calculation points, and their
+        weights.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        sel_sp: numpy.ndarray of bool
-            The selection of points, shape: (n_states, n_points)
-        variable: str
-            The variable name for which the wake deltas applies
-        wake_delta: numpy.ndarray
-            The original wake deltas, shape: (n_states, n_points)
-        wake_model_result: numpy.ndarray
-            The new wake deltas of the selected points,
-            shape: (n_sel_sp,)
 
         Returns
         -------
-        wdelta: numpy.ndarray
-            The updated wake deltas, shape: (n_states, n_points)
+        rpoints: numpy.ndarray
+            The wake calculation points, shape:
+            (n_states, n_turbines, n_tpoints, 3)
+        rweights: numpy.ndarray
+            The target point weights, shape: (n_tpoints,)
 
         """
-        if variable not in [FV.REWS, FV.REWS2, FV.REWS3, FV.WS]:
-            raise ValueError(
-                f"Superposition '{self.name}': Expecting wind speed variable, got {variable}"
-            )
-
-        if np.any(sel_sp):
-            scale = self.get_data(
-                FV.AMB_REWS if self.scale_amb else FV.REWS,
-                FC.STATE_POINT,
-                lookup="w",
-                algo=algo,
-                fdata=fdata,
-                pdata=pdata,
-                upcast=True,
-                states_source_turbine=states_source_turbine,
-            )[sel_sp]
-
-            wake_delta[sel_sp] += np.abs(scale * wake_model_result) ** self.pow
+        return (
+            self.rotor.get_rotor_points(algo, mdata, fdata),
+            self.rotor.rotor_point_weights(),
+        )
 
-        return wake_delta
-
-    def calc_final_wake_delta(
+    def finalize_wakes(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        variable,
-        amb_results,
-        wake_delta,
+        tdata,
+        amb_res,
+        rpoint_weights,
+        wake_deltas,
+        wmodel,
+        downwind_index,
     ):
         """
-        Calculate the final wake delta after adding all
-        contributions.
+        Updates the wake_deltas at the selected target
+        downwind index.
+
+        Modifies wake_deltas on the fly.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        variable: str
-            The variable name for which the wake deltas applies
-        amb_results: numpy.ndarray
-            The ambient results, shape: (n_states, n_points)
-        wake_delta: numpy.ndarray
-            The wake deltas, shape: (n_states, n_points)
+        tdata: foxes.core.Data
+            The target point data
+        amb_res: dict
+            The ambient results at the target points
+            of all rotors. Key: variable name, value
+            np.ndarray of shape:
+            (n_states, n_turbines, n_rotor_points)
+        rpoint_weights: numpy.ndarray
+            The rotor point weights, shape: (n_rotor_points,)
+        wake_deltas: dict
+            The wake deltas. Key: variable name,
+            value: np.ndarray of shape
+            (n_states, n_turbines, n_tpoints)
+        wmodel: foxes.core.WakeModel
+            The wake model
+        downwind_index: int
+            The index in the downwind order
 
         Returns
         -------
-        final_wake_delta: numpy.ndarray
-            The final wake delta, which will be added to the ambient
-            results by simple plus operation. Shape: (n_states, n_points)
+        final_wake_deltas: dict
+            The final wake deltas at the selected downwind
+            turbines. Key: variable name, value: np.ndarray
+            of shape (n_states, n_rotor_points)
+
+        """
+        n_states = fdata.n_states
+        n_rotor_points = len(rpoint_weights)
+        gweights = tdata[FC.TWEIGHTS]
+
+        wdel = {v: d[:, downwind_index, None].copy() for v, d in wake_deltas.items()}
+
+        if n_rotor_points == tdata.n_tpoints:
+            ares = {v: d[:, downwind_index, None] for v, d in amb_res.items()}
+        else:
+            ares = {}
+            for v, d in amb_res.items():
+                ares[v] = np.zeros((n_states, 1, tdata.n_tpoints), dtype=FC.DTYPE)
+                ares[v][:] = np.einsum("sp,p->s", d[:, downwind_index], rpoint_weights)[
+                    :, None, None
+                ]
+
+        wmodel.finalize_wake_deltas(algo, mdata, fdata, ares, wdel)
+
+        for v in wdel.keys():
+            hdel = np.zeros((n_states, n_rotor_points), dtype=FC.DTYPE)
+            hdel[:] = np.einsum("sp,p->s", wdel[v][:, 0], gweights)[:, None]
+            wdel[v] = hdel
 
-        """
-        w = -(wake_delta ** (1 / self.pow))
-        if self.lim_low is not None:
-            w = np.maximum(w, self.lim_low - amb_results)
-        if self.lim_high is not None:
-            w = np.minimum(w, self.lim_high - amb_results)
-        return w
+        return wdel
```

### Comparing `foxes-0.6.2/foxes/models/wake_superpositions/ws_quadratic.py` & `foxes-0.7/foxes/core/partial_wakes_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,173 +1,202 @@
-import numpy as np
+from abc import abstractmethod
 
-from foxes.core import WakeSuperposition
-import foxes.variables as FV
-import foxes.constants as FC
+from foxes.utils import all_subclasses
 
+from .model import Model
 
-class WSQuadratic(WakeSuperposition):
+
+class PartialWakesModel(Model):
     """
-    Quadratic supersposition of wind deficit results
+    Abstract base class for partial wakes models.
+
+    Partial wakes models compute wake effects
+    for rotor effective quantities.
 
     Attributes
     ----------
-    scale_amb: bool
-        Flag for scaling wind deficit with ambient wind speed
-        instead of waked wind speed
-    lim_low: float
-        Lower limit of the final waked wind speed
-    lim_high: float
-        Upper limit of the final waked wind speed
+    wake_models: list of foxes.core.WakeModel
+        The wake model selection
+    wake_frame: foxes.core.WakeFrame, optional
+        The wake frame
 
-    :group: models.wake_superpositions
+    :group: core
 
     """
 
-    def __init__(self, scale_amb=False, lim_low=None, lim_high=None):
+    @abstractmethod
+    def get_wake_points(self, algo, mdata, fdata):
         """
-        Constructor.
+        Get the wake calculation points, and their
+        weights.
 
         Parameters
         ----------
-        scale_amb: bool
-            Flag for scaling wind deficit with ambient wind speed
-            instead of waked wind speed
-        lim_low: float
-            Lower limit of the final waked wind speed
-        lim_high: float
-            Upper limit of the final waked wind speed
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.Data
+            The model data
+        fdata: foxes.core.Data
+            The farm data
 
-        """
-        super().__init__()
+        Returns
+        -------
+        rpoints: numpy.ndarray
+            The wake calculation points, shape:
+            (n_states, n_turbines, n_tpoints, 3)
+        rweights: numpy.ndarray
+            The target point weights, shape: (n_tpoints,)
 
-        self.scale_amb = scale_amb
-        self.lim_low = lim_low
-        self.lim_high = lim_high
+        """
+        pass
 
-    def input_farm_vars(self, algo):
+    def new_wake_deltas(self, algo, mdata, fdata, tdata, wmodel):
         """
-        The variables which are needed for running
-        the model.
+        Creates new initial wake deltas, filled
+        with zeros.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
+        mdata: foxes.core.Data
+            The model data
+        fdata: foxes.core.Data
+            The farm data
+        tdata: foxes.core.Data
+            The target point data
+        wmodel: foxes.core.WakeModel
+            The wake model
+        wpoints: numpy.ndarray
+            The wake evaluation points,
+            shape: (n_states, n_turbines, n_tpoints, 3)
 
         Returns
         -------
-        input_vars: list of str
-            The input variable names
+        wake_deltas: dict
+            Key: variable name, value: The zero filled
+            wake deltas, shape: (n_states, n_turbines, n_tpoints, ...)
 
         """
-        return [FV.AMB_REWS] if self.scale_amb else [FV.REWS]
+        return wmodel.new_wake_deltas(algo, mdata, fdata, tdata)
 
-    def calc_wakes_plus_wake(
+    def contribute(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        states_source_turbine,
-        sel_sp,
-        variable,
-        wake_delta,
-        wake_model_result,
+        tdata,
+        downwind_index,
+        wake_deltas,
+        wmodel,
     ):
         """
-        Add a wake delta to previous wake deltas.
+        Modifies wake deltas at target points by
+        contributions from the specified wake source turbines.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        sel_sp: numpy.ndarray of bool
-            The selection of points, shape: (n_states, n_points)
-        variable: str
-            The variable name for which the wake deltas applies
-        wake_delta: numpy.ndarray
-            The original wake deltas, shape: (n_states, n_points)
-        wake_model_result: numpy.ndarray
-            The new wake deltas of the selected points,
-            shape: (n_sel_sp,)
-
-        Returns
-        -------
-        wdelta: numpy.ndarray
-            The updated wake deltas, shape: (n_states, n_points)
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        wake_deltas: dict
+            The wake deltas. Key: variable name,
+            value: numpy.ndarray with shape
+            (n_states, n_targets, n_tpoints, ...)
+        wmodel: foxes.core.WakeModel
+            The wake model
 
         """
-        if variable not in [FV.REWS, FV.REWS2, FV.REWS3, FV.WS]:
-            raise ValueError(
-                f"Superposition '{self.name}': Expecting wind speed variable, got {variable}"
-            )
-
-        if np.any(sel_sp):
-            scale = self.get_data(
-                FV.AMB_REWS if self.scale_amb else FV.REWS,
-                FC.STATE_POINT,
-                lookup="w",
-                algo=algo,
-                fdata=fdata,
-                pdata=pdata,
-                upcast=True,
-                states_source_turbine=states_source_turbine,
-            )[sel_sp]
-
-            wake_delta[sel_sp] += (scale * wake_model_result) ** 2
-
-        return wake_delta
+        wcoos = algo.wake_frame.get_wake_coos(algo, mdata, fdata, tdata, downwind_index)
+        wmodel.contribute(algo, mdata, fdata, tdata, downwind_index, wcoos, wake_deltas)
 
-    def calc_final_wake_delta(
+    @abstractmethod
+    def finalize_wakes(
         self,
         algo,
         mdata,
         fdata,
-        pdata,
-        variable,
-        amb_results,
-        wake_delta,
+        tdata,
+        amb_res,
+        rpoint_weights,
+        wake_deltas,
+        wmodel,
+        downwind_index,
     ):
         """
-        Calculate the final wake delta after adding all
-        contributions.
+        Updates the wake_deltas at the selected target
+        downwind index.
+
+        Modifies wake_deltas on the fly.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
-        pdata: foxes.core.Data
-            The evaluation point data
-        variable: str
-            The variable name for which the wake deltas applies
-        amb_results: numpy.ndarray
-            The ambient results, shape: (n_states, n_points)
-        wake_delta: numpy.ndarray
-            The wake deltas, shape: (n_states, n_points)
+        tdata: foxes.core.Data
+            The target point data
+        amb_res: dict
+            The ambient results at the target points
+            of all rotors. Key: variable name, value
+            np.ndarray of shape:
+            (n_states, n_turbines, n_rotor_points)
+        rpoint_weights: numpy.ndarray
+            The rotor point weights, shape: (n_rotor_points,)
+        wake_deltas: dict
+            The wake deltas. Key: variable name,
+            value: np.ndarray of shape
+            (n_states, n_turbines, n_tpoints)
+        wmodel: foxes.core.WakeModel
+            The wake model
+        downwind_index: int
+            The index in the downwind order
 
         Returns
         -------
-        final_wake_delta: numpy.ndarray
-            The final wake delta, which will be added to the ambient
-            results by simple plus operation. Shape: (n_states, n_points)
+        final_wake_deltas: dict
+            The final wake deltas at the selected downwind
+            turbines. Key: variable name, value: np.ndarray
+            of shape (n_states, n_rotor_points)
+
+        """
+        pass
 
+    @classmethod
+    def new(cls, pwake_type, **kwargs):
         """
-        w = -np.sqrt(wake_delta)
-        if self.lim_low is not None:
-            w = np.maximum(w, self.lim_low - amb_results)
-        if self.lim_high is not None:
-            w = np.minimum(w, self.lim_high - amb_results)
-        return w
+        Run-time partial wakes factory.
+
+        Parameters
+        ----------
+        pwake_type: str
+            The selected derived class name
+
+        """
+
+        if pwake_type is None:
+            return None
+
+        allc = all_subclasses(cls)
+        found = pwake_type in [scls.__name__ for scls in allc]
+
+        if found:
+            for scls in allc:
+                if scls.__name__ == pwake_type:
+                    return scls(**kwargs)
+
+        else:
+            estr = "Partial wakes model type '{}' is not defined, available types are \n {}".format(
+                pwake_type, sorted([i.__name__ for i in allc])
+            )
+            raise KeyError(estr)
```

### Comparing `foxes-0.6.2/foxes/opt/constraints/area_geometry.py` & `foxes-0.7/foxes/opt/constraints/area_geometry.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/opt/constraints/min_dist.py` & `foxes-0.7/foxes/opt/constraints/min_dist.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/opt/core/farm_constraint.py` & `foxes-0.7/foxes/opt/core/farm_constraint.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/opt/core/farm_objective.py` & `foxes-0.7/foxes/opt/core/farm_objective.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/opt/core/farm_opt_problem.py` & `foxes-0.7/foxes/opt/core/farm_opt_problem.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/opt/core/farm_vars_problem.py` & `foxes-0.7/foxes/opt/core/farm_vars_problem.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/opt/objectives/farm_vars.py` & `foxes-0.7/foxes/opt/objectives/farm_vars.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/opt/problems/layout/geom_layouts/constraints.py` & `foxes-0.7/foxes/opt/problems/layout/geom_layouts/constraints.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/opt/problems/layout/geom_layouts/geom_layout.py` & `foxes-0.7/foxes/opt/problems/layout/geom_layouts/geom_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py` & `foxes-0.7/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py` & `foxes-0.7/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py` & `foxes-0.7/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/opt/problems/layout/geom_layouts/objectives.py` & `foxes-0.7/foxes/opt/problems/layout/geom_layouts/objectives.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/opt/problems/layout/reggrids_layout.py` & `foxes-0.7/foxes/opt/problems/layout/reggrids_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/opt/problems/layout/regular_layout.py` & `foxes-0.7/foxes/opt/problems/layout/regular_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/opt/problems/opt_farm_vars.py` & `foxes-0.7/foxes/opt/problems/opt_farm_vars.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/output/__init__.py` & `foxes-0.7/foxes/output/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,10 +9,11 @@
 from .rose_plot import RosePlotOutput, StatesRosePlotOutput
 from .results_writer import ResultsWriter
 from .state_turbine_map import StateTurbineMap
 from .turbine_type_curves import TurbineTypeCurves
 from .animation import Animator
 from .calc_points import PointCalculator
 from .slice_data import SliceData
+from .rotor_point_plots import RotorPointPlot
 
 from .flow_plots_2d import FlowPlots2D, SeqFlowAnimationPlugin
 from . import grids
```

### Comparing `foxes-0.6.2/foxes/output/animation.py` & `foxes-0.7/foxes/output/animation.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/output/farm_layout.py` & `foxes-0.7/foxes/output/farm_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/output/farm_results_eval.py` & `foxes-0.7/foxes/output/farm_results_eval.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/output/flow_plots_2d/flow_plots.py` & `foxes-0.7/foxes/output/flow_plots_2d/flow_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -721,14 +721,15 @@
         data, states, gdata = self.get_states_data_xz(
             variables=variables,
             vmin={var: vmin} if vmin is not None else {},
             vmax={var: vmax} if vmax is not None else {},
             data_format="numpy",
             ret_states=True,
             ret_grid=True,
+            x_direction=x_direction,
             **kwargs,
         )
         x_pos, y_pos, z_pos, __ = gdata
 
         # define wind vector arrows:
         qpars = dict(angles="xy", scale_units="xy", scale=0.05)
         qpars.update(quiver_pars)
@@ -894,14 +895,15 @@
         data, states, gdata = self.get_states_data_yz(
             variables=variables,
             vmin={var: vmin} if vmin is not None else {},
             vmax={var: vmax} if vmax is not None else {},
             data_format="numpy",
             ret_states=True,
             ret_grid=True,
+            x_direction=x_direction,
             **kwargs,
         )
         x_pos, y_pos, z_pos, __ = gdata
 
         # define wind vector arrows:
         qpars = dict(angles="xy", scale_units="xy", scale=0.05)
         qpars.update(quiver_pars)
```

### Comparing `foxes-0.6.2/foxes/output/flow_plots_2d/get_fig.py` & `foxes-0.7/foxes/output/flow_plots_2d/get_fig.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/output/flow_plots_2d/seq_flow_ani_plugin.py` & `foxes-0.7/foxes/output/flow_plots_2d/seq_flow_ani_plugin.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/output/grids.py` & `foxes-0.7/foxes/output/grids.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/output/output.py` & `foxes-0.7/foxes/output/output.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/output/results_writer.py` & `foxes-0.7/foxes/output/results_writer.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/output/rose_plot.py` & `foxes-0.7/foxes/output/rose_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
         Parameters
         ----------
         results: xarray.Dataset
             The calculation results (farm or points)
 
         """
-        dims = list(results.dims.keys())
+        dims = list(results.sizes.keys())
         if dims[1] == FC.TURBINE:
             self._rtype = FC.TURBINE
         elif dims[1] == FC.POINT:
             self._rtype = FC.POINT
         else:
             raise KeyError(
                 f"Results dimension 1 is neither '{FC.TURBINE}' nor '{FC.POINT}': dims = {results.dims}"
@@ -166,15 +166,15 @@
         data.drop(["u", "v"], axis=1, inplace=True)
         if not start0:
             data.loc[data["wd"] > 360.0 - dwd / 2, "wd"] -= 360.0
 
         data[wd_var] = pd.cut(data["wd"], wdb, labels=wds)
         data[lgd] = pd.cut(data[lgd], var_bins, right=False, include_lowest=True)
 
-        grp = data[[wd_var, lgd, "frequency"]].groupby([wd_var, lgd])
+        grp = data[[wd_var, lgd, "frequency"]].groupby([wd_var, lgd], observed=False)
         data = grp.sum().reset_index()
 
         data[wd_var] = data[wd_var].astype(np.float64)
         data[lgd] = list(data[lgd])
         if start0:
             data[wd_var] += dwd / 2
 
@@ -382,12 +382,12 @@
                 H=point[2],
                 turbine_models=["null_type"],
             ),
             verbosity=0,
         )
 
         mbook = mbook if mbook is not None else ModelBook()
-        algo = Downwind(mbook, farm, states, wake_models=[], verbosity=0)
+        algo = Downwind(farm, states, wake_models=[], mbook=mbook, verbosity=0)
 
         results = algo.calc_farm(ambient=True).rename_vars({ws_var: FV.AMB_WS})
 
         super().__init__(results)
```

### Comparing `foxes-0.6.2/foxes/output/slice_data.py` & `foxes-0.7/foxes/output/slice_data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/output/state_turbine_map.py` & `foxes-0.7/foxes/output/state_turbine_map.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/output/turbine_type_curves.py` & `foxes-0.7/foxes/output/turbine_type_curves.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
         farm = WindFarm()
         farm.add_turbine(
             Turbine(xy=[0.0, 0.0], turbine_models=models),
             verbosity=0,
         )
 
-        algo = Downwind(self.mbook, farm, states, wake_models=[], verbosity=0)
+        algo = Downwind(farm, states, wake_models=[], mbook=self.mbook, verbosity=0)
 
         results = algo.calc_farm()
 
         if P_max is not None:
             sname = f"_{type(self).__name__}_set_Pmax"
             self.mbook.turbine_models[sname] = SetFarmVars()
             self.mbook.turbine_models[sname].add_var(FV.MAX_P, P_max)
@@ -145,15 +145,15 @@
 
             farm = WindFarm()
             farm.add_turbine(
                 Turbine(xy=[0.0, 0.0], turbine_models=models),
                 verbosity=0,
             )
 
-            algo = Downwind(self.mbook, farm, states, wake_models=[], verbosity=0)
+            algo = Downwind(farm, states, wake_models=[], mbook=self.mbook, verbosity=0)
 
             results1 = algo.calc_farm()
 
             del self.mbook.turbine_models[sname]
 
         for i, v in enumerate(vars):
             ax = axs[i]
```

### Comparing `foxes-0.6.2/foxes/utils/__init__.py` & `foxes-0.7/foxes/utils/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .pandas_utils import PandasFileHelper
 from .xarray_utils import write_nc
 from .subclasses import all_subclasses
 from .dict import Dict
 from .data_book import DataBook
 from .cubic_roots import cubic_roots
 from .geopandas_utils import read_shp, shp2csv, read_shp_polygons, shp2geom2d
-from .load import import_module
+from .load import import_module, load_module
 from .exec_python import exec_python
 from .regularize import sqrt_reg
 from .windrose_plot import TabWindroseAxes
 from .tab_files import read_tab_file
 from .random_xy import random_xy_square
 
 from . import two_circles
```

### Comparing `foxes-0.6.2/foxes/utils/abl/neutral.py` & `foxes-0.7/foxes/utils/abl/neutral.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/abl/stable.py` & `foxes-0.7/foxes/utils/abl/stable.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/abl/unstable.py` & `foxes-0.7/foxes/utils/abl/unstable.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/cubic_roots.py` & `foxes-0.7/foxes/utils/cubic_roots.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/data_book.py` & `foxes-0.7/foxes/utils/data_book.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/dict.py` & `foxes-0.7/foxes/utils/dict.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/exec_python.py` & `foxes-0.7/foxes/utils/exec_python.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/geom2d/area_geometry.py` & `foxes-0.7/foxes/utils/geom2d/area_geometry.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/geom2d/circle.py` & `foxes-0.7/foxes/utils/geom2d/circle.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/geom2d/example_intersection.py` & `foxes-0.7/foxes/utils/geom2d/example_intersection.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/geom2d/example_union.py` & `foxes-0.7/foxes/utils/geom2d/example_union.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/geom2d/half_plane.py` & `foxes-0.7/foxes/utils/geom2d/half_plane.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/geom2d/polygon.py` & `foxes-0.7/foxes/utils/geom2d/polygon.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/geopandas_helpers.py` & `foxes-0.7/foxes/utils/geopandas_helpers.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/geopandas_utils.py` & `foxes-0.7/foxes/utils/geopandas_utils.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/pandas_helpers.py` & `foxes-0.7/foxes/utils/pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/pandas_utils.py` & `foxes-0.7/foxes/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/random_xy.py` & `foxes-0.7/foxes/utils/random_xy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import numpy as np
 from scipy.spatial.distance import cdist
 
+
 def random_xy_square(
-        n, 
-        min_dist=500, 
-        xmax_ini=None, 
-        growth=1.02, 
-        seed=None, 
-        verbosity=1,
-    ):
-    """ 
+    n,
+    min_dist=500,
+    xmax_ini=None,
+    growth=1.02,
+    seed=None,
+    verbosity=1,
+):
+    """
     Creates random xy positions within a square,
     with mean (0, 0)
 
     Parameters
     ----------
     n: int
         The number of positions
     min_dist: float
         The minimal distance between any two positions
     xmax_ini: float, optional
         The initial maximal distance of any coordinates
     growth: float
-        The growth factor of the initial radius, must be 
+        The growth factor of the initial radius, must be
         greater 1
     seed: int, optional
         The random seed
     verbosity: int
         The verbosity level. 0 = silent
-    
+
     Returns
     -------
     xy: numpy.ndarray
         The positions, shape: (n, 2)
 
     :group: utils
```

### Comparing `foxes-0.6.2/foxes/utils/regularize.py` & `foxes-0.7/foxes/utils/regularize.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/runners/runners.py` & `foxes-0.7/foxes/utils/runners/runners.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,23 +192,22 @@
 
     def initialize(self):
         """
         Initialize the runner
         """
         if self.scheduler is not None:
             dask.config.set(scheduler=self.scheduler)
-        
+
         if self.scheduler == "dthreads":
             self.print("Launching local dask cluster..")
 
             cargs = deepcopy(self.cluster_args)
             del cargs["processes"]
-            self._client = Client(
-                processes=False, **self.client_args, **cargs)
-            
+            self._client = Client(processes=False, **self.client_args, **cargs)
+
             self.print(f"Dashboard: {self._client.dashboard_link}\n")
 
         elif self.scheduler == "distributed":
             self.print("Launching local dask cluster..")
 
             self._cluster = LocalCluster(**self.cluster_args)
             self._client = Client(self._cluster, **self.client_args)
```

### Comparing `foxes-0.6.2/foxes/utils/tab_files.py` & `foxes-0.7/foxes/utils/tab_files.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/two_circles.py` & `foxes-0.7/foxes/utils/two_circles.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/wind_dir.py` & `foxes-0.7/foxes/utils/wind_dir.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/utils/windrose_plot.py` & `foxes-0.7/foxes/utils/windrose_plot.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
             if nsector is None:
                 nsector = 16
             angles = np.arange(0, -2 * np.pi, -2 * np.pi / nsector) + np.pi / 2
 
             angle = 360.0 / nsector
             dir_bins = np.arange(-angle / 2, 360.0 + angle, angle, dtype=float)
             dir_edges = dir_bins.tolist()
+
             dir_edges.pop(-1)
             dir_edges[0] = dir_edges.pop(-1)
             dir_bins[0] = 0.0
 
         table = np.histogram2d(
             x=var, y=direction, bins=[bins, dir_bins], density=False, weights=weights
         )[0]
@@ -115,15 +116,14 @@
         table = table[:, :-1]
 
         self._info["dir"], self._info["bins"], self._info["table"] = (
             dir_edges,
             bins,
             table,
         )
-
         return bins, nbins, nsector, colors, angles, kwargs
 
     def legend(self, loc="upper right", *args, **kwargs):
         return super().legend(loc, *args, **kwargs)
 
 
 if __name__ == "__main__":
```

### Comparing `foxes-0.6.2/foxes/utils/xarray_utils.py` & `foxes-0.7/foxes/utils/xarray_utils.py`

 * *Files identical despite different names*

### Comparing `foxes-0.6.2/foxes/variables.py` & `foxes-0.7/foxes/variables.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,24 @@
 """
 
 ORDER = "order"
 """ The turbine order
 :group: foxes.variables
 """
 
+ORDER_INV = "order_inv"
+""" The inverse of the turbine order
+:group: foxes.variables
+"""
+
+ORDER_SSEL = "order_ssel"
+""" The states selection for applying the order
+:group: foxes.variables
+"""
+
 WS = "WS"
 """ The wind speed in m/s
 :group: foxes.variables
 """
 
 WD = "WD"
 """ The wind direction in degrees
```

### Comparing `foxes-0.6.2/foxes.egg-info/PKG-INFO` & `foxes-0.7/foxes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxes
-Version: 0.6.2
+Version: 0.7
 Summary: Farm Optimization and eXtended yield Evaluation Software
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
 Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
@@ -34,14 +34,15 @@
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx-immaterial; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
 Requires-Dist: ipykernel; extra == "doc"
 Requires-Dist: ipywidgets; extra == "doc"
 Requires-Dist: m2r2; extra == "doc"
+Requires-Dist: lxml_html_clean; extra == "doc"
 Provides-Extra: all
 Requires-Dist: windio>=1.0; extra == "all"
 Requires-Dist: flake8; extra == "all"
 Requires-Dist: pytest; extra == "all"
 Requires-Dist: pymoo>=0.6; extra == "all"
 Requires-Dist: sphinx; extra == "all"
 Requires-Dist: sphinx-immaterial; extra == "all"
@@ -98,24 +99,23 @@
     volume = {8}, 
     number = {86}, 
     pages = {5464}, 
     journal = {Journal of Open Source Software} 
 }
  ```
 
-## Requirements
+## Installation via pip
 
 The supported Python versions are: 
 
 - `Python 3.8`
 - `Python 3.9`
 - `Python 3.10`
 - `Python 3.11`
-
-## Installation via pip
+- `Python 3.12`
 
 ### Virtual Python environment
 
 First create a new `venv` environment, for example called `foxes` and located at `~/venv/foxes` (choose any other convenient name and location in your file system if you prefer), by
 
 ```console
 python3 -m venv ~/venv/foxes
@@ -158,14 +158,22 @@
 cd foxes
 pip install -e .
 ```
 The last line makes sure that all your code changes are included whenever importing `foxes`. Concerning the `git clone` line, we actually recommend that you fork `foxes` on GitHub and then replace that command by cloning your fork instead.
 
 ## Installation via conda
 
+The supported Python versions are: 
+
+- `Python 3.8`
+- `Python 3.9`
+- `Python 3.10`
+- `Python 3.11`
+- `Python 3.12`
+
 ### Preparation
 
 It is strongly recommend to use the `libmamba` dependency solver instead of the default solver. Install it once by
 
 ```console
 conda install conda-libmamba-solver -n base -c conda-forge
 ```
@@ -229,20 +237,18 @@
 For detailed examples of how to run _foxes_, check the `examples` and `notebooks` folders in this repository. A minimal running example is the following, based on provided static `csv` data files:
 
 ```python
 import foxes
 
 states = foxes.input.states.Timeseries("timeseries_3000.csv.gz", ["WS", "WD","TI","RHO"])
 
-mbook = foxes.ModelBook()
-
 farm = foxes.WindFarm()
 foxes.input.farm_layout.add_from_file(farm, "test_farm_67.csv", turbine_models=["NREL5MW"])
 
-algo = foxes.algorithms.Downwind(mbook, farm, states, ["Jensen_linear_k007"])
+algo = foxes.algorithms.Downwind(farm, states, ["Jensen_linear_k007"])
 farm_results = algo.calc_farm()
 
 print(farm_results)
 ```
 
 ## Testing
```

### Comparing `foxes-0.6.2/foxes.egg-info/SOURCES.txt` & `foxes-0.7/foxes.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 foxes.egg-info/requires.txt
 foxes.egg-info/top_level.txt
 foxes.egg-info/zip-safe
 foxes/algorithms/__init__.py
 foxes/algorithms/downwind/__init__.py
 foxes/algorithms/downwind/downwind.py
 foxes/algorithms/downwind/models/__init__.py
-foxes/algorithms/downwind/models/calc_order.py
 foxes/algorithms/downwind/models/farm_wakes_calc.py
+foxes/algorithms/downwind/models/init_farm_data.py
 foxes/algorithms/downwind/models/point_wakes_calc.py
+foxes/algorithms/downwind/models/reorder_farm_output.py
 foxes/algorithms/downwind/models/set_amb_farm_results.py
 foxes/algorithms/downwind/models/set_amb_point_results.py
 foxes/algorithms/iterative/__init__.py
 foxes/algorithms/iterative/iterative.py
 foxes/algorithms/iterative/models/__init__.py
 foxes/algorithms/iterative/models/convergence.py
 foxes/algorithms/iterative/models/farm_wakes_calc.py
@@ -103,18 +104,17 @@
 foxes/models/farm_controllers/__init__.py
 foxes/models/farm_controllers/basic.py
 foxes/models/farm_models/__init__.py
 foxes/models/farm_models/turbine2farm.py
 foxes/models/partial_wakes/__init__.py
 foxes/models/partial_wakes/axiwake.py
 foxes/models/partial_wakes/centre.py
-foxes/models/partial_wakes/distsliced.py
 foxes/models/partial_wakes/grid.py
-foxes/models/partial_wakes/mapped.py
 foxes/models/partial_wakes/rotor_points.py
+foxes/models/partial_wakes/segregated.py
 foxes/models/partial_wakes/top_hat.py
 foxes/models/point_models/__init__.py
 foxes/models/point_models/set_uniform_data.py
 foxes/models/point_models/tke2ti.py
 foxes/models/point_models/wake_deltas.py
 foxes/models/rotor_models/__init__.py
 foxes/models/rotor_models/centre.py
@@ -123,15 +123,14 @@
 foxes/models/turbine_models/__init__.py
 foxes/models/turbine_models/calculator.py
 foxes/models/turbine_models/kTI_model.py
 foxes/models/turbine_models/lookup_table.py
 foxes/models/turbine_models/power_mask.py
 foxes/models/turbine_models/rotor_centre_calc.py
 foxes/models/turbine_models/sector_management.py
-foxes/models/turbine_models/set_XYHD.py
 foxes/models/turbine_models/set_farm_vars.py
 foxes/models/turbine_models/table_factors.py
 foxes/models/turbine_models/thrust2ct.py
 foxes/models/turbine_models/yaw2yawm.py
 foxes/models/turbine_models/yawm2yaw.py
 foxes/models/turbine_types/CpCt_file.py
 foxes/models/turbine_types/CpCt_from_two.py
@@ -217,14 +216,15 @@
 foxes/output/farm_layout.py
 foxes/output/farm_results_eval.py
 foxes/output/flow_plots_2d.py
 foxes/output/grids.py
 foxes/output/output.py
 foxes/output/results_writer.py
 foxes/output/rose_plot.py
+foxes/output/rotor_point_plots.py
 foxes/output/round.py
 foxes/output/slice_data.py
 foxes/output/state_turbine_map.py
 foxes/output/turbine_type_curves.py
 foxes/output/flow_plots_2d/__init__.py
 foxes/output/flow_plots_2d/flow_plots.py
 foxes/output/flow_plots_2d/get_fig.py
```

### Comparing `foxes-0.6.2/setup.cfg` & `foxes-0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 doc = 
 	sphinx
 	sphinx-immaterial
 	nbsphinx
 	ipykernel
 	ipywidgets
 	m2r2
+	lxml_html_clean
 all = 
 	windio>=1.0
 	flake8
 	pytest
 	pymoo>=0.6
 	sphinx
 	sphinx-immaterial
```

