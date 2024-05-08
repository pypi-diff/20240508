# Comparing `tmp/toga_android-0.4.3.tar.gz` & `tmp/toga_android-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga_android-0.4.3.tar", last modified: Mon May  6 06:43:39 2024, max compression
+gzip compressed data, was "toga_android-0.4.4.tar", last modified: Wed May  8 00:58:13 2024, max compression
```

## Comparing `toga_android-0.4.3.tar` & `toga_android-0.4.4.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.056879 toga_android-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 06:43:04.000000 toga_android-0.4.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:04.000000 toga_android-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-06 06:43:39.056879 toga_android-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-06 06:43:04.000000 toga_android-0.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-06 06:43:04.000000 toga_android-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:39.056879 toga_android-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.040879 toga_android-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.044879 toga_android-0.4.3/src/toga_android/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.044879 toga_android-0.4.3/src/toga_android/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/hardware/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/hardware/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/keys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.044879 toga_android-0.4.3/src/toga_android/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18992 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/libs/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.044879 toga_android-0.4.3/src/toga_android/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/resources/marker.png
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/resources/optioncontainer-tab.png
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/resources/toga.png
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/screens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.048879 toga_android-0.4.3/src/toga_android/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/dateinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/imageview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.052879 toga_android-0.4.3/src/toga_android/widgets/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/internal/pickers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/mapview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/timeinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-06 06:43:04.000000 toga_android-0.4.3/src/toga_android/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.056879 toga_android-0.4.3/src/toga_android.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-06 06:43:38.000000 toga_android-0.4.3/src/toga_android.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-06 06:43:39.000000 toga_android-0.4.3/src/toga_android.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:38.000000 toga_android-0.4.3/src/toga_android.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-06 06:43:38.000000 toga_android-0.4.3/src/toga_android.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 06:43:38.000000 toga_android-0.4.3/src/toga_android.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 06:43:38.000000 toga_android-0.4.3/src/toga_android.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.052879 toga_android-0.4.3/tests_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.052879 toga_android-0.4.3/tests_backend/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/hardware/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/hardware/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/hardware/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/probe.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/screens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.056879 toga_android-0.4.3/tests_backend/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/dateinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/mapview.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/timeinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-06 06:43:04.000000 toga_android-0.4.3/tests_backend/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.656571 toga_android-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 00:57:42.000000 toga_android-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-08 00:57:42.000000 toga_android-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-08 00:58:13.656571 toga_android-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-08 00:57:42.000000 toga_android-0.4.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-08 00:57:42.000000 toga_android-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:58:13.656571 toga_android-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.636571 toga_android-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.640571 toga_android-0.4.4/src/toga_android/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.640571 toga_android-0.4.4/src/toga_android/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/hardware/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/hardware/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.640571 toga_android-0.4.4/src/toga_android/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18992 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/libs/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.644571 toga_android-0.4.4/src/toga_android/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/resources/marker.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/resources/optioncontainer-tab.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/resources/toga.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.648571 toga_android-0.4.4/src/toga_android/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/dateinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/imageview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.648571 toga_android-0.4.4/src/toga_android/widgets/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/internal/pickers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/timeinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-08 00:57:42.000000 toga_android-0.4.4/src/toga_android/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.656571 toga_android-0.4.4/src/toga_android.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-08 00:58:13.000000 toga_android-0.4.4/src/toga_android.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-08 00:58:13.000000 toga_android-0.4.4/src/toga_android.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:58:13.000000 toga_android-0.4.4/src/toga_android.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-08 00:58:13.000000 toga_android-0.4.4/src/toga_android.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 00:58:13.000000 toga_android-0.4.4/src/toga_android.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 00:58:13.000000 toga_android-0.4.4/src/toga_android.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.648571 toga_android-0.4.4/tests_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.648571 toga_android-0.4.4/tests_backend/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/hardware/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/hardware/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/hardware/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.652571 toga_android-0.4.4/tests_backend/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/dateinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/timeinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-08 00:57:42.000000 toga_android-0.4.4/tests_backend/window.py
```

### Comparing `toga_android-0.4.3/LICENSE` & `toga_android-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/PKG-INFO` & `toga_android-0.4.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-android
-Version: 0.4.3
+Version: 0.4.4
 Summary: An Android backend for the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: toga-core==0.4.3
+Requires-Dist: toga-core==0.4.4
 
 toga-android
 ============
 
 An Android backend for the `Toga widget toolkit`_.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_,
