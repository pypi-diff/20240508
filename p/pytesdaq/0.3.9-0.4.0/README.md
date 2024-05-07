# Comparing `tmp/pytesdaq-0.3.9.tar.gz` & `tmp/pytesdaq-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytesdaq-0.3.9.tar", last modified: Tue Apr  2 23:49:15 2024, max compression
+gzip compressed data, was "pytesdaq-0.4.0.tar", last modified: Tue May  7 22:15:01 2024, max compression
```

## Comparing `pytesdaq-0.3.9.tar` & `pytesdaq-0.4.0.tar`

### file list

```diff
@@ -1,73 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.439793 pytesdaq-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-02 23:49:15.439793 pytesdaq-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.431793 pytesdaq-0.3.9/pytesdaq/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.431793 pytesdaq-0.3.9/pytesdaq/analyzer/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27099 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/analyzer/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.431793 pytesdaq-0.3.9/pytesdaq/config/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27396 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/config/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.435793 pytesdaq-0.3.9/pytesdaq/daq/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/daq/daq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/daq/nidaqtask.py
--rw-r--r--   0 runner    (1001) docker     (127)    13736 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/daq/polaris.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.435793 pytesdaq-0.3.9/pytesdaq/display/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20524 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/display/series.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.435793 pytesdaq-0.3.9/pytesdaq/instruments/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)    79504 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/control.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.435793 pytesdaq-0.3.9/pytesdaq/instruments/feb/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/feb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25655 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/feb/feb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.435793 pytesdaq-0.3.9/pytesdaq/instruments/imacrt/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/imacrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18154 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/imacrt/imacrt.py
--rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/imacrt/macrtmodule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.435793 pytesdaq-0.3.9/pytesdaq/instruments/keysight/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/keysight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/keysight/keysight.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.435793 pytesdaq-0.3.9/pytesdaq/instruments/lakeshore/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/lakeshore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61202 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/lakeshore/lakeshore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.435793 pytesdaq-0.3.9/pytesdaq/instruments/magnicon/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/magnicon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52274 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/magnicon/magnicon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.435793 pytesdaq-0.3.9/pytesdaq/instruments/niadc/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/niadc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/instruments/niadc/nidevice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.439793 pytesdaq-0.3.9/pytesdaq/io/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23570 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/io/filter_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    71265 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/io/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.439793 pytesdaq-0.3.9/pytesdaq/processing/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65026 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/processing/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.439793 pytesdaq-0.3.9/pytesdaq/scope/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/scope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38417 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/scope/readout.py
--rw-r--r--   0 runner    (1001) docker     (127)    67331 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/scope/scope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.439793 pytesdaq-0.3.9/pytesdaq/sequencer/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/sequencer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45448 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/sequencer/iv_didv.py
--rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/sequencer/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/sequencer/tc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.439793 pytesdaq-0.3.9/pytesdaq/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/utils/arg_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/utils/connection_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/pytesdaq/utils/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:15.439793 pytesdaq-0.3.9/pytesdaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-02 23:49:15.000000 pytesdaq-0.3.9/pytesdaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-02 23:49:15.000000 pytesdaq-0.3.9/pytesdaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 23:49:15.000000 pytesdaq-0.3.9/pytesdaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 23:49:15.000000 pytesdaq-0.3.9/pytesdaq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-02 23:49:15.000000 pytesdaq-0.3.9/pytesdaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 23:49:15.000000 pytesdaq-0.3.9/pytesdaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 23:49:15.439793 pytesdaq-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-02 23:49:10.000000 pytesdaq-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.279431 pytesdaq-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-07 22:15:01.279431 pytesdaq-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.267432 pytesdaq-0.4.0/pytesdaq/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.267432 pytesdaq-0.4.0/pytesdaq/analyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27444 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/analyzer/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.271432 pytesdaq-0.4.0/pytesdaq/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28505 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/config/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.271432 pytesdaq-0.4.0/pytesdaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/daq/daq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49463 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/daq/daqcontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/daq/nidaqtask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13667 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/daq/polaris.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.271432 pytesdaq-0.4.0/pytesdaq/display/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20524 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/display/series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.271432 pytesdaq-0.4.0/pytesdaq/instruments/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.271432 pytesdaq-0.4.0/pytesdaq/instruments/agilent/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/agilent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/agilent/agilent33500B.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106641 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/control.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.271432 pytesdaq-0.4.0/pytesdaq/instruments/feb/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/feb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25657 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/feb/feb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.271432 pytesdaq-0.4.0/pytesdaq/instruments/imacrt/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/imacrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18154 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/imacrt/imacrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/imacrt/macrtmodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.275431 pytesdaq-0.4.0/pytesdaq/instruments/keithley/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/keithley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/keithley/keithley2400.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.275431 pytesdaq-0.4.0/pytesdaq/instruments/keysight/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/keysight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/keysight/keysightDSOX1200.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.275431 pytesdaq-0.4.0/pytesdaq/instruments/lakeshore/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/lakeshore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61202 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/lakeshore/lakeshore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.275431 pytesdaq-0.4.0/pytesdaq/instruments/magnicon/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/magnicon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52274 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/magnicon/magnicon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.275431 pytesdaq-0.4.0/pytesdaq/instruments/niadc/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/niadc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/instruments/niadc/nidevice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.275431 pytesdaq-0.4.0/pytesdaq/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19341 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/io/filter_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71715 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/io/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.275431 pytesdaq-0.4.0/pytesdaq/scope/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/scope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38502 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/scope/readout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67392 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/scope/scope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.279431 pytesdaq-0.4.0/pytesdaq/sequencer/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/sequencer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45881 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/sequencer/iv_didv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/sequencer/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/sequencer/tc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.279431 pytesdaq-0.4.0/pytesdaq/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/utils/arg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/utils/connection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/pytesdaq/utils/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:15:01.279431 pytesdaq-0.4.0/pytesdaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-07 22:15:01.000000 pytesdaq-0.4.0/pytesdaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-07 22:15:01.000000 pytesdaq-0.4.0/pytesdaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:15:01.000000 pytesdaq-0.4.0/pytesdaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:15:01.000000 pytesdaq-0.4.0/pytesdaq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-07 22:15:01.000000 pytesdaq-0.4.0/pytesdaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 22:15:01.000000 pytesdaq-0.4.0/pytesdaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:15:01.279431 pytesdaq-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-07 22:14:57.000000 pytesdaq-0.4.0/setup.py
```

### Comparing `pytesdaq-0.3.9/PKG-INFO` & `pytesdaq-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytesdaq
-Version: 0.3.9
+Version: 0.4.0
 Summary: DAQ and Intruments control for TES development
 Home-page: https://github.com/spice-herald/pytesdaq
 Author: Bruno Serfass
 Author-email: serfass@berkeley.edu
 Description-Content-Type: text/markdown
 Requires-Dist: PyQt5
 Requires-Dist: matplotlib
```

### Comparing `pytesdaq-0.3.9/README.md` & `pytesdaq-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.9/pytesdaq/analyzer/analyzer.py` & `pytesdaq-0.4.0/pytesdaq/analyzer/analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,21 +233,15 @@
             elif unit=='uAmps':
                 data_array_norm[ichan,:] *= 1e6
             elif unit=='pAmps':
                 data_array_norm[ichan,:] *= 1e12
             
         
         return data_array_norm
-        
-
-
-    
-
-
-
+     
     
     def calc_psd(self, data_array, sample_rate):
         """
         calculate PSD
         """
         
         # initialize
@@ -277,16 +271,14 @@
         """
         Calculate offset
         """
                 
         offset = np.mean(data_array, axis=1)
         return offset
 
-
-    
             
     def fit_didv(self, data_array=None, sample_rate=None, unit='Amps',
                  mask=None, fit_config=None, add_autocuts=True):
         
         """
         dIdV fit:  1 pole (SC, Normal TES) or 2/3 poles (TES in transition)
 
@@ -471,16 +463,26 @@
             if ichan==0:
                 nb_samples = didv_inst._tmean.shape[0]
                 data_array_truncated = np.zeros((nb_channels,nb_samples),
                                                 dtype=np.float64)
                 fit_array = np.zeros((nb_channels,nb_samples),
                                      dtype=np.float64)
                 
-            data_array_truncated[ichan,:] = (didv_inst._tmean - didv_inst._offset)*norm
-          
+            data_array_truncated[ichan,:] = (didv_inst._tmean
+                                             - didv_inst._offset)*norm
+
+            # apply low pass
+            nyq = sample_rate/2
+            cut_off = 30000/nyq
+            b,a = signal.butter(2, cut_off)
+            data_array_truncated[ichan,:] = (
+                signal.filtfilt(b, a, data_array_truncated[ichan,:], axis=-1,
+                                padtype='even')
+            )
+            
             
             # fit
             result = None
             if do_fit_1pole:
                 print('Info: Starting dIdV 1-pole Fit')
                 didv_inst.dofit(1)
                 result = didv_inst.fitresult(1)
@@ -515,15 +517,16 @@
 
                 # P0
                 p0_infinite = tes_bias*rshunt*i0_infinite - (rp + rshunt)*pow(i0_infinite,2)
                 result['infinite_l'] = dict()
                 result['infinite_l']['r0'] = r0_infinite
                 result['infinite_l']['i0'] = i0_infinite
                 result['infinite_l']['p0'] = p0_infinite
-            
+
+                
 
                 
             # Add result to list
             result_list.append(result)
 
             # Fitted response
             dt = 1/sample_rate
@@ -608,22 +611,24 @@
         
         # delete elements
         if self._nb_events_running_avg>=self._analysis_config['nb_events_avg']:
 
             nb_to_delete = self._nb_events_running_avg-self._analysis_config['nb_events_avg']+1
             
             # data buffer
-            self._data_buffer = np.delete(self._data_buffer, list(range(nb_to_delete)), axis=2)
+            self._data_buffer = np.delete(self._data_buffer,
+                                          list(range(nb_to_delete)), axis=2)
 
             # cut buffer
             if self._analysis_config['enable_pileup_rejection']:
                 for cut_name,val in self._cut_buffer.items():
-                    self._cut_buffer[cut_name] = np.delete(val,
-                                                            list(range(nb_to_delete)),
-                                                            axis=1)
+                    self._cut_buffer[cut_name] = np.delete(
+                        val,
+                        list(range(nb_to_delete)),
+                        axis=1)
                 
         # append elements
         self._data_buffer = np.append(self._data_buffer, data_array, axis=2)
         if self._analysis_config['enable_pileup_rejection']:
             for cut_name,val in self._cut_buffer.items():
                 self._cut_buffer[cut_name] = np.append(self._cut_buffer[cut_name],
                                                         cuts_val[cut_name], axis=1)
@@ -797,18 +802,15 @@
         if 'baseline' in self._analysis_config['pileup_cuts']:
             cut_val =  np.mean(data_array, axis=1)
             cut_val.shape += (1,)
             cuts_val['baseline'] = cut_val 
         
 
         return cuts_val
-    
-
   
-
         
         
     def _initialize_config(self):
         """
         Initialize analysis configuration
         """
         
@@ -823,15 +825,15 @@
         self._analysis_config['enable_lowpass_filter'] = False
         self._analysis_config['lowpass_cutoff'] = 50
         self._analysis_config['signal_gen_current'] = None
         self._analysis_config['signal_gen_frequency'] = None
         self._analysis_config['tes_bias'] = None
         self._analysis_config['rshunt'] = 0.005
         self._analysis_config['rp'] = 0.003
-        self._analysis_config['r0'] = 0.2
+        self._analysis_config['r0'] = 0.1
         self._analysis_config['dt'] = 2e-6
         self._analysis_config['add_180phase'] = False
         self._analysis_config['fit_didv'] = False
         self._analysis_config['didv_1pole'] = False
         self._analysis_config['didv_2pole'] = False
         self._analysis_config['didv_3pole'] = False
         self._analysis_config['didv_measurement'] = False
```

### Comparing `pytesdaq-0.3.9/pytesdaq/config/settings.py` & `pytesdaq-0.4.0/pytesdaq/config/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import traceback
 from math import nan
 import os
 import sys
 import copy
 from datetime import datetime
 import time
+import copy
 
 from pytesdaq.utils import connection_utils
 
 
 
 class Config:
     
@@ -163,86 +164,87 @@
             else:
                 output_setup[measurement_name] = config_dict
                           
         except:
             print('WARNING: Problem reading settings file for "'+
                   measurement_name + '" measurement!')
 
-        return output_setup 
+        output_setup_copy = copy.deepcopy(output_setup)
+            
+        return output_setup_copy
 
 
   
     def get_squid_controller(self):
         """
         get SQUID controller device name
         
         Returns:
-           str - no type conversion happens here!
+           str or NoneType
         """
-        controller = str()
+        controller = None
         try:
             controller =  self._get_setting('setup','squid_controller')
         except:
             pass
     
         return controller
 
     def get_tes_controller(self):
         """
         get TES controller device name
         
         Returns:
