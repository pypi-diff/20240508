# Comparing `tmp/Photini-2024.4.0.tar.gz` & `tmp/Photini-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jim/Documents/projects/Photini/main/dist/tmp8t4cthkf/Photini-2024.4.0.tar", last modified: Thu Apr 25 08:47:45 2024, max compression
+gzip compressed data, was "/home/jim/Documents/projects/Photini/main/dist/tmpepv3v3qf/Photini-2024.5.0.tar", last modified: Wed May  8 10:00:14 2024, max compression
```

## Comparing `Photini-2024.4.0.tar` & `Photini-2024.5.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/
--rw-r--r--   0 jim       (1026) users      (100)    17042 2024-04-25 08:46:39.000000 Photini-2024.4.0/CHANGELOG.txt
--rw-r--r--   0 jim       (1026) users      (100)    35147 2023-09-11 09:27:18.000000 Photini-2024.4.0/LICENSE.txt
--rw-r--r--   0 jim       (1026) users      (100)      529 2023-09-11 09:27:18.000000 Photini-2024.4.0/MANIFEST.in
--rw-r--r--   0 jim       (1026) users      (100)     9342 2024-04-25 08:47:45.000000 Photini-2024.4.0/PKG-INFO
--rw-r--r--   0 jim       (1026) users      (100)     8245 2024-04-25 08:46:39.000000 Photini-2024.4.0/README.rst
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/custom_build/
--rw-r--r--   0 jim       (1026) users      (100)     2294 2023-09-11 09:27:18.000000 Photini-2024.4.0/custom_build/backend.py
--rw-r--r--   0 jim       (1026) users      (100)     3659 2024-04-25 08:46:39.000000 Photini-2024.4.0/pyproject.toml
--rw-r--r--   0 jim       (1026) users      (100)       38 2024-04-25 08:47:45.000000 Photini-2024.4.0/setup.cfg
--rw-r--r--   0 jim       (1026) users      (100)     2562 2024-02-01 09:20:49.000000 Photini-2024.4.0/setup.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/Photini.egg-info/
--rw-r--r--   0 jim       (1026) users      (100)     1746 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/Photini.egg-info/SOURCES.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/photini/
--rw-r--r--   0 jim       (1026) users      (100)     1048 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/__init__.py
--rw-r--r--   0 jim       (1026) users      (100)      917 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/__main__.py
--rw-r--r--   0 jim       (1026) users      (100)      148 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/_version.py
--rw-r--r--   0 jim       (1026) users      (100)    19671 2024-02-17 12:07:53.000000 Photini-2024.4.0/src/photini/address.py
--rw-r--r--   0 jim       (1026) users      (100)     4704 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/bingmap.py
--rw-r--r--   0 jim       (1026) users      (100)     5060 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/configstore.py
--rw-r--r--   0 jim       (1026) users      (100)     6890 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/cv.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/photini/data/
--rw-r--r--   0 jim       (1026) users      (100)    35147 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/LICENSE.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/photini/data/icons/
--rw-r--r--   0 jim       (1026) users      (100)    14554 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/icons/photini_128.png
--rw-r--r--   0 jim       (1026) users      (100)     3262 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/icons/photini_48.png
--rw-r--r--   0 jim       (1026) users      (100)    86598 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/icons/photini_win.ico
--rw-r--r--   0 jim       (1026) users      (100)     2205 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/data/keys.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/photini/data/lang/
--rw-r--r--   0 jim       (1026) users      (100)    22126 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.ca.qm
--rw-r--r--   0 jim       (1026) users      (100)    32936 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.cs.qm
--rw-r--r--   0 jim       (1026) users      (100)    47788 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.de.qm
--rw-r--r--   0 jim       (1026) users      (100)    51535 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.en.qm
--rw-r--r--   0 jim       (1026) users      (100)    55444 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.es.qm
--rw-r--r--   0 jim       (1026) users      (100)    43003 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.fr.qm
--rw-r--r--   0 jim       (1026) users      (100)    55640 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.it.qm
--rw-r--r--   0 jim       (1026) users      (100)     2026 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.ko.qm
--rw-r--r--   0 jim       (1026) users      (100)    21271 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.nb.qm
--rw-r--r--   0 jim       (1026) users      (100)    14017 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.pl.qm
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/photini/data/linux/
--rw-r--r--   0 jim       (1026) users      (100)      321 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/linux/photini.desktop
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/photini/data/map/
--rw-r--r--   0 jim       (1026) users      (100)     7400 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/data/map/bingmap.js
--rw-r--r--   0 jim       (1026) users      (100)      209 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/map/circle_blue.png
--rw-r--r--   0 jim       (1026) users      (100)      207 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/map/circle_red.png
--rw-r--r--   0 jim       (1026) users      (100)     6186 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/data/map/googlemap.js
--rw-r--r--   0 jim       (1026) users      (100)     5687 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/data/map/mapboxmap.js
--rw-r--r--   0 jim       (1026) users      (100)     1867 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/map/pin_grey.png
--rw-r--r--   0 jim       (1026) users      (100)     2016 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/map/pin_red.png
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/photini/data/windows/
--rw-r--r--   0 jim       (1026) users      (100)     2638 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/windows/install_shortcuts.vbs
--rw-r--r--   0 jim       (1026) users      (100)    13496 2023-09-11 09:44:02.000000 Photini-2024.4.0/src/photini/descriptive.py
--rw-r--r--   0 jim       (1026) users      (100)    23113 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/editor.py
--rw-r--r--   0 jim       (1026) users      (100)     8435 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/editsettings.py
--rw-r--r--   0 jim       (1026) users      (100)    34091 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/exiv2.py
--rw-r--r--   0 jim       (1026) users      (100)     3287 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/ffmpeg.py
--rw-r--r--   0 jim       (1026) users      (100)    33323 2023-09-11 09:44:02.000000 Photini-2024.4.0/src/photini/flickr.py
--rw-r--r--   0 jim       (1026) users      (100)     4264 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/googlemap.py
--rw-r--r--   0 jim       (1026) users      (100)    13099 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/googlephotos.py
--rw-r--r--   0 jim       (1026) users      (100)     4504 2023-09-11 09:44:02.000000 Photini-2024.4.0/src/photini/gpximporter.py
--rw-r--r--   0 jim       (1026) users      (100)    40589 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/imagelist.py
--rw-r--r--   0 jim       (1026) users      (100)    27950 2023-09-11 09:44:02.000000 Photini-2024.4.0/src/photini/importer.py
--rw-r--r--   0 jim       (1026) users      (100)    27318 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/ipernity.py
--rw-r--r--   0 jim       (1026) users      (100)     5491 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/loggerwindow.py
--rw-r--r--   0 jim       (1026) users      (100)     4228 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/mapboxmap.py
--rw-r--r--   0 jim       (1026) users      (100)    38967 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/metadata.py
--rw-r--r--   0 jim       (1026) users      (100)    21920 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/ownership.py
--rw-r--r--   0 jim       (1026) users      (100)    25878 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/photinimap.py
--rw-r--r--   0 jim       (1026) users      (100)    37798 2023-09-11 09:44:02.000000 Photini-2024.4.0/src/photini/pixelfed.py
--rw-r--r--   0 jim       (1026) users      (100)    10708 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/pyqt.py
--rw-r--r--   0 jim       (1026) users      (100)    37963 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/regions.py
--rw-r--r--   0 jim       (1026) users      (100)     7689 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/scripts.py
--rw-r--r--   0 jim       (1026) users      (100)     3869 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/spelling.py
--rw-r--r--   0 jim       (1026) users      (100)    40941 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/technical.py
--rw-r--r--   0 jim       (1026) users      (100)    72730 2024-02-17 12:07:53.000000 Photini-2024.4.0/src/photini/types.py
--rw-r--r--   0 jim       (1026) users      (100)    46234 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/uploader.py
--rw-r--r--   0 jim       (1026) users      (100)    36486 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/widgets.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-05-08 10:00:14.000000 Photini-2024.5.0/
+-rw-r--r--   0 jim       (1026) users      (100)    17178 2024-05-08 09:59:24.000000 Photini-2024.5.0/CHANGELOG.txt
+-rw-r--r--   0 jim       (1026) users      (100)    35147 2023-09-11 09:27:18.000000 Photini-2024.5.0/LICENSE.txt
+-rw-r--r--   0 jim       (1026) users      (100)      529 2023-09-11 09:27:18.000000 Photini-2024.5.0/MANIFEST.in
+-rw-r--r--   0 jim       (1026) users      (100)     9342 2024-05-08 10:00:14.000000 Photini-2024.5.0/PKG-INFO
+-rw-r--r--   0 jim       (1026) users      (100)     8245 2024-04-25 08:46:39.000000 Photini-2024.5.0/README.rst
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-05-08 10:00:14.000000 Photini-2024.5.0/custom_build/
+-rw-r--r--   0 jim       (1026) users      (100)     2294 2023-09-11 09:27:18.000000 Photini-2024.5.0/custom_build/backend.py
+-rw-r--r--   0 jim       (1026) users      (100)     3659 2024-04-25 08:46:39.000000 Photini-2024.5.0/pyproject.toml
+-rw-r--r--   0 jim       (1026) users      (100)       38 2024-05-08 10:00:14.000000 Photini-2024.5.0/setup.cfg
+-rw-r--r--   0 jim       (1026) users      (100)     2562 2024-02-01 09:20:49.000000 Photini-2024.5.0/setup.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-05-08 10:00:14.000000 Photini-2024.5.0/src/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-05-08 10:00:14.000000 Photini-2024.5.0/src/Photini.egg-info/
+-rw-r--r--   0 jim       (1026) users      (100)     1787 2024-05-08 10:00:13.000000 Photini-2024.5.0/src/Photini.egg-info/SOURCES.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-05-08 10:00:14.000000 Photini-2024.5.0/src/photini/
+-rw-r--r--   0 jim       (1026) users      (100)     1048 2024-02-01 09:20:49.000000 Photini-2024.5.0/src/photini/__init__.py
+-rw-r--r--   0 jim       (1026) users      (100)      917 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/__main__.py
+-rw-r--r--   0 jim       (1026) users      (100)      148 2024-05-08 10:00:13.000000 Photini-2024.5.0/src/photini/_version.py
+-rw-r--r--   0 jim       (1026) users      (100)    19671 2024-02-17 12:07:53.000000 Photini-2024.5.0/src/photini/address.py
+-rw-r--r--   0 jim       (1026) users      (100)     4766 2024-05-08 09:59:24.000000 Photini-2024.5.0/src/photini/bingmap.py
+-rw-r--r--   0 jim       (1026) users      (100)     5060 2024-02-01 09:20:49.000000 Photini-2024.5.0/src/photini/configstore.py
+-rw-r--r--   0 jim       (1026) users      (100)     6890 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/cv.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-05-08 10:00:14.000000 Photini-2024.5.0/src/photini/data/
+-rw-r--r--   0 jim       (1026) users      (100)    35147 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/data/LICENSE.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-05-08 10:00:14.000000 Photini-2024.5.0/src/photini/data/icons/
+-rw-r--r--   0 jim       (1026) users      (100)    14554 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/data/icons/photini_128.png
+-rw-r--r--   0 jim       (1026) users      (100)     3262 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/data/icons/photini_48.png
+-rw-r--r--   0 jim       (1026) users      (100)    86598 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/data/icons/photini_win.ico
+-rw-r--r--   0 jim       (1026) users      (100)     2205 2024-04-25 08:46:39.000000 Photini-2024.5.0/src/photini/data/keys.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-05-08 10:00:14.000000 Photini-2024.5.0/src/photini/data/lang/
+-rw-r--r--   0 jim       (1026) users      (100)    22126 2024-05-08 10:00:13.000000 Photini-2024.5.0/src/photini/data/lang/photini.ca.qm
+-rw-r--r--   0 jim       (1026) users      (100)    32936 2024-05-08 10:00:13.000000 Photini-2024.5.0/src/photini/data/lang/photini.cs.qm
+-rw-r--r--   0 jim       (1026) users      (100)    47788 2024-05-08 10:00:13.000000 Photini-2024.5.0/src/photini/data/lang/photini.de.qm
+-rw-r--r--   0 jim       (1026) users      (100)    51535 2024-05-08 10:00:13.000000 Photini-2024.5.0/src/photini/data/lang/photini.en.qm
+-rw-r--r--   0 jim       (1026) users      (100)    55444 2024-05-08 10:00:13.000000 Photini-2024.5.0/src/photini/data/lang/photini.es.qm
+-rw-r--r--   0 jim       (1026) users      (100)    43003 2024-05-08 10:00:13.000000 Photini-2024.5.0/src/photini/data/lang/photini.fr.qm
+-rw-r--r--   0 jim       (1026) users      (100)    55640 2024-05-08 10:00:13.000000 Photini-2024.5.0/src/photini/data/lang/photini.it.qm
+-rw-r--r--   0 jim       (1026) users      (100)     2026 2024-05-08 10:00:13.000000 Photini-2024.5.0/src/photini/data/lang/photini.ko.qm
+-rw-r--r--   0 jim       (1026) users      (100)    21271 2024-05-08 10:00:13.000000 Photini-2024.5.0/src/photini/data/lang/photini.nb.qm
+-rw-r--r--   0 jim       (1026) users      (100)    14017 2024-05-08 10:00:13.000000 Photini-2024.5.0/src/photini/data/lang/photini.pl.qm
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-05-08 10:00:14.000000 Photini-2024.5.0/src/photini/data/linux/
+-rw-r--r--   0 jim       (1026) users      (100)      321 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/data/linux/photini.desktop
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-05-08 10:00:14.000000 Photini-2024.5.0/src/photini/data/map/
+-rw-r--r--   0 jim       (1026) users      (100)     7400 2024-02-01 09:20:49.000000 Photini-2024.5.0/src/photini/data/map/bingmap.js
+-rw-r--r--   0 jim       (1026) users      (100)      209 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/data/map/circle_blue.png
+-rw-r--r--   0 jim       (1026) users      (100)      207 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/data/map/circle_red.png
+-rw-r--r--   0 jim       (1026) users      (100)     6070 2024-05-08 09:59:24.000000 Photini-2024.5.0/src/photini/data/map/googlemap.js
+-rw-r--r--   0 jim       (1026) users      (100)     6459 2024-05-08 09:59:24.000000 Photini-2024.5.0/src/photini/data/map/googlemap_legacy.js
+-rw-r--r--   0 jim       (1026) users      (100)     5687 2024-02-01 09:20:49.000000 Photini-2024.5.0/src/photini/data/map/mapboxmap.js
+-rw-r--r--   0 jim       (1026) users      (100)     1867 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/data/map/pin_grey.png
+-rw-r--r--   0 jim       (1026) users      (100)     2016 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/data/map/pin_red.png
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-05-08 10:00:14.000000 Photini-2024.5.0/src/photini/data/windows/
+-rw-r--r--   0 jim       (1026) users      (100)     2638 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/data/windows/install_shortcuts.vbs
+-rw-r--r--   0 jim       (1026) users      (100)    13496 2023-09-11 09:44:02.000000 Photini-2024.5.0/src/photini/descriptive.py
+-rw-r--r--   0 jim       (1026) users      (100)    23113 2024-02-01 09:20:49.000000 Photini-2024.5.0/src/photini/editor.py
+-rw-r--r--   0 jim       (1026) users      (100)     8435 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/editsettings.py
+-rw-r--r--   0 jim       (1026) users      (100)    34091 2024-02-01 09:20:49.000000 Photini-2024.5.0/src/photini/exiv2.py
+-rw-r--r--   0 jim       (1026) users      (100)     3287 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/ffmpeg.py
+-rw-r--r--   0 jim       (1026) users      (100)    33323 2023-09-11 09:44:02.000000 Photini-2024.5.0/src/photini/flickr.py
+-rw-r--r--   0 jim       (1026) users      (100)     4764 2024-05-08 09:59:24.000000 Photini-2024.5.0/src/photini/googlemap.py
+-rw-r--r--   0 jim       (1026) users      (100)    13099 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/googlephotos.py
+-rw-r--r--   0 jim       (1026) users      (100)     4504 2023-09-11 09:44:02.000000 Photini-2024.5.0/src/photini/gpximporter.py
+-rw-r--r--   0 jim       (1026) users      (100)    40589 2024-04-25 08:46:39.000000 Photini-2024.5.0/src/photini/imagelist.py
+-rw-r--r--   0 jim       (1026) users      (100)    28455 2024-05-08 09:59:24.000000 Photini-2024.5.0/src/photini/importer.py
+-rw-r--r--   0 jim       (1026) users      (100)    27318 2024-02-01 09:20:49.000000 Photini-2024.5.0/src/photini/ipernity.py
+-rw-r--r--   0 jim       (1026) users      (100)     5491 2024-04-25 08:46:39.000000 Photini-2024.5.0/src/photini/loggerwindow.py
+-rw-r--r--   0 jim       (1026) users      (100)     4277 2024-05-08 09:59:24.000000 Photini-2024.5.0/src/photini/mapboxmap.py
+-rw-r--r--   0 jim       (1026) users      (100)    38967 2024-04-25 08:46:39.000000 Photini-2024.5.0/src/photini/metadata.py
+-rw-r--r--   0 jim       (1026) users      (100)    21920 2023-09-11 09:27:18.000000 Photini-2024.5.0/src/photini/ownership.py
+-rw-r--r--   0 jim       (1026) users      (100)    25833 2024-05-08 09:59:24.000000 Photini-2024.5.0/src/photini/photinimap.py
+-rw-r--r--   0 jim       (1026) users      (100)    37798 2023-09-11 09:44:02.000000 Photini-2024.5.0/src/photini/pixelfed.py
+-rw-r--r--   0 jim       (1026) users      (100)    10691 2024-05-08 09:59:24.000000 Photini-2024.5.0/src/photini/pyqt.py
+-rw-r--r--   0 jim       (1026) users      (100)    37963 2024-04-25 08:46:39.000000 Photini-2024.5.0/src/photini/regions.py
+-rw-r--r--   0 jim       (1026) users      (100)     7672 2024-05-08 09:59:24.000000 Photini-2024.5.0/src/photini/scripts.py
+-rw-r--r--   0 jim       (1026) users      (100)     3869 2024-04-25 08:46:39.000000 Photini-2024.5.0/src/photini/spelling.py
+-rw-r--r--   0 jim       (1026) users      (100)    40941 2024-02-01 09:20:49.000000 Photini-2024.5.0/src/photini/technical.py
+-rw-r--r--   0 jim       (1026) users      (100)    72730 2024-02-17 12:07:53.000000 Photini-2024.5.0/src/photini/types.py
+-rw-r--r--   0 jim       (1026) users      (100)    46234 2024-04-25 08:46:39.000000 Photini-2024.5.0/src/photini/uploader.py
+-rw-r--r--   0 jim       (1026) users      (100)    36486 2024-02-01 09:20:49.000000 Photini-2024.5.0/src/photini/widgets.py
```

### Comparing `Photini-2024.4.0/CHANGELOG.txt` & `Photini-2024.5.0/CHANGELOG.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see
 <http://www.gnu.org/licenses/>.
 
