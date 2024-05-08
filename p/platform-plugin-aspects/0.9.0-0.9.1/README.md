# Comparing `tmp/platform_plugin_aspects-0.9.0.tar.gz` & `tmp/platform_plugin_aspects-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform_plugin_aspects-0.9.0.tar", last modified: Mon May  6 20:11:03 2024, max compression
+gzip compressed data, was "platform_plugin_aspects-0.9.1.tar", last modified: Wed May  8 18:56:24 2024, max compression
```

## Comparing `platform_plugin_aspects-0.9.0.tar` & `platform_plugin_aspects-0.9.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:03.903921 platform_plugin_aspects-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-05-06 20:11:03.903921 platform_plugin_aspects-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:03.895921 platform_plugin_aspects-0.9.0/platform_plugin_aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:03.899921 platform_plugin_aspects-0.9.0/platform_plugin_aspects/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/extensions/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:03.899921 platform_plugin_aspects-0.9.0/platform_plugin_aspects/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:03.899921 platform_plugin_aspects-0.9.0/platform_plugin_aspects/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/management/commands/load_test_tracking_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:03.899921 platform_plugin_aspects-0.9.0/platform_plugin_aspects/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:03.899921 platform_plugin_aspects-0.9.0/platform_plugin_aspects/sinks/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/sinks/base_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/sinks/course_overview_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/sinks/external_id_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/sinks/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/sinks/user_profile_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/sinks/user_retire_sink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:03.895921 platform_plugin_aspects-0.9.0/platform_plugin_aspects/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:03.899921 platform_plugin_aspects-0.9.0/platform_plugin_aspects/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/static/css/superset.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:03.899921 platform_plugin_aspects-0.9.0/platform_plugin_aspects/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/static/html/superset.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/static/html/superset_student.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:03.903921 platform_plugin_aspects-0.9.0/platform_plugin_aspects/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/static/js/embed_dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/static/js/install_required.js
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/static/js/superset.js
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:03.895921 platform_plugin_aspects-0.9.0/platform_plugin_aspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:03.903921 platform_plugin_aspects-0.9.0/platform_plugin_aspects/templates/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/waffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects/xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:03.903921 platform_plugin_aspects-0.9.0/platform_plugin_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-05-06 20:11:03.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-06 20:11:03.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:11:03.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-06 20:11:03.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:11:03.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-06 20:11:03.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 20:11:03.000000 platform_plugin_aspects-0.9.0/platform_plugin_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:03.903921 platform_plugin_aspects-0.9.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-06 20:11:03.903921 platform_plugin_aspects-0.9.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6997 2024-05-06 20:10:58.000000 platform_plugin_aspects-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:24.003554 platform_plugin_aspects-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-08 18:56:24.003554 platform_plugin_aspects-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:23.999554 platform_plugin_aspects-0.9.1/platform_plugin_aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:23.999554 platform_plugin_aspects-0.9.1/platform_plugin_aspects/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/extensions/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:23.999554 platform_plugin_aspects-0.9.1/platform_plugin_aspects/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:23.999554 platform_plugin_aspects-0.9.1/platform_plugin_aspects/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/management/commands/load_test_tracking_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:24.003554 platform_plugin_aspects-0.9.1/platform_plugin_aspects/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:24.003554 platform_plugin_aspects-0.9.1/platform_plugin_aspects/sinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/sinks/base_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/sinks/course_overview_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/sinks/external_id_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/sinks/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/sinks/user_profile_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/sinks/user_retire_sink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:23.995554 platform_plugin_aspects-0.9.1/platform_plugin_aspects/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:24.003554 platform_plugin_aspects-0.9.1/platform_plugin_aspects/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/static/css/superset.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:24.003554 platform_plugin_aspects-0.9.1/platform_plugin_aspects/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/static/html/superset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/static/html/superset_student.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:24.003554 platform_plugin_aspects-0.9.1/platform_plugin_aspects/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/static/js/embed_dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/static/js/install_required.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/static/js/superset.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:23.995554 platform_plugin_aspects-0.9.1/platform_plugin_aspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:24.003554 platform_plugin_aspects-0.9.1/platform_plugin_aspects/templates/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects/xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:24.003554 platform_plugin_aspects-0.9.1/platform_plugin_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-08 18:56:23.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-08 18:56:23.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:56:23.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-08 18:56:23.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:56:23.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-08 18:56:23.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 18:56:23.000000 platform_plugin_aspects-0.9.1/platform_plugin_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:56:24.003554 platform_plugin_aspects-0.9.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-08 18:56:24.003554 platform_plugin_aspects-0.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6997 2024-05-08 18:56:20.000000 platform_plugin_aspects-0.9.1/setup.py
```

### Comparing `platform_plugin_aspects-0.9.0/CHANGELOG.rst` & `platform_plugin_aspects-0.9.1/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+0.9.1 - 2024-05-08
+******************
+
+Fixes
+=====
+
+* Fix an ImportError in the Aspects Xblock on pre-Quince releases
+
+
 0.9.0 - 2024-05-06
 ******************
 
 Added
 =====
 
 * Allow embedded dashboard tab names to be localized
