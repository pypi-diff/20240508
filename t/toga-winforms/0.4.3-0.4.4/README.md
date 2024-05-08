# Comparing `tmp/toga_winforms-0.4.3.tar.gz` & `tmp/toga_winforms-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga_winforms-0.4.3.tar", last modified: Mon May  6 06:43:39 2024, max compression
+gzip compressed data, was "toga_winforms-0.4.4.tar", last modified: Wed May  8 00:59:00 2024, max compression
```

## Comparing `toga_winforms-0.4.3.tar` & `toga_winforms-0.4.4.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.325712 toga_winforms-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-06 06:43:39.325712 toga_winforms-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:39.325712 toga_winforms-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.305712 toga_winforms-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.309712 toga_winforms-0.4.3/src/toga_winforms/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15821 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.309712 toga_winforms-0.4.3/src/toga_winforms/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/keys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.313712 toga_winforms-0.4.3/src/toga_winforms/libs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.313712 toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)   306600 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/Microsoft.Web.WebView2.Core.dll
--rw-r--r--   0 runner    (1001) docker     (127)    35280 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/Microsoft.Web.WebView2.WinForms.dll
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.313712 toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/arm64/
--rw-r--r--   0 runner    (1001) docker     (127)   127912 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/arm64/WebView2Loader.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.313712 toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/x64/
--rw-r--r--   0 runner    (1001) docker     (127)   141224 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/x64/WebView2Loader.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.313712 toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/x86/
--rw-r--r--   0 runner    (1001) docker     (127)   110504 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/x86/WebView2Loader.dll
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/libs/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/libs/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/libs/proactor.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/libs/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.313712 toga_winforms-0.4.3/src/toga_winforms/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   370070 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/resources/toga.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/screens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.321712 toga_winforms-0.4.3/src/toga_winforms/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)    11920 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/dateinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/mapview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/timeinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/src/toga_winforms/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.325712 toga_winforms-0.4.3/src/toga_winforms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-06 06:43:39.000000 toga_winforms-0.4.3/src/toga_winforms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-06 06:43:39.000000 toga_winforms-0.4.3/src/toga_winforms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:39.000000 toga_winforms-0.4.3/src/toga_winforms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-06 06:43:39.000000 toga_winforms-0.4.3/src/toga_winforms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-06 06:43:39.000000 toga_winforms-0.4.3/src/toga_winforms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-06 06:43:39.000000 toga_winforms-0.4.3/src/toga_winforms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.321712 toga_winforms-0.4.3/tests_backend/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/probe.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/screens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:39.325712 toga_winforms-0.4.3/tests_backend/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/dateinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/detailedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/mapview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/multilinetextinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/optioncontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/scrollcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/splitcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/timeinput.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/widgets/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-06 06:43:04.000000 toga_winforms-0.4.3/tests_backend/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:00.359329 toga_winforms-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-08 00:59:00.359329 toga_winforms-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:59:00.359329 toga_winforms-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:00.339329 toga_winforms-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:00.343329 toga_winforms-0.4.4/src/toga_winforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15821 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:00.343329 toga_winforms-0.4.4/src/toga_winforms/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:00.347329 toga_winforms-0.4.4/src/toga_winforms/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:00.347329 toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)   306600 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/Microsoft.Web.WebView2.Core.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    35280 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/Microsoft.Web.WebView2.WinForms.dll
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:00.347329 toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/arm64/
+-rw-r--r--   0 runner    (1001) docker     (127)   127912 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/arm64/WebView2Loader.dll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:00.347329 toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/x64/
+-rw-r--r--   0 runner    (1001) docker     (127)   141224 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/x64/WebView2Loader.dll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:00.347329 toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/x86/
+-rw-r--r--   0 runner    (1001) docker     (127)   110504 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/x86/WebView2Loader.dll
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/libs/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/libs/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/libs/proactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/libs/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:00.347329 toga_winforms-0.4.4/src/toga_winforms/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   370070 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/resources/toga.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:00.355329 toga_winforms-0.4.4/src/toga_winforms/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11920 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/dateinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/timeinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/src/toga_winforms/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:00.359329 toga_winforms-0.4.4/src/toga_winforms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-08 00:59:00.000000 toga_winforms-0.4.4/src/toga_winforms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-08 00:59:00.000000 toga_winforms-0.4.4/src/toga_winforms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:59:00.000000 toga_winforms-0.4.4/src/toga_winforms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 00:59:00.000000 toga_winforms-0.4.4/src/toga_winforms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 00:59:00.000000 toga_winforms-0.4.4/src/toga_winforms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 00:59:00.000000 toga_winforms-0.4.4/src/toga_winforms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:00.355329 toga_winforms-0.4.4/tests_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:00.359329 toga_winforms-0.4.4/tests_backend/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/dateinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/mapview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/timeinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-08 00:58:29.000000 toga_winforms-0.4.4/tests_backend/window.py
```

### Comparing `toga_winforms-0.4.3/LICENSE` & `toga_winforms-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/PKG-INFO` & `toga_winforms-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-winforms
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Windows backend for the Toga widget toolkit using the WinForms API.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -27,15 +27,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pythonnet>=3.0.0
-Requires-Dist: toga-core==0.4.3
+Requires-Dist: toga-core==0.4.4
 
 toga-winforms
 =============
 
 A Microsoft .NET backend for the `Toga widget toolkit`_ utilizing the WinForms API.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
