# Comparing `tmp/jaeger-1.7.0.tar.gz` & `tmp/jaeger-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaeger-1.7.0.tar", max compression
+gzip compressed data, was "jaeger-1.7.1.tar", max compression
```

## Comparing `jaeger-1.7.0.tar` & `jaeger-1.7.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1504 2024-04-29 22:17:03.934525 jaeger-1.7.0/LICENSE.md
--rw-r--r--   0        0        0     2393 2024-04-29 22:17:03.934525 jaeger-1.7.0/README.md
--rw-r--r--   0        0        0     3612 2024-04-29 22:17:03.934525 jaeger-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     1764 2024-04-29 22:17:03.934525 jaeger-1.7.0/src/jaeger/__init__.py
--rw-r--r--   0        0        0    20331 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/__main__.py
--rw-r--r--   0        0        0       61 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/__init__.py
--rw-r--r--   0        0        0     5033 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/actor.py
--rw-r--r--   0        0        0      816 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/__init__.py
--rw-r--r--   0        0        0     1029 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/alerts.py
--rw-r--r--   0        0        0     1182 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/can.py
--rw-r--r--   0        0        0     3381 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/chiller.py
--rw-r--r--   0        0        0    35363 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/configuration.py
--rw-r--r--   0        0        0      722 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/debug.py
--rw-r--r--   0        0        0     2690 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/disable.py
--rw-r--r--   0        0        0    15119 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/fvc.py
--rw-r--r--   0        0        0    11373 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/home.py
--rw-r--r--   0        0        0     5314 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/ieb.py
--rw-r--r--   0        0        0     1410 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/pollers.py
--rw-r--r--   0        0        0    16070 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/positioner.py
--rw-r--r--   0        0        0     9994 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/power.py
--rw-r--r--   0        0        0      990 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/snapshot.py
--rw-r--r--   0        0        0     1397 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/talk.py
--rw-r--r--   0        0        0     1034 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/testing.py
--rw-r--r--   0        0        0     3579 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/unwind.py
--rw-r--r--   0        0        0      949 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/actor/commands/version.py
--rw-r--r--   0        0        0    14065 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/alerts.py
--rw-r--r--   0        0        0    21709 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/can.py
--rw-r--r--   0        0        0     5257 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/chiller.py
--rw-r--r--   0        0        0     4054 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/commands/__init__.py
--rw-r--r--   0        0        0    22135 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/commands/base.py
--rw-r--r--   0        0        0     9010 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/commands/bootloader.py
--rw-r--r--   0        0        0    12181 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/commands/calibration.py
--rw-r--r--   0        0        0    10788 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/commands/goto.py
--rw-r--r--   0        0        0     6013 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/commands/status.py
--rw-r--r--   0        0        0    26797 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/commands/trajectory.py
--rw-r--r--   0        0        0    10030 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/etc/chiller_APO.yaml
--rw-r--r--   0        0        0     7487 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/etc/chiller_APO_variables.csv
--rw-r--r--   0        0        0     1317 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/etc/fvc.yaml
--rw-r--r--   0        0        0    10541 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/etc/ieb_APO.yaml
--rw-r--r--   0        0        0    10539 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/etc/ieb_LCO.yaml
--rw-r--r--   0        0        0     3329 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/etc/jaeger_APO.yml
--rw-r--r--   0        0        0     3302 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/etc/jaeger_LCO.yml
--rw-r--r--   0        0        0     8711 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/etc/schema.json
--rw-r--r--   0        0        0     1815 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/etc/sextants/epfl.yaml
--rw-r--r--   0        0        0     2367 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/etc/sextants/osu.yaml
--rw-r--r--   0        0        0     1512 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/etc/sextants/schema.json
--rw-r--r--   0        0        0     2364 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/etc/sextants/uw.yaml
--rw-r--r--   0        0        0     3545 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/exceptions.py
--rw-r--r--   0        0        0    52574 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/fps.py
--rw-r--r--   0        0        0    42572 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/fvc.py
--rw-r--r--   0        0        0     4518 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/ieb.py
--rw-r--r--   0        0        0      162 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/interfaces/__init__.py
--rw-r--r--   0        0        0     1142 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/interfaces/bus.py
--rw-r--r--   0        0        0     6759 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/interfaces/cannet.py
--rw-r--r--   0        0        0    12892 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/interfaces/message.py
--rw-r--r--   0        0        0     1874 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/interfaces/notifier.py
--rw-r--r--   0        0        0     1199 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/interfaces/virtual.py
--rw-r--r--   0        0        0    20177 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/kaiju.py
--rw-r--r--   0        0        0     8034 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/maskbits.py
--rw-r--r--   0        0        0     7797 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/plotting.py
--rw-r--r--   0        0        0    18121 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/positioner.py
--rw-r--r--   0        0        0        0 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/scripts/__init__.py
--rw-r--r--   0        0        0     1851 2024-04-29 22:17:03.938525 jaeger-1.7.0/src/jaeger/scripts/generate_chiller_yaml.py
--rw-r--r--   0        0        0      346 2024-04-29 22:17:03.942525 jaeger-1.7.0/src/jaeger/target/__init__.py
--rw-r--r--   0        0        0    18703 2024-04-29 22:17:03.942525 jaeger-1.7.0/src/jaeger/target/assignment.py
--rw-r--r--   0        0        0    40466 2024-04-29 22:17:03.942525 jaeger-1.7.0/src/jaeger/target/configuration.py
--rw-r--r--   0        0        0    15567 2024-04-29 22:17:03.942525 jaeger-1.7.0/src/jaeger/target/coordinates.py
--rw-r--r--   0        0        0    10095 2024-04-29 22:17:03.942525 jaeger-1.7.0/src/jaeger/target/design.py
--rw-r--r--   0        0        0     5572 2024-04-29 22:17:03.942525 jaeger-1.7.0/src/jaeger/target/schemas.py
--rw-r--r--   0        0        0    15992 2024-04-29 22:17:03.942525 jaeger-1.7.0/src/jaeger/target/tools.py
--rw-r--r--   0        0        0    15709 2024-04-29 22:17:03.942525 jaeger-1.7.0/src/jaeger/testing.py
--rw-r--r--   0        0        0       60 2024-04-29 22:17:03.942525 jaeger-1.7.0/src/jaeger/utils/__init__.py
--rw-r--r--   0        0        0     9610 2024-04-29 22:17:03.942525 jaeger-1.7.0/src/jaeger/utils/database.py
--rw-r--r--   0        0        0    14611 2024-04-29 22:17:03.942525 jaeger-1.7.0/src/jaeger/utils/helpers.py
--rw-r--r--   0        0        0     9549 2024-04-29 22:17:03.942525 jaeger-1.7.0/src/jaeger/utils/utils.py
--rw-r--r--   0        0        0     4059 1970-01-01 00:00:00.000000 jaeger-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-05-08 15:20:54.176815 jaeger-1.7.1/LICENSE.md
+-rw-r--r--   0        0        0     2393 2024-05-08 15:20:54.176815 jaeger-1.7.1/README.md
+-rw-r--r--   0        0        0     3613 2024-05-08 15:20:54.180815 jaeger-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1764 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/__init__.py
+-rw-r--r--   0        0        0    20331 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/__main__.py
+-rw-r--r--   0        0        0       61 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/__init__.py
+-rw-r--r--   0        0        0     5033 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/actor.py
+-rw-r--r--   0        0        0      816 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1029 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/alerts.py
+-rw-r--r--   0        0        0     1182 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/can.py
+-rw-r--r--   0        0        0     3381 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/chiller.py
+-rw-r--r--   0        0        0    35363 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/configuration.py
+-rw-r--r--   0        0        0      722 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/debug.py
+-rw-r--r--   0        0        0     2690 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/disable.py
+-rw-r--r--   0        0        0    15119 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/fvc.py
+-rw-r--r--   0        0        0    11373 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/home.py
+-rw-r--r--   0        0        0     5314 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/ieb.py
+-rw-r--r--   0        0        0     1410 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/pollers.py
+-rw-r--r--   0        0        0    16070 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/positioner.py
+-rw-r--r--   0        0        0     9994 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/power.py
+-rw-r--r--   0        0        0      990 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/snapshot.py
+-rw-r--r--   0        0        0     1397 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/talk.py
+-rw-r--r--   0        0        0     1034 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/testing.py
+-rw-r--r--   0        0        0     3579 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/unwind.py
+-rw-r--r--   0        0        0      949 2024-05-08 15:20:54.180815 jaeger-1.7.1/src/jaeger/actor/commands/version.py
+-rw-r--r--   0        0        0    14035 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/alerts.py
+-rw-r--r--   0        0        0    21709 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/can.py
+-rw-r--r--   0        0        0     5257 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/chiller.py
+-rw-r--r--   0        0        0     4054 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/commands/__init__.py
+-rw-r--r--   0        0        0    22135 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/commands/base.py
+-rw-r--r--   0        0        0     9010 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/commands/bootloader.py
+-rw-r--r--   0        0        0    12181 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/commands/calibration.py
+-rw-r--r--   0        0        0    10788 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/commands/goto.py
+-rw-r--r--   0        0        0     6013 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/commands/status.py
+-rw-r--r--   0        0        0    26797 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/commands/trajectory.py
+-rw-r--r--   0        0        0    10030 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/chiller_APO.yaml
+-rw-r--r--   0        0        0     7487 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/chiller_APO_variables.csv
+-rw-r--r--   0        0        0     1317 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/fvc.yaml
+-rw-r--r--   0        0        0    10541 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/ieb_APO.yaml
+-rw-r--r--   0        0        0    10539 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/ieb_LCO.yaml
+-rw-r--r--   0        0        0     3329 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/jaeger_APO.yml
+-rw-r--r--   0        0        0     3302 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/jaeger_LCO.yml
+-rw-r--r--   0        0        0     8711 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/schema.json
+-rw-r--r--   0        0        0     1815 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/sextants/epfl.yaml
+-rw-r--r--   0        0        0     2367 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/sextants/osu.yaml
+-rw-r--r--   0        0        0     1512 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/sextants/schema.json
+-rw-r--r--   0        0        0     2364 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/etc/sextants/uw.yaml
+-rw-r--r--   0        0        0     3545 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/exceptions.py
+-rw-r--r--   0        0        0    52574 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/fps.py
+-rw-r--r--   0        0        0    42572 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/fvc.py
+-rw-r--r--   0        0        0     4518 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/ieb.py
+-rw-r--r--   0        0        0      162 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/interfaces/__init__.py
+-rw-r--r--   0        0        0     1142 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/interfaces/bus.py
+-rw-r--r--   0        0        0     6759 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/interfaces/cannet.py
+-rw-r--r--   0        0        0    12892 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/interfaces/message.py
+-rw-r--r--   0        0        0     1874 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/interfaces/notifier.py
+-rw-r--r--   0        0        0     1199 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/interfaces/virtual.py
+-rw-r--r--   0        0        0    20177 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/kaiju.py
+-rw-r--r--   0        0        0     8034 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/maskbits.py
+-rw-r--r--   0        0        0     7797 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/plotting.py
+-rw-r--r--   0        0        0    18121 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/positioner.py
+-rw-r--r--   0        0        0        0 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/scripts/__init__.py
+-rw-r--r--   0        0        0     1851 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/scripts/generate_chiller_yaml.py
+-rw-r--r--   0        0        0      346 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/target/__init__.py
+-rw-r--r--   0        0        0    18703 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/target/assignment.py
+-rw-r--r--   0        0        0    40466 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/target/configuration.py
+-rw-r--r--   0        0        0    17185 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/target/coordinates.py
+-rw-r--r--   0        0        0    10095 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/target/design.py
+-rw-r--r--   0        0        0     5476 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/target/schemas.py
+-rw-r--r--   0        0        0    15992 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/target/tools.py
+-rw-r--r--   0        0        0    15709 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/testing.py
+-rw-r--r--   0        0        0       60 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/utils/__init__.py
+-rw-r--r--   0        0        0     9610 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/utils/database.py
+-rw-r--r--   0        0        0    14611 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/utils/helpers.py
+-rw-r--r--   0        0        0     9549 2024-05-08 15:20:54.184815 jaeger-1.7.1/src/jaeger/utils/utils.py
+-rw-r--r--   0        0        0     4060 1970-01-01 00:00:00.000000 jaeger-1.7.1/PKG-INFO
```

### Comparing `jaeger-1.7.0/LICENSE.md` & `jaeger-1.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/README.md` & `jaeger-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/pyproject.toml` & `jaeger-1.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaeger"
-version = "1.7.0"
+version = "1.7.1"
 description = "Controllers for the SDSS-V FPS"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/jaeger"
 repository = "https://github.com/sdss/jaeger"
 documentation = "https://sdss-jaeger.readthedocs.io/en/latest/"
