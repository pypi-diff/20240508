# Comparing `tmp/naludaq-0.26.3.tar.gz` & `tmp/naludaq-0.26.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naludaq-0.26.3.tar", last modified: Mon Apr 22 17:33:27 2024, max compression
+gzip compressed data, was "naludaq-0.26.4.tar", last modified: Wed May  8 00:39:57 2024, max compression
```

## Comparing `naludaq-0.26.3.tar` & `naludaq-0.26.4.tar`

### file list

```diff
@@ -1,266 +1,266 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.409141 naludaq-0.26.3/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-22 17:33:14.000000 naludaq-0.26.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-04-22 17:33:27.409141 naludaq-0.26.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14876 2024-04-22 17:33:14.000000 naludaq-0.26.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-22 17:33:14.000000 naludaq-0.26.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 17:33:27.409141 naludaq-0.26.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-22 17:33:14.000000 naludaq-0.26.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.357141 naludaq-0.26.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.365141 naludaq-0.26.3/src/naludaq/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.365141 naludaq-0.26.3/src/naludaq/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/backend/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/backend/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/backend/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.365141 naludaq-0.26.3/src/naludaq/backend/managers/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/backend/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/backend/managers/acquisitions.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/backend/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/backend/managers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/backend/managers/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/backend/managers/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.365141 naludaq-0.26.3/src/naludaq/backend/models/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/backend/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39569 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/backend/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/backend/models/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.369141 naludaq-0.26.3/src/naludaq/board/
--rw-r--r--   0 runner    (1001) docker     (127)    30544 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24036 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/board_inits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.369141 naludaq-0.26.3/src/naludaq/board/connections/
--rw-r--r--   0 runner    (1001) docker     (127)    19599 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/connections/_FTDI.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/connections/_MockUART.py
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/connections/_UART.py
--rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/connections/_USB.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/connections/base_ethernet.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/connections/base_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/connections/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/connections/tcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/connections/udp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.373141 naludaq-0.26.3/src/naludaq/board/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/initializers/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/initializers/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/initializers/asocv3s.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/initializers/init_aodsv2_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/initializers/init_hdsocv1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/initializers/init_udc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/initializers/init_upac96.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/initializers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17749 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/board/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.373141 naludaq-0.26.3/src/naludaq/communication/
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/communication/_chip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/communication/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/communication/_fpga.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/communication/analog_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/communication/chip_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/communication/control_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/communication/digital_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/communication/i2c.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/communication/i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20416 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/communication/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.373141 naludaq-0.26.3/src/naludaq/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/analog_debug_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.377141 naludaq-0.26.3/src/naludaq/controllers/biasing_mode/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/biasing_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/biasing_mode/udc16.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.377141 naludaq-0.26.3/src/naludaq/controllers/board/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/board/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/board/asocv3s.py
--rw-r--r--   0 runner    (1001) docker     (127)    15507 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/board/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/board/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/board/oleas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/board/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/board/udc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/board/upac.py
--rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/board/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.377141 naludaq-0.26.3/src/naludaq/controllers/connection/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21101 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/connection/connection_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/connection/upac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/connection/upac96.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.381141 naludaq-0.26.3/src/naludaq/controllers/external_dac/
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/external_dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/external_dac/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/external_dac/ad5671.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/external_dac/ad5675.py
--rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/external_dac/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/external_dac/dac7578.py
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/external_dac/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/external_dac/i2c_dac.py
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/external_dac/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/external_dac/upac32.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.381141 naludaq-0.26.3/src/naludaq/controllers/gainstages/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/gainstages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/gainstages/aodsv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/gainstages/oddsock_aods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.381141 naludaq-0.26.3/src/naludaq/controllers/peripherals/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/peripherals/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/peripherals/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/peripherals/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/peripherals/peripherals_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/peripherals/upac.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/peripherals/upac96.py
--rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/project_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.385141 naludaq-0.26.3/src/naludaq/controllers/readout/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/readout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/readout/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/readout/asocv3.py
--rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/readout/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/readout/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/readout/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/si5341_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.385141 naludaq-0.26.3/src/naludaq/controllers/tia/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/tia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/tia/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/tia/hdsoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.385141 naludaq-0.26.3/src/naludaq/controllers/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/trigger/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/trigger/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/trigger/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/trigger/siread.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/trigger/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/trigger/upac.py
--rw-r--r--   0 runner    (1001) docker     (127)    16581 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/controllers/trigger/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.385141 naludaq-0.26.3/src/naludaq/daq/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/daq/debugdaq.py
--rw-r--r--   0 runner    (1001) docker     (127)    20482 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/daq/lightdaq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/daq/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.389141 naludaq-0.26.3/src/naludaq/daq/workers/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/daq/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/daq/workers/answer_parser_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/daq/workers/csv_storage_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.389141 naludaq-0.26.3/src/naludaq/daq/workers/packager/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/daq/workers/packager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/daq/workers/packager/worker_packager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/daq/workers/packager/worker_packager_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/daq/workers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/daq/workers/worker_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/daq/workers/worker_serial_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/daq/workers/worker_usb_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.389141 naludaq-0.26.3/src/naludaq/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/devices/eeprom.py
--rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/devices/i2c_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/devices/ltc2990.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.393141 naludaq-0.26.3/src/naludaq/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/helpers/fancyiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/helpers/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/helpers/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/helpers/register_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/helpers/semiton.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/helpers/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.393141 naludaq-0.26.3/src/naludaq/io/
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22338 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/io/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    35939 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/io/io_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.393141 naludaq-0.26.3/src/naludaq/models/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/models/acq_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/naludaq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.397141 naludaq-0.26.3/src/naludaq/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/aardvarcv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/answer_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/aodsoc_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/asocv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/asocv3s_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/hdsoc_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.397141 naludaq-0.26.3/src/naludaq/parsers/headers/
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/headers/asoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/headers/asocv2.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/headers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/headers/siread.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/headers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/headers/upac32.py
--rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/trbhm_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/udc_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/upac96_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/parsers/upac_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.397141 naludaq-0.26.3/src/naludaq/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.401142 naludaq-0.26.3/src/naludaq/tools/adc2mv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/adc2mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/adc2mv/adc_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14397 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/adc2mv/adc_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/adc2mv/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/adc2mv/pre_adc2mv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/autoaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.401142 naludaq-0.26.3/src/naludaq/tools/autotrigger/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/autotrigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/autotrigger/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/board_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.401142 naludaq-0.26.3/src/naludaq/tools/dac_sweep/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/dac_sweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.401142 naludaq-0.26.3/src/naludaq/tools/data_collector/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/data_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/data_collector/_daq_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    16831 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/data_collector/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/data_collector/udc16.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/ft60x.py
--rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/ftdi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.401142 naludaq-0.26.3/src/naludaq/tools/lookup_table/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/lookup_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/lookup_table/lookup_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/lookup_table/lookup_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.401142 naludaq-0.26.3/src/naludaq/tools/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/optimizers/bayesian_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.401142 naludaq-0.26.3/src/naludaq/tools/optimizers/conversion_ramp/
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/optimizers/conversion_ramp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22275 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/optimizers/conversion_ramp/udc16.py
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/optimizers/gainstagetuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.405141 naludaq-0.26.3/src/naludaq/tools/pedestals/
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/pedestals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.405141 naludaq-0.26.3/src/naludaq/tools/pedestals/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/pedestals/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/pedestals/generators/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/pedestals/generators/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/pedestals/generators/udc16.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/pedestals/generators/upac96.py
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/pedestals/pedestals_correcter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/pedestals/pedestals_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.405141 naludaq-0.26.3/src/naludaq/tools/threshold_scan/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/threshold_scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/threshold_scan/threshold_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/threshold_scan/upac96_thresholdscan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.405141 naludaq-0.26.3/src/naludaq/tools/timing_cal/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/timing_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/timing_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/timing_cal/correcter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.405141 naludaq-0.26.3/src/naludaq/tools/waiter/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/waiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-22 17:33:14.000000 naludaq-0.26.3/src/naludaq/tools/waiter/eventwaiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.405141 naludaq-0.26.3/src/naludaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-04-22 17:33:27.000000 naludaq-0.26.3/src/naludaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-04-22 17:33:27.000000 naludaq-0.26.3/src/naludaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 17:33:27.000000 naludaq-0.26.3/src/naludaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-22 17:33:27.000000 naludaq-0.26.3/src/naludaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 17:33:27.000000 naludaq-0.26.3/src/naludaq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:33:27.405141 naludaq-0.26.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-22 17:33:14.000000 naludaq-0.26.3/tests/test_naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.046204 naludaq-0.26.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-08 00:39:45.000000 naludaq-0.26.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-05-08 00:39:57.046204 naludaq-0.26.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14876 2024-05-08 00:39:45.000000 naludaq-0.26.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-08 00:39:45.000000 naludaq-0.26.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:39:57.046204 naludaq-0.26.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-08 00:39:45.000000 naludaq-0.26.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:56.994203 naludaq-0.26.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.002203 naludaq-0.26.4/src/naludaq/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.006203 naludaq-0.26.4/src/naludaq/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/backend/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/backend/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/backend/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.006203 naludaq-0.26.4/src/naludaq/backend/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/backend/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/backend/managers/acquisitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/backend/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/backend/managers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/backend/managers/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/backend/managers/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.006203 naludaq-0.26.4/src/naludaq/backend/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/backend/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39569 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/backend/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/backend/models/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.006203 naludaq-0.26.4/src/naludaq/board/
+-rw-r--r--   0 runner    (1001) docker     (127)    31381 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24036 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/board_inits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.010203 naludaq-0.26.4/src/naludaq/board/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)    20239 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/connections/_FTDI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/connections/_MockUART.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/connections/_UART.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/connections/_USB.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/connections/base_ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/connections/base_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/connections/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/connections/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/connections/udp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.010203 naludaq-0.26.4/src/naludaq/board/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/initializers/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/initializers/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/initializers/asocv3s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/initializers/init_aodsv2_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/initializers/init_hdsocv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/initializers/init_udc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/initializers/init_upac96.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/initializers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17749 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/board/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.014203 naludaq-0.26.4/src/naludaq/communication/
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/communication/_chip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/communication/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/communication/_fpga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/communication/analog_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/communication/chip_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/communication/control_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/communication/digital_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/communication/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/communication/i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20416 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/communication/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.014203 naludaq-0.26.4/src/naludaq/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/analog_debug_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.014203 naludaq-0.26.4/src/naludaq/controllers/biasing_mode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/biasing_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/biasing_mode/udc16.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.014203 naludaq-0.26.4/src/naludaq/controllers/board/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/board/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/board/asocv3s.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15507 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/board/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/board/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/board/oleas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/board/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/board/udc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/board/upac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/board/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.018203 naludaq-0.26.4/src/naludaq/controllers/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22085 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/connection/connection_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/connection/upac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/connection/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.018203 naludaq-0.26.4/src/naludaq/controllers/external_dac/
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/external_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/external_dac/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/external_dac/ad5671.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/external_dac/ad5675.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/external_dac/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/external_dac/dac7578.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/external_dac/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/external_dac/i2c_dac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/external_dac/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/external_dac/upac32.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.018203 naludaq-0.26.4/src/naludaq/controllers/gainstages/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/gainstages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/gainstages/aodsv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/gainstages/oddsock_aods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.022204 naludaq-0.26.4/src/naludaq/controllers/peripherals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/peripherals/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/peripherals/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/peripherals/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/peripherals/peripherals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/peripherals/upac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/peripherals/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/project_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.022204 naludaq-0.26.4/src/naludaq/controllers/readout/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/readout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/readout/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/readout/asocv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/readout/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/readout/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/readout/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/si5341_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.022204 naludaq-0.26.4/src/naludaq/controllers/tia/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/tia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/tia/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/tia/hdsoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.022204 naludaq-0.26.4/src/naludaq/controllers/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/trigger/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/trigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/trigger/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/trigger/siread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/trigger/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/trigger/upac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16581 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/controllers/trigger/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.026203 naludaq-0.26.4/src/naludaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/daq/debugdaq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20482 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/daq/lightdaq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/daq/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.026203 naludaq-0.26.4/src/naludaq/daq/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/daq/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/daq/workers/answer_parser_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/daq/workers/csv_storage_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.026203 naludaq-0.26.4/src/naludaq/daq/workers/packager/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/daq/workers/packager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/daq/workers/packager/worker_packager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/daq/workers/packager/worker_packager_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/daq/workers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/daq/workers/worker_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/daq/workers/worker_serial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/daq/workers/worker_usb_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.026203 naludaq-0.26.4/src/naludaq/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/devices/eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/devices/i2c_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/devices/ltc2990.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.030203 naludaq-0.26.4/src/naludaq/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/helpers/fancyiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/helpers/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/helpers/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/helpers/register_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/helpers/semiton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/helpers/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.030203 naludaq-0.26.4/src/naludaq/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22338 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/io/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35939 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/io/io_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.030203 naludaq-0.26.4/src/naludaq/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/models/acq_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.034204 naludaq-0.26.4/src/naludaq/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/aardvarcv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/answer_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/aodsoc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/asocv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/asocv3s_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/hdsoc_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.034204 naludaq-0.26.4/src/naludaq/parsers/headers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/headers/asoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/headers/asocv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/headers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/headers/siread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/headers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/headers/upac32.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/trbhm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/udc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/upac96_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/parsers/upac_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.034204 naludaq-0.26.4/src/naludaq/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.038204 naludaq-0.26.4/src/naludaq/tools/adc2mv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/adc2mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/adc2mv/adc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14397 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/adc2mv/adc_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/adc2mv/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/adc2mv/pre_adc2mv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/autoaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.038204 naludaq-0.26.4/src/naludaq/tools/autotrigger/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/autotrigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/autotrigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/board_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.038204 naludaq-0.26.4/src/naludaq/tools/dac_sweep/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/dac_sweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.038204 naludaq-0.26.4/src/naludaq/tools/data_collector/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/data_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/data_collector/_daq_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16831 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/data_collector/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/data_collector/udc16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/ft60x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/ftdi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.038204 naludaq-0.26.4/src/naludaq/tools/lookup_table/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/lookup_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/lookup_table/lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/lookup_table/lookup_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.038204 naludaq-0.26.4/src/naludaq/tools/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/optimizers/bayesian_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.038204 naludaq-0.26.4/src/naludaq/tools/optimizers/conversion_ramp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/optimizers/conversion_ramp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22275 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/optimizers/conversion_ramp/udc16.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/optimizers/gainstagetuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.042204 naludaq-0.26.4/src/naludaq/tools/pedestals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/pedestals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.042204 naludaq-0.26.4/src/naludaq/tools/pedestals/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/pedestals/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/pedestals/generators/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/pedestals/generators/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/pedestals/generators/udc16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/pedestals/generators/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/pedestals/pedestals_correcter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/pedestals/pedestals_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.042204 naludaq-0.26.4/src/naludaq/tools/threshold_scan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/threshold_scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/threshold_scan/threshold_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/threshold_scan/upac96_thresholdscan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.042204 naludaq-0.26.4/src/naludaq/tools/timing_cal/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/timing_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/timing_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/timing_cal/correcter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.042204 naludaq-0.26.4/src/naludaq/tools/waiter/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/waiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-08 00:39:45.000000 naludaq-0.26.4/src/naludaq/tools/waiter/eventwaiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.046204 naludaq-0.26.4/src/naludaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-05-08 00:39:56.000000 naludaq-0.26.4/src/naludaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-05-08 00:39:56.000000 naludaq-0.26.4/src/naludaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:39:56.000000 naludaq-0.26.4/src/naludaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-08 00:39:56.000000 naludaq-0.26.4/src/naludaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 00:39:56.000000 naludaq-0.26.4/src/naludaq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:39:57.042204 naludaq-0.26.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-08 00:39:46.000000 naludaq-0.26.4/tests/test_naludaq.py
```

### Comparing `naludaq-0.26.3/LICENSE.txt` & `naludaq-0.26.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/PKG-INFO` & `naludaq-0.26.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.26.3
+Version: 0.26.4
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naludaq-0.26.3/README.md` & `naludaq-0.26.4/README.md`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/pyproject.toml` & `naludaq-0.26.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/setup.py` & `naludaq-0.26.4/setup.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/backend/__init__.py` & `naludaq-0.26.4/src/naludaq/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/backend/client.py` & `naludaq-0.26.4/src/naludaq/backend/client.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/backend/context.py` & `naludaq-0.26.4/src/naludaq/backend/context.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/backend/exceptions.py` & `naludaq-0.26.4/src/naludaq/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/backend/managers/acquisitions.py` & `naludaq-0.26.4/src/naludaq/backend/managers/acquisitions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/backend/managers/config.py` & `naludaq-0.26.4/src/naludaq/backend/managers/config.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/backend/managers/connection.py` & `naludaq-0.26.4/src/naludaq/backend/managers/connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/backend/managers/io.py` & `naludaq-0.26.4/src/naludaq/backend/managers/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,15 +80,16 @@
 
         Args:
             command (str | bytes): read command to send.
 
         Returns:
             bytes: the response.
         """
-        return self.read_all([command])[0]
+        response = self.read_all([command])[0]
+        return response
 
     def read_all(self, commands: "list[str | bytes]") -> list[bytes]:
         """Sends several read commands to the board and retrieves the responses.
 
         Args:
             commands (list[str | bytes]): commands to send
```

