# Comparing `tmp/toga_core-0.4.3.tar.gz` & `tmp/toga_core-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga_core-0.4.3.tar", last modified: Mon May  6 06:43:32 2024, max compression
+gzip compressed data, was "toga_core-0.4.4.tar", last modified: Wed May  8 00:58:11 2024, max compression
```

## Comparing `toga_core-0.4.3.tar` & `toga_core-0.4.4.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.847061 toga_core-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 06:43:02.000000 toga_core-0.4.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:02.000000 toga_core-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-06 06:43:32.847061 toga_core-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-06 06:43:02.000000 toga_core-0.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-06 06:43:02.000000 toga_core-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:32.847061 toga_core-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.807061 toga_core-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.815061 toga_core-0.4.3/src/toga/
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33715 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/app.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14886 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.815061 toga_core-0.4.3/src/toga/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.815061 toga_core-0.4.3/src/toga/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/hardware/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/hardware/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.815061 toga_core-0.4.3/src/toga/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/plugins/image_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.815061 toga_core-0.4.3/src/toga/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/screens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.815061 toga_core-0.4.3/src/toga/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/sources/accessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/sources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/sources/list_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    14790 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/sources/tree_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/sources/value_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.819061 toga_core-0.4.3/src/toga/style/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/style/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/style/applicator.py
--rw-r--r--   0 runner    (1001) docker     (127)    40828 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/style/pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    21252 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.823061 toga_core-0.4.3/src/toga/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8969 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)    59957 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/dateinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/mapview.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    16574 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11762 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/timeinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    11440 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)    33283 2024-05-06 06:43:02.000000 toga_core-0.4.3/src/toga/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.843061 toga_core-0.4.3/src/toga_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-06 06:43:32.000000 toga_core-0.4.3/src/toga_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-06 06:43:32.000000 toga_core-0.4.3/src/toga_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:32.000000 toga_core-0.4.3/src/toga_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-06 06:43:32.000000 toga_core-0.4.3/src/toga_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-06 06:43:32.000000 toga_core-0.4.3/src/toga_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 06:43:32.000000 toga_core-0.4.3/src/toga_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.827061 toga_core-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.827061 toga_core-0.4.3/tests/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19065 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/app/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/app/test_documentapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/app/test_mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/app/test_screens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/app/test_widget_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/app/test_windowset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.827061 toga_core-0.4.3/tests/command/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/command/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/command/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/command/test_commandset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/command/test_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.827061 toga_core-0.4.3/tests/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/hardware/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/hardware/test_location.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.831061 toga_core-0.4.3/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/blue.png
--rw-r--r--   0 runner    (1001) docker     (127)    20874 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/orange.bmp
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/orange.png
--rw-r--r--   0 runner    (1001) docker     (127)   772491 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/photo.png
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/red-16.png
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/red-32.png
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/red-72.png
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/red.png
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/sample-dummy.png
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/sample.png
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/resources/toga.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.831061 toga_core-0.4.3/tests/sources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/test_accessors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/test_list_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    13928 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/test_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/test_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/test_tree_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/sources/test_value_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.835061 toga_core-0.4.3/tests/style/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.835061 toga_core-0.4.3/tests/style/pack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.835061 toga_core-0.4.3/tests/style/pack/layout/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_beeliza.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_column_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)    20644 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_flex.py
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_row_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_rtl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_tutorial0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_tutorial1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/layout/test_tutorial3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/test_css.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/pack/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/style/test_applicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)    20019 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    20080 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.835061 toga_core-0.4.3/tests/testbed/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.835061 toga_core-0.4.3/tests/testbed/customize/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/customize/sitecustomize.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.835061 toga_core-0.4.3/tests/testbed/simple/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/simple/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/simple/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.839061 toga_core-0.4.3/tests/testbed/subclassed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/subclassed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/subclassed/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/testbed/subclassed/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.843061 toga_core-0.4.3/tests/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.843061 toga_core-0.4.3/tests/widgets/canvas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/canvas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/canvas/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12753 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/canvas/test_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)    25495 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/canvas/test_context_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/canvas/test_draw_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/canvas/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)    34610 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_dateinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_divider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_label.py
--rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_mapview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    20517 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16386 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_timeinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/widgets/test_webview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.843061 toga_core-0.4.3/tests/window/
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/window/test_filtered_widget_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    30138 2024-05-06 06:43:02.000000 toga_core-0.4.3/tests/window/test_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.386469 toga_core-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 00:57:42.000000 toga_core-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-08 00:57:42.000000 toga_core-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-08 00:58:11.386469 toga_core-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-08 00:57:42.000000 toga_core-0.4.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-08 00:57:42.000000 toga_core-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:58:11.386469 toga_core-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.350469 toga_core-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.354469 toga_core-0.4.4/src/toga/
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33715 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14886 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.354469 toga_core-0.4.4/src/toga/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.354469 toga_core-0.4.4/src/toga/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/hardware/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/hardware/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.354469 toga_core-0.4.4/src/toga/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/plugins/image_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.354469 toga_core-0.4.4/src/toga/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.358469 toga_core-0.4.4/src/toga/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/sources/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/sources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/sources/list_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14790 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/sources/tree_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/sources/value_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.358469 toga_core-0.4.4/src/toga/style/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/style/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/style/applicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40828 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/style/pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21252 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.362469 toga_core-0.4.4/src/toga/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8969 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59957 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/dateinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16574 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11762 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/timeinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11440 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33283 2024-05-08 00:57:42.000000 toga_core-0.4.4/src/toga/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.382469 toga_core-0.4.4/src/toga_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-08 00:58:11.000000 toga_core-0.4.4/src/toga_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-08 00:58:11.000000 toga_core-0.4.4/src/toga_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:58:11.000000 toga_core-0.4.4/src/toga_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 00:58:11.000000 toga_core-0.4.4/src/toga_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-08 00:58:11.000000 toga_core-0.4.4/src/toga_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 00:58:11.000000 toga_core-0.4.4/src/toga_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.366469 toga_core-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.366469 toga_core-0.4.4/tests/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19065 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/app/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/app/test_documentapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/app/test_mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/app/test_screens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/app/test_widget_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/app/test_windowset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.366469 toga_core-0.4.4/tests/command/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/command/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/command/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/command/test_commandset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/command/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.366469 toga_core-0.4.4/tests/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/hardware/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/hardware/test_location.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.370469 toga_core-0.4.4/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/resources/blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20874 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/resources/orange.bmp
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/resources/orange.png
+-rw-r--r--   0 runner    (1001) docker     (127)   772491 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/resources/photo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/resources/red-16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/resources/red-32.png
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/resources/red-72.png
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/resources/red.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/resources/sample-dummy.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/resources/sample.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/resources/toga.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.374469 toga_core-0.4.4/tests/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/sources/test_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/sources/test_list_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13928 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/sources/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/sources/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/sources/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/sources/test_tree_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/sources/test_value_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.374469 toga_core-0.4.4/tests/style/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.374469 toga_core-0.4.4/tests/style/pack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/pack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.374469 toga_core-0.4.4/tests/style/pack/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/pack/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/pack/layout/test_beeliza.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/pack/layout/test_column_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/pack/layout/test_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20644 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/pack/layout/test_flex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/pack/layout/test_row_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/pack/layout/test_rtl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/pack/layout/test_tutorial0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/pack/layout/test_tutorial1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/pack/layout/test_tutorial3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/pack/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/pack/test_css.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/pack/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/style/test_applicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/test_documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/test_fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20019 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/test_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/test_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20080 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.374469 toga_core-0.4.4/tests/testbed/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.374469 toga_core-0.4.4/tests/testbed/customize/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/testbed/customize/sitecustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/testbed/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.378469 toga_core-0.4.4/tests/testbed/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/testbed/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/testbed/simple/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/testbed/simple/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.378469 toga_core-0.4.4/tests/testbed/subclassed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/testbed/subclassed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/testbed/subclassed/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/testbed/subclassed/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.382469 toga_core-0.4.4/tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.382469 toga_core-0.4.4/tests/widgets/canvas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/canvas/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12753 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/canvas/test_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25495 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/canvas/test_context_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/canvas/test_draw_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/canvas/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34610 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_dateinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20517 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16386 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_timeinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/widgets/test_webview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.382469 toga_core-0.4.4/tests/window/
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/window/test_filtered_widget_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30138 2024-05-08 00:57:42.000000 toga_core-0.4.4/tests/window/test_window.py
```

### Comparing `toga_core-0.4.3/LICENSE` & `toga_core-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/PKG-INFO` & `toga_core-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-core
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Python native, OS native GUI toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
```

### Comparing `toga_core-0.4.3/README.rst` & `toga_core-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/pyproject.toml` & `toga_core-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/__init__.py` & `toga_core-0.4.4/src/toga/__init__.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/app.py` & `toga_core-0.4.4/src/toga/app.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/command.py` & `toga_core-0.4.4/src/toga/command.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/constants/__init__.py` & `toga_core-0.4.4/src/toga/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/documents.py` & `toga_core-0.4.4/src/toga/documents.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/fonts.py` & `toga_core-0.4.4/src/toga/fonts.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/handlers.py` & `toga_core-0.4.4/src/toga/handlers.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/hardware/camera.py` & `toga_core-0.4.4/src/toga/hardware/camera.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/hardware/location.py` & `toga_core-0.4.4/src/toga/hardware/location.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/icons.py` & `toga_core-0.4.4/src/toga/icons.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,19 +87,20 @@
     ):
         """Create a new icon.
 
         :param path: Base filename for the icon. The path can be an absolute file system
             path, or a path relative to the module that defines your Toga application
             class. This base filename should *not* contain an extension. If an extension
             is specified, it will be ignored. If the icon cannot be found, the default
-            icon will be :attr:`~toga.Icon.DEFAULT_ICON`.
+            icon will be :attr:`~toga.Icon.DEFAULT_ICON`. If an icon file is found, but
+            it cannot be loaded (due to a file format or permission error), an exception
+            will be raised.
         :param system: **For internal use only**
         """
         self.factory = get_platform_factory()