+Changes in v2024.5.0:
+  1/ Use deprecated Google Map marker with QtWebEngline v5.15.2 or lower.
+  2/ Copy files from camera in chunks.
+
 Changes in v2024.4.0:
   1/ Google Map no longer used deprecated marker.
   2/ Improved handling of multiple language configurations.
   3/ Pillow is now a required dependency.
 
 Changes in v2024.2.1:
   1/ Fix bug in LangAlt values without a default language.
```

### Comparing `Photini-2024.4.0/LICENSE.txt` & `Photini-2024.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/MANIFEST.in` & `Photini-2024.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/PKG-INFO` & `Photini-2024.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Photini
-Version: 2024.4.0
+Version: 2024.5.0
 Summary: Simple photo metadata editor
 Home-page: https://github.com/jim-easterbrook/Photini
 Author: Jim Easterbrook
 Author-email: jim@jim-easterbrook.me.uk
 License: GPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Photini-2024.4.0/README.rst` & `Photini-2024.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/custom_build/backend.py` & `Photini-2024.5.0/custom_build/backend.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/pyproject.toml` & `Photini-2024.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/setup.py` & `Photini-2024.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/Photini.egg-info/SOURCES.txt` & `Photini-2024.5.0/src/Photini.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,11 +54,12 @@
 src/photini/data/lang/photini.nb.qm
 src/photini/data/lang/photini.pl.qm
 src/photini/data/linux/photini.desktop
 src/photini/data/map/bingmap.js
 src/photini/data/map/circle_blue.png
 src/photini/data/map/circle_red.png
 src/photini/data/map/googlemap.js