### Comparing `naludaq-0.26.3/src/naludaq/backend/models/acquisition.py` & `naludaq-0.26.4/src/naludaq/backend/models/acquisition.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/backend/models/device.py` & `naludaq-0.26.4/src/naludaq/backend/models/device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/__init__.py` & `naludaq-0.26.4/src/naludaq/board/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -490,14 +490,36 @@
         except ConnectionError as error_msg:
             self.connection = None
             raise ConnectionError("No connection established due to: %s", error_msg)
         else:
             self._context = None
             self._using_new_backend = False
             get_connection_controller(self).configure_connection()
+    
+    def get_udp_connection(self, board_addr: tuple, receiver_addr: tuple):
+        """Open a UDP connection."""
+        self.connection_info = {
+            "type": "udp",
+            "model": self.model,
+            "stop_word": self.params["stop_word"],
+            "board_addr": board_addr,
+            "receiver_addr": receiver_addr,
+            "speed": int(200e6),  # gigabit!
+        }
+
+        try:
+            self.connection = get_connection(self.connection_info)
+            self.connection.open()
+        except ConnectionError as error_msg:
+            self.connection = None
+            raise ConnectionError("No connection established due to: %s", error_msg)
+        else:
+            self._context = None
+            self._using_new_backend = False
+            get_connection_controller(self).configure_connection()
 
     def get_mock_uart_connection(self, user_port, board_port, ip="127.0.0.1"):
         """Connect to a mock board.
 
         Args:
             user_port (tuple): the port of the user
             board_port (tuple): the port of the board
```

### Comparing `naludaq-0.26.3/src/naludaq/board/board_inits.py` & `naludaq-0.26.4/src/naludaq/board/board_inits.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/connections/_FTDI.py` & `naludaq-0.26.4/src/naludaq/board/connections/_FTDI.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Marcus Luck - Nalu Scientific
 email: marcus@naluscientific.com
 January 2022
 """
 import binascii
 import logging
 import time
