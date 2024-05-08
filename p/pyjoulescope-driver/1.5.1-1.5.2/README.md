# Comparing `tmp/pyjoulescope_driver-1.5.1.tar.gz` & `tmp/pyjoulescope_driver-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjoulescope_driver-1.5.1.tar", last modified: Fri Apr 26 12:32:40 2024, max compression
+gzip compressed data, was "pyjoulescope_driver-1.5.2.tar", last modified: Wed May  8 14:58:40 2024, max compression
```

## Comparing `pyjoulescope_driver-1.5.1.tar` & `pyjoulescope_driver-1.5.2.tar`

### file list

```diff
@@ -1,438 +1,438 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.992906 pyjoulescope_driver-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-26 12:32:40.992906 pyjoulescope_driver-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/credits.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.916907 pyjoulescope_driver-1.5.1/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.916907 pyjoulescope_driver-1.5.1/include/jsdrv/
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include/jsdrv/cmacro_inc.h
--rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include/jsdrv/cstr.h
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include/jsdrv/error_code.h
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include/jsdrv/log.h
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include/jsdrv/meta.h
--rw-r--r--   0 runner    (1001) docker     (127)    13434 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include/jsdrv/time.h
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include/jsdrv/topic.h
--rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include/jsdrv/union.h
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include/jsdrv/version.h
--rw-r--r--   0 runner    (1001) docker     (127)    29008 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include/jsdrv.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.920907 pyjoulescope_driver-1.5.1/include_private/
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/js220_api.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.924907 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/assert.h
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/backend.h
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/buffer.h
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/buffer_signal.h
--rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/cdef.h
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/dbc.h
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/device.h
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/devices.h
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/downsample.h
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/event.h
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/frontend.h
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/js110_cal.h
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/js110_sample_processor.h
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/js110_stats.h
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/js220_i128.h
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/js220_stats.h
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/json.h
--rw-r--r--   0 runner    (1001) docker     (127)    13617 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/list.h
--rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/log.h
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/msg_queue.h
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/mutex.h
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/platform.h
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/pubsub.h
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/sample_buffer_f32.h
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/statistics.h
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/thread.h
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/time_map_filter.h
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/usb_spec.h
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/windows.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.928907 pyjoulescope_driver-1.5.1/pyjoulescope_driver/
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2058853 2024-04-26 12:32:38.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/binding.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.932906 pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/api_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/gpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/set_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/threads.py
--rw-r--r--   0 runner    (1001) docker     (127)   631808 2024-04-26 12:32:40.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/img_alpha.img
--rw-r--r--   0 runner    (1001) docker     (127)   631808 2024-04-26 12:32:40.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/img_beta.img
--rw-r--r--   0 runner    (1001) docker     (127)   631808 2024-04-26 12:32:40.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/img_stable.img
--rw-r--r--   0 runner    (1001) docker     (127)    10121 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.932906 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.932906 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.936907 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_app/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_app/index.json
--rw-r--r--   0 runner    (1001) docker     (127)   104448 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_app/js220_ctrl_app_1_0_1.img
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_app/js220_ctrl_app_1_0_1_CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.936907 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater1/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater1/index.json
--rw-r--r--   0 runner    (1001) docker     (127)   104448 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater1/js220_ctrl_updater1_1_0_1.img
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater1/js220_ctrl_updater1_1_0_1_CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.936907 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater2/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater2/index.json
--rw-r--r--   0 runner    (1001) docker     (127)   104448 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater2/js220_ctrl_updater2_1_0_1.img
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater2/js220_ctrl_updater2_1_0_1_CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/index.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.940907 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/sensor_fpga/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/sensor_fpga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/sensor_fpga/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/sensor_fpga/index.json
--rw-r--r--   0 runner    (1001) docker     (127)   291840 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/sensor_fpga/js220_fpga_1_0_1.img
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/sensor_fpga/js220_fpga_1_0_1_CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/test_calibration_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/test_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/test_time64.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/time64.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.992906 pyjoulescope_driver-1.5.1/pyjoulescope_driver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-26 12:32:40.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15137 2024-04-26 12:32:40.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 12:32:40.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-26 12:32:40.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 12:32:40.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-26 12:32:40.000000 pyjoulescope_driver-1.5.1/pyjoulescope_driver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-26 12:32:40.992906 pyjoulescope_driver-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.944907 pyjoulescope_driver-1.5.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.944907 pyjoulescope_driver-1.5.1/src/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.944907 pyjoulescope_driver-1.5.1/src/backend/libusb/
--rw-r--r--   0 runner    (1001) docker     (127)    29503 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/backend/libusb/backend.c
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/backend/libusb/msg_queue.c
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/backend/posix.c
--rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/backend/windows.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.944907 pyjoulescope_driver-1.5.1/src/backend/winusb/
--rw-r--r--   0 runner    (1001) docker     (127)    37443 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/backend/winusb/backend.c
--rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/backend/winusb/device_change_notifier.c
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/backend/winusb/device_change_notifier.h
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/backend/winusb/msg_queue.c
--rw-r--r--   0 runner    (1001) docker     (127)    27269 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/buffer.c
--rw-r--r--   0 runner    (1001) docker     (127)    31877 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/buffer_signal.c
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/calibration_hash.c
--rw-r--r--   0 runner    (1001) docker     (127)    13226 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/cstr.c
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/devices.c
--rw-r--r--   0 runner    (1001) docker     (127)    10229 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/downsample.c
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/emu.c
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/emulated.c
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/error_code.c
--rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/js110_api.h
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/js110_cal.c
--rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/js110_sample_processor.c
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/js110_stats.c
--rw-r--r--   0 runner    (1001) docker     (127)    56352 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/js110_usb.c
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/js220_i128.c
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/js220_params.c
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/js220_stats.c
--rw-r--r--   0 runner    (1001) docker     (127)    66170 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/js220_usb.c
--rw-r--r--   0 runner    (1001) docker     (127)    38869 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/jsdrv.c
--rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/json.c
--rw-r--r--   0 runner    (1001) docker     (127)    15969 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/log.c
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/meta.c
--rw-r--r--   0 runner    (1001) docker     (127)    23556 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/pubsub.c
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/sample_buffer_f32.c
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/statistics.c
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/time.c
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/time_map_filter.c
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/topic.c
--rw-r--r--   0 runner    (1001) docker     (127)    12502 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/union.c
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/src/version.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.948907 pyjoulescope_driver-1.5.1/third-party/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.948907 pyjoulescope_driver-1.5.1/third-party/cmocka/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/.clang_complete
--rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/.ycm_extra_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/5.patch
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/CPackConfig.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/CTestConfig.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/CompilerChecks.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/ConfigureChecks.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/DefineOptions.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.948907 pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.952906 pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/FindNSIS.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Toolchain-cross-m32.cmake
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/cmocka-build-tree-settings.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/cmocka-config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/cmocka.pc.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/config.h.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.952906 pyjoulescope_driver-1.5.1/third-party/cmocka/coverity/
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/coverity/coverity_assert_model.c
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/coverity/coverity_internal_model.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.952906 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26268 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/mainpage.dox
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.952906 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.952906 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/doc.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/folderclosed.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/folderopen.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/mag_glass.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/nav_edge_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/nav_edge_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/splitbar_handle.svg
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/sync_off.png
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/sync_on.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.956906 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/js/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/js/striped_bg.js
--rw-r--r--   0 runner    (1001) docker     (127)    31024 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/that_style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.956906 pyjoulescope_driver-1.5.1/third-party/cmocka/example/
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/allocate_module.c
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/allocate_module_test.c
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/assert_macro.c
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/assert_macro.h
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/assert_macro_test.c
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/assert_module.c
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/assert_module.h
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/assert_module_test.c
--rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/calculator.c
--rw-r--r--   0 runner    (1001) docker     (127)    15762 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/calculator_test.c
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/database.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.956906 pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.956906 pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/chef_wrap/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/chef_wrap/chef.c
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/chef_wrap/chef.h
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.960907 pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/uptime/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/uptime/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/uptime/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/uptime/proc_uptime.c
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/uptime/proc_uptime.h
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/uptime/test_uptime.c
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/uptime/uptime.c
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/example/simple_test.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.960907 pyjoulescope_driver-1.5.1/third-party/cmocka/include/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/include/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    75566 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/include/cmocka.h
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/include/cmocka_pbc.h
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/include/cmocka_private.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.960907 pyjoulescope_driver-1.5.1/third-party/cmocka/include/cmockery/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/include/cmockery/cmockery.h
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/include/cmockery/pbc.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.960907 pyjoulescope_driver-1.5.1/third-party/cmocka/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)   116417 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/src/cmocka.c
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/src/cmocka.def
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.964907 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/cmocka_test.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/ctest-default.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_alloc.c
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_assert_macros.c
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_assert_macros_fail.c
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_basics.c
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_cmockery.c
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_exception_handler.c
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_fixtures.c
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_float_macros.c
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_group_fixtures.c
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_group_setup_assert.c
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_group_setup_fail.c
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_groups.c
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_ordering.c
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_ordering_fail.c
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_returns.c
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_returns_fail.c
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_setup_fail.c
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_skip.c
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_skip_filter.c
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_strmatch.c
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_wildcard.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.968906 pyjoulescope_driver-1.5.1/third-party/libusb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.968906 pyjoulescope_driver-1.5.1/third-party/libusb/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/.github/cifuzz.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.968906 pyjoulescope_driver-1.5.1/third-party/libusb/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/.github/workflows/linux.yml
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/.github/workflows/msys2.yml
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.968906 pyjoulescope_driver-1.5.1/third-party/libusb/.private/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/.private/README.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      526 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/.private/appveyor_build.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1370 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/.private/bm.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1042 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/.private/ci-build.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1404 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/.private/ci-container-build.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/.private/post-rewrite.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1943 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/.private/pre-commit.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/.private/wbs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/INSTALL_WIN.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/README-FORK.md
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/README.git
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.972906 pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/common.xcconfig
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/debug.xcconfig
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/libusb.xcconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.972906 pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/libusb.xcodeproj/
--rw-r--r--   0 runner    (1001) docker     (127)    60925 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/libusb_debug.xcconfig
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/libusb_release.xcconfig
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/release.xcconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.972906 pyjoulescope_driver-1.5.1/third-party/libusb/android/
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/android/config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.972906 pyjoulescope_driver-1.5.1/third-party/libusb/android/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/android/examples/unrooted_android.c
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/android/examples/unrooted_android.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.972906 pyjoulescope_driver-1.5.1/third-party/libusb/android/jni/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/android/jni/Android.mk
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/android/jni/Application.mk
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/android/jni/examples.mk
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/android/jni/libusb.mk
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/android/jni/tests.mk
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/appveyor.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/autogen.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       99 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (127)    16083 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/configure.ac
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.972906 pyjoulescope_driver-1.5.1/third-party/libusb/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/doc/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)   113076 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/doc/doxygen.cfg.in
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/doc/libusb.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.976906 pyjoulescope_driver-1.5.1/third-party/libusb/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/examples/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (127)    15101 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/examples/dpfp.c
--rw-r--r--   0 runner    (1001) docker     (127)    23732 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/examples/ezusb.c
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/examples/ezusb.h
--rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/examples/fxload.c
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/examples/hotplugtest.c
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/examples/listdevs.c
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/examples/sam3u_benchmark.c
--rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/examples/testlibusb.c
--rw-r--r--   0 runner    (1001) docker     (127)    38869 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/examples/xusb.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.916907 pyjoulescope_driver-1.5.1/third-party/libusb/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.976906 pyjoulescope_driver-1.5.1/third-party/libusb/include/linux/
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/include/linux/config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.976906 pyjoulescope_driver-1.5.1/third-party/libusb/include/macos/
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/include/macos/config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.980906 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/Makefile.am.extra
--rw-r--r--   0 runner    (1001) docker     (127)    96432 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/core.c
--rw-r--r--   0 runner    (1001) docker     (127)    36393 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/descriptor.c
--rw-r--r--   0 runner    (1001) docker     (127)    15083 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/hotplug.c
--rw-r--r--   0 runner    (1001) docker     (127)   111044 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/io.c
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/libusb-1.0.def
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/libusb-1.0.rc
--rw-r--r--   0 runner    (1001) docker     (127)    76595 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/libusb.h
--rw-r--r--   0 runner    (1001) docker     (127)    52013 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/libusbi.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.984907 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/
--rw-r--r--   0 runner    (1001) docker     (127)   100505 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/darwin_usb.c
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/darwin_usb.h
--rw-r--r--   0 runner    (1001) docker     (127)    23699 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/emscripten_webusb.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/events_posix.c
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/events_posix.h
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/events_windows.c
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/events_windows.h
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/haiku_pollfs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/haiku_usb.h
--rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/haiku_usb_backend.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/haiku_usb_raw.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/haiku_usb_raw.h
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/linux_netlink.c
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/linux_udev.c
--rw-r--r--   0 runner    (1001) docker     (127)    80453 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/linux_usbfs.c
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/linux_usbfs.h
--rw-r--r--   0 runner    (1001) docker     (127)    15662 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/netbsd_usb.c
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/null_usb.c
--rw-r--r--   0 runner    (1001) docker     (127)    17479 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/openbsd_usb.c
--rw-r--r--   0 runner    (1001) docker     (127)    43595 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/sunos_usb.c
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/sunos_usb.h
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/threads_posix.c
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/threads_posix.h
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/threads_windows.c
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/threads_windows.h
--rw-r--r--   0 runner    (1001) docker     (127)    29603 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/windows_common.c
--rw-r--r--   0 runner    (1001) docker     (127)    13931 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/windows_common.h
--rw-r--r--   0 runner    (1001) docker     (127)    23767 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/windows_usbdk.c
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/windows_usbdk.h
--rw-r--r--   0 runner    (1001) docker     (127)   166758 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/windows_winusb.c
--rw-r--r--   0 runner    (1001) docker     (127)    23891 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/windows_winusb.h
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/strerror.c
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/sync.c
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/version.h
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb/version_nano.h
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/libusb-1.0.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.988906 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/Base.props
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/Configuration.Application.props
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/Configuration.Base.props
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/Configuration.DynamicLibrary.props
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/Configuration.StaticLibrary.props
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/ProjectConfigurations.Base.props
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/build_all.ps1
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/dpfp.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/dpfp_threaded.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/fxload.vcxproj
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.988906 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/getopt/
--rw-r--r--   0 runner    (1001) docker     (127)    30281 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/getopt/getopt.c
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/getopt/getopt.h
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/getopt/getopt1.c
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/getopt.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/hotplugtest.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)    17271 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/libusb.sln
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/libusb_dll.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/libusb_static.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/listdevs.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/sam3u_benchmark.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/stress.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/testlibusb.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/msvc/xusb.vcxproj
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.992906 pyjoulescope_driver-1.5.1/third-party/libusb/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/tests/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/tests/libusb_testlib.h
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/tests/stress.c
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/tests/testlib.c
--rw-r--r--   0 runner    (1001) docker     (127)    36048 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/libusb/tests/umockdev.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 12:32:40.992906 pyjoulescope_driver-1.5.1/third-party/tinyprintf/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/tinyprintf/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/tinyprintf/tinyprintf.c
--rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/tinyprintf/tinyprintf.h
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-26 12:32:30.000000 pyjoulescope_driver-1.5.1/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.619052 pyjoulescope_driver-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11400 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-05-08 14:58:40.619052 pyjoulescope_driver-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/credits.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.547051 pyjoulescope_driver-1.5.2/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.551051 pyjoulescope_driver-1.5.2/include/jsdrv/
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include/jsdrv/cmacro_inc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include/jsdrv/cstr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include/jsdrv/error_code.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include/jsdrv/log.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include/jsdrv/meta.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13434 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include/jsdrv/time.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include/jsdrv/topic.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include/jsdrv/union.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include/jsdrv/version.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29008 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include/jsdrv.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.551051 pyjoulescope_driver-1.5.2/include_private/
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/js220_api.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.555051 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/assert.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/backend.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/buffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/buffer_signal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/cdef.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/dbc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/device.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/devices.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/downsample.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/event.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/frontend.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/js110_cal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/js110_sample_processor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/js110_stats.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/js220_i128.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/js220_stats.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/json.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13617 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/list.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/log.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/msg_queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/mutex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/platform.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/pubsub.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/sample_buffer_f32.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/statistics.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/thread.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/time_map_filter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/usb_spec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/windows.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.559051 pyjoulescope_driver-1.5.2/pyjoulescope_driver/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2058853 2024-05-08 14:58:37.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/binding.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.563051 pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/api_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/gpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/set_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)   631808 2024-05-08 14:58:40.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/img_alpha.img
+-rw-r--r--   0 runner    (1001) docker     (127)   631808 2024-05-08 14:58:40.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/img_beta.img
+-rw-r--r--   0 runner    (1001) docker     (127)   631808 2024-05-08 14:58:40.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/img_stable.img
+-rw-r--r--   0 runner    (1001) docker     (127)    10121 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.563051 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.563051 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.567051 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_app/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_app/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)   104448 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_app/js220_ctrl_app_1_0_1.img
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_app/js220_ctrl_app_1_0_1_CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.567051 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater1/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater1/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)   104448 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater1/js220_ctrl_updater1_1_0_1.img
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater1/js220_ctrl_updater1_1_0_1_CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.567051 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater2/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater2/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)   104448 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater2/js220_ctrl_updater2_1_0_1.img
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater2/js220_ctrl_updater2_1_0_1_CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/index.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.571051 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/sensor_fpga/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/sensor_fpga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/sensor_fpga/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/sensor_fpga/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)   291840 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/sensor_fpga/js220_fpga_1_0_1.img
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/sensor_fpga/js220_fpga_1_0_1_CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/test_calibration_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/test_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/test_time64.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/time64.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.619052 pyjoulescope_driver-1.5.2/pyjoulescope_driver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-05-08 14:58:40.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15137 2024-05-08 14:58:40.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:58:40.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 14:58:40.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 14:58:40.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-08 14:58:40.000000 pyjoulescope_driver-1.5.2/pyjoulescope_driver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-08 14:58:40.619052 pyjoulescope_driver-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.575051 pyjoulescope_driver-1.5.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.575051 pyjoulescope_driver-1.5.2/src/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.575051 pyjoulescope_driver-1.5.2/src/backend/libusb/
+-rw-r--r--   0 runner    (1001) docker     (127)    29503 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/backend/libusb/backend.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/backend/libusb/msg_queue.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/backend/posix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/backend/windows.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.575051 pyjoulescope_driver-1.5.2/src/backend/winusb/
+-rw-r--r--   0 runner    (1001) docker     (127)    37443 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/backend/winusb/backend.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/backend/winusb/device_change_notifier.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/backend/winusb/device_change_notifier.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/backend/winusb/msg_queue.c
+-rw-r--r--   0 runner    (1001) docker     (127)    27269 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/buffer.c
+-rw-r--r--   0 runner    (1001) docker     (127)    31877 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/buffer_signal.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/calibration_hash.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13226 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/cstr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/devices.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10229 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/downsample.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/emu.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/emulated.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/error_code.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/js110_api.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/js110_cal.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/js110_sample_processor.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/js110_stats.c
+-rw-r--r--   0 runner    (1001) docker     (127)    56352 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/js110_usb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/js220_i128.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/js220_params.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/js220_stats.c
+-rw-r--r--   0 runner    (1001) docker     (127)    66170 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/js220_usb.c
+-rw-r--r--   0 runner    (1001) docker     (127)    38869 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/jsdrv.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/json.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15969 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/log.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/meta.c
+-rw-r--r--   0 runner    (1001) docker     (127)    23556 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/pubsub.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/sample_buffer_f32.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/statistics.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/time.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/time_map_filter.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/topic.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12502 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/union.c
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/src/version.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.575051 pyjoulescope_driver-1.5.2/third-party/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.579051 pyjoulescope_driver-1.5.2/third-party/cmocka/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/.clang_complete
+-rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/.ycm_extra_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/5.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/CPackConfig.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/CTestConfig.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/CompilerChecks.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/ConfigureChecks.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/DefineOptions.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.579051 pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.583052 pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/FindNSIS.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Toolchain-cross-m32.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/cmocka-build-tree-settings.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/cmocka-config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/cmocka.pc.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/config.h.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.583052 pyjoulescope_driver-1.5.2/third-party/cmocka/coverity/
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/coverity/coverity_assert_model.c
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/coverity/coverity_internal_model.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.583052 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26268 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/mainpage.dox
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.583052 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.583052 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/doc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/folderclosed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/folderopen.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/mag_glass.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/nav_edge_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/nav_edge_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/splitbar_handle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/sync_off.png
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/sync_on.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.583052 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/js/striped_bg.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31024 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/that_style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.587051 pyjoulescope_driver-1.5.2/third-party/cmocka/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/allocate_module.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/allocate_module_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/assert_macro.c
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/assert_macro.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/assert_macro_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/assert_module.c
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/assert_module.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/assert_module_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/calculator.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15762 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/calculator_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/database.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.587051 pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.587051 pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/chef_wrap/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/chef_wrap/chef.c
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/chef_wrap/chef.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.591051 pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/uptime/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/uptime/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/uptime/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/uptime/proc_uptime.c
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/uptime/proc_uptime.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/uptime/test_uptime.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/uptime/uptime.c
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/example/simple_test.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.591051 pyjoulescope_driver-1.5.2/third-party/cmocka/include/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/include/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    75566 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/include/cmocka.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/include/cmocka_pbc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/include/cmocka_private.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.591051 pyjoulescope_driver-1.5.2/third-party/cmocka/include/cmockery/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/include/cmockery/cmockery.h
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/include/cmockery/pbc.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.591051 pyjoulescope_driver-1.5.2/third-party/cmocka/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   116417 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/src/cmocka.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/src/cmocka.def
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.595052 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/cmocka_test.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/ctest-default.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_alloc.c
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_assert_macros.c
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_assert_macros_fail.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_basics.c
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_cmockery.c
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_exception_handler.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_fixtures.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_float_macros.c
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_group_fixtures.c
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_group_setup_assert.c
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_group_setup_fail.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_groups.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_ordering.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_ordering_fail.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_returns.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_returns_fail.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_setup_fail.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_skip.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_skip_filter.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_strmatch.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_wildcard.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.599052 pyjoulescope_driver-1.5.2/third-party/libusb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.599052 pyjoulescope_driver-1.5.2/third-party/libusb/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/.github/cifuzz.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.599052 pyjoulescope_driver-1.5.2/third-party/libusb/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/.github/workflows/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/.github/workflows/msys2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.599052 pyjoulescope_driver-1.5.2/third-party/libusb/.private/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/.private/README.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      526 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/.private/appveyor_build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1370 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/.private/bm.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1042 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/.private/ci-build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1404 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/.private/ci-container-build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/.private/post-rewrite.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1943 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/.private/pre-commit.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/.private/wbs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/INSTALL_WIN.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/README-FORK.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/README.git
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.599052 pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/common.xcconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/debug.xcconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/libusb.xcconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.599052 pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/libusb.xcodeproj/
+-rw-r--r--   0 runner    (1001) docker     (127)    60925 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/libusb_debug.xcconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/libusb_release.xcconfig
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/release.xcconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.599052 pyjoulescope_driver-1.5.2/third-party/libusb/android/
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/android/config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.603052 pyjoulescope_driver-1.5.2/third-party/libusb/android/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/android/examples/unrooted_android.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/android/examples/unrooted_android.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.603052 pyjoulescope_driver-1.5.2/third-party/libusb/android/jni/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/android/jni/Android.mk
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/android/jni/Application.mk
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/android/jni/examples.mk
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/android/jni/libusb.mk
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/android/jni/tests.mk
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/appveyor.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/autogen.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       99 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    16083 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/configure.ac
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.603052 pyjoulescope_driver-1.5.2/third-party/libusb/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/doc/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)   113076 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/doc/doxygen.cfg.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/doc/libusb.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.603052 pyjoulescope_driver-1.5.2/third-party/libusb/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/examples/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (127)    15101 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/examples/dpfp.c
+-rw-r--r--   0 runner    (1001) docker     (127)    23732 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/examples/ezusb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/examples/ezusb.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/examples/fxload.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/examples/hotplugtest.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/examples/listdevs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/examples/sam3u_benchmark.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/examples/testlibusb.c
+-rw-r--r--   0 runner    (1001) docker     (127)    38869 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/examples/xusb.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.547051 pyjoulescope_driver-1.5.2/third-party/libusb/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.603052 pyjoulescope_driver-1.5.2/third-party/libusb/include/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/include/linux/config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.607052 pyjoulescope_driver-1.5.2/third-party/libusb/include/macos/
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/include/macos/config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.607052 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/Makefile.am.extra
+-rw-r--r--   0 runner    (1001) docker     (127)    96432 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/core.c
+-rw-r--r--   0 runner    (1001) docker     (127)    36393 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/descriptor.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15083 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/hotplug.c
+-rw-r--r--   0 runner    (1001) docker     (127)   111044 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/io.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/libusb-1.0.def
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/libusb-1.0.rc
+-rw-r--r--   0 runner    (1001) docker     (127)    76595 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/libusb.h
+-rw-r--r--   0 runner    (1001) docker     (127)    52013 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/libusbi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.615052 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/
+-rw-r--r--   0 runner    (1001) docker     (127)   100505 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/darwin_usb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/darwin_usb.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23699 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/emscripten_webusb.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/events_posix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/events_posix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/events_windows.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/events_windows.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/haiku_pollfs.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/haiku_usb.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/haiku_usb_backend.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/haiku_usb_raw.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/haiku_usb_raw.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/linux_netlink.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/linux_udev.c
+-rw-r--r--   0 runner    (1001) docker     (127)    80453 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/linux_usbfs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/linux_usbfs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15662 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/netbsd_usb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/null_usb.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17479 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/openbsd_usb.c
+-rw-r--r--   0 runner    (1001) docker     (127)    43595 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/sunos_usb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/sunos_usb.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/threads_posix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/threads_posix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/threads_windows.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/threads_windows.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29603 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/windows_common.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13931 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/windows_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23767 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/windows_usbdk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/windows_usbdk.h
+-rw-r--r--   0 runner    (1001) docker     (127)   166758 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/windows_winusb.c
+-rw-r--r--   0 runner    (1001) docker     (127)    23891 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/windows_winusb.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/strerror.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/sync.c
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/version.h
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb/version_nano.h
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/libusb-1.0.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.619052 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/Base.props
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/Configuration.Application.props
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/Configuration.Base.props
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/Configuration.DynamicLibrary.props
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/Configuration.StaticLibrary.props
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/ProjectConfigurations.Base.props
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/build_all.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/dpfp.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/dpfp_threaded.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/fxload.vcxproj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.619052 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/getopt/
+-rw-r--r--   0 runner    (1001) docker     (127)    30281 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/getopt/getopt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/getopt/getopt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/getopt/getopt1.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/getopt.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/hotplugtest.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)    17271 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/libusb.sln
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/libusb_dll.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/libusb_static.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/listdevs.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/sam3u_benchmark.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/stress.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/testlibusb.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/msvc/xusb.vcxproj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.619052 pyjoulescope_driver-1.5.2/third-party/libusb/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/tests/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/tests/libusb_testlib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/tests/stress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/tests/testlib.c
+-rw-r--r--   0 runner    (1001) docker     (127)    36048 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/libusb/tests/umockdev.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:58:40.619052 pyjoulescope_driver-1.5.2/third-party/tinyprintf/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/tinyprintf/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/tinyprintf/tinyprintf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/tinyprintf/tinyprintf.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-08 14:58:28.000000 pyjoulescope_driver-1.5.2/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new
```

### Comparing `pyjoulescope_driver-1.5.1/CHANGELOG.md` & `pyjoulescope_driver-1.5.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to the Joulescope driver.
 
 
+## 1.5.2
+
+2024 May 8
+
+* Added "capture" subcommand to jsdrv example executable.
+
+
 ## 1.5.1
 
 2024 Apr 27
 
 * Fixed JSDRV_DOWNSAMPLE_MODE_AVERAGE glitches due to C type conversion.
 * Fixed incorrect downsampling initialization.
