# Comparing `tmp/sbp-5.0.8.tar.gz` & `tmp/sbp-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbp-5.0.8.tar", last modified: Fri Mar 29 23:44:04 2024, max compression
+gzip compressed data, was "sbp-6.0.0.tar", last modified: Wed May  8 00:02:21 2024, max compression
```

## Comparing `sbp-5.0.8.tar` & `sbp-6.0.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxr-x   0 sokhea    (1000) sokhea    (1000)        0 2024-03-29 23:44:04.516988 sbp-5.0.8/
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     1149 2024-03-29 23:43:59.000000 sbp-5.0.8/.gitignore
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)      225 2024-03-29 23:43:59.000000 sbp-5.0.8/MANIFEST.in
--rw-r--r--   0 sokhea    (1000) sokhea    (1000)     2961 2024-03-29 23:44:04.516988 sbp-5.0.8/PKG-INFO
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     1831 2024-03-29 23:43:59.000000 sbp-5.0.8/README.rst
-drwxrwxr-x   0 sokhea    (1000) sokhea    (1000)        0 2024-03-29 23:44:04.512988 sbp-5.0.8/bin/
--rwxrwxr-x   0 sokhea    (1000) sokhea    (1000)      106 2024-03-18 06:19:44.000000 sbp-5.0.8/bin/sbp2json
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     5192 2024-03-29 23:43:59.000000 sbp-5.0.8/deploy.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)       44 2024-03-29 23:43:59.000000 sbp-5.0.8/requirements.txt
-drwxrwxr-x   0 sokhea    (1000) sokhea    (1000)        0 2024-03-29 23:44:04.516988 sbp-5.0.8/sbp/
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)        5 2024-03-29 23:31:35.000000 sbp-5.0.8/sbp/RELEASE-VERSION
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)      636 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/__init__.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)      178 2024-03-29 23:44:04.000000 sbp-5.0.8/sbp/_version.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)    23820 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/acquisition.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)    15233 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/bootload.py
-drwxrwxr-x   0 sokhea    (1000) sokhea    (1000)        0 2024-03-29 23:44:04.516988 sbp-5.0.8/sbp/client/
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)      619 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/__init__.py
-drwxrwxr-x   0 sokhea    (1000) sokhea    (1000)        0 2024-03-29 23:44:04.516988 sbp-5.0.8/sbp/client/drivers/
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)        0 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/drivers/__init__.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     3204 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/drivers/base_driver.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     2019 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/drivers/cdc_driver.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     2958 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/drivers/file_driver.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     3912 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/drivers/network_drivers.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     1071 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/drivers/pyftdi_driver.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     3742 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/drivers/pyserial_driver.py
-drwxrwxr-x   0 sokhea    (1000) sokhea    (1000)        0 2024-03-29 23:44:04.516988 sbp-5.0.8/sbp/client/examples/
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)        0 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/examples/__init__.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     1706 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/examples/simple.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     1756 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/examples/tcp.py
--rwxrwxr-x   0 sokhea    (1000) sokhea    (1000)     2363 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/examples/udp.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     1854 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/forwarder.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     5828 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/framer.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)    10474 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/handler.py
-drwxrwxr-x   0 sokhea    (1000) sokhea    (1000)        0 2024-03-29 23:44:04.516988 sbp-5.0.8/sbp/client/loggers/
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)        0 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/loggers/__init__.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     3237 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/loggers/base_logger.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     6242 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/loggers/json_logger.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)      879 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/loggers/null_logger.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     2074 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/loggers/rotating_logger.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     1264 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/loggers/udp_logger.py
-drwxrwxr-x   0 sokhea    (1000) sokhea    (1000)        0 2024-03-29 23:44:04.516988 sbp-5.0.8/sbp/client/util/
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)        0 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/util/__init__.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     6642 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/util/fftmonitor.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     4808 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/client/util/settingmonitor.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     2799 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/constants.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     4078 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/ext_events.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)    29601 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/file_io.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)    28974 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/flash.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     7543 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/gnss.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     7988 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/imu.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)    29225 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/integrity.py
-drwxrwxr-x   0 sokhea    (1000) sokhea    (1000)        0 2024-03-29 23:44:04.516988 sbp-5.0.8/sbp/jit/
--rwxrwxr-x   0 sokhea    (1000) sokhea    (1000)       87 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/jit/__init__.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)    40966 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/linux.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     9083 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/logging.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     3974 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/mag.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     7183 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/msg.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)   175339 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/navigation.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     5137 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/ndb.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)   192966 2024-03-29 23:20:21.000000 sbp-5.0.8/sbp/observation.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)    16064 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/orientation.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)    70610 2024-03-29 23:20:21.000000 sbp-5.0.8/sbp/piksi.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     4899 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/profiling.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     3922 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/sbas.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     6981 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/sbp2json.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)    29596 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/settings.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)    39543 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/signing.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)    13871 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/solution_meta.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)   112844 2024-03-29 23:20:21.000000 sbp-5.0.8/sbp/ssr.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)    45560 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/system.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     4066 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/table.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     6541 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/telemetry.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)    39652 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/tracking.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     3374 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/user.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     2495 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/utils.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     8453 2024-03-29 23:20:20.000000 sbp-5.0.8/sbp/vehicle.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     2998 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp/version.py
-drwxrwxr-x   0 sokhea    (1000) sokhea    (1000)        0 2024-03-29 23:44:04.516988 sbp-5.0.8/sbp.egg-info/
--rw-r--r--   0 sokhea    (1000) sokhea    (1000)     2961 2024-03-29 23:44:04.000000 sbp-5.0.8/sbp.egg-info/PKG-INFO
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     1656 2024-03-29 23:44:04.000000 sbp-5.0.8/sbp.egg-info/SOURCES.txt
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)        1 2024-03-29 23:44:04.000000 sbp-5.0.8/sbp.egg-info/dependency_links.txt
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)        1 2024-03-18 06:26:37.000000 sbp-5.0.8/sbp.egg-info/not-zip-safe
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)       92 2024-03-29 23:44:04.000000 sbp-5.0.8/sbp.egg-info/requires.txt
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)       13 2024-03-29 23:44:04.000000 sbp-5.0.8/sbp.egg-info/top_level.txt
-drwxrwxr-x   0 sokhea    (1000) sokhea    (1000)        0 2024-03-29 23:44:04.516988 sbp-5.0.8/sbp2json/
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)        0 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp2json/__init__.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)       83 2024-03-18 06:19:44.000000 sbp-5.0.8/sbp2json/__main__.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)      103 2024-03-29 23:44:04.516988 sbp-5.0.8/setup.cfg
--rwxrwxr-x   0 sokhea    (1000) sokhea    (1000)     6006 2024-03-29 23:43:59.000000 sbp-5.0.8/setup.py
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)       11 2024-03-29 23:43:59.000000 sbp-5.0.8/setup_requirements.txt
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)      112 2024-03-29 23:43:59.000000 sbp-5.0.8/test_requirements.txt
--rw-rw-r--   0 sokhea    (1000) sokhea    (1000)     1044 2024-03-29 23:43:59.000000 sbp-5.0.8/tox.ini
+drwxrwxr-x   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-08 00:02:21.634200 sbp-6.0.0/
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     1149 2024-05-08 00:02:17.000000 sbp-6.0.0/.gitignore
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)      225 2024-05-08 00:02:17.000000 sbp-6.0.0/MANIFEST.in
+-rw-r--r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     2961 2024-05-08 00:02:21.634200 sbp-6.0.0/PKG-INFO
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     1831 2024-05-08 00:02:17.000000 sbp-6.0.0/README.rst
+drwxrwxr-x   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-08 00:02:21.630200 sbp-6.0.0/bin/
+-rwxrwxr-x   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)      106 2024-05-07 20:44:20.000000 sbp-6.0.0/bin/sbp2json
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     5192 2024-05-08 00:02:17.000000 sbp-6.0.0/deploy.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)       44 2024-05-08 00:02:17.000000 sbp-6.0.0/requirements.txt
+drwxrwxr-x   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-08 00:02:21.630200 sbp-6.0.0/sbp/
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        5 2024-05-07 23:19:54.000000 sbp-6.0.0/sbp/RELEASE-VERSION
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)      636 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/__init__.py
+-rw-r--r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)      178 2024-05-08 00:02:21.000000 sbp-6.0.0/sbp/_version.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)    23820 2024-05-07 23:09:21.000000 sbp-6.0.0/sbp/acquisition.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)    15233 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/bootload.py
+drwxrwxr-x   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-08 00:02:21.630200 sbp-6.0.0/sbp/client/
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)      619 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/__init__.py
+drwxrwxr-x   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-08 00:02:21.630200 sbp-6.0.0/sbp/client/drivers/
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/drivers/__init__.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     3204 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/drivers/base_driver.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     2019 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/drivers/cdc_driver.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     2958 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/drivers/file_driver.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     3912 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/drivers/network_drivers.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     1071 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/drivers/pyftdi_driver.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     3742 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/drivers/pyserial_driver.py
+drwxrwxr-x   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-08 00:02:21.630200 sbp-6.0.0/sbp/client/examples/
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/examples/__init__.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     1706 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/examples/simple.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     1756 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/examples/tcp.py
+-rwxrwxr-x   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     2363 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/examples/udp.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     1854 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/forwarder.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     5828 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/framer.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)    10474 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/handler.py
+drwxrwxr-x   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-08 00:02:21.630200 sbp-6.0.0/sbp/client/loggers/
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/loggers/__init__.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     3237 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/loggers/base_logger.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     6242 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/loggers/json_logger.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)      879 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/loggers/null_logger.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     2074 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/loggers/rotating_logger.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     1264 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/loggers/udp_logger.py
+drwxrwxr-x   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-08 00:02:21.630200 sbp-6.0.0/sbp/client/util/
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/util/__init__.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     6642 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/util/fftmonitor.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     4808 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/client/util/settingmonitor.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     2799 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/constants.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     4078 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/ext_events.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)    29601 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/file_io.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)    28974 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/flash.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     7543 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/gnss.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     7988 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/imu.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)    29225 2024-05-07 23:09:21.000000 sbp-6.0.0/sbp/integrity.py
+drwxrwxr-x   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-08 00:02:21.630200 sbp-6.0.0/sbp/jit/
+-rwxrwxr-x   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)       87 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/jit/__init__.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)    40966 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/linux.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     9083 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/logging.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     3974 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/mag.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     7183 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/msg.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)   175339 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/navigation.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     5137 2024-05-07 23:09:21.000000 sbp-6.0.0/sbp/ndb.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)   192966 2024-05-07 23:09:21.000000 sbp-6.0.0/sbp/observation.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)    16064 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/orientation.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)    70610 2024-05-07 23:09:21.000000 sbp-6.0.0/sbp/piksi.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     4899 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/profiling.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     3922 2024-05-07 23:09:21.000000 sbp-6.0.0/sbp/sbas.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     6981 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/sbp2json.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)    29596 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/settings.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)    39543 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/signing.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)    13871 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/solution_meta.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)   112844 2024-05-07 23:09:21.000000 sbp-6.0.0/sbp/ssr.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)    45560 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/system.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     4066 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/table.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     6541 2024-05-07 23:09:21.000000 sbp-6.0.0/sbp/telemetry.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)    39652 2024-05-07 23:09:21.000000 sbp-6.0.0/sbp/tracking.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     3374 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/user.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     2495 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/utils.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     8453 2024-05-07 23:09:20.000000 sbp-6.0.0/sbp/vehicle.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     2998 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp/version.py
+drwxrwxr-x   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-08 00:02:21.630200 sbp-6.0.0/sbp.egg-info/
+-rw-r--r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     2961 2024-05-08 00:02:21.000000 sbp-6.0.0/sbp.egg-info/PKG-INFO
+-rw-r--r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     1656 2024-05-08 00:02:21.000000 sbp-6.0.0/sbp.egg-info/SOURCES.txt
+-rw-r--r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        1 2024-05-08 00:02:21.000000 sbp-6.0.0/sbp.egg-info/dependency_links.txt
+-rw-r--r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        1 2024-05-07 22:09:21.000000 sbp-6.0.0/sbp.egg-info/not-zip-safe
+-rw-r--r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)       92 2024-05-08 00:02:21.000000 sbp-6.0.0/sbp.egg-info/requires.txt
+-rw-r--r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)       13 2024-05-08 00:02:21.000000 sbp-6.0.0/sbp.egg-info/top_level.txt
+drwxrwxr-x   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-08 00:02:21.630200 sbp-6.0.0/sbp2json/
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)        0 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp2json/__init__.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)       83 2024-05-07 20:44:20.000000 sbp-6.0.0/sbp2json/__main__.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)      103 2024-05-08 00:02:21.634200 sbp-6.0.0/setup.cfg
+-rwxrwxr-x   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     6006 2024-05-08 00:02:17.000000 sbp-6.0.0/setup.py
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)       11 2024-05-08 00:02:17.000000 sbp-6.0.0/setup_requirements.txt
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)      112 2024-05-08 00:02:17.000000 sbp-6.0.0/test_requirements.txt
+-rw-rw-r--   0 swiftnav-madhu  (1000) swiftnav-madhu  (1000)     1044 2024-05-08 00:02:17.000000 sbp-6.0.0/tox.ini
```

### Comparing `sbp-5.0.8/.gitignore` & `sbp-6.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/PKG-INFO` & `sbp-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbp
-Version: 5.0.8
+Version: 6.0.0
 Summary: Python bindings for Swift Binary Protocol
 Home-page: https://github.com/swift-nav/libsbp
 Author: Swift Navigation
 Author-email: dev@swift-nav.com
 Platform: linux
 Platform: osx
 Platform: win32