+src/photini/data/map/googlemap_legacy.js
 src/photini/data/map/mapboxmap.js
 src/photini/data/map/pin_grey.png
 src/photini/data/map/pin_red.png
 src/photini/data/windows/install_shortcuts.vbs
```

### Comparing `Photini-2024.4.0/src/photini/__init__.py` & `Photini-2024.5.0/src/photini/__init__.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/__main__.py` & `Photini-2024.5.0/src/photini/__main__.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/address.py` & `Photini-2024.5.0/src/photini/address.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/bingmap.py` & `Photini-2024.5.0/src/photini/bingmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,16 @@
             url += '&setMkt=' + culture
             language, sep, region = culture.partition('-')
             url += '&setLang=' + language
         if self.app.options.test:
             url += '&branch=experimental'
         return '''    <script type="text/javascript"
       src="{}" async>
-    </script>'''.format(url)
+    </script>
+    <script type="text/javascript" src="bingmap.js"></script>'''.format(url)
 
     @catch_all
     def new_status(self, status):
         super(TabWidget, self).new_status(status)
         if 'session_id' in status:
             # use map session key to make API calls non-billable
             self.geocoder.api_key = status['session_id']
```

### Comparing `Photini-2024.4.0/src/photini/configstore.py` & `Photini-2024.5.0/src/photini/configstore.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/cv.py` & `Photini-2024.5.0/src/photini/cv.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/LICENSE.txt` & `Photini-2024.5.0/src/photini/data/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/icons/photini_128.png` & `Photini-2024.5.0/src/photini/data/icons/photini_128.png`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/icons/photini_48.png` & `Photini-2024.5.0/src/photini/data/icons/photini_48.png`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/icons/photini_win.ico` & `Photini-2024.5.0/src/photini/data/icons/photini_win.ico`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/keys.txt` & `Photini-2024.5.0/src/photini/data/keys.txt`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/lang/photini.ca.qm` & `Photini-2024.5.0/src/photini/data/lang/photini.ca.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/lang/photini.cs.qm` & `Photini-2024.5.0/src/photini/data/lang/photini.cs.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/lang/photini.de.qm` & `Photini-2024.5.0/src/photini/data/lang/photini.de.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/lang/photini.en.qm` & `Photini-2024.5.0/src/photini/data/lang/photini.en.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/lang/photini.es.qm` & `Photini-2024.5.0/src/photini/data/lang/photini.es.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/lang/photini.fr.qm` & `Photini-2024.5.0/src/photini/data/lang/photini.fr.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/lang/photini.it.qm` & `Photini-2024.5.0/src/photini/data/lang/photini.it.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/lang/photini.ko.qm` & `Photini-2024.5.0/src/photini/data/lang/photini.ko.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/lang/photini.nb.qm` & `Photini-2024.5.0/src/photini/data/lang/photini.nb.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/lang/photini.pl.qm` & `Photini-2024.5.0/src/photini/data/lang/photini.pl.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/map/bingmap.js` & `Photini-2024.5.0/src/photini/data/map/bingmap.js`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/map/googlemap.js` & `Photini-2024.5.0/src/photini/data/map/googlemap.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -98,62 +98,55 @@
         map.fitBounds(bounds);
     else if (mapBounds.intersects(bounds))
         map.panToBounds(bounds);
     else
         map.panTo(bounds.getCenter());
 }
 
-function newGPSCircle(active) {
-    var result = document.createElement("img");
-    result.src = active ? 'circle_red.png' : 'circle_blue.png';
-    result.style.transform = 'translate(0.5px,8.5px)';
-    return result;
-}
-
 function plotGPS(points) {
     for (var i = 0; i < points.length; i++) {
         var latlng = new google.maps.LatLng(points[i][0], points[i][1]);
         var id = points[i][2];
+        var circle = document.createElement("img");
+        circle.src = 'circle_blue.png';
+        circle.style.transform = 'translate(0.5px,8.5px)';
         gpsMarkers[id] = new google.maps.marker.AdvancedMarkerElement({
             map: map,
             position: latlng,
-            content: newGPSCircle(false),
+            content: circle,
             zIndex: 2
         });
     }
 }
 
 function enableGPS(ids) {
     for (var id in gpsMarkers)
-        gpsMarkers[id].content = newGPSCircle(ids.includes(id));
+        gpsMarkers[id].content.src =
+        ids.includes(id) ? 'circle_red.png' : 'circle_blue.png';
     gpsMarkers[id].zIndex = ids.includes(id) ? 3 : 2;
 }
 
 function clearGPS() {
     for (var id in gpsMarkers)
         gpsMarkers[id].setMap(null);
     gpsMarkers = {};
 }
 
-function newIcon(active) {
-    var result = document.createElement("img");
-    result.src = active ? 'pin_red.png' : 'pin_grey.png';
-    result.style.transform = 'translate(1.5px,3px)';
-    return result;
-}
-
 function enableMarker(id, active) {
     var marker = markers[id];
-    marker.content = newIcon(active);
+    marker.content.src = active ? 'pin_red.png' : 'pin_grey.png';
     marker.zIndex = active ? 1 : 0;
 }
 
 function addMarker(id, lat, lng, active) {
+    var icon = document.createElement("img");
+    icon.src = 'pin_grey.png';
+    icon.style.transform = 'translate(1.5px,3px)';
     var marker = new google.maps.marker.AdvancedMarkerElement({
-        content: newIcon(false),
+        content: icon,
         position: new google.maps.LatLng(lat, lng),
         map: map,
         gmpDraggable: true,
     });
     markers[id] = marker;
     google.maps.event.addListener(marker, 'click', markerClick);
     google.maps.event.addListener(marker, 'dragstart', markerClick);
```

### Comparing `Photini-2024.4.0/src/photini/data/map/mapboxmap.js` & `Photini-2024.5.0/src/photini/data/map/mapboxmap.js`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/map/pin_grey.png` & `Photini-2024.5.0/src/photini/data/map/pin_grey.png`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/map/pin_red.png` & `Photini-2024.5.0/src/photini/data/map/pin_red.png`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/data/windows/install_shortcuts.vbs` & `Photini-2024.5.0/src/photini/data/windows/install_shortcuts.vbs`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/descriptive.py` & `Photini-2024.5.0/src/photini/descriptive.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/editor.py` & `Photini-2024.5.0/src/photini/editor.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/editsettings.py` & `Photini-2024.5.0/src/photini/editsettings.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/exiv2.py` & `Photini-2024.5.0/src/photini/exiv2.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/ffmpeg.py` & `Photini-2024.5.0/src/photini/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/flickr.py` & `Photini-2024.5.0/src/photini/flickr.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/googlemap.py` & `Photini-2024.5.0/src/photini/googlemap.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ##
 ##  You should have received a copy of the GNU General Public License
 ##  along with this program.  If not, see
 ##  <http://www.gnu.org/licenses/>.
 
 import locale
 import logging
+import re
 
 import requests
 
 from photini.configstore import key_store
 from photini.photinimap import GeocoderBase, PhotiniMap
 from photini.pyqt import Busy, Qt, QtCore, QtWidgets, scale_font
 from photini.widgets import Label
@@ -97,23 +98,35 @@
     def tab_name():
         return translate('MapTabGoogle', 'Map (&Google)')
 
     def get_geocoder(self):
         return GoogleGeocoder(parent=self)
 
     def get_head(self):
+        user_agent = self.widgets['map'].page().profile().httpUserAgent()
+        match = re.search(r'\sChrome/(\d+)\.', user_agent)
+        if match:
+            chrome_version = int(match.group(1))
+        else:
+            chrome_version = 0
         url = ('http://maps.googleapis.com/maps/api/js'
                '?callback=initialize'
-               '&loading=async'
-               '&libraries=marker')
+               '&loading=async')
+        # AdvancedMarkerElement requires Chrome v86+
+        if chrome_version >= 86:
+            url += '&libraries=marker'
+            script = 'googlemap.js'
+        else:
+            script = 'googlemap_legacy.js'
         if self.app.options.test:
             url += '&v=beta'
         url += '&key=' + self.api_key
         lang, encoding = locale.getlocale()
         if lang:
             language, sep, region = lang.replace('_', '-').partition('-')
             url += '&language=' + language
             if region:
                 url += '&region=' + region
         return '''    <script type="text/javascript"
       src="{}" async>