@@ -28,15 +28,15 @@
 sdss-clu = "^2.0.0"
 sdsstools = "^1.6.0"
 sdssdb = "^0.11.3"
 sdss-kaiju =  [
     {version="^1.4.0b1", python=">=3.11"},
     {version="^1.3.0,<1.4.0", python=">=3.10,<3.11"}
 ]
-sdss-coordio = "^1.9.2"
+sdss-coordio = "^1.11.0"
 click_default_group = ">=1.2.2"
 "zc.lockfile" = "^2.0"
 polars = "^0.20.9"
 adbc-driver-postgresql = ">=0.9.0"
 pyarrow = ">=15.0.0"
 tables = "^3.9.2"
 nptyping = "^2.5.0"
```

### Comparing `jaeger-1.7.0/src/jaeger/__init__.py` & `jaeger-1.7.1/src/jaeger/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/__main__.py` & `jaeger-1.7.1/src/jaeger/__main__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/actor.py` & `jaeger-1.7.1/src/jaeger/actor/actor.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/__init__.py` & `jaeger-1.7.1/src/jaeger/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/alerts.py` & `jaeger-1.7.1/src/jaeger/actor/commands/alerts.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/can.py` & `jaeger-1.7.1/src/jaeger/actor/commands/can.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/chiller.py` & `jaeger-1.7.1/src/jaeger/actor/commands/chiller.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/configuration.py` & `jaeger-1.7.1/src/jaeger/actor/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/debug.py` & `jaeger-1.7.1/src/jaeger/actor/commands/debug.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/disable.py` & `jaeger-1.7.1/src/jaeger/actor/commands/disable.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/fvc.py` & `jaeger-1.7.1/src/jaeger/actor/commands/fvc.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/home.py` & `jaeger-1.7.1/src/jaeger/actor/commands/home.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/ieb.py` & `jaeger-1.7.1/src/jaeger/actor/commands/ieb.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/pollers.py` & `jaeger-1.7.1/src/jaeger/actor/commands/pollers.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/positioner.py` & `jaeger-1.7.1/src/jaeger/actor/commands/positioner.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/power.py` & `jaeger-1.7.1/src/jaeger/actor/commands/power.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/snapshot.py` & `jaeger-1.7.1/src/jaeger/actor/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/talk.py` & `jaeger-1.7.1/src/jaeger/actor/commands/talk.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/testing.py` & `jaeger-1.7.1/src/jaeger/actor/commands/testing.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/unwind.py` & `jaeger-1.7.1/src/jaeger/actor/commands/unwind.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/actor/commands/version.py` & `jaeger-1.7.1/src/jaeger/actor/commands/version.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/alerts.py` & `jaeger-1.7.1/src/jaeger/alerts.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,39 +374,38 @@
             self.notify("IEB not connected. Cannot run chiller checks.")
             return
 
         chiller = Chiller.create()
         assert chiller is not None
 
         try:
-            # setpoint = (await chiller.read_device("TEMPERATURE_USER_SETPOINT"))[0]
+            setpoint = (await chiller.read_device("TEMPERATURE_USER_SETPOINT"))[0]
             fluid_temp = (await chiller.read_device("DISPLAY_VALUE"))[0]
-        except Exception:
-            # self.notify(f"Failed reading chiller values: {err}", level=logging.ERROR)
-            return
+        except Exception as err:
+            self.notify(f"Failed reading chiller values: {err}", level=logging.ERROR)
 
         _, t_d = await self.get_dew_point_temperarure()
 
         if fluid_temp < t_d + config["alerts"]["temperature"]["dew_threshold"]:
             self.set_keyword("alert_chiller_dew_point", True)
             self.notify("Fluid temperature is approaching dew point limit.")
 
         else:
             self.set_keyword("alert_chiller_dew_point", False)
 
-        # chiller_config = config["alerts"]["chiller"]
+        chiller_config = config["alerts"]["chiller"]
 
-        # supply_temp = (await self.ieb.read_device(chiller_config["sensor_supply"]))[0]
+        supply_temp = (await self.ieb.read_device(chiller_config["sensor_supply"]))[0]
 
-        # if abs(setpoint - supply_temp) > chiller_config["threshold"]:
-        #     self.set_keyword("alert_fluid_temperature", True)
-        #     self.notify("Chiller set point is different from supply temperature.")
+        if abs(setpoint - supply_temp) > chiller_config["threshold"]:
+            self.set_keyword("alert_fluid_temperature", True)
+            self.notify("Chiller set point is different from supply temperature.")
 
