# Comparing `tmp/reactpy_django-3.8.0.tar.gz` & `tmp/reactpy_django-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactpy_django-3.8.0.tar", last modified: Wed Feb 21 01:55:12 2024, max compression
+gzip compressed data, was "reactpy_django-3.8.1.tar", last modified: Tue May  7 23:44:03 2024, max compression
```

## Comparing `reactpy_django-3.8.0.tar` & `reactpy_django-3.8.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 01:55:12.490877 reactpy_django-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7153 2024-02-21 01:55:12.490877 reactpy_django-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-21 01:55:12.490877 reactpy_django-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 01:55:12.478877 reactpy_django-3.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 01:55:12.486877 reactpy_django-3.8.0/src/reactpy_django/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    20457 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     9273 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17160 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 01:55:12.486877 reactpy_django-3.8.0/src/reactpy_django/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/http/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/http/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 01:55:12.486877 reactpy_django-3.8.0/src/reactpy_django/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 01:55:12.486877 reactpy_django-3.8.0/src/reactpy_django/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/management/commands/clean_reactpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 01:55:12.486877 reactpy_django-3.8.0/src/reactpy_django/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/migrations/0002_rename_created_at_componentparams_last_accessed.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/migrations/0004_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/migrations/0005_alter_componentsession_last_accessed.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/migrations/0006_userdatamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 01:55:12.490877 reactpy_django-3.8.0/src/reactpy_django/router/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/router/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/router/resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 01:55:12.478877 reactpy_django-3.8.0/src/reactpy_django/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 01:55:12.490877 reactpy_django-3.8.0/src/reactpy_django/static/reactpy_django/
--rw-r--r--   0 runner    (1001) docker     (127)   173276 2024-02-21 01:55:12.000000 reactpy_django-3.8.0/src/reactpy_django/static/reactpy_django/client.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 01:55:12.478877 reactpy_django-3.8.0/src/reactpy_django/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 01:55:12.490877 reactpy_django-3.8.0/src/reactpy_django/templates/reactpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/templates/reactpy/component.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 01:55:12.490877 reactpy_django-3.8.0/src/reactpy_django/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/templatetags/reactpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    13168 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 01:55:12.490877 reactpy_django-3.8.0/src/reactpy_django/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/websocket/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-21 01:54:49.000000 reactpy_django-3.8.0/src/reactpy_django/websocket/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 01:55:12.490877 reactpy_django-3.8.0/src/reactpy_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7153 2024-02-21 01:55:12.000000 reactpy_django-3.8.0/src/reactpy_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-02-21 01:55:12.000000 reactpy_django-3.8.0/src/reactpy_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 01:55:12.000000 reactpy_django-3.8.0/src/reactpy_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 01:55:05.000000 reactpy_django-3.8.0/src/reactpy_django.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-21 01:55:12.000000 reactpy_django-3.8.0/src/reactpy_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-21 01:55:12.000000 reactpy_django-3.8.0/src/reactpy_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:44:03.981609 reactpy_django-3.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-07 23:44:03.981609 reactpy_django-3.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 23:44:03.981609 reactpy_django-3.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:44:03.969609 reactpy_django-3.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:44:03.977609 reactpy_django-3.8.1/src/reactpy_django/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20457 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9273 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:44:03.977609 reactpy_django-3.8.1/src/reactpy_django/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/http/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/http/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:44:03.977609 reactpy_django-3.8.1/src/reactpy_django/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:44:03.977609 reactpy_django-3.8.1/src/reactpy_django/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/management/commands/clean_reactpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:44:03.981609 reactpy_django-3.8.1/src/reactpy_django/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/migrations/0002_rename_created_at_componentparams_last_accessed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/migrations/0004_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/migrations/0005_alter_componentsession_last_accessed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/migrations/0006_userdatamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:44:03.981609 reactpy_django-3.8.1/src/reactpy_django/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/router/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/router/resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:44:03.973609 reactpy_django-3.8.1/src/reactpy_django/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:44:03.981609 reactpy_django-3.8.1/src/reactpy_django/static/reactpy_django/
+-rw-r--r--   0 runner    (1001) docker     (127)   173276 2024-05-07 23:44:03.000000 reactpy_django-3.8.1/src/reactpy_django/static/reactpy_django/client.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:44:03.973609 reactpy_django-3.8.1/src/reactpy_django/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:44:03.981609 reactpy_django-3.8.1/src/reactpy_django/templates/reactpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/templates/reactpy/component.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:44:03.981609 reactpy_django-3.8.1/src/reactpy_django/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/templatetags/reactpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:44:03.981609 reactpy_django-3.8.1/src/reactpy_django/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/websocket/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-07 23:43:45.000000 reactpy_django-3.8.1/src/reactpy_django/websocket/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:44:03.981609 reactpy_django-3.8.1/src/reactpy_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-07 23:44:03.000000 reactpy_django-3.8.1/src/reactpy_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-07 23:44:03.000000 reactpy_django-3.8.1/src/reactpy_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:44:03.000000 reactpy_django-3.8.1/src/reactpy_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:43:57.000000 reactpy_django-3.8.1/src/reactpy_django.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 23:44:03.000000 reactpy_django-3.8.1/src/reactpy_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 23:44:03.000000 reactpy_django-3.8.1/src/reactpy_django.egg-info/top_level.txt
```

### Comparing `reactpy_django-3.8.0/LICENSE.md` & `reactpy_django-3.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/PKG-INFO` & `reactpy_django-3.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: reactpy_django
-Version: 3.8.0
+Version: 3.8.1
 Summary: It's React, but in Python. Now with Django integration.
 Home-page: https://github.com/reactive-python/reactpy-django
 Author: Mark Bakhit
 Author-email: archiethemonger@gmail.com
 License: MIT
 Keywords: interactive,reactive,widgets,DOM,React,ReactJS,ReactPy
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Environment :: Web Environment
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -49,15 +50,15 @@
         <img src="https://img.shields.io/website?down_message=offline&label=Docs&logo=read%20the%20docs&logoColor=white&up_message=online&url=https%3A%2F%2Freactive-python.github.io%2Freactpy-django%2F">
     </a>
     <a href="https://discord.gg/uNb5P4hA9X">
         <img src="https://img.shields.io/discord/1111078259854168116?label=Discord&logo=discord">
     </a>
 </p>
 
