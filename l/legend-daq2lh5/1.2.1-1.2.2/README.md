# Comparing `tmp/legend_daq2lh5-1.2.1.tar.gz` & `tmp/legend_daq2lh5-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legend_daq2lh5-1.2.1.tar", last modified: Mon Apr 15 09:03:18 2024, max compression
+gzip compressed data, was "legend_daq2lh5-1.2.2.tar", last modified: Wed May  8 13:40:02 2024, max compression
```

## Comparing `legend_daq2lh5-1.2.1.tar` & `legend_daq2lh5-1.2.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.125933 legend_daq2lh5-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-15 09:03:18.125933 legend_daq2lh5-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-15 09:03:18.125933 legend_daq2lh5-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.109933 legend_daq2lh5-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.113933 legend_daq2lh5-1.2.1/src/daq2lh5/
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 09:03:18.000000 legend_daq2lh5-1.2.1/src/daq2lh5/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.113933 legend_daq2lh5-1.2.1/src/daq2lh5/buffer_processor/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/buffer_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/buffer_processor/buffer_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/buffer_processor/lh5_buffer_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/build_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.113933 legend_daq2lh5-1.2.1/src/daq2lh5/compass/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/compass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_header_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_streamer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10672 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/data_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/data_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.113933 legend_daq2lh5-1.2.1/src/daq2lh5/fc/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/fc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_config_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_status_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_streamer.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.117933 legend_daq2lh5-1.2.1/src/daq2lh5/orca/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    20867 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_digitizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    33096 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_flashcam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_header_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_packet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_run_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15693 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_streamer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17688 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/raw_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.121933 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-15 09:03:18.000000 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-15 09:03:18.000000 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:03:18.000000 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-15 09:03:18.000000 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:03:17.000000 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-15 09:03:18.000000 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 09:03:18.000000 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.117933 legend_daq2lh5-1.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.121933 legend_daq2lh5-1.2.1/tests/buffer_processor/
--rw-r--r--   0 runner    (1001) docker     (127)    55148 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.121933 legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor_configs/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor_configs/raw_out_spec_no_proc.json
--rw-r--r--   0 runner    (1001) docker     (127)    43754 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/buffer_processor/test_lh5_buffer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.121933 legend_daq2lh5-1.2.1/tests/compass/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/compass/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/compass/test_compass_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/compass/test_compass_header_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/compass/test_compass_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.121933 legend_daq2lh5-1.2.1/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/configs/fc-out-spec.json
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/configs/orca-out-spec-cli.json
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/configs/orca-out-spec.json
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.121933 legend_daq2lh5-1.2.1/tests/fc/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/fc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/fc/test_fc_config_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/fc/test_fc_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/fc/test_fc_status_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/fc/test_fc_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.121933 legend_daq2lh5-1.2.1/tests/orca/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/orca/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/orca/test_or_run_decoder_for_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/orca/test_orca_fc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/orca/test_orca_packet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/test_build_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/test_daq_to_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/test_raw_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:02.600221 legend_daq2lh5-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-08 13:40:02.600221 legend_daq2lh5-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-08 13:40:02.600221 legend_daq2lh5-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:02.588221 legend_daq2lh5-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:02.592221 legend_daq2lh5-1.2.2/src/daq2lh5/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 13:40:02.000000 legend_daq2lh5-1.2.2/src/daq2lh5/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:02.592221 legend_daq2lh5-1.2.2/src/daq2lh5/buffer_processor/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/buffer_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/buffer_processor/buffer_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/buffer_processor/lh5_buffer_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/build_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:02.592221 legend_daq2lh5-1.2.2/src/daq2lh5/compass/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/compass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/compass/compass_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/compass/compass_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/compass/compass_header_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/compass/compass_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10677 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/data_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/data_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:02.592221 legend_daq2lh5-1.2.2/src/daq2lh5/fc/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/fc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/fc/fc_config_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/fc/fc_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/fc/fc_status_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/fc/fc_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:02.596221 legend_daq2lh5-1.2.2/src/daq2lh5/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20867 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_digitizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33096 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_flashcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_header_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_run_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15693 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17688 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/src/daq2lh5/raw_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:02.600221 legend_daq2lh5-1.2.2/src/legend_daq2lh5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-08 13:40:02.000000 legend_daq2lh5-1.2.2/src/legend_daq2lh5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-08 13:40:02.000000 legend_daq2lh5-1.2.2/src/legend_daq2lh5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:40:02.000000 legend_daq2lh5-1.2.2/src/legend_daq2lh5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 13:40:02.000000 legend_daq2lh5-1.2.2/src/legend_daq2lh5.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:40:02.000000 legend_daq2lh5-1.2.2/src/legend_daq2lh5.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-08 13:40:02.000000 legend_daq2lh5-1.2.2/src/legend_daq2lh5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 13:40:02.000000 legend_daq2lh5-1.2.2/src/legend_daq2lh5.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:02.596221 legend_daq2lh5-1.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:02.596221 legend_daq2lh5-1.2.2/tests/buffer_processor/
+-rw-r--r--   0 runner    (1001) docker     (127)    55148 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/buffer_processor/test_buffer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:02.596221 legend_daq2lh5-1.2.2/tests/buffer_processor/test_buffer_processor_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/buffer_processor/test_buffer_processor_configs/raw_out_spec_no_proc.json
+-rw-r--r--   0 runner    (1001) docker     (127)    43754 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/buffer_processor/test_lh5_buffer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:02.600221 legend_daq2lh5-1.2.2/tests/compass/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/compass/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/compass/test_compass_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/compass/test_compass_header_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/compass/test_compass_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:02.600221 legend_daq2lh5-1.2.2/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/configs/fc-out-spec.json
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/configs/orca-out-spec-cli.json
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/configs/orca-out-spec.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:02.600221 legend_daq2lh5-1.2.2/tests/fc/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/fc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/fc/test_fc_config_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/fc/test_fc_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/fc/test_fc_status_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/fc/test_fc_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:40:02.600221 legend_daq2lh5-1.2.2/tests/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/orca/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/orca/test_or_run_decoder_for_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/orca/test_orca_fc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/orca/test_orca_packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/test_build_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/test_daq_to_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-08 13:39:56.000000 legend_daq2lh5-1.2.2/tests/test_raw_buffer.py
```

### Comparing `legend_daq2lh5-1.2.1/LICENSE` & `legend_daq2lh5-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/PKG-INFO` & `legend_daq2lh5-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_daq2lh5
-Version: 1.2.1
+Version: 1.2.2
 Summary: Convert digitizer data to LH5
 Home-page: https://github.com/legend-exp/legend-daq2lh5
 Author: Jason Detwiler
 Author-email: jasondet@uw.edu
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `legend_daq2lh5-1.2.1/README.md` & `legend_daq2lh5-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/setup.cfg` & `legend_daq2lh5-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/__init__.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/__init__.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/buffer_processor/buffer_processor.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/buffer_processor/buffer_processor.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/buffer_processor/lh5_buffer_processor.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/buffer_processor/lh5_buffer_processor.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/build_raw.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/build_raw.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/cli.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/cli.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_config_parser.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/compass/compass_config_parser.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_event_decoder.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/compass/compass_event_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_header_decoder.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/compass/compass_header_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_streamer.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/compass/compass_streamer.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/data_decoder.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/data_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     found, call :meth:`.put_in_garbage`. User should set up an enum or bitbank
     of garbage codes to be stored along with the garbage packets.
     """
 
     def __init__(
         self, garbage_length: int = 256, packet_size_guess: int = 1024
     ) -> None:
-        self.garbage_table = lgdo.Table(garbage_length)
+        self.garbage_table = lgdo.Table(size=garbage_length)
         shape_guess = (garbage_length, packet_size_guess)
         self.garbage_table.add_field(
             "packets", lgdo.VectorOfVectors(shape_guess=shape_guess, dtype="uint8")
         )
         self.garbage_table.add_field(
             "packet_id", lgdo.Array(shape=garbage_length, dtype="uint32")
         )
```

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/data_streamer.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/data_streamer.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_config_decoder.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/fc/fc_config_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_event_decoder.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/fc/fc_event_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_status_decoder.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/fc/fc_status_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_streamer.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/fc/fc_streamer.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/logging.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/logging.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_base.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_base.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_digitizers.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_digitizers.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_flashcam.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_flashcam.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_header.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_header.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_header_decoder.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_header_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_packet.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_packet.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_run_decoder.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_run_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_streamer.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/orca/orca_streamer.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/daq2lh5/raw_buffer.py` & `legend_daq2lh5-1.2.2/src/daq2lh5/raw_buffer.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/PKG-INFO` & `legend_daq2lh5-1.2.2/src/legend_daq2lh5.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_daq2lh5
-Version: 1.2.1
+Version: 1.2.2
 Summary: Convert digitizer data to LH5
 Home-page: https://github.com/legend-exp/legend-daq2lh5
 Author: Jason Detwiler
 Author-email: jasondet@uw.edu
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/SOURCES.txt` & `legend_daq2lh5-1.2.2/src/legend_daq2lh5.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor.py` & `legend_daq2lh5-1.2.2/tests/buffer_processor/test_buffer_processor.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json` & `legend_daq2lh5-1.2.2/tests/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json` & `legend_daq2lh5-1.2.2/tests/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/buffer_processor/test_lh5_buffer_processor.py` & `legend_daq2lh5-1.2.2/tests/buffer_processor/test_lh5_buffer_processor.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/compass/conftest.py` & `legend_daq2lh5-1.2.2/tests/compass/conftest.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/compass/test_compass_event_decoder.py` & `legend_daq2lh5-1.2.2/tests/compass/test_compass_event_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/compass/test_compass_header_decoder.py` & `legend_daq2lh5-1.2.2/tests/compass/test_compass_header_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/compass/test_compass_streamer.py` & `legend_daq2lh5-1.2.2/tests/compass/test_compass_streamer.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/conftest.py` & `legend_daq2lh5-1.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/fc/test_fc_config_decoder.py` & `legend_daq2lh5-1.2.2/tests/fc/test_fc_config_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/fc/test_fc_event_decoder.py` & `legend_daq2lh5-1.2.2/tests/fc/test_fc_event_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/fc/test_fc_status_decoder.py` & `legend_daq2lh5-1.2.2/tests/fc/test_fc_status_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/fc/test_fc_streamer.py` & `legend_daq2lh5-1.2.2/tests/fc/test_fc_streamer.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/orca/test_or_run_decoder_for_run.py` & `legend_daq2lh5-1.2.2/tests/orca/test_or_run_decoder_for_run.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/orca/test_orca_fc.py` & `legend_daq2lh5-1.2.2/tests/orca/test_orca_fc.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/orca/test_orca_packet.py` & `legend_daq2lh5-1.2.2/tests/orca/test_orca_packet.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/test_build_raw.py` & `legend_daq2lh5-1.2.2/tests/test_build_raw.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/test_cli.py` & `legend_daq2lh5-1.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/test_daq_to_raw.py` & `legend_daq2lh5-1.2.2/tests/test_daq_to_raw.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.1/tests/test_raw_buffer.py` & `legend_daq2lh5-1.2.2/tests/test_raw_buffer.py`

 * *Files identical despite different names*