```

### Comparing `pyjoulescope_driver-1.5.1/LICENSE.txt` & `pyjoulescope_driver-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/PKG-INFO` & `pyjoulescope_driver-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjoulescope_driver
-Version: 1.5.1
+Version: 1.5.2
 Summary: Joulescope™ driver
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_driver/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjoulescope_driver-1.5.1/README.md` & `pyjoulescope_driver-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/credits.html` & `pyjoulescope_driver-1.5.2/credits.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include/jsdrv/cmacro_inc.h` & `pyjoulescope_driver-1.5.2/include/jsdrv/cmacro_inc.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include/jsdrv/cstr.h` & `pyjoulescope_driver-1.5.2/include/jsdrv/cstr.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include/jsdrv/error_code.h` & `pyjoulescope_driver-1.5.2/include/jsdrv/error_code.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include/jsdrv/log.h` & `pyjoulescope_driver-1.5.2/include/jsdrv/log.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include/jsdrv/meta.h` & `pyjoulescope_driver-1.5.2/include/jsdrv/meta.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include/jsdrv/time.h` & `pyjoulescope_driver-1.5.2/include/jsdrv/time.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include/jsdrv/topic.h` & `pyjoulescope_driver-1.5.2/include/jsdrv/topic.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include/jsdrv/union.h` & `pyjoulescope_driver-1.5.2/include/jsdrv/union.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include/jsdrv/version.h` & `pyjoulescope_driver-1.5.2/include/jsdrv/version.h`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 #define JSDRV_VERSION_MINOR 5
 
 /**
  * @brief The Joulescope driver patch version.
  *
  * Changes in the patch version indicate bug fixes and improvements.
  */
-#define JSDRV_VERSION_PATCH 1
+#define JSDRV_VERSION_PATCH 2
 
 /**
  * \brief The maximum version string length.
  *
  * The actual length is 14 bytes (MMM.mmm.ppppp\\x00), but round up
  * to simplify packing.
  */
```