-           str - no type conversion happens here!
+           str or NoneType
         """
-        controller = str()
+        
+        controller = None
         try:
-            controller =  self._get_setting('setup','tes_controller')
+            controller =  self._get_setting(
+                'setup','tes_controller')
         except:
             pass
     
         return controller
 
-
     def get_temperature_controllers(self):
         """
         get temperature controller device names
         (comma separated)
             
         Returns:
             list of strings - no type conversion happens here!
         """
-        controllers=list()
+        controllers = list()
         
         try:
-            controllers =  self._get_comma_separated_setting('setup','temperature_controllers')
+            controllers =  self._get_comma_separated_setting(
+                'setup','temperature_controllers')
         except:
             pass
         
         return controllers
 
 
-
-
     def get_signal_generator(self):
         """
         get signal generator device name
             
         Returns:
-             str - no type conversion happens here!
+             str o NoneType
         """
-        controller=str()
+        controller = None
         try:
             controller = self._get_setting('setup','signal_generator')
         except:
             pass
     
         return controller
 
 
-
     def enable_redis(self):
         """
         Enable redis
             
         Returns:
              bool
         """
@@ -317,85 +319,65 @@
 
         # default
         preamp_fix_gain = 1
         
         if controller_name is None:
             controller_name = self.get_squid_controller()
 
-
-        if self._has_setting(controller_name,'preamp_fix_gain') and controller_name is not None:
-            preamp_fix_gain =  float(self._get_setting(controller_name,'preamp_fix_gain'))
-            
+        if (controller_name is not None
+            and self._has_setting(controller_name,'preamp_fix_gain')):
+            preamp_fix_gain =  float(self._get_setting(controller_name,
+                                                       'preamp_fix_gain'))
+                   
             
         return preamp_fix_gain
-
-
     
     
     def get_feedback_fix_gain(self, controller_name=None):
         """
         Get SQUID readout feedback fix gain
         """
 
         # default
         feedback_fix_gain = 1
         
         if controller_name is None:
             controller_name = self.get_squid_controller()
 
-
-        if self._has_setting(controller_name,'feedback_fix_gain') and controller_name is not None:
-            feedback_fix_gain =  float(self._get_setting(controller_name,'feedback_fix_gain'))
-            
+        if (controller_name is not None
+            and self._has_setting(controller_name,'feedback_fix_gain')):
+            feedback_fix_gain =  float(self._get_setting(controller_name,
+                                                         'feedback_fix_gain'))
             
         return feedback_fix_gain
 
-
-
-
     
     def get_output_fix_gain(self, controller_name=None):
         """
         Get SQUID readout output driver fix gain
         """
         output_fix_gain = 1
 
         if controller_name is None:
             controller_name = self.get_squid_controller()
 
-        
-        if self._has_setting(controller_name,'output_fix_gain') and controller_name is not None:
-            output_fix_gain =  float(self._get_setting(controller_name,'output_fix_gain'))
-            
+        if (controller_name is not None
+            and self._has_setting(controller_name,'output_fix_gain')):
+            output_fix_gain =  float(self._get_setting(controller_name,
+                                                       'output_fix_gain'))
+                   
         return output_fix_gain
 
-
     
-
-    def get_signal_gen_tes_resistance(self, controller_name=None):
-        """
-        Get SQUID readout output driver fix gain
-        """
-        resistance = nan
-
-        if controller_name is None:
-            controller_name = self.get_squid_controller()
-
-        
-        if self._has_setting(controller_name,'signal_gen_tes_resistance') and controller_name is not None:
-            resistance  =  float(self._get_setting(controller_name,'signal_gen_tes_resistance'))
-            
-        return resistance
-
-
     
     def get_adc_list(self):
         adc_list = list()
         try:
-            adc_list =  self._get_comma_separated_setting('setup','enable_adc')
+            adc_list =  self._get_comma_separated_setting(
+                'setup', 'enable_adc')
         except:
             pass
         
         return adc_list
     
  
     def get_adc_setup(self, adc_id):
@@ -437,17 +419,17 @@
             else:
                 setup[item[0]] = item[1]       
                     
 
         connection_table = pd.DataFrame(adc_connections, columns = column_list)
         setup['connection_table'] = connection_table
         
-
-
-        return setup
+        setup_copy = copy.deepcopy(setup)
+         
+        return setup_copy
 
      
     def get_adc_connections(self, adc_id=None):
         """
         get ADC connections
             
         Returns:
@@ -465,89 +447,91 @@
             for adc in adc_list:
                 adc_setup = self.get_adc_setup(adc)
                 if 'connection_table' in adc_setup:
                     connection_table_list.append(adc_setup['connection_table'])
             if connection_table_list:
                 connection_table = pd.concat(connection_table_list)
             
-        return connection_table 
+        return connection_table.copy() 
 
 
     
     def get_detector_config(self, adc_id=None, adc_channel_list=None):
         """
         get detector config from setup.ini file 
             
         Returns:
            dictionary with config
         """
 
 
         # check arguments
         if  adc_id is None or adc_channel_list is None:
-            raise ValueError('ERROR in get_detector_config: "adc_id" and "adc_channel_list" required!')
+            raise ValueError('ERROR in get_detector_config: "adc_id" and '
+                             '"adc_channel_list" required!')
 
         adc_list = self.get_adc_list()
         if adc_id not in adc_list:
-            raise ValueError('ERROR in get_detector_config: No information in setup file for "'
+            raise ValueError('ERROR in get_detector_config: No information '
+                             + 'in setup file for "'
                              + str(acd_id) + '"!')
 
 
         # intialize
         param_list = ['tes_bias','squid_bias','lock_point_voltage','output_offset',
                       'output_gain','preamp_gain','feedback_polarity','feedback_mode',
                       'signal_source','signal_gen_current','signal_gen_frequency',
                       'squid_turn_ratio','shunt_resistance', 'feedback_resistance',
-                      'parasitic_resistance',
-                      'signal_gen_tes_resistance','close_loop_norm']
-        
+                      'parasitic_resistance', 'tes_bias_resistance',
+                      'signal_gen_resistance','close_loop_norm']
+             
         detector_config = dict()
         for param in param_list:
             detector_config[param] = list()
-            
 
         # store channel lost
         detector_config['adc_name'] = adc_id
         detector_config['channel_type'] = 'adc'
         detector_config['channel_list'] = adc_channel_list
-
-
             
         # loop channel list
         for adc_chan in adc_channel_list:
             item = 'detector_config' + str(adc_chan)
             if not self._has_setting(adc_id, item):
                 continue
 
             settings = self._get_comma_separated_setting(adc_id, item)
             for param in settings:
                 param_split = param.split(':')
                 param_name = param_split[0]
                 param_val = float(param_split[1])
 
                 # some conversion needed
-                if param_name=='tes_bias' or param_name=='squid_bias' or param_name=='signal_gen_current':
+                if (param_name=='tes_bias'
+                    or param_name=='squid_bias'
+                    or param_name=='signal_gen_current'):
                     param_val = param_val/1000000.0
                 if param_name=='lock_point_voltage':
                     param_val = param_val/1000.0
 
                 # add in config
                 detector_config[param_name].append(param_val)
 
-                       
-        return detector_config 
+        detector_config_copy = copy.deepcopy(detector_config)
+        return detector_config_copy
 
     def get_visa_library(self):
         """
         get VISA Library
         
         Returns:
             str - no type conversion happens here!
         """
         library_path = None
+        
         try:
             if self._has_setting('setup','visa_library'):
                 library_path =  self._get_setting('setup','visa_library')
         except:
             pass
     
         return library_path
@@ -556,15 +540,15 @@
     def get_feb_address(self):
         """
         get FEB GPIB address
         
         Returns:
             str - no type conversion happens here!
         """
-        address=str()
+        address = str()
         try:
             address =  self._get_setting('feb','visa_address')
         except:
             pass
     
         return address
 
@@ -661,60 +645,86 @@
             info['reset_active'] = int(self._get_setting('magnicon', 'reset_active'))
         except Exception as e:
             print('ERROR: Could not get complete controller info for Magnicon')
             print(str(e))
             traceback.print_exc()
 
         return info
-
-
-    def get_signal_generator_visa_address(self, device_name):
+    
+    def get_device_visa_address(self, device_name):
         """
-        get function generators
-        
-        Returns:
-            str - no type conversion happens here!
+        get visa address of a device assuming:
+        [device_name]
+           visa_address = ...
+
         """
 
-        key = device_name + '_visa_address'
+        address = None
         
-        address=str()
-        try:
-            address =  self._get_setting('signal_generators',key)
-        except:
-            pass
-    
-        return address
+        # back compatibility if device is "keysight"
+        if device_name == 'keysight':
+            key = 'keysight_visa_address'
+            if self._has_setting('signal_generators', key):
+                address =  str(self._get_setting('signal_generators', key))
+                return address
+            else:
+                # it has been rename to agilent33500B
+                device_name = 'agilent33500B'
 
+                
+        if self._has_setting(device_name, 'visa_address'):
+            address = str(self._get_setting(device_name, 'visa_address'))
+            
+        return address
 
-    def get_signal_generator_attenuation(self, device_name):
+    
+    def get_device_parameters(self, device_name, parameter=None):
         """
-        get function generator attenuation 
+        get visa address of a device assuming:
+        [device_name]
+           visa_address = ...
 
-        Parameters:
-        ----------        
-        device_name : str
-          signal generator name (field in .ini configuration file)
- 
-        Returns:
-        --------
-            attenuation : float
         """
+        
+        # back compatibility if device is "keysight"
+        # (only "attenuation" available)
+        parameters = dict()
+        
+        if device_name == 'keysight':
 
-        key = device_name + '_attenuation'
-    
-        attenuation = 1
-        try:
-            attenuation =  float(self._get_setting('signal_generators', key))
-        except:
-            pass
-    
-        return attenuation
+            if self._has_section('signal_generators'):
+                key = 'keysight_attenuation'
+                if self._has_setting('signal_generators', key):
+                    parameters['attenuation'] = (
+                        float(self._get_setting('signal_generators', key))
+                    )
+                else:
+                    parameters['attenuation'] = None
+                    
+                if parameter == 'attenuation':
+                    return parameters['attenuation']
+                else:
+                    return parameters
+            else:
+                device_name = 'agilent33500B'
+
+        parameters = None
+        if self._has_section(device_name):
+            
+            parameters = self._get_section_dict(device_name)
 
+            if parameter is not None:
+                if parameter in parameters.keys():
+                    parameters = parameters[parameter]
+                else:
+                    parameters = None
 
+        return parameters
+
+   
     def get_temperature_controller_setup(self, device_name):
         """
         get function generators
     
         Args:
             devic_name = "lakeshore" or "macrt"
 
@@ -774,35 +784,33 @@
             # add thermometer and heater list
             output_dict['thermometers'] = thermometer_list
             output_dict['heaters'] =  heater_list
                             
         except:
             raise ValueError('ERROR: Unknown temperature_controllers format!')
                 
-        
-        return output_dict
+        output_dict_copy = copy.deepcopy(output_dict)
+        return output_dict_copy
 
 
-    def get_daq_config(self, trigger_type):
+    def get_daq_config(self, acquisition_type):
         """
         Get daq config by trigger type
         """
-        if  not self._has_section(trigger_type):
-            print('ERROR: Trigger type "' + trigger_type + '" '
-                  + 'not recognized. Available types: '
-                  + 'continuous, randoms, didv, threshold')
-            print('Check code...')
+        
+        if  not self._has_section(acquisition_type):
             return None
 
-        return self._get_section_dict(trigger_type)
+        daq_config = copy.deepcopy(
+            self._get_section_dict(acquisition_type)
+        )
 
-        
-        
-    
+        return daq_config
 
+      
     
     def _get_ini_path(self, ini_filename):
         """
         Get the path where the ini files live. ini files
         should be placed in the same directory as the settings.py module.
     
         Args:
@@ -827,15 +835,14 @@
            
         Returns:
              
         """
         return self._cached_config.items(section) 
 
 
-
     def _has_section(self, section):
         """
         check is section exist
         
         Args:
         
         * section (str)
@@ -864,16 +871,14 @@
         
         Returns:
              str - no type conversion happens here!
         """
         return self._cached_config.get(section, name) 
 
 
-    
-
     def _has_setting(self, section, name):
         """
         check is setting exist
         
         Args:
         
         * section (str)
```

### Comparing `pytesdaq-0.3.9/pytesdaq/daq/daq.py` & `pytesdaq-0.4.0/pytesdaq/daq/daq.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,39 +4,32 @@
 
 from pytesdaq.config import settings
 from pytesdaq.daq import polaris
 from pytesdaq.daq import nidaqtask
 
 
 class DAQ:
-
     
     def __init__(self, driver_name='polaris', verbose=True, setup_file=None):
         
         
         # initialize
         self._verbose = verbose
         self._driver_name = driver_name
         self._driver = None
-           
-      
+          
         # run purpose dict 
         self._run_purpose_dict = {1:'Test', 2:'LowBg', 3:'Calibration', 4:'Noise',
                                   100:'Rp',101:'Rn',102: 'IV', 103:'dIdV'}
         
-      
         # Configuration
         self._config = settings.Config(setup_file=setup_file)