+from typing import Optional
 
 try:
     import ftd2xx as ftd
     import ftd2xx.defines as ftd_defines
 except (FileNotFoundError, OSError):
     raise FileNotFoundError("FTDI driver not installed")
 except ImportError:
@@ -25,14 +26,16 @@
 from naludaq.helpers import validations
 from naludaq.helpers.exceptions import FTDIError
 from naludaq.parsers.answer_parser import get_answer_parser
 from naludaq.tools.ftdi import index_from_comport, index_from_serial, list_ftdi_devices
 
 logger = logging.getLogger("naludaq.FTDI")
 
+_WRITE_MESSAGE_NIBBLES = 8
+
 
 class FTDI(BaseSerialConnection):
     """FTDI is a communications class for talking to the boards.
 
     Uses the ftd2xx Python package, which requires d2xx drivers
     to be properly installed. For information about using d2xx:
     https://ftdichip.com/wp-content/uploads/2020/08/D2XX_Programmers_GuideFT_000071.pdf
@@ -59,14 +62,16 @@
         self._serial_number: str = None
         self._dev_word_len = ftd_defines.BITS_8
         self._dev_stop_bits = ftd_defines.STOP_BITS_1
         self._dev_parity = ftd_defines.PARITY_NONE
         self._rx_timeout = 100  # ms
         self._tx_timeout = 100  # ms
         self._rtscts = False
+        self.tx_pause = 0.0
+        self.bundle_mode = False
 
         self._baud = conn_info["speed"]
         self._model = conn_info["model"]
         self.stopword = conn_info.get("stop_word", b"\xca\xfe")  # b'\xfa\xce'
         self.new_firmware = conn_info.get("new_firmware", False)
         self.response_length = 4
         self.parse_answer = get_answer_parser()
@@ -261,39 +266,52 @@
             try:
                 self.ser.close()
             except Exception as e:
                 logger.debug("Failed to close connection due to: %s", e)
             self.ser = None
         self._is_open = False
 
-    def send(self, data, pause=0.02):
+    def send(self, data, pause: Optional[float] = None, bundle: Optional[bool] = None):
         """Converts the string to a series of bytes to send in the correct format
 
         Input:
             data (hex): A hex type string (interface needs 32 bits, so 8 hex chars minimum)
             pause (float): How logn to wait in between send.
         """
+        if bundle is None:
+            bundle = self.bundle_mode
+        if pause is None:
+            pause = self.tx_pause
+
         if len(data) % 8 != 0:
             logger.debug(
                 "FTDI.send(): need multiples of 8 hex chars, you gave me %s", len(data)
             )
             logger.debug("command:%s", data)
             return
 
+        logger.debug("Sending: %s in %s mode", data, "bundle" if bundle else "single")
+        if (len(data) > _WRITE_MESSAGE_NIBBLES) and bundle is False:
+            for i in range(0, len(data), _WRITE_MESSAGE_NIBBLES):
+                self._send(data[i : i + _WRITE_MESSAGE_NIBBLES], pause)
+        else:
+            self._send(data, pause)
+
+    def _send(self, data, pause):
         try:
             tosend = binascii.a2b_hex(data)
         except binascii.Error as e:
             logger.error(f"FTDI.send(): could not convert hex data: {e}")
             return
 
-        logger.debug("Sending: %s", data)
         try:
             self.ser.write(tosend)
         except AttributeError as error_msg:
             logger.error("Can't send command to board, no connection available.")
+        time.sleep(pause)
 
     def read_until(self, stopword: bytes):
         """Pulls data from the connection until a set of characters is found.
 
         Args:
             stopword (bytes): the sequence of characters that indicate
                 when to stop reading.
