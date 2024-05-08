# Comparing `tmp/openedx-events-9.9.1.tar.gz` & `tmp/openedx_events-9.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-events-9.9.1.tar", last modified: Fri Apr 12 13:04:56 2024, max compression
+gzip compressed data, was "openedx_events-9.9.2.tar", last modified: Thu Apr 18 19:40:03 2024, max compression
```

## Comparing `openedx-events-9.9.1.tar` & `openedx_events-9.9.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:04:56.015689 openedx-events-9.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)    12733 2024-04-12 13:04:52.000000 openedx-events-9.9.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-12 13:04:52.000000 openedx-events-9.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-12 13:04:52.000000 openedx-events-9.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18065 2024-04-12 13:04:56.015689 openedx-events-9.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-12 13:04:52.000000 openedx-events-9.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:04:56.011690 openedx-events-9.9.1/openedx_events/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:04:56.011690 openedx-events-9.9.1/openedx_events/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/analytics/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/analytics/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:04:56.011690 openedx-events-9.9.1/openedx_events/content_authoring/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/content_authoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/content_authoring/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/content_authoring/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:04:56.011690 openedx-events-9.9.1/openedx_events/enterprise/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/enterprise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/enterprise/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/enterprise/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:04:56.011690 openedx-events-9.9.1/openedx_events/event_bus/
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/event_bus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:04:56.011690 openedx-events-9.9.1/openedx_events/event_bus/avro/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/event_bus/avro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/event_bus/avro/custom_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/event_bus/avro/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/event_bus/avro/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/event_bus/avro/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:04:56.015689 openedx-events-9.9.1/openedx_events/event_bus/avro/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/event_bus/avro/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/event_bus/avro/tests/test_avro.py
--rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/event_bus/avro/tests/test_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/event_bus/avro/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/event_bus/avro/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/event_bus/avro/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/event_bus/avro/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:04:56.015689 openedx-events-9.9.1/openedx_events/event_bus/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/event_bus/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:04:56.015689 openedx-events-9.9.1/openedx_events/learning/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/learning/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/learning/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:04:56.015689 openedx-events-9.9.1/openedx_events/management/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:04:56.015689 openedx-events-9.9.1/openedx_events/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/management/commands/consume_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/management/commands/generate_avro_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:04:56.015689 openedx-events-9.9.1/openedx_events/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/tests/test_consume_events_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/tests/test_generate_avro_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/tests/test_producer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14475 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12820 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/tooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-12 13:04:52.000000 openedx-events-9.9.1/openedx_events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:04:56.015689 openedx-events-9.9.1/openedx_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18065 2024-04-12 13:04:55.000000 openedx-events-9.9.1/openedx_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-12 13:04:56.000000 openedx-events-9.9.1/openedx_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:04:55.000000 openedx-events-9.9.1/openedx_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:04:55.000000 openedx-events-9.9.1/openedx_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 13:04:55.000000 openedx-events-9.9.1/openedx_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 13:04:55.000000 openedx-events-9.9.1/openedx_events.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:04:56.015689 openedx-events-9.9.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-12 13:04:52.000000 openedx-events-9.9.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-12 13:04:52.000000 openedx-events-9.9.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-12 13:04:56.015689 openedx-events-9.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-04-12 13:04:52.000000 openedx-events-9.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:03.922649 openedx_events-9.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    12833 2024-04-18 19:39:57.000000 openedx_events-9.9.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-18 19:39:57.000000 openedx_events-9.9.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-18 19:39:57.000000 openedx_events-9.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18165 2024-04-18 19:40:03.922649 openedx_events-9.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-18 19:39:57.000000 openedx_events-9.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:03.918649 openedx_events-9.9.2/openedx_events/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:03.918649 openedx_events-9.9.2/openedx_events/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/analytics/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/analytics/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:03.918649 openedx_events-9.9.2/openedx_events/content_authoring/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/content_authoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/content_authoring/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/content_authoring/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:03.918649 openedx_events-9.9.2/openedx_events/enterprise/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/enterprise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/enterprise/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/enterprise/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:03.918649 openedx_events-9.9.2/openedx_events/event_bus/
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/event_bus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:03.918649 openedx_events-9.9.2/openedx_events/event_bus/avro/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/event_bus/avro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/event_bus/avro/custom_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/event_bus/avro/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/event_bus/avro/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/event_bus/avro/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:03.922649 openedx_events-9.9.2/openedx_events/event_bus/avro/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/event_bus/avro/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/event_bus/avro/tests/test_avro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/event_bus/avro/tests/test_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/event_bus/avro/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/event_bus/avro/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/event_bus/avro/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/event_bus/avro/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:03.922649 openedx_events-9.9.2/openedx_events/event_bus/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/event_bus/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:03.922649 openedx_events-9.9.2/openedx_events/learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18898 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/learning/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/learning/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:03.922649 openedx_events-9.9.2/openedx_events/management/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:03.922649 openedx_events-9.9.2/openedx_events/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/management/commands/consume_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/management/commands/generate_avro_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:03.922649 openedx_events-9.9.2/openedx_events/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/tests/test_consume_events_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/tests/test_generate_avro_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/tests/test_producer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14475 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12820 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-18 19:39:57.000000 openedx_events-9.9.2/openedx_events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:03.922649 openedx_events-9.9.2/openedx_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18165 2024-04-18 19:40:03.000000 openedx_events-9.9.2/openedx_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-18 19:40:03.000000 openedx_events-9.9.2/openedx_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:40:03.000000 openedx_events-9.9.2/openedx_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:40:03.000000 openedx_events-9.9.2/openedx_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 19:40:03.000000 openedx_events-9.9.2/openedx_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 19:40:03.000000 openedx_events-9.9.2/openedx_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:40:03.922649 openedx_events-9.9.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-18 19:39:57.000000 openedx_events-9.9.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-18 19:39:57.000000 openedx_events-9.9.2/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-18 19:40:03.922649 openedx_events-9.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-04-18 19:39:57.000000 openedx_events-9.9.2/setup.py
```

### Comparing `openedx-events-9.9.1/CHANGELOG.rst` & `openedx_events-9.9.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[9.9.2] - 2024-04-18
+--------------------
+
+Changed
+~~~~~~~
+
+* Updated ``ORASubmissionData`` class.
+
 [9.9.1] - 2024-04-12
 --------------------
 
 Changed
 ~~~~~~~
 
 * Updated Python classifiers to include Python 3.11.