-      
 
         # instantiate driver 
         self._instantiate_driver()
-
-      
-        
           
             
     @property
     def driver_name(self):
         return self._driver_name
         
 
@@ -125,15 +118,15 @@
             return
        
         if self._driver_name=='polaris' or self._driver_name=='pydaqmx':
             self._driver.set_adc_config_from_dict(config_dict)
           
             
 
-    def set_adc_config(self,adc_name, sample_rate=[],nb_samples=[],
+    def set_adc_config(self, adc_name, sample_rate=[],nb_samples=[],
                        voltage_min=list(),voltage_max=list(),
                        channel_list=list(),
                        buffer_length= [],
                        trigger_type=[]):
         
 
         if self._driver_name=='polaris' or self._driver_name=='pydaqmx':
@@ -158,16 +151,20 @@
         if self._driver_name=='polaris':
             self._driver.set_detector_config(config_dict)
         
 
 
     def run(self, run_time=60, run_type=1, run_comment='No comment',
             group_name='None', group_comment='No comment',
-            group_time=None, data_prefix='raw', data_path=None,
-            write_config=True, debug=False):
+            group_time=None, data_prefix='raw',
+            data_path=None, write_config=True,
+            restricted=False, debug=False):
+        """
+        Run data taking
+        """
         
         success = False
 
         # run purpose (using "run type" -> "run pupose" table)
         run_purpose = 'Test'
         if run_type in self._run_purpose_dict:
             run_purpose = self._run_purpose_dict[run_type]
@@ -177,15 +174,14 @@
         fridge_run = self._config.get_fridge_run()
         fridge_run_start = self._config.get_fridge_run_start()
           
         # data path
         if data_path is None:
             data_path = self._config.get_data_path()
 
-
         # series start time
         time_now = int(round(time.time()))
       
         # run polaris
         if self._driver_name=='polaris':
 
             # polaris config
@@ -199,35 +195,33 @@
             run_config['fridge_run'] = fridge_run
             run_config['fridge_run_start'] = fridge_run_start
             run_config['series_start'] = time_now
             if group_time is not None:
                 run_config['group_start'] = group_time 
             run_config['comment'] = '"' + run_comment + '"'
             run_config['data_purpose'] = run_purpose
-            run_config['data_type'] = run_type
+            run_config['restricted'] = int(restricted)
+            run_config['data_prefix'] = data_prefix
             run_config['run_purpose'] = run_purpose
-            run_config['run_type'] = run_type
+            run_config['run_type'] = run_purpose
             run_config['group_name'] = group_name
             run_config['group_comment'] = '"' + group_comment + '"'
             
             prefix = data_path + '/'
             if data_prefix:
                 prefix =  prefix + data_prefix
             run_config['prefix'] = prefix
 
             self._driver.set_run_config(run_config)
             
             # run
             success = self._driver.run(run_time=run_time, run_comment=run_comment,
                                        write_config=write_config, debug=debug)
 
-
         elif self._driver_name=='pydaqmx':
-            
-            # run 
             success = self._driver.run(run_time=run_time, run_comment=run_comment)
 
         return success
 
 
     def read_single_event(self, data_array, do_clear_task=False):
         """
```

### Comparing `pytesdaq-0.3.9/pytesdaq/daq/nidaqtask.py` & `pytesdaq-0.4.0/pytesdaq/daq/nidaqtask.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.9/pytesdaq/daq/polaris.py` & `pytesdaq-0.4.0/pytesdaq/daq/polaris.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,16 +161,15 @@
     def set_adc_config(self,adc_name, device_name=str(), sample_rate=[], nb_samples=[],
                        voltage_min=list(), voltage_max=list(), channel_list=list(), 
                        trigger_type = [],buffer_length=[]):
         
         """
         Set ADC config
         """
-     
-   
+      
         adc_dict = dict()
         if not self._adc_config:
             self._adc_config = dict()
         elif adc_name in self._adc_config:
             adc_dict = self._adc_config[adc_name]
             
             
@@ -229,31 +228,25 @@
             polaris_cmd = polaris_cmd + ' --verbose'
         if self._quiet:
             polaris_cmd = polaris_cmd + ' --quiet'
         if debug:
             polaris_cmd = polaris_cmd + ' --debug'
         if self._log_file:
              polaris_cmd = polaris_cmd + ' --log ' + self._log_file
-
-             
        
         print('INFO: Polaris command: ' + polaris_cmd)
         print('INFO: Starting data taking using polaris!')
         
-               
         # lock
         if self._lock_daq and self._lock_file:
             polaris_cmd = 'flock -n ' + self._lock_file + ' -c '+ '\''+ polaris_cmd +'\''
-
-      
    
         start = datetime.now()
         env = os.environ.copy() # specific environment for polaris?
-  
-     
+       
         with subprocess.Popen(polaris_cmd,shell=True,stdout=subprocess.PIPE, 
                               stderr=subprocess.STDOUT,env=env) as running_task:
      
             while running_task.poll() == None:
 
                 if self._verbose:
                     output = running_task.stdout.readline()
@@ -307,19 +300,16 @@
             print('ERROR: ADC configuration not available! Unable to start run')
             return False
 
         if not self._run_config: 
             print('ERROR: Run configuration not available! Unable to start run')
             return False
 
-
-
         # initialize list
         cfg_list = list()
-
         
         # date
         now = datetime.now()
         dt_string = now.strftime('%d/%m/%Y %H:%M:%S')
         cfg_list.append('# Configuration file production date: ' +  dt_string + '\n\n')
 
        
@@ -332,16 +322,15 @@
                 cfg_list.append('\t\t' + key + ' : ' + str(config_dict[key]) + ',\n')
             cfg_list.append('\t}\n')
         cfg_list.append('}\n\n')
 
         # run config
         for key in self._run_config:
             cfg_list.append(key + ' : ' + str(self._run_config[key]) + ',\n')
-                        
-        
+           
         # adc config
         for adc_name in self._adc_config:
 
             cfg_list.append('\n' + adc_name + ' {\n')
             config_dict = self._adc_config[adc_name]
             
             # check parameter
@@ -389,15 +378,14 @@
                                
             # connection
             for config in config_dict:
                 if 'connection' in config and 'connection_table'!= config:
                     val = ' '.join(map(str,config_dict[config]))
                     cfg_list.append('\t' + config + ' : ' + val + ',\n')
 
-
             data_mode = 'cont'
             if int(config_dict['trigger_type'])==2:
                 data_mode = 'trig-ext'
             
             cfg_list.append('\tdata_mode : ' + data_mode + ',\n')
 
             if data_mode == 'trig-ext':
```

### Comparing `pytesdaq-0.3.9/pytesdaq/display/series.py` & `pytesdaq-0.4.0/pytesdaq/display/series.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.9/pytesdaq/instruments/communication.py` & `pytesdaq-0.4.0/pytesdaq/instruments/communication.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,37 +14,67 @@
                  port=None, recv_port=None,
                  visa_library=None,
                  raise_errors=True, verbose=True):
 
         self._protocol = protocol.lower()
         self._timeout = timeout
         self._termination = termination
-        self._ip_address = ip_address
-        self._visa_address = visa_address
+
+
+        # IP or Visa Address
+        if (ip_address is not None
+            and visa_address is not None):
+            raise ValueError(
+                'InstrumentComm: Choose between '
+                '"ip_address" or "visa_address", '
+                'not both ')
+        self._address = None
+        if ip_address is not None:
+            self._address = ip_address
+        elif visa_address is not None:
+            self._address = visa_address
+            
         self._port = port
         self._recv_port  = recv_port
         if recv_port is None:
             self._recv_port = port
         self._visa_library = visa_library
         self._verbose = verbose
         self._raise_errors = raise_errors
 
         # instrument
         self._inst = None
 
         # debug
         self._debug = False
-        
+
+    @property
+    def address(self):
+        return self._address
+    
         
     def set_address(self, ip_address=None, visa_address=None,
                     port=None, recv_port=None):
         """
         Address
         """
-        self._address = ip_address
+        
+        # IP or Visa Address
+        if (ip_address is not None
+            and visa_address is not None):
+            raise ValueError(
+                'InstrumentComm: Choose between '
+                '"ip_address" or "visa_address", '
+                'not both ')
+       
+        if ip_address is not None:
+            self._address = ip_address
+        elif visa_address is not None:
+            self._address = visa_address
+            
         self._port = port
         self._recv_port  = recv_port
         if recv_port is None:
             self._recv_port = port
 
             
     def get_idn(self):
@@ -126,18 +156,18 @@
 
 
     
     def close(self):
         """
         Close connection to instrument
         """
-        
-        self._inst.close()
-        if self._debug:
-            print('DEBUG: Session closed!')
+        if self._inst  is not None:
+            self._inst.close()
+            if self._debug:
+                print('DEBUG: Session closed!')
 
         self._inst = None
 
 
         
     def disconnect(self):
         """
@@ -178,24 +208,24 @@
             if self._visa_library is None:
                 rm = visa.ResourceManager()
             else:
                 rm = visa.ResourceManager(self._visa_library)
                 
             try:
                 if self._verbose:
-                    print('INFO: Opening VISA resource "{}"'.format(self._visa_address))
+                    print('INFO: Opening VISA resource "{}"'.format(self._address))
 
-                self._inst = rm.open_resource(self._visa_address)
+                self._inst = rm.open_resource(self._address)
                 if self._termination is not None:
                     self._inst.read_termination = self._termination
             
             except visa.VisaIOError as e:
             
                 if self._verbose:
-                    print('ERROR opening VISA resource "{}"'.format(self._visa_address))
+                    print('ERROR opening VISA resource "{}"'.format(self._address))
                 if self._raise_errors:
                     raise
                 else:
                     return None
 
             
     def scan(self, message, scan_port, broadcast_address, coding='utf-8'):
```

### Comparing `pytesdaq-0.3.9/pytesdaq/instruments/feb/feb.py` & `pytesdaq-0.4.0/pytesdaq/instruments/feb/feb.py`

 * *Files 1% similar despite different names*

```diff
@@ -673,15 +673,15 @@
         # address  number
         address = (slot << 8) + (setting << 4) + channel
         
         # data number
         data = 0
         if setting == FEBSettings.SENSORBIAS.value:
             if self._is_modified:
-                data = int(round(4095.0 * (500.0 + value) / 1000.0))
+                data = int(round(4095.0 * (166.67 + value) / 333.33))
             else:
                 data = int(round(4095.0 * (2000.0 + value) / 4000.0)) 
         if setting == FEBSettings.SQUIDBIAS.value:
             data = int(round(4095.0 * (200.0 + value) / 400.0))
         if setting == FEBSettings.SQUIDLOCK.value:
             data = int(round(4095.0 * (8.0 - value) / 16.0))
         if setting == FEBSettings.SQUIDGAIN.value:
@@ -709,15 +709,15 @@
         time.sleep(millisec_delay)
 
         bias_val_hex = self._read_feb(subrack, address)
         decimal_result = int(bias_val_hex, 16) & 4095
 
         if setting == FEBSettings.SENSORBIAS.value:
             if self._is_modified:
-                output_val = 1000.0 * float(decimal_result) / 4095.0 - 500.0
+                output_val = 333.33 * float(decimal_result) / 4095.0 - 166.67
             else:
                 output_val = 4000.0 * float(decimal_result) / 4095.0 - 2000.0
         elif setting == FEBSettings.SQUIDBIAS.value:
             output_val = 400.0 * float(decimal_result) / 4095.0 - 200.0
         elif setting == FEBSettings.SQUIDLOCK.value:
             output_val = -16.0 * float(decimal_result) / 4095.0 + 8.0
         elif setting == FEBSettings.SQUIDGAIN.value:
```

### Comparing `pytesdaq-0.3.9/pytesdaq/instruments/imacrt/imacrt.py` & `pytesdaq-0.4.0/pytesdaq/instruments/imacrt/imacrt.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.9/pytesdaq/instruments/imacrt/macrtmodule.py` & `pytesdaq-0.4.0/pytesdaq/instruments/imacrt/macrtmodule.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.9/pytesdaq/instruments/keysight/keysight.py` & `pytesdaq-0.4.0/pytesdaq/instruments/agilent/agilent33500B.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 from enum import Enum
 from pytesdaq.instruments.communication import InstrumentComm
 
 