-    </script>'''.format(url)
+    </script>
+    <script type="text/javascript" src="{}"></script>'''.format(url, script)
```

### Comparing `Photini-2024.4.0/src/photini/googlephotos.py` & `Photini-2024.5.0/src/photini/googlephotos.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/gpximporter.py` & `Photini-2024.5.0/src/photini/gpximporter.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/imagelist.py` & `Photini-2024.5.0/src/photini/imagelist.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/importer.py` & `Photini-2024.5.0/src/photini/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##  Photini - a simple photo metadata editor.
 ##  http://github.com/jim-easterbrook/Photini
-##  Copyright (C) 2012-23  Jim Easterbrook  jim@jim-easterbrook.me.uk
+##  Copyright (C) 2012-24  Jim Easterbrook  jim@jim-easterbrook.me.uk
 ##
 ##  This program is free software: you can redistribute it and/or
 ##  modify it under the terms of the GNU General Public License as
 ##  published by the Free Software Foundation, either version 3 of the
 ##  License, or (at your option) any later version.
 ##
 ##  This program is distributed in the hope that it will be useful,
@@ -162,27 +162,38 @@
                 except gp.GPhoto2Error:
                     return None
                 timestamp = datetime.utcfromtimestamp(info.file.mtime)
                 file_data[name] = {
                     'camera'    : self.model,
                     'folder'    : folder,
                     'name'      : name,
+                    'size'      : info.file.size,
                     'timestamp' : timestamp,
                     }
         return file_data
 
     def copy_files(self, info_list, move):
         with self.session() as camera:
             for info in info_list:
                 dest_dir = os.path.dirname(info['dest_path'])
                 if not os.path.isdir(dest_dir):
                     os.makedirs(dest_dir)