```

### Comparing `sbp-5.0.8/README.rst` & `sbp-6.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/deploy.py` & `sbp-6.0.0/deploy.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/__init__.py` & `sbp-6.0.0/sbp/__init__.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/acquisition.py` & `sbp-6.0.0/sbp/acquisition.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/bootload.py` & `sbp-6.0.0/sbp/bootload.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/__init__.py` & `sbp-6.0.0/sbp/client/__init__.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/drivers/base_driver.py` & `sbp-6.0.0/sbp/client/drivers/base_driver.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/drivers/cdc_driver.py` & `sbp-6.0.0/sbp/client/drivers/cdc_driver.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/drivers/file_driver.py` & `sbp-6.0.0/sbp/client/drivers/file_driver.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/drivers/network_drivers.py` & `sbp-6.0.0/sbp/client/drivers/network_drivers.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/drivers/pyftdi_driver.py` & `sbp-6.0.0/sbp/client/drivers/pyftdi_driver.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/drivers/pyserial_driver.py` & `sbp-6.0.0/sbp/client/drivers/pyserial_driver.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/examples/simple.py` & `sbp-6.0.0/sbp/client/examples/simple.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/examples/tcp.py` & `sbp-6.0.0/sbp/client/examples/tcp.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/examples/udp.py` & `sbp-6.0.0/sbp/client/examples/udp.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/forwarder.py` & `sbp-6.0.0/sbp/client/forwarder.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/framer.py` & `sbp-6.0.0/sbp/client/framer.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/handler.py` & `sbp-6.0.0/sbp/client/handler.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/loggers/base_logger.py` & `sbp-6.0.0/sbp/client/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/loggers/json_logger.py` & `sbp-6.0.0/sbp/client/loggers/json_logger.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/loggers/null_logger.py` & `sbp-6.0.0/sbp/client/loggers/null_logger.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/loggers/rotating_logger.py` & `sbp-6.0.0/sbp/client/loggers/rotating_logger.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/loggers/udp_logger.py` & `sbp-6.0.0/sbp/client/loggers/udp_logger.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/util/fftmonitor.py` & `sbp-6.0.0/sbp/client/util/fftmonitor.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/client/util/settingmonitor.py` & `sbp-6.0.0/sbp/client/util/settingmonitor.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/constants.py` & `sbp-6.0.0/sbp/constants.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/ext_events.py` & `sbp-6.0.0/sbp/ext_events.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/file_io.py` & `sbp-6.0.0/sbp/file_io.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/flash.py` & `sbp-6.0.0/sbp/flash.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/gnss.py` & `sbp-6.0.0/sbp/gnss.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/imu.py` & `sbp-6.0.0/sbp/imu.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/integrity.py` & `sbp-6.0.0/sbp/integrity.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/linux.py` & `sbp-6.0.0/sbp/linux.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/logging.py` & `sbp-6.0.0/sbp/logging.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/mag.py` & `sbp-6.0.0/sbp/mag.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/msg.py` & `sbp-6.0.0/sbp/msg.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/navigation.py` & `sbp-6.0.0/sbp/navigation.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/ndb.py` & `sbp-6.0.0/sbp/ndb.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/observation.py` & `sbp-6.0.0/sbp/observation.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/orientation.py` & `sbp-6.0.0/sbp/orientation.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/piksi.py` & `sbp-6.0.0/sbp/piksi.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/profiling.py` & `sbp-6.0.0/sbp/profiling.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/sbas.py` & `sbp-6.0.0/sbp/sbas.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/sbp2json.py` & `sbp-6.0.0/sbp/sbp2json.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/settings.py` & `sbp-6.0.0/sbp/settings.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/signing.py` & `sbp-6.0.0/sbp/signing.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/solution_meta.py` & `sbp-6.0.0/sbp/solution_meta.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/ssr.py` & `sbp-6.0.0/sbp/ssr.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/system.py` & `sbp-6.0.0/sbp/system.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/table.py` & `sbp-6.0.0/sbp/table.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/telemetry.py` & `sbp-6.0.0/sbp/telemetry.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/tracking.py` & `sbp-6.0.0/sbp/tracking.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/user.py` & `sbp-6.0.0/sbp/user.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/utils.py` & `sbp-6.0.0/sbp/utils.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/vehicle.py` & `sbp-6.0.0/sbp/vehicle.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp/version.py` & `sbp-6.0.0/sbp/version.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/sbp.egg-info/PKG-INFO` & `sbp-6.0.0/sbp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbp
-Version: 5.0.8
+Version: 6.0.0
 Summary: Python bindings for Swift Binary Protocol
 Home-page: https://github.com/swift-nav/libsbp
 Author: Swift Navigation
 Author-email: dev@swift-nav.com
 Platform: linux
 Platform: osx
 Platform: win32
```

### Comparing `sbp-5.0.8/sbp.egg-info/SOURCES.txt` & `sbp-6.0.0/sbp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/setup.py` & `sbp-6.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `sbp-5.0.8/tox.ini` & `sbp-6.0.0/tox.ini`

 * *Files identical despite different names*

