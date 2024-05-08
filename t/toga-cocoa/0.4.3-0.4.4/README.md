# Comparing `tmp/toga_cocoa-0.4.3.tar.gz` & `tmp/toga_cocoa-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga_cocoa-0.4.3.tar", last modified: Mon May  6 06:43:37 2024, max compression
+gzip compressed data, was "toga_cocoa-0.4.4.tar", last modified: Wed May  8 00:58:11 2024, max compression
```

## Comparing `toga_cocoa-0.4.3.tar` & `toga_cocoa-0.4.4.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.825609 toga_cocoa-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-06 06:43:37.825609 toga_cocoa-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:37.825609 toga_cocoa-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.805608 toga_cocoa-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.809608 toga_cocoa-0.4.3/src/toga_cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20027 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.813608 toga_cocoa-0.4.3/src/toga_cocoa/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/hardware/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/hardware/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/keys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.813608 toga_cocoa-0.4.3/src/toga_cocoa/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/appkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/av_foundation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/core_graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/core_location.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/core_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/foundation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/mapkit.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/libs/webkit.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.813608 toga_cocoa-0.4.3/src/toga_cocoa/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/resources/camera.png
--rw-r--r--   0 runner    (1001) docker     (127)   396417 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/resources/toga.icns
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/screens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.817608 toga_cocoa-0.4.3/src/toga_cocoa/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/imageview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.821608 toga_cocoa-0.4.3/src/toga_cocoa/widgets/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/internal/cells.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/internal/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12148 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/internal/refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/mapview.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)    13159 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/src/toga_cocoa/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.825609 toga_cocoa-0.4.3/src/toga_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-06 06:43:37.000000 toga_cocoa-0.4.3/src/toga_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-06 06:43:37.000000 toga_cocoa-0.4.3/src/toga_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:37.000000 toga_cocoa-0.4.3/src/toga_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 06:43:37.000000 toga_cocoa-0.4.3/src/toga_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 06:43:37.000000 toga_cocoa-0.4.3/src/toga_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 06:43:37.000000 toga_cocoa-0.4.3/src/toga_cocoa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.821608 toga_cocoa-0.4.3/tests_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.821608 toga_cocoa-0.4.3/tests_backend/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/hardware/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/hardware/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/probe.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/screens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.825609 toga_cocoa-0.4.3/tests_backend/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/mapview.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-05-06 06:43:02.000000 toga_cocoa-0.4.3/tests_backend/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.157875 toga_cocoa-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-08 00:58:11.153875 toga_cocoa-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:58:11.157875 toga_cocoa-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.137875 toga_cocoa-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.141875 toga_cocoa-0.4.4/src/toga_cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20027 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.141875 toga_cocoa-0.4.4/src/toga_cocoa/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/hardware/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/hardware/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.145875 toga_cocoa-0.4.4/src/toga_cocoa/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/libs/appkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/libs/av_foundation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/libs/core_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/libs/core_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/libs/core_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/libs/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/libs/mapkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/libs/webkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.145875 toga_cocoa-0.4.4/src/toga_cocoa/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/resources/camera.png
+-rw-r--r--   0 runner    (1001) docker     (127)   396417 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/resources/toga.icns
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.149875 toga_cocoa-0.4.4/src/toga_cocoa/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/imageview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.149875 toga_cocoa-0.4.4/src/toga_cocoa/widgets/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/internal/cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/internal/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12148 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/internal/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13159 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/src/toga_cocoa/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.153875 toga_cocoa-0.4.4/src/toga_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-08 00:58:10.000000 toga_cocoa-0.4.4/src/toga_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-08 00:58:11.000000 toga_cocoa-0.4.4/src/toga_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:58:10.000000 toga_cocoa-0.4.4/src/toga_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 00:58:10.000000 toga_cocoa-0.4.4/src/toga_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 00:58:10.000000 toga_cocoa-0.4.4/src/toga_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 00:58:10.000000 toga_cocoa-0.4.4/src/toga_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.149875 toga_cocoa-0.4.4/tests_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.149875 toga_cocoa-0.4.4/tests_backend/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/hardware/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/hardware/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.153875 toga_cocoa-0.4.4/tests_backend/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-05-08 00:57:42.000000 toga_cocoa-0.4.4/tests_backend/window.py
```

### Comparing `toga_cocoa-0.4.3/LICENSE` & `toga_cocoa-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/PKG-INFO` & `toga_cocoa-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-cocoa
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Cocoa (macOS) backend for the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -28,15 +28,15 @@
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: fonttools<5.0.0,>=4.42.1
 Requires-Dist: rubicon-objc<0.5.0,>=0.4.7
-Requires-Dist: toga-core==0.4.3
+Requires-Dist: toga-core==0.4.4
 
 toga-cocoa
 ==========
 
 A Cocoa backend for the `Toga widget toolkit`_.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