```

### Comparing `platform_plugin_aspects-0.9.0/LICENSE` & `platform_plugin_aspects-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/PKG-INFO` & `platform_plugin_aspects-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.9.0
+Version: 0.9.1
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -272,14 +272,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+0.9.1 - 2024-05-08
+******************
+
+Fixes
+=====
+
+* Fix an ImportError in the Aspects Xblock on pre-Quince releases
+
+
 0.9.0 - 2024-05-06
 ******************
 
 Added
 =====
 
 * Allow embedded dashboard tab names to be localized
```

### Comparing `platform_plugin_aspects-0.9.0/README.rst` & `platform_plugin_aspects-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/apps.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/apps.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/extensions/filters.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/extensions/filters.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/management/commands/load_test_tracking_events.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/management/commands/load_test_tracking_events.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/settings/common.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/settings/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         "internal_service_url": "http://superset:8088",
         "username": "superset",
         "password": "superset",
     }
     settings.ASPECTS_INSTRUCTOR_DASHBOARDS = [
         {
             "name": _("Course Dashboard"),
-            "slug": "course-dashboard-v1",
+            "slug": "course-dashboard",
             "uuid": "c0e64194-33d1-4d5a-8c10-4f51530c5ee9",
             "allow_translations": True,
         },
         {
             "name": _("Individual Learner Dashboard"),
             "slug": "individual-learner",
             "uuid": "abae8a25-1ba4-4653-81bd-d3937a162a11",
```

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/settings/production.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/settings/production.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/signals.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/signals.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/sinks/base_sink.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/sinks/base_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/sinks/course_overview_sink.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/sinks/course_overview_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/sinks/external_id_sink.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/sinks/external_id_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/sinks/serializers.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/sinks/serializers.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/sinks/user_profile_sink.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/sinks/user_profile_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/sinks/user_retire_sink.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/sinks/user_retire_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/static/css/superset.css` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/static/css/superset.css`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/static/html/superset.html` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/static/html/superset.html`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/static/js/embed_dashboard.js` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/static/js/embed_dashboard.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/static/js/superset.js` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/static/js/superset.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/tasks.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/tasks.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/templates/instructor_dashboard/aspects.html`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/urls.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/urls.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/utils.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/utils.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/views.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/views.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects/xblock.py` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects/xblock.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,23 @@
 from django.core.exceptions import ImproperlyConfigured
 from django.utils import translation
 from web_fragments.fragment import Fragment
 from webob import Response
 from xblock.core import XBlock
 from xblock.exceptions import JsonHandlerError
 from xblock.fields import List, Scope, String
-from xblock.utils.resources import ResourceLoader
-from xblock.utils.studio_editable import StudioEditableXBlockMixin
+
+# These moved from xblockutils to xblock in Quince, these can be removed
+# when we stop supporting earlier versions.
+try:  # pragma: no-cover
+    from xblock.utils.resources import ResourceLoader
+    from xblock.utils.studio_editable import StudioEditableXBlockMixin
+except ImportError:
+    from xblockutils.resources import ResourceLoader
+    from xblockutils.studio_editable import StudioEditableXBlockMixin
 
 from .utils import (
     DEFAULT_FILTERS_FORMAT,
     _,
     generate_guest_token,
     generate_superset_context,
 )
```

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects.egg-info/PKG-INFO` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.9.0
+Version: 0.9.1
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -272,14 +272,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+0.9.1 - 2024-05-08
+******************
+
+Fixes
+=====
+
+* Fix an ImportError in the Aspects Xblock on pre-Quince releases
+
+
 0.9.0 - 2024-05-06
 ******************
 
 Added
 =====
 
 * Allow embedded dashboard tab names to be localized
```

### Comparing `platform_plugin_aspects-0.9.0/platform_plugin_aspects.egg-info/SOURCES.txt` & `platform_plugin_aspects-0.9.1/platform_plugin_aspects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/requirements/constraints.txt` & `platform_plugin_aspects-0.9.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.0/setup.py` & `platform_plugin_aspects-0.9.1/setup.py`

 * *Files identical despite different names*

