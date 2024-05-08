# Comparing `tmp/toga_gtk-0.4.3.tar.gz` & `tmp/toga_gtk-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga_gtk-0.4.3.tar", last modified: Mon May  6 06:43:35 2024, max compression
+gzip compressed data, was "toga_gtk-0.4.4.tar", last modified: Wed May  8 00:58:55 2024, max compression
```

## Comparing `toga_gtk-0.4.3.tar` & `toga_gtk-0.4.4.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.174737 toga_gtk-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-06 06:43:35.174737 toga_gtk-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:35.174737 toga_gtk-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.154737 toga_gtk-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.158737 toga_gtk-0.4.3/src/toga_gtk/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11447 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.162737 toga_gtk-0.4.3/src/toga_gtk/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/keys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.162737 toga_gtk-0.4.3/src/toga_gtk/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/libs/fontconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/libs/gtk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/libs/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/libs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.162737 toga_gtk-0.4.3/src/toga_gtk/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/resources/toga.png
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/screens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.166737 toga_gtk-0.4.3/src/toga_gtk/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/mapview.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/src/toga_gtk/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.174737 toga_gtk-0.4.3/src/toga_gtk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-06 06:43:35.000000 toga_gtk-0.4.3/src/toga_gtk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-06 06:43:35.000000 toga_gtk-0.4.3/src/toga_gtk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:35.000000 toga_gtk-0.4.3/src/toga_gtk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 06:43:35.000000 toga_gtk-0.4.3/src/toga_gtk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-06 06:43:35.000000 toga_gtk-0.4.3/src/toga_gtk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 06:43:35.000000 toga_gtk-0.4.3/src/toga_gtk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.170737 toga_gtk-0.4.3/tests_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/images.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/probe.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/screens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:35.174737 toga_gtk-0.4.3/tests_backend/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/mapview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-05-06 06:43:03.000000 toga_gtk-0.4.3/tests_backend/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.238960 toga_gtk-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-08 00:58:55.238960 toga_gtk-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:58:55.238960 toga_gtk-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.218960 toga_gtk-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.222960 toga_gtk-0.4.4/src/toga_gtk/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11447 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.226960 toga_gtk-0.4.4/src/toga_gtk/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.226960 toga_gtk-0.4.4/src/toga_gtk/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/libs/fontconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/libs/gtk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/libs/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/libs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.226960 toga_gtk-0.4.4/src/toga_gtk/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/resources/toga.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.230960 toga_gtk-0.4.4/src/toga_gtk/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/src/toga_gtk/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.238960 toga_gtk-0.4.4/src/toga_gtk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-08 00:58:55.000000 toga_gtk-0.4.4/src/toga_gtk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-08 00:58:55.000000 toga_gtk-0.4.4/src/toga_gtk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:58:55.000000 toga_gtk-0.4.4/src/toga_gtk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 00:58:55.000000 toga_gtk-0.4.4/src/toga_gtk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 00:58:55.000000 toga_gtk-0.4.4/src/toga_gtk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 00:58:55.000000 toga_gtk-0.4.4/src/toga_gtk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.230960 toga_gtk-0.4.4/tests_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.234960 toga_gtk-0.4.4/tests_backend/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-05-08 00:58:23.000000 toga_gtk-0.4.4/tests_backend/window.py
```

### Comparing `toga_gtk-0.4.3/LICENSE` & `toga_gtk-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/PKG-INFO` & `toga_gtk-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-gtk
-Version: 0.4.3
+Version: 0.4.4
 Summary: A GTK backend for the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -29,15 +29,15 @@
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: gbulb>=0.5.3
 Requires-Dist: pycairo>=1.17.0
 Requires-Dist: pygobject>=3.46.0
-Requires-Dist: toga-core==0.4.3
+Requires-Dist: toga-core==0.4.4
 
 toga-gtk
 ========
 
 A GTK backend for the `Toga widget toolkit`_.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