```

### Comparing `toga_cocoa-0.4.3/README.rst` & `toga_cocoa-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/pyproject.toml` & `toga_cocoa-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/app.py` & `toga_cocoa-0.4.4/src/toga_cocoa/app.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/command.py` & `toga_cocoa-0.4.4/src/toga_cocoa/command.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/constraints.py` & `toga_cocoa-0.4.4/src/toga_cocoa/constraints.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/container.py` & `toga_cocoa-0.4.4/src/toga_cocoa/container.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/dialogs.py` & `toga_cocoa-0.4.4/src/toga_cocoa/dialogs.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/documents.py` & `toga_cocoa-0.4.4/src/toga_cocoa/documents.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/factory.py` & `toga_cocoa-0.4.4/src/toga_cocoa/factory.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/fonts.py` & `toga_cocoa-0.4.4/src/toga_cocoa/fonts.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/hardware/camera.py` & `toga_cocoa-0.4.4/src/toga_cocoa/hardware/camera.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/hardware/location.py` & `toga_cocoa-0.4.4/src/toga_cocoa/hardware/location.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/images.py` & `toga_cocoa-0.4.4/src/toga_cocoa/images.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/keys.py` & `toga_cocoa-0.4.4/src/toga_cocoa/keys.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/libs/__init__.py` & `toga_cocoa-0.4.4/src/toga_cocoa/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/libs/appkit.py` & `toga_cocoa-0.4.4/src/toga_cocoa/libs/appkit.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/libs/av_foundation.py` & `toga_cocoa-0.4.4/src/toga_cocoa/libs/av_foundation.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/libs/core_graphics.py` & `toga_cocoa-0.4.4/src/toga_cocoa/libs/core_graphics.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/libs/core_location.py` & `toga_cocoa-0.4.4/src/toga_cocoa/libs/core_location.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/libs/core_text.py` & `toga_cocoa-0.4.4/src/toga_cocoa/libs/core_text.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/libs/foundation.py` & `toga_cocoa-0.4.4/src/toga_cocoa/libs/foundation.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/libs/mapkit.py` & `toga_cocoa-0.4.4/src/toga_cocoa/libs/mapkit.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/libs/webkit.py` & `toga_cocoa-0.4.4/src/toga_cocoa/libs/webkit.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/paths.py` & `toga_cocoa-0.4.4/src/toga_cocoa/paths.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/resources/camera.png` & `toga_cocoa-0.4.4/src/toga_cocoa/resources/camera.png`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/resources/toga.icns` & `toga_cocoa-0.4.4/src/toga_cocoa/resources/toga.icns`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/screens.py` & `toga_cocoa-0.4.4/src/toga_cocoa/screens.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/activityindicator.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/activityindicator.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/base.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/box.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/box.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/button.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/button.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/canvas.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/detailedlist.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/detailedlist.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/divider.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/divider.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/imageview.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/imageview.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/internal/cells.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/internal/cells.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/internal/refresh.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/internal/refresh.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/label.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/label.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/mapview.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/mapview.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/multilinetextinput.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/multilinetextinput.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/numberinput.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/numberinput.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/optioncontainer.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/passwordinput.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/passwordinput.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/progressbar.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/scrollcontainer.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/selection.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/selection.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/slider.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/splitcontainer.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/splitcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/switch.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/table.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/table.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/textinput.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/tree.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/tree.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/widgets/webview.py` & `toga_cocoa-0.4.4/src/toga_cocoa/widgets/webview.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa/window.py` & `toga_cocoa-0.4.4/src/toga_cocoa/window.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa.egg-info/PKG-INFO` & `toga_cocoa-0.4.4/src/toga_cocoa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-cocoa
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Cocoa (macOS) backend for the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -28,15 +28,15 @@
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: fonttools<5.0.0,>=4.42.1
 Requires-Dist: rubicon-objc<0.5.0,>=0.4.7
-Requires-Dist: toga-core==0.4.3
+Requires-Dist: toga-core==0.4.4
 
 toga-cocoa
 ==========
 
 A Cocoa backend for the `Toga widget toolkit`_.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
```

### Comparing `toga_cocoa-0.4.3/src/toga_cocoa.egg-info/SOURCES.txt` & `toga_cocoa-0.4.4/src/toga_cocoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/app.py` & `toga_cocoa-0.4.4/tests_backend/app.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/fonts.py` & `toga_cocoa-0.4.4/tests_backend/fonts.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/hardware/camera.py` & `toga_cocoa-0.4.4/tests_backend/hardware/camera.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/hardware/location.py` & `toga_cocoa-0.4.4/tests_backend/hardware/location.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/icons.py` & `toga_cocoa-0.4.4/tests_backend/icons.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/probe.py` & `toga_cocoa-0.4.4/tests_backend/probe.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/base.py` & `toga_cocoa-0.4.4/tests_backend/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/button.py` & `toga_cocoa-0.4.4/tests_backend/widgets/button.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/canvas.py` & `toga_cocoa-0.4.4/tests_backend/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/detailedlist.py` & `toga_cocoa-0.4.4/tests_backend/widgets/detailedlist.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/label.py` & `toga_cocoa-0.4.4/tests_backend/widgets/label.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/mapview.py` & `toga_cocoa-0.4.4/tests_backend/widgets/mapview.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/multilinetextinput.py` & `toga_cocoa-0.4.4/tests_backend/widgets/multilinetextinput.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/numberinput.py` & `toga_cocoa-0.4.4/tests_backend/widgets/numberinput.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/optioncontainer.py` & `toga_cocoa-0.4.4/tests_backend/widgets/optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/progressbar.py` & `toga_cocoa-0.4.4/tests_backend/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/properties.py` & `toga_cocoa-0.4.4/tests_backend/widgets/properties.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/scrollcontainer.py` & `toga_cocoa-0.4.4/tests_backend/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/selection.py` & `toga_cocoa-0.4.4/tests_backend/widgets/selection.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/slider.py` & `toga_cocoa-0.4.4/tests_backend/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/splitcontainer.py` & `toga_cocoa-0.4.4/tests_backend/widgets/splitcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/table.py` & `toga_cocoa-0.4.4/tests_backend/widgets/table.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/textinput.py` & `toga_cocoa-0.4.4/tests_backend/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/widgets/tree.py` & `toga_cocoa-0.4.4/tests_backend/widgets/tree.py`

 * *Files identical despite different names*

### Comparing `toga_cocoa-0.4.3/tests_backend/window.py` & `toga_cocoa-0.4.4/tests_backend/window.py`

 * *Files identical despite different names*