```

### Comparing `toga_android-0.4.3/README.rst` & `toga_android-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/pyproject.toml` & `toga_android-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/app.py` & `toga_android-0.4.4/src/toga_android/app.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/container.py` & `toga_android-0.4.4/src/toga_android/container.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/dialogs.py` & `toga_android-0.4.4/src/toga_android/dialogs.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/factory.py` & `toga_android-0.4.4/src/toga_android/factory.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/fonts.py` & `toga_android-0.4.4/src/toga_android/fonts.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/hardware/camera.py` & `toga_android-0.4.4/src/toga_android/hardware/camera.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/hardware/location.py` & `toga_android-0.4.4/src/toga_android/hardware/location.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/icons.py` & `toga_android-0.4.4/src/toga_android/icons.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/images.py` & `toga_android-0.4.4/src/toga_android/images.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/keys.py` & `toga_android-0.4.4/src/toga_android/keys.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/libs/events.py` & `toga_android-0.4.4/src/toga_android/libs/events.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/paths.py` & `toga_android-0.4.4/src/toga_android/paths.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/resources/marker.png` & `toga_android-0.4.4/src/toga_android/resources/marker.png`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/resources/optioncontainer-tab.png` & `toga_android-0.4.4/src/toga_android/resources/optioncontainer-tab.png`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/resources/toga.png` & `toga_android-0.4.4/src/toga_android/resources/toga.png`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/screens.py` & `toga_android-0.4.4/src/toga_android/screens.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/base.py` & `toga_android-0.4.4/src/toga_android/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/button.py` & `toga_android-0.4.4/src/toga_android/widgets/button.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/canvas.py` & `toga_android-0.4.4/src/toga_android/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/dateinput.py` & `toga_android-0.4.4/src/toga_android/widgets/dateinput.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/detailedlist.py` & `toga_android-0.4.4/src/toga_android/widgets/detailedlist.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/divider.py` & `toga_android-0.4.4/src/toga_android/widgets/divider.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/imageview.py` & `toga_android-0.4.4/src/toga_android/widgets/imageview.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/internal/pickers.py` & `toga_android-0.4.4/src/toga_android/widgets/internal/pickers.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/label.py` & `toga_android-0.4.4/src/toga_android/widgets/label.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/mapview.py` & `toga_android-0.4.4/src/toga_android/widgets/mapview.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/multilinetextinput.py` & `toga_android-0.4.4/src/toga_android/widgets/multilinetextinput.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/numberinput.py` & `toga_android-0.4.4/src/toga_android/widgets/numberinput.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/optioncontainer.py` & `toga_android-0.4.4/src/toga_android/widgets/optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/progressbar.py` & `toga_android-0.4.4/src/toga_android/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/scrollcontainer.py` & `toga_android-0.4.4/src/toga_android/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/selection.py` & `toga_android-0.4.4/src/toga_android/widgets/selection.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/slider.py` & `toga_android-0.4.4/src/toga_android/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/switch.py` & `toga_android-0.4.4/src/toga_android/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/table.py` & `toga_android-0.4.4/src/toga_android/widgets/table.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/textinput.py` & `toga_android-0.4.4/src/toga_android/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/timeinput.py` & `toga_android-0.4.4/src/toga_android/widgets/timeinput.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/widgets/webview.py` & `toga_android-0.4.4/src/toga_android/widgets/webview.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android/window.py` & `toga_android-0.4.4/src/toga_android/window.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/src/toga_android.egg-info/PKG-INFO` & `toga_android-0.4.4/src/toga_android.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-android
-Version: 0.4.3
+Version: 0.4.4
 Summary: An Android backend for the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: toga-core==0.4.3
+Requires-Dist: toga-core==0.4.4
 
 toga-android
 ============
 
 An Android backend for the `Toga widget toolkit`_.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_,
```

### Comparing `toga_android-0.4.3/src/toga_android.egg-info/SOURCES.txt` & `toga_android-0.4.4/src/toga_android.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/app.py` & `toga_android-0.4.4/tests_backend/app.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/fonts.py` & `toga_android-0.4.4/tests_backend/fonts.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/hardware/camera.py` & `toga_android-0.4.4/tests_backend/hardware/camera.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/hardware/hardware.py` & `toga_android-0.4.4/tests_backend/hardware/hardware.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/hardware/location.py` & `toga_android-0.4.4/tests_backend/hardware/location.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/icons.py` & `toga_android-0.4.4/tests_backend/icons.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/probe.py` & `toga_android-0.4.4/tests_backend/probe.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/screens.py` & `toga_android-0.4.4/tests_backend/screens.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/base.py` & `toga_android-0.4.4/tests_backend/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/button.py` & `toga_android-0.4.4/tests_backend/widgets/button.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/canvas.py` & `toga_android-0.4.4/tests_backend/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/dateinput.py` & `toga_android-0.4.4/tests_backend/widgets/dateinput.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/detailedlist.py` & `toga_android-0.4.4/tests_backend/widgets/detailedlist.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/label.py` & `toga_android-0.4.4/tests_backend/widgets/label.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/mapview.py` & `toga_android-0.4.4/tests_backend/widgets/mapview.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/numberinput.py` & `toga_android-0.4.4/tests_backend/widgets/numberinput.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/optioncontainer.py` & `toga_android-0.4.4/tests_backend/widgets/optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/progressbar.py` & `toga_android-0.4.4/tests_backend/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/properties.py` & `toga_android-0.4.4/tests_backend/widgets/properties.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/scrollcontainer.py` & `toga_android-0.4.4/tests_backend/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/selection.py` & `toga_android-0.4.4/tests_backend/widgets/selection.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/slider.py` & `toga_android-0.4.4/tests_backend/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/table.py` & `toga_android-0.4.4/tests_backend/widgets/table.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/textinput.py` & `toga_android-0.4.4/tests_backend/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/widgets/timeinput.py` & `toga_android-0.4.4/tests_backend/widgets/timeinput.py`

 * *Files identical despite different names*

### Comparing `toga_android-0.4.3/tests_backend/window.py` & `toga_android-0.4.4/tests_backend/window.py`

 * *Files identical despite different names*