### Comparing `pyjoulescope_driver-1.5.1/include/jsdrv.h` & `pyjoulescope_driver-1.5.2/include/jsdrv.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/js220_api.h` & `pyjoulescope_driver-1.5.2/include_private/js220_api.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/assert.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/assert.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/backend.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/backend.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/buffer.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/buffer.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/buffer_signal.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/buffer_signal.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/cdef.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/cdef.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/dbc.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/dbc.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/device.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/device.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/devices.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/devices.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/downsample.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/downsample.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/event.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/event.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/frontend.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/frontend.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/js110_cal.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/js110_cal.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/js110_sample_processor.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/js110_sample_processor.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/js110_stats.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/js110_stats.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/js220_i128.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/js220_i128.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/js220_stats.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/js220_stats.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/json.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/json.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/list.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/list.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/log.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/log.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/msg_queue.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/msg_queue.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/mutex.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/mutex.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/platform.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/platform.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/pubsub.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/pubsub.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/sample_buffer_f32.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/sample_buffer_f32.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/statistics.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/statistics.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/thread.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/thread.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/time_map_filter.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/time_map_filter.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/usb_spec.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/usb_spec.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/include_private/jsdrv_prv/windows.h` & `pyjoulescope_driver-1.5.2/include_private/jsdrv_prv/windows.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/__init__.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/__main__.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/__main__.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/binding.c` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/binding.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
             "/home/runner/work/joulescope_driver/joulescope_driver/include",
             "/home/runner/work/joulescope_driver/joulescope_driver/include_private",
             "/home/runner/work/joulescope_driver/joulescope_driver/third-party/tinyprintf",