-
         try:
             # Try to load the icon with the given path snippet. If the request is for the
             # app icon, use ``resources/<app name>`` as the path.
             if path is _APP_ICON:
                 self.path = Path(f"resources/{toga.App.app.app_name}")
             else:
                 self.path = Path(path)
@@ -127,15 +128,15 @@
                     size=None,
                     extensions=self.factory.Icon.EXTENSIONS,
                     resource_path=resource_path,
                 )
 
             self._impl = self.factory.Icon(interface=self, path=full_path)
         except FileNotFoundError:
-            # Icon path couldn't be loaded. If the path is the sentinel for the app
+            # Icon path couldn't be found. If the path is the sentinel for the app
             # icon, and this isn't running as a script, fall back to the application
             # binary
             if path is _APP_ICON:
                 if Path(sys.executable).stem not in {
                     "python",
                     f"python{sys.version_info.major}",
                     f"python{sys.version_info.major}.{sys.version_info.minor}",
```

### Comparing `toga_core-0.4.3/src/toga/images.py` & `toga_core-0.4.4/src/toga/images.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/keys.py` & `toga_core-0.4.4/src/toga/keys.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/paths.py` & `toga_core-0.4.4/src/toga/paths.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/platform.py` & `toga_core-0.4.4/src/toga/platform.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/plugins/image_formats.py` & `toga_core-0.4.4/src/toga/plugins/image_formats.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/screens.py` & `toga_core-0.4.4/src/toga/screens.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/sources/accessors.py` & `toga_core-0.4.4/src/toga/sources/accessors.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/sources/base.py` & `toga_core-0.4.4/src/toga/sources/base.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/sources/list_source.py` & `toga_core-0.4.4/src/toga/sources/list_source.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/sources/tree_source.py` & `toga_core-0.4.4/src/toga/sources/tree_source.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/style/applicator.py` & `toga_core-0.4.4/src/toga/style/applicator.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/style/pack.py` & `toga_core-0.4.4/src/toga/style/pack.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/validators.py` & `toga_core-0.4.4/src/toga/validators.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/activityindicator.py` & `toga_core-0.4.4/src/toga/widgets/activityindicator.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/base.py` & `toga_core-0.4.4/src/toga/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/box.py` & `toga_core-0.4.4/src/toga/widgets/box.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/button.py` & `toga_core-0.4.4/src/toga/widgets/button.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/canvas.py` & `toga_core-0.4.4/src/toga/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/dateinput.py` & `toga_core-0.4.4/src/toga/widgets/dateinput.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/detailedlist.py` & `toga_core-0.4.4/src/toga/widgets/detailedlist.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/divider.py` & `toga_core-0.4.4/src/toga/widgets/divider.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/imageview.py` & `toga_core-0.4.4/src/toga/widgets/imageview.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/label.py` & `toga_core-0.4.4/src/toga/widgets/label.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/mapview.py` & `toga_core-0.4.4/src/toga/widgets/mapview.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/multilinetextinput.py` & `toga_core-0.4.4/src/toga/widgets/multilinetextinput.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/numberinput.py` & `toga_core-0.4.4/src/toga/widgets/numberinput.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/optioncontainer.py` & `toga_core-0.4.4/src/toga/widgets/optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/progressbar.py` & `toga_core-0.4.4/src/toga/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/scrollcontainer.py` & `toga_core-0.4.4/src/toga/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/selection.py` & `toga_core-0.4.4/src/toga/widgets/selection.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/slider.py` & `toga_core-0.4.4/src/toga/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/splitcontainer.py` & `toga_core-0.4.4/src/toga/widgets/splitcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/switch.py` & `toga_core-0.4.4/src/toga/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/table.py` & `toga_core-0.4.4/src/toga/widgets/table.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/textinput.py` & `toga_core-0.4.4/src/toga/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/timeinput.py` & `toga_core-0.4.4/src/toga/widgets/timeinput.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/tree.py` & `toga_core-0.4.4/src/toga/widgets/tree.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/widgets/webview.py` & `toga_core-0.4.4/src/toga/widgets/webview.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga/window.py` & `toga_core-0.4.4/src/toga/window.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga_core.egg-info/PKG-INFO` & `toga_core-0.4.4/src/toga_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-core
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Python native, OS native GUI toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
```

### Comparing `toga_core-0.4.3/src/toga_core.egg-info/SOURCES.txt` & `toga_core-0.4.4/src/toga_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/src/toga_core.egg-info/requires.txt` & `toga_core-0.4.4/src/toga_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/app/test_app.py` & `toga_core-0.4.4/tests/app/test_app.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/app/test_documentapp.py` & `toga_core-0.4.4/tests/app/test_documentapp.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/app/test_mainwindow.py` & `toga_core-0.4.4/tests/app/test_mainwindow.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/app/test_screens.py` & `toga_core-0.4.4/tests/app/test_screens.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/app/test_widget_registry.py` & `toga_core-0.4.4/tests/app/test_widget_registry.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/app/test_windowset.py` & `toga_core-0.4.4/tests/app/test_windowset.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/command/conftest.py` & `toga_core-0.4.4/tests/command/conftest.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/command/test_command.py` & `toga_core-0.4.4/tests/command/test_command.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/command/test_commandset.py` & `toga_core-0.4.4/tests/command/test_commandset.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/command/test_group.py` & `toga_core-0.4.4/tests/command/test_group.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/conftest.py` & `toga_core-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/hardware/test_camera.py` & `toga_core-0.4.4/tests/hardware/test_camera.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/hardware/test_location.py` & `toga_core-0.4.4/tests/hardware/test_location.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/resources/blue.png` & `toga_core-0.4.4/tests/resources/blue.png`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/resources/orange.bmp` & `toga_core-0.4.4/tests/resources/orange.bmp`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/resources/orange.png` & `toga_core-0.4.4/tests/resources/orange.png`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/resources/photo.png` & `toga_core-0.4.4/tests/resources/photo.png`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/resources/red-32.png` & `toga_core-0.4.4/tests/resources/red-32.png`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/resources/red-72.png` & `toga_core-0.4.4/tests/resources/red-72.png`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/resources/red.png` & `toga_core-0.4.4/tests/resources/red.png`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/resources/sample-dummy.png` & `toga_core-0.4.4/tests/resources/sample-dummy.png`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/resources/sample.png` & `toga_core-0.4.4/tests/resources/sample.png`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/resources/toga.png` & `toga_core-0.4.4/tests/resources/toga.png`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/sources/test_accessors.py` & `toga_core-0.4.4/tests/sources/test_accessors.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/sources/test_list_source.py` & `toga_core-0.4.4/tests/sources/test_list_source.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/sources/test_node.py` & `toga_core-0.4.4/tests/sources/test_node.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/sources/test_row.py` & `toga_core-0.4.4/tests/sources/test_row.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/sources/test_source.py` & `toga_core-0.4.4/tests/sources/test_source.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/sources/test_tree_source.py` & `toga_core-0.4.4/tests/sources/test_tree_source.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/sources/test_value_source.py` & `toga_core-0.4.4/tests/sources/test_value_source.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/style/pack/layout/test_beeliza.py` & `toga_core-0.4.4/tests/style/pack/layout/test_beeliza.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/style/pack/layout/test_column_alignment.py` & `toga_core-0.4.4/tests/style/pack/layout/test_column_alignment.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/style/pack/layout/test_fixed.py` & `toga_core-0.4.4/tests/style/pack/layout/test_fixed.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/style/pack/layout/test_flex.py` & `toga_core-0.4.4/tests/style/pack/layout/test_flex.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/style/pack/layout/test_row_alignment.py` & `toga_core-0.4.4/tests/style/pack/layout/test_row_alignment.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/style/pack/layout/test_rtl.py` & `toga_core-0.4.4/tests/style/pack/layout/test_rtl.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/style/pack/layout/test_tutorial0.py` & `toga_core-0.4.4/tests/style/pack/layout/test_tutorial0.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/style/pack/layout/test_tutorial1.py` & `toga_core-0.4.4/tests/style/pack/layout/test_tutorial1.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/style/pack/layout/test_tutorial3.py` & `toga_core-0.4.4/tests/style/pack/layout/test_tutorial3.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/style/pack/test_apply.py` & `toga_core-0.4.4/tests/style/pack/test_apply.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/style/pack/test_css.py` & `toga_core-0.4.4/tests/style/pack/test_css.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/style/pack/utils.py` & `toga_core-0.4.4/tests/style/pack/utils.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/style/test_applicator.py` & `toga_core-0.4.4/tests/style/test_applicator.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/test_documents.py` & `toga_core-0.4.4/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/test_fonts.py` & `toga_core-0.4.4/tests/test_fonts.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/test_handlers.py` & `toga_core-0.4.4/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/test_icons.py` & `toga_core-0.4.4/tests/test_icons.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,28 +109,48 @@
     # impl/interface round trips
     assert icon._impl.interface == icon
 
     # The icon's path is fully qualified
     assert icon._impl.path == final_paths
 
 
-def test_create_fallback(app, capsys):
+def test_create_fallback_missing(monkeypatch, app, capsys):
     """If a resource doesn't exist, a fallback icon is used."""
+    # Prime the dummy so the app icon cannot be loaded
+    monkeypatch.setattr(
+        DummyIcon,
+        "ICON_FAILURE",
+        FileNotFoundError(),
+    )
+
     icon = toga.Icon("resources/missing")
 
     assert icon._impl is not None
     assert icon._impl.interface == toga.Icon.DEFAULT_ICON
 
     # A warning was printed; allow for windows separators
     assert (
         "WARNING: Can't find icon resources/missing"
         in capsys.readouterr().out.replace("\\", "/")
     )
 
 
+def test_create_fallback_unloadable(monkeypatch, app, capsys):
+    """If a resource exists, but can't be loaded, an error is raised."""
+    # Prime the dummy so the app icon cannot be loaded
+    monkeypatch.setattr(
+        DummyIcon,
+        "ICON_FAILURE",
+        ValueError("Icon could not be loaded"),
+    )
+
+    with pytest.raises(ValueError):
+        toga.Icon("resources/sample")
+
+
 def test_create_fallback_variants(monkeypatch, app, capsys):
     """If a resource with size variants doesn't exist, a fallback icon is used."""
     monkeypatch.setattr(DummyIcon, "SIZES", [32, 72])
 
     icon = toga.Icon("resources/missing")
 
     assert icon._impl is not None
@@ -160,15 +180,15 @@
     assert icon._impl.path == Path(APP_RESOURCES / "sample.png")
 
     # No warning was printed, as the app icon exists.
     assert capsys.readouterr().out == ""
 
 
 def test_create_app_icon_missing(monkeypatch, app, capsys):
-    """The app icon can be constructed"""
+    """If the app icon is missing, a fallback is used"""
     # When running under pytest, code will identify as running as a script
 
     # Load the app default icon.
     icon = toga.Icon(_APP_ICON)
 
     # The impl is the app icon.
     assert icon._impl is not None
@@ -192,17 +212,21 @@
     assert icon._impl.path == "<APP ICON>"
 
     # No warning was printed, as we're running as a script.
     assert capsys.readouterr().out == ""
 
 
 def test_create_app_icon_missing_non_script(monkeypatch, app, capsys):
-    """The binary executableThe app icon can be reset to the default"""
-    # Prime the dummy so the app icon cannot be loaded
-    monkeypatch.setattr(DummyIcon, "ICON_EXISTS", False)
+    """If the icon from binary executable cannot be found, the app icon is reset to the default"""
+    # Prime the dummy so the app icon cannot be found
+    monkeypatch.setattr(
+        DummyIcon,
+        "ICON_FAILURE",
+        FileNotFoundError(),
+    )
 
     # Patch sys.executable so the test looks like it's running as a packaged binary
     monkeypatch.setattr(sys, "executable", "/path/to/App")
 
     # Load the app default icon
     icon = toga.Icon(_APP_ICON)
```

### Comparing `toga_core-0.4.3/tests/test_images.py` & `toga_core-0.4.4/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/test_keys.py` & `toga_core-0.4.4/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/test_paths.py` & `toga_core-0.4.4/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/test_platform.py` & `toga_core-0.4.4/tests/test_platform.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/test_validators.py` & `toga_core-0.4.4/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/testbed/interactive.py` & `toga_core-0.4.4/tests/testbed/interactive.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/testbed/subclassed/app.py` & `toga_core-0.4.4/tests/testbed/subclassed/app.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/canvas/conftest.py` & `toga_core-0.4.4/tests/widgets/canvas/conftest.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/canvas/test_canvas.py` & `toga_core-0.4.4/tests/widgets/canvas/test_canvas.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/canvas/test_context_objects.py` & `toga_core-0.4.4/tests/widgets/canvas/test_context_objects.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/canvas/test_draw_operations.py` & `toga_core-0.4.4/tests/widgets/canvas/test_draw_operations.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/canvas/test_helpers.py` & `toga_core-0.4.4/tests/widgets/canvas/test_helpers.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_activityindicator.py` & `toga_core-0.4.4/tests/widgets/test_activityindicator.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_base.py` & `toga_core-0.4.4/tests/widgets/test_base.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_box.py` & `toga_core-0.4.4/tests/widgets/test_box.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_button.py` & `toga_core-0.4.4/tests/widgets/test_button.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_dateinput.py` & `toga_core-0.4.4/tests/widgets/test_dateinput.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_detailedlist.py` & `toga_core-0.4.4/tests/widgets/test_detailedlist.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_divider.py` & `toga_core-0.4.4/tests/widgets/test_divider.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_imageview.py` & `toga_core-0.4.4/tests/widgets/test_imageview.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_label.py` & `toga_core-0.4.4/tests/widgets/test_label.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_mapview.py` & `toga_core-0.4.4/tests/widgets/test_mapview.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_multilinetextinput.py` & `toga_core-0.4.4/tests/widgets/test_multilinetextinput.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_numberinput.py` & `toga_core-0.4.4/tests/widgets/test_numberinput.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_optioncontainer.py` & `toga_core-0.4.4/tests/widgets/test_optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_passwordinput.py` & `toga_core-0.4.4/tests/widgets/test_passwordinput.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_progressbar.py` & `toga_core-0.4.4/tests/widgets/test_progressbar.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_scrollcontainer.py` & `toga_core-0.4.4/tests/widgets/test_scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_selection.py` & `toga_core-0.4.4/tests/widgets/test_selection.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_slider.py` & `toga_core-0.4.4/tests/widgets/test_slider.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_splitcontainer.py` & `toga_core-0.4.4/tests/widgets/test_splitcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_switch.py` & `toga_core-0.4.4/tests/widgets/test_switch.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_table.py` & `toga_core-0.4.4/tests/widgets/test_table.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_textinput.py` & `toga_core-0.4.4/tests/widgets/test_textinput.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_timeinput.py` & `toga_core-0.4.4/tests/widgets/test_timeinput.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_tree.py` & `toga_core-0.4.4/tests/widgets/test_tree.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/widgets/test_webview.py` & `toga_core-0.4.4/tests/widgets/test_webview.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/window/test_filtered_widget_registry.py` & `toga_core-0.4.4/tests/window/test_filtered_widget_registry.py`

 * *Files identical despite different names*

### Comparing `toga_core-0.4.3/tests/window/test_window.py` & `toga_core-0.4.4/tests/window/test_window.py`

 * *Files identical despite different names*

