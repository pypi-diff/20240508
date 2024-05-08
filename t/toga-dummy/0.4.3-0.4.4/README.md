# Comparing `tmp/toga_dummy-0.4.3.tar.gz` & `tmp/toga_dummy-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga_dummy-0.4.3.tar", last modified: Mon May  6 06:43:33 2024, max compression
+gzip compressed data, was "toga_dummy-0.4.4.tar", last modified: Wed May  8 00:58:53 2024, max compression
```

## Comparing `toga_dummy-0.4.3.tar` & `toga_dummy-0.4.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.416354 toga_dummy-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-06 06:43:33.416354 toga_dummy-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:33.416354 toga_dummy-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.404354 toga_dummy-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.408354 toga_dummy-0.4.3/src/toga_dummy/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/app.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.408354 toga_dummy-0.4.3/src/toga_dummy/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/hardware/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/hardware/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/images.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.412354 toga_dummy-0.4.3/src/toga_dummy/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/plugins/image_formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.412354 toga_dummy-0.4.3/src/toga_dummy/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/resources/sample.png
--rw-r--r--   0 runner    (1001) docker     (127)    37825 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/resources/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/resources/toga.png
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/screens.py
--rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.416354 toga_dummy-0.4.3/src/toga_dummy/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/dateinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/mapview.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/timeinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-06 06:43:02.000000 toga_dummy-0.4.3/src/toga_dummy/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.416354 toga_dummy-0.4.3/src/toga_dummy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-06 06:43:33.000000 toga_dummy-0.4.3/src/toga_dummy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-06 06:43:33.000000 toga_dummy-0.4.3/src/toga_dummy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:33.000000 toga_dummy-0.4.3/src/toga_dummy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-06 06:43:33.000000 toga_dummy-0.4.3/src/toga_dummy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 06:43:33.000000 toga_dummy-0.4.3/src/toga_dummy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 06:43:33.000000 toga_dummy-0.4.3/src/toga_dummy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:53.696826 toga_dummy-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-08 00:58:53.696826 toga_dummy-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:58:53.696826 toga_dummy-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:53.684826 toga_dummy-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:53.688826 toga_dummy-0.4.4/src/toga_dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:53.688826 toga_dummy-0.4.4/src/toga_dummy/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/hardware/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/hardware/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:53.688826 toga_dummy-0.4.4/src/toga_dummy/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/plugins/image_formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:53.688826 toga_dummy-0.4.4/src/toga_dummy/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/resources/sample.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37825 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/resources/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/resources/toga.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/screens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:53.696826 toga_dummy-0.4.4/src/toga_dummy/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/dateinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/timeinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-08 00:58:22.000000 toga_dummy-0.4.4/src/toga_dummy/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:53.696826 toga_dummy-0.4.4/src/toga_dummy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-08 00:58:53.000000 toga_dummy-0.4.4/src/toga_dummy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-08 00:58:53.000000 toga_dummy-0.4.4/src/toga_dummy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:58:53.000000 toga_dummy-0.4.4/src/toga_dummy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-08 00:58:53.000000 toga_dummy-0.4.4/src/toga_dummy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 00:58:53.000000 toga_dummy-0.4.4/src/toga_dummy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 00:58:53.000000 toga_dummy-0.4.4/src/toga_dummy.egg-info/top_level.txt
```

### Comparing `toga_dummy-0.4.3/LICENSE` & `toga_dummy-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/PKG-INFO` & `toga_dummy-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-dummy
-Version: 0.4.3
+Version: 0.4.4
 Summary: A dummy testing backend for the Toga widget toolkit.
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
 
 toga-dummy
 ==========
 
 An Dummy backend for the `Toga widget toolkit`_. This doesn't actually display
 anything; it exists purely as a testing environment.
```

### Comparing `toga_dummy-0.4.3/README.rst` & `toga_dummy-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/pyproject.toml` & `toga_dummy-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/app.py` & `toga_dummy-0.4.4/src/toga_dummy/app.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/dialogs.py` & `toga_dummy-0.4.4/src/toga_dummy/dialogs.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/factory.py` & `toga_dummy-0.4.4/src/toga_dummy/factory.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/fonts.py` & `toga_dummy-0.4.4/src/toga_dummy/fonts.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/hardware/camera.py` & `toga_dummy-0.4.4/src/toga_dummy/hardware/camera.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/hardware/location.py` & `toga_dummy-0.4.4/src/toga_dummy/hardware/location.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/images.py` & `toga_dummy-0.4.4/src/toga_dummy/images.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/plugins/image_formats.py` & `toga_dummy-0.4.4/src/toga_dummy/plugins/image_formats.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/resources/sample.png` & `toga_dummy-0.4.4/src/toga_dummy/resources/sample.png`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/resources/screenshot.png` & `toga_dummy-0.4.4/src/toga_dummy/resources/screenshot.png`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/resources/toga.png` & `toga_dummy-0.4.4/src/toga_dummy/resources/toga.png`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/screens.py` & `toga_dummy-0.4.4/src/toga_dummy/screens.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/utils.py` & `toga_dummy-0.4.4/src/toga_dummy/utils.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/base.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/canvas.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/dateinput.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/dateinput.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/detailedlist.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/detailedlist.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/mapview.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/mapview.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/multilinetextinput.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/multilinetextinput.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/numberinput.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/numberinput.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/optioncontainer.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/progressbar.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/scrollcontainer.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/selection.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/selection.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/slider.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/splitcontainer.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/splitcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/switch.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/table.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/table.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/textinput.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/timeinput.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/timeinput.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/tree.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/tree.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/widgets/webview.py` & `toga_dummy-0.4.4/src/toga_dummy/widgets/webview.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy/window.py` & `toga_dummy-0.4.4/src/toga_dummy/window.py`

 * *Files identical despite different names*

### Comparing `toga_dummy-0.4.3/src/toga_dummy.egg-info/PKG-INFO` & `toga_dummy-0.4.4/src/toga_dummy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-dummy
-Version: 0.4.3
+Version: 0.4.4
 Summary: A dummy testing backend for the Toga widget toolkit.
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
 
 toga-dummy
 ==========
 
 An Dummy backend for the `Toga widget toolkit`_. This doesn't actually display
 anything; it exists purely as a testing environment.
```

### Comparing `toga_dummy-0.4.3/src/toga_dummy.egg-info/SOURCES.txt` & `toga_dummy-0.4.4/src/toga_dummy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