-class KeysightFuncGenerator(InstrumentComm):
+class Agilent33500B(InstrumentComm):
     """
     Keysight function generators management
         
     """
 
     def __init__(self, visa_address, visa_library=None,
                  attenuation=1, raise_errors=True,
@@ -22,30 +22,102 @@
 
         # connect to instrument
         self.connect()
 
         # get idn
         self._device_idn = self.get_idn()
 
-
         # model 3312
         self._is_model_3312 = False
         if '3312' in self._device_idn:
              self._is_model_3312 = True
         
         # is generator on 
         self._generator_onoff = 'off'
-        
-
+     
         # signal generator attenuation
         self._attenuation = attenuation
+
+        self.set_auto_range(1)
+
+    def set_auto_range(self, auto, source=1):
+
+        # check input
+        if isinstance(auto, int):
+            if auto==0:
+                auto = 'OFF'
+            else:
+                auto = 'ON'
+            
+        auto = auto.upper()
+
+        if auto != 'ON' and auto != 'OFF':
+            print('ERROR: Argument should be "on" or "off"')
+            if self._raise_errors:
+                raise
+            else:
+                return None
+        command = 'SOURCE' + str(source) +':VOLTAGE:RANGE:AUTO ' + str(auto)
+        #command = 'SOURCE1:VOLTAGE:RANGE:AUTO OFF'
+        self.write(command)
         
         
+
+    def set_load_resistance(self, load='infinity', source=1):
+        """
+        Set output load [Ohms]
+
+        Parameters
+        ---------
+        load: int or string
+            'infinity' or 'inf'
+            'minimum' or 'min'
+            'maximum' or 'max'
+            'default' or 'def'
+            or resistance value in Ohm
+        """
+        # check input
+        if isinstance(load, int):
+            if load<50:
+                load = 50
+            if load>1e6:
+                load = 'infinity'
+        else:
+            load_list = ['infinity', 'inf', 'maximum','max', 'minimum', 'min',
+                         'default', 'def']
+            if load not in load_list:
+
+                print('ERROR: Load type not recognized!')
+                print('Choice is "inf", "max", "min", or "def"')
+                if self._raise_errors:
+                    raise
+
+        # set load
+        command = 'OUTPUT' + str(source) + ':LOAD ' + str(load)
+        self.write(command)
+
+    def get_load_resistance(self, source=1):
+        """
+        Get output load [Ohms]
+
+        Parameters
+        ---------
+        source : int
+           channel (default=1)
+
+        """
+        
+        command = 'OUTPUT' + str(source) + ':LOAD?'
+        resistance = float(self.query(command))
+
+        return resistance
+
+
         
-    def set_shape(self, shape,source=1):
+    def set_shape(self, shape, source=1):
         """
         Set signal shape
 
         
         Parameters
         ----------
         shape: string
@@ -72,15 +144,16 @@
         function_list = ['sinusoid', 'sine', 'square','triangle', 'ramp', 'dc',
                          'arb', 'noise', 'pulse']
 
         
         if shape not in function_list:
 
             print('ERROR: Function type not recognized!')
-            print('Choice is "sine", "square","triangle", "ramp", "dc","arb", "noise", or "pulse"') 
+            print('Choice is "sine", "square","triangle", "ramp",'
+                  '"dc","arb", "noise", or "pulse"') 
             if self._raise_errors:
                 raise
             
         if shape == 'sine':
             shape = 'sin'
 
         # write to device
@@ -95,15 +168,16 @@
 
         Parameters
         ----------
         source: integer
            signal genertor output channel
 
         Returns: string
-          Shape name (lower case): sine, square,triangle, ramp, pulse, prbs, noise,arb,dc
+          Shape name (lower case): sine, square,triangle, ramp, 
+          pulse, prbs, noise,arb,dc
  
         """
 
         # query from device
         command = 'SOUR' + str(source) + ':FUNC?'
         shape = self.query(command)
         shape = shape.lower()
@@ -144,30 +218,36 @@
            signal genertor output channel
 
         
         NOTE: SCPI Names  = {VPP|VRMS|DBM}
         """
 
 
-        unit_list = ['Vpp', 'mVpp', 'Vrms', 'dbm']
+        unit_list = ['V','Vpp', 'mV', 'mVpp', 'Vrms', 'dbm']
 
         if unit not in unit_list:
             print('ERROR: Unit not recognized!')
             print('Choice is "Vpp","mVpp","Vrms",or "dbm"')
             if self._raise_errors:
                 raise
             else:
                 return
-                     
+
+        if unit == 'V':
+            unit = 'Vpp'
+        if unit == 'mV':
+            unit = 'mVpp'
+
+            
         if unit == 'mVpp':
             amplitude = float(amplitude)/1000
             unit = 'Vpp'
 
 
-        # remove attenuation
+        # take into account  attenuation
         amplitude *= self._attenuation
             
         # set unit
         command = 'SOUR' + str(source) + ':VOLT:UNIT ' + unit
         self.write(command)
 
 
@@ -194,24 +274,28 @@
         -------
         
         amplitude: float
           amplitude with unit based on "unit" parameter
 
         """
 
-        unit_list = ['Vpp','mVpp','Vrms','dbm']
+        unit_list = ['V','Vpp','mV', 'mVpp','Vrms','dbm']
 
         if unit not in unit_list:
             print('ERROR: Unit not recognized!')
             print('Choice is "Vpp","mVpp","Vrms",or "dbm"')
             if self._raise_errors:
                 raise
             else:
                 return None
 
+        if unit == 'V':
+            unit = 'Vpp'
+        if unit == 'mV':
+            unit = 'mVpp'
 
         convert_mVpp = False
         if unit == 'mVpp':
             unit = 'Vpp'
             convert_mVpp = True
             
             
@@ -224,15 +308,14 @@
         command = 'SOUR' + str(source) + ':VOLT?'
         amplitude = float(self.query(command))
 
 
         # attenuation
         amplitude /= self._attenuation
         
-
         if convert_mVpp:
             amplitude *= 1000
 
         return amplitude
 
 
     def set_offset(self, offset, unit='V', source=1):
@@ -250,34 +333,38 @@
 
         source: integer
            signal genertor output channel
 
         """
 
 
-        unit_list = ['V', 'mV']
+        unit_list = ['V', 'mV', 'Vpp','mVpp']
 
         if unit not in unit_list:
             print('ERROR: Unit not recognized!')
             print('Choice is "V","mV"')
             if self._raise_errors:
                 raise
             else:
                 return
+
+        if unit == 'Vpp':
+            unit = 'V'
+        if unit == 'mVpp':
+            unit = 'mV'
                      
         if unit == 'mV':
             offset = float(offset)/1000
-            
-     
+
+        # take into account  attenuation
+        offset *= self._attenuation
+                   
         # set offset
         command = 'SOUR' + str(source) + ':VOLT:OFFS ' + str(offset)
         self.write(command)
-
-
-
         
     def get_offset(self, unit='V', source=1):
         
         """
         Get signal offset
        
         Parameters
@@ -293,39 +380,81 @@
         -------
         
         offset: float
           offset with unit based on "unit" parameter
 
 
         """
-
-
-        unit_list = ['V', 'mV']
+        unit_list = ['V', 'mV', 'Vpp', 'mVpp']
 
         if unit not in unit_list:
             print('ERROR: Unit not recognized!')
             print('Choice is "V","mV"')
             if self._raise_errors:
                 raise
             else:
                 return
-         
+     
+        if unit == 'Vpp':
+            unit = 'V'
+        if unit == 'mVpp':
+            unit = 'mV'
+            
         # query offset
         command = 'SOUR' + str(source) + ':VOLT:OFFS?'
         offset = float(self.query(command))
 
+        # attenuation
+        offset /= self._attenuation
+              
         if unit=='mV':
             offset *= 1000
 
         return offset
 
+    
+    def set_phase(self, phase, source=1):
+
+        """
+        Set signal phase
+       
+        Parameters
+        ----------
+        phase: float
+          signal generator phase [degree]
 
-          
+        source: integer
+           signal generator output channel
+
+        """
+
+        # set frequency
+        command = 'SOUR' + str(source) + ':PHAS ' + str(phase)
+        self.write(command)
+
+
+    def get_phase(self, source=1):
+
+        """
+        Get signal phase
+       
+        Parameters
+        ----------
+           source: integer
+              signal generator output channel
+
+        """
+
+        # set frequency
+        command = 'SOUR' + str(source) + ':PHAS?'
+        phase = float(self.query(command))
+        return phase
+    
     
-    def set_frequency(self,frequency,unit='Hz',source=1):
+    def set_frequency(self, frequency, unit='Hz', source=1):
 
         """
         Set signal frequency
        
         Parameters
         ----------
         frequency: float
@@ -356,16 +485,15 @@
             frequency *= 1000
         elif unit=='MHz':
             frequency *= 1e6
             
         # set frequency
         command = 'SOUR' + str(source) + ':FREQ ' + str(frequency)
         self.write(command)
-        
-
+    
         
     def get_frequency(self, unit='Hz', source=1):
         """
         Get signal frequency
        
         Parameters
         ----------
```

### Comparing `pytesdaq-0.3.9/pytesdaq/instruments/lakeshore/lakeshore.py` & `pytesdaq-0.4.0/pytesdaq/instruments/lakeshore/lakeshore.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.9/pytesdaq/instruments/magnicon/magnicon.py` & `pytesdaq-0.4.0/pytesdaq/instruments/magnicon/magnicon.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.9/pytesdaq/instruments/niadc/nidevice.py` & `pytesdaq-0.4.0/pytesdaq/instruments/niadc/nidevice.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.9/pytesdaq/io/hdf5.py` & `pytesdaq-0.4.0/pytesdaq/io/hdf5.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import warnings
 import copy
 
 from pytesdaq.utils import connection_utils
 
 __all__ = ['H5Reader', 'H5Writer',
            'extract_series_num', 'extract_series_name',
-           'extract_dump_num']
+           'extract_dump_num',
+           'convert_length_msec_to_samples']
 
 def extract_series_num(series_name):
     """
     Extract series number from file name or series name
     Assume series name has the following. This function
     should only be used if "series_num" is not stored in raw 
     data.
@@ -117,14 +118,39 @@
     pos = file_name.find('_F')
     if pos>0:
         dump_num = int(file_name[pos+2:pos+6])
           
     return dump_num
 
 
+def convert_length_msec_to_samples(trace_length_msec, fs):
+    """
+    Convert trace length in msec to samples
+
+    Parameters
+    ----------
+    trace_length : float
+      trace length in milli sec
+
+    fs : float
+      sample rate 
+
+    Return
+    ------
+    
+    nb_samples : int
+      trace length samples
+ 
+    """
+
+
+    nb_samples = int(round(fs*trace_length_msec/1000))
+    return nb_samples
+    
+
 
 
 class H5Reader:
     """
     Class to read raw data hdf5 files taken by pytesdaq
     """
```

### Comparing `pytesdaq-0.3.9/pytesdaq/io/redis.py` & `pytesdaq-0.4.0/pytesdaq/io/redis.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.9/pytesdaq/scope/readout.py` & `pytesdaq-0.4.0/pytesdaq/scope/readout.py`

 * *Files 1% similar despite different names*

```diff
@@ -841,21 +841,23 @@
             self._analyzer.set_config('signal_gen_frequency', signal_gen_info['frequency'])
             
             
         # TES bias
         tes_bias_list = list()
         if read_bias or read_sg:
             for chan in self._adc_config['selected_channel_list']:
-                bias = float(self._instrument.get_tes_bias(adc_id=self._adc_name,
-                                                           adc_channel=chan))
+                bias = float(
+                    self._instrument.get_tes_bias(adc_id=self._adc_name,
+                                                  adc_channel=chan,
+                                                  unit='uA')
+                )
                 tes_bias_list.append(bias*1e-6)
+                
             self._analyzer.set_config('tes_bias', tes_bias_list)
-            
-            
-
+    
     def _plot_data(self, data_array, fit_array=None, fit_dt=None, freq_array=[]):
 
 
         if self._do_stop_run:
             return
```

### Comparing `pytesdaq-0.3.9/pytesdaq/scope/scope.py` & `pytesdaq-0.4.0/pytesdaq/scope/scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -1270,17 +1270,16 @@
         self._readout.update_analysis_config(rshunt=rshunt)
 
         if self._phase180_checkbox.isChecked():
             self._readout.update_analysis_config(add_180phase=True)
         else:
             self._readout.update_analysis_config(add_180phase=False)
             
-
-        r0 = float(self._r0_spinbox.value()/1000)
-        self._readout.update_analysis_config(r0=r0)
+        #r0 = float(self._r0_spinbox.value()/1000)
+        #self._readout.update_analysis_config(r0=r0)
 
         # clear field
         self._text_field.clear()
 
         # enable 
         self._readout.update_analysis_config(fit_didv=True)
         
@@ -1378,27 +1377,27 @@
                 self._rp_spinbox.setEnabled(False)
             else:
                 self._tools_tabs.setTabText(0,'Rn Fit')
                 self._rp_spinbox.setEnabled(True)
                 measurement = 'Rn'
             self._tools_tabs.setTabVisible(0,True)
             self._tools_tabs.setCurrentIndex(0)
-            self._r0_spinbox.setEnabled(False)
+            #self._r0_spinbox.setEnabled(False)
             
         elif selection == 'Transition dIdV Fit':
             self._setup_didv_fit()
             self._didv_fit_1pole.setChecked(False)
             self._didv_fit_1pole.setEnabled(False)
             self._didv_fit_2pole.setEnabled(True)
             self._didv_fit_2pole.setChecked(True)
             self._didv_fit_3pole.setEnabled(True)
             self._didv_fit_3pole.setChecked(True)
             self._tools_tabs.setTabText(0,'R0 Fit')
             self._rp_spinbox.setEnabled(True)
-            self._r0_spinbox.setEnabled(True)
+            #self._r0_spinbox.setEnabled(True)
             self._tools_tabs.setTabVisible(0,True)
             self._tools_tabs.setCurrentIndex(0)
             measurement = 'R0'
                        
         else:
             self._didv_fit_1pole.setChecked(False)
             self._didv_fit_2pole.setChecked(False)
@@ -1602,15 +1601,15 @@
         rshunt_label.setText('Rshunt:')
 
         self._rshunt_spinbox = QtWidgets.QDoubleSpinBox(self._didv_tab)
         self._rshunt_spinbox.setGeometry(QtCore.QRect(70, 42, 70, 20))
         self._rshunt_spinbox.setMaximum(100000)
         self._rshunt_spinbox.setProperty('value', 5.0)
         self._rshunt_spinbox.setObjectName('rshuntSpinBox')
-        self._rshunt_spinbox.setDecimals(1)
+        self._rshunt_spinbox.setDecimals(3)
 
         step_type = QtWidgets.QAbstractSpinBox.AdaptiveDecimalStepType
         self._rshunt_spinbox.setStepType(step_type)
         
         # Rp
         rp_label = QtWidgets.QLabel(self._didv_tab)
         rp_label.setGeometry(QtCore.QRect(42, 70, 50, 15))
@@ -1619,71 +1618,64 @@
         rp_label.setText('Rp:')
 
         self._rp_spinbox = QtWidgets.QDoubleSpinBox(self._didv_tab)
         self._rp_spinbox.setGeometry(QtCore.QRect(70, 67, 70, 20))
         self._rp_spinbox.setMaximum(100000)
         self._rp_spinbox.setProperty('value', 2.5)
         self._rp_spinbox.setObjectName('rpSpinBox')
-        self._rp_spinbox.setDecimals(1)
+        self._rp_spinbox.setDecimals(3)
         self._rp_spinbox.setStepType(step_type)
 
-
-
         # R0
-        r0_label = QtWidgets.QLabel(self._didv_tab)
-        r0_label.setGeometry(QtCore.QRect(42, 96, 50, 15))
-        r0_label.setFont(font)
-        r0_label.setObjectName('r0Label')
-        r0_label.setText('R0:')
-
-        self._r0_spinbox = QtWidgets.QDoubleSpinBox(self._didv_tab)
-        self._r0_spinbox.setGeometry(QtCore.QRect(70, 92, 70, 20))
-        self._r0_spinbox.setMaximum(100000)
-        self._r0_spinbox.setProperty('value', 200)
-        self._r0_spinbox.setObjectName('r0SpinBox')
-        self._r0_spinbox.setDecimals(1)
-        self._r0_spinbox.setStepType(step_type)
-
-
-
-
-
+        #r0_label = QtWidgets.QLabel(self._didv_tab)
+        #r0_label.setGeometry(QtCore.QRect(42, 96, 50, 15))
+        #r0_label.setFont(font)
+        #r0_label.setObjectName('r0Label')
+        #r0_label.setText('R0:')
+
+        #self._r0_spinbox = QtWidgets.QDoubleSpinBox(self._didv_tab)
+        #self._r0_spinbox.setGeometry(QtCore.QRect(70, 92, 70, 20))
+        #self._r0_spinbox.setMaximum(100000)
+        #self._r0_spinbox.setProperty('value', 200)
+        #self._r0_spinbox.setObjectName('r0SpinBox')
+        #self._r0_spinbox.setDecimals(1)
+        #self._r0_spinbox.setStepType(step_type)
 
         
         unit_label = QtWidgets.QLabel(self._didv_tab)
-        unit_label.setGeometry(QtCore.QRect(150, 70, 60, 15))
+        unit_label.setGeometry(QtCore.QRect(150, 60, 60, 15))
         unit_label.setFont(font)
         unit_label.setObjectName('rshuntUniyLabel')
         unit_label.setText('[mOhms]')
 
 
         # dt
         dt_label = QtWidgets.QLabel(self._didv_tab)
-        dt_label.setGeometry(QtCore.QRect(39, 120, 50, 15))
+        dt_label.setGeometry(QtCore.QRect(39, 96, 50, 15))
         dt_label.setFont(font)
         dt_label.setObjectName('dtLabel')
         dt_label.setText('dt0:')
 
         self._dt_spinbox = QtWidgets.QDoubleSpinBox(self._didv_tab)
-        self._dt_spinbox.setGeometry(QtCore.QRect(70, 117, 70, 20))
+        self._dt_spinbox.setGeometry(QtCore.QRect(70, 92, 70, 20))
         self._dt_spinbox.setMaximum(100000)
         self._dt_spinbox.setProperty('value', 2)
         self._dt_spinbox.setObjectName('dtSpinBox')
         self._dt_spinbox.setDecimals(1)
         self._dt_spinbox.setStepType(step_type)
 
         dt_unit_label = QtWidgets.QLabel(self._didv_tab)
-        dt_unit_label.setGeometry(QtCore.QRect(150, 118, 60, 15))
+        dt_unit_label.setGeometry(QtCore.QRect(150, 94, 60, 15))
         dt_unit_label.setFont(font)
         dt_unit_label.setObjectName('dtUniyLabel')
         dt_unit_label.setText('[mus]')
         
         # add phase
         self._phase180_checkbox = QtWidgets.QCheckBox(self._didv_tab)
-        self._phase180_checkbox.setGeometry(QtCore.QRect(215, 117, 149, 21))
+        self._phase180_checkbox.setGeometry(QtCore.QRect(42, 117, 149, 21))
         self._phase180_checkbox.setFont(font)
         self._phase180_checkbox.setObjectName('phase180CheckBox')
         self._phase180_checkbox.setText('Add 180 Phase')
 
         
 
 
@@ -1793,22 +1785,24 @@
 
         # Baseline cut
         self._baseline_checkbox = QtWidgets.QCheckBox(self._pileup_cuts_tab)
         self._baseline_checkbox.setGeometry(QtCore.QRect(15, 140, 120, 21))
         self._baseline_checkbox.setFont(font)
         self._baseline_checkbox.setObjectName('baselineCheckBox')
         self._baseline_checkbox.setText('Baseline')
+        self._baseline_checkbox.setChecked(True)
 
+        
         # Baseline sigma
         self._baseline_spinbox = QtWidgets.QSpinBox(self._pileup_cuts_tab)
         self._baseline_spinbox.setGeometry(QtCore.QRect(150, 140, 40, 20))
         self._baseline_spinbox.setMaximum(10)
         self._baseline_spinbox.setProperty('value', 2)
         self._baseline_spinbox.setObjectName('baselineSpinBox')
-        
+       
 
         # OF chi2 cut
         self._ofchi2_checkbox = QtWidgets.QCheckBox(self._pileup_cuts_tab)
         self._ofchi2_checkbox.setGeometry(QtCore.QRect(15, 170, 120, 21))
         self._ofchi2_checkbox.setFont(font)
         self._ofchi2_checkbox.setObjectName('ofchi2CheckBox')
         self._ofchi2_checkbox.setText('OF Chi2')
```

### Comparing `pytesdaq-0.3.9/pytesdaq/sequencer/iv_didv.py` & `pytesdaq-0.4.0/pytesdaq/sequencer/iv_didv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import time
-import pprint as pprint
+from pprint import pprint
 import copy
 from pytesdaq.daq import daq
 import pytesdaq.config.settings as settings
 import pytesdaq.instruments.control as instrument
 from pytesdaq.sequencer.sequencer import Sequencer
 from pytesdaq.utils import connection_utils
 from pytesdaq.utils import arg_utils
@@ -16,15 +16,16 @@
 class IV_dIdV(Sequencer):
     
     def __init__(self, iv =False, didv =False, rp=False, rn=False,
                  temperature_sweep=False,
                  tes_bias_sweep=True,
                  comment='No comment',
                  sweep_channels=None, saved_channels=None,
-                 sequencer_file=None, setup_file=None, sequencer_pickle_file=None,
+                 sequencer_file=None, setup_file=None,
+                 sequencer_pickle_file=None,
                  dummy_mode=False,
                  do_relock=False, do_zero=False, do_zap=False,
                  verbose=True):
 
         # measurements
         self._enable_iv = iv
         self._enable_didv = didv
@@ -59,95 +60,144 @@
                          sequencer_pickle_file=sequencer_pickle_file,
                          dummy_mode=dummy_mode,
                          verbose=verbose)
             
         
         # configure measurements
         self._configure()