-        # else:
-        #     self.set_keyword("alert_fluid_temperature", False)
+        else:
+            self.set_keyword("alert_fluid_temperature", False)
 
         # Check if there are chiller alerts.
         chiller_alerts: list[str] = []
         chiller_mod = chiller.modules["chiller"]
         for chiller_dev_name in chiller_mod.devices:
             if chiller_dev_name.startswith("alert_"):
                 value: Any = await chiller.read_device(chiller_dev_name, adapt=False)
```

### Comparing `jaeger-1.7.0/src/jaeger/can.py` & `jaeger-1.7.1/src/jaeger/can.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/chiller.py` & `jaeger-1.7.1/src/jaeger/chiller.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/commands/__init__.py` & `jaeger-1.7.1/src/jaeger/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/commands/base.py` & `jaeger-1.7.1/src/jaeger/commands/base.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/commands/bootloader.py` & `jaeger-1.7.1/src/jaeger/commands/bootloader.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/commands/calibration.py` & `jaeger-1.7.1/src/jaeger/commands/calibration.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/commands/goto.py` & `jaeger-1.7.1/src/jaeger/commands/goto.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/commands/status.py` & `jaeger-1.7.1/src/jaeger/commands/status.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/commands/trajectory.py` & `jaeger-1.7.1/src/jaeger/commands/trajectory.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/etc/chiller_APO.yaml` & `jaeger-1.7.1/src/jaeger/etc/chiller_APO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/etc/chiller_APO_variables.csv` & `jaeger-1.7.1/src/jaeger/etc/chiller_APO_variables.csv`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/etc/fvc.yaml` & `jaeger-1.7.1/src/jaeger/etc/fvc.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/etc/ieb_APO.yaml` & `jaeger-1.7.1/src/jaeger/etc/ieb_APO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/etc/ieb_LCO.yaml` & `jaeger-1.7.1/src/jaeger/etc/ieb_LCO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/etc/jaeger_APO.yml` & `jaeger-1.7.1/src/jaeger/etc/jaeger_APO.yml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/etc/jaeger_LCO.yml` & `jaeger-1.7.1/src/jaeger/etc/jaeger_LCO.yml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/etc/schema.json` & `jaeger-1.7.1/src/jaeger/etc/schema.json`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/etc/sextants/epfl.yaml` & `jaeger-1.7.1/src/jaeger/etc/sextants/epfl.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/etc/sextants/osu.yaml` & `jaeger-1.7.1/src/jaeger/etc/sextants/osu.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/etc/sextants/schema.json` & `jaeger-1.7.1/src/jaeger/etc/sextants/schema.json`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/etc/sextants/uw.yaml` & `jaeger-1.7.1/src/jaeger/etc/sextants/uw.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/exceptions.py` & `jaeger-1.7.1/src/jaeger/exceptions.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/fps.py` & `jaeger-1.7.1/src/jaeger/fps.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/fvc.py` & `jaeger-1.7.1/src/jaeger/fvc.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/ieb.py` & `jaeger-1.7.1/src/jaeger/ieb.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/interfaces/bus.py` & `jaeger-1.7.1/src/jaeger/interfaces/bus.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/interfaces/cannet.py` & `jaeger-1.7.1/src/jaeger/interfaces/cannet.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/interfaces/message.py` & `jaeger-1.7.1/src/jaeger/interfaces/message.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/interfaces/notifier.py` & `jaeger-1.7.1/src/jaeger/interfaces/notifier.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/interfaces/virtual.py` & `jaeger-1.7.1/src/jaeger/interfaces/virtual.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/kaiju.py` & `jaeger-1.7.1/src/jaeger/kaiju.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/maskbits.py` & `jaeger-1.7.1/src/jaeger/maskbits.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/plotting.py` & `jaeger-1.7.1/src/jaeger/plotting.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/positioner.py` & `jaeger-1.7.1/src/jaeger/positioner.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/scripts/generate_chiller_yaml.py` & `jaeger-1.7.1/src/jaeger/scripts/generate_chiller_yaml.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/target/assignment.py` & `jaeger-1.7.1/src/jaeger/target/assignment.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/target/configuration.py` & `jaeger-1.7.1/src/jaeger/target/configuration.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/target/design.py` & `jaeger-1.7.1/src/jaeger/target/design.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/target/schemas.py` & `jaeger-1.7.1/src/jaeger/target/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,17 +114,14 @@
     "zwok": polars.Float64,
     "xwok_kaiju": polars.Float64,
     "ywok_kaiju": polars.Float64,
     "zwok_kaiju": polars.Float64,
     "xwok_measured": polars.Float64,
     "ywok_measured": polars.Float64,
     "zwok_measured": polars.Float64,
-    "xtangent": polars.Float64,
-    "ytangent": polars.Float64,
-    "ztangent": polars.Float64,
     "alpha": polars.Float64,
     "beta": polars.Float64,
 }
 
 
 CONFIGURATION_SCHEMA: SchemaType = FIBRE_DATA_SCHEMA.copy()
 CONFIGURATION_SCHEMA.update(
```

