# Comparing `tmp/vfbLib-0.6.4.tar.gz` & `tmp/vfblib-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vfbLib-0.6.4.tar", last modified: Fri Feb 16 11:28:28 2024, max compression
+gzip compressed data, was "vfblib-0.6.5.tar", last modified: Wed May  8 13:54:41 2024, max compression
```

## Comparing `vfbLib-0.6.4.tar` & `vfblib-0.6.5.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 11:28:28.968975 vfbLib-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-02-16 11:28:18.000000 vfbLib-0.6.4/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-02-16 11:28:18.000000 vfbLib-0.6.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 11:28:28.956975 vfbLib-0.6.4/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 11:28:28.960975 vfbLib-0.6.4/Lib/vfbLib/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/cmdline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 11:28:28.964975 vfbLib-0.6.4/Lib/vfbLib/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/compilers/glyph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/compilers/value.py
--rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/cu2qu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 11:28:28.964975 vfbLib-0.6.4/Lib/vfbLib/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/parsers/bitmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/parsers/cmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    16883 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/parsers/glyph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/parsers/guides.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/parsers/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/parsers/mm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/parsers/numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/parsers/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/parsers/ps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/parsers/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/parsers/truetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/parsers/value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 11:28:28.964975 vfbLib-0.6.4/Lib/vfbLib/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/templates/glyph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/truetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 11:28:28.968975 vfbLib-0.6.4/Lib/vfbLib/ufo/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31274 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/designspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/glyph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/guides.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/kerning.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/pshints.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/tth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/ufo/vfb2ufo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/value.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 11:28:28.968975 vfbLib-0.6.4/Lib/vfbLib/vfb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/vfb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/vfb/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/vfb/glyph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/vfb/header.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/vfb/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/vfb/pens.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-02-16 11:28:18.000000 vfbLib-0.6.4/Lib/vfbLib/vfb/vfb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 11:28:28.968975 vfbLib-0.6.4/Lib/vfbLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-02-16 11:28:28.000000 vfbLib-0.6.4/Lib/vfbLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-02-16 11:28:28.000000 vfbLib-0.6.4/Lib/vfbLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 11:28:28.000000 vfbLib-0.6.4/Lib/vfbLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-16 11:28:28.000000 vfbLib-0.6.4/Lib/vfbLib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 11:28:28.000000 vfbLib-0.6.4/Lib/vfbLib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-16 11:28:28.000000 vfbLib-0.6.4/Lib/vfbLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-16 11:28:28.000000 vfbLib-0.6.4/Lib/vfbLib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-02-16 11:28:28.968975 vfbLib-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-02-16 11:28:18.000000 vfbLib-0.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-16 11:28:19.000000 vfbLib-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-02-16 11:28:28.968975 vfbLib-0.6.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-02-16 11:28:19.000000 vfbLib-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:41.706300 vfblib-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-08 13:54:34.000000 vfblib-0.6.5/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-08 13:54:34.000000 vfblib-0.6.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:41.690300 vfblib-0.6.5/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:41.694300 vfblib-0.6.5/Lib/vfbLib/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/cmdline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:41.698300 vfblib-0.6.5/Lib/vfbLib/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/compilers/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/compilers/value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/cu2qu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:41.698300 vfblib-0.6.5/Lib/vfbLib/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/parsers/bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/parsers/cmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16883 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/parsers/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/parsers/guides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/parsers/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/parsers/mm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/parsers/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/parsers/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/parsers/ps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/parsers/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/parsers/truetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/parsers/value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:41.698300 vfblib-0.6.5/Lib/vfbLib/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/templates/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/truetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:41.702300 vfblib-0.6.5/Lib/vfbLib/ufo/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31285 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/designspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/guides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/kerning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/pshints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/tth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/ufo/vfb2ufo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/value.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:41.706300 vfblib-0.6.5/Lib/vfbLib/vfb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/vfb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/vfb/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/vfb/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/vfb/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/vfb/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/vfb/pens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-08 13:54:34.000000 vfblib-0.6.5/Lib/vfbLib/vfb/vfb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:41.706300 vfblib-0.6.5/Lib/vfbLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-08 13:54:41.000000 vfblib-0.6.5/Lib/vfbLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-08 13:54:41.000000 vfblib-0.6.5/Lib/vfbLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:54:41.000000 vfblib-0.6.5/Lib/vfbLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-08 13:54:41.000000 vfblib-0.6.5/Lib/vfbLib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:54:41.000000 vfblib-0.6.5/Lib/vfbLib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-08 13:54:41.000000 vfblib-0.6.5/Lib/vfbLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 13:54:41.000000 vfblib-0.6.5/Lib/vfbLib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-08 13:54:41.706300 vfblib-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-08 13:54:34.000000 vfblib-0.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 13:54:34.000000 vfblib-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-08 13:54:41.706300 vfblib-0.6.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-05-08 13:54:34.000000 vfblib-0.6.5/setup.py
```

### Comparing `vfbLib-0.6.4/DESCRIPTION.md` & `vfblib-0.6.5/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/LICENSE` & `vfblib-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/cmdline.py` & `vfblib-0.6.5/Lib/vfbLib/cmdline.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/compilers/__init__.py` & `vfblib-0.6.5/Lib/vfbLib/compilers/__init__.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/compilers/glyph.py` & `vfblib-0.6.5/Lib/vfbLib/compilers/glyph.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/compilers/value.py` & `vfblib-0.6.5/Lib/vfbLib/compilers/value.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/constants.py` & `vfblib-0.6.5/Lib/vfbLib/constants.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/cu2qu.py` & `vfblib-0.6.5/Lib/vfbLib/cu2qu.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/diff.py` & `vfblib-0.6.5/Lib/vfbLib/diff.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/parsers/base.py` & `vfblib-0.6.5/Lib/vfbLib/parsers/base.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/parsers/bitmap.py` & `vfblib-0.6.5/Lib/vfbLib/parsers/bitmap.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/parsers/cmap.py` & `vfblib-0.6.5/Lib/vfbLib/parsers/cmap.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/parsers/glyph.py` & `vfblib-0.6.5/Lib/vfbLib/parsers/glyph.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/parsers/guides.py` & `vfblib-0.6.5/Lib/vfbLib/parsers/guides.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/parsers/header.py` & `vfblib-0.6.5/Lib/vfbLib/parsers/header.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/parsers/mm.py` & `vfblib-0.6.5/Lib/vfbLib/parsers/mm.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/parsers/numeric.py` & `vfblib-0.6.5/Lib/vfbLib/parsers/numeric.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/parsers/options.py` & `vfblib-0.6.5/Lib/vfbLib/parsers/options.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/parsers/ps.py` & `vfblib-0.6.5/Lib/vfbLib/parsers/ps.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/parsers/text.py` & `vfblib-0.6.5/Lib/vfbLib/parsers/text.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/parsers/truetype.py` & `vfblib-0.6.5/Lib/vfbLib/parsers/truetype.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/parsers/value.py` & `vfblib-0.6.5/Lib/vfbLib/parsers/value.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/truetype.py` & `vfblib-0.6.5/Lib/vfbLib/truetype.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/typing.py` & `vfblib-0.6.5/Lib/vfbLib/typing.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/ufo/builder.py` & `vfblib-0.6.5/Lib/vfbLib/ufo/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
                     "Optical Size": "opsz",
                     "Serif": "SERF",
                 }
                 self.axes.append(
                     AxisDescriptor(tag=tags.get(data, data.upper()[:4]), name=data)
                 )
             elif name == "Axis Mappings Count":  # 1515