@@ -377,18 +395,18 @@
                 continue
 
         logger.debug("Couldn't sync")
         return False
 
     def reset_input_buffer(self, iterations: int = 100):
         """Discards any data currently in the boards output buffer.
-        
+
         This will empty both the computer input buffer and the hardware
         output buffer.
-        
+
         However, this will only run 100 times at the most which is ~400kb.
 
         Args:
             iterations (int): maximum number of times to purge the buffer.
                 A cap is necessary since the board may be sending data faster
                 than it can be purged.
         """
```

### Comparing `naludaq-0.26.3/src/naludaq/board/connections/_MockUART.py` & `naludaq-0.26.4/src/naludaq/board/connections/_MockUART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/connections/_UART.py` & `naludaq-0.26.4/src/naludaq/board/connections/_UART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/connections/_USB.py` & `naludaq-0.26.4/src/naludaq/board/connections/_USB.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/connections/base_connection.py` & `naludaq-0.26.4/src/naludaq/board/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/connections/connection_factory.py` & `naludaq-0.26.4/src/naludaq/board/connections/connection_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 Creates and returns a connection of the specified type.
 """
 from logging import getLogger
 
 from ._MockUART import MockUART
 from ._UART import UART
 from .tcp import TCP
+from .udp import UDP
 
 LOGGER = getLogger(__name__)
 
 # This list gets updated based on whether or not certain
 # connection types are actually available
 VALID_CONNECTION_TYPES = [
     "ftdi",
     "tcp",
+    "udp",
     "uart",
     "ft60x",
     "none",
 ]
 try:
     from ._FTDI import FTDI
 except (ImportError, FileNotFoundError) as e:
@@ -52,14 +54,16 @@
         ConnectionError if connection can't be created.
     """
     conn_type = _get_connection_type_or_raise(conn_info)
     connection = None
     try:
         if conn_type == "tcp":
             connection = _set_tcp_connection(conn_info)
+        elif conn_type == "udp":
+            connection = _set_udp_connection(conn_info)
         elif conn_type == "uart":
             connection = _set_uart_connection(conn_info=conn_info)
         elif conn_type == "ftdi":
             connection = _set_ftdi_connection(conn_info=conn_info)
         elif conn_type == "ft60x":
             connection = _set_ft60x_connection(conn_info=conn_info)
     except (ConnectionError, Exception) as error_msg:
@@ -169,14 +173,39 @@
         connection = TCP(ip, port, stop_word)
         connection.open()
     except ConnectionError:
         raise
     return connection
 
 
+def _set_udp_connection(conn_info):
+    """Connect to over UDP socket.
+
+    sets self.connection to the UDP connection.
+
+    Args:
+        conn_info (dict): containing the connection params for the UDP connection obj.
+
+    Returns:
+        An open UDP connection
+    """
+    try:
+        conn_info["stop_word"]
+    except KeyError as e:
+        raise ValueError(f"Connection is missing required parameter 'stop_word'")
+
+    connection = None
+    try:
+        connection = UDP(conn_info)
+        connection.open()
+    except ConnectionError:
+        raise
+    return connection
+
+
 def _get_connection_type_or_raise(conn_info: dict):
     conn_type = conn_info.get("type", None)
     if conn_type is None:
         raise AttributeError('Connection info missing "type" key')
     if not isinstance(conn_type, str):
         raise TypeError("Connection type must be a string")
     conn_type = conn_type.lower()
```

### Comparing `naludaq-0.26.3/src/naludaq/board/connections/tcp.py` & `naludaq-0.26.4/src/naludaq/board/connections/tcp.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/connections/udp.py` & `naludaq-0.26.4/src/naludaq/board/connections/udp.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,109 +1,88 @@
 import binascii
 import logging
 import select
 import socket
 import time
+from typing import Optional
 
 import numpy as np
 
 from naludaq.board.connections.base_connection import BaseConnection
 from naludaq.parsers.answer_parser import get_answer_parser
 
 logger = logging.getLogger(__name__)
 
+_UDP_READ_BUFFER_SIZE = 1500
+_UDP_HEADER_BYTES = 16
+_WRITE_MESSAGE_NIBBLES = 8
+_DEFAULT_TIMEOUT = 0.005
+
 
 class UDP(BaseConnection):
     def __init__(self, connection_info: dict):
         """Class for communication over an ethernet connection.
 
         Args:
             connection_info (dict): the connection configuration
         """
         super().__init__()
 
         # Store connection info