-[ReactPy-Django](https://github.com/reactive-python/reactpy-django) is used to add used to add [ReactPy](https://reactpy.dev/) support to an existing **Django project**. This package also turbocharges ReactPy with features such as...
+[ReactPy-Django](https://github.com/reactive-python/reactpy-django) is used to add [ReactPy](https://reactpy.dev/) support to an existing **Django project**. This package also turbocharges ReactPy with features such as...
 
 -   [SEO compatible rendering](https://reactive-python.github.io/reactpy-django/latest/reference/settings/#reactpy_prerender)
 -   [Single page application (SPA) capabilities](https://reactive-python.github.io/reactpy-django/latest/reference/router/#django-router)
 -   [Distributed computing](https://reactive-python.github.io/reactpy-django/latest/reference/settings/#reactpy_default_hosts)
 -   [Performance enhancements](https://reactive-python.github.io/reactpy-django/latest/reference/settings/#performance-settings)
 -   [Customizable reconnection behavior](https://reactive-python.github.io/reactpy-django/latest/reference/settings/#stability-settings)
 -   [Customizable disconnection behavior](https://reactive-python.github.io/reactpy-django/latest/reference/template-tag)
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: reactpy_django Version: 3.8.0 Summary: It's React,
+Metadata-Version: 2.1 Name: reactpy_django Version: 3.8.1 Summary: It's React,
 but in Python. Now with Django integration. Home-page: https://github.com/
 reactive-python/reactpy-django Author: Mark Bakhit Author-email:
 archiethemonger@gmail.com License: MIT Keywords:
 interactive,reactive,widgets,DOM,React,ReactJS,ReactPy Platform: Linux
 Platform: Mac OS X Platform: Windows Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Operating System :: OS
-Independent Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Science/Research Classifier: Topic :: Multimedia :: Graphics
-Classifier: Environment :: Web Environment Requires-Python: >=3.9 Description-
-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
-channels>=4.0.0 Requires-Dist: django>=4.2.0 Requires-Dist:
-reactpy<1.1.0,>=1.0.2 Requires-Dist: reactpy-router<1.0.0,>=0.1.1 Requires-
-Dist: aiofile>=3.0 Requires-Dist: dill>=0.3.5 Requires-Dist: orjson>=3.6.0
-Requires-Dist: nest_asyncio>=1.5.0 Requires-Dist: typing_extensions # [https://
-raw.githubusercontent.com/reactive-python/reactpy/main/branding/svg/reactpy-
-logo-square.svg]ReactPy Django
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Operating System :: OS Independent Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Science/
+Research Classifier: Topic :: Multimedia :: Graphics Classifier: Environment ::
+Web Environment Requires-Python: >=3.9 Description-Content-Type: text/markdown
+License-File: LICENSE.md Requires-Dist: channels>=4.0.0 Requires-Dist:
+django>=4.2.0 Requires-Dist: reactpy<1.1.0,>=1.0.2 Requires-Dist: reactpy-
+router<1.0.0,>=0.1.1 Requires-Dist: aiofile>=3.0 Requires-Dist: dill>=0.3.5
+Requires-Dist: orjson>=3.6.0 Requires-Dist: nest_asyncio>=1.5.0 Requires-Dist:
+typing_extensions # [https://raw.githubusercontent.com/reactive-python/reactpy/
+main/branding/svg/reactpy-logo-square.svg]ReactPy Django
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_r_e_a_c_t_i_v_e_-_p_y_t_h_o_n_/_r_e_a_c_t_p_y_-_d_j_a_n_g_o_/_w_o_r_k_f_l_o_w_s_/_T_e_s_t_/
 _b_a_d_g_e_._s_v_g_?_e_v_e_n_t_=_p_u_s_h_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_r_e_a_c_t_p_y_-
 _d_j_a_n_g_o_._s_v_g_?_l_a_b_e_l_=_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_p_u_r_p_l_e_._s_v_g_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_d_o_w_n___m_e_s_s_a_g_e_=_o_f_f_l_i_n_e_&_l_a_b_e_l_=_D_o_c_s_&_l_o_g_o_=_r_e_a_d_%_2_0_t_h_e_%_2_0_d_o_c_s_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_&_u_p___m_e_s_s_a_g_e_=_o_n_l_i_n_e_&_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_r_e_a_c_t_i_v_e_-
 _p_y_t_h_o_n_._g_i_t_h_u_b_._i_o_%_2_F_r_e_a_c_t_p_y_-_d_j_a_n_g_o_%_2_F_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_i_s_c_o_r_d_/
 _1_1_1_1_0_7_8_2_5_9_8_5_4_1_6_8_1_1_6_?_l_a_b_e_l_=_D_i_s_c_o_r_d_&_l_o_g_o_=_d_i_s_c_o_r_d_]
 [ReactPy-Django](https://github.com/reactive-python/reactpy-django) is used to
-add used to add [ReactPy](https://reactpy.dev/) support to an existing **Django
-project**. This package also turbocharges ReactPy with features such as... -
-[SEO compatible rendering](https://reactive-python.github.io/reactpy-django/
-latest/reference/settings/#reactpy_prerender) - [Single page application (SPA)
+add [ReactPy](https://reactpy.dev/) support to an existing **Django project**.
+This package also turbocharges ReactPy with features such as... - [SEO
+compatible rendering](https://reactive-python.github.io/reactpy-django/latest/
+reference/settings/#reactpy_prerender) - [Single page application (SPA)
 capabilities](https://reactive-python.github.io/reactpy-django/latest/
 reference/router/#django-router) - [Distributed computing](https://reactive-
 python.github.io/reactpy-django/latest/reference/settings/
 #reactpy_default_hosts) - [Performance enhancements](https://reactive-
 python.github.io/reactpy-django/latest/reference/settings/#performance-
 settings) - [Customizable reconnection behavior](https://reactive-
 python.github.io/reactpy-django/latest/reference/settings/#stability-settings)
```

### Comparing `reactpy_django-3.8.0/README.md` & `reactpy_django-3.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         <img src="https://img.shields.io/website?down_message=offline&label=Docs&logo=read%20the%20docs&logoColor=white&up_message=online&url=https%3A%2F%2Freactive-python.github.io%2Freactpy-django%2F">
     </a>
     <a href="https://discord.gg/uNb5P4hA9X">
         <img src="https://img.shields.io/discord/1111078259854168116?label=Discord&logo=discord">
     </a>
 </p>
 
-[ReactPy-Django](https://github.com/reactive-python/reactpy-django) is used to add used to add [ReactPy](https://reactpy.dev/) support to an existing **Django project**. This package also turbocharges ReactPy with features such as...
+[ReactPy-Django](https://github.com/reactive-python/reactpy-django) is used to add [ReactPy](https://reactpy.dev/) support to an existing **Django project**. This package also turbocharges ReactPy with features such as...
 
 -   [SEO compatible rendering](https://reactive-python.github.io/reactpy-django/latest/reference/settings/#reactpy_prerender)
 -   [Single page application (SPA) capabilities](https://reactive-python.github.io/reactpy-django/latest/reference/router/#django-router)
 -   [Distributed computing](https://reactive-python.github.io/reactpy-django/latest/reference/settings/#reactpy_default_hosts)
 -   [Performance enhancements](https://reactive-python.github.io/reactpy-django/latest/reference/settings/#performance-settings)
 -   [Customizable reconnection behavior](https://reactive-python.github.io/reactpy-django/latest/reference/settings/#stability-settings)
 -   [Customizable disconnection behavior](https://reactive-python.github.io/reactpy-django/latest/reference/template-tag)
```

#### html2text {}

```diff
@@ -4,18 +4,18 @@
 _b_a_d_g_e_._s_v_g_?_e_v_e_n_t_=_p_u_s_h_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_r_e_a_c_t_p_y_-
 _d_j_a_n_g_o_._s_v_g_?_l_a_b_e_l_=_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_p_u_r_p_l_e_._s_v_g_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_d_o_w_n___m_e_s_s_a_g_e_=_o_f_f_l_i_n_e_&_l_a_b_e_l_=_D_o_c_s_&_l_o_g_o_=_r_e_a_d_%_2_0_t_h_e_%_2_0_d_o_c_s_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_&_u_p___m_e_s_s_a_g_e_=_o_n_l_i_n_e_&_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_r_e_a_c_t_i_v_e_-
 _p_y_t_h_o_n_._g_i_t_h_u_b_._i_o_%_2_F_r_e_a_c_t_p_y_-_d_j_a_n_g_o_%_2_F_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_i_s_c_o_r_d_/
 _1_1_1_1_0_7_8_2_5_9_8_5_4_1_6_8_1_1_6_?_l_a_b_e_l_=_D_i_s_c_o_r_d_&_l_o_g_o_=_d_i_s_c_o_r_d_]
 [ReactPy-Django](https://github.com/reactive-python/reactpy-django) is used to
-add used to add [ReactPy](https://reactpy.dev/) support to an existing **Django
-project**. This package also turbocharges ReactPy with features such as... -
-[SEO compatible rendering](https://reactive-python.github.io/reactpy-django/
-latest/reference/settings/#reactpy_prerender) - [Single page application (SPA)
+add [ReactPy](https://reactpy.dev/) support to an existing **Django project**.
+This package also turbocharges ReactPy with features such as... - [SEO
+compatible rendering](https://reactive-python.github.io/reactpy-django/latest/
+reference/settings/#reactpy_prerender) - [Single page application (SPA)
 capabilities](https://reactive-python.github.io/reactpy-django/latest/
 reference/router/#django-router) - [Distributed computing](https://reactive-
 python.github.io/reactpy-django/latest/reference/settings/
 #reactpy_default_hosts) - [Performance enhancements](https://reactive-
 python.github.io/reactpy-django/latest/reference/settings/#performance-
 settings) - [Customizable reconnection behavior](https://reactive-
 python.github.io/reactpy-django/latest/reference/settings/#stability-settings)
```

### Comparing `reactpy_django-3.8.0/setup.py` & `reactpy_django-3.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     "zip_safe": False,
     "classifiers": [
         "Framework :: Django",
         "Framework :: Django :: 4.0",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Topic :: Multimedia :: Graphics",
         "Environment :: Web Environment",
     ],
 }
```

### Comparing `reactpy_django-3.8.0/src/reactpy_django/__init__.py` & `reactpy_django-3.8.1/src/reactpy_django/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from reactpy_django import checks, components, decorators, hooks, router, types, utils
 from reactpy_django.websocket.paths import (
     REACTPY_WEBSOCKET_PATH,
     REACTPY_WEBSOCKET_ROUTE,
 )
 
-__version__ = "3.8.0"
+__version__ = "3.8.1"
 __all__ = [
     "REACTPY_WEBSOCKET_PATH",
     "REACTPY_WEBSOCKET_ROUTE",
     "hooks",
     "components",
     "decorators",
     "types",
```

### Comparing `reactpy_django-3.8.0/src/reactpy_django/checks.py` & `reactpy_django-3.8.1/src/reactpy_django/checks.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/clean.py` & `reactpy_django-3.8.1/src/reactpy_django/clean.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/components.py` & `reactpy_django-3.8.1/src/reactpy_django/components.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/config.py` & `reactpy_django-3.8.1/src/reactpy_django/config.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/database.py` & `reactpy_django-3.8.1/src/reactpy_django/database.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/decorators.py` & `reactpy_django-3.8.1/src/reactpy_django/decorators.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/hooks.py` & `reactpy_django-3.8.1/src/reactpy_django/hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Sequence,
     Union,
     cast,
     overload,
 )
 from uuid import uuid4
 
-import orjson as pickle
+import orjson
 from channels import DEFAULT_CHANNEL_LAYER
 from channels.db import database_sync_to_async
 from channels.layers import InMemoryChannelLayer, get_channel_layer
 from reactpy import use_callback, use_effect, use_memo, use_ref, use_state
 from reactpy import use_connection as _use_connection
 from reactpy import use_location as _use_location
 from reactpy import use_scope as _use_scope
@@ -347,15 +347,15 @@
         if not isinstance(data, dict):
             raise TypeError(f"Expected dict while setting user data, got {type(data)}")
         if user.is_anonymous:
             raise ValueError("AnonymousUser cannot have user data.")
 
         pk = get_pk(user)
         model, _ = await UserDataModel.objects.aget_or_create(user_pk=pk)
-        model.data = pickle.dumps(data)
+        model.data = orjson.dumps(data)
         await model.asave()
 
     query: Query[dict | None] = use_query(
         QueryOptions(postprocessor=None),
         _get_user_data,
         user=user,
         default_data=default_data,
@@ -467,15 +467,15 @@
     from reactpy_django.models import UserDataModel
 
     if not user or user.is_anonymous:
         return None
 
     pk = get_pk(user)
     model, _ = await UserDataModel.objects.aget_or_create(user_pk=pk)
-    data = pickle.loads(model.data) if model.data else {}
+    data = orjson.loads(model.data) if model.data else {}
 
     if not isinstance(data, dict):
         raise TypeError(f"Expected dict while loading user data, got {type(data)}")
 
     # Set default values, if needed
     if default_data:
         changed = False
@@ -485,12 +485,12 @@
                 if asyncio.iscoroutinefunction(value):
                     new_value = await value()
                 elif callable(value):
                     new_value = value()
                 data[key] = new_value
                 changed = True
         if changed:
-            model.data = pickle.dumps(data)
+            model.data = orjson.dumps(data)
             if save_default_data:
                 await model.asave()
 
     return data
```

### Comparing `reactpy_django-3.8.0/src/reactpy_django/http/views.py` & `reactpy_django-3.8.1/src/reactpy_django/http/views.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/management/commands/clean_reactpy.py` & `reactpy_django-3.8.1/src/reactpy_django/management/commands/clean_reactpy.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/migrations/0001_initial.py` & `reactpy_django-3.8.1/src/reactpy_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py` & `reactpy_django-3.8.1/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/migrations/0004_config.py` & `reactpy_django-3.8.1/src/reactpy_django/migrations/0004_config.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/migrations/0006_userdatamodel.py` & `reactpy_django-3.8.1/src/reactpy_django/migrations/0006_userdatamodel.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/models.py` & `reactpy_django-3.8.1/src/reactpy_django/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from django.contrib.auth import get_user_model
 from django.db import models
 from django.db.models.signals import pre_delete
 from django.dispatch import receiver
 
+from reactpy_django.utils import get_pk
+
 
 class ComponentSession(models.Model):
     """A model for storing component sessions."""
 
     uuid = models.UUIDField(primary_key=True, editable=False, unique=True)  # type: ignore
     params = models.BinaryField(editable=False)  # type: ignore
     last_accessed = models.DateTimeField(auto_now=True)  # type: ignore
@@ -37,10 +39,10 @@
     user_pk = models.CharField(max_length=255, unique=True)  # type: ignore
     data = models.BinaryField(null=True, blank=True)  # type: ignore
 
 
 @receiver(pre_delete, sender=get_user_model(), dispatch_uid="reactpy_delete_user_data")
 def delete_user_data(sender, instance, **kwargs):
     """Delete ReactPy's `UserDataModel` when a Django `User` is deleted."""
-    pk = getattr(instance, instance._meta.pk.name)
+    pk = get_pk(instance)
 
     UserDataModel.objects.filter(user_pk=pk).delete()
```

### Comparing `reactpy_django-3.8.0/src/reactpy_django/router/resolvers.py` & `reactpy_django-3.8.1/src/reactpy_django/router/resolvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,11 +48,11 @@
         pattern += re.escape(path[last_match_end : match.start()])
         pattern += f"(?P<{param_name}>{param_conv['regex']})"
         converters[param_name] = param_conv["func"]
         last_match_end = match.end()
     pattern += f"{re.escape(path[last_match_end:])}$"
 
     # Replace literal `*` with "match anything" regex pattern, if it's at the end of the path
-    if pattern.endswith("\*$"):
+    if pattern.endswith(r"\*$"):
         pattern = f"{pattern[:-3]}.*$"
 
     return re.compile(pattern), converters
```

### Comparing `reactpy_django-3.8.0/src/reactpy_django/static/reactpy_django/client.js` & `reactpy_django-3.8.1/src/reactpy_django/static/reactpy_django/client.js`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/templates/reactpy/component.html` & `reactpy_django-3.8.1/src/reactpy_django/templates/reactpy/component.html`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/templatetags/reactpy.py` & `reactpy_django-3.8.1/src/reactpy_django/templatetags/reactpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-from distutils.util import strtobool
 from logging import getLogger
 from uuid import uuid4
 
 import dill as pickle
 from django import template
 from django.http import HttpRequest
 from django.urls import NoReverseMatch, reverse
@@ -18,15 +17,15 @@
     ComponentCarrierError,
     ComponentDoesNotExistError,
     ComponentParamError,
     InvalidHostError,
     OfflineComponentMissing,
 )
 from reactpy_django.types import ComponentParams
-from reactpy_django.utils import SyncLayout, validate_component_args
+from reactpy_django.utils import SyncLayout, strtobool, validate_component_args
 
 try:
     RESOLVED_WEB_MODULES_PATH = reverse("reactpy:web_modules", args=["/"]).strip("/")
 except NoReverseMatch:
     RESOLVED_WEB_MODULES_PATH = ""
 register = template.Library()
 _logger = getLogger(__name__)
```

### Comparing `reactpy_django-3.8.0/src/reactpy_django/types.py` & `reactpy_django-3.8.1/src/reactpy_django/types.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/utils.py` & `reactpy_django-3.8.1/src/reactpy_django/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -362,7 +362,23 @@
     def render(self):
         return async_to_sync(super().render)()
 
 
 def get_pk(model):
     """Returns the value of the primary key for a Django model."""
     return getattr(model, model._meta.pk.name)
+
+
+def strtobool(val):
+    """Convert a string representation of truth to true (1) or false (0).
+
+    True values are 'y', 'yes', 't', 'true', 'on', and '1'; false values
+    are 'n', 'no', 'f', 'false', 'off', and '0'.  Raises ValueError if
+    'val' is anything else.
+    """
+    val = val.lower()
+    if val in ("y", "yes", "t", "true", "on", "1"):
+        return 1
+    elif val in ("n", "no", "f", "false", "off", "0"):
+        return 0
+    else:
+        raise ValueError("invalid truth value %r" % (val,))
```

### Comparing `reactpy_django-3.8.0/src/reactpy_django/websocket/consumer.py` & `reactpy_django-3.8.1/src/reactpy_django/websocket/consumer.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django/websocket/paths.py` & `reactpy_django-3.8.1/src/reactpy_django/websocket/paths.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.8.0/src/reactpy_django.egg-info/PKG-INFO` & `reactpy_django-3.8.1/src/reactpy_django.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: reactpy_django
-Version: 3.8.0
+Version: 3.8.1
 Summary: It's React, but in Python. Now with Django integration.
 Home-page: https://github.com/reactive-python/reactpy-django
 Author: Mark Bakhit
 Author-email: archiethemonger@gmail.com
 License: MIT
 Keywords: interactive,reactive,widgets,DOM,React,ReactJS,ReactPy
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Environment :: Web Environment
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -49,15 +50,15 @@
         <img src="https://img.shields.io/website?down_message=offline&label=Docs&logo=read%20the%20docs&logoColor=white&up_message=online&url=https%3A%2F%2Freactive-python.github.io%2Freactpy-django%2F">
     </a>
     <a href="https://discord.gg/uNb5P4hA9X">
         <img src="https://img.shields.io/discord/1111078259854168116?label=Discord&logo=discord">
     </a>
 </p>
 
-[ReactPy-Django](https://github.com/reactive-python/reactpy-django) is used to add used to add [ReactPy](https://reactpy.dev/) support to an existing **Django project**. This package also turbocharges ReactPy with features such as...
+[ReactPy-Django](https://github.com/reactive-python/reactpy-django) is used to add [ReactPy](https://reactpy.dev/) support to an existing **Django project**. This package also turbocharges ReactPy with features such as...
 
 -   [SEO compatible rendering](https://reactive-python.github.io/reactpy-django/latest/reference/settings/#reactpy_prerender)
 -   [Single page application (SPA) capabilities](https://reactive-python.github.io/reactpy-django/latest/reference/router/#django-router)
 -   [Distributed computing](https://reactive-python.github.io/reactpy-django/latest/reference/settings/#reactpy_default_hosts)
 -   [Performance enhancements](https://reactive-python.github.io/reactpy-django/latest/reference/settings/#performance-settings)
 -   [Customizable reconnection behavior](https://reactive-python.github.io/reactpy-django/latest/reference/settings/#stability-settings)
 -   [Customizable disconnection behavior](https://reactive-python.github.io/reactpy-django/latest/reference/template-tag)
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: reactpy_django Version: 3.8.0 Summary: It's React,
+Metadata-Version: 2.1 Name: reactpy_django Version: 3.8.1 Summary: It's React,
 but in Python. Now with Django integration. Home-page: https://github.com/
 reactive-python/reactpy-django Author: Mark Bakhit Author-email:
 archiethemonger@gmail.com License: MIT Keywords:
 interactive,reactive,widgets,DOM,React,ReactJS,ReactPy Platform: Linux
 Platform: Mac OS X Platform: Windows Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Operating System :: OS
-Independent Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Science/Research Classifier: Topic :: Multimedia :: Graphics
-Classifier: Environment :: Web Environment Requires-Python: >=3.9 Description-
-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
-channels>=4.0.0 Requires-Dist: django>=4.2.0 Requires-Dist:
-reactpy<1.1.0,>=1.0.2 Requires-Dist: reactpy-router<1.0.0,>=0.1.1 Requires-
-Dist: aiofile>=3.0 Requires-Dist: dill>=0.3.5 Requires-Dist: orjson>=3.6.0
-Requires-Dist: nest_asyncio>=1.5.0 Requires-Dist: typing_extensions # [https://
-raw.githubusercontent.com/reactive-python/reactpy/main/branding/svg/reactpy-
-logo-square.svg]ReactPy Django
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Operating System :: OS Independent Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Science/
+Research Classifier: Topic :: Multimedia :: Graphics Classifier: Environment ::
+Web Environment Requires-Python: >=3.9 Description-Content-Type: text/markdown
+License-File: LICENSE.md Requires-Dist: channels>=4.0.0 Requires-Dist:
+django>=4.2.0 Requires-Dist: reactpy<1.1.0,>=1.0.2 Requires-Dist: reactpy-
+router<1.0.0,>=0.1.1 Requires-Dist: aiofile>=3.0 Requires-Dist: dill>=0.3.5
+Requires-Dist: orjson>=3.6.0 Requires-Dist: nest_asyncio>=1.5.0 Requires-Dist:
+typing_extensions # [https://raw.githubusercontent.com/reactive-python/reactpy/
+main/branding/svg/reactpy-logo-square.svg]ReactPy Django
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_r_e_a_c_t_i_v_e_-_p_y_t_h_o_n_/_r_e_a_c_t_p_y_-_d_j_a_n_g_o_/_w_o_r_k_f_l_o_w_s_/_T_e_s_t_/
 _b_a_d_g_e_._s_v_g_?_e_v_e_n_t_=_p_u_s_h_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_r_e_a_c_t_p_y_-
 _d_j_a_n_g_o_._s_v_g_?_l_a_b_e_l_=_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_p_u_r_p_l_e_._s_v_g_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_d_o_w_n___m_e_s_s_a_g_e_=_o_f_f_l_i_n_e_&_l_a_b_e_l_=_D_o_c_s_&_l_o_g_o_=_r_e_a_d_%_2_0_t_h_e_%_2_0_d_o_c_s_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_&_u_p___m_e_s_s_a_g_e_=_o_n_l_i_n_e_&_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_r_e_a_c_t_i_v_e_-
 _p_y_t_h_o_n_._g_i_t_h_u_b_._i_o_%_2_F_r_e_a_c_t_p_y_-_d_j_a_n_g_o_%_2_F_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_i_s_c_o_r_d_/
 _1_1_1_1_0_7_8_2_5_9_8_5_4_1_6_8_1_1_6_?_l_a_b_e_l_=_D_i_s_c_o_r_d_&_l_o_g_o_=_d_i_s_c_o_r_d_]
 [ReactPy-Django](https://github.com/reactive-python/reactpy-django) is used to
-add used to add [ReactPy](https://reactpy.dev/) support to an existing **Django
-project**. This package also turbocharges ReactPy with features such as... -
-[SEO compatible rendering](https://reactive-python.github.io/reactpy-django/
-latest/reference/settings/#reactpy_prerender) - [Single page application (SPA)
+add [ReactPy](https://reactpy.dev/) support to an existing **Django project**.
+This package also turbocharges ReactPy with features such as... - [SEO
+compatible rendering](https://reactive-python.github.io/reactpy-django/latest/
+reference/settings/#reactpy_prerender) - [Single page application (SPA)
 capabilities](https://reactive-python.github.io/reactpy-django/latest/
 reference/router/#django-router) - [Distributed computing](https://reactive-
 python.github.io/reactpy-django/latest/reference/settings/
 #reactpy_default_hosts) - [Performance enhancements](https://reactive-
 python.github.io/reactpy-django/latest/reference/settings/#performance-
 settings) - [Customizable reconnection behavior](https://reactive-
 python.github.io/reactpy-django/latest/reference/settings/#stability-settings)
```

### Comparing `reactpy_django-3.8.0/src/reactpy_django.egg-info/SOURCES.txt` & `reactpy_django-3.8.1/src/reactpy_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