-            "/tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/core/include",
+            "/tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/core/include",
             "/home/runner/work/joulescope_driver/joulescope_driver/third-party/libusb/libusb",
             "/home/runner/work/joulescope_driver/joulescope_driver/third-party/libusb/include/linux"
         ],
         "libraries": [
             "pthread",
             "m",
             "udev"
@@ -1730,177 +1730,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1934,42 +1934,42 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_19pyjoulescope_driver_7binding_Driver;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -20638,261 +20638,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -20901,29 +20901,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -20934,15 +20934,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -20951,29 +20951,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -20984,15 +20984,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -21001,29 +21001,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -21034,15 +21034,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -21051,29 +21051,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -21084,15 +21084,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -21101,29 +21101,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -21134,217 +21134,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -21360,15 +21360,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -21376,68 +21376,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -21445,15 +21445,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -21468,15 +21468,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21492,15 +21492,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -21508,68 +21508,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -21577,15 +21577,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21600,15 +21600,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21624,15 +21624,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -21640,68 +21640,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -21709,15 +21709,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -21732,170 +21732,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -34210,26 +34210,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-uooqnf5t/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-o6pewurw/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
```

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/__init__.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/api_timeout.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/api_timeout.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/gpi.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/gpi.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/info.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/info.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/measure.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/measure.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/program.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/program.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/record.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/record.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/scan.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/scan.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/set_parameter.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/set_parameter.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/statistics.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/statistics.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/entry_points/threads.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/entry_points/threads.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/img_alpha.img` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/img_alpha.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/img_beta.img` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/img_beta.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/img_stable.img` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/img_stable.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/program.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/program.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/record.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/record.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/release.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/release.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_app/index.html` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_app/index.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_app/index.json` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_app/index.json`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_app/js220_ctrl_app_1_0_1.img` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_app/js220_ctrl_app_1_0_1.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_app/js220_ctrl_app_1_0_1_CHANGELOG.md` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_app/js220_ctrl_app_1_0_1_CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater1/index.html` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater1/index.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater1/index.json` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater1/index.json`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater1/js220_ctrl_updater1_1_0_1.img` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater1/js220_ctrl_updater1_1_0_1.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater1/js220_ctrl_updater1_1_0_1_CHANGELOG.md` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater1/js220_ctrl_updater1_1_0_1_CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater2/index.html` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater2/index.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater2/index.json` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater2/index.json`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater2/js220_ctrl_updater2_1_0_1.img` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater2/js220_ctrl_updater2_1_0_1.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/ctrl_updater2/js220_ctrl_updater2_1_0_1_CHANGELOG.md` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/ctrl_updater2/js220_ctrl_updater2_1_0_1_CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/index.html` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/index.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/index.json` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/index.json`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/sensor_fpga/index.html` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/sensor_fpga/index.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/sensor_fpga/index.json` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/sensor_fpga/index.json`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/sensor_fpga/js220_fpga_1_0_1.img` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/sensor_fpga/js220_fpga_1_0_1.img`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/release/sensor_fpga/js220_fpga_1_0_1_CHANGELOG.md` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/release/sensor_fpga/js220_fpga_1_0_1_CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/test_calibration_hash.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/test_calibration_hash.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/test_release.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/test_release.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/test/test_time64.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/test/test_time64.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/time64.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/time64.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver/version.py` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "1.5.1"
+__version__ = "1.5.2"
 
 __title__ = "pyjoulescope_driver"
 __description__ = 'Joulescope™ driver'
 __url__ = 'https://joulescope.readthedocs.io'
 __author__ = 'Jetperch LLC'
 __author_email__ = 'joulescope-dev@jetperch.com'
 __license__ = 'Apache 2.0'
```

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver.egg-info/PKG-INFO` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjoulescope_driver
-Version: 1.5.1
+Version: 1.5.2
 Summary: Joulescope™ driver
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_driver/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjoulescope_driver-1.5.1/pyjoulescope_driver.egg-info/SOURCES.txt` & `pyjoulescope_driver-1.5.2/pyjoulescope_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/pyproject.toml` & `pyjoulescope_driver-1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/setup.py` & `pyjoulescope_driver-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/CMakeLists.txt` & `pyjoulescope_driver-1.5.2/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/backend/libusb/backend.c` & `pyjoulescope_driver-1.5.2/src/backend/libusb/backend.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/backend/libusb/msg_queue.c` & `pyjoulescope_driver-1.5.2/src/backend/libusb/msg_queue.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/backend/posix.c` & `pyjoulescope_driver-1.5.2/src/backend/posix.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/backend/windows.c` & `pyjoulescope_driver-1.5.2/src/backend/windows.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/backend/winusb/backend.c` & `pyjoulescope_driver-1.5.2/src/backend/winusb/backend.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/backend/winusb/device_change_notifier.c` & `pyjoulescope_driver-1.5.2/src/backend/winusb/device_change_notifier.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/backend/winusb/device_change_notifier.h` & `pyjoulescope_driver-1.5.2/src/backend/winusb/device_change_notifier.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/backend/winusb/msg_queue.c` & `pyjoulescope_driver-1.5.2/src/backend/winusb/msg_queue.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/buffer.c` & `pyjoulescope_driver-1.5.2/src/buffer.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/buffer_signal.c` & `pyjoulescope_driver-1.5.2/src/buffer_signal.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/calibration_hash.c` & `pyjoulescope_driver-1.5.2/src/calibration_hash.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/cstr.c` & `pyjoulescope_driver-1.5.2/src/cstr.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/devices.c` & `pyjoulescope_driver-1.5.2/src/devices.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/downsample.c` & `pyjoulescope_driver-1.5.2/src/downsample.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/emu.c` & `pyjoulescope_driver-1.5.2/src/emu.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/emulated.c` & `pyjoulescope_driver-1.5.2/src/emulated.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/error_code.c` & `pyjoulescope_driver-1.5.2/src/error_code.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/js110_api.h` & `pyjoulescope_driver-1.5.2/src/js110_api.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/js110_cal.c` & `pyjoulescope_driver-1.5.2/src/js110_cal.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/js110_sample_processor.c` & `pyjoulescope_driver-1.5.2/src/js110_sample_processor.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/js110_stats.c` & `pyjoulescope_driver-1.5.2/src/js110_stats.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/js110_usb.c` & `pyjoulescope_driver-1.5.2/src/js110_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/js220_i128.c` & `pyjoulescope_driver-1.5.2/src/js220_i128.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/js220_params.c` & `pyjoulescope_driver-1.5.2/src/js220_params.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/js220_stats.c` & `pyjoulescope_driver-1.5.2/src/js220_stats.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/js220_usb.c` & `pyjoulescope_driver-1.5.2/src/js220_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/jsdrv.c` & `pyjoulescope_driver-1.5.2/src/jsdrv.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/json.c` & `pyjoulescope_driver-1.5.2/src/json.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/log.c` & `pyjoulescope_driver-1.5.2/src/log.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/meta.c` & `pyjoulescope_driver-1.5.2/src/meta.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/pubsub.c` & `pyjoulescope_driver-1.5.2/src/pubsub.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/sample_buffer_f32.c` & `pyjoulescope_driver-1.5.2/src/sample_buffer_f32.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/statistics.c` & `pyjoulescope_driver-1.5.2/src/statistics.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/time.c` & `pyjoulescope_driver-1.5.2/src/time.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/time_map_filter.c` & `pyjoulescope_driver-1.5.2/src/time_map_filter.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/topic.c` & `pyjoulescope_driver-1.5.2/src/topic.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/union.c` & `pyjoulescope_driver-1.5.2/src/union.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/src/version.c` & `pyjoulescope_driver-1.5.2/src/version.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/CMakeLists.txt` & `pyjoulescope_driver-1.5.2/third-party/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/.gitlab-ci.yml` & `pyjoulescope_driver-1.5.2/third-party/cmocka/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/.ycm_extra_conf.py` & `pyjoulescope_driver-1.5.2/third-party/cmocka/.ycm_extra_conf.py`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/5.patch` & `pyjoulescope_driver-1.5.2/third-party/cmocka/5.patch`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/CMakeLists.txt` & `pyjoulescope_driver-1.5.2/third-party/cmocka/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/CPackConfig.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/CPackConfig.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/CompilerChecks.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/CompilerChecks.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/ConfigureChecks.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/ConfigureChecks.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/INSTALL.md` & `pyjoulescope_driver-1.5.2/third-party/cmocka/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/README.md` & `pyjoulescope_driver-1.5.2/third-party/cmocka/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/AddCCompilerFlag.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/AddCMockaTest.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/CheckCCompilerFlagSSP.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/DefineCMakeDefaults.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/DefineCompilerFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/DefinePlatformDefaults.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/FindNSIS.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/FindNSIS.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Modules/MacroEnsureOutOfSourceBuild.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Toolchain-Debian-mips.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/cmake/Toolchain-cross-m32.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/cmake/Toolchain-cross-m32.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/config.h.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/coverity/coverity_assert_model.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/coverity/coverity_assert_model.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/doc/CMakeLists.txt` & `pyjoulescope_driver-1.5.2/third-party/cmocka/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/doc/index.html` & `pyjoulescope_driver-1.5.2/third-party/cmocka/doc/index.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/doc/mainpage.dox` & `pyjoulescope_driver-1.5.2/third-party/cmocka/doc/mainpage.dox`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/README.md` & `pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/header.html` & `pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/header.html`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/doc.svg` & `pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/doc.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/folderclosed.svg` & `pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/folderclosed.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/folderopen.svg` & `pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/folderopen.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/mag_glass.svg` & `pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/mag_glass.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg` & `pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/nav_edge_inter.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/nav_edge_left.svg` & `pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/nav_edge_left.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/nav_edge_right.svg` & `pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/nav_edge_right.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/img/splitbar_handle.svg` & `pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/img/splitbar_handle.svg`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/js/striped_bg.js` & `pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/js/striped_bg.js`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/doc/that_style/that_style.css` & `pyjoulescope_driver-1.5.2/third-party/cmocka/doc/that_style/that_style.css`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/CMakeLists.txt` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/allocate_module.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/allocate_module.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/allocate_module_test.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/allocate_module_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/assert_macro.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/assert_macro.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/assert_macro_test.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/assert_macro_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/assert_module.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/assert_module.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/assert_module.h` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/assert_module.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/assert_module_test.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/assert_module_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/calculator.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/calculator.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/calculator_test.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/calculator_test.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/database.h` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/database.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/chef_wrap/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/chef_wrap/chef.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/chef_wrap/chef.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/chef_wrap/chef.h` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/chef_wrap/chef.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/chef_wrap/waiter_test_wrap.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/uptime/CMakeLists.txt` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/uptime/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/uptime/README.md` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/uptime/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/uptime/proc_uptime.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/uptime/proc_uptime.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/uptime/proc_uptime.h` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/uptime/proc_uptime.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/uptime/test_uptime.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/uptime/test_uptime.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/example/mock/uptime/uptime.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/example/mock/uptime/uptime.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/include/cmocka.h` & `pyjoulescope_driver-1.5.2/third-party/cmocka/include/cmocka.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/include/cmocka_pbc.h` & `pyjoulescope_driver-1.5.2/third-party/cmocka/include/cmocka_pbc.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/include/cmocka_private.h` & `pyjoulescope_driver-1.5.2/third-party/cmocka/include/cmocka_private.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/src/CMakeLists.txt` & `pyjoulescope_driver-1.5.2/third-party/cmocka/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/src/cmocka.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/src/cmocka.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/src/cmocka.def` & `pyjoulescope_driver-1.5.2/third-party/cmocka/src/cmocka.def`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/CMakeLists.txt` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/cmocka_test.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/cmocka_test.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/ctest-default.cmake` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/ctest-default.cmake`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_alloc.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_alloc.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_assert_macros.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_assert_macros.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_assert_macros_fail.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_assert_macros_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_basics.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_basics.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_cmockery.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_cmockery.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_exception_handler.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_exception_handler.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_fixtures.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_fixtures.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_float_macros.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_float_macros.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_group_fixtures.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_group_fixtures.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_group_setup_assert.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_group_setup_assert.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_group_setup_fail.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_group_setup_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_groups.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_groups.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_ordering.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_ordering.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_ordering_fail.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_ordering_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_returns.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_returns.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_returns_fail.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_returns_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_setup_fail.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_setup_fail.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_skip.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_skip.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_skip_filter.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_skip_filter.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_strmatch.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_strmatch.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/cmocka/tests/test_wildcard.c` & `pyjoulescope_driver-1.5.2/third-party/cmocka/tests/test_wildcard.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/.github/cifuzz.yml` & `pyjoulescope_driver-1.5.2/third-party/libusb/.github/cifuzz.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/.github/workflows/linux.yml` & `pyjoulescope_driver-1.5.2/third-party/libusb/.github/workflows/linux.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/.github/workflows/macos.yml` & `pyjoulescope_driver-1.5.2/third-party/libusb/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/.gitignore` & `pyjoulescope_driver-1.5.2/third-party/libusb/.gitignore`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/.private/appveyor_build.sh` & `pyjoulescope_driver-1.5.2/third-party/libusb/.private/appveyor_build.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/.private/bm.sh` & `pyjoulescope_driver-1.5.2/third-party/libusb/.private/bm.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/.private/ci-build.sh` & `pyjoulescope_driver-1.5.2/third-party/libusb/.private/ci-build.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/.private/ci-container-build.sh` & `pyjoulescope_driver-1.5.2/third-party/libusb/.private/ci-container-build.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/.private/post-rewrite.sh` & `pyjoulescope_driver-1.5.2/third-party/libusb/.private/post-rewrite.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/.private/pre-commit.sh` & `pyjoulescope_driver-1.5.2/third-party/libusb/.private/pre-commit.sh`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/.private/wbs.txt` & `pyjoulescope_driver-1.5.2/third-party/libusb/.private/wbs.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/.travis.yml` & `pyjoulescope_driver-1.5.2/third-party/libusb/.travis.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/CMakeLists.txt` & `pyjoulescope_driver-1.5.2/third-party/libusb/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/INSTALL_WIN.txt` & `pyjoulescope_driver-1.5.2/third-party/libusb/INSTALL_WIN.txt`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/Makefile.am` & `pyjoulescope_driver-1.5.2/third-party/libusb/Makefile.am`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/README-FORK.md` & `pyjoulescope_driver-1.5.2/third-party/libusb/README-FORK.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/README.git` & `pyjoulescope_driver-1.5.2/third-party/libusb/README.git`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/README.md` & `pyjoulescope_driver-1.5.2/third-party/libusb/README.md`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/common.xcconfig` & `pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/common.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/config.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/debug.xcconfig` & `pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/debug.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/libusb.xcconfig` & `pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/libusb.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj` & `pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/libusb.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/libusb_debug.xcconfig` & `pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/libusb_debug.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/libusb_release.xcconfig` & `pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/libusb_release.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/Xcode/release.xcconfig` & `pyjoulescope_driver-1.5.2/third-party/libusb/Xcode/release.xcconfig`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/android/config.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/android/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/android/examples/unrooted_android.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/android/examples/unrooted_android.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/android/examples/unrooted_android.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/android/examples/unrooted_android.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/android/jni/Android.mk` & `pyjoulescope_driver-1.5.2/third-party/libusb/android/jni/Android.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/android/jni/Application.mk` & `pyjoulescope_driver-1.5.2/third-party/libusb/android/jni/Application.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/android/jni/examples.mk` & `pyjoulescope_driver-1.5.2/third-party/libusb/android/jni/examples.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/android/jni/libusb.mk` & `pyjoulescope_driver-1.5.2/third-party/libusb/android/jni/libusb.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/android/jni/tests.mk` & `pyjoulescope_driver-1.5.2/third-party/libusb/android/jni/tests.mk`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/appveyor.yml` & `pyjoulescope_driver-1.5.2/third-party/libusb/appveyor.yml`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/configure.ac` & `pyjoulescope_driver-1.5.2/third-party/libusb/configure.ac`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/doc/Makefile.in` & `pyjoulescope_driver-1.5.2/third-party/libusb/doc/Makefile.in`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/doc/doxygen.cfg.in` & `pyjoulescope_driver-1.5.2/third-party/libusb/doc/doxygen.cfg.in`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/doc/libusb.png` & `pyjoulescope_driver-1.5.2/third-party/libusb/doc/libusb.png`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/examples/dpfp.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/examples/dpfp.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/examples/ezusb.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/examples/ezusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/examples/ezusb.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/examples/ezusb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/examples/fxload.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/examples/fxload.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/examples/hotplugtest.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/examples/hotplugtest.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/examples/listdevs.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/examples/listdevs.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/examples/sam3u_benchmark.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/examples/sam3u_benchmark.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/examples/testlibusb.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/examples/testlibusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/examples/xusb.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/examples/xusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/include/linux/config.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/include/linux/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/include/macos/config.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/include/macos/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/Makefile.am` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/Makefile.am`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/Makefile.am.extra` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/Makefile.am.extra`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/core.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/core.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/descriptor.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/descriptor.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/hotplug.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/hotplug.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/io.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/io.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/libusb-1.0.def` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/libusb-1.0.def`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/libusb-1.0.rc` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/libusb-1.0.rc`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/libusb.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/libusb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/libusbi.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/libusbi.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/darwin_usb.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/darwin_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/darwin_usb.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/darwin_usb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/emscripten_webusb.cpp` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/emscripten_webusb.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/events_posix.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/events_posix.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/events_posix.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/events_posix.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/events_windows.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/events_windows.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/events_windows.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/events_windows.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/haiku_pollfs.cpp` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/haiku_pollfs.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/haiku_usb.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/haiku_usb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/haiku_usb_backend.cpp` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/haiku_usb_backend.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/haiku_usb_raw.cpp` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/haiku_usb_raw.cpp`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/haiku_usb_raw.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/haiku_usb_raw.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/linux_netlink.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/linux_netlink.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/linux_udev.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/linux_udev.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/linux_usbfs.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/linux_usbfs.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/linux_usbfs.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/linux_usbfs.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/netbsd_usb.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/netbsd_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/null_usb.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/null_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/openbsd_usb.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/openbsd_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/sunos_usb.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/sunos_usb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/sunos_usb.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/sunos_usb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/threads_posix.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/threads_posix.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/threads_posix.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/threads_posix.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/threads_windows.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/threads_windows.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/threads_windows.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/threads_windows.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/windows_common.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/windows_common.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/windows_common.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/windows_common.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/windows_usbdk.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/windows_usbdk.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/windows_usbdk.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/windows_usbdk.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/windows_winusb.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/windows_winusb.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/os/windows_winusb.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/os/windows_winusb.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/strerror.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/strerror.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/libusb/sync.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/libusb/sync.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/Base.props` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/Base.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/Configuration.Base.props` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/Configuration.Base.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/Configuration.DynamicLibrary.props` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/Configuration.DynamicLibrary.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/ProjectConfigurations.Base.props` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/ProjectConfigurations.Base.props`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/build_all.ps1` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/build_all.ps1`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/config.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/config.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/dpfp.vcxproj` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/dpfp.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/dpfp_threaded.vcxproj` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/dpfp_threaded.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/fxload.vcxproj` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/fxload.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/getopt/getopt.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/getopt/getopt.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/getopt/getopt.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/getopt/getopt.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/getopt/getopt1.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/getopt/getopt1.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/getopt.vcxproj` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/getopt.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/hotplugtest.vcxproj` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/hotplugtest.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/libusb.sln` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/libusb.sln`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/libusb_dll.vcxproj` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/libusb_dll.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/libusb_static.vcxproj` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/libusb_static.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/listdevs.vcxproj` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/listdevs.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/sam3u_benchmark.vcxproj` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/sam3u_benchmark.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/stress.vcxproj` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/stress.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/testlibusb.vcxproj` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/testlibusb.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/msvc/xusb.vcxproj` & `pyjoulescope_driver-1.5.2/third-party/libusb/msvc/xusb.vcxproj`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/tests/Makefile.am` & `pyjoulescope_driver-1.5.2/third-party/libusb/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/tests/libusb_testlib.h` & `pyjoulescope_driver-1.5.2/third-party/libusb/tests/libusb_testlib.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/tests/stress.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/tests/stress.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/tests/testlib.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/tests/testlib.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/libusb/tests/umockdev.c` & `pyjoulescope_driver-1.5.2/third-party/libusb/tests/umockdev.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/tinyprintf/tinyprintf.c` & `pyjoulescope_driver-1.5.2/third-party/tinyprintf/tinyprintf.c`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/tinyprintf/tinyprintf.h` & `pyjoulescope_driver-1.5.2/third-party/tinyprintf/tinyprintf.h`

 * *Files identical despite different names*

### Comparing `pyjoulescope_driver-1.5.1/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new` & `pyjoulescope_driver-1.5.2/third-party/tinyprintf/tinyprintf_LICENSE.BSD-new`

 * *Files identical despite different names*