### Comparing `jaeger-1.7.0/src/jaeger/target/tools.py` & `jaeger-1.7.1/src/jaeger/target/tools.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/testing.py` & `jaeger-1.7.1/src/jaeger/testing.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/utils/database.py` & `jaeger-1.7.1/src/jaeger/utils/database.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/utils/helpers.py` & `jaeger-1.7.1/src/jaeger/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/src/jaeger/utils/utils.py` & `jaeger-1.7.1/src/jaeger/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.0/PKG-INFO` & `jaeger-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaeger
-Version: 1.7.0
+Version: 1.7.1
 Summary: Controllers for the SDSS-V FPS
 Home-page: https://github.com/sdss/jaeger
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<3.13
@@ -21,15 +21,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: adbc-driver-postgresql (>=0.9.0)
 Requires-Dist: click_default_group (>=1.2.2)
 Requires-Dist: nptyping (>=2.5.0,<3.0.0)
 Requires-Dist: polars (>=0.20.9,<0.21.0)
 Requires-Dist: pyarrow (>=15.0.0)
 Requires-Dist: sdss-clu (>=2.0.0,<3.0.0)
-Requires-Dist: sdss-coordio (>=1.9.2,<2.0.0)
+Requires-Dist: sdss-coordio (>=1.11.0,<2.0.0)
 Requires-Dist: sdss-drift (>=1.0.0,<2.0.0)
 Requires-Dist: sdss-kaiju (>=1.3.0,<1.4.0) ; python_version >= "3.10" and python_version < "3.11"
 Requires-Dist: sdss-kaiju (>=1.4.0b1,<2.0.0) ; python_version >= "3.11"
 Requires-Dist: sdssdb (>=0.11.3,<0.12.0)
 Requires-Dist: sdsstools (>=1.6.0,<2.0.0)
 Requires-Dist: tables (>=3.9.2,<4.0.0)
 Requires-Dist: zc.lockfile (>=2.0,<3.0)
```