```

### Comparing `openedx-events-9.9.1/LICENSE.txt` & `openedx_events-9.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/PKG-INFO` & `openedx_events-9.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 9.9.1
+Version: 9.9.2
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -165,14 +165,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[9.9.2] - 2024-04-18
+--------------------
+
+Changed
+~~~~~~~
+
+* Updated ``ORASubmissionData`` class.
+
 [9.9.1] - 2024-04-12
 --------------------
 
 Changed
 ~~~~~~~
 
 * Updated Python classifiers to include Python 3.11.
```

### Comparing `openedx-events-9.9.1/README.rst` & `openedx_events-9.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/analytics/data.py` & `openedx_events-9.9.2/openedx_events/analytics/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/analytics/signals.py` & `openedx_events-9.9.2/openedx_events/analytics/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/apps.py` & `openedx_events-9.9.2/openedx_events/apps.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/content_authoring/data.py` & `openedx_events-9.9.2/openedx_events/content_authoring/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/content_authoring/signals.py` & `openedx_events-9.9.2/openedx_events/content_authoring/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/data.py` & `openedx_events-9.9.2/openedx_events/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/enterprise/data.py` & `openedx_events-9.9.2/openedx_events/enterprise/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/enterprise/signals.py` & `openedx_events-9.9.2/openedx_events/enterprise/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/event_bus/__init__.py` & `openedx_events-9.9.2/openedx_events/event_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/event_bus/avro/custom_serializers.py` & `openedx_events-9.9.2/openedx_events/event_bus/avro/custom_serializers.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/event_bus/avro/deserializer.py` & `openedx_events-9.9.2/openedx_events/event_bus/avro/deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/event_bus/avro/schema.py` & `openedx_events-9.9.2/openedx_events/event_bus/avro/schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/event_bus/avro/serializer.py` & `openedx_events-9.9.2/openedx_events/event_bus/avro/serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/event_bus/avro/tests/test_avro.py` & `openedx_events-9.9.2/openedx_events/event_bus/avro/tests/test_avro.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/event_bus/avro/tests/test_deserializer.py` & `openedx_events-9.9.2/openedx_events/event_bus/avro/tests/test_deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/event_bus/avro/tests/test_schema.py` & `openedx_events-9.9.2/openedx_events/event_bus/avro/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/event_bus/avro/tests/test_serializer.py` & `openedx_events-9.9.2/openedx_events/event_bus/avro/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/event_bus/avro/tests/test_utilities.py` & `openedx_events-9.9.2/openedx_events/event_bus/avro/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/event_bus/tests/test_loader.py` & `openedx_events-9.9.2/openedx_events/event_bus/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/exceptions.py` & `openedx_events-9.9.2/openedx_events/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/learning/data.py` & `openedx_events-9.9.2/openedx_events/learning/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -443,36 +443,53 @@
     notification_type = attr.ib(type=str)
     content_url = attr.ib(type=str)
     content_context = attr.ib(type=dict, factory=dict)
     audience_filters = attr.ib(type=dict, factory=dict)
 
 
 @attr.s(frozen=True)