-                camera_file = camera.file_get(
-                    info['folder'], info['name'], gp.GP_FILE_TYPE_NORMAL)
-                camera_file.save(info['dest_path'])
+                buf = bytearray(min(info['size'], 32 * 1024 * 1024))
+                try:
+                    with open(info['dest_path'], 'wb') as of:
+                        offset = 0
+                        while offset < info['size']:
+                            count = camera.file_read(
+                                info['folder'], info['name'],
+                                gp.GP_FILE_TYPE_NORMAL, offset, buf)
+                            of.write(buf[:count])
+                            offset += count
+                except Exception:
+                    os.unlink(info['dest_path'])
+                    raise
                 if move:
                     camera.file_delete(info['folder'], info['name'])
                 yield info
 
 
 class FileCopier(QtCore.QObject):
     def __init__(self, source, copy_list, move, copier_result, *args, **kwds):
```

### Comparing `Photini-2024.4.0/src/photini/ipernity.py` & `Photini-2024.5.0/src/photini/ipernity.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/loggerwindow.py` & `Photini-2024.5.0/src/photini/loggerwindow.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/mapboxmap.py` & `Photini-2024.5.0/src/photini/mapboxmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,9 +111,10 @@
 
     def get_head(self):
         return '''    <link rel="stylesheet" href="{url}/mapbox.css" />
     <script type="text/javascript" src="{url}/mapbox.js">
     </script>
     <script type="text/javascript">
       L.mapbox.accessToken = "{key}";
-    </script>'''.format(key=self.api_key,
-                        url='https://api.mapbox.com/mapbox.js/v3.3.1')
+    </script>
+    <script type="text/javascript" src="mapboxmap.js"></script>'''.format(
+        key=self.api_key, url='https://api.mapbox.com/mapbox.js/v3.3.1')
```

### Comparing `Photini-2024.4.0/src/photini/metadata.py` & `Photini-2024.5.0/src/photini/metadata.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/ownership.py` & `Photini-2024.5.0/src/photini/ownership.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/photinimap.py` & `Photini-2024.5.0/src/photini/photinimap.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,15 @@
         self.transient = transient
         if self.call_handler:
             self.web_channel = QWebChannel(parent=self)
             self.setWebChannel(self.web_channel)
             self.web_channel.registerObject('python', self.call_handler)
         self.profile().setCachePath(
             os.path.join(appdirs.user_cache_dir('photini'), 'WebEngine'))
+        logger.debug('user agent: %s', self.profile().httpUserAgent())
 
     @catch_all
     def acceptNavigationRequest(self, url, type_, isMainFrame):
         if type_ != self.NavigationType.NavigationTypeLinkClicked:
             return super(MapWebPage, self).acceptNavigationRequest(
                 url, type_, isMainFrame)
         if url.isLocalFile():
@@ -296,15 +297,14 @@
     <meta name="viewport" content="initial-scale=1.0, user-scalable=no" />
     <style type="text/css">
       html, body {{ height: 100%; margin: 0; padding: 0 }}
       #mapDiv {{ position: relative; width: 100%; height: 100% }}
     </style>
 {initialize}
 {head}
-    <script type="text/javascript" src="{script}.js"></script>
   </head>
   <body ondragstart="return false">
     <div id="mapDiv"></div>
   </body>
 </html>'''
         lat, lng = self.app.config_store.get('map', 'centre', (51.0, 0.0))
         zoom = int(self.app.config_store.get('map', 'zoom', 11))