-        user_ip = connection_info["user_ip"]
-        board_ip = connection_info["board_ip"]
-        command_port = connection_info["command_port"]
-        readout_port = connection_info["readout_port"]
-        self._user_command_addr = (user_ip, command_port)
-        self._user_readout_addr = (user_ip, readout_port)
-        self._board_command_addr = (board_ip, command_port)
-        self._board_readout_addr = (board_ip, readout_port)
+        self._receiver_addr = connection_info["receiver_addr"]
+        self._board_addr = connection_info["board_addr"]
 
         self._model = connection_info["model"]
-        self.stopword = connection_info["stop_word"]
-
+        self.stop_word = connection_info["stop_word"]
+        self._timeout = _DEFAULT_TIMEOUT
         self.read_addr = "AD"
         self.write_addr = "AF"
         self.response_length = 8
         self.parse_answer = get_answer_parser(True)
 
+        self.tx_pause = 0.01
+        self.bundle_mode = True
+
+        self._rx_fifo = bytearray()
+
         self.socket: socket.socket = None
 
     @property
-    def user_command_addr(self) -> tuple:
+    def receiver_addr(self) -> tuple:
         """Get/set the user command address.
 
         Setting the address will close and reopen the connection
         if the connection is already open
 
         Args:
             addr (tuple): the address
         """
-        return self._user_command_addr
+        return self._receiver_addr
 
-    @user_command_addr.setter
-    def user_command_addr(self, addr: tuple):
-        self._user_command_addr = addr
+    @receiver_addr.setter
+    def receiver_addr(self, addr: tuple):
+        self._receiver_addr = addr
 
         # Reopen the socket
         if self.socket:
             self.close()
             self.open()
 
     @property
-    def user_readout_addr(self) -> tuple:
-        """Get/set the user readout address.
-
-        Args:
-            addr (tuple): the address
-        """
-        return self._user_readout_addr
-
-    @user_readout_addr.setter
-    def user_readout_addr(self, addr: tuple):
-        self._user_readout_addr = addr
-
-    @property
-    def board_command_addr(self) -> tuple:
+    def board_addr(self) -> tuple:
         """Get/set the board command address.
 
         Args:
             addr (tuple): the address
         """
-        return self._board_command_addr
-
-    @board_command_addr.setter
-    def board_command_addr(self, addr: tuple):
-        self._board_command_addr = addr
-
-    @property
-    def board_readout_addr(self) -> tuple:
-        """Get/set the board readout address.
-
-        Args:
-            addr (tuple): the address
-        """
-        return self._board_readout_addr
+        return self._board_addr
 
-    @board_readout_addr.setter
-    def board_readout_addr(self, addr: tuple):
-        self._board_readout_addr = addr
+    @board_addr.setter
+    def board_addr(self, addr: tuple):
+        self._board_addr = addr
 
     @property
     def is_open(self) -> bool:
         """Indicates whether the connection is open."""
         return self.socket is not None
 
     def set_answer_parser(self, new_firmware: bool = True):
@@ -129,85 +108,138 @@
     def __del__(self):
         self.close()
 
     def open(self):
         """Opens the connection."""
         if not self.socket:
             self.socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-            self.socket.setblocking(False)
-            self.socket.bind(self._user_command_addr)
+            self.socket.bind(self._receiver_addr)
+            # self.socket.setblocking(False)
+            self.socket.settimeout(self._timeout)
 
     def close(self):
         """Closes the connection."""
         try:
             self.socket.close()
             self.socket = None
         except:
             pass
 
-    def send(self, data: str, pause: float = 0.02):
+    def send(
+        self, data: str, pause: Optional[float] = None, bundle: Optional[bool] = None
+    ):
         """Sends a string of hex characters.
 
         Args:
             data (str): the data string. Only hex characters are allowed!
             pause (float): the time in seconds to wait after sending
         """
-        num_chars = len(data)
-
+        if bundle is None:
+            bundle = self.bundle_mode
+        if pause is None:
+            pause = self.tx_pause
         # Make sure the length of the input is a multiple of 8
-        if num_chars % 8 != 0:
+        if len(data) % 8 != 0:
             logger.debug(
-                "UDP.send(): need multiples of 8 hex chars, you gave me %s", num_chars
+                "UDP.send(): need multiples of 8 hex chars, you gave me %s", len(data)
             )
             logger.debug("command:%s", data)
             return
 
+        logger.debug("Sending: %s in %s mode", data, "bundle" if bundle else "single")
+        if (len(data) > _WRITE_MESSAGE_NIBBLES) and bundle is False:
+            for i in range(0, len(data), _WRITE_MESSAGE_NIBBLES):
+                self._send(data[i : i + _WRITE_MESSAGE_NIBBLES], pause)
+        else:
+            self._send(data, pause)
+
+    def _send(self, data: str, pause: float):
         # Convert hex data string to binary
         # data_binary = binascii.unhexlify(self.sync_word + data)
         data_binary = binascii.unhexlify(data)
 
         # Send the data over the socket
-        self.socket.sendto(data_binary, self._board_command_addr)
+        self.socket.sendto(data_binary, self._board_addr)
         time.sleep(pause)
 
     @property
     def in_waiting(self) -> bool:
         """Checks data is waiting in the socket buffer."""
         data_in_socket, _, _ = select.select([self.socket], [], [], 0)
         return len(data_in_socket) != 0
 
+    def read(self, amount: int) -> bytes:
+        """Reads bytes, discards first 16 bytes (UDP Header)"""
+        # With datagrams, the min amount to read is 16 (header) + 8 (data) = 24
+        # But we have to set the buffer to the largest datagram we can receive
+        buf_size = max(amount, _UDP_READ_BUFFER_SIZE)
+        try:
+            data = self.socket.recv(buf_size)
+        except Exception as e:
+            return b""
+        if len(data) < _UDP_HEADER_BYTES:
+            return b""
+        return data[_UDP_HEADER_BYTES:]
+
+    def read_until(self, stopword: bytes):
+        """Pulls data from the connection until a set of characters is found.
+
+        Args:
+            stopword (bytes): the sequence of characters that indicate
+                when to stop reading.
+
+        Returns:
+            A bytearray containing the data, including the trailing stop word.
+            The buffer is empty or incomplete if timed out
+        """
+        buff = bytearray()
+        lenstop = len(stopword)
+        while buff[-lenstop:] != stopword:
+            try:
+                next = self.read(24)
+                buff.extend(next)
+            except Exception as e:
+                break
+            if len(next) == 0:
+                logger.debug(
+                    "read_until(): did not end with correct stop word (got %s)",
+                    buff[-lenstop:],
+                )
+                break
+        if len(buff) == 0:
+            logger.debug("Receive timeout, no data returned")
+        return buff
+
+    def read_all(self) -> bytes:
+        """Read all waiting bytes"""
+        fifo = self._rx_fifo
+        while True:
+            try:
+                data = self.read(_UDP_READ_BUFFER_SIZE)
+                fifo.extend(data)
+            except Exception as e:
+                break
+            if len(data) == 0:
+                break
+        self._rx_fifo = bytearray()
+        return fifo
+
     def receive(self, length: int = -1, timeout: int = 100, raw: bool = False):
         """Receives data from the socket.
 
         Args:
             length (int): the number of bytes to receive
             timeout (int): the number of milliseconds to wait before giving up
             raw (bool): return bytes (True), or return a hex string (False)
 
         Returns:
             Hex string or bytes, depending on the `raw` flag, or None if
             no data was received in time.
         """