```

### Comparing `toga_gtk-0.4.3/README.rst` & `toga_gtk-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/pyproject.toml` & `toga_gtk-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/app.py` & `toga_gtk-0.4.4/src/toga_gtk/app.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/command.py` & `toga_gtk-0.4.4/src/toga_gtk/command.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/container.py` & `toga_gtk-0.4.4/src/toga_gtk/container.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/dialogs.py` & `toga_gtk-0.4.4/src/toga_gtk/dialogs.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/factory.py` & `toga_gtk-0.4.4/src/toga_gtk/factory.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/fonts.py` & `toga_gtk-0.4.4/src/toga_gtk/fonts.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/icons.py` & `toga_gtk-0.4.4/src/toga_gtk/icons.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/images.py` & `toga_gtk-0.4.4/src/toga_gtk/images.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/keys.py` & `toga_gtk-0.4.4/src/toga_gtk/keys.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/libs/fontconfig.py` & `toga_gtk-0.4.4/src/toga_gtk/libs/fontconfig.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/libs/gtk.py` & `toga_gtk-0.4.4/src/toga_gtk/libs/gtk.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/libs/styles.py` & `toga_gtk-0.4.4/src/toga_gtk/libs/styles.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/resources/toga.png` & `toga_gtk-0.4.4/src/toga_gtk/resources/toga.png`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/screens.py` & `toga_gtk-0.4.4/src/toga_gtk/screens.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/activityindicator.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/activityindicator.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/base.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/button.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/button.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/canvas.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/detailedlist.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/detailedlist.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/divider.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/divider.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/imageview.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/imageview.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/label.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/label.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/mapview.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/mapview.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 </head>
 <body>
     <div id="map"></div>
     <script>
         const map = L.map("map");
         const pins = {};
         const tiles = L.tileLayer("https://tile.openstreetmap.org/{z}/{x}/{y}.png", {
-            maxZoom: 19,
+            maxZoom: 20,
             attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
         }).addTo(map);
     </script>
 </body>
 </html>
 """
```

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/multilinetextinput.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/multilinetextinput.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/numberinput.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/numberinput.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/optioncontainer.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/progressbar.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/scrollcontainer.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/selection.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/selection.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/slider.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/splitcontainer.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/splitcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/switch.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/table.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/table.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/textinput.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/tree.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/tree.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/widgets/webview.py` & `toga_gtk-0.4.4/src/toga_gtk/widgets/webview.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk/window.py` & `toga_gtk-0.4.4/src/toga_gtk/window.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/src/toga_gtk.egg-info/PKG-INFO` & `toga_gtk-0.4.4/src/toga_gtk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-gtk
-Version: 0.4.3
+Version: 0.4.4
 Summary: A GTK backend for the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -29,15 +29,15 @@
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: gbulb>=0.5.3
 Requires-Dist: pycairo>=1.17.0
 Requires-Dist: pygobject>=3.46.0
-Requires-Dist: toga-core==0.4.3
+Requires-Dist: toga-core==0.4.4
 
 toga-gtk
 ========
 
 A GTK backend for the `Toga widget toolkit`_.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
```

### Comparing `toga_gtk-0.4.3/src/toga_gtk.egg-info/SOURCES.txt` & `toga_gtk-0.4.4/src/toga_gtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/app.py` & `toga_gtk-0.4.4/tests_backend/app.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/fonts.py` & `toga_gtk-0.4.4/tests_backend/fonts.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/icons.py` & `toga_gtk-0.4.4/tests_backend/icons.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/probe.py` & `toga_gtk-0.4.4/tests_backend/probe.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/screens.py` & `toga_gtk-0.4.4/tests_backend/screens.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/base.py` & `toga_gtk-0.4.4/tests_backend/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/button.py` & `toga_gtk-0.4.4/tests_backend/widgets/button.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/canvas.py` & `toga_gtk-0.4.4/tests_backend/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/detailedlist.py` & `toga_gtk-0.4.4/tests_backend/widgets/detailedlist.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/label.py` & `toga_gtk-0.4.4/tests_backend/widgets/label.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/mapview.py` & `toga_gtk-0.4.4/tests_backend/widgets/mapview.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/multilinetextinput.py` & `toga_gtk-0.4.4/tests_backend/widgets/multilinetextinput.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/numberinput.py` & `toga_gtk-0.4.4/tests_backend/widgets/numberinput.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/optioncontainer.py` & `toga_gtk-0.4.4/tests_backend/widgets/optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/progressbar.py` & `toga_gtk-0.4.4/tests_backend/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/properties.py` & `toga_gtk-0.4.4/tests_backend/widgets/properties.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/scrollcontainer.py` & `toga_gtk-0.4.4/tests_backend/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/selection.py` & `toga_gtk-0.4.4/tests_backend/widgets/selection.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/slider.py` & `toga_gtk-0.4.4/tests_backend/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/splitcontainer.py` & `toga_gtk-0.4.4/tests_backend/widgets/splitcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/switch.py` & `toga_gtk-0.4.4/tests_backend/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/table.py` & `toga_gtk-0.4.4/tests_backend/widgets/table.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/textinput.py` & `toga_gtk-0.4.4/tests_backend/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/widgets/tree.py` & `toga_gtk-0.4.4/tests_backend/widgets/tree.py`

 * *Files identical despite different names*

### Comparing `toga_gtk-0.4.3/tests_backend/window.py` & `toga_gtk-0.4.4/tests_backend/window.py`

 * *Files identical despite different names*