@@ -321,15 +321,14 @@
       {{
           python = channel.objects.python;
           loadMap({lat}, {lng}, {zoom});
       }}
     </script>'''
         page = page.format(
             head = self.get_head(),
-            script = self.__module__.split('.')[-1],
             initialize = initialize.format(lat=lat, lng=lng, zoom=zoom))
         QtWidgets.QApplication.setOverrideCursor(Qt.CursorShape.WaitCursor)
         self.widgets['map'].setHtml(
             page, QtCore.QUrl.fromLocalFile(self.script_dir + '/'))
 
     @catch_all
     def initialize_finished(self):
```

### Comparing `Photini-2024.4.0/src/photini/pixelfed.py` & `Photini-2024.5.0/src/photini/pixelfed.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/pyqt.py` & `Photini-2024.5.0/src/photini/pyqt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##  Photini - a simple photo metadata editor.
 ##  http://github.com/jim-easterbrook/Photini
-##  Copyright (C) 2015-23  Jim Easterbrook  jim@jim-easterbrook.me.uk
+##  Copyright (C) 2015-24  Jim Easterbrook  jim@jim-easterbrook.me.uk
 ##
 ##  This program is free software: you can redistribute it and/or
 ##  modify it under the terms of the GNU General Public License as
 ##  published by the Free Software Foundation, either version 3 of the
 ##  License, or (at your option) any later version.
 ##
 ##  This program is distributed in the hope that it will be useful,
@@ -15,15 +15,14 @@
 ##  You should have received a copy of the GNU General Public License
 ##  along with this program.  If not, see
 ##  <http://www.gnu.org/licenses/>.
 
 from collections import namedtuple
 from contextlib import contextmanager
 from functools import wraps
-import importlib
 import logging
 import os
 import sys
 
 from photini.configstore import BaseConfigStore
 
 logger = logging.getLogger(__name__)
```

### Comparing `Photini-2024.4.0/src/photini/regions.py` & `Photini-2024.5.0/src/photini/regions.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/scripts.py` & `Photini-2024.5.0/src/photini/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 ##  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 ##  General Public License for more details.
 ##
 ##  You should have received a copy of the GNU General Public License
 ##  along with this program.  If not, see
 ##  <http://www.gnu.org/licenses/>.
 
-import importlib
 import logging
 from optparse import OptionParser
 import os
 import platform
 import site
 import subprocess
 import sys
```

### Comparing `Photini-2024.4.0/src/photini/spelling.py` & `Photini-2024.5.0/src/photini/spelling.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/technical.py` & `Photini-2024.5.0/src/photini/technical.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/types.py` & `Photini-2024.5.0/src/photini/types.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/uploader.py` & `Photini-2024.5.0/src/photini/uploader.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.4.0/src/photini/widgets.py` & `Photini-2024.5.0/src/photini/widgets.py`

 * *Files identical despite different names*