-        if length <= 0:
-            length = self.response_length
-
-        while not self.in_waiting and timeout > 0:
-            timeout -= 1
-            time.sleep(0.001)
-
-        if not self.in_waiting:
-            return None
-
-        # Read a single command from the socket
-        buff, _ = self.socket.recvfrom(length)
-
-        if raw:
-            return buff
-        else:
-            return binascii.hexlify(buff)
+        return self.read_until(self.stop_word)
 
     def receive_all(self, timeout: int = 100, raw: bool = False):
         """Receives all waiting data from the socket.
 
         Args:
             timeout (int): the number of milliseconds to wait before giving up
             raw (bool): return bytes (True), or return a hex string (False)
```

### Comparing `naludaq-0.26.3/src/naludaq/board/initializers/__init__.py` & `naludaq-0.26.4/src/naludaq/board/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/initializers/aardvarcv3.py` & `naludaq-0.26.4/src/naludaq/board/initializers/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/initializers/aodsoc.py` & `naludaq-0.26.4/src/naludaq/board/initializers/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/initializers/asocv3s.py` & `naludaq-0.26.4/src/naludaq/board/initializers/asocv3s.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/initializers/init_aodsv2_eval.py` & `naludaq-0.26.4/src/naludaq/board/initializers/init_aodsv2_eval.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/initializers/init_hdsocv1.py` & `naludaq-0.26.4/src/naludaq/board/initializers/init_hdsocv1.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/initializers/init_udc.py` & `naludaq-0.26.4/src/naludaq/board/initializers/init_udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/initializers/init_upac96.py` & `naludaq-0.26.4/src/naludaq/board/initializers/init_upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/initializers/trbhm.py` & `naludaq-0.26.4/src/naludaq/board/initializers/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/board/params.py` & `naludaq-0.26.4/src/naludaq/board/params.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/communication/__init__.py` & `naludaq-0.26.4/src/naludaq/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/communication/_chip.py` & `naludaq-0.26.4/src/naludaq/communication/_chip.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/communication/_common.py` & `naludaq-0.26.4/src/naludaq/communication/_common.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/communication/_fpga.py` & `naludaq-0.26.4/src/naludaq/communication/_fpga.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/communication/analog_registers.py` & `naludaq-0.26.4/src/naludaq/communication/analog_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/communication/chip_selection.py` & `naludaq-0.26.4/src/naludaq/communication/chip_selection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/communication/control_registers.py` & `naludaq-0.26.4/src/naludaq/communication/control_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/communication/digital_registers.py` & `naludaq-0.26.4/src/naludaq/communication/digital_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/communication/i2c.py` & `naludaq-0.26.4/src/naludaq/communication/i2c.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/communication/i2c_registers.py` & `naludaq-0.26.4/src/naludaq/communication/i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/communication/registers.py` & `naludaq-0.26.4/src/naludaq/communication/registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/__init__.py` & `naludaq-0.26.4/src/naludaq/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/analog_debug_controller.py` & `naludaq-0.26.4/src/naludaq/controllers/analog_debug_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/biasing_mode/__init__.py` & `naludaq-0.26.4/src/naludaq/controllers/biasing_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/biasing_mode/udc16.py` & `naludaq-0.26.4/src/naludaq/controllers/biasing_mode/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/board/__init__.py` & `naludaq-0.26.4/src/naludaq/controllers/board/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/board/aodsoc.py` & `naludaq-0.26.4/src/naludaq/controllers/board/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/board/asocv3s.py` & `naludaq-0.26.4/src/naludaq/controllers/board/asocv3s.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/board/default.py` & `naludaq-0.26.4/src/naludaq/controllers/board/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/board/hdsoc.py` & `naludaq-0.26.4/src/naludaq/controllers/board/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/board/oleas.py` & `naludaq-0.26.4/src/naludaq/controllers/board/oleas.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/board/trbhm.py` & `naludaq-0.26.4/src/naludaq/controllers/board/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/board/udc.py` & `naludaq-0.26.4/src/naludaq/controllers/board/udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/board/upac.py` & `naludaq-0.26.4/src/naludaq/controllers/board/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/board/upac96.py` & `naludaq-0.26.4/src/naludaq/controllers/board/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/connection/__init__.py` & `naludaq-0.26.4/src/naludaq/controllers/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/connection/connection_controller.py` & `naludaq-0.26.4/src/naludaq/controllers/connection/connection_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -323,27 +323,49 @@
 
         - For ethernet, this means setting tx_mode to ETH and updating the receiver address registers.
         - For non-ethernet, this means setting tx_mode to UART.
         """
         if (
             self.board.using_new_backend
             and ConnectionManager(self.board).device.type == DeviceType.UDP
+            or self.board.connection_info.get("type", "") == "udp"
         ):
             self._configure_ethernet()
         else:
             self._configure_non_ethernet()
 
     def _configure_non_ethernet(self):
         """Configure non-ethernet based (UART/FTDI/USB3) connections."""
         try:
             # enable UART, disable UDP
             self._write_control("tx_mode", 0)
             time.sleep(0.01)
         except:
             LOGGER.debug("Board does not have ethernet capabilities")
+        usb_params = self.board.params.get("uart", {})
+        bundle_mode = usb_params.get("bundle_mode", False)
+        tx_pause = usb_params.get("tx_pause", 0.02)
+        self.set_bundle_mode(bundle_mode)
+        self.set_tx_pause(tx_pause)
+
+    def set_bundle_mode(self, bundle_mode: bool):
+        """Sets the bundle mode on the board."""
+        try:
+            self.board.connection.bundle_mode = bundle_mode
+        except AttributeError:
+            LOGGER.warning("Bundle mode not supported on this connection.")
+        self.board.params["uart"]["bundle_mode"] = bundle_mode
+
+    def set_tx_pause(self, tx_pause: float):
+        """Sets the transmission pause on the board."""
+        try:
+            self.board.connection.tx_pause = tx_pause
+        except AttributeError:
+            LOGGER.warning("TX pause not supported on this connection.")
+        self.board.params["uart"]["tx_pause"] = tx_pause
 
     def _configure_ethernet(self):
         """Configure an ethernet-based connection"""
         recv_ip, recv_port = self.board.connection_info["receiver_addr"]
         recv_octets = self._get_octets_or_raise(recv_ip)
 
         # enable UDP, disable UART