-
-
-         
-
   
 
     def run(self):
 
         """ 
         Run IV / dIdV sequencer
         """
-  
-                      
+
         # Instantiate instrumment controller
-        self._instrument = instrument.Control(setup_file=self._setup_file,
-                                              dummy_mode=self._dummy_mode)
-        
+        self._instruments_inst = instrument.Control(
+            setup_file=self._setup_file,
+            dummy_mode=self._dummy_mode
+        )
         
         # ------------
         # Rp/Rn
         # ------------
 
         if self._enable_rp or  self._enable_rn:
             self._run_rp_rn()
         
-
         # ------------
         # IV/dIdV sweep
         # ------------
         if self._enable_iv or self._enable_didv:
             self._run_iv_didv()
 
 
         print('INFO: Sequencer done!')
 
 
-
-
     def _run_iv_didv(self):
         """
         IV/dIdV sweep
         """
 
-
         if not (self._enable_iv or self._enable_didv):
             return True
 
-    
-
         # display
         if self._verbose:
             measurement = str()
             if self._enable_iv and self._enable_didv:
                 measurement = 'IV and dIdV measurements'
             elif self._enable_iv:
                 measurement = 'IV measurement'
             else:
                 measurement = 'dIdV measurement'
         
             print('\n===============================')
             print(measurement) 
             print('===============================\n')
 
-
-
         # sweep config
         sweep_config = self._measurement_config['iv_didv']
         iv_config =  dict()
         didv_config = dict()
         
         if self._enable_iv:
             iv_config =  self._measurement_config['iv']
+
         if self._enable_didv:
+            
             didv_config = self._measurement_config['didv']
+            
             # signal gen amplitude can be either voltage or current
             if 'signal_gen_voltage' not in didv_config:
                 didv_config['signal_gen_voltage'] = None
             if 'signal_gen_current' not in didv_config:
                 didv_config['signal_gen_current'] = None
+
+
+        # for case TES / SG controllers
+        # Tune auto-range and turn off
+        if self._instruments_inst.is_tes_signal_gen_inst_common():
+
+            print('INFO: Case TES and Signal generator controllers '
+                  'are the same: fix signal generator range')
+
+            # get signal gen and tes controllers
+            signal_gen_controller = (
+                self._instruments_inst.get_signal_gen_controller()
+            )
+            tes_controller = self._instruments_inst.get_tes_controller()
+
+            for channel in self._detector_channels:
+
+                # set autorange on 
+                signal_gen_controller.set_auto_range('on')
+                
+                self._instruments_inst.set_tes_bias(
+                    np.max(sweep_config['tes_bias_vect']),
+                    unit='uA',
+                    detector_channel=channel
+                )
+                
+                signal_gen_voltage = 2
+                signal_gen_frequency = 80
+                
+                if 'signal_gen_voltage' in didv_config:
+                    signal_gen_voltage = didv_config['signal_gen_voltage']
+                if 'signal_gen_frequency' in didv_config:
+                    signal_gen_frequency = didv_config['signal_gen_frequency']
+                    
+                print(f'Max func gen offset is {signal_gen_offset} mV')
+                self._instruments_inst.set_signal_gen_onoff(
+                    'on',
+                    detector_channel=channel)
+                
+                self._instruments_inst.set_signal_gen_params(
+                    detector_channel=channel,
+                    source='tes', 
+                    voltage=signal_gen_voltage,
+                    voltage_unit='mV',
+                    frequency=signal_gen_frequency,
+                    frequency_unit='Hz',
+                    shape='square'
+                )
+
+                # set auto range off
+                signal_gen_controller.set_auto_range('off')
+                
+                time.sleep(5)
+
+        # turn SG ouput off (this set to 'dc' if SG/TES controllers are same)
+        for channel in self._detector_channels:
+            self._instruments_inst.set_signal_gen_onoff(
+                'off',
+                detector_channel=channel)
             
-        
                 
         # Temperature loop
         temperature_vect = []
         nb_temperature_steps = 1
         if self._enable_temperature_sweep:
 
             # temperature array
@@ -206,77 +256,75 @@
             if self._enable_temperature_sweep:
                 
                 temperature = temperature_vect[istep]/1000
                 print('INFO: Setting temperature to '
                       + str(temperature*1000) +'mK!')
 
                 