```

### Comparing `toga_winforms-0.4.3/README.rst` & `toga_winforms-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/pyproject.toml` & `toga_winforms-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/__init__.py` & `toga_winforms-0.4.4/src/toga_winforms/__init__.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/app.py` & `toga_winforms-0.4.4/src/toga_winforms/app.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/container.py` & `toga_winforms-0.4.4/src/toga_winforms/container.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/dialogs.py` & `toga_winforms-0.4.4/src/toga_winforms/dialogs.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/factory.py` & `toga_winforms-0.4.4/src/toga_winforms/factory.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/fonts.py` & `toga_winforms-0.4.4/src/toga_winforms/fonts.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/icons.py` & `toga_winforms-0.4.4/src/toga_winforms/icons.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/images.py` & `toga_winforms-0.4.4/src/toga_winforms/images.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/keys.py` & `toga_winforms-0.4.4/src/toga_winforms/keys.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/LICENSE.md` & `toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/Microsoft.Web.WebView2.Core.dll` & `toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/Microsoft.Web.WebView2.Core.dll`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/Microsoft.Web.WebView2.WinForms.dll` & `toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/Microsoft.Web.WebView2.WinForms.dll`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/README.md` & `toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/README.md`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/arm64/WebView2Loader.dll` & `toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/arm64/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/x64/WebView2Loader.dll` & `toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/x64/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/libs/WebView2/x86/WebView2Loader.dll` & `toga_winforms-0.4.4/src/toga_winforms/libs/WebView2/x86/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/libs/extensions.py` & `toga_winforms-0.4.4/src/toga_winforms/libs/extensions.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/libs/fonts.py` & `toga_winforms-0.4.4/src/toga_winforms/libs/fonts.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/libs/proactor.py` & `toga_winforms-0.4.4/src/toga_winforms/libs/proactor.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/libs/wrapper.py` & `toga_winforms-0.4.4/src/toga_winforms/libs/wrapper.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/paths.py` & `toga_winforms-0.4.4/src/toga_winforms/paths.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/resources/toga.ico` & `toga_winforms-0.4.4/src/toga_winforms/resources/toga.ico`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/screens.py` & `toga_winforms-0.4.4/src/toga_winforms/screens.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/base.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/button.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/button.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/canvas.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/dateinput.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/dateinput.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/detailedlist.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/detailedlist.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/divider.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/divider.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/imageview.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/imageview.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/label.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/label.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/mapview.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/mapview.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
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

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/multilinetextinput.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/multilinetextinput.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/numberinput.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/numberinput.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/optioncontainer.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/progressbar.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/scrollcontainer.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/selection.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/selection.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/slider.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/splitcontainer.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/splitcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/switch.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/table.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/table.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/textinput.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/timeinput.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/timeinput.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/widgets/webview.py` & `toga_winforms-0.4.4/src/toga_winforms/widgets/webview.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms/window.py` & `toga_winforms-0.4.4/src/toga_winforms/window.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/src/toga_winforms.egg-info/PKG-INFO` & `toga_winforms-0.4.4/src/toga_winforms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-winforms
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Windows backend for the Toga widget toolkit using the WinForms API.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -27,15 +27,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pythonnet>=3.0.0
-Requires-Dist: toga-core==0.4.3
+Requires-Dist: toga-core==0.4.4
 
 toga-winforms
 =============
 
 A Microsoft .NET backend for the `Toga widget toolkit`_ utilizing the WinForms API.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
```

### Comparing `toga_winforms-0.4.3/src/toga_winforms.egg-info/SOURCES.txt` & `toga_winforms-0.4.4/src/toga_winforms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/app.py` & `toga_winforms-0.4.4/tests_backend/app.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/fonts.py` & `toga_winforms-0.4.4/tests_backend/fonts.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/icons.py` & `toga_winforms-0.4.4/tests_backend/icons.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/probe.py` & `toga_winforms-0.4.4/tests_backend/probe.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/base.py` & `toga_winforms-0.4.4/tests_backend/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/button.py` & `toga_winforms-0.4.4/tests_backend/widgets/button.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/canvas.py` & `toga_winforms-0.4.4/tests_backend/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/dateinput.py` & `toga_winforms-0.4.4/tests_backend/widgets/dateinput.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/mapview.py` & `toga_winforms-0.4.4/tests_backend/widgets/mapview.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/multilinetextinput.py` & `toga_winforms-0.4.4/tests_backend/widgets/multilinetextinput.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/numberinput.py` & `toga_winforms-0.4.4/tests_backend/widgets/numberinput.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/optioncontainer.py` & `toga_winforms-0.4.4/tests_backend/widgets/optioncontainer.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/progressbar.py` & `toga_winforms-0.4.4/tests_backend/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/properties.py` & `toga_winforms-0.4.4/tests_backend/widgets/properties.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/scrollcontainer.py` & `toga_winforms-0.4.4/tests_backend/widgets/scrollcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/selection.py` & `toga_winforms-0.4.4/tests_backend/widgets/selection.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/slider.py` & `toga_winforms-0.4.4/tests_backend/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/splitcontainer.py` & `toga_winforms-0.4.4/tests_backend/widgets/splitcontainer.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/table.py` & `toga_winforms-0.4.4/tests_backend/widgets/table.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/textinput.py` & `toga_winforms-0.4.4/tests_backend/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/widgets/timeinput.py` & `toga_winforms-0.4.4/tests_backend/widgets/timeinput.py`

 * *Files identical despite different names*

### Comparing `toga_winforms-0.4.3/tests_backend/window.py` & `toga_winforms-0.4.4/tests_backend/window.py`

 * *Files identical despite different names*