-class ORAFileDownloadsData:
+class ORASubmissionAnswer:
     """
-    Attributes defined to represent file downloads in an ORA submission.
+    Attributes defined to represent the answer submitted by the user in an ORA submission.
 
     Arguments:
-        download_url (str): URL to download the file.
-        description (str): Description of the file.
-        name (str): Name of the file.
-        size (int): Size of the file.
+        parts (List[dict]): List with the response text in the ORA submission.
+
+        The following attributes are used to represent the files submitted in the ORA submission:
+
+        file_keys (List[str]): List of file keys in the ORA submission.
+        file_descriptions (List[str]): List of file descriptions in the ORA submission.
+        file_names (List[str]): List of file names in the ORA submission.
+        file_sizes (List[int]): List of file sizes in the ORA submission.
+        file_urls (List[str]): List of file URLs in the ORA submission.
     """
 
-    download_url = attr.ib(type=str)
-    description = attr.ib(type=str)
-    name = attr.ib(type=str)
-    size = attr.ib(type=int)
+    parts = attr.ib(type=List[dict], factory=list)
+    file_keys = attr.ib(type=List[str], factory=list)
+    file_descriptions = attr.ib(type=List[str], factory=list)
+    file_names = attr.ib(type=List[str], factory=list)
+    file_sizes = attr.ib(type=List[int], factory=list)
+    file_urls = attr.ib(type=List[str], factory=list)
 
 
 @attr.s(frozen=True)
 class ORASubmissionData:
     """
     Attributes defined to represent event when a user submits an ORA assignment.
 
     Arguments:
-        id (str): identifier of the ORA submission.
-        file_downloads (List[ORAFileDownloadsData]): list of related files in the ORA submission.
+        uuid (str): The UUID of the ORA submission.
+        anonymous_user_id (str): Optional. Anonymous user ID of the user who submitted the ORA submission.
+        location (str): Optional. Location of the ORA submission.
+        attempt_number (int): Attempt number of the ORA submission.
+        created_at (datetime): Date and time when the ORA submission was created.
+        submitted_at (datetime): Date and time when the ORA submission was submitted.
+        answer (ORASubmissionAnswer): Answer submitted by the user in the ORA submission.
     """
 
-    id = attr.ib(type=str)
-    file_downloads = attr.ib(type=List[ORAFileDownloadsData], factory=list)
+    uuid = attr.ib(type=str)
+    anonymous_user_id = attr.ib(type=str)
+    location = attr.ib(type=str)
+    attempt_number = attr.ib(type=int)
+    created_at = attr.ib(type=datetime)
+    submitted_at = attr.ib(type=datetime)
+    answer = attr.ib(type=ORASubmissionAnswer)
```

### Comparing `openedx-events-9.9.1/openedx_events/learning/signals.py` & `openedx_events-9.9.2/openedx_events/learning/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/management/commands/consume_events.py` & `openedx_events-9.9.2/openedx_events/management/commands/consume_events.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/management/commands/generate_avro_schemas.py` & `openedx_events-9.9.2/openedx_events/management/commands/generate_avro_schemas.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/tests/test_consume_events_command.py` & `openedx_events-9.9.2/openedx_events/tests/test_consume_events_command.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/tests/test_data.py` & `openedx_events-9.9.2/openedx_events/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/tests/test_generate_avro_schemas.py` & `openedx_events-9.9.2/openedx_events/tests/test_generate_avro_schemas.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/tests/test_producer_config.py` & `openedx_events-9.9.2/openedx_events/tests/test_producer_config.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/tests/test_tooling.py` & `openedx_events-9.9.2/openedx_events/tests/test_tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/tests/utils.py` & `openedx_events-9.9.2/openedx_events/tests/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/tooling.py` & `openedx_events-9.9.2/openedx_events/tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events/utils.py` & `openedx_events-9.9.2/openedx_events/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/openedx_events.egg-info/PKG-INFO` & `openedx_events-9.9.2/openedx_events.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 9.9.1
+Version: 9.9.2
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -165,14 +165,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[9.9.2] - 2024-04-18
+--------------------
+
+Changed
+~~~~~~~
+
+* Updated ``ORASubmissionData`` class.
+
 [9.9.1] - 2024-04-12
 --------------------
 
 Changed
 ~~~~~~~
 
 * Updated Python classifiers to include Python 3.11.
```

### Comparing `openedx-events-9.9.1/openedx_events.egg-info/SOURCES.txt` & `openedx_events-9.9.2/openedx_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/requirements/constraints.txt` & `openedx_events-9.9.2/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-9.9.1/setup.py` & `openedx_events-9.9.2/setup.py`

 * *Files identical despite different names*