-                self.axis_mappings_count = data
+                self.axis_mappings_count: List[int] = data
             elif name == "Axis Mappings":  # 1516
                 self.add_axis_mappings(data)
             elif name == "Anisotropic Interpolation Mappings":  # 1523
                 # TODO: Can we properly output this to designspace?
                 for axis in data:
                     for a, b in axis:
                         if a != b:
```

### Comparing `vfbLib-0.6.4/Lib/vfbLib/ufo/designspace.py` & `vfblib-0.6.5/Lib/vfbLib/ufo/designspace.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/ufo/features.py` & `vfblib-0.6.5/Lib/vfbLib/ufo/features.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/ufo/glyph.py` & `vfblib-0.6.5/Lib/vfbLib/ufo/glyph.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/ufo/groups.py` & `vfblib-0.6.5/Lib/vfbLib/ufo/groups.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/ufo/guides.py` & `vfblib-0.6.5/Lib/vfbLib/ufo/guides.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/ufo/helpers.py` & `vfblib-0.6.5/Lib/vfbLib/ufo/helpers.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/ufo/info.py` & `vfblib-0.6.5/Lib/vfbLib/ufo/info.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/ufo/kerning.py` & `vfblib-0.6.5/Lib/vfbLib/ufo/kerning.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/ufo/paths.py` & `vfblib-0.6.5/Lib/vfbLib/ufo/paths.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/ufo/pshints.py` & `vfblib-0.6.5/Lib/vfbLib/ufo/pshints.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/ufo/time.py` & `vfblib-0.6.5/Lib/vfbLib/ufo/time.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/ufo/tth.py` & `vfblib-0.6.5/Lib/vfbLib/ufo/tth.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                     zd = "ttZonesT"
                 d["zone"] = self.zone_names[zd][params["zone"]]
             elif code in ("AlignH", "AlignV"):
                 d["point"] = self.glyph.get_point_label(params["pt"], code)
                 if "align" in params:
                     align = params["align"]
                     if align > -1:
-                        d["align"] = vfb2ufo_alignment_rev[align]
+                        d["align"] = vfb2ufo_alignment_rev.get(align, "round")
             elif code in (
                 "SingleLinkH",
                 "SingleLinkV",
                 "DoubleLinkH",
                 "DoubleLinkV",
             ):
                 d["point1"] = self.glyph.get_point_label(params["pt1"], code)
@@ -135,26 +135,26 @@
                             logger.warning(f"{code}: {params}")
                             logger.warning(self.stems[stem_dir])
                             stem = 0
                         d["stem"] = self.stems[stem_dir][stem]["name"]
                 if "align" in params:
                     align = params["align"]
                     if align > -1:
-                        d["align"] = vfb2ufo_alignment_rev[align]
+                        d["align"] = vfb2ufo_alignment_rev.get(align, "round")
             elif code in (
                 "InterpolateH",
                 "InterpolateV",
             ):
                 d["point"] = self.glyph.get_point_label(params["pti"], code)
                 d["point1"] = self.glyph.get_point_label(params["pt1"], code)
                 d["point2"] = self.glyph.get_point_label(params["pt2"], code)
                 if "align" in params:
                     align = params["align"]
                     if align > -1:
-                        d["align"] = vfb2ufo_alignment_rev[align]
+                        d["align"] = vfb2ufo_alignment_rev.get(align, "round")
             elif code in (
                 "MDeltaH",
                 "MDeltaV",
                 "FDeltaH",
                 "FDeltaV",
             ):
                 d["point"] = self.glyph.get_point_label(params["pt"], code)
```

### Comparing `vfbLib-0.6.4/Lib/vfbLib/ufo/typing.py` & `vfblib-0.6.5/Lib/vfbLib/ufo/typing.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/ufo/vfb2ufo.py` & `vfblib-0.6.5/Lib/vfbLib/ufo/vfb2ufo.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     "left": ALIGN_LEFT_BOTTOM,
     "top": ALIGN_RIGHT_TOP,  # Alias
     "right": ALIGN_RIGHT_TOP,
     "center": ALIGN_CENTER,
     "double": ALIGN_DOUBLE,
 }
 
+# There may be other values in the wild, which should be mapped to "round".
+# TODO: Use defaultdict?
 vfb2ufo_alignment_rev = {
     -1: "default",
     ALIGN_CLOSEST_PIXEL: "round",
     ALIGN_LEFT_BOTTOM: "left",
     ALIGN_RIGHT_TOP: "right",
     ALIGN_CENTER: "center",
     ALIGN_DOUBLE: "double",
```

### Comparing `vfbLib-0.6.4/Lib/vfbLib/value.py` & `vfblib-0.6.5/Lib/vfbLib/value.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/vfb/entry.py` & `vfblib-0.6.5/Lib/vfbLib/vfb/entry.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/vfb/glyph.py` & `vfblib-0.6.5/Lib/vfbLib/vfb/glyph.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/vfb/header.py` & `vfblib-0.6.5/Lib/vfbLib/vfb/header.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/vfb/info.py` & `vfblib-0.6.5/Lib/vfbLib/vfb/info.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/vfb/pens.py` & `vfblib-0.6.5/Lib/vfbLib/vfb/pens.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib/vfb/vfb.py` & `vfblib-0.6.5/Lib/vfbLib/vfb/vfb.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/Lib/vfbLib.egg-info/PKG-INFO` & `vfblib-0.6.5/Lib/vfbLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfbLib
-Version: 0.6.4
+Version: 0.6.5
 Summary: Tools for converting FontLab Studio 5 (VFB) files.
 Home-page: https://pypi.org/project/vfblib/
 Author: Jens Kutilek
 License: GPLv3
 Project-URL: Source, https://github.com/LucasFonts/vfbLib
 Project-URL: Tracker, https://github.com/LucasFonts/vfbLib/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vfbLib-0.6.4/Lib/vfbLib.egg-info/SOURCES.txt` & `vfblib-0.6.5/Lib/vfbLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/PKG-INFO` & `vfblib-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfbLib
-Version: 0.6.4
+Version: 0.6.5
 Summary: Tools for converting FontLab Studio 5 (VFB) files.
 Home-page: https://pypi.org/project/vfblib/
 Author: Jens Kutilek
 License: GPLv3
 Project-URL: Source, https://github.com/LucasFonts/vfbLib
 Project-URL: Tracker, https://github.com/LucasFonts/vfbLib/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vfbLib-0.6.4/README.md` & `vfblib-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `vfbLib-0.6.4/setup.cfg` & `vfblib-0.6.5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vfbLib
-version = 0.6.4
+version = 0.6.5
 description = Tools for converting FontLab Studio 5 (VFB) files.
 long_description = file: DESCRIPTION.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://pypi.org/project/vfblib/
 author = Jens Kutilek
 license = GPLv3
 license_files = LICENSE
@@ -35,20 +35,19 @@
 where = Lib
 
 [bdist_wheel]
 universal = 1
 
 [options.entry_points]
 console_scripts = 
-	diffvfb = vfbLib.diff:diffvfb
+	normalize_vfb2ufo = vfbLib.ufo.helpers:normalize
 	vfb2json = vfbLib.cmdline:vfb2json
 	vfb3ufo = vfbLib.cmdline:vfb2ufo
 	vfbcu2qu = vfbLib.cu2qu:vfbcu2qu
-	normalize_vfb2ufo = vfbLib.ufo.helpers:normalize
-	yuri = vfbLib.value:yuri
+	vfbdiff = vfbLib.diff:diffvfb
 
 [flake8]
 select = B, C, E, F, W, T4, B9
 ignore = W503
 max-line-length = 88
 max-complexity = 19
 exclude = .git, __pycache__, build, dist, .eggs, .tox
```