```

### Comparing `naludaq-0.26.3/src/naludaq/controllers/connection/upac.py` & `naludaq-0.26.4/src/naludaq/controllers/connection/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/connection/upac96.py` & `naludaq-0.26.4/src/naludaq/controllers/connection/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/external_dac/__init__.py` & `naludaq-0.26.4/src/naludaq/controllers/external_dac/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/external_dac/aardvarcv3.py` & `naludaq-0.26.4/src/naludaq/controllers/external_dac/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/external_dac/ad5671.py` & `naludaq-0.26.4/src/naludaq/controllers/external_dac/ad5671.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/external_dac/ad5675.py` & `naludaq-0.26.4/src/naludaq/controllers/external_dac/ad5675.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/external_dac/base.py` & `naludaq-0.26.4/src/naludaq/controllers/external_dac/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/external_dac/dac7578.py` & `naludaq-0.26.4/src/naludaq/controllers/external_dac/dac7578.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/external_dac/hdsoc.py` & `naludaq-0.26.4/src/naludaq/controllers/external_dac/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/external_dac/i2c_dac.py` & `naludaq-0.26.4/src/naludaq/controllers/external_dac/i2c_dac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/external_dac/trbhm.py` & `naludaq-0.26.4/src/naludaq/controllers/external_dac/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/external_dac/upac32.py` & `naludaq-0.26.4/src/naludaq/controllers/external_dac/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/gainstages/__init__.py` & `naludaq-0.26.4/src/naludaq/controllers/gainstages/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/gainstages/aodsv2.py` & `naludaq-0.26.4/src/naludaq/controllers/gainstages/aodsv2.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/gainstages/oddsock_aods.py` & `naludaq-0.26.4/src/naludaq/controllers/gainstages/oddsock_aods.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/peripherals/__init__.py` & `naludaq-0.26.4/src/naludaq/controllers/peripherals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/peripherals/aardvarcv3.py` & `naludaq-0.26.4/src/naludaq/controllers/peripherals/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/peripherals/aodsoc.py` & `naludaq-0.26.4/src/naludaq/controllers/peripherals/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/peripherals/hdsoc.py` & `naludaq-0.26.4/src/naludaq/controllers/peripherals/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/peripherals/peripherals_controller.py` & `naludaq-0.26.4/src/naludaq/controllers/peripherals/peripherals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/peripherals/upac.py` & `naludaq-0.26.4/src/naludaq/controllers/peripherals/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/peripherals/upac96.py` & `naludaq-0.26.4/src/naludaq/controllers/peripherals/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/project_controller.py` & `naludaq-0.26.4/src/naludaq/controllers/project_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/readout/__init__.py` & `naludaq-0.26.4/src/naludaq/controllers/readout/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/readout/aardvarcv3.py` & `naludaq-0.26.4/src/naludaq/controllers/readout/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/readout/asocv3.py` & `naludaq-0.26.4/src/naludaq/controllers/readout/asocv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/readout/default.py` & `naludaq-0.26.4/src/naludaq/controllers/readout/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/readout/hdsoc.py` & `naludaq-0.26.4/src/naludaq/controllers/readout/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/readout/trbhm.py` & `naludaq-0.26.4/src/naludaq/controllers/readout/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/si5341_controller.py` & `naludaq-0.26.4/src/naludaq/controllers/si5341_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/tia/__init__.py` & `naludaq-0.26.4/src/naludaq/controllers/tia/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/tia/base.py` & `naludaq-0.26.4/src/naludaq/controllers/tia/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/tia/hdsoc.py` & `naludaq-0.26.4/src/naludaq/controllers/tia/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/trigger/__init__.py` & `naludaq-0.26.4/src/naludaq/controllers/trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/trigger/aodsoc.py` & `naludaq-0.26.4/src/naludaq/controllers/trigger/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/trigger/default.py` & `naludaq-0.26.4/src/naludaq/controllers/trigger/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/trigger/hdsoc.py` & `naludaq-0.26.4/src/naludaq/controllers/trigger/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/trigger/trbhm.py` & `naludaq-0.26.4/src/naludaq/controllers/trigger/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/trigger/upac.py` & `naludaq-0.26.4/src/naludaq/controllers/trigger/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/controllers/trigger/upac96.py` & `naludaq-0.26.4/src/naludaq/controllers/trigger/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/daq/__init__.py` & `naludaq-0.26.4/src/naludaq/daq/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/daq/debugdaq.py` & `naludaq-0.26.4/src/naludaq/daq/debugdaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/daq/lightdaq.py` & `naludaq-0.26.4/src/naludaq/daq/lightdaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/daq/preprocess.py` & `naludaq-0.26.4/src/naludaq/daq/preprocess.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/daq/workers/__init__.py` & `naludaq-0.26.4/src/naludaq/daq/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/daq/workers/answer_parser_worker.py` & `naludaq-0.26.4/src/naludaq/daq/workers/answer_parser_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/daq/workers/csv_storage_worker.py` & `naludaq-0.26.4/src/naludaq/daq/workers/csv_storage_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/daq/workers/packager/__init__.py` & `naludaq-0.26.4/src/naludaq/daq/workers/packager/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/daq/workers/packager/worker_packager.py` & `naludaq-0.26.4/src/naludaq/daq/workers/packager/worker_packager.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/daq/workers/packager/worker_packager_debug.py` & `naludaq-0.26.4/src/naludaq/daq/workers/packager/worker_packager_debug.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py` & `naludaq-0.26.4/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/daq/workers/postprocessing.py` & `naludaq-0.26.4/src/naludaq/daq/workers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/daq/workers/worker_parser.py` & `naludaq-0.26.4/src/naludaq/daq/workers/worker_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/daq/workers/worker_serial_reader.py` & `naludaq-0.26.4/src/naludaq/daq/workers/worker_serial_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/daq/workers/worker_usb_reader.py` & `naludaq-0.26.4/src/naludaq/daq/workers/worker_usb_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/devices/eeprom.py` & `naludaq-0.26.4/src/naludaq/devices/eeprom.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/devices/i2c_device.py` & `naludaq-0.26.4/src/naludaq/devices/i2c_device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/devices/ltc2990.py` & `naludaq-0.26.4/src/naludaq/devices/ltc2990.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/helpers/decorators.py` & `naludaq-0.26.4/src/naludaq/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/helpers/exceptions.py` & `naludaq-0.26.4/src/naludaq/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/helpers/fancyiter.py` & `naludaq-0.26.4/src/naludaq/helpers/fancyiter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/helpers/helper_functions.py` & `naludaq-0.26.4/src/naludaq/helpers/helper_functions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/helpers/operations.py` & `naludaq-0.26.4/src/naludaq/helpers/operations.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/helpers/register_cache.py` & `naludaq-0.26.4/src/naludaq/helpers/register_cache.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/helpers/semiton.py` & `naludaq-0.26.4/src/naludaq/helpers/semiton.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/helpers/validations.py` & `naludaq-0.26.4/src/naludaq/helpers/validations.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/io/__init__.py` & `naludaq-0.26.4/src/naludaq/io/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/io/csv_writer.py` & `naludaq-0.26.4/src/naludaq/io/csv_writer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/io/hdf5.py` & `naludaq-0.26.4/src/naludaq/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/io/io_manager.py` & `naludaq-0.26.4/src/naludaq/io/io_manager.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/models/acq_converters.py` & `naludaq-0.26.4/src/naludaq/models/acq_converters.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/models/acquisition.py` & `naludaq-0.26.4/src/naludaq/models/acquisition.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/naludaq.py` & `naludaq-0.26.4/src/naludaq/naludaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/__init__.py` & `naludaq-0.26.4/src/naludaq/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/aardvarcv3_parser.py` & `naludaq-0.26.4/src/naludaq/parsers/aardvarcv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/answer_parser.py` & `naludaq-0.26.4/src/naludaq/parsers/answer_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/aodsoc_parser.py` & `naludaq-0.26.4/src/naludaq/parsers/aodsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/asocv3_parser.py` & `naludaq-0.26.4/src/naludaq/parsers/asocv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/asocv3s_parser.py` & `naludaq-0.26.4/src/naludaq/parsers/asocv3s_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/hdsoc_parser.py` & `naludaq-0.26.4/src/naludaq/parsers/hdsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/headers/__init__.py` & `naludaq-0.26.4/src/naludaq/parsers/headers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/headers/asoc.py` & `naludaq-0.26.4/src/naludaq/parsers/headers/asoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/headers/asocv2.py` & `naludaq-0.26.4/src/naludaq/parsers/headers/asocv2.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/headers/base.py` & `naludaq-0.26.4/src/naludaq/parsers/headers/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/headers/siread.py` & `naludaq-0.26.4/src/naludaq/parsers/headers/siread.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/headers/trbhm.py` & `naludaq-0.26.4/src/naludaq/parsers/headers/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/headers/upac32.py` & `naludaq-0.26.4/src/naludaq/parsers/headers/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/parser.py` & `naludaq-0.26.4/src/naludaq/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/trbhm_parser.py` & `naludaq-0.26.4/src/naludaq/parsers/trbhm_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/udc_parser.py` & `naludaq-0.26.4/src/naludaq/parsers/udc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/upac96_parser.py` & `naludaq-0.26.4/src/naludaq/parsers/upac96_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/parsers/upac_parser.py` & `naludaq-0.26.4/src/naludaq/parsers/upac_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/adc2mv/adc_converter.py` & `naludaq-0.26.4/src/naludaq/tools/adc2mv/adc_converter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/adc2mv/adc_linear_regression.py` & `naludaq-0.26.4/src/naludaq/tools/adc2mv/adc_linear_regression.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/adc2mv/generate.py` & `naludaq-0.26.4/src/naludaq/tools/adc2mv/generate.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/adc2mv/pre_adc2mv.py` & `naludaq-0.26.4/src/naludaq/tools/adc2mv/pre_adc2mv.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/autoaction.py` & `naludaq-0.26.4/src/naludaq/tools/autoaction.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/autotrigger/default.py` & `naludaq-0.26.4/src/naludaq/tools/autotrigger/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/board_backup.py` & `naludaq-0.26.4/src/naludaq/tools/board_backup.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/dac_sweep/dac_sweep_controller.py` & `naludaq-0.26.4/src/naludaq/tools/dac_sweep/dac_sweep_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/data_collector/_daq_interface.py` & `naludaq-0.26.4/src/naludaq/tools/data_collector/_daq_interface.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/data_collector/default.py` & `naludaq-0.26.4/src/naludaq/tools/data_collector/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/data_collector/udc16.py` & `naludaq-0.26.4/src/naludaq/tools/data_collector/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/features.py` & `naludaq-0.26.4/src/naludaq/tools/features.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/ft60x.py` & `naludaq-0.26.4/src/naludaq/tools/ft60x.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/ftdi.py` & `naludaq-0.26.4/src/naludaq/tools/ftdi.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/lookup_table/lookup_table.py` & `naludaq-0.26.4/src/naludaq/tools/lookup_table/lookup_table.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/lookup_table/lookup_table_generator.py` & `naludaq-0.26.4/src/naludaq/tools/lookup_table/lookup_table_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/metadata.py` & `naludaq-0.26.4/src/naludaq/tools/metadata.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/optimizers/bayesian_optimizer.py` & `naludaq-0.26.4/src/naludaq/tools/optimizers/bayesian_optimizer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/optimizers/conversion_ramp/__init__.py` & `naludaq-0.26.4/src/naludaq/tools/optimizers/conversion_ramp/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py` & `naludaq-0.26.4/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/optimizers/conversion_ramp/udc16.py` & `naludaq-0.26.4/src/naludaq/tools/optimizers/conversion_ramp/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/optimizers/gainstagetuner.py` & `naludaq-0.26.4/src/naludaq/tools/optimizers/gainstagetuner.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/pedestals/__init__.py` & `naludaq-0.26.4/src/naludaq/tools/pedestals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/pedestals/generators/__init__.py` & `naludaq-0.26.4/src/naludaq/tools/pedestals/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/pedestals/generators/default.py` & `naludaq-0.26.4/src/naludaq/tools/pedestals/generators/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/pedestals/generators/hdsoc.py` & `naludaq-0.26.4/src/naludaq/tools/pedestals/generators/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/pedestals/generators/udc16.py` & `naludaq-0.26.4/src/naludaq/tools/pedestals/generators/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/pedestals/generators/upac96.py` & `naludaq-0.26.4/src/naludaq/tools/pedestals/generators/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/pedestals/pedestals_correcter.py` & `naludaq-0.26.4/src/naludaq/tools/pedestals/pedestals_correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/pedestals/pedestals_processor.py` & `naludaq-0.26.4/src/naludaq/tools/pedestals/pedestals_processor.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/pedestals/upac32_pedestals_controller.py` & `naludaq-0.26.4/src/naludaq/tools/pedestals/upac32_pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/threshold_scan/__init__.py` & `naludaq-0.26.4/src/naludaq/tools/threshold_scan/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py` & `naludaq-0.26.4/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/threshold_scan/threshold_scan.py` & `naludaq-0.26.4/src/naludaq/tools/threshold_scan/threshold_scan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/threshold_scan/upac96_thresholdscan.py` & `naludaq-0.26.4/src/naludaq/tools/threshold_scan/upac96_thresholdscan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/timing_cal/__init__.py` & `naludaq-0.26.4/src/naludaq/tools/timing_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/timing_cal/calibration.py` & `naludaq-0.26.4/src/naludaq/tools/timing_cal/calibration.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/timing_cal/correcter.py` & `naludaq-0.26.4/src/naludaq/tools/timing_cal/correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq/tools/waiter/eventwaiter.py` & `naludaq-0.26.4/src/naludaq/tools/waiter/eventwaiter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.3/src/naludaq.egg-info/PKG-INFO` & `naludaq-0.26.4/src/naludaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.26.3
+Version: 0.26.4
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naludaq-0.26.3/src/naludaq.egg-info/SOURCES.txt` & `naludaq-0.26.4/src/naludaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