-                self._instrument.set_temperature(
+                self._instruments_inst.set_temperature(
                     temperature,
                     channel_name=thermometer_name,
                     global_channel_number=thermometer_global_num,
                     heater_channel_name=heater_name,
                     heater_global_channel_number=heater_global_num,
                     wait_temperature_reached=True,
                     wait_cycle_time=5,
                     wait_stable_time=wait_stable_time,
                     max_wait_time=max_wait_time,
                     tolerance=tolerance
                 )
-            
-                
-
+   
             # create sequencer directory
-            if (self._enable_tes_bias_sweep or
-                self._group_name is None):
+            if (self._enable_tes_bias_sweep or self._group_name is None):
                 basename = str()
                 if self._enable_iv:
                     basename += '_iv'
                 if self._enable_didv:
                     basename += '_didv'
         
                 if basename[0] == '_':
                     basename = basename[1:]
 
                 self._create_measurement_directories(basename)
         
 
-
             # ZAP TES
             if self._do_zap_tes:
-                tes_bias_max = 500
+                tes_bias_max = 140
                 if sweep_config['use_negative_tes_bias']:
-                    tes_bias_max = -500
+                    tes_bias_max = -140
                     
-                print('INFO: Zapping TES  with bias ' + str(tes_bias_max) + 'uA') 
+                print('INFO: Zapping TES  with bias '
+                      + str(tes_bias_max) + 'uA')
+                
                 for channel in self._detector_channels:
-                    self._instrument.set_tes_bias(tes_bias_max,
-                                                  detector_channel=channel)
+                    self._instruments_inst.set_tes_bias(
+                        tes_bias_max, unit='uA',
+                        detector_channel=channel)
+                    
                 time.sleep(5)
-
-
             
             # IV-dIdV:  TES bias loop
-            sleeptime_s = float(sweep_config['tes_bias_change_sleep_time'])
+            sleeptime_s = 5
+            if 'tes_bias_change_sleep_time' in sweep_config:
+                sleeptime_s = float(sweep_config['tes_bias_change_sleep_time'])
+                
             tes_bias_vect = sweep_config['tes_bias_vect']
             if not self._enable_tes_bias_sweep:
                 tes_bias_vect = [None]
                 
             nb_steps = len(tes_bias_vect)
             istep = 0
 
-                        
-
+         
             # Instantiate DAQ
             self._daq = daq.DAQ(driver_name=self._daq_driver,
                                 verbose=self._verbose,
                                 setup_file=self._setup_file)
 
-
-
             # Initialize online IV
             nb_channels = len(self._detector_channels)
             ivobj = None
             online_iv_offset = None
             online_iv_offset_err = None
             online_iv_std = None
             online_iv_tes_bias = None
@@ -284,37 +332,42 @@
           
 
             # ==========================
             # LOOP QET Bias
             # ==========================
             for bias in tes_bias_vect:
 
-                # set bias all channels
                 istep+=1
+
+                # set TES bias all channels
                 if self._enable_tes_bias_sweep:
-                    print('INFO: Sequencer step #' + str(istep) + ' out of total '
-                          + str(nb_steps) + ' steps!')
-                    print('INFO: Setting TES bias all channels to : '
-                          + str(bias) + 'uA!')
-                    for channel in self._detector_channels:
-                        self._instrument.set_tes_bias(bias, detector_channel=channel)
                     
+                    print(f'INFO: Sequencer step #{istep} '
+                          f'out of total {nb_steps} steps!')
+                    
+                    print(f'INFO: Setting TES bias all channels to : '
+                          f'{bias} uA!')
+                    # set TES bias all channels
+                    for channel in self._detector_channels:
+
+                        self._instruments_inst.set_tes_bias(
+                            bias, unit='uA',
+                            detector_channel=channel
+                        )
+                                
                     # sleep
-                    #if tes_bias_change_sleep_time in sweep_config:
-                    print('INFO: Sleeping for ' + str(sleeptime_s) + ' seconds!')
                     time.sleep(sleeptime_s)
 
-
                 # Relock
                 if self._do_relock:
                 
                     # relock each channel
                     for channel in self._detector_channels:
                         print('INFO: Relocking channel ' + channel) 
-                        self._instrument.relock(detector_channel=channel)
+                        self._instruments_inst.relock(detector_channel=channel)
                 
                 # if step 1: tes zap, relock, zero
                 if istep==1:
                         
                     # Zero
                     if self._do_zero_offset:
 
@@ -342,56 +395,56 @@
                             setup_dict[adc_id]['channel_list'] = adc_list
                             setup_dict[adc_id]['trigger_type'] = 3
                             sample_rate = setup_dict[adc_id]['sample_rate']
                             
                         daq_online.set_adc_config_from_dict(setup_dict)
 
                         # get data
-                        data_array = daq_online.read_many_events(100,
-                                                                 adctovolt=True)
+                        data_array = daq_online.read_many_events(
+                            100,
+                            adctovolt=True)
 
                         # clear
                         daq_online.clear()
 
                        
                         # loop channels and zero once for each
                         for  ichan in range(len(self._detector_channels)):
 
-
                             traces = data_array[:,ichan,:]
-                            cut = qp.autocuts(traces,
-                                              fs=sample_rate)
-                            
-
+                            cut = qp.autocuts(traces, fs=sample_rate)
                             trace_mean = np.mean(traces, axis=0)
                             offset = np.median(trace_mean)
 
-                         
                             # detector channel
                             channel = self._detector_channels[ichan]
-                          
-                            
+
                             # zero
-                            driver_gain = self._instrument.get_output_total_gain(
-                                detector_channel=channel
+                            driver_gain = (
+                                self._instruments_inst.get_output_total_gain(
+                                    detector_channel=channel
+                                )
                             )
-                            current_offset = self._instrument.get_output_offset(
-                                detector_channel=channel
+                            current_offset = (
+                                self._instruments_inst.get_output_offset(
+                                    detector_channel=channel
+                                )
                             )
+                            
                             new_offset = current_offset-offset/driver_gain
-                            self._instrument.set_output_offset(
+                            self._instruments_inst.set_output_offset(
                                 new_offset, detector_channel=channel
                             )
                         
 
                         
                 # get temperature
                 if self._enable_temperature_sweep:
                     
-                    temperature = self._instrument.get_temperature(
+                    temperature = self._instruments_inst.get_temperature(
                         channel_name=thermometer_name,
                         global_channel_number=thermometer_global_num
                     )
 
                     if thermometer_name is not None:
                         print('INFO: ' + thermometer_name + ' temperature is '
                               + str(temperature*1000) +'mK!')
@@ -399,15 +452,15 @@
                          print('INFO: Temperature is '
                                + str(temperature*1000) +'mK!')
 
                     if monitoring_thermometer_names is not None:
                         monitoring_temperature_list = list()
                         for thermometer in monitoring_thermometer_names:
                             monitoring_temperature_list.append(
-                                self._instrument.get_temperature(
+                                self._instruments_inst.get_temperature(
                                     channel_name=thermometer)
                             )
                             time.sleep(2)
 
 
                             
                 # -----------
@@ -416,27 +469,24 @@
                 if self._enable_tes_bias_sweep:
 
 
                     # intialize 
                     offsets = list()
                     offsets_err = list()
                     stds = list()
-                                        
-                    
+                                   
                      # instantiate nidaq
                     daq_online = daq.DAQ(driver_name='pydaqmx', verbose=False)
-                    
-                    
+                                   
                     # get corresponding ADC channels
                     adc_dict = connection_utils.get_adc_channel_list(
                         self._detector_connection_table,
                         detector_channel_list=self._detector_channels
                     )
-                    
-                    
+                                  
                     # set ADC
                     sample_rate = None
                     setup_dict = dict()
                     for adc_id, adc_list in adc_dict.items():
                         setup_dict[adc_id] = copy.deepcopy(
                             self._config.get_adc_setup(adc_id)
                         )
@@ -450,28 +500,28 @@
                     # get data
                     data_array = daq_online.read_many_events(100,
                                                              adctovolt=True)
 
                     # clear
                     daq_online.clear()
 
-
                     # loop channels and zero once for each
                     for  ichan in range(len(self._detector_channels)):
 
-
                         traces = data_array[:,ichan,:]
                         cut = qp.autocuts(traces,
                                           fs=sample_rate)
                         
                         traces = traces[cut]
                         
                         # convert to amps
-                        norm = self._instrument.get_volts_to_amps_close_loop_norm(
-                            detector_channel=channel
+                        norm = (
+                            self._instruments_inst.get_volts_to_amps_close_loop_norm(
+                                detector_channel=channel
+                            )
                         )
 
                         traces /= norm
 
                         # offset
                         offset, offset_err = qp.utils.calc_offset(traces)
                         offsets.append([offset])
@@ -483,18 +533,15 @@
                         b,a = signal.butter(2, cut_off)
                         traces = signal.filtfilt(b, a, traces, axis=1,
                                                  padtype='even')
 
                         traces_std = np.std(traces, axis=1)
                         std_median = np.median(traces_std, axis=0)
                         stds.append([std_median])
-                    
-
-
-
+          
                     # save
                     bias_array = [[-bias*1e-6]]*nb_channels
                     bias_err_array = [[0]]*nb_channels
                     
                     if online_iv_offset is None:
                         online_iv_offset = np.array(offsets)
                     else:
@@ -526,206 +573,187 @@
                     if online_iv_tes_bias_err is None:
                         online_iv_tes_bias_err = np.array(bias_err_array)
                     else:
                         online_iv_tes_bias_err = np.append(
                             online_iv_tes_bias_err,  bias_err_array, axis=1
                         )  
 
-
                     # analyze
                     if istep>=3:
 
                         # analyze
+                        rshunt = self._instruments_inst.get_shunt_resistance(
+                            detector_channel=self._detector_channels[0])
+                        
                         ivobj = qp.IBIS(
                             dites=online_iv_offset,
                             dites_err=online_iv_offset_err,
                             ibias=online_iv_tes_bias,
                             ibias_err=online_iv_tes_bias_err,
-                            rsh=5e-3,
-                            rsh_err=0.05*5e-3,
+                            rsh=rshunt,
+                            rsh_err=0.05*rshunt,
                             rp_guess=np.array([2e-3]*nb_channels),
                             rp_err_guess=np.zeros(nb_channels),
                             chan_names=self._detector_channels,
                             fitsc=False,
                             normalinds=list(range(3)),
                             scinds=None,
                         )
                     
                         ivobj.analyze()
                         
-
-                        # get signal gen amplitude
-                        #for  ichan in range(len(self._detector_channels)):
-                        #    r0 = ivobj.r0[0, ichan, -1]
-                        #    noise_std = online_iv_std[ichan, -1]
-                        #    print('trace_std = ' + str(noise_std))
-                        #    print('r0: ' + str(r0))
-                        #    sig_gen_current = noise_std *(r0+5e-3+2e-3)/5e-3
-                        #    sig_gen_volt = sig_gen_current*10000*1000
-                        #    print('Vsg [mV] = ' + str(sig_gen_volt))
-                                                    
-                        
                             
                 # -----------
                 # IV
                 # ----------
                 
                 if self._enable_iv:
 
-                    # set detector
-                    for channel in self._detector_channels:
+
+                    # turn SG output "off" 
+                    # If SG/TES controllers are same:
+                    #   SG will be set to DC, output on
+                  
                     
+                    for channel in self._detector_channels:
+
                         # disconnect signal generator
-                        self._instrument.set_signal_gen_onoff('off', detector_channel=channel)
+                        self._instruments_inst.set_signal_gen_onoff(
+                            'off',
+                            detector_channel=channel)
 
                         # disconnect from TES
-                        self._instrument.connect_signal_gen_to_tes(False, detector_channel=channel)
+                        self._instruments_inst.connect_signal_gen_to_tes(
+                            False,
+                            detector_channel=channel)
                         
                         # other parameters
                         if 'output_gain' in iv_config:
-                            self._instrument.set_output_gain(float(iv_config['output_gain']),
-                                                             detector_channel=channel)
+                            self._instruments_inst.set_output_gain(
+                                float(iv_config['output_gain']),
+                                detector_channel=channel)
                             
                     # wait 5 seconds
                     time.sleep(5)
                     
                     # setup ADC
                     self._daq.set_adc_config_from_dict(iv_config['adc_setup'])
                     
                     # get/set detector config metadata
                     det_config = dict()
                     adc_channel_dict = connection_utils.get_adc_channel_list(
                         self._detector_connection_table,
                         detector_channel_list=self._saved_detector_channels
                     )
-
                                      
                     for adc_name in adc_channel_dict:
-                        det_config[adc_name] = self._instrument.read_all(
+                        det_config[adc_name] = self._instruments_inst.read_all(
                             adc_id=adc_name,
                             adc_channel_list=adc_channel_dict[adc_name]
                         )
 
-                        if temperature is not None:
-                            key_temp = 'temperature'
-                            if thermometer_name  is not None:
-                                key_temp += '_' + thermometer_name.lower()
-                            elif thermometer_global_num is not None:
-                                key_temp += '_' + str(hermometer_global_num)
-                            det_config[adc_name][key_temp] = temperature
-
-                        if monitoring_temperature_list is not None:
-                            for itherm in range(len(monitoring_temperature_list)):
-                                det_config[adc_name][
-                                    'temperature_' + monitoring_thermometer_names[itherm].lower()
-                                ] = monitoring_temperature_list[itherm]
-                            
                     self._daq.set_detector_config(det_config)
                     
                     # take data
                     if self._enable_tes_bias_sweep:
-                        run_comment = 'IV: ' + ' TES bias = ' + str(bias) + 'uA'
-                        print('INFO: Starting IV data taking with TES bias = ' + str(bias) + 'uA!')
+                        run_comment = ('IV: ' + ' TES bias = '
+                                       + str(bias) + 'uA')
+                        
+                        print('INFO: Starting IV data taking with TES bias = '
+                              + str(bias) + 'uA!')
                     else:
                         run_comment = 'IV (bias sweep disabled)'
                         print('INFO: Starting IV data taking (bias sweep disabled)!')
 
                     if self._enable_temperature_sweep:
-                        run_comment = run_comment + ', T = ' + str(temperature) + 'mK'
+                        run_comment = (run_comment + ', T = '
+                                       + str(temperature) + 'mK')
                         
                     success = self._daq.run(run_time=int(iv_config['run_time']),
                                             run_type=102,
                                             run_comment=run_comment,
                                             group_name=self._group_name,
                                             group_comment=self._comment,
                                             data_path=self._raw_data_path,
                                             data_prefix='iv')
 
                     if not success:
                         print('ERROR taking data! Stopping sequencer')
                         return False
 
-
-                                
                 # -----------
                 # dIdV
                 # ----------
                 
                 if self._enable_didv:
 
 
                     # ADC setup
                     self._daq.set_adc_config_from_dict(didv_config['adc_setup'])
-                    
-
+                                                                              
                     # set detector
                     for channel in self._detector_channels:
-                    
-                        # signal generator
+
+                        # turn on signal gen output
+                        # if SG same as TES controller, set shape "square"
+                        self._instruments_inst.set_signal_gen_onoff(
+                            'on', detector_channel=channel
+                        )
                         
-                        self._instrument.set_signal_gen_params(
-                            detector_channel=channel,source='tes', 
+                        self._instruments_inst.set_signal_gen_params(
+                            detector_channel=channel,
+                            source='tes', 
                             voltage=didv_config['signal_gen_voltage'],
+                            voltage_unit='mV',
                             current=didv_config['signal_gen_current'],
+                            current_unit='uA',
                             frequency=didv_config['signal_gen_frequency'],
+                            frequency_unit='Hz',
                             shape='square'
                         )
-
-
-                    
-                        self._instrument.set_signal_gen_onoff('on', detector_channel=channel)
-
+                   
                         # connect to TES
-                        self._instrument.connect_signal_gen_to_tes(True, detector_channel=channel)
+                        self._instruments_inst.connect_signal_gen_to_tes(
+                            True, detector_channel=channel)
 
-                        
                         # other parameters
                         if 'output_gain' in didv_config:
-                            self._instrument.set_output_gain(float(didv_config['output_gain']),
-                                                             detector_channel=channel)
+                            self._instruments_inst.set_output_gain(
+                                float(didv_config['output_gain']),
+                                detector_channel=channel)
                             
                         # wait 5 seconds
                         time.sleep(5)
                     
                         
                         if didv_config['loop_channels']:
                                                 
                             # get/set detector config metadata
                             det_config = dict()
-                            adc_channel_dict = connection_utils.get_adc_channel_list(
-                                self._detector_connection_table,
-                                detector_channel_list=self._saved_detector_channels
+                            adc_channel_dict = (
+                                connection_utils.get_adc_channel_list(
+                                    self._detector_connection_table,
+                                    detector_channel_list=self._saved_detector_channels
+                                )
                             )
                             
                             for adc_name in adc_channel_dict:
-                                det_config[adc_name] = self._instrument.read_all(
-                                    adc_id=adc_name,
-                                    adc_channel_list=adc_channel_dict[adc_name]
-                                )
                                 
-
-                                if temperature is not None:
-                                    key_temp = 'temperature'
-                                    if thermometer_name  is not None:
-                                        key_temp += '_' + thermometer_name.lower()
-                                    elif thermometer_global_num is not None:
-                                        key_temp += '_' + str(hermometer_global_num)
-                                    det_config[adc_name][key_temp] = temperature
-
-                                if monitoring_temperature_list is not None:
-                                    for itherm in range(len(monitoring_temperature_list)):
-                                        det_config[adc_name][
-                                            'temperature_' + monitoring_thermometer_names[itherm].lower()
-                                        ] = monitoring_temperature_list[itherm]
+                                det_config[adc_name] = (
+                                    self._instruments_inst.read_all(
+                                        adc_id=adc_name,
+                                        adc_channel_list=adc_channel_dict[adc_name]
+                                    )
+                                )
                             
                             self._daq.set_detector_config(det_config)
-
                     
                             # take data
-                            run_comment = ('dIdV chan ' + str(channel) + ': TES bias = '
+                            run_comment = ('dIdV chan ' + str(channel)
+                                           + ': TES bias = '
                                            + str(bias) + 'uA')
                          
                             if self._enable_tes_bias_sweep:
                                 run_comment = ('dIdV chan ' + str(channel)
                                                + ': TES bias = ' + str(bias) + 'uA')
                                 print('INFO: Starting dIdV data taking for channel '
                                       + str(channel)
@@ -734,85 +762,78 @@
                                 run_comment = ('dIdV chan ' + str(channel)
                                                + ' (bias sweep disabled)')
                                 print('INFO: Starting dIdV data taking for channel '
                                       + str(channel)
                                       + ' (bias sweep disabled)')
 
                             if self._enable_temperature_sweep:
-                                run_comment = run_comment + ', T = ' + str(temperature) + 'mK'
+                                run_comment = (run_comment + ', T = '
+                                               + str(temperature) + 'mK')
 
                               
-                            success = self._daq.run(run_time=int(didv_config['run_time']),
-                                                    run_type=103,
-                                                    run_comment=run_comment,
-                                                    group_name=self._group_name,
-                                                    group_comment=self._comment,
-                                                    data_path=self._raw_data_path,
-                                                    data_prefix='didv')
+                            success = self._daq.run(
+                                run_time=int(didv_config['run_time']),
+                                run_type=103,
+                                run_comment=run_comment,
+                                group_name=self._group_name,
+                                group_comment=self._comment,
+                                data_path=self._raw_data_path,
+                                data_prefix='didv')
                            
                             if not success:
                                 print('ERROR taking data! Stopping sequencer')
                                 return False
                      
                             # turn off signal genrator
-                            self._instrument.connect_signal_gen_to_tes(False, detector_channel=channel)
+                            self._instruments_inst.connect_signal_gen_to_tes(
+                                False, detector_channel=channel)
                             
                          
 
                     # take data (if all channels)
                     if not didv_config['loop_channels']:
  
                         # get/set detector config metadata
                         det_config = dict()
                         adc_channel_dict= connection_utils.get_adc_channel_list(
                             self._detector_connection_table,
                             detector_channel_list=self._saved_detector_channels
                         )
 
                         for adc_name in adc_channel_dict:
-                            det_config[adc_name] = self._instrument.read_all(
+                            det_config[adc_name] = self._instruments_inst.read_all(
                                 adc_id=adc_name,
                                 adc_channel_list=adc_channel_dict[adc_name]
                             )
-
-                            if temperature is not None:
-                                key_temp = 'temperature'
-                                if thermometer_name  is not None:
-                                    key_temp += '_' + thermometer_name.lower()
-                                elif thermometer_global_num is not None:
-                                    key_temp += '_' + str(hermometer_global_num)
-                                det_config[adc_name][key_temp] = temperature
-
-                            if monitoring_temperature_list is not None:
-                                for itherm in range(len(monitoring_temperature_list)):
-                                    det_config[adc_name][
-                                        'temperature_' + monitoring_thermometer_names[itherm].lower()
-                                    ] = monitoring_temperature_list[itherm]
                                                               
                         self._daq.set_detector_config(det_config)
 
 
                         # start run
                         if self._enable_tes_bias_sweep:
-                            run_comment = 'dIdV: ' + ' TES bias = ' + str(bias) + 'uA'
-                            print('INFO: Starting IV data taking with TES bias = ' + str(bias) + 'uA!')
+                            run_comment = ('dIdV: ' + ' TES bias = '
+                                           + str(bias) + 'uA')
+                            print('INFO: Starting IV data taking with TES bias = '
+                                  + str(bias) + 'uA!')
                         else:
                             run_comment = 'dIdV (bias sweep disabled)'
                             print('INFO: Starting dIdV data taking (bias sweep disabled)!')
 
                         if self._enable_temperature_sweep:
-                            run_comment = run_comment + ', T = ' + str(temperature) + 'mK'
+                            run_comment = (run_comment + ', T = '
+                                           + str(temperature) + 'mK')
                       
-                        success = self._daq.run(run_time=int(didv_config['run_time']),
-                                                run_type=103,
-                                                run_comment=run_comment,
-                                                group_name=self._group_name,
-                                                group_comment=self._comment,
-                                                data_path=self._raw_data_path,
-                                                data_prefix='didv')
+                        success = self._daq.run(
+                            run_time=int(didv_config['run_time']),
+                            run_type=103,
+                            run_comment=run_comment,
+                            group_name=self._group_name,
+                            group_comment=self._comment,
+                            data_path=self._raw_data_path,
+                            data_prefix='didv')
 
                         if not success:
                             print('ERROR taking data! Stopping sequencer')
                             return False
                             
             self._daq.clear()
 
@@ -823,54 +844,52 @@
             
             print('INFO: Making IV diagnostic plots!')
 
             diagnostic_path = self._raw_data_path + '/diagnostic/'
             arg_utils.make_directories(diagnostic_path)
                     
             now = datetime.now()
-            series_date = now.strftime('%Y') +  now.strftime('%m') + now.strftime('%d') 
-            series_time = now.strftime('%H') + now.strftime('%M') +  now.strftime('%S')
+            series_date = (now.strftime('%Y') +  now.strftime('%m')
+                           + now.strftime('%d'))
+            series_time = (now.strftime('%H') + now.strftime('%M')
+                           + now.strftime('%S'))
+            
             savename = series_date + '_' + series_time
                       
             ivobj.plot_all_curves(showfit=True, lgcsave=True,
                                   savepath=diagnostic_path,
                                   savename=savename)
              
 
         # set heater back to 0%?
         if self._enable_temperature_sweep:
             print('INFO: setting heater back to 0!')
-            self._instrument.set_temperature(
+            self._instruments_inst.set_temperature(
                 0,
                 channel_name=thermometer_name,
                 global_channel_number=thermometer_global_num,
                 heater_channel_name=heater_name,
                 heater_global_channel_number=heater_global_num,
                 wait_temperature_reached=False)
             
             
 
         if self._verbose:
             print('IV/dIdV successfully finished!')
 
       
-
-
-
-
-
     def _run_rp_rn(self):
         """
         Measure Rp/Rn
         """
 
-        if self._daq is None or self._instrument is None:
+        if self._daq is None or self._instruments_inst is None:
             print('WARNING: daq or instrument has not been instanciated!')
             self._daq = None
-            self._instrument = None
+            self._instruments_inst = None
             return
 
 
         # measurement list
         measurement_list = list()
         if self._enable_rp:
             measurement_list.append('Rp')
@@ -893,27 +912,29 @@
             # configuration
             config_dict = self._measurement_config[measurement.lower()]
            
             # initialize detector
             for channel in self._detector_channels:
                 
                 # QET bias
-                self._instrument.set_tes_bias(config_dict['tes_bias'],
-                                              detector_channel=channel)
+                self._instruments_inst.set_tes_bias(
+                    config_dict['tes_bias'], unit='uA',
+                    detector_channel=channel)
                 
                 # Other detector settings
                 if 'output_gain' in config_dict:
-                    self._instrument.set_output_gain(float(config_dict['output_gain']),
-                                                     detector_channel=channel)
+                    self._instruments_inst.set_output_gain(
+                        float(config_dict['output_gain']),
+                        detector_channel=channel)
                          
 
-
                 #  turn off signal generator (avoid cross talk)
-                self._instrument.set_signal_gen_onoff('off', detector_channel=channel)
-                          
+                self._instruments_inst.set_signal_gen_onoff(
+                    'off', detector_channel=channel)
+                                           
                 # Eventually close loop, relock, zero once, etc. 
                 
 
             
             # wait 5 seconds
             time.sleep(5)
 
@@ -921,78 +942,86 @@
             self._daq.set_adc_config_from_dict(config_dict['adc_setup'])
             
             # connect signal gen and take data
             run_comment = measurement + ' measurement'
             run_type = 100
             if measurement=='Rn':
                 run_type = 101
-                
+
             for channel in self._detector_channels:
-                
-                
+                                     
                 # signal generator
-                self._instrument.set_signal_gen_params(detector_channel=channel,
-                                                       source='tes', 
-                                                       voltage=didv_config['signal_gen_voltage'],
-                                                       current=didv_config['signal_gen_current'],
-                                                       frequency=didv_config['signal_gen_frequency'],
-                                                       shape='square')
-            
-                self._instrument.set_signal_gen_onoff('on', detector_channel=channel)
+                self._instruments_inst.set_signal_gen_onoff(
+                    'on', detector_channel=channel)
+                
+                self._instruments_inst.set_signal_gen_params(
+                    detector_channel=channel,
+                    source='tes', 
+                    voltage=didv_config['signal_gen_voltage'],
+                    voltage_unit='mV',
+                    current=didv_config['signal_gen_current'],
+                    current_unit='uA',
+                    frequency=didv_config['signal_gen_frequency'],
+                    frequency_unit='Hz',
+                    shape='square')
+                           
                 time.sleep(2)
 
                
                 # take data
                 if config_dict['loop_channels']:
 
                     # read and store detector settings
                     det_config = dict()
                     adc_channel_dict = connection_utils.get_adc_channel_list(
                         self._detector_connection_table,
                         detector_channel_list=self._detector_channels
                     )
                     
                     for adc_name in adc_channel_dict:
-                        det_config[adc_name] = self._instrument.read_all(
+                        det_config[adc_name] = self._instruments_inst.read_all(
                             adc_id=adc_name,
                             adc_channel_list=adc_channel_dict[adc_name]
                         )
 
                     self._daq.set_detector_config(det_config)
                  
 
                     # take data
-                    success = self._daq.run(run_time=int(config_dict['run_time']),
-                                            run_type=run_type,
-                                            run_comment=run_comment,
-                                            group_name=self._group_name,
-                                            group_comment=self._comment,
-                                            data_path=self._raw_data_path,
-                                            data_prefix=measurement.lower())
+                    success = self._daq.run(
+                        run_time=int(config_dict['run_time']),
+                        run_type=run_type,
+                        run_comment=run_comment,
+                        group_name=self._group_name,
+                        group_comment=self._comment,
+                        data_path=self._raw_data_path,
+                        data_prefix=measurement.lower())
+                    
                     if not success:
                         print('ERROR taking data! Stopping sequencer')
                         return False
                       
                     # disconnect
-                    self._instrument.set_signal_gen_onoff('off', detector_channel=channel)
-                    
-
-
+                    if not is_tes_signa_gen_common:
+                        self._instruments_inst.set_signal_gen_onoff(
+                            'off',
+                            detector_channel=channel)
+                 
             # take data (case all channels together)
             if not config_dict['loop_channels']:
 
                 # read and store detector settings
                 det_config = dict()
                 adc_channel_dict= connection_utils.get_adc_channel_list(
                     self._detector_connection_table,
                     detector_channel_list=self._detector_channels
                 )
 
                 for adc_name in adc_channel_dict:
-                    det_config[adc_name] = self._instrument.read_all(
+                    det_config[adc_name] = self._instruments_inst.read_all(
                         adc_id=adc_name,
                         adc_channel_list=adc_channel_dict[adc_name]
                     )
                     
                 self._daq.set_detector_config(det_config)
                                  
                 # take data
@@ -1005,39 +1034,32 @@
                                         data_prefix=measurement.lower())
                 
                 if not success:
                     print('ERROR taking data! Stopping sequencer')
                     return False
                                 
 
-   
-
-
     def _configure(self):
         """
         Configure IV/dIdV/Rp/Rn measurements
         """
-
-
         #  IV / dIdV:  TES sweep parameters
         if self._enable_iv or self._enable_didv:
 
             config_dict = self._measurement_config['iv_didv']
          
             # Build TES bias vector
             tes_bias_vect = []
             temperature_vect = []
             if config_dict['use_tes_bias_vect']: 
                 if not config_dict['tes_bias_vect']:
                     raise ValueError('IV/dIdV sweep required bias vector if "use_tes_bias_vect" = true!')
                 else:
                     tes_bias_vect = [float(bias) for bias in config_dict['tes_bias_vect']]
-                    tes_bias_vect = np.unique(np.asarray(tes_bias_vect))
-                    tes_bias_vect = tes_bias_vect[::-1]
-             
+                    tes_bias_vect = np.asarray(tes_bias_vect)
             else:
                 required_parameter = ['use_negative_tes_bias',
                                       'tes_bias_min','tes_bias_max','tes_bias_step_n',
                                       'tes_bias_step_t','tes_bias_t']
 
                 for key in required_parameter:
                     if key not in config_dict:
```

### Comparing `pytesdaq-0.3.9/pytesdaq/sequencer/sequencer.py` & `pytesdaq-0.4.0/pytesdaq/sequencer/sequencer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numpy as np
 import time
 from datetime import datetime
 import os
 import shutil
 import stat
-
-
+import copy
 import pytesdaq.config.settings as settings
 import pytesdaq.instruments.control as instrument
 from pytesdaq.utils import connection_utils
 from pytesdaq.utils import arg_utils
 from pytesdaq.daq import daq
 
 class Sequencer:
@@ -101,17 +100,15 @@
                self._redis_db.connect()
                
           
           # Initialize daq / instrument
           self._daq = None
           self._instrument = None
                
-               
-
-
+  
      @property
      def verbose(self):
           return self._verbose
           
      @verbose.setter
      def verbose(self,value):
           self._verbose=value
@@ -153,15 +150,15 @@
           # data path
           data_path = self._config.get_data_path()
           
           # append run#
           self._fridge_run = self._config.get_fridge_run()
           fridge_run_name = 'run' + str(self._fridge_run)
           if data_path.find(fridge_run_name)==-1:
-               data_path += '/' + fridge_run_name
+               data_path += ('/' + fridge_run_name)
           self._base_raw_data_path =  data_path + '/raw'
           self._base_automation_data_path  =  data_path + '/automation'
           arg_utils.make_directories([data_path, self._base_raw_data_path,
                                       self._base_automation_data_path])
 
           
           # channels
@@ -225,23 +222,23 @@
           # add or replace parameter from measurement_config
           required_parameters = ['sample_rate','voltage_min','voltage_max']
           required_parameters_didv = ['signal_gen_frequency', 'signal_gen_shape']
           if self._config.get_signal_generator()=='magnicon':
                required_parameters_didv.append('signal_gen_current')
           else:
                required_parameters_didv.append('signal_gen_voltage')
-          
-        
-
+    
           # loop measurements
           for measurement in  self._measurement_list:
+
+                # copy adc_dict
+               adc_dict_meas = copy.deepcopy(adc_dict)
                
                # measurement config
                config_dict = self._measurement_config[measurement]
-
                
                # dIdV flag
                is_didv_used = (measurement != 'iv'
                                and  measurement != 'noise')
 
                # check dIdV parameters
                if is_didv_used:
@@ -252,19 +249,19 @@
                          if item not in config_dict:
                               raise ValueError(measurement
                                                + ' measurement require '
                                                + str(item)
                                                + '! Please check configuration')
                          
                # ADC parameters
-               for adc_id in adc_dict:
-                    for item,value in adc_dict[adc_id].items():
+               for adc_id in adc_dict_meas:
+                    for item,value in adc_dict_meas[adc_id].items():
                          if item in config_dict:
                               value = config_dict[item]
-                              adc_dict[adc_id][item] = value
+                              adc_dict_meas[adc_id][item] = value
 
                     # calculate number of samples (dIdV fit)
                     nb_samples = 0
                     sample_rate = int(config_dict['sample_rate'])
                     if (is_didv_used and 'nb_cycles' in config_dict):
                          signal_gen_freq = float(config_dict['signal_gen_frequency'])
                          nb_samples= round(
@@ -273,34 +270,33 @@
                     elif 'trace_length_ms' in config_dict:
                          nb_samples= round(float(config_dict['trace_length_ms'])*sample_rate/1000)
                     elif 'trace_length_adc' in config_dict:
                          nb_samples = int(config_dict['trace_length_adc'])
                     else:
                          raise ValueError('Nb of cycles or trace length required for "'
                                           + measurement + '" measurement!')
-                    
-
+                 
                     # trigger
                     trigger_type = 1
                     if is_didv_used:
                          trigger_type = 2
                
                     # add parameters
-                    for adc_id in adc_dict:
-                         adc_dict[adc_id]['nb_samples'] = int(nb_samples)
-                         adc_dict[adc_id]['trigger_type'] =  trigger_type
+                    for adc_id in adc_dict_meas:
+                         adc_dict_meas[adc_id]['nb_samples'] = int(nb_samples)
+                         adc_dict_meas[adc_id]['trigger_type'] =  trigger_type
                          if trigger_type==2:
                               trigger_channel = '/Dev1/pfi0'
-                              if ('device_name' in adc_dict[adc_id] and 
-                                  'trigger_channel' in  adc_dict[adc_id]):
-                                   trigger_channel = '/' + adc_dict[adc_id]['device_name'] + '/' 
-                                   trigger_channel += adc_dict[adc_id]['trigger_channel']
-                              adc_dict[adc_id]['trigger_channel'] = trigger_channel
+                              if ('device_name' in adc_dict_meas[adc_id] and 
+                                  'trigger_channel' in  adc_dict_meas[adc_id]):
+                                   trigger_channel = '/' + adc_dict_meas[adc_id]['device_name'] + '/' 
+                                   trigger_channel += adc_dict_meas[adc_id]['trigger_channel']
+                              adc_dict_meas[adc_id]['trigger_channel'] = trigger_channel
 
-               self._measurement_config[measurement]['adc_setup'] = adc_dict
+               self._measurement_config[measurement]['adc_setup'] = adc_dict_meas
 
                          
                          
 
      def _read_pickle(self):
           print('Reading pickle -> Not implemented...')
```

### Comparing `pytesdaq-0.3.9/pytesdaq/sequencer/tc.py` & `pytesdaq-0.4.0/pytesdaq/sequencer/tc.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.9/pytesdaq/utils/arg_utils.py` & `pytesdaq-0.4.0/pytesdaq/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.9/pytesdaq/utils/connection_utils.py` & `pytesdaq-0.4.0/pytesdaq/utils/connection_utils.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.9/pytesdaq/utils/remote.py` & `pytesdaq-0.4.0/pytesdaq/utils/remote.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.9/pytesdaq.egg-info/PKG-INFO` & `pytesdaq-0.4.0/pytesdaq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytesdaq
-Version: 0.3.9
+Version: 0.4.0
 Summary: DAQ and Intruments control for TES development
 Home-page: https://github.com/spice-herald/pytesdaq
 Author: Bruno Serfass
 Author-email: serfass@berkeley.edu
 Description-Content-Type: text/markdown
 Requires-Dist: PyQt5
 Requires-Dist: matplotlib
```

### Comparing `pytesdaq-0.3.9/pytesdaq.egg-info/SOURCES.txt` & `pytesdaq-0.4.0/pytesdaq.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,40 +9,43 @@
 pytesdaq.egg-info/top_level.txt
 pytesdaq/analyzer/__init__.py
 pytesdaq/analyzer/analyzer.py
 pytesdaq/config/__init__.py
 pytesdaq/config/settings.py
 pytesdaq/daq/__init__.py
 pytesdaq/daq/daq.py
+pytesdaq/daq/daqcontrol.py
 pytesdaq/daq/nidaqtask.py
 pytesdaq/daq/polaris.py
 pytesdaq/display/__init__.py
 pytesdaq/display/series.py
 pytesdaq/instruments/__init__.py
 pytesdaq/instruments/communication.py
 pytesdaq/instruments/control.py
+pytesdaq/instruments/agilent/__init__.py
+pytesdaq/instruments/agilent/agilent33500B.py
 pytesdaq/instruments/feb/__init__.py
 pytesdaq/instruments/feb/feb.py
 pytesdaq/instruments/imacrt/__init__.py
 pytesdaq/instruments/imacrt/imacrt.py
 pytesdaq/instruments/imacrt/macrtmodule.py
+pytesdaq/instruments/keithley/__init__.py
+pytesdaq/instruments/keithley/keithley2400.py
 pytesdaq/instruments/keysight/__init__.py
-pytesdaq/instruments/keysight/keysight.py
+pytesdaq/instruments/keysight/keysightDSOX1200.py
 pytesdaq/instruments/lakeshore/__init__.py
 pytesdaq/instruments/lakeshore/lakeshore.py
 pytesdaq/instruments/magnicon/__init__.py
 pytesdaq/instruments/magnicon/magnicon.py
 pytesdaq/instruments/niadc/__init__.py
 pytesdaq/instruments/niadc/nidevice.py
 pytesdaq/io/__init__.py
 pytesdaq/io/filter_hdf5.py
 pytesdaq/io/hdf5.py
 pytesdaq/io/redis.py
-pytesdaq/processing/__init__.py
-pytesdaq/processing/trigger.py
 pytesdaq/scope/__init__.py
 pytesdaq/scope/readout.py
 pytesdaq/scope/scope.py
 pytesdaq/sequencer/__init__.py
 pytesdaq/sequencer/iv_didv.py
 pytesdaq/sequencer/sequencer.py
 pytesdaq/sequencer/tc.py
```

### Comparing `pytesdaq-0.3.9/setup.py` & `pytesdaq-0.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
       long_description = f.read()
 
 
 setup(name='pytesdaq',
-      version='0.3.9',
+      version='0.4.0',
       description='DAQ and Intruments control for TES development',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Bruno Serfass',
       author_email='serfass@berkeley.edu',
       url="https://github.com/spice-herald/pytesdaq",
       zip_safe = False,
```

