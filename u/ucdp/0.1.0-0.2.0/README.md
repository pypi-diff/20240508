# Comparing `tmp/ucdp-0.1.0.tar.gz` & `tmp/ucdp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucdp-0.1.0.tar", max compression
+gzip compressed data, was "ucdp-0.2.0.tar", last modified: Wed May  8 15:34:46 2024, max compression
```

## Comparing `ucdp-0.1.0.tar` & `ucdp-0.2.0.tar`

### file list

```diff
@@ -1,47 +1,95 @@
--rw-r--r--   0        0        0     1067 2023-07-15 01:51:59.914904 ucdp-0.1.0/LICENSE
--rw-r--r--   0        0        0     1142 2023-07-15 01:51:59.914904 ucdp-0.1.0/README.md
--rw-r--r--   0        0        0     2386 2023-07-15 01:51:59.914904 ucdp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3429 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/__init__.py
--rw-r--r--   0        0        0    17934 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/assigns.py
--rw-r--r--   0        0        0     2992 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/attrs.py
--rw-r--r--   0        0        0     4672 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/const.py
--rw-r--r--   0        0        0     5103 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/doc.py
--rw-r--r--   0        0        0     1109 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/examples/simple/glbl/__init__.py
--rw-r--r--   0        0        0     2556 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/examples/simple/glbl/bus.py
--rw-r--r--   0        0        0     1447 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/examples/simple/glbl/clkgate.py
--rw-r--r--   0        0        0     2840 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/examples/simple/glbl/regf.py
--rw-r--r--   0        0        0     1225 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/examples/simple/glbl/regf_tb.py
--rw-r--r--   0        0        0     1109 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/examples/simple/uart/__init__.py
--rw-r--r--   0        0        0     3121 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/examples/simple/uart/uart.py
--rw-r--r--   0        0        0    25569 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/expr.py
--rw-r--r--   0        0        0     2416 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/flipflop.py
--rw-r--r--   0        0        0    15294 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/ident.py
--rw-r--r--   0        0        0     2907 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/loader.py
--rw-r--r--   0        0        0     1127 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/mod/__init__.py
--rw-r--r--   0        0        0    27593 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/mod/base.py
--rw-r--r--   0        0        0     7078 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/mod/config.py
--rw-r--r--   0        0        0    16655 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/mod/iter.py
--rw-r--r--   0        0        0    21248 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/mod/mods.py
--rw-r--r--   0        0        0     3333 2023-07-15 01:51:59.918904 ucdp-0.1.0/ucdp/mod/util.py
--rw-r--r--   0        0        0     3076 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/modref.py
--rw-r--r--   0        0        0     4519 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/mux.py
--rw-r--r--   0        0        0     4425 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/namespace.py
--rw-r--r--   0        0        0     5949 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/nameutil.py
--rw-r--r--   0        0        0     4758 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/param.py
--rw-r--r--   0        0        0    13437 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/router.py
--rw-r--r--   0        0        0     7582 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/signal.py
--rw-r--r--   0        0        0     1305 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/test.py
--rw-r--r--   0        0        0     4117 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/top.py
--rw-r--r--   0        0        0     3377 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/topref.py
--rw-r--r--   0        0        0     1131 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/types/__init__.py
--rw-r--r--   0        0        0     3470 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/types/array.py
--rw-r--r--   0        0        0     5754 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/types/base.py
--rw-r--r--   0        0        0     5117 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/types/clkrst.py
--rw-r--r--   0        0        0     8088 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/types/descriptivestruct.py
--rw-r--r--   0        0        0    18847 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/types/enum.py
--rw-r--r--   0        0        0     2988 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/types/iter.py
--rw-r--r--   0        0        0     6206 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/types/orientation.py
--rw-r--r--   0        0        0    23744 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/types/scalar.py
--rw-r--r--   0        0        0    10412 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/types/struct.py
--rw-r--r--   0        0        0     4759 2023-07-15 01:51:59.922904 ucdp-0.1.0/ucdp/util.py
--rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 ucdp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-08 15:34:32.481678 ucdp-0.2.0/LICENSE
+-rw-r--r--   0        0        0      939 2024-05-08 15:34:32.481678 ucdp-0.2.0/README.md
+-rw-r--r--   0        0        0     2635 2024-05-08 15:34:46.397773 ucdp-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6939 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/__init__.py
+-rw-r--r--   0        0        0     2972 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/_modbuilder.py
+-rw-r--r--   0        0        0    12128 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/assigns.py
+-rw-r--r--   0        0        0     1959 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/baseclassinfo.py
+-rw-r--r--   0        0        0      360 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/buildproduct.py
+-rw-r--r--   0        0        0     5545 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/cli.py
+-rw-r--r--   0        0        0     5680 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/config.py
+-rw-r--r--   0        0        0     3332 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/const.py
+-rw-r--r--   0        0        0     1350 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/consts.py
+-rw-r--r--   0        0        0     2683 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/dict.py
+-rw-r--r--   0        0        0     3492 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/doc.py
+-rw-r--r--   0        0        0     2372 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/docutil.py
+-rw-r--r--   0        0        0     1144 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/bad/glbl_bad/__init__.py
+-rw-r--r--   0        0        0     1371 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/bad/glbl_bad/regf.py
+-rw-r--r--   0        0        0     1443 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/filelist/filelist_lib/filelist.py
+-rw-r--r--   0        0        0       67 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/filelist/filelist_lib/mod.f
+-rw-r--r--   0        0        0     1758 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/fileliststandard.py
+-rw-r--r--   0        0        0     1140 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/glbl/__init__.py
+-rw-r--r--   0        0        0     2696 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/glbl/bus.py
+-rw-r--r--   0        0        0     1565 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/glbl/clk_gate.py
+-rw-r--r--   0        0        0     3405 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/glbl/regf.py
+-rw-r--r--   0        0        0     1388 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/glbl/regf_tb.py
+-rw-r--r--   0        0        0     1129 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/uart/__init__.py
+-rw-r--r--   0        0        0     2607 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/uart/uart.py
+-rw-r--r--   0        0        0     1587 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/exceptions.py
+-rw-r--r--   0        0        0    16035 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/expr.py
+-rw-r--r--   0        0        0    13341 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/exprparser.py
+-rw-r--r--   0        0        0     5040 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/exprresolver.py
+-rw-r--r--   0        0        0     3603 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/filelistparser.py
+-rw-r--r--   0        0        0     2908 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/fileset.py
+-rw-r--r--   0        0        0     1762 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/flipflop.py
+-rw-r--r--   0        0        0     2817 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/generate.py
+-rw-r--r--   0        0        0     1884 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/humannum.py
+-rw-r--r--   0        0        0    12472 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/ident.py
+-rw-r--r--   0        0        0     3472 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/iterutil.py
+-rw-r--r--   0        0        0     2908 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/loader.py
+-rw-r--r--   0        0        0     1179 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/logging.py
+-rw-r--r--   0        0        0     2221 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/mod.py
+-rw-r--r--   0        0        0    32207 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modbase.py
+-rw-r--r--   0        0        0     2232 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modbasetop.py
+-rw-r--r--   0        0        0     3761 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modconfigurable.py
+-rw-r--r--   0        0        0     2772 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modcore.py
+-rw-r--r--   0        0        0     7539 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modfilelist.py
+-rw-r--r--   0        0        0    11630 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/moditer.py
+-rw-r--r--   0        0        0     3190 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modref.py
+-rw-r--r--   0        0        0     5551 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modtailored.py
+-rw-r--r--   0        0        0     5808 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modtb.py
+-rw-r--r--   0        0        0     3388 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modtopref.py
+-rw-r--r--   0        0        0     1686 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modutil.py
+-rw-r--r--   0        0        0     4047 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/mux.py
+-rw-r--r--   0        0        0     6419 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/namespace.py
+-rw-r--r--   0        0        0     4942 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/nameutil.py
+-rw-r--r--   0        0        0      514 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/note.py
+-rw-r--r--   0        0        0     4690 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/object.py
+-rw-r--r--   0        0        0     5440 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/orientation.py
+-rw-r--r--   0        0        0     3970 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/param.py
+-rw-r--r--   0        0        0     3898 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/pathutil.py
+-rw-r--r--   0        0        0     5735 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/routepath.py
+-rw-r--r--   0        0        0     7439 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/signal.py
+-rw-r--r--   0        0        0     8021 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/slices.py
+-rw-r--r--   0        0        0     1258 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/test.py
+-rw-r--r--   0        0        0     3167 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/top.py
+-rw-r--r--   0        0        0     3644 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typearray.py
+-rw-r--r--   0        0        0     4922 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typebase.py
+-rw-r--r--   0        0        0     5457 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typeclkrst.py
+-rw-r--r--   0        0        0     7908 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typedescriptivestruct.py
+-rw-r--r--   0        0        0    20080 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typeenum.py
+-rw-r--r--   0        0        0    22840 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typescalar.py
+-rw-r--r--   0        0        0     2043 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typestring.py
+-rw-r--r--   0        0        0    12024 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typestruct.py
+-rw-r--r--   0        0        0     1476 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/util.py
+-rw-r--r--   0        0        0       13 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0    16826 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_assigns.py
+-rw-r--r--   0        0        0     2876 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_baseclassinfo.py
+-rw-r--r--   0        0        0     1611 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_buildproduct.py
+-rw-r--r--   0        0        0     1914 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_config.py
+-rw-r--r--   0        0        0     2793 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_examples.py
+-rw-r--r--   0        0        0     1637 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_exprparser.py
+-rw-r--r--   0        0        0     1877 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_fileset.py
+-rw-r--r--   0        0        0     2077 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_flipflop.py
+-rw-r--r--   0        0        0     4756 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_light_object.py
+-rw-r--r--   0        0        0     6054 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_loader.py
+-rw-r--r--   0        0        0     2842 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_modfilelist.py
+-rw-r--r--   0        0        0     1587 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_mux.py
+-rw-r--r--   0        0        0    13658 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_namespace.py
+-rw-r--r--   0        0        0     4665 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_object.py
+-rw-r--r--   0        0        0     8485 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_pathutil.py
+-rw-r--r--   0        0        0     3489 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_typeenum.py
+-rw-r--r--   0        0        0     5436 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_typescalar.py
+-rw-r--r--   0        0        0     4047 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_typestruct.py
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 ucdp-0.2.0/PKG-INFO
```

### Comparing `ucdp-0.1.0/LICENSE` & `ucdp-0.2.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 nbiotcloud
+Copyright (c) 2024 nbiotcloud
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ucdp-0.1.0/README.md` & `ucdp-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,36 @@
+Metadata-Version: 2.1
+Name: ucdp
+Version: 0.2.0
+Summary: Unified Chip Design Platform
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Project-URL: Homepage, https://github.com/nbiotcloud/ucdp
+Project-URL: Documentation, https://ucdp.readthedocs.io/en/latest/
+Project-URL: Bug tracker, https://github.com/nbiotcloud/ucdp/issues
+Requires-Python: <4.0,>=3.10.0
+Requires-Dist: anytree>=2.12.1
+Requires-Dist: case-converter>=1.1.0
+Requires-Dist: click>=8.1.7
+Requires-Dist: fuzzywuzzy>=0.18.0
+Requires-Dist: humannum>=1.0.0
+Requires-Dist: icdutil>=0.3.1
+Requires-Dist: makolator>=2.4.0
+Requires-Dist: matchor>=0.1.0
+Requires-Dist: pydantic>=2.7.0
+Requires-Dist: python-Levenshtein>=0.25.1
+Requires-Dist: rich>=13.7.1
+Requires-Dist: uniquer>=1.0.2
+Description-Content-Type: text/markdown
+
 [![PyPI Version](https://badge.fury.io/py/ucdp.svg)](https://badge.fury.io/py/ucdp)
 [![Python Build](https://github.com/nbiotcloud/ucdp/actions/workflows/main.yml/badge.svg)](https://github.com/nbiotcloud/ucdp/actions/workflows/main.yml)
 [![Documentation](https://readthedocs.org/projects/ucdp/badge/?version=latest)](https://ucdp.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/nbiotcloud/ucdp/badge.svg?branch=main)](https://coveralls.io/github/nbiotcloud/ucdp?branch=main)
 [![python-versions](https://img.shields.io/pypi/pyversions/ucdp.svg)](https://pypi.python.org/pypi/ucdp)
-[![pylint](https://img.shields.io/badge/linter-pylint-%231674b1?style=flat)](https://www.pylint.org/)
-[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # Unified Chip Design Platform
 
 * [Documentation](https://ucdp.readthedocs.io/en/latest/)
 * [PyPI](https://pypi.org/project/ucdp/)
 * [Sources](https://github.com/nbiotcloud/ucdp)
 * [Issues](https://github.com/nbiotcloud/ucdp/issues)
```

### Comparing `ucdp-0.1.0/ucdp/examples/simple/glbl/__init__.py` & `ucdp-0.2.0/src/ucdp/examples/simple/uart/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,7 +17,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
+"""UART Example."""
```

### Comparing `ucdp-0.1.0/ucdp/examples/simple/glbl/bus.py` & `ucdp-0.2.0/src/ucdp/examples/simple/glbl/bus.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,65 +18,70 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """Bus Infrastructure."""
-import ucdp
 
-# Type Aliases
+import ucdp as u
 
 
-class AddrType(ucdp.UintType):
+class AddrType(u.UintType):
+    """Address Type."""
+
     def __init__(self):
-        super().__init__(32)
+        super().__init__(width=32)
 
 
-class DataType(ucdp.UintType):
-    def __init__(self, width=32, default=0):
-        super().__init__(width, default=default)
+class DataType(u.UintType):
+    """Data Type."""
 
+    def __init__(self, width=32, default=0):
+        super().__init__(width=width, default=default)
 
-# Enumerations with a detailed encoding
 
+class TransType(u.AEnumType):
+    """Transport Type."""
 
-class TransType(ucdp.AEnumType):
-    keytype = ucdp.UintType(2)
+    keytype: u.AScalarType = u.UintType(width=2)
 
-    def _build(self):
+    def _build(self) -> None:
         self._add(0, "idle", "No transfer.")
         self._add(1, "busy", "Idle cycle within transfer.")
         self._add(2, "nonseq", "Single transfer or first transfer of a burst.")
         self._add(3, "seq", "Consecutive transfers of a burst.")
 
 
-class WriteType(ucdp.AEnumType):
-    keytype = ucdp.BitType()
+class WriteType(u.AEnumType):
+    """Write Type."""
 
-    def _build(self):
+    keytype: u.AScalarType = u.BitType()
+
+    def _build(self) -> None:
         self._add(0, "read", "Read operation.")
         self._add(1, "write", "Write operation.")
 
 
-class RespType(ucdp.AEnumType):
-    keytype = ucdp.BitType()
+class RespType(u.AEnumType):
+    """Response Type."""
+
+    keytype: u.AScalarType = u.BitType()
 
-    def _build(self):
+    def _build(self) -> None:
         self._add(0, "okay", "OK.")
         self._add(1, "error", "Error.")
 
 
-# The BUS
-
+class BusType(u.AStructType):
+    """The Bus Type."""
 
-class BusType(ucdp.AStructType):
-    def _build(self):
+    def _build(self) -> None:
         # FWD
         self._add("trans", TransType())
         self._add("addr", AddrType())
         self._add("write", WriteType())
         self._add("wdata", DataType())
         # BWD
-        self._add("ready", ucdp.BitType(default=1), ucdp.BWD, descr="Transfer is finished on HIGH.")
-        self._add("resp", RespType(), ucdp.BWD)
-        self._add("rdata", DataType(), ucdp.BWD)
+        self._add("ready", u.BitType(default=1), u.BWD, descr="Transfer is finished on HIGH.")
+        self._add("resp", RespType(), u.BWD)
+        self._add("rdata", DataType(), u.BWD)
```

### Comparing `ucdp-0.1.0/ucdp/examples/simple/glbl/clkgate.py` & `ucdp-0.2.0/src/ucdp/examples/simple/glbl/clk_gate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,22 +18,27 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """Clock Gate."""
-import ucdp
 
+from typing import ClassVar
+
+import ucdp as u  # (1)
+from fileliststandard import HdlFileList
 
-class ClkGateMod(ucdp.AMod):
-    """Clock Gate."""
 
-    # Year for File Header Copyright
-    copyright_end_year = 2022
+class ClkGateMod(u.AMod):
+    """Clock Gate."""
 
-    comment = __doc__
+    # File Lists
+    filelists: ClassVar[u.ModFileLists] = (  # (2)
+        HdlFileList(),
+    )
 
-    def _build(self):
-        self.add_port(ucdp.ClkType(), "clk_i")
-        self.add_port(ucdp.ClkType(), "clk_o")
-        self.add_port(ucdp.EnaType(), "ena_i")
+    def _build(self) -> None:
+        # Port Declarations (3)
+        self.add_port(u.ClkType(), "clk_i")
+        self.add_port(u.ClkType(), "clk_o")
+        self.add_port(u.EnaType(), "ena_i")
```

### Comparing `ucdp-0.1.0/ucdp/examples/simple/glbl/regf_tb.py` & `ucdp-0.2.0/src/ucdp/examples/simple/glbl/regf_tb.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,16 +17,22 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-import ucdp
 
+"""A Simplified Register File Testbench."""
 
-class RegfTbMod(ucdp.ATbMod):
+from typing import ClassVar
 
+import ucdp as u
+
+
+class RegfTbMod(u.ATbMod):
     """Register File Testbench."""
 
+    filelists: ClassVar[u.ModFileLists] = (u.ModFileList(name="hdl", gen="inplace"),)
+
     def _build(self):
         pass
```

### Comparing `ucdp-0.1.0/ucdp/examples/simple/uart/__init__.py` & `ucdp-0.2.0/src/ucdp/examples/bad/glbl_bad/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,7 +17,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
+"""Example: Global Bad Library."""
```

### Comparing `ucdp-0.1.0/ucdp/examples/simple/uart/uart.py` & `ucdp-0.2.0/src/ucdp/examples/simple/uart/uart.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,72 +18,56 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """UART Example."""
-from glbl.bus import BusType
-from glbl.clkgate import ClkGateMod
-from glbl.regf import RegfMod
 
-import ucdp
+from typing import ClassVar
 
+import ucdp as u  # (1)
+from fileliststandard import HdlFileList
+from glbl.bus import BusType  # (2)
+from glbl.clk_gate import ClkGateMod  # (3)
+from glbl.regf import RegfMod  # (4)
 
-class UartIoType(ucdp.AStructType):
-    title = "UART"
-    comment = "RX/TX"
 
-    def _build(self):
-        self._add("rx", ucdp.BitType(), ucdp.BWD)
-        self._add("tx", ucdp.BitType(), ucdp.BWD)
+class UartIoType(u.AStructType):
+    """UART IO."""
 
+    title: str = "UART"
+    comment: str = "RX/TX"
 
-class UartMod(ucdp.AMod):
-    """A Simple UART."""
+    def _build(self) -> None:
+        self._add("rx", u.BitType(), u.BWD)  # (5)
+        self._add("tx", u.BitType(), u.FWD)  # (6)
 
-    # Year for File Header Copyright
-    copyright_end_year = 2022
 
-    comment = """\
-My Description
+class UartMod(u.AMod):
+    """A Simple UART."""
 
-Mode  Power       Description
-----  ----------  ------------------
-"""
+    filelists: ClassVar[u.ModFileLists] = (HdlFileList(gen="full"),)
 
-    def _build(self):
-        self.add_port(ucdp.ClkRstAnType())
+    def _build(self) -> None:
+        self.add_port(u.ClkRstAnType(), "main_i")
         self.add_port(UartIoType(), "uart_i", route="create(u_core/uart_i)")
         self.add_port(BusType(), "bus_i")
 
-        divmax_p = self.add_param(ucdp.IntegerType(default=2**16 - 1), "divmax_p")
-
-        clkgate = ClkGateMod(self, "u_clkgate")
+        clkgate = ClkGateMod(self, "u_clk_gate")
         clkgate.con("clk_i", "clk_i")
         clkgate.con("clk_o", "create(clk_s)")
 
         regf = RegfMod(self, "u_regf")
-        regf.con("", "")
+        regf.con("main_i", "main_i")
         regf.con("bus_i", "bus_i")
 
-        core = ucdp.CoreMod(self, "u_core", paramdict={"divmax_p": divmax_p})
-        core.add_param(ucdp.IntegerType(default=2**16 - 1), "divmax_p")
-
-        core.add_const(ucdp.IntegerType(default=ucdp.log2(divmax_p - 1)), "divwid_p")
-        core.add_port(ucdp.ClkRstAnType(), "")
-        core.con("clk_i", "clk_s")
-        core.con("rst_an_i", "rst_an_i")
-
-        core.add_port(ucdp.UintType(2), "sel_i")
-        core.add_port(ucdp.UintType(8), "y_o")
-        core.add_port(ucdp.UintType(6), "d_o")
-        core.add_port(ucdp.UintType(9), "a_i")
-
-        core.add_flipflop(ucdp.UintType(6), "d_r", nxt="a_i[7:2]", route="d_o")
+        core = u.CoreMod(parent=self, name="u_core")
 
-        coremux = core.add_mux("mymux")
-        coremux.set("sel_i", "2d1", "y_o", "a_i[7:0]")
+        core.add_port(u.ClkRstAnType(), "main_i")
+        core.con("main_clk_i", "clk_s")
+        core.con("main_rst_an_i", "rst_an_i")
+        core.con("create(regf_i)", "u_regf/regf_o")
 
         word = regf.add_word("ctrl")
-        word.add_field("ena", ucdp.EnaType(), is_readable=True, route="u_clkgate/ena_i")
-        word.add_field("strt", ucdp.BitType(), is_writable=True, route="create(u_core/strt_i)")
+        word.add_field("ena", u.EnaType(), is_readable=True, route="u_clk_gate/ena_i")
+        word.add_field("strt", u.BitType(), is_writable=True, route="create(u_core/strt_i)")
```

### Comparing `ucdp-0.1.0/ucdp/flipflop.py` & `ucdp-0.2.0/src/ucdp/flipflop.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,52 +19,30 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 """Flip Flop."""
-from typing import Optional
 
 from .assigns import Assigns
-from .attrs import define, field
 from .expr import BoolOp
-from .ident import Idents
-from .signal import ASignal
+from .object import model_validator
+from .signal import BaseSignal
+from .typeclkrst import ClkType, RstAnType
 
 
-@define
 class FlipFlop(Assigns):
-
     """FlipFlop."""
 
-    # pylint: disable=too-many-instance-attributes
-
-    clk: ASignal = field()
-    rst_an: ASignal = field()
-    rst: Optional[BoolOp] = field(default=None)
-    ena: Optional[BoolOp] = field(default=None)
-    targets: Idents = field(factory=Idents, repr=False)
-    sources: Idents = field(factory=Idents, repr=False)
-    drivers: dict = field(factory=dict, repr=False)
-
-    @staticmethod
-    def create(
-        mod, flipflops: dict, clk: ASignal, rst_an: ASignal, rst: Optional[BoolOp], ena: Optional[BoolOp]
-    ) -> "FlipFlop":
-        """Create FlipFlop Or Use Exisiting One."""
-        # pylint: disable=too-many-arguments
-        key = clk, rst_an, rst, ena
-        try:
-            flipflop = flipflops[key]
-        except KeyError:
-            flipflop = FlipFlop(
-                clk,
-                rst_an,
-                rst=rst,
-                ena=ena,
-                targets=mod.portssignals,
-                sources=mod.namespace,
-                drivers=mod.drivers,
-            )
-            flipflops[key] = flipflop
-        return flipflop
+    clk: BaseSignal
+    rst_an: BaseSignal
+    rst: BoolOp | None = None
+    ena: BoolOp | None = None
+
+    @model_validator(mode="after")
+    def __post_init(self) -> "FlipFlop":
+        if not isinstance(self.clk.type_, ClkType):
+            raise ValueError("clk is not of ClkType")
+        if not isinstance(self.rst_an.type_, RstAnType):
+            raise ValueError("rst_an is not of RstAnType")
+        return self
```

### Comparing `ucdp-0.1.0/ucdp/ident.py` & `ucdp-0.2.0/src/ucdp/ident.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,430 +21,356 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 """
 Identifier.
 
-All symbols within a hardware module are identifier and derived from :any:`Ident`.
-Identifier should be stored in :any:`Idents`.
-Identifier are itself part of an expression and therefore a child of :any:`Expr`.
-
-Example:
-
->>> import ucdp
->>> class ModeType(ucdp.AEnumType):
-...     keytype = ucdp.UintType(2)
-...     def _build(self):
-...         self._add(0, "add")
-...         self._add(1, "sub")
-...         self._add(2, "max")
->>> class MyType(ucdp.AStructType):
-...     def _build(self):
-...         self._add("mode", ModeType())
-...         self._add("send", ucdp.ArrayType(ucdp.UintType(8), 3))
-...         self._add("return", ucdp.UintType(4), ucdp.BWD)
->>> idents = ucdp.Idents([
-...     ucdp.Port(ucdp.UintType(8), "vec_a_i"),
-...     ucdp.Port(ucdp.UintType(8), "vec_a_o"),
-...     ucdp.Signal(ucdp.UintType(4), "vec_c_s"),
-...     ucdp.Signal(MyType(), "my_a_s"),
-...     ucdp.Signal(MyType(), "my_b_s"),
-... ])
-
-Retrieve an item:
-
->>> idents['vec_a_i']
-Port(UintType(8), name='vec_a_i')
->>> idents['my_a_mode_s']
-Signal(ModeType(), 'my_a_mode_s', level=1)
-
-Simple iteration:
-
->>> for ident in idents:
-...     ident
-Port(UintType(8), name='vec_a_i')
-Port(UintType(8), name='vec_a_o')
-Signal(UintType(4), 'vec_c_s')
-Signal(MyType(), 'my_a_s')
-Signal(MyType(), 'my_b_s')
-
-Unrolling iteration:
-
->>> for ident in idents.iter():
-...     ident
-Port(UintType(8), name='vec_a_i')
-Port(UintType(8), name='vec_a_o')
-Signal(UintType(4), 'vec_c_s')
-Signal(MyType(), 'my_a_s')
-Signal(ModeType(), 'my_a_mode_s', level=1)
-Signal(UintType(8), 'my_a_send_s', level=1, dims=(Slice('0:2'),))
-Signal(UintType(4), 'my_a_return_s', level=1, direction=BWD)
-Signal(MyType(), 'my_b_s')
-Signal(ModeType(), 'my_b_mode_s', level=1)
-Signal(UintType(8), 'my_b_send_s', level=1, dims=(Slice('0:2'),))
-Signal(UintType(4), 'my_b_return_s', level=1, direction=BWD)
-
-Some features:
-
->>> idents['my_b_send_s']
-Signal(UintType(8), 'my_b_send_s', level=1, dims=(Slice('0:2'),))
->>> 'my_b_send_s' in idents
-True
->>> 'my_b_send' in idents
-False
+All symbols within a hardware module are identifier and derived from [Ident][ucdp.ident.Ident].
+Identifier should be stored in [Idents][ucdp.ident.Idents].
+Identifier are itself part of an expression and therefore a child of [Expr][ucdp.expr.Expr].
+
+??? Example "Identifier Examples"
+    Basics:
+
+        >>> import ucdp as u
+        >>> class ModeType(u.AEnumType):
+        ...     keytype: u.AScalarType = u.UintType(2)
+        ...     def _build(self) -> None:
+        ...         self._add(0, "add")
+        ...         self._add(1, "sub")
+        ...         self._add(2, "max")
+        >>> class MyType(u.AStructType):
+        ...     def _build(self) -> None:
+        ...         self._add("mode", ModeType())
+        ...         self._add("send", u.ArrayType(u.UintType(8), 3))
+        ...         self._add("return", u.UintType(4), u.BWD)
+        >>> idents = u.Idents([
+        ...     u.Ident(u.UintType(8), "vec_a_i"),
+        ...     u.Ident(u.UintType(8), "vec_a_o"),
+        ...     u.Ident(u.UintType(4), "vec_c_s"),
+        ...     u.Ident(MyType(), "my_a_s"),
+        ...     u.Ident(u.ArrayType(MyType(), 4), "my_b_s"),
+        ... ])
+
+??? Example "Retrieve An Item"
+    Retrieve an item:
+
+        >>> idents['vec_a_i']
+        Ident(UintType(8), 'vec_a_i')
+        >>> idents['my_a_mode_s']
+        Ident(ModeType(), 'my_a_mode_s')
+
+??? Example "Simple Iteration"
+    Simple iteration:
+
+        >>> for ident in idents:
+        ...     ident
+        Ident(UintType(8), 'vec_a_i')
+        Ident(UintType(8), 'vec_a_o')
+        Ident(UintType(4), 'vec_c_s')
+        Ident(MyType(), 'my_a_s')
+        Ident(ArrayType(MyType(), 4), 'my_b_s')
+
+??? Example "Unrolling Iteration"
+    Unrolling iteration:
+
+        >>> for ident in idents.iter():
+        ...     ident
+        Ident(UintType(8), 'vec_a_i')
+        Ident(UintType(8), 'vec_a_o')
+        Ident(UintType(4), 'vec_c_s')
+        Ident(MyType(), 'my_a_s')
+        Ident(ModeType(), 'my_a_mode_s')
+        Ident(ArrayType(UintType(8), 3), 'my_a_send_s')
+        Ident(UintType(4), 'my_a_return_s')
+        Ident(ArrayType(MyType(), 4), 'my_b_s')
+        Ident(ArrayType(UintType(4), 4), 'my_b_return_s')
+        Ident(ArrayType(ArrayType(UintType(8), 3), 4), 'my_b_send_s')
+        Ident(ArrayType(ModeType(), 4), 'my_b_mode_s')
+
+??? Example "Some Features"
+    Some features:
+
+        >>> idents['my_b_send_s']
+        Ident(ArrayType(ArrayType(UintType(8), 3), 4), 'my_b_send_s')
+        >>> 'my_b_send_s' in idents
+        True
+        >>> 'my_b_send' in idents
+        False
+
 """
 
 from collections import deque
-from inspect import isclass
-from typing import Iterator, List, Optional, Tuple
-
-from aligntext import align
-from icdutil.slices import Slice
+from collections.abc import Callable, Iterable, Iterator
+from typing import Any
 
-from .attrs import evolve, field, frozen
+from .consts import PAT_IDENTIFIER
 from .doc import Doc
-from .expr import Expr
+from .expr import ConcatExpr, ConstExpr, Expr, Log2Expr, MaximumExpr, MinimumExpr, Op, SliceOp, SOp, TernaryExpr
 from .namespace import Namespace
-from .nameutil import didyoumean, split_suffix, validate_identifier
-from .types.array import ArrayType
-from .types.base import AType
-from .types.orientation import AOrientation
-from .types.struct import AGlobalStructType, AStructType, DynamicStructType
-
-
-class Idents(Namespace):
-    """
-    Identifier Dictionary.
-
-    See examples above.
-    """
+from .nameutil import join_names, split_suffix
+from .object import Field, NamedObject
+from .orientation import AOrientation
+from .typearray import ArrayType
+from .typebase import BaseType
+from .typestruct import BaseStructType
 
-    def iter(self, filter_=None, stop=None, maxlevel=None) -> Iterator:
-        """Iterate over all Identifier."""
-        for ident in self.values():
-            yield from ident.iter(filter_=filter_, stop=stop, maxlevel=maxlevel)
-
-    def iterhier(self, filter_=None, stop=None, maxlevel=None) -> Iterator:
-        """Iterate over all Identifier and return hierarchy."""
-        for ident in self.values():
-            yield from ident.iterhier(filter_=filter_, stop=stop, maxlevel=maxlevel)
-
-    def findfirst(self, filter_=None, stop=None, maxlevel=None) -> Optional["Ident"]:
-        """Iterate Over Identifier And Find First Match."""
-        for ident in self.iter(filter_=filter_, stop=stop, maxlevel=maxlevel):
-            return ident
-        return None
 
-    def __getitem__(self, name):
-        return get_ident(self, name)
-
-    def get(self, name):
-        return get_ident(self, name, dym=True)
-
-    def __contains__(self, item):
-        if isinstance(item, Ident):
-            name = item.name
-        elif isinstance(item, str):
-            name = item
-        else:
-            return False
-        return _get_ident(self.values(), name) is not None
-
-
-@frozen(cmp=False, hash=True)
-class Ident(Expr):
-
-    """
-    Identifier.
+class Ident(Expr, NamedObject):
+    """Identifier.
 
     Args:
         type_: Type.
-        name (str): Hierarchical name.
+        name: Name.
 
-    Keyword Args:
-        direction: (Direction): Orient or Direction.
-        dims: (tuple): Dimensions
-        level (int): Hierarchy Level
-        doc (Doc): Documentation Container
-        ifdef (str): IFDEF encapsulation
-
-    >>> import ucdp
-    >>> ident = Ident(ucdp.UintType(32), 'base_sub_i', level=1)
-    >>> ident.type_
-    UintType(32)
-    >>> ident.name
-    'base_sub_i'
-    >>> ident.level
-    1
-    >>> ident.direction
-    >>> ident.dims
-    ()
-    >>> ident.doc
-    Doc()
-
-    Calculated Properties:
-
-    >>> ident.basename
-    'base_sub_i'
-    >>> ident.suffix
-    ''
-    >>> ident.name
-    'base_sub_i'
+    Attributes:
+        direction: Direction.
+        doc: Documentation Container
+        ifdef: IFDEF encapsulation
+
+    ??? Example "Ident Examples"
+        Attributes:
+
+            >>> import ucdp as u
+            >>> ident = Ident(u.UintType(32), 'base_sub_i')
+            >>> ident.type_
+            UintType(32)
+            >>> ident.name
+            'base_sub_i'
+            >>> ident.direction
+            >>> ident.doc
+            Doc()
+
+        Calculated Properties:
+
+            >>> ident.basename
+            'base_sub'
+            >>> ident.suffix
+            '_i'
     """
 
-    # pylint: disable=too-many-instance-attributes
+    type_: BaseType
+    name: str = Field(pattern=PAT_IDENTIFIER)
+    direction: AOrientation | None = Field(default=None, init=False)
+    doc: Doc = Doc()
+    ifdef: str | None = None
 
-    type_: AType = field()
-    name: str = field()
-    basename: str = field(init=False)
-    suffix: str = field(init=False)
-    direction: Optional[AOrientation] = field(default=None, kw_only=True)
-    level: int = field(default=0, kw_only=True)
-    dims: Tuple[Slice, ...] = field(default=tuple(), kw_only=True)
-    doc: Doc = field(default=Doc(), kw_only=True)
-    ifdef: Optional[str] = field(default=None, kw_only=True)
-
-    _children = field(init=False, factory=list, hash=False)
-    _suffixes: Tuple[str, ...] = ()
-
-    @name.validator
-    def _name_validator(self, name, value):
-        # pylint: disable=unused-argument
-        validate_identifier(value)
-
-    @basename.default
-    def _basename_default(self) -> str:
-        return split_suffix(self.name, suffixes=self._suffixes)[0]
-
-    @suffix.default
-    def _suffix_default(self) -> str:
-        return split_suffix(self.name, suffixes=self._suffixes)[1]
-
-    @type_.validator
-    def _type_validator(self, name, value):
-        # pylint: disable=unused-argument
-        if isclass(value) and issubclass(value, AType):
-            raise ValueError("{value!r} is a class, but must be an instance. You missed the brackets '()'!")
-
-    def __attrs_post_init__(self):
-        # Static Children are initialized here once instead of constructing
-        # them every time
-        type_ = self.type_
-        if isinstance(type_, (AGlobalStructType, AStructType)):
-            children = self._children
-            for sitem in type_.values():
-                level = self.level + 1
-                direction = self.direction and self.direction * sitem.orientation
-                # pylint: disable=consider-using-ternary
-                suffix = (direction and direction.suffix) or self.suffix
-                ibasename = self.basename
-                sname = sitem.name
-                basename = f"{ibasename}_{sname}" if ibasename and sname else ibasename or sname
-                name = f"{basename}{suffix}"
-                ifdef = sitem.ifdef or self.ifdef
-                child = evolve(
-                    self,
-                    type_=sitem.type_,
-                    name=name,
-                    level=level,
-                    direction=direction,
-                    dims=self.dims,
-                    doc=sitem.doc,
-                    ifdef=ifdef,
-                )
-                children.append(child)
-        elif isinstance(type_, ArrayType):
-            dims = self.dims + (type_.slice_,)
-            self._children.append(evolve(self, type_=type_.type_, dims=dims))
+    _posargs: tuple[str, ...] = ("type_", "name")
 
-    @property
-    def title(self):
-        """Alias to `doc.title`."""
-        return self.doc.title
+    def __init__(self, type_: BaseType, name: str, **kwargs):
+        super().__init__(type_=type_, name=name, **kwargs)  # type: ignore[call-arg]
 
     @property
-    def descr(self):
-        """Alias to `doc.descr`."""
-        return self.doc.descr
+    def basename(self):
+        """Base Name."""
+        return split_suffix(self.name)[0]
 
     @property
-    def comment(self):
-        """Alias to `doc.comment`."""
-        return self.doc.comment
-
-    def new(self, **kwargs) -> "Ident":
-        """Return A Copy With Updated Attributes."""
-        return evolve(self, **kwargs)
+    def suffix(self):
+        """Suffix."""
+        return split_suffix(self.name)[1]
+
+    def __str__(self) -> str:
+        return self.name
 
     def __int__(self):
         return int(self.type_.default)
 
     def __iter__(self):
-        return self.iter()
+        return _iters([self])
 
-    def iter(self, filter_=None, stop=None, maxlevel=None, value=None) -> Iterator:
+    def iter(self, filter_=None, stop=None, value=None) -> Iterator:
         """Iterate over Hierarchy."""
-        return _iters([self], filter_=filter_, stop=stop, maxlevel=maxlevel, value=value)
+        return _iters([self], filter_=filter_, stop=stop, value=value)
 
-    def iterhier(self, filter_=None, stop=None, maxlevel=None, value=None) -> Iterator:
-        """Iterate over Hierarchy."""
-        hier: List[Ident] = []
-        for ident in self.iter(stop=stop, maxlevel=maxlevel, value=value):
-            hier = hier[: ident.level] + [ident]
-            if not filter_ or filter_(ident):
-                yield tuple(hier)
 
-    def get(self, name, value=None):
-        """
-        Get Member of Hierarchy.
+#     def iterhier(self, filter_=None, stop=None, maxlevel=None, value=None) -> Iterator:
+#         """Iterate over Hierarchy."""
+#         hier: List[Ident] = []
+#         for ident in self.iter(stop=stop, maxlevel=maxlevel, value=value):
+#             hier = hier[: ident.level] + [ident]
+#             if not filter_ or filter_(ident):
+#                 yield tuple(hier)
+
+#     def get(self, name, value=None):
+#         """
+#         Get Member of Hierarchy.
+
+#         Args:
+#             name: Name
+
+#         Keyword Args:
+#             value: value
+#             dym (bool): Enriched `ValueError` exception.
+#         """
+#         if name.startswith("_"):
+#             name = f"{self.basename}{name}"
+#         return get_ident([self], name, value=value, dym=True)
+
+IdentFilter = Callable[[Ident], bool]
+IdentStop = Callable[[Ident], bool]
+
+
+class Idents(Namespace):
+    """
+    Identifier Dictionary.
+
+    See examples above.
+    """
+
+    def iter(self, filter_: IdentFilter | None = None, stop: IdentStop | None = None) -> Iterator[Ident]:
+        """Iterate over all Identifier."""
+        for ident in self.values():
+            yield from ident.iter(filter_=filter_, stop=stop)
 
-        Args:
-            name: Name
+    # def iterhier(self, filter_=None, stop=None, maxlevel=None) -> Iterator:
+    #     """Iterate over all Identifier and return hierarchy."""
+    #     for ident in self.values():
+    #         yield from ident.iterhier(filter_=filter_, stop=stop, maxlevel=maxlevel)
+
+    # def findfirst(self, filter_=None, stop=None, maxlevel=None) -> "Ident" | None:
+    #     """Iterate Over Identifier And Find First Match."""
+    #     for ident in self.iter(filter_=filter_, stop=stop, maxlevel=maxlevel):
+    #         return ident
+    #     return None
+
+    def __getitem__(self, name):
+        return get_ident(self, name)
 
-        Keyword Args:
-            value: value
-            dym (bool): Enriched `ValueError` exception.
-        """
-        if name.startswith("_"):
-            name = f"{self.basename}{name}"
-        return get_ident([self], name, value=value, dym=True)
+    def __contains__(self, item: Any) -> bool:
+        if isinstance(item, Ident):
+            name = item.name
+        elif isinstance(item, str):
+            name = item
+        else:
+            return False
+        return _get_ident(self.values(), name) is not None
 
 
-def _iters(idents, filter_=None, stop=None, maxlevel=None, value=None):
+def _iters(idents: Iterable[Ident], filter_=None, stop=None, value=None) -> Iterator[Ident]:  # noqa: C901
     # highly optimized!
-    # pylint: disable=too-many-locals,too-many-nested-blocks,too-many-branches
-    for ident in idents:
-        stack = deque([ident])
+
+    for rootident in idents:
+        stack = deque([rootident])
         while True:
             try:
                 ident = stack.pop()
             except IndexError:
                 break
+
             if stop and stop(ident):
                 break
+
             type_ = ident.type_
             assert value is None, "TODO"
-            # pylint: disable=protected-access
-            if type_._yield and (not filter_ or filter_(ident)):
+
+            if not filter_ or filter_(ident):
                 yield ident
-            if isinstance(type_, (AGlobalStructType, AStructType)):
-                level = ident.level + 1
-                if maxlevel is None or level <= maxlevel:
-                    for child in reversed(ident._children):
-                        if not stop or not stop(child):
-                            stack.append(child)
-            elif isinstance(type_, DynamicStructType):
-                level = ident.level + 1
-                if maxlevel is None or level <= maxlevel:
-                    for sitem in reversed(type_.values()):
-                        direction = ident.direction and ident.direction * sitem.orient
-                        # pylint: disable=consider-using-ternary
-                        suffix = (direction and direction.suffix) or ident.suffix
-                        ibasename = ident.basename
-                        sname = sitem.name
-                        basename = f"{ibasename}_{sname}" if ibasename and sname else ibasename or sname
-                        name = f"{basename}{suffix}"
-                        ifdef = sitem.ifdef or ident.ifdef
-                        child = evolve(
-                            ident,
-                            type_=sitem.type_,
-                            name=name,
-                            level=level,
-                            direction=direction,
-                            doc=sitem.doc,
-                            ifdef=ifdef,
-                        )
-                        if not stop or not stop(child):
-                            stack.append(child)
+            if isinstance(type_, BaseStructType):
+                for structitem in reversed(type_.values()):
+                    direction = ident.direction and ident.direction * structitem.orientation
+                    suffix = (direction and direction.suffix) or ident.suffix
+                    basename = join_names(ident.basename, structitem.name)
+                    child = ident.new(
+                        type_=structitem.type_,
+                        name=f"{basename}{suffix}",
+                        direction=direction,
+                        doc=structitem.doc,
+                        ifdef=structitem.ifdef or ident.ifdef,
+                    )
+                    if not stop or not stop(child):
+                        stack.append(child)
             elif isinstance(type_, ArrayType):
-                dims = ident.dims + (type_.slice_,)
-                child = evolve(ident, type_=type_.type_, dims=dims)
-                if not stop or not stop(child):
-                    stack.append(child)
+                elementident = ident.new(type_=type_.itemtype)
+                # do not forward stop and filter_ as these are just intermediate identifiers
+                subidents = tuple(_iters([elementident]))
+                for subident in subidents[1:]:
+                    # create array with new element type
+                    childtype = type_.new(itemtype=subident.type_)
+                    child = subident.new(type_=childtype)
+                    if not stop or not stop(child):
+                        stack.append(child)
 
 
-def get_ident(idents, name, value=None, dym=False):
+def get_ident(idents: Iterable[Ident], name: str, value=None, dym=False) -> Ident | None:
     """Retrieve identifier by `name`, without iterating over the entire identifier tree."""
     assert value is None, "TODO"
     ident = _get_ident(idents, name)
     if ident is not None:
         return ident
 
     # Beautiful error handling
     msg = f"'{name}' is not known."
-    if dym and any(idents):
-        names = [ident.name for ident in _iters(idents)]
-        nametree = align(_get_identtree(idents), rtrim=True)
-        msg += f" Known are\n{nametree}\n\n{msg}\n"
-        msg += didyoumean(name, names, multiline=True)
+    #     if dym and any(idents):
+    #         names = [ident.name for ident in _iters(idents)]
+    #         nametree = align(_get_identtree(idents), rtrim=True)
+    #         msg += f" Known are\n{nametree}\n\n{msg}\n"
+    #         msg += didyoumean(name, names, multiline=True)
     raise ValueError(msg)
 
 
-def get_subname(parent: Ident, ident: Ident):
-    """Get name relative to parent."""
-    if parent is ident:
-        return ident.suffix
-    parentbasename = parent.basename
-    name = ident.name
-    assert name.startswith(parentbasename)
-    return name[len(parentbasename) + 1 :]
-
-
-def get_subnames(idents):
-    """Return names of hierarchical idents."""
-    names = []
-    prefix = ""
-    for ident in idents:
-        basename = ident.basename
-        names.append(basename.removeprefix(prefix))
-        prefix = f"{basename}_"
-    return names
-
-
-def _get_ident(idents, name):
-    # This method is a derived implementation of _iters and has to be kept in sync with it.
-    idents = deque(idents)
-    while True:
-        try:
-            ident = idents.pop()
-        except IndexError:
-            break
-        type_ = ident.type_
-        # pylint: disable=protected-access
-        if type_._yield and ident.name == name:
+# def get_subname(parent: Ident, ident: Ident):
+#     """Get name relative to parent."""
+#     if parent is ident:
+#         return ident.suffix
+#     parentbasename = parent.basename
+#     name = ident.name
+#     assert name.startswith(parentbasename)
+#     return name[len(parentbasename) + 1 :]
+
+
+# def get_subnames(idents):
+#     """Return names of hierarchical idents."""
+#     names = []
+#     prefix = ""
+#     for ident in idents:
+#         basename = ident.basename
+#         names.append(basename.removeprefix(prefix))
+#         prefix = f"{basename}_"
+#     return names
+
+
+def _get_ident(idents, name) -> Ident | None:
+    # TODO: optimize
+    for ident in _iters(idents):
+        if ident.name == name:
             return ident
-        # pylint: disable=protected-access
-        if type_._dynamic:
-            for sitem in reversed(type_.values()):
-                ibasename = ident.basename
-                sname = sitem.name
-                basename = f"{ibasename}_{sname}" if ibasename and sname else ibasename or sname
-                if name.startswith(basename):
-                    level = ident.level + 1
-                    direction = ident.direction and ident.direction * sitem.orient
-                    # pylint: disable=consider-using-ternary
-                    suffix = (direction and direction.suffix) or ident.suffix
-                    sname = f"{basename}{suffix}"
-                    ifdef = sitem.ifdef or ident.ifdef
-                    child = evolve(
-                        ident,
-                        type_=sitem.type_,
-                        name=sname,
-                        level=level,
-                        direction=direction,
-                        doc=sitem.doc,
-                        ifdef=ifdef,
-                    )
-                    idents.append(child)
-        else:
-            # pylint: disable=protected-access
-            for child in ident._children:
-                if name.startswith(child.basename):
-                    idents.append(child)
     return None
 
 
-def _get_identtree(idents, pre=""):
-    for ident in _iters(idents):
-        pre = "  " * ident.level
-        yield f"{pre}'{ident.name}'", ident.type_
+# def _get_identtree(idents, pre=""):
+#     for ident in _iters(idents):
+#         pre = "  " * ident.level
+#         yield f"{pre}'{ident.name}'", ident.type_
+
+
+def get_expridents(expr: Expr) -> tuple[Ident, ...]:
+    """
+    Determine used identifier in `expr`.
+    """
+    idents = {}
+    heap = deque((expr,))
+    while heap:
+        item = heap.popleft()
+        if isinstance(item, ConstExpr):
+            pass
+        elif isinstance(item, Op):
+            heap.append(item.left)
+            heap.append(item.right)
+        elif isinstance(item, (SOp, SliceOp)):
+            heap.append(item.one)
+        elif isinstance(item, (ConcatExpr, MinimumExpr, MaximumExpr)):
+            heap.extend(item.items)
+        elif isinstance(item, TernaryExpr):
+            heap.append(item.cond.left)
+            heap.append(item.cond.right)
+            heap.append(item.one)
+            heap.append(item.other)
+        elif isinstance(item, Log2Expr):
+            heap.append(item.expr)
+        elif isinstance(item, Ident):
+            if item.name not in idents:
+                idents[item.name] = item
+        else:
+            raise TypeError(f"Unknown expr {item}")
+    return tuple(idents.values())
```

### Comparing `ucdp-0.1.0/ucdp/loader.py` & `ucdp-0.2.0/src/ucdp/loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,75 +19,71 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 """
-Top Loading.
+Loader.
 
 * :any:`load()` is one and only method to pickup and instantiate the topmost hardware module.
 """
-import logging
+
 from functools import lru_cache
 from importlib import import_module
-from typing import Union
 
 from caseconverter import pascalcase
 
-from .mod.base import BaseMod
-from .mod.iter import get_mod
-from .mod.mods import ATbMod
+from .logging import LOGGER
+from .modbase import BaseMod
+from .moditer import get_mod
 from .modref import ModRef
+from .modtb import ATbMod
+from .modtopref import TopModRef
 from .top import Top
-from .topref import TopRef
-
-_LOGGER = logging.getLogger("ucdp")
 
 
-def load(topref: Union[TopRef, str]) -> Top:
+def load(topmodref: TopModRef | str) -> Top:
     """
-    Load Module from ``topref`` and return :any:`Top`.
-
-    Args:
-        topref (TopRef):
+    Load Module from ``topmodref`` and return :any:`Top`.
 
     Load ``topref.top``.
 
     In case of a given ``topref.sub`` search for a submodule named ``sub`` within the
     module hierarchy of ``topmod`` using :any:`Top.get_mod()`.
 
     In case of a given ``tb`` search for a testbench ``tb`` and pair it.
     """
-    topref = TopRef.convert(topref)
-    topmod = _load_topmod(topref)
-    return Top(topref, topmod)
+    topmodref = TopModRef.cast(topmodref)
+    mod = _load_topmod(topmodref)
+    return Top(ref=topmodref, mod=mod)
 
 
 @lru_cache
-def _load_topmod(topref: TopRef) -> BaseMod:
-    _LOGGER.info("Loading %s", topref)
+def _load_topmod(ref: TopModRef) -> BaseMod:
+    LOGGER.info("Loading %r", str(ref))
 
-    modcls = _load_modcls(topref.top)
+    modcls = _load_modcls(ref.top)
     mod = _build_top(modcls)
-    if topref.sub:
-        mod = get_mod(mod, str(topref.sub))
-    if topref.tb:
-        tbcls = _load_modcls(topref.tb)
+    if ref.sub:
+        mod = get_mod(mod, ref.sub)
+    if ref.tb:
+        tbcls = _load_modcls(ref.tb)
         if not issubclass(tbcls, ATbMod):
-            raise ValueError(f"{tbcls} is not a testbench module")
+            raise ValueError(f"{tbcls} is not a testbench module aka child of <class ucdp.ATbMod>.")
         return tbcls.build_tb(mod)
     return mod
 
 
 @lru_cache
 def _build_top(modcls, **kwargs):
     return modcls.build_top(**kwargs)
 
 
 @lru_cache
 def _load_modcls(modref: ModRef):
-    """Load Module Class."""
-    pymodname = f"{modref.pkg}.{modref.mod}" if modref.pkg else modref.mod
-    pymod = import_module(pymodname)
-    clsname = modref.cls if modref.cls else f"{pascalcase(modref.mod)}Mod"
-    return getattr(pymod, clsname)
+    pymod = import_module(f"{modref.lib}.{modref.mod}")
+    modclsname = modref.modcls or f"{pascalcase(modref.mod)}Mod"
+    modcls = getattr(pymod, modclsname)
+    if not issubclass(modcls, BaseMod):
+        raise ValueError(f"{modcls} is not a module aka child of <class ucdp.BaseMod>.")
+    return modcls
```

### Comparing `ucdp-0.1.0/ucdp/mod/__init__.py` & `ucdp-0.2.0/src/ucdp/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,9 +19,13 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 """
-Modules.
+Logging.
 """
+
+import logging
+
+LOGGER = logging.getLogger("ucdp")
```

### Comparing `ucdp-0.1.0/ucdp/mod/config.py` & `ucdp-0.2.0/src/ucdp/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,228 +18,177 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """Configuration."""
+
 import datetime
 import hashlib
-from pathlib import Path
-
-from humannum import Hex, hex_
-
-from ..attrs import asdict, define, evolve, field
-from ..nameutil import validate_identifier
-from ..util import opt
-
-
-def config(maybe_cls=None, **kwargs):
-    """Configuration Decorator - see :any:`BaseConfig`."""
-    return define(maybe_cls, frozen=True, repr=False, **kwargs)
-
 
-@config
-class BaseConfig:
-    """Base Class for all Configurations."""
+from .consts import PAT_IDENTIFIER
+from .object import Field, LightObject
 
-    name: str = ""
 
-    def __repr__(self):
-        return f"{self.__class__.__qualname__}({self.name!r})"
-
-    def new(self, **kwargs) -> "BaseConfig":
-        """Return A Copy With Updated Attributes."""
-        return evolve(self, **kwargs)
-
-    def iter_overview(self):
-        """Iterate Overview."""
-        yield from asdict(self, recurse=False).items()
-
-
-@config
-class AConfig(BaseConfig):
+class AConfig(LightObject):
     """
     Configuration Container.
 
     Args:
-        name (str): Configuration name, used as suffix of the generated module.
+        name: Configuration name, used as suffix of the generated module.
 
     A configuration is nothing more than a receipe how to assemble a module:
 
     * if a specific option should be built-in or not
     * how many instances or which instances should be created
 
     A configuration **MUST** have at least a name.
 
     Due to the frozen instance approach, configurations have to be implemented
-    via `ucdp.field()`.
+    via `u.field()`.
 
     Example:
-
-    >>> import ucdp
-    >>> from humannum import bytes_, hex_
-    >>> @ucdp.config
-    ... class MyConfig(ucdp.AConfig):
-    ...
-    ...     mem_baseaddr = ucdp.field(converter=hex_) # required without default
-    ...     ram_size = ucdp.field(converter=bytes_, default="256 KB")  # required with default
-    ...     rom_size = ucdp.field(converter=opt(bytes_), default=None)  # optional
-    ...     feature: bool = ucdp.field(default=False) # boolean
-
-    >>> variant0  = MyConfig('variant0', 4*1024)
-    >>> variant0
-    MyConfig('variant0')
-    >>> variant0.mem_baseaddr
-    Hex('0x1000')
-    >>> variant0.ram_size
-    Bytes('256 KB')
-    >>> variant0.rom_size
-    >>> variant0.feature
-    False
-
-    >>> for name, value in variant0.iter_overview():
-    ...     name, value
-    ('name', 'variant0')
-    ('mem_baseaddr', Hex('0x1000'))
-    ('ram_size', Bytes('256 KB'))
-    ('rom_size', None)
-    ('feature', False)
-
-    >>> variant1  = MyConfig('variant1', 8*1024, rom_size="2KB", ram_size="4KB", feature=True)
-    >>> variant1
-    MyConfig('variant1')
-    >>> variant1.mem_baseaddr
-    Hex('0x2000')
-    >>> variant1.ram_size
-    Bytes('4 KB')
-    >>> variant1.rom_size
-    Bytes('2 KB')
-    >>> variant1.feature
-    True
+        >>> import ucdp as u
+        >>> class MyConfig(u.AConfig):
+        ...
+        ...     mem_baseaddr: u.Hex # required without default
+        ...     ram_size: u.Bytes
+        ...     rom_size: u.Bytes|None = None
+        ...     feature: bool = False
+
+        >>> variant0  = MyConfig(name='variant0', mem_baseaddr=4*1024, ram_size='16kB')
+        >>> variant0
+        MyConfig('variant0', mem_baseaddr=Hex('0x1000'), ram_size=Bytes('16 KB'))
+        >>> variant0.mem_baseaddr
+        Hex('0x1000')
+        >>> variant0.ram_size
+        Bytes('16 KB')
+        >>> variant0.rom_size
+        >>> variant0.feature
+        False
+
+        >>> for name, value in variant0:
+        ...     name, value
+        ('name', 'variant0')
+        ('mem_baseaddr', Hex('0x1000'))
+        ('ram_size', Bytes('16 KB'))
+        ('rom_size', None)
+        ('feature', False)
+
+        >>> variant1  = MyConfig('variant1', mem_baseaddr=8*1024, rom_size="2KB", ram_size="4KB", feature=True)
+        >>> variant1
+        MyConfig('variant1', mem_baseaddr=Hex('0x2000'), ram_size=Bytes('4 KB'), rom_size=Bytes('2 KB'), feature=True)
+        >>> variant1.mem_baseaddr
+        Hex('0x2000')
+        >>> variant1.ram_size
+        Bytes('4 KB')
+        >>> variant1.rom_size
+        Bytes('2 KB')
+        >>> variant1.feature
+        True
 
     To create another variant based on an existing:
 
     >>> variant2 = variant1.new(name='variant2', rom_size='8KB')
     >>> variant2
-    MyConfig('variant2')
+    MyConfig('variant2', mem_baseaddr=Hex('0x2000'), ram_size=Bytes('4 KB'), rom_size=Bytes('8 KB'), feature=True)
     >>> variant2.mem_baseaddr
     Hex('0x2000')
     >>> variant2.ram_size
     Bytes('4 KB')
     >>> variant2.rom_size
     Bytes('8 KB')
     >>> variant2.feature
     True
     """
 
-    name: str = field()
+    name: str = Field(pattern=PAT_IDENTIFIER)
 
-    @name.validator  # type: ignore
-    def _name_validator(self, attribute, value):
-        # pylint: disable=unused-argument
-        validate_identifier(value)
+    _posargs: tuple[str, ...] = ("name",)
 
+    def __init__(self, name, **kwargs):
+        super().__init__(name=name, **kwargs)
 
-@config
-class AUniqueConfig(BaseConfig):
 
+class AUniqueConfig(LightObject):
     """
     A Unique Configuration.
 
     The configuration name is automatically derived from the attribute values.
 
-    >>> import ucdp
+    >>> import ucdp as u
     >>> import datetime
     >>> from typing import Tuple
-    >>> @ucdp.config
-    ... class MyUniqueConfig(ucdp.AUniqueConfig):
-    ...     mem_baseaddr: int = ucdp.field(converter=hex_)
-    ...     width: int = ucdp.field(default=32)
-    ...     feature: bool = ucdp.field(default=False)
-    ...     coeffs: Tuple[int, ...] = ucdp.field(factory=tuple)
+    >>> class MyUniqueConfig(u.AUniqueConfig):
+    ...     mem_baseaddr: u.Hex
+    ...     width: int = 32
+    ...     feature: bool = False
+    ...     coeffs: tuple[int, ...] = tuple()
 
     >>> config = MyUniqueConfig(
     ...     mem_baseaddr=0x12340000,
     ... )
     >>> config.name
-    'aa440a0fab478a72'
+    '5e813dde214238ae'
 
-    >>> for name, value in config.iter_overview():
+    >>> for name, value in config:
     ...     name, value
     ('mem_baseaddr', Hex('0x12340000'))
     ('width', 32)
     ('feature', False)
     ('coeffs', ())
 
     >>> config = MyUniqueConfig(
     ...     mem_baseaddr=0x12340000,
     ...     coeffs=(1,2,3),
     ... )
     >>> config.name
-    '087561fbb5f4aaac'
+    '9818217751e9d3b4'
     """
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Assembled name from configuration values."""
-        parts = []
-        for value in asdict(self, recurse=False).values():
-            if isinstance(value, bool):
-                value = int(value)
-            parts.append(str(value).replace(" ", ""))
-        return hashlib.sha256("_".join(parts).encode("utf-8")).hexdigest()[:16]
+        return hashlib.sha256(str(self.model_dump()).encode("utf-8")).hexdigest()[:16]
 
 
-@config
-class AVersionConfig(AConfig):
+BaseConfig = AConfig | AUniqueConfig
 
+
+class AVersionConfig(AConfig):
     """
     Version Configuration Container.
 
-    >>> import ucdp
+    >>> import ucdp as u
     >>> import datetime
-    >>> @ucdp.config
-    ... class MyVersionConfig(ucdp.AVersionConfig):
-    ...     mem_baseaddr = ucdp.field(converter=hex_) # required without default
+    >>> class MyVersionConfig(u.AVersionConfig):
+    ...     mem_baseaddr: u.Hex
 
     >>> version = MyVersionConfig(
     ...     'my',
     ...     title="Title",
     ...     version="1.2.3",
     ...     timestamp=datetime.datetime(2020, 10, 17, 23, 42),
-    ...     rand=0x65DDB0631,
-    ...     file=__file__,
     ...     mem_baseaddr=0x12340000
     ... )
     >>> version.name
     'my'
     >>> version.title
     'Title'
     >>> version.timestamp
     datetime.datetime(2020, 10, 17, 23, 42)
-    >>> version.rand
-    Hex('0x65DDB0631')
     >>> version.mem_baseaddr
     Hex('0x12340000')
 
-    >>> for name, value in version.iter_overview():
+    >>> for name, value in version:
     ...     name, value
     ('name', 'my')
     ('title', 'Title')
     ('version', '1.2.3')
     ('timestamp', datetime.datetime(2020, 10, 17, 23, 42))
     ('mem_baseaddr', Hex('0x12340000'))
     """
 
-    title: str = field(kw_only=True)
-    version: str = field(kw_only=True)
-    timestamp: datetime.datetime = field(kw_only=True)
-    rand: Hex = field(kw_only=True, converter=opt(hex_))
-    file: Path = field(kw_only=True)
-
-    def iter_overview(self):
-        """Iterate Overview."""
-        for name, value in asdict(self, recurse=False).items():
-            if name in ("rand", "file"):
-                continue
-            yield name, value
+    title: str
+    version: str
+    timestamp: datetime.datetime
```

### Comparing `ucdp-0.1.0/ucdp/mod/util.py` & `ucdp-0.2.0/src/ucdp/modconfigurable.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,85 +18,91 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
+"""
+Configurable Module.
+"""
 
-"""Module Utilities."""
+from typing import ClassVar
 
-from collections import deque
-from typing import Optional
+from caseconverter import snakecase
 
-from .base import BaseMod
-from .config import AVersionConfig
-from .mods import CoreMod
+from .config import BaseConfig
+from .modbase import BaseMod
+from .modbasetop import BaseTopMod
+from .nameutil import join_names
 
 
-def get_topmod(mod: BaseMod) -> BaseMod:
-    """Return topmost module of `mod`."""
-    while mod.parent:
-        mod = mod.parent
-    return mod
-
+class AConfigurableMod(BaseTopMod):
+    """
+    A Module Which Is Assembled According To A Receipe (:any:`AConfig`).
 
-def get_modbase(mod, required=False):
-    """Return module basemodule."""
-    modbasename = mod.modbasenames[0]
-    base = modbasename if isinstance(mod, CoreMod) or required or mod.modname != modbasename else None
-    while isinstance(mod, CoreMod):
-        subbase = get_modbase(mod.parent, required=True)
-        base = f"{subbase}/{base}"
-        mod = mod.parent
-    return base
+    See :any:`BaseMod` for arguments, attributes and details.
 
+    Additionally the config has to be provided at instantiation.
+    A :any:`AConfigurableMod` may define a `default_config` which is taken if no `config` is provided at instantiaion.
 
-def walk(mod, ref):
-    """
-    Walk from `mod` to `ref`.
+    All module parameter, local parameter, ports, signals and submodules
+    **MUST** be added and created within the `_build` method depending on the config.
+
+
+    .. attention:: It is forbidden to implement `add` methods or any other *tailored* functionality.
+                   Use a tailored module instead!
+
+    Configurable modules are located next to the python file and use the configuration name in the module name.
+
+    Example:
+    >>> import ucdp as u
+    >>> class MyConfig(u.AConfig):
+    ...
+    ...     feature: bool = False
+
+    >>> class ProcMod(u.AConfigurableMod):
+    ...
+    ...     default_config = MyConfig('default')
+    ...
+    ...     def _build(self) -> None:
+    ...         if self.config.feature:
+    ...             self.add_port(u.UintType(8), "feature_i")
+    ...             self.add_port(u.UintType(8), "feature_o")
+    ...         else:
+    ...             self.add_port(u.UintType(8), "default_o")
+
+    >>> my = ProcMod()
+    >>> my.modname
+    'proc_default'
+    >>> my.ports
+    Idents([Port(UintType(8), 'default_o', direction=OUT)])
+
+    >>> my = ProcMod(config=MyConfig('other', feature=True))
+    >>> my.modname
+    'proc_other'
+    >>> my.ports
+    Idents([Port(UintType(8), 'feature_i', direction=IN), Port(UintType(8), 'feature_o', direction=OUT)])
     """
-    yield from _get_relpath(mod, ref)
 
+    default_config: ClassVar[BaseConfig | None] = None
+    config: BaseConfig
 
-def get_relpath(mod, ref):
-    """Determine Relative path of `mod` to `ref`."""
-    return tuple(item.name for item in _get_relpath(mod, ref))
-
-
-def _get_relpath(mod, ref):
-    """Determine Relative path of `mod` to `ref`."""
-    if mod is ref:
-        return tuple()
-    stack = deque([(mod, [])])
-    while stack:
-        mod, path = stack.pop()
-        while mod.parents and ref not in mod.parents:
-            path.insert(0, mod)
-            if len(mod.parents) > 1:
-                for parent in mod.parents[1:]:
-                    stack.appendleft((parent, path))
-            mod = mod.parents[0]
-        if ref in mod.parents:
-            path.insert(0, mod)
-            return tuple(path)
-    raise ValueError(f"{mod} is not a submodule of {ref}")
-
-
-def get_versionconfig(mod, required=False) -> Optional[AVersionConfig]:
-    """Return :any:`AVersionConfig`."""
-    config = getattr(mod, "version_config", None) or getattr(mod, "config", None)
-    if config:
-        if not isinstance(config, AVersionConfig):
-            raise ValueError(f"{config} is not a ucdp.AVersionConfig")
-        return config
-    if required:
-        raise ValueError(f"No 'config' or 'version_config' found on {mod}")
-    return None
-
-
-def get_version(mod, required=False):
-    """Return version of mod."""
-    config = get_versionconfig(mod, required=required)
-    if config:
-        return config.version
-    return None
+    def __init__(
+        self, parent: BaseMod | None = None, name: str | None = None, config: BaseConfig | None = None, **kwargs
+    ):
+        if config is None:
+            config = self.__class__.default_config
+        super().__init__(parent=parent, name=name, config=config, **kwargs)  # type: ignore[call-arg]
+
+    @property
+    def modname(self) -> str:
+        """Module Name."""
+        modname = self.basename
+        if self.config:
+            return join_names(modname, self.config.name)
+        return modname
+
+    @property
+    def topmodname(self) -> str:
+        """Top Module Name."""
+        return snakecase(self.__class__.__name__.removesuffix("Mod"))
```

### Comparing `ucdp-0.1.0/ucdp/modref.py` & `ucdp-0.2.0/src/ucdp/modref.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,99 +18,90 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
-"""Module Specification."""
+"""Module Reference."""
+
+# DOCME: pkg vs lib
 
 import re
-from typing import Optional, Union
+from typing import Union
 
-from .attrs import field, frozen
+from .consts import PAT_IDENTIFIER
+from .object import Field, LightObject
 
+RE_MODREF = re.compile(
+    # lib
+    r"(?P<lib>[a-zA-Z][a-zA-Z_0-9]*)\."
+    # mod
+    r"(?P<mod>[a-zA-Z][a-zA-Z_0-9]*)"
+    # cls
+    r"(\.(?P<modcls>[A-Z][a-zA-Z_0-9]*Mod))?"
+)
+PAT_MODREF = "lib.my[.MyMod]"
 
-@frozen
-class ModRef:
 
+class ModRef(LightObject):
     """
-    Module Specification.
+    Module Reference.
 
     Args:
+        lib: Library Name
         mod: Module Name
 
     Keyword Args:
-        pkg: Package Name
-        cls: Class Name
+        modcls: Class Name
+
+    >>> ModRef('glbl_lib', 'clk_gate', modcls='ClkGateMod')
+    ModRef('glbl_lib', 'clk_gate', modcls='ClkGateMod')
+
+    Just a module:
+
+    >>> spec = ModRef.cast('glbl_lib.clk_gate')
+    >>> spec
+    ModRef('glbl_lib', 'clk_gate')
+    >>> str(spec)
+    'glbl_lib.clk_gate'
+
+    Module from a package and explicit class:
+
+    >>> spec = ModRef.cast('glbl_lib.clk_gate.ClkGateMod')
+    >>> spec
+    ModRef('glbl_lib', 'clk_gate', modcls='ClkGateMod')
+    >>> str(spec)
+    'glbl_lib.clk_gate.ClkGateMod'
+
+    Invalid Pattern:
+
+    >>> ModRef.cast('lib.my:c-ls')
+    Traceback (most recent call last):
+    ..
+    ValueError: 'lib.my:c-ls' does not match pattern 'lib.my[.MyMod]'
     """
 
-    mod: str = field()
-    pkg: str = field(default=None)
-    cls: Optional[str] = field(default=None)
-
-    _re = re.compile(
-        # pkg
-        r"((?P<pkg>[a-zA-Z][a-zA-Z_0-9]*)\.)?"
-        # mod
-        r"(?P<mod>[a-zA-Z][a-zA-Z_0-9]*)"
-        # cls
-        r"(\:(?P<cls>[a-zA-Z][a-zA-Z_0-9]*))?"
-    )
-    _pat = "lib.mod[:cls]"
+    lib: str = Field(pattern=PAT_IDENTIFIER)
+    mod: str = Field(pattern=PAT_IDENTIFIER)
+    modcls: str | None = Field(pattern=PAT_IDENTIFIER, default=None)
+
+    _posargs: tuple[str, ...] = ("lib", "mod")
+
+    def __init__(self, lib: str, mod: str, modcls: str | None = None):
+        super().__init__(lib=lib, mod=mod, modcls=modcls)  # type: ignore[call-arg]
+
+    def __str__(self) -> str:
+        modcls = f".{self.modcls}" if self.modcls else ""
+        return f"{self.lib}.{self.mod}{modcls}"
 
     @staticmethod
-    def convert(value: Union["ModRef", str]) -> "ModRef":
-        """
-        Convert.
-
-        Just a module:
-
-        >>> spec = ModRef.convert('mod')
-        >>> spec
-        ModRef('mod')
-        >>> str(spec)
-        'mod'
-
-        Module from a package:
-
-        >>> spec = ModRef.convert('lib.mod')
-        >>> spec
-        ModRef('mod', pkg='lib')
-        >>> str(spec)
-        'lib.mod'
-
-        Module from a package and explicit class:
-
-        >>> spec = ModRef.convert('lib.mod:cls')
-        >>> spec
-        ModRef('mod', pkg='lib', cls='cls')
-        >>> str(spec)
-        'lib.mod:cls'
-
-        A :any:`ModRef` is kept:
-
-        >>> ModRef.convert(ModRef('mod'))
-        ModRef('mod')
-
-        Invalid Pattern:
-
-        >>> ModRef.convert('mod:c-ls')
-        Traceback (most recent call last):
-        ..
-        ValueError: 'mod:c-ls' does not match pattern 'lib.mod[:cls]'
-        """
-
+    def cast(value: Union["ModRef", str]) -> "ModRef":
+        """Cast `value` to `ModRef`."""
         if isinstance(value, ModRef):
             return value
 
-        mat = ModRef._re.fullmatch(value)
+        mat = RE_MODREF.fullmatch(value)
         if mat:
             return ModRef(**mat.groupdict())
 
-        raise ValueError(f"{value!r} does not match pattern {ModRef._pat!r}")
-
-    def __str__(self):
-        pkg = f"{self.pkg}." if self.pkg else ""
-        mod = self.mod
-        cls = f":{self.cls}" if self.cls else ""
-        return f"{pkg}{mod}{cls}"
+        raise ValueError(f"{value!r} does not match pattern {PAT_MODREF!r}")
```

### Comparing `ucdp-0.1.0/ucdp/mux.py` & `ucdp-0.2.0/src/ucdp/mux.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,120 +18,99 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """Multiplexer."""
+
 from collections import defaultdict
-from typing import Generator
+from collections.abc import Iterator
 
-from .assigns import Assign, Assigns
-from .attrs import field, frozen
+from .assigns import Assign, Assigns, Drivers
 from .doc import Doc
-from .expr import Expr, parse
+from .expr import Expr
+from .exprparser import ExprParser, Parseable
 from .ident import Ident, Idents
-from .signal import Signal
-from .types.base import AScalarType, AVecType
-from .types.enum import AEnumType
+from .object import Field, NamedObject, computed_field
+from .signal import BaseSignal
+from .typebase import BaseScalarType
 
+MuxBranch = dict[Expr, Assigns]
 
-@frozen
-class Mux:
 
+class Mux(NamedObject):
     """
     Multiplexer.
 
     Args:
         name (str): Name
         targets (Idents): Ports and signals allowed to be assigned
         namespace (Idents): Ports, signals, parameter and local parameter as source
         drivers (dict): Drivers, for multiple-driver tracking.
     """
 
-    name: str = field()
-    targets: Idents = field(repr=False)
-    namespace: Idents = field(repr=False)
-    drivers: dict = field(repr=False)
-    doc: Doc = field(factory=Doc)
-
-    __assigns: Assigns = field(init=False)  # tracker of all assigned signals
-    __mux: dict = field(init=False)  # mux structure
-
-    @__assigns.default
-    def _assigns_default(self):
-        return Assigns(self.targets, self.namespace, drivers=self.drivers)
-
-    @__mux.default
-    def _mux_default(self):
-        return defaultdict(dict)
-
-    @property
-    def title(self):
-        """Alias to `doc.title`."""
-        return self.doc.title
+    targets: Idents = Field(repr=False)
+    namespace: Idents = Field(repr=False)
+    drivers: Drivers = Field(repr=False, default_factory=dict)
+    parser: ExprParser = Field(repr=False)
+    doc: Doc = Doc()
 
+    @computed_field(repr=False)
     @property
-    def descr(self):
-        """Alias to `doc.descr`."""
-        return self.doc.descr
+    def __assigns(self) -> Assigns:
+        return Assigns(targets=self.targets, sources=self.namespace, drivers=self.drivers)
 
+    @computed_field(repr=False)
     @property
-    def comment(self):
-        """Alias to `doc.comment`."""
-        return self.doc.comment
+    def __mux(self) -> dict[Expr, MuxBranch]:
+        return defaultdict(dict)
 
-    def set(self, sel: Signal, cond: Expr, out: Expr, value: Expr):
+    def set(self, sel: Parseable, cond: Parseable, out: Parseable, value: Parseable):
         """
         Set Multiplexer.
 
         Args:
-            sel (Signal): Select Signal
-            cond (Expr): Condition to be met on `sel`
-            out (Expr): Output to be assigned
-            value (Expr): Value.
+            sel: Select Signal
+            cond: Condition to be met on `sel`
+            out: Output to be assigned
+            value: Value.
         """
-        sel = parse(sel, namespace=self.namespace, types=(AScalarType, AVecType, AEnumType))
-        cond = parse(cond, namespace=self.namespace, strict=False)
-        out = parse(out, namespace=self.namespace)
-        value = parse(value, namespace=self.namespace)
-        # conditem = cond.range_ if isinstance(cond, Range) else cond
-        # if conditem not in sel.type_:
-        #     raise ValueError(f"Condition {cond} is not within range of {sel.type_}")
+        parse = self.parser.parse
+        selexpr = parse(sel, types=BaseScalarType)
+        condexpr = parse(cond)
+        outexpr: BaseSignal = parse(out, only=BaseSignal)  # type: ignore[assignment]
+        valueexpr = parse(value)
         mux = self.__mux
         # Track Assignments
-        self.__assigns.set(out, value, overwrite=True)
+        self.__assigns.set(outexpr, valueexpr, overwrite=True)
         # Mux Assignments
         try:
-            # pylint: disable=unsubscriptable-object
-            condassigns = mux[sel][cond]
+            condassigns = mux[selexpr][condexpr]
         except KeyError:
-            # pylint: disable=unsubscriptable-object
-            mux[sel][cond] = condassigns = Assigns(self.targets, self.namespace)
-        condassigns.set(out, value)
+            mux[selexpr][condexpr] = condassigns = Assigns(targets=self.targets, sources=self.namespace)
+        condassigns.set(outexpr, valueexpr)
 
-    def set_default(self, out: Expr, value: Expr):
+    def set_default(self, out: Parseable, value: Parseable):
         """
         Set Multiplexer.
 
         Args:
             out (Expr): Output to be assigned
             value (Expr): Value.
         """
-        out = parse(out, namespace=self.namespace)
-        value = parse(value, namespace=self.namespace)
-        self.__assigns.set_default(out, value)
+        parse = self.parser.parse
+        outexpr: BaseSignal = parse(out, only=BaseSignal)  # type: ignore[assignment]
+        valueexpr = parse(value)
+        self.__assigns.set_default(outexpr, valueexpr)
 
-    def defaults(self) -> Generator[Assign, None, None]:
+    def defaults(self) -> Iterator[Assign]:
         """Defaults."""
-        return self.__assigns.iter_defaults()
+        return self.__assigns.defaults()
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[tuple[Expr, MuxBranch]]:  # type: ignore[override]
         yield from self.__mux.items()
 
     @property
-    def sels(self) -> Generator[Ident, None, None]:
+    def sels(self) -> tuple[Ident, ...]:
         """Selects."""
-        return self.__mux.keys()
-
-    def __bool__(self):
-        return bool(self.__mux)
+        return tuple(self.__mux.keys())  # type: ignore[arg-type]
```

### Comparing `ucdp-0.1.0/ucdp/nameutil.py` & `ucdp-0.2.0/src/ucdp/nameutil.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,105 +17,58 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-"""Name Utilities."""
+
+"""
+Name Utilities.
+"""
+
 import functools
 import re
-from typing import Any, Tuple
 
 from caseconverter import snakecase
 from fuzzywuzzy import process
 from humanfriendly.text import concatenate
 
-_RE_SPLIT_PREFIX = re.compile(r"(?i)(?P<prefix>([a-z]|inst)_)(?P<basename>([a-z][a-z0-9\._]*)?)\Z")
-_RE_SPLIT_SUFFIX = re.compile(r"(?i)(?P<basename>([a-z][a-z0-9\._]*)?)(?P<suffix>_([a-z]|io))\Z")
-_RE_NAME = re.compile(r"[a-zA-Z0-9][a-zA-Z_0-9\-]*")
-_RE_IDENTIFIER = re.compile(r"[a-zA-Z][a-zA-Z_0-9]*")
-
-
-def validate_name(value: Any):
-    """
-    Ensure `value` is a name.
-
-    >>> validate_name('abc')
-    'abc'
-    >>> validate_name('_abc')
-    Traceback (most recent call last):
-        ...
-    ValueError: Invalid name '_abc'
-    >>> validate_name('aB9_a')
-    'aB9_a'
-    >>> validate_name('9ab')
-    '9ab'
-    """
-    if not _RE_NAME.fullmatch(str(value)):
-        raise ValueError(f"Invalid name '{value}'")
-    return value
-
-
-def validate_identifier(value: Any):
-    """
-    Ensure `value` is an identifier.
-
-    >>> validate_identifier('abc')
-    'abc'
-    >>> validate_identifier('_abc')
-    Traceback (most recent call last):
-        ...
-    ValueError: Invalid identifier '_abc'
-    >>> validate_identifier('aB9_a')
-    'aB9_a'
-    >>> validate_identifier('9ab')
-    Traceback (most recent call last):
-        ...
-    ValueError: Invalid identifier '9ab'
-    """
-    if not _RE_IDENTIFIER.fullmatch(str(value)):
-        raise ValueError(f"Invalid identifier '{value}'")
-    return value
+_FUZZY_MINRATIO: int = 80
+_RE_STARTNUM = re.compile(r"^[0-9]")
+_RE_SPLIT_PREFIX = re.compile(r"(?i)(?P<prefix>([a-z][a-z]?)_)(?P<basename>([a-z][a-z0-9_]*)?)\Z")
+_RE_SPLIT_SUFFIX = re.compile(r"(?i)(?P<basename>([a-z][a-z0-9_]*)?)(?P<suffix>_([a-z][a-z]?))\Z")
 
 
-@functools.lru_cache()
-def split_prefix(name: str, prefixes=None) -> Tuple[str, str]:
+@functools.lru_cache
+def split_prefix(name: str) -> tuple[str, str]:
     """
     Split Name Into Prefix and Basename.
 
     >>> split_prefix("i_count")
     ('i_', 'count')
     >>> split_prefix("u_count")
     ('u_', 'count')
-    >>> split_prefix("inst_count")
-    ('inst_', 'count')
     >>> split_prefix("I_VERY_LONG_NAME")
     ('I_', 'VERY_LONG_NAME')
     >>> split_prefix("BT_VERY_LONG_NAME")
-    ('', 'BT_VERY_LONG_NAME')
+    ('BT_', 'VERY_LONG_NAME')
     >>> split_prefix("")
     ('', '')
 
     The counterpart to this function is `join_names`.
     """
-
     mat = _RE_SPLIT_PREFIX.match(name)
     if mat:
-        if prefixes is not None:
-            prefix, basename = mat.group("prefix", "basename")  # type: ignore
-            if prefix in prefixes:
-                return prefix, basename
-        else:
-            return mat.group("prefix", "basename")  # type: ignore
+        return mat.group("prefix", "basename")  # type: ignore[return-value]
     return "", name
 
 
-@functools.lru_cache()
-def split_suffix(name: str, suffixes=None) -> Tuple[str, str]:
+@functools.lru_cache
+def split_suffix(name: str, suffixes=None) -> tuple[str, str]:
     """
     Split Name Into Basename And Suffix.
 
     >>> split_suffix("count_i")
     ('count', '_i')
     >>> split_suffix("count_o")
     ('count', '_o')
@@ -132,23 +85,17 @@
     >>> split_suffix("VERY_LONG_NAME_S")
     ('VERY_LONG_NAME', '_S')
     >>> split_suffix("")
     ('', '')
 
     The counterpart to this function is `join_names`.
     """
-
     mat = _RE_SPLIT_SUFFIX.match(name)
     if mat:
-        if suffixes is not None:
-            basename, suffix = mat.group("basename", "suffix")  # type: ignore
-            if suffix in suffixes:
-                return basename, suffix
-        else:
-            return mat.group("basename", "suffix")  # type: ignore
+        return mat.group("basename", "suffix")  # type: ignore[return-value]
     return name, ""
 
 
 def join_names(*names, concat="_") -> str:
     """
     Join Names.
 
@@ -180,24 +127,48 @@
     if known:
         knowns = concatenate(repr(name) for name in names)
         msg = f"{sep}Known are {knowns}."
     else:
         msg = ""
     # fuzzy
     if names:
-        fuzzyitems = (repr(item) for item, ratio in process.extract(name, names, limit=5) if ratio >= 80)
+        fuzzyitems = (repr(item) for item, ratio in process.extract(name, names, limit=5) if ratio >= _FUZZY_MINRATIO)
         fuzzy = concatenate(fuzzyitems, conjunction="or")
         if fuzzy:
             msg = f"{msg}{sep}Did you mean {fuzzy}?"
     return msg
 
 
-def get_snakecasename(cls):
+def get_snakecasename(item):
     """
     Get snakecase name of `cls`.
 
     >>> class MyClass:
     ...     pass
     >>> get_snakecasename(MyClass)
     'my_class'
+    >>> get_snakecasename("MyClass")
+    'my_class'
+    >>> get_snakecasename("MYClass")
+    'myclass'
+    """
+    if not isinstance(item, str):
+        item = item.__name__
+    return snakecase(item).removeprefix("_")
+
+
+def str2identifier(value: str) -> str:
+    """
+    Convert Any String To Identifier.
+
+    >>> str2identifier('A B C')
+    'a_b_c'
+    >>> str2identifier('1 2 3')
+    'v1_2_3'
+    >>> str2identifier('12.3')
+    'v123'
     """
-    return snakecase(cls.__name__).removeprefix("_")
+    value = snakecase(value)
+    mat = _RE_STARTNUM.match(value)
+    if mat:
+        value = f"v{value}"
+    return value
```

### Comparing `ucdp-0.1.0/ucdp/param.py` & `ucdp-0.2.0/src/ucdp/param.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -23,79 +23,75 @@
 #
 """
 Module Parameter .
 
 Usage:
 
 >>> from tabulate import tabulate
->>> import ucdp
->>> ucdp.Param(ucdp.UintType(6), "param_p")
+>>> import ucdp as u
+>>> u.Param(u.UintType(6), "param_p")
 Param(UintType(6), 'param_p')
 
 Also complex types can simply be used:
 
->>> class AType(ucdp.AStructType):
-...     def _build(self):
-...         self._add("req", ucdp.BitType())
-...         self._add("data", ucdp.ArrayType(ucdp.UintType(16), 5))
-...         self._add("ack", ucdp.BitType(), ucdp.BWD)
-...         self._add("error", ucdp.BitType(), ucdp.BIDIR)
->>> class MType(ucdp.AEnumType):
-...     keytype = ucdp.UintType(2)
-...     def _build(self):
+>>> class AType(u.AStructType):
+...     def _build(self) -> None:
+...         self._add("req", u.BitType())
+...         self._add("data", u.ArrayType(u.UintType(16), 5))
+...         self._add("ack", u.BitType(), u.BWD)
+>>> class MType(u.AEnumType):
+...     keytype: u.AScalarType = u.UintType(2)
+...     def _build(self) -> None:
 ...         self._add(0, "Linear")
 ...         self._add(1, "Cyclic")
->>> class BType(ucdp.AStructType):
-...     def _build(self):
+>>> class BType(u.AStructType):
+...     def _build(self) -> None:
 ...         self._add("foo", AType())
 ...         self._add("mode", MType())
-...         self._add("bar", ucdp.ArrayType(AType(), 3), ucdp.BWD)
+...         self._add("bar", u.ArrayType(AType(), 3), u.BWD)
 
 These types are automatically resolved by iterating over the parameter:
 
->>> param = ucdp.Param(BType(), "param_p")
+>>> param = u.Param(BType(), "param_p")
 >>> for item in param:
 ...     print(repr(item))
 Param(BType(), 'param_p')
-Param(AType(), 'param_foo_p', level=1)
-Param(BitType(), 'param_foo_req_p', level=2)
-Param(UintType(16), 'param_foo_data_p', level=2, dims=(Slice('0:4'),))
-Param(BitType(), 'param_foo_ack_p', level=2)
-Param(BitType(), 'param_foo_error_p', level=2)
-Param(MType(), 'param_mode_p', level=1)
-Param(AType(), 'param_bar_p', level=1, dims=(Slice('0:2'),))
-Param(BitType(), 'param_bar_req_p', level=2, dims=(Slice('0:2'),))
-Param(UintType(16), 'param_bar_data_p', level=2, dims=(Slice('0:2'), Slice('0:4')))
-Param(BitType(), 'param_bar_ack_p', level=2, dims=(Slice('0:2'),))
-Param(BitType(), 'param_bar_error_p', level=2, dims=(Slice('0:2'),))
+Param(AType(), 'param_foo_p')
+Param(BitType(), 'param_foo_req_p')
+Param(ArrayType(UintType(16), 5), 'param_foo_data_p')
+Param(BitType(), 'param_foo_ack_p')
+Param(MType(), 'param_mode_p')
+Param(ArrayType(AType(), 3), 'param_bar_p')
+Param(ArrayType(BitType(), 3), 'param_bar_ack_p')
+Param(ArrayType(ArrayType(UintType(16), 5), 3), 'param_bar_data_p')
+Param(ArrayType(BitType(), 3), 'param_bar_req_p')
 """
 
-from typing import Iterator, Tuple
+from collections.abc import Iterator
+from typing import Any
 
-from .attrs import field, frozen
-from .ident import Ident
+from .ident import Ident, _iters
 
 
-@frozen(cmp=False, hash=True)
 class Param(Ident):
     """
     Module Parameter.
 
     Args:
         type_ (AType): Type.
         name (Name()): Name.
 
     Keyword Args:
         doc (Doc): Documentation Container
         value: Value.
 
     Parameter names should end with '_p', but must not.
 
-    >>> import ucdp
-    >>> cnt = ucdp.Param(ucdp.UintType(6), "cnt_p")
+    >>> import ucdp as u
+    >>> cnt = u.Param(u.UintType(6), "cnt_p")
     >>> cnt
     Param(UintType(6), 'cnt_p')
     >>> cnt.type_
     UintType(6)
     >>> cnt.name
     'cnt_p'
     >>> cnt.basename
@@ -104,45 +100,34 @@
     '_p'
     >>> cnt.doc
     Doc()
     >>> cnt.value
 
     If the parameter is casted via `int()` it returns `value` if set, other `type_.default`.
 
-    >>> int(ucdp.Param(ucdp.UintType(6, default=2), "cnt_p"))
+    >>> int(u.Param(u.UintType(6, default=2), "cnt_p"))
     2
-    >>> int(ucdp.Param(ucdp.UintType(6, default=2), "cnt_p", value=4))
+    >>> int(u.Param(u.UintType(6, default=2), "cnt_p", value=4))
     4
 
     Parameter are Singleton:
 
-    >>> ucdp.Param(ucdp.UintType(6), "cnt_p") is ucdp.Param(ucdp.UintType(6), "cnt_p")
+    >>> u.Param(u.UintType(6), "cnt_p") is u.Param(u.UintType(6), "cnt_p")
     True
     """
 
-    _suffixes: Tuple[str, ...] = ("_p",)
-
-    value = field(default=None, kw_only=True)
-
-    @value.validator
-    def _value_validator(self, attribute, value):
-        # pylint: disable=unused-argument
-        if value is not None:
-            self.type_.check(value)
+    value: Any = None
 
     def __int__(self):
         value = self.value
         if value is None:
             value = self.type_.default
         return int(value or 0)
 
-    def iter(self, filter_=None, stop=None, maxlevel=None, value=None) -> Iterator:
-        """Iterate over Parameter Hierarchy."""
-        # if value is None:
-        #     value = self.value
-        return super().iter(filter_=filter_, stop=stop, maxlevel=maxlevel, value=value)
-
-    def get(self, name, value=None) -> Iterator:
-        """Get a specific member in the Parameter Hierarchy."""
-        # if value is None:
-        #     value = self.value
-        return super().get(name, value=value)
+    def __iter__(self):
+        return _iters([self], value=self.value)
+
+    def iter(self, filter_=None, stop=None, value=None) -> Iterator:
+        """Iterate over Hierarchy."""
+        if value is None:
+            value = self.value
+        return _iters([self], filter_=filter_, stop=stop, value=value)
```

### Comparing `ucdp-0.1.0/ucdp/signal.py` & `ucdp-0.2.0/src/ucdp/signal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,203 +20,203 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """
 Signal and Port Handling.
 
-A :any:`Signal` is a module internal signal.
-A :any:`Port` is a module interface signal with a direction IN, OUT or INOUT.
+A [Signal][ucdp.signal.Signal] is a module internal signal.
+A [Port][ucdp.signal.Port] is a module interface signal with a direction IN, OUT or INOUT.
 
-Usage:
+??? Example "Simple Types"
+    Usage:
+
+        >>> from tabulate import tabulate
+        >>> import ucdp as u
+        >>> u.Signal(u.UintType(6), "sig_s")
+        Signal(UintType(6), 'sig_s')
+
+        >>> u.Port(u.UintType(6), "port_i")
+        Port(UintType(6), 'port_i', direction=IN)
+        >>> u.Port(u.UintType(6), "port_o")
+        Port(UintType(6), 'port_o', direction=OUT)
+
+??? Example "Complex Types"
+    Also complex types can simply be used:
+
+        >>> class AType(u.AStructType):
+        ...     def _build(self) -> None:
+        ...         self._add("req", u.BitType())
+        ...         self._add("data", u.ArrayType(u.UintType(16), 5))
+        ...         self._add("ack", u.BitType(), u.BWD)
+        >>> class MType(u.AEnumType):
+        ...     keytype: u.AScalarType = u.UintType(2)
+        ...     def _build(self) -> None:
+        ...         self._add(0, "Linear")
+        ...         self._add(1, "Cyclic")
+        >>> class BType(u.AStructType):
+        ...     def _build(self) -> None:
+        ...         self._add("foo", AType())
+        ...         self._add("mode", MType())
+        ...         self._add("bar", u.ArrayType(AType(), 3), u.BWD)
+
+
+??? Example "Resolving Types"
+    These types are automatically resolved by iterating over the port:
+
+        >>> sig = u.Signal(BType(), "sig_s")
+        >>> for item in sig:
+        ...     print(repr(item))
+        Signal(BType(), 'sig_s')
+        Signal(AType(), 'sig_foo_s')
+        Signal(BitType(), 'sig_foo_req_s')
+        Signal(ArrayType(UintType(16), 5), 'sig_foo_data_s')
+        Signal(BitType(), 'sig_foo_ack_s', direction=BWD)
+        Signal(MType(), 'sig_mode_s')
+        Signal(ArrayType(AType(), 3), 'sig_bar_s', direction=BWD)
+        Signal(ArrayType(BitType(), 3), 'sig_bar_ack_s')
+        Signal(ArrayType(ArrayType(UintType(16), 5), 3), 'sig_bar_data_s', direction=BWD)
+        Signal(ArrayType(BitType(), 3), 'sig_bar_req_s', direction=BWD)
+
+        >>> inp = u.Port(BType(), "inp_i")
+        >>> for item in inp:
+        ...     print(repr(item))
+        Port(BType(), 'inp_i', direction=IN)
+        Port(AType(), 'inp_foo_i', direction=IN)
+        Port(BitType(), 'inp_foo_req_i', direction=IN)
+        Port(ArrayType(UintType(16), 5), 'inp_foo_data_i', direction=IN)
+        Port(BitType(), 'inp_foo_ack_o', direction=OUT)
+        Port(MType(), 'inp_mode_i', direction=IN)
+        Port(ArrayType(AType(), 3), 'inp_bar_o', direction=OUT)
+        Port(ArrayType(BitType(), 3), 'inp_bar_ack_i', direction=IN)
+        Port(ArrayType(ArrayType(UintType(16), 5), 3), 'inp_bar_data_o', direction=OUT)
+        Port(ArrayType(BitType(), 3), 'inp_bar_req_o', direction=OUT)
 
->>> from tabulate import tabulate
->>> import ucdp
->>> ucdp.Signal(ucdp.UintType(6), "sig_s")
-Signal(UintType(6), 'sig_s')
-
->>> ucdp.Port(ucdp.UintType(6), "port_i")
-Port(UintType(6), name='port_i')
->>> ucdp.Port(ucdp.UintType(6), "port_o")
-Port(UintType(6), name='port_o')
-
-Also complex types can simply be used:
-
->>> class AType(ucdp.AStructType):
-...     def _build(self):
-...         self._add("req", ucdp.BitType())
-...         self._add("data", ucdp.ArrayType(ucdp.UintType(16), 5))
-...         self._add("ack", ucdp.BitType(), ucdp.BWD)
-...         self._add("error", ucdp.BitType(), ucdp.BIDIR)
->>> class MType(ucdp.AEnumType):
-...     keytype = ucdp.UintType(2)
-...     def _build(self):
-...         self._add(0, "Linear")
-...         self._add(1, "Cyclic")
->>> class BType(ucdp.AStructType):
-...     def _build(self):
-...         self._add("foo", AType())
-...         self._add("mode", MType())
-...         self._add("bar", ucdp.ArrayType(AType(), 3), ucdp.BWD)
-
-These types are automatically resolved by iterating over the port:
-
->>> sig = ucdp.Signal(BType(), "sig_s")
->>> for item in sig:
-...     print(repr(item))
-Signal(BType(), 'sig_s')
-Signal(AType(), 'sig_foo_s', level=1)
-Signal(BitType(), 'sig_foo_req_s', level=2)
-Signal(UintType(16), 'sig_foo_data_s', level=2, dims=(Slice('0:4'),))
-Signal(BitType(), 'sig_foo_ack_s', level=2, direction=BWD)
-Signal(BitType(), 'sig_foo_error_s', level=2, direction=BIDIR)
-Signal(MType(), 'sig_mode_s', level=1)
-Signal(AType(), 'sig_bar_s', level=1, direction=BWD, dims=(Slice('0:2'),))
-Signal(BitType(), 'sig_bar_req_s', level=2, direction=BWD, dims=(Slice('0:2'),))
-Signal(UintType(16), 'sig_bar_data_s', level=2, direction=BWD, dims=(Slice('0:2'), Slice('0:4')))
-Signal(BitType(), 'sig_bar_ack_s', level=2, dims=(Slice('0:2'),))
-Signal(BitType(), 'sig_bar_error_s', level=2, direction=BIDIR, dims=(Slice('0:2'),))
-
->>> inp = ucdp.Port(BType(), "inp_i")
->>> for item in inp:
-...     print(repr(item))
-Port(BType(), name='inp_i')
-Port(AType(), name='inp_foo_i', level=1)
-Port(BitType(), name='inp_foo_req_i', level=2)
-Port(UintType(16), name='inp_foo_data_i', level=2, dims=(Slice('0:4'),))
-Port(BitType(), name='inp_foo_ack_o', level=2)
-Port(BitType(), name='inp_foo_error_io', level=2)
-Port(MType(), name='inp_mode_i', level=1)
-Port(AType(), name='inp_bar_o', level=1, dims=(Slice('0:2'),))
-Port(BitType(), name='inp_bar_req_o', level=2, dims=(Slice('0:2'),))
-Port(UintType(16), name='inp_bar_data_o', level=2, dims=(Slice('0:2'), Slice('0:4')))
-Port(BitType(), name='inp_bar_ack_i', level=2, dims=(Slice('0:2'),))
-Port(BitType(), name='inp_bar_error_io', level=2, dims=(Slice('0:2'),))
 """
-from typing import Any, Optional, Tuple
 
-from .attrs import field, frozen
-from .doc import Doc
 from .ident import Ident
-from .nameutil import split_suffix
-from .types.orientation import FWD, IN, AOrientation, Direction, convert_aorientation, convert_direction
+from .orientation import FWD, AOrientation, Direction
+from .typebase import BaseType
 
 
-@frozen(cmp=False, hash=True)
-class ASignal(Ident):
+class BaseSignal(Ident):
+    """Base Class for All Signals ([Port][ucdp.signal.Port], [Signal][ucdp.signal.Signal]).
 
-    """Base Class for All Signals (:any:`Port`, :any:`Signal`)."""
+    Args:
+        type_: Type.
+        name: Name.
 
-    # Direction is always forward
-    direction: AOrientation = field(default=FWD, converter=convert_aorientation, kw_only=True)
-    dims: Tuple[Any, ...] = field(default=tuple(), kw_only=True)
-    doc: Doc = field(default=Doc(), kw_only=True)
+    Attributes:
+        direction: Direction.
+        doc: Documentation Container
+        ifdef: IFDEF encapsulation
 
+    ???+ bug "Todo"
+        * fix inherited_members / Attributes Types
+    """
 
-@frozen(cmp=False, hash=True)
-class Signal(ASignal):
+    direction: AOrientation = FWD
 
+
+class Signal(BaseSignal):
     """
     Module Internal Signal.
 
     Args:
-        type_ (AbstractType): Type.
-        name (Name()): Name.
+        type_: Type.
+        name: Name.
 
-    >>> import ucdp
-    >>> count = ucdp.Signal(ucdp.UintType(6), "count_s")
-    >>> count
-    Signal(UintType(6), 'count_s')
-    >>> count.type_
-    UintType(6)
-    >>> count.name
-    'count_s'
-    >>> count.basename
-    'count'
-    >>> count.suffix
-    '_s'
+    Attributes:
+        direction: Direction.
+        doc: Documentation Container
+        ifdef: IFDEF encapsulation
+
+    ???+ bug "Todo"
+        * fix inherited_members / Attributes Types
+
+    ??? Example "Signal Examples"
+        Examples.
+
+            >>> import ucdp as u
+            >>> count = u.Signal(u.UintType(6), "count_s")
+            >>> count
+            Signal(UintType(6), 'count_s')
+            >>> count.type_
+            UintType(6)
+            >>> count.name
+            'count_s'
+            >>> count.basename
+            'count'
+            >>> count.suffix
+            '_s'
+            >>> count.direction
+            FWD
+            >>> count.ifdef
 
-    Signal names should end with '_r' or '_s', but must not.
+    Note:
+        Signal names should end with '_r' or '_s', but must not.
     """
 
-    _suffixes: Tuple[str, ...] = ("_r", "_s")
-
+    def __init__(self, type_: BaseType, name: str, **kwargs):
+        kwargs.setdefault("direction", FWD)
+        super().__init__(type_=type_, name=name, **kwargs)  # type: ignore[call-arg]
 
-@frozen(cmp=False, hash=True)
-class Port(ASignal):
 
+class Port(BaseSignal):
     """
     Module Port.
 
     Args:
-        type_ (AbstractType): Type.
+        type_: Type.
+        name: Name.
 
-    Keyword Args:
-        name (Name()): Name. Default is None.
-        direction (Direction): Signal Direction. Automatically detected if `name` ends with '_i', '_o', '_io'.
-        title (str): Full Spoken Name.
-        descr (str): Documentation Description.
-        comment (str): Source Code Comment.
-        ifdef (str): Encapsulate port with ifdef.
-
-    >>> import ucdp
-    >>> count = ucdp.Port(ucdp.UintType(6), "count_i")
-    >>> count
-    Port(UintType(6), name='count_i')
-    >>> count.type_
-    UintType(6)
-    >>> count.name
-    'count_i'
-    >>> count.direction
-    IN
-    >>> count.basename
-    'count'
-    >>> count.suffix
-    '_i'
-
-    The port direction is automatically determined from the name or needs to be specified explicitly:
-
-    >>> ucdp.Port(ucdp.UintType(6)).direction
-    IN
-    >>> ucdp.Port(ucdp.UintType(6), "count_i").direction
-    IN
-    >>> ucdp.Port(ucdp.UintType(6), "count_o").direction
-    OUT
-    >>> ucdp.Port(ucdp.UintType(6), "count_io").direction
-    INOUT
-    >>> ucdp.Port(ucdp.UintType(6), "count").direction
-    Traceback (most recent call last):
-      ...
-    ValueError: 'direction' is required (could not be retrieved from name 'count').
-    >>> ucdp.Port(ucdp.UintType(6), "count", direction=ucdp.OUT).direction
-    OUT
+    Attributes:
+        direction: Direction.
+        doc: Documentation Container
+        ifdef: IFDEF encapsulation
+
+    ???+ bug "Todo"
+        * fix inherited_members / Attributes Types
+
+    ??? Example "Port Examples"
+        Examples.
+
+            >>> import ucdp as u
+            >>> count = u.Port(u.UintType(6), "count_i")
+            >>> count
+            Port(UintType(6), 'count_i', direction=IN)
+            >>> count.type_
+            UintType(6)
+            >>> count.name
+            'count_i'
+            >>> count.basename
+            'count'
+            >>> count.suffix
+            '_i'
+            >>> count.ifdef
+
+    ??? Example "Direction"
+        The port direction is automatically determined from the name or needs to be specified explicitly:
+
+            >>> u.Port(u.UintType(6), "count_i").direction
+            IN
+            >>> u.Port(u.UintType(6), "count_o").direction
+            OUT
+            >>> u.Port(u.UintType(6), "count_io").direction
+            INOUT
+            >>> u.Port(u.UintType(6), "count").direction
+            Traceback (most recent call last):
+            ...
+            ValueError: 'direction' is required (could not be retrieved from name 'count').
+            >>> u.Port(u.UintType(6), "count", direction=u.OUT).direction
+            OUT
     """
 
-    # pylint: disable=too-many-instance-attributes
+    direction: Direction
+    _posargs: tuple[str, ...] = ("type_", "name")
 
-    name: str = field(default="")
-    basename: str = field(init=False)
-    suffix: str = field(init=False)
-    direction: Direction = field(converter=convert_direction, kw_only=True)
-    level: int = field(default=0, kw_only=True)
-    dims: Tuple[Any, ...] = field(default=tuple(), kw_only=True)
-    doc: Doc = field(default=Doc(), kw_only=True)
-    ifdef: Optional[str] = field(default=None, kw_only=True)
-
-    _suffixes = ("_i", "_o", "_io")
-
-    @basename.default
-    def _basename_default(self) -> str:
-        return split_suffix(self.name, suffixes=self._suffixes)[0]
-
-    @suffix.default
-    def _suffix_default(self) -> str:
-        return split_suffix(self.name, suffixes=self._suffixes)[1]
-
-    @direction.default
-    def _direction_default(self):
-        if self.name:
-            direction = Direction.from_name(self.name)
+    def __init__(self, type_: BaseType, name: str, **kwargs):
+        if "direction" not in kwargs:
+            kwargs["direction"] = direction = Direction.from_name(name)
             if direction is None:
-                raise ValueError(f"'direction' is required (could not be retrieved from name {self.name!r}).")
-            return direction
-        return IN
+                raise ValueError(f"'direction' is required (could not be retrieved from name {name!r}).")
+        super().__init__(type_=type_, name=name, **kwargs)  # type: ignore[call-arg]
```

### Comparing `ucdp-0.1.0/ucdp/test.py` & `ucdp-0.2.0/src/ucdp/examples/simple/glbl/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,21 +17,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-
-"""Test."""
-from .attrs import field, frozen
-
-
-@frozen
-class Test:
-
-    """Test."""
-
-    # pylint: disable=too-few-public-methods
-
-    name: str = field()
-    options: dict = field(factory=dict)
+"""Example: Global Library."""
```

### Comparing `ucdp-0.1.0/ucdp/topref.py` & `ucdp-0.2.0/src/ucdp/modtopref.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,102 +18,85 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
-"""Top Module Reference."""
+"""Top Reference."""
 
 import re
-from typing import Optional
+from typing import Union
 
-from .attrs import field, frozen
 from .modref import ModRef
-from .util import opt
+from .object import Field, LightObject
 
+RE_TOPMODREF = re.compile(
+    # [tb]#
+    r"((?P<tb>[a-zA-Z_0-9_\.]+)#)?"
+    # top
+    r"(?P<top>[a-zA-Z_0-9_\.]+)"
+    # [-sub]
+    r"(-(?P<sub>[a-zA-Z_0-9_\.]+))?"
+)
+PAT_TOPMODREF = "[tb_lib.tb#]top_lib.top[-sub_lib.sub]"
+RE_MODREF = r"[a-zA-Z][a-zA-Z_0-9]*\.[a-zA-Z][a-zA-Z_0-9]*"
 
-@frozen
-class TopRef:
 
+class TopModRef(LightObject):
     """
     Top Module Reference.
 
     Args:
-        top (str): Name of the top module.
+        top: Top Module Reference
 
     Keyword Args:
-        sub (str): Name of the sub module within top module.
-        tb (str): Name of the testbench.
-    """
+        sub: Sub Module Reference
+        tb: Testbench Module Reference
 
-    top: ModRef = field(converter=ModRef.convert)
-    sub: Optional[ModRef] = field(converter=opt(ModRef.convert), default=None)
-    tb: Optional[ModRef] = field(converter=opt(ModRef.convert), default=None)
-
-    _re = re.compile(
-        # [tb]#
-        r"((?P<tb>[^#\- ]+)#)?"
-        # top
-        r"(?P<top>[^#\- ]+)"
-        # [-sub]
-        r"(-(?P<sub>[^#\- ]+))?"
-    )
-    _pat = "[tb#]top[-sub]"
+    >>> import ucdp as u
+    >>> u.TopModRef.cast('top_lib.top_mod')
+    TopModRef(ModRef('top_lib', 'top_mod'))
+    >>> u.TopModRef.cast('top_lib.top_mod-sub_lib.sub_mod')
+    TopModRef(ModRef('top_lib', 'top_mod'), sub='sub_lib.sub_mod')
+    >>> u.TopModRef.cast('mod_tb_lib.mod_tb#top_lib.top_mod')
+    TopModRef(ModRef('top_lib', 'top_mod'), tb=ModRef('mod_tb_lib', 'mod_tb'))
+
+    Invalid Pattern:
+
+    >>> TopModRef.cast('lib.mod:c-ls.1')
+    Traceback (most recent call last):
+    ..
+    ValueError: 'lib.mod:c-ls.1' does not match pattern '[tb_lib.tb#]top_lib.top[-sub_lib.sub]'
+    """
 
-    @staticmethod
-    def convert(value) -> "TopRef":
-        """
-        Create :any:`TopRef` from string `value`.
-
-        Just a top module:
-
-        >>> topref = TopRef.convert("chip")
-        >>> topref
-        TopRef(ModRef('chip'))
-        >>> str(topref)
-        'chip'
-
-        Top Module with Testbench:
-
-        >>> topref = TopRef.convert("tb#chip")
-        >>> topref
-        TopRef(ModRef('chip'), tb=ModRef('tb'))
-        >>> str(topref)
-        'tb#chip'
-
-        # Top Module with Testbench and Sub:
-
-        >>> topref = TopRef.convert("tb#chip-sub")
-        >>> topref
-        TopRef(ModRef('chip'), sub=ModRef('sub'), tb=ModRef('tb'))
-        >>> str(topref)
-        'tb#chip-sub'
-
-        A :any:`ModRef` is kept:
-
-        >>> TopRef.convert(TopRef(ModRef('chip')))
-        TopRef(ModRef('chip'))
-
-        Invalid Pattern:
-
-        >>> TopRef.convert('mo#d#e')
-        Traceback (most recent call last):
-        ..
-        ValueError: 'mo#d#e' does not match pattern '[tb#]top[-sub]'
-        """
-        if isinstance(value, TopRef):
-            return value
+    top: ModRef
+    sub: str | None = Field(default=None, pattern=RE_MODREF)
+    tb: ModRef | None = None
 
-        mat = TopRef._re.fullmatch(value)
-        if mat:
-            return TopRef(**mat.groupdict())
+    _posargs: tuple[str, ...] = ("top",)
 
-        raise ValueError(f"{value!r} does not match pattern {TopRef._pat!r}")
+    def __init__(self, top: ModRef, sub: str | None = None, tb: ModRef | None = None):
+        super().__init__(top=top, sub=sub, tb=tb)  # type: ignore[call-arg]
 
-    def __str__(self):
+    def __str__(self) -> str:
         result = str(self.top)
         if self.sub:
             result = f"{result}-{self.sub}"
         if self.tb:
             result = f"{self.tb}#{result}"
         return result
+
+    @staticmethod
+    def cast(value: Union["TopModRef", str]) -> "TopModRef":
+        """Cast `value` to `TopModRef`."""
+        if isinstance(value, TopModRef):
+            return value
+
+        mat = RE_TOPMODREF.fullmatch(value)
+        if mat:
+            top = ModRef.cast(mat.group("top"))
+            sub = mat.group("sub")
+            tb = ModRef.cast(mat.group("tb")) if mat.group("tb") else None
+            return TopModRef(top=top, sub=sub, tb=tb)
+
+        raise ValueError(f"{value!r} does not match pattern {PAT_TOPMODREF!r}")
```

### Comparing `ucdp-0.1.0/ucdp/types/__init__.py` & `ucdp-0.2.0/src/ucdp/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,10 +18,34 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
-"""
-Type Engine.
-"""
+"""Exceptions."""
+
+from typing import Any
+
+
+class LockError(ValueError):
+    """Lock."""
+
+    def __init__(self, inst: Any):
+        msg = f"{inst!r} is already locked for modification."
+        super().__init__(msg)
+
+
+class DuplicateError(ValueError):
+    """Duplicate Error."""
+
+
+class InvalidExpr(TypeError):
+    """Invalid Expression."""
+
+
+class DirectionError(ValueError):
+    """Signal Direction Error."""
+
+
+class BuildError(RuntimeError):
+    """Cannot Build Module."""
```

### Comparing `ucdp-0.1.0/ucdp/types/array.py` & `ucdp-0.2.0/src/ucdp/typearray.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,91 +21,95 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 """
 Array Type.
 """
-from icdutil.slices import UP, Slice
 
-from ..attrs import ReusedFrozen, field, frozen
-from .base import ACompositeType, AType
+from typing import Any
 
+from .object import Light
+from .slices import UP, Slice
+from .typebase import ACompositeType, BaseType
 
-@frozen
-class ArrayType(ACompositeType, ReusedFrozen):
 
+class ArrayType(ACompositeType, Light):
     """
-    Array of `type_`.
+    Array of `itemtype`.
 
     Args:
-        type_ (AType): Element Type.
+        itemtype (AType): Element Type.
         depth (int):    depth.
 
     Example:
-
-    >>> import ucdp
-    >>> mem = ucdp.ArrayType(ucdp.UintType(16), 10)
+    >>> import ucdp as u
+    >>> mem = u.ArrayType(u.UintType(16), 10)
     >>> mem
     ArrayType(UintType(16), 10)
 
     Arrays can be nested and combined with all other types.
 
-    >>> class BusType(ucdp.AStructType):
-    ...     def _build(self):
-    ...         self._add('data', ucdp.UintType(8))
-    ...         self._add('valid', ucdp.BitType())
-    ...         self._add('accept', ucdp.BitType(), orientation=ucdp.BWD)
+    >>> class BusType(u.AStructType):
+    ...     def _build(self) -> None:
+    ...         self._add('data', u.UintType(8))
+    ...         self._add('valid', u.BitType())
+    ...         self._add('accept', u.BitType(), orientation=u.BWD)
 
-    >>> structmatrix = ucdp.ArrayType(ucdp.ArrayType(BusType(), 10), 22)
+    >>> structmatrix = u.ArrayType(u.ArrayType(BusType(), 10), 22)
     >>> structmatrix
     ArrayType(ArrayType(BusType(), 10), 22)
 
-    Systemverilog Declaration:
-
     Slicing:
 
+    >>> structmatrix.slice_
+    Slice('0:21')
     >>> structmatrix[0:15]
     ArrayType(ArrayType(BusType(), 10), 16)
     >>> structmatrix[3]
     ArrayType(BusType(), 10)
     >>> structmatrix[3][3]
     BusType()
     """
 
-    type_: AType = field()
-    depth: int = field()
-    left: int = field(default=0)
+    itemtype: BaseType
+    depth: Any
+    left: Any = 0
+
+    _posargs: tuple[str, ...] = ("itemtype", "depth")
 
-    _yield = False  # Do not yield on iterations
+    def __init__(self, itemtype: BaseType, depth: Any, left=0):
+        super().__init__(itemtype=itemtype, depth=depth, left=left)  # type: ignore[call-arg]
 
     @property
     def slice_(self):
-        """Get Slice of Matrix"""
+        """Get Slice of Matrix."""
         return Slice(left=self.left, right=self.depth - 1)
 
-    def is_connectable(self, other):
+    def is_connectable(self, other) -> bool:
         """
         Check For Valid Connection To `other`.
 
         Connections are only allowed to other :any:`ArrayType` of the same depth and type.
 
         >>> from ucdp import ArrayType, UintType, SintType
         >>> ArrayType(UintType(8), 8).is_connectable(ArrayType(UintType(8), 8))
         True
         >>> ArrayType(UintType(8), 8).is_connectable(ArrayType(UintType(8), 9))
         False
         >>> ArrayType(UintType(8), 8).is_connectable(ArrayType(SintType(8), 8))
         False
         """
-        return isinstance(other, ArrayType) and self.depth == other.depth and self.type_.is_connectable(other.type_)
+        return (
+            isinstance(other, ArrayType) and self.depth == other.depth and self.itemtype.is_connectable(other.itemtype)
+        )
 
     def __getitem__(self, slice_):
         slice_ = Slice.cast(slice_, direction=UP)
         if slice_.width == 1:
-            return self.type_
-        return ArrayType(self.type_, slice_.width, left=slice_.left)
+            return self.itemtype
+        return ArrayType(self.itemtype, slice_.width, left=slice_.left)
 
     @property
     def bits(self):
         """Size in Bits."""
-        return self.depth * self.type_.bits
+        return self.depth * self.itemtype.bits
```

### Comparing `ucdp-0.1.0/ucdp/types/base.py` & `ucdp-0.2.0/src/ucdp/typebase.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,211 +20,175 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 """
 Basic Types.
-"""
 
-from typing import Any, Optional
+DOCME
+
+* :any:`Type` - Base Class for all Types
+* :any:`AScalarType` - Base Class for all Single Value Types
+* :any:`VecType` - Base Class for all vector-mapped Scalars.
+* :any:`CompositeType` - Base class for all assembling Types.
+"""
 
-from icdutil.slices import DOWN, Slice
+from abc import abstractmethod
+from typing import Any
 
-from ..attrs import ReusedFrozen, evolve, field, frozen
+from pydantic import model_validator
 
-tailoredtype = frozen
+from .doc import Doc
+from .object import Light, Object
+from .slices import DOWN, Slice
 
 
-@frozen
-class AType:
+class BaseType(Object):
     """
     Base Class for all Types.
+    """
 
+    title: str | None = None
+    descr: str | None = None
+    comment: str | None = None
 
-    Documentation defaults are empty by default:
+    @property
+    def doc(self) -> Doc:
+        """Documentation."""
+        return Doc(title=self.title, descr=self.descr, comment=self.comment)
 
-    >>> import ucdp
-    >>> ucdp.AType.title
-    >>> ucdp.AType.descr
-    >>> ucdp.AType.comment
-    """
-
-    # Defaults
-    title: Optional[str] = None
-    descr: Optional[str] = None
-    comment: Optional[str] = None
-    width: Optional[Any] = None
-    min_: Optional[Any] = None
-    max_: Optional[Any] = None
-
-    _dynamic = False
-    _yield = True
-
-    def new(self, **kwargs) -> "AType":
-        """Return A Copy With Updated Attributes."""
-        return evolve(self, **kwargs)
+    def is_connectable(self, other: "BaseType"):
+        """
+        Check For Valid Connection To `other`.
+
+        This method has to be overwritten.
+        """
+        raise NotImplementedError
+
+    def cast(self, other: "BaseType"):
+        """
+        How to cast an input of type `self` from a value of type `other`.
+
+        `self = cast(other)`
+        """
+        return NotImplemented
+
+    @property
+    def bits(self):
+        """
+        Size in Bits.
+
+        This method has to be overwritten.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def __getitem__(self, slice_):
+        """
+        Return Sliced Variant.
+        """
+
+
+class BaseScalarType(BaseType):
+    """
+    Base Type For All Native Types.
+    """
+
+    default: Any | None = None
+
+
+class AScalarType(BaseScalarType, Light):
+    """
+    Abstract Type For All Native Types.
+    """
+
+    width: Any = 1
+
+    @model_validator(mode="after")
+    def __post_init(self) -> "AScalarType":
+        default = self.default
+        if default is not None:
+            self.check(default, what="default")
+        return self
 
     def check(self, value, what="Value"):
         """
         Check if `value` can be handled by type`.
 
-        >>> import ucdp
-        >>> atype = ucdp.AType()
+        >>> import ucdp as u
+        >>> atype = u.AScalarType()
         >>> atype.check(1)
         1
         """
-        # pylint: disable=unused-argument
         return value  # pragma: no cover
 
     def encode(self, value, usedefault=False):
         """
         Encode Value.
 
-        >>> import ucdp
-        >>> atype = ucdp.AType()
+        >>> import ucdp as u
+        >>> atype = u.AScalarType()
         >>> atype.encode(1)
         1
         """
-        # pylint: disable=unused-argument
         return int(value)
 
     def get_hex(self, value=None):
         """
         Return Hex Value.
 
-        >>> import ucdp
-        >>> ucdp.AType().get_hex()
+        >>> import ucdp as u
+        >>> u.AScalarType().get_hex()
         """
-        # pylint: disable=unused-argument
-        return None
+        return
 
     def __getitem__(self, slice_):
         """
         Return Sliced Variant.
 
-        >>> import ucdp
-        >>> ucdp.AType()[4]
+        >>> import ucdp as u
+        >>> u.AScalarType()[4]
         Traceback (most recent call last):
             ...
-        ValueError: Cannot slice (4) from AType()
+        ValueError: Cannot slice (4) from AScalarType()
         """
         slice_ = Slice.cast(slice_, direction=DOWN)
         raise ValueError(f"Cannot slice ({slice_}) from {self}")
 
-    @property
-    def bits(self):
-        """
-        Size in Bits.
-
-        This method has to be overwritten.
-        """
-        raise NotImplementedError()
-
-    def is_connectable(self, other):
-        """
-        Check For Valid Connection To `other`.
-
-        This method has to be overwritten.
-        """
-        raise NotImplementedError()
-
-    def cast(self, other):
-        """
-        How to cast an input of type `self` from a value of type `other`.
-
-        `self = cast(other)`
-        """
-        # pylint: disable=unused-argument
-        return NotImplemented
-
     def __contains__(self, item):
         try:
             if isinstance(item, range):
                 items = tuple(item)
                 self.check(self.encode(items[0]))
                 self.check(self.encode(items[-1]))
             else:
                 self.check(self.encode(item))
             return True
         except ValueError:
             return False
 
-
-@frozen
-class AScalarType(AType):
-
-    """
-    Base Type For All Native Types.
-
-    All subclasses will carry later-on the systemverilog construct 'logic' or 'wire'.
-    """
-
-    default: int = field(default=0, kw_only=True)
-    width = 1
-
-    @default.validator
-    def _default_validator(self, attribute, value):
-        # pylint: disable=unused-argument
-        self.check(value, what="default")
-
-    def is_connectable(self, other):
-        """
-        Check For Valid Connection To `other`.
-
-        This method has to be overwritten.
-        """
-        raise NotImplementedError()
-
     @property
     def bits(self):
         """Size in Bits."""
         return self.width
 
 
-@frozen
-class AVecType(AScalarType, ReusedFrozen):
-
+class AVecType(AScalarType):
     """Base Class for all Vector Types."""
 
-    width = field()
-    right = field(default=0, kw_only=True)
-    default = field(default=0, kw_only=True)
-
-    @width.validator
-    def _width_validator(self, attribute, value):
-        # pylint: disable=unused-argument
-        assert not isinstance(value, float)
-
-    @default.validator
-    def _default_validator(self, attribute, value):
-        # pylint: disable=unused-argument
-        self.check(value, what="default")
+    default: Any = 0
+    right: Any = 0
+
+    _posargs: tuple[str, ...] = ("width",)
+
+    def __init__(self, width, **kwargs):
+        super().__init__(width=width, **kwargs)
 
     @property
     def slice_(self):
         """Slice."""
         return Slice(left=self.right + self.width - 1, right=self.right)
 
-    def is_connectable(self, other):
-        """
-        Check For Valid Connection To `other`.
-
-        This method has to be overwritten.
-        """
-        raise NotImplementedError()
-
-    @property
-    def bits(self):
-        """Size in Bits."""
-        return self.width
-
-
-@frozen
-class ACompositeType(AType):
 
+class ACompositeType(BaseType):
     """Base Class For All Composite Types."""
-
-    @property
-    def bits(self):
-        """Size in Bits."""
-        raise NotImplementedError()
```

### Comparing `ucdp-0.1.0/ucdp/types/clkrst.py` & `ucdp-0.2.0/src/ucdp/typeclkrst.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -28,168 +28,169 @@
 * :any:`RstAType` - Asynchronous Reset (High-Active)
 * :any:`RstAnType` - Asynchronous Reset (Low-Active)
 * :any:`RstType` - Synchronous Reset (High-Active)
 * :any:`ClkRstAnType` - Clock and Async Reset Pair
 * :any:`DiffClkType` - Differential Clock
 * :any:`DiffClkRstAnType` - Differential Clock and Async Reset
 """
-from .enum import AEnumType
-from .scalar import BitType
-from .struct import AStructType
 
+from .typebase import AScalarType
+from .typeenum import AEnumType
+from .typescalar import BitType
+from .typestruct import AStructType
 
-class ClkType(BitType):
 
+class ClkType(BitType):
     """
     Clock Type.
 
     Single bit used as clock.
 
-    >>> clk = ClkType()
+    >>> import ucdp as u
+    >>> clk = u.ClkType()
     >>> clk
     ClkType()
     >>> clk.width
     1
     """
 
-    title = "Clock"
+    title: str = "Clock"
 
 
 class RstAType(AEnumType):
-
     """
     Async high-active Reset Type.
 
     Single bit used as asynchronous reset.
 
-    >>> rst = RstAType()
+    >>> import ucdp as u
+    >>> rst = u.RstAType()
     >>> rst
     RstAType()
     >>> rst.width
     1
     >>> for item in rst.values():
     ...     print(repr(item))
     EnumItem(0, 'inactive', doc=Doc(title='Reset not active'))
     EnumItem(1, 'active', doc=Doc(title='Reset active'))
     """
 
-    keytype = BitType()
-    title = "Async Reset"
-    descr = "High-Active"
-    comment = "Async Reset (High-Active)"
+    keytype: AScalarType = BitType()
+    title: str = "Async Reset"
+    descr: str = "High-Active"
+    comment: str = "Async Reset (High-Active)"
 
-    def _build(self):
+    def _build(self) -> None:
         self._add(0, "inactive", "Reset not active")
         self._add(1, "active", "Reset active")
 
 
 class RstAnType(AEnumType):
-
     """
     Async low-active Reset Type.
 
     Single bit used as asynchronous low-active reset.
 
-    >>> rst = RstAnType()
+    >>> import ucdp as u
+    >>> rst = u.RstAnType()
     >>> rst
     RstAnType()
     >>> rst.width
     1
     >>> for item in rst.values():
     ...     print(repr(item))
     EnumItem(0, 'active', doc=Doc(title='Reset active'))
     EnumItem(1, 'inactive', doc=Doc(title='Reset not active'))
     """
 
-    keytype = BitType()
-    title = "Async Reset"
-    descr = "Low-Active"
-    comment = "Async Reset (Low-Active)"
+    keytype: AScalarType = BitType()
+    title: str = "Async Reset"
+    descr: str = "Low-Active"
+    comment: str = "Async Reset (Low-Active)"
 
-    def _build(self):
+    def _build(self) -> None:
         self._add(0, "active", "Reset active")
         self._add(1, "inactive", "Reset not active")
 
 
 class RstType(AEnumType):
-
     """
     Sync Reset.
 
     Single bit used as synchronous reset.
 
-    >>> rst = RstType()
+    >>> import ucdp as u
+    >>> rst = u.RstType()
     >>> rst
     RstType()
     >>> rst.width
     1
     >>> for item in rst.values():
     ...     print(repr(item))
     EnumItem(0, 'inactive', doc=Doc(title='Reset not active'))
     EnumItem(1, 'active', doc=Doc(title='Reset active'))
     """
 
-    keytype = BitType()
-    title = "Synchronous Reset"
-    descr = "High-Active"
+    keytype: AScalarType = BitType()
+    title: str = "Synchronous Reset"
+    descr: str = "High-Active"
 
-    def _build(self):
+    def _build(self) -> None:
         self._add(0, "inactive", "Reset not active")
         self._add(1, "active", "Reset active")
 
 
 class ClkRstAnType(AStructType):
-
     """
     Clock, Async Reset Pair.
 
-    >>> clkrst = ClkRstAnType()
+    >>> import ucdp as u
+    >>> clkrst = u.ClkRstAnType()
     >>> for item in clkrst.values():
     ...     print(repr(item))
     StructItem('clk', ClkType(), doc=Doc(title='Clock'))
     StructItem('rst_an', RstAnType(), doc=Doc(title='Async Reset', descr='Low-Active', comment='Async Reset ...'))
     """
 
-    title = "Clock and Reset"
+    title: str = "Clock and Reset"
 
-    def _build(self):
+    def _build(self) -> None:
         self._add("clk", ClkType())
         self._add("rst_an", RstAnType())
 
 
 class DiffClkType(AStructType):
-
     """
     Differential Clock.
 
-    >>> diffclk = DiffClkType()
+    >>> import ucdp as u
+    >>> diffclk = u.DiffClkType()
     >>> for item in diffclk.values():
     ...     print(repr(item))
     StructItem('p', ClkType(), doc=Doc(title='Clock'))
     StructItem('n', ClkType(default=1), doc=Doc(title='Inverted Clock'))
     """
 
-    title = "Differential Clock"
+    title: str = "Differential Clock"
 
-    def _build(self):
+    def _build(self) -> None:
         self._add("p", ClkType(default=0))
-        title = "Inverted Clock"
-        self._add("n", ClkType(default=1), title=title, comment=title)
+        self._add("n", ClkType(default=1), title="Inverted Clock")
 
 
 class DiffClkRstAnType(AStructType):
-
     """
-    Differential Clock and Reset
+    Differential Clock and Reset.
 
-    >>> diffclkrst = DiffClkRstAnType()
+    >>> import ucdp as u
+    >>> diffclkrst = u.DiffClkRstAnType()
     >>> for item in diffclkrst.values():
     ...     print(repr(item))
     StructItem('clk', DiffClkType(), doc=Doc(title='Differential Clock'))
     StructItem('rst_an', RstAnType(), doc=Doc(title='Async Reset', descr='Low-Active', comment='Async Reset ...'))
     """
 
-    title = "Differential Clock and Reset"
+    title: str = "Differential Clock and Reset"
 
-    def _build(self):
+    def _build(self) -> None:
         self._add("clk", DiffClkType())
         self._add("rst_an", RstAnType())
```

### Comparing `ucdp-0.1.0/ucdp/types/descriptivestruct.py` & `ucdp-0.2.0/src/ucdp/typedescriptivestruct.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -22,152 +22,152 @@
 # SOFTWARE.
 #
 """
 Descriptive Struct Type.
 
 This module serves a struct type variant :any:`DescriptiveStructType` which describes a given `type_` with constants.
 """
-from caseconverter import snakecase
 
-from ..attrs import field, frozen
-from .array import ArrayType
-from .base import AType
-from .enum import BaseEnumType
+from .nameutil import str2identifier
 from .orientation import BWD, FWD
-from .scalar import BitType, IntegerType
-from .struct import AStructType, BaseStructType
+from .typearray import ArrayType
+from .typebase import BaseType
+from .typeenum import BaseEnumType
+from .typescalar import IntegerType, SintType, UintType
+from .typestruct import AStructType, BaseStructType, StructFilter
 
 
-@frozen
 class DescriptiveStructType(AStructType):
-
     """
     Struct with constants describing `type_`.
 
     Args:
-        type_(AType): Type to be described
+        type_(Type): Type to be described
 
     Bit:
 
-    >>> import ucdp
-    >>> for item in DescriptiveStructType(ucdp.BitType(default=1)).values():
+    >>> import ucdp as u
+    >>> for item in u.DescriptiveStructType(u.BitType(default=1)).values():
     ...     repr(item)
     "StructItem('default_p', BitType(default=1), doc=Doc(title='Default Value'))"
 
     Unsigned Integer:
 
-    >>> for item in DescriptiveStructType(ucdp.UintType(16, default=3),
-    ...                                   filter_=lambda item: item.name in ("default_p", "max_p")):
-    ...     repr(item)
-    "StructItem('max_p', UintType(16, default=65535), doc=Doc(title='Maximal Value'))"
-    "StructItem('default_p', UintType(16, default=3), doc=Doc(title='Default Value'))"
+    >>> for item in u.DescriptiveStructType(u.UintType(16, default=3),
+    ...                                   filter_=lambda item: item.name in ("default_p", "max_p")).values():
+    ...     item
+    StructItem('max_p', UintType(16, default=65535), doc=Doc(title='Maximal Value'))
+    StructItem('default_p', UintType(16, default=3), doc=Doc(title='Default Value'))
 
     Signed Integer:
 
-    >>> for item in DescriptiveStructType(ucdp.SintType(8, default=-3)).values():
+    >>> for item in u.DescriptiveStructType(u.SintType(8, default=-3)).values():
     ...     repr(item)
     "StructItem('width_p', IntegerType(default=8), doc=Doc(title='Width in Bits'))"
     "StructItem('min_p', SintType(8, default=-128), doc=Doc(title='Minimal Value'))"
     "StructItem('max_p', SintType(8, default=127), doc=Doc(title='Maximal Value'))"
     "StructItem('default_p', SintType(8, default=-3), doc=Doc(title='Default Value'))"
 
     Enum:
 
-    >>> class MyEnumType(ucdp.AEnumType):
-    ...     keytype = ucdp.UintType(2, default=0)
-    ...     def _build(self):
+    >>> class MyEnumType(u.AEnumType):
+    ...     keytype: u.AScalarType = u.UintType(2, default=0)
+    ...     def _build(self) -> None:
     ...         self._add(0, "Forward")
     ...         self._add(1, 8)
     ...         self._add(2, "Bi-Dir")
-    >>> for item in DescriptiveStructType(MyEnumType()).values():
+    >>> for item in u.DescriptiveStructType(MyEnumType()).values():
     ...     repr(item)
     "StructItem('width_p', IntegerType(default=2), doc=Doc(title='Width in Bits'))"
-    "StructItem('min_p', MyEnumType(), doc=Doc(title='Minimal Value'))"
+    "StructItem('min_p', MyEnumType(default=0), doc=Doc(title='Minimal Value'))"
     "StructItem('max_p', MyEnumType(default=3), doc=Doc(title='Maximal Value'))"
     "StructItem('forward_e', UintType(2))"
-    "StructItem('8_e', UintType(2, default=1))"
+    "StructItem('v8_e', UintType(2, default=1))"
     "StructItem('bi_dir_e', UintType(2, default=2))"
     "StructItem('default_p', MyEnumType(), doc=Doc(title='Default Value'))"
 
     Struct:
 
-    >>> class SubStructType(ucdp.AStructType):
-    ...     def _build(self):
-    ...         self._add('a', ucdp.UintType(2))
-    ...         self._add('b', ucdp.UintType(3), ucdp.BWD)
-    ...         self._add('c', ucdp.UintType(4), ucdp.BIDIR)
-    >>> class MyStructType(ucdp.AStructType):
-    ...     def _build(self):
-    ...         self._add('ctrl', ucdp.UintType(4), title='Control')
-    ...         self._add('data', ucdp.ArrayType(ucdp.SintType(16, default=5), 8), ucdp.FWD, descr='Data to be handled')
-    ...         self._add('resp', ucdp.BitType(), ucdp.BWD, comment='Sink response')
-    ...         self._add('mode', MyEnumType(), ucdp.BWD, comment='Enum')
-    ...         self._add('bi', ucdp.UintType(5), ucdp.BIDIR)
-    ...         self._add('sub', SubStructType(), ucdp.BWD)
-    >>> for item in DescriptiveStructType(MyStructType()).values():
+    >>> class SubStructType(u.AStructType):
+    ...     def _build(self) -> None:
+    ...         self._add('a', u.UintType(2))
+    ...         self._add('b', u.UintType(3), u.BWD)
+    >>> class MyStructType(u.AStructType):
+    ...     def _build(self) -> None:
+    ...         self._add('ctrl', u.UintType(4), title='Control')
+    ...         self._add('data', u.ArrayType(u.SintType(16, default=5), 8), u.FWD, descr='Data to be handled')
+    ...         self._add('resp', u.BitType(), u.BWD, comment='Sink response')
+    ...         self._add('mode', MyEnumType(), u.BWD, comment='Enum')
+    ...         self._add('sub', SubStructType(), u.BWD)
+    >>> for item in u.DescriptiveStructType(MyStructType()).values():
     ...     repr(item)
-    "StructItem('bits_p', IntegerType(default=149), doc=Doc(title='Size in Bits'))"
+    "StructItem('bits_p', IntegerType(default=140), doc=Doc(title='Size in Bits'))"
     "StructItem('fwdbits_p', IntegerType(default=135), doc=Doc(title='Forward Size in Bits'))"
     "StructItem('bwdbits_p', IntegerType(default=5), doc=Doc(title='Backward Size in Bits'))"
-    "StructItem('bibits_p', IntegerType(default=9), doc=Doc(title='Bi-Directional Size in Bits'))"
-
-    All this works for parameterized types too:
+    "StructItem('bibits_p', IntegerType(), doc=Doc(title='Bi-Directional Size in Bits'))"
 
-    >>> width_p = ucdp.Param(ucdp.IntegerType(default=16), 'width_p')
-    >>> type_ = ucdp.UintType(width_p, default=4)
-    >>> for item in DescriptiveStructType(type_).values():
-    ...     repr(item)
-    "StructItem('width_p', IntegerType(default=Param(IntegerType(default=16), 'width_p')), doc=...
-    "StructItem('min_p', UintType(Param(IntegerType(default=16), 'width_p')), doc=...
-    "StructItem('max_p', UintType(Param(IntegerType(default=16), 'width_p'), default=Op(Op(2, '**', Param(...
-    "StructItem('default_p', UintType(Param(IntegerType(default=16), 'width_p'), default=4), doc=...
     """
 
-    type_: AType = field()
-    enumitem_suffix: str = field(default="e")
+    # All this works for parameterized types too:
+
+    # >>> width_p = u.Param(u.IntegerType(default=16), 'width_p')
+    # >>> type_ = u.UintType(width_p, default=4)
+    # >>> for item in u.DescriptiveStructType(type_).values():
+    # ...     repr(item)
+    # "StructItem('width_p', IntegerType(default=Param(IntegerType(default=16), 'width_p')), doc=...
+    # "StructItem('min_p', UintType(Param(IntegerType(default=16), 'width_p')), doc=...
+    # "StructItem('max_p', UintType(Param(IntegerType(default=16), 'width_p'), default=Op(Op(2, '**', Param(...
+    # "StructItem('default_p', UintType(Param(IntegerType(default=16), 'width_p'), default=4), doc=...
+
+    type_: BaseType
+    enumitem_suffix: str = "e"
+    filter_: StructFilter | None = None
+
+    def __init__(self, type_: BaseType, **kwargs):
+        super().__init__(type_=type_, **kwargs)  # type: ignore[call-arg]
 
     def _build(self) -> None:
         self._add_type(self.type_)
 
-    def _add_type(self, type_: AType) -> None:
+    def _add_type(self, type_: BaseType) -> None:
         # Width
-        if not isinstance(type_, (BitType, IntegerType, ArrayType, BaseStructType)):
+        if isinstance(type_, (UintType, SintType, BaseEnumType)):
             title = "Width in Bits"
-            self._add("width_p", IntegerType(default=type_.width), title=title, descr=None, comment=title)
+            self._add("width_p", IntegerType(default=type_.width), title=title)
             title = "Minimal Value"
-            self._add("min_p", type_.new(default=type_.min_), title=title, descr=None, comment=title)
+            self._add("min_p", type_.new(default=type_.min_), title=title)
             title = "Maximal Value"
-            self._add("max_p", type_.new(default=type_.max_), title=title, descr=None, comment=title)
+            self._add("max_p", type_.new(default=type_.max_), title=title)
         if isinstance(type_, (ArrayType, BaseStructType)):
             title = "Size in Bits"
-            self._add("bits_p", IntegerType(default=type_.bits), title=title, descr=None, comment=title)
+            self._add("bits_p", IntegerType(default=type_.bits), title=title)
             fwdbits, bwdbits, bibits = _get_dirwith(type_)
             title = "Forward Size in Bits"
-            self._add("fwdbits_p", IntegerType(default=fwdbits), title=title, descr=None, comment=title)
+            self._add("fwdbits_p", IntegerType(default=fwdbits), title=title)
             title = "Backward Size in Bits"
-            self._add("bwdbits_p", IntegerType(default=bwdbits), title=title, descr=None, comment=title)
+            self._add("bwdbits_p", IntegerType(default=bwdbits), title=title)
             title = "Bi-Directional Size in Bits"
-            self._add("bibits_p", IntegerType(default=bibits), title=title, descr=None, comment=title)
+            self._add("bibits_p", IntegerType(default=bibits), title=title)
         # Enum Items
         if isinstance(type_, BaseEnumType):
             enumitem_suffix = self.enumitem_suffix
             for eitem in type_.values():
-                ename = snakecase(str(eitem.value))
+                ename = str2identifier(str(eitem.value))
                 etype = type_.keytype.new(default=eitem.key)
                 doc = eitem.doc
                 self._add(f"{ename}_{enumitem_suffix}", etype, title=doc.title, descr=doc.descr, comment=doc.comment)
         # Default
         if not isinstance(type_, (BaseStructType, ArrayType)):
             title = "Default Value"
-            self._add("default_p", type_, title=title, descr=None, comment=title)
+            self._add("default_p", type_, title=title)
 
 
 def _get_dirwith(type_, orientation=FWD):
     fwd, bwd, bid = 0, 0, 0
-    for item in type_:
+    for item in type_.values():
         itype_ = item.type_
         iorientation = item.orientation * orientation
         if isinstance(itype_, BaseStructType):
             ifwd, ibwd, ibid = _get_dirwith(itype_, iorientation)
             fwd += ifwd
             bwd += ibwd
             bid += ibid
```

### Comparing `ucdp-0.1.0/ucdp/types/enum.py` & `ucdp-0.2.0/src/ucdp/typeenum.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -30,126 +30,97 @@
 * :any:`AEnumType` - Standard Enumeration
 * :any:`AGlobalEnumType` - A public enumeration which fills up through all instances.
 * :any:`DynamicEnumType` - A public enumeration which fills up per instance.
 * :any:`EnaType` - Native single bit with `ena` and `dis` enumeration, active-high
 * :any:`DisType` - Native single bit with `ena` and `dis` enumeration, low-high
 """
 
-from typing import Any, Callable, Optional
+from abc import abstractmethod
+from collections.abc import Callable
+from typing import Any
 
 from humanfriendly.text import concatenate
+from pydantic import model_validator
 
-from ..attrs import NOTHING, ReusedFrozen, field, frozen
-from ..doc import Doc
-from ..nameutil import validate_name
-from ..util import AutoNum
-from .scalar import AType, BitType, IntegerType
+from .consts import AUTO
+from .dict import Dict
+from .doc import Doc
+from .exceptions import LockError
+from .object import Field, Light, Object, PrivateField
+from .typebase import BaseScalarType
+from .typescalar import AScalarType, BitType, IntegerType
 
-_ENUMNUM = AutoNum()
-AUTO = object()
-
-
-@frozen
-class EnumItem(ReusedFrozen):
 
+class EnumItem(Object):
     """
-    Enumeration Item.
+    Enumeration NamedObject.
 
     Args:
         key (int): key value to be mapped.
         value: Mapped value.
 
     Keyword Args:
         doc (Doc): Documentation Container
 
-    Enumeration items are typically created by :any:`AEnumType._add`.
+    Enumeration items are typically created by :any:`EnumType._add`.
     """
 
-    key: int = field()
-    value = field()
-    doc: Doc = field(default=Doc())
+    key: int
+    value: Any
+    doc: Doc = Doc()
 
-    @property
-    def title(self):
-        """Alias to `doc.title`."""
-        return self.doc.title
+    _posargs: tuple[str, ...] = ("key", "value")
 
-    @property
-    def descr(self):
-        """Alias to `doc.descr`."""
-        return self.doc.descr
-
-    @property
-    def comment(self):
-        """Alias to `doc.comment`."""
-        return self.doc.comment
+    def __init__(self, key, value, **kwargs):
+        super().__init__(key=key, value=value, **kwargs)
 
 
 ItemFilter = Callable[[EnumItem], bool]
 
 
-@frozen
-class BaseEnumType(AType, dict):
-
+class BaseEnumType(BaseScalarType, Dict):
     """Base Type for all Enums."""
 
-    keytype: Any = IntegerType()
+    keytype: AScalarType = IntegerType()
     valuetype: Any = None
-    default: Any = field(kw_only=True)
-    filter_: ItemFilter = field(default=None, kw_only=True, repr=False)
-    _locked: bool = False
-
-    @default.default
-    def _default_default(self):
-        return self.keytype.default
-
-    @default.validator
-    def _default_validator(self, attribute, value):
-        # pylint: disable=unused-argument
-        self.check(value, what="default")
+    default: Any = None
+    filter_: ItemFilter | None = Field(default=None, repr=False)
+    _locked: bool = PrivateField(default=False)
 
-    def __attrs_post_init__(self):
-        self._build()
-
-    def _build(self) -> None:
-        """Build Type."""
-
-    def _add(self, key, value, title: Optional[str] = None, descr: Optional[str] = None, comment=NOTHING) -> None:
+    def _add(self, key, value, title: str | None = None, descr: str | None = None, comment: str | None = None) -> None:
         """
-        Add Item To Enumeration.
+        Add NamedObject To Enumeration.
 
         Args:
             key (int): key value to be mapped.
             value: Mapped value.
 
         Keyword Args:
             title (str): Full Spoken Name.
             descr (str): Documentation Description.
             comment (str): Source Code Comment.
 
         :meta public:
         """
-        # pylint: disable=too-many-arguments
-        assert not self._locked, f"{self} is not public and forbidden to be modified."
+        if self._locked:
+            raise LockError(self)
+        items = self._items
         if key is AUTO:
-            keys = self.keys()
+            keys = items.keys()
             key = max(keys) + 1 if keys else 0
         self.keytype.check(key)
         valuetype = self.valuetype
         if valuetype:
             valuetype.check(value)
-        else:
-            validate_name(value)
-        if key in self.keys():
+        if key in items.keys():
             raise ValueError(f"key {key!r} already exists in {self}")
-        doc = Doc(title, descr, comment)
-        enumitem = EnumItem(key, value, doc)
-        # pylint: disable=not-callable
+        doc = Doc(title=title, descr=descr, comment=comment)
+        enumitem = EnumItem(key, value, doc=doc)
         if not self.filter_ or self.filter_(enumitem):
-            self[key] = enumitem
+            items[key] = enumitem
 
     @property
     def width(self):
         """Width in Bits."""
         return self.keytype.width
 
     def check(self, value, what="Value"):
@@ -200,32 +171,32 @@
         """Return `value` for `key`."""
         return self.get_bykey(key).value
 
     def get_key(self, value):
         """Return `key` for `value`."""
         return self.get_byvalue(value).key
 
-    def __iter__(self):
-        yield from self.values()
-
     def get_hex(self, value=None):
         """Get Hex Value."""
         if value is None:
             value = self.default
         return self.keytype.get_hex(value=value)
 
     def is_connectable(self, other):
         """Check For Valid Connection To `other`."""
         return (
             isinstance(other, BaseEnumType)
             and self.keytype.is_connectable(other.keytype)
             and self.valuetype == other.valuetype
             and len(self) == len(other)
             and self.keys() == other.keys()
-            and all(selfitem.value == otheritem.value for selfitem, otheritem in zip(self, other))
+            and all(
+                selfitem.value == otheritem.value
+                for selfitem, otheritem in zip(self.values(), other.values(), strict=False)
+            )
         ) or (self.keytype.is_connectable(other))
 
     def __getitem__(self, slice_):
         """Return Slice."""
         return self.keytype[slice_]
 
     @property
@@ -245,74 +216,80 @@
 
     # def cast(self, other):
     #     """
     #     How to cast an input of type `self` from a value of type `other`.
 
     #     `self = cast(other)`
     #     """
-    #     # pylint: disable=arguments-differ
     #     if isinstance(other, BaseEnumType) and self.keytype.is_connectable(other.keytype):
     #         yield "", ""
     #     return NotImplemented
 
+    @model_validator(mode="after")
+    def __post_init(self) -> "BaseEnumType":
+        if self.default is None:
+            self.__dict__["default"] = self.keytype.default
+        return self
 
-@frozen
-class AEnumType(BaseEnumType, ReusedFrozen):
+    @abstractmethod
+    def _build(self) -> None:
+        """Build Type."""
 
+
+class AEnumType(BaseEnumType, Light):
     """
     Base class for all enumerations, behaves like a dictionary.
 
     Keyword Args:
         default (int): Default Value. Default value of `keytype` by default.
         iso (int): Isolation Value. Default value of `keytype` by default.
-        no_codecov: Exclude from toggle code coverage. Default value of `keytype` by default.
 
     The protected method `_build()` should be used to build the type.
 
     Definition of an enumeration:
 
-    >>> import ucdp
-    >>> class ModeType(ucdp.AEnumType):
-    ...     keytype = ucdp.UintType(2, default=1)
-    ...     def _build(self):
+    >>> import ucdp as u
+    >>> class ModeType(u.AEnumType):
+    ...     keytype: u.AScalarType = u.UintType(2, default=1)
+    ...     def _build(self) -> None:
     ...         self._add(0, "linear", title="Linear Mode", descr="Just Linear", comment="be careful")
     ...         self._add(1, "cyclic", title="Cyclic Mode", descr="The Cyclic Mode")
     ...         self._add(2, "loop", title="Run in a Loop")
 
     Usage of an Enumeration:
 
     >>> mode = ModeType()
     >>> mode
     ModeType()
 
     The enumeration behaves like a `dict`, with elements hashed by `name`.
     But different to a regular `dict`, it returns items on pure iteration:
 
     >>> tuple(mode)
-    (EnumItem(0, 'linear', doc=...), EnumItem(1, 'cyclic', doc=...), EnumItem(2, 'loop', doc=...))
+    (0, 1, 2)
     >>> mode.keys()
     dict_keys([0, 1, 2])
     >>> mode.values()
     dict_values([EnumItem(0, 'linear', doc=...), EnumItem(1, 'cyclic', doc=...), EnumItem(2, 'loop', doc=...)])
     >>> for key, item in mode.items():
     ...     print(key, item)
     0 EnumItem(0, 'linear', doc=...)
     1 EnumItem(1, 'cyclic', doc=...)
     2 EnumItem(2, 'loop', doc=...)
 
     Enumeration items have these attributes:
 
     >>> from tabulate import tabulate
-    >>> print(tabulate([(item.key, item.value, item.title, item.descr, item.comment) for item in mode],
-    ...                headers=(".key", ".value", ".title", ".descr", ".comment")))
-      .key  .value    .title         .descr           .comment
-    ------  --------  -------------  ---------------  -------------
-         0  linear    Linear Mode    Just Linear      be careful
-         1  cyclic    Cyclic Mode    The Cyclic Mode  Cyclic Mode
-         2  loop      Run in a Loop                   Run in a Loop
+    >>> print(tabulate([(item.key, item.value, item.doc) for item in mode.values()],
+    ...                headers=(".key", ".value", ".doc")))
+      .key  .value    .doc
+    ------  --------  -------------------------------------------------------------------
+         0  linear    Doc(title='Linear Mode', descr='Just Linear', comment='be careful')
+         1  cyclic    Doc(title='Cyclic Mode', descr='The Cyclic Mode')
+         2  loop      Doc(title='Run in a Loop')
 
     To retrieve an item by value:
 
     >>> mode.get_byvalue('loop')
     EnumItem(2, 'loop', doc=Doc(title='Run in a Loop'))
     >>> mode.get_byvalue('unknown')
     Traceback (most recent call last):
@@ -354,62 +331,62 @@
       ...
     ValueError: ModeType() does not contain key 3. Known keys are 0, 1 and 2.
     >>> mode.decode(3, usedefault=True)
     'cyclic'
 
     You can also check, if a value is within the range:
 
-    >>> 'linear' in mode
+    >>> 0 in mode
     True
-    >>> 'foo' in mode
+    >>> 3 in mode
     False
 
     Enumerations are also singleton:
 
     >>> ModeType() is ModeType()
     True
     >>> ModeType() is ModeType(default=1)
     False
 
     >>> ModeType() == ModeType()
     True
     >>> ModeType() == ModeType(default=2)
     False
 
-    Attributes `width`, `default`, `iso` and `no_codecov` are taken from `keytype`:
+    Attributes `width`, `default` are taken from `keytype`:
 
     >>> mode = ModeType()
     >>> mode.width
     2
     >>> mode.default
     1
     >>> mode.check(3)
     3
     >>> mode.check(4)
     Traceback (most recent call last):
       ...
     ValueError: Value 4 is not a 2-bit integer with range [0, 3]
 
-    Attributes `default`, `iso` and `no_codecov` can be ovewritten:
+    Attributes `default` can be overwritten:
 
     >>> mode = ModeType(default=2)
     >>> mode.width
     2
     >>> mode.default
     2
 
     A mapping type, which translates one type to another:
 
     Definition of an enumeration:
 
-    >>> import ucdp
-    >>> class MappingType(ucdp.AEnumType):
-    ...     keytype = ucdp.UintType(2)
-    ...     valuetype = ucdp.UintType(16)
-    ...     def _build(self):
+    >>> import ucdp as u
+    >>> class MappingType(u.AEnumType):
+    ...     keytype: u.AScalarType = u.UintType(2)
+    ...     valuetype: u.UintType = u.UintType(16)
+    ...     def _build(self) -> None:
     ...         self._add(0, 7)
     ...         self._add(1, 31)
     ...         self._add(2, 2**14-1)
     ...         self._add(3, 2**16-1)
     >>> mapping = MappingType()
     >>> for item in mapping.values():
     ...     print(repr(item))
@@ -428,43 +405,43 @@
     Size in Bits:
 
     >>> mapping.bits
     2
 
     To determine if the enumeration is fully decoded, use `is_full`:
 
-    >>> import ucdp
-    >>> class AType(ucdp.AEnumType):
-    ...     keytype = ucdp.UintType(1)  # 2 possible values
-    ...     def _build(self):
+    >>> import ucdp as u
+    >>> class AType(u.AEnumType):
+    ...     keytype: u.AScalarType = u.UintType(1)  # 2 possible values
+    ...     def _build(self) -> None:
     ...         self._add(0, "linear")
     ...         self._add(1, "cyclic")
     >>> AType().is_full
     True
 
-    >>> class BType(ucdp.AEnumType):
-    ...     keytype = ucdp.UintType(2) # 4 possible values
-    ...     def _build(self):
+    >>> class BType(u.AEnumType):
+    ...     keytype: u.AScalarType = u.UintType(2) # 4 possible values
+    ...     def _build(self) -> None:
     ...         self._add(0, "linear")
     ...         self._add(1, "cyclic")
     >>> BType().is_full
     False
 
-    Connections are only allowed to other :any:`AEnumType` with the same key-value mapping.
+    Connections are only allowed to other :any:`EnumType` with the same key-value mapping.
     Default and isolation values are ignored.
 
-    >>> class CType(ucdp.AEnumType):
-    ...     keytype = ucdp.UintType(1)  # 2 possible values
-    ...     def _build(self):
+    >>> class CType(u.AEnumType):
+    ...     keytype: u.AScalarType = u.UintType(1)  # 2 possible values
+    ...     def _build(self) -> None:
     ...         self._add(0, "linear", title="other comment")
     ...         self._add(1, "cyclic")
 
-    >>> class DType(ucdp.AEnumType):
-    ...     keytype = ucdp.UintType(1)  # 2 possible values
-    ...     def _build(self):
+    >>> class DType(u.AEnumType):
+    ...     keytype: u.AScalarType = u.UintType(1)  # 2 possible values
+    ...     def _build(self) -> None:
     ...         self._add(0, "linear")
 
     >>> AType().is_connectable(AType())
     True
     >>> AType().is_connectable(BType())
     False
     >>> AType().is_connectable(CType())
@@ -477,17 +454,17 @@
     >>> BType()[1:0]
     UintType(2)
     >>> BType()[1]
     UintType(1)
 
     Values can be used twice:
 
-    >>> class DuplType(ucdp.AEnumType):
-    ...     keytype = ucdp.UintType(2)
-    ...     def _build(self):
+    >>> class DuplType(u.AEnumType):
+    ...     keytype: u.AScalarType = u.UintType(2)
+    ...     def _build(self) -> None:
     ...         self._add(0, 'a')
     ...         self._add(1, 'b')
     ...         self._add(2, 'c')
     ...         self._add(3, 'b')
 
     >>> dupl = DuplType()
     >>> dupl
@@ -497,43 +474,42 @@
     >>> dupl.get_value(3)
     'b'
     >>> dupl.get_key('b')
     1
 
     The `new()` method creates a new variant:
 
-    >>> class MyType(ucdp.AEnumType):
-    ...     keytype = ucdp.UintType(2)
-    ...     def _build(self):
+    >>> class MyType(u.AEnumType):
+    ...     keytype: u.AScalarType = u.UintType(2)
+    ...     def _build(self) -> None:
     ...         self._add(0, "linear")
     ...         self._add(1, "cyclic")
     ...         self._add(2, "auto")
 
     >>> MyType()
     MyType()
     >>> MyType().new(default=1)
     MyType(default=1)
     >>> MyType().new(filter_=lambda item: item.value != "cyclic")
     MyType()
     """
 
-    def __attrs_post_init__(self):
+    def model_post_init(self, __context: Any) -> None:
+        """Run Build."""
         self._build()
-        object.__setattr__(self, "_locked", True)
-
+        self._locked = True
 
-@frozen
-class AGlobalEnumType(BaseEnumType, ReusedFrozen):
 
+class AGlobalEnumType(BaseEnumType, Light):
     """
     A singleton enumeration which can be filled outside `_build` and is **shared** between instances.
 
-    >>> import ucdp
-    >>> class CtrlType(ucdp.AGlobalEnumType):
-    ...     keytype = ucdp.UintType(3)
+    >>> import ucdp as u
+    >>> class CtrlType(u.AGlobalEnumType):
+    ...     keytype: u.AScalarType = u.UintType(3)
     >>> ctrl = CtrlType()
     >>> ctrl.add(0, 'zero')
 
     >>> ctrl = CtrlType()
     >>> ctrl.add(1, 'one')
     >>> ctrl.add(7, 'seven')
 
@@ -542,64 +518,105 @@
 
     >>> ctrl = CtrlType()
     >>> ctrl.keys()
     dict_keys([0, 1, 7])
 
     This is forbidden on normal enumeration:
 
-    >>> class CtrlType(ucdp.AEnumType):
-    ...     keytype = ucdp.UintType(3)
+    >>> class CtrlType(u.AEnumType):
+    ...     keytype: u.AScalarType = u.UintType(3)
+    ...     def _build(self) -> None:
+    ...         pass
     >>> ctrl = CtrlType()
     >>> ctrl._add(0, 'zero')
     Traceback (most recent call last):
       ...
-    AssertionError: CtrlType() is not public and forbidden to be modified.
+    ucdp.exceptions.LockError: CtrlType() is already locked for modification.
     """
 
-    add = BaseEnumType._add
+    def add(self, key, value, title: str | None = None, descr: str | None = None, comment: str | None = None) -> None:
+        """
+        Add NamedObject To Enumeration.
 
+        Args:
+            key (int): key value to be mapped.
+            value: Mapped value.
 
-@frozen
-class DynamicEnumType(BaseEnumType):
+        Keyword Args:
+            title (str): Full Spoken Name.
+            descr (str): Documentation Description.
+            comment (str): Source Code Comment.
+        """
+        self._add(key=key, value=value, title=title, descr=descr, comment=comment)
 
+    def _build(self) -> None:
+        """Build Type."""
+
+    def model_post_init(self, __context: Any) -> None:
+        """Run Build."""
+        if self.__class__ is AGlobalEnumType:
+            raise TypeError("Can't instantiate abstract class AGlobalEnumType. Please create a subclass.")
+        self._build()
+
+
+class DynamicEnumType(BaseEnumType):
     """
     A enumeration which can be filled outside `_build` and is **not** shared between instances.
 
-    >>> import ucdp
-    >>> class CtrlType(ucdp.DynamicEnumType):
-    ...     keytype = ucdp.UintType(3)
+    >>> import ucdp as u
+    >>> class CtrlType(u.DynamicEnumType):
+    ...     keytype: u.AScalarType = u.UintType(3)
     >>> ctrl = CtrlType()
     >>> ctrl.add(0, 'zero')
     >>> ctrl.keys()
     dict_keys([0])
 
     >>> ctrl = CtrlType()
     >>> ctrl.add(1, 'one')
     >>> ctrl.add(7, 'seven')
     >>> ctrl.keys()
     dict_keys([1, 7])
 
     This is forbidden on normal enumeration:
 
-    >>> class CtrlType(ucdp.AEnumType):
-    ...     keytype = ucdp.UintType(3)
+    >>> class CtrlType(u.AEnumType):
+    ...     keytype: u.AScalarType = u.UintType(3)
+    ...     def _build(self) -> None:
+    ...         pass
     >>> ctrl = CtrlType()
     >>> ctrl._add(0, 'zero')
     Traceback (most recent call last):
       ...
-    AssertionError: CtrlType() is not public and forbidden to be modified.
+    ucdp.exceptions.LockError: CtrlType() is already locked for modification.
     """
 
-    idx = field(factory=_ENUMNUM.get, init=False)
+    def add(self, key, value, title: str | None = None, descr: str | None = None, comment: str | None = None) -> None:
+        """
+        Add NamedObject To Enumeration.
+
+        Args:
+            key (int): key value to be mapped.
+            value: Mapped value.
+
+        Keyword Args:
+            title (str): Full Spoken Name.
+            descr (str): Documentation Description.
+            comment (str): Source Code Comment.
+        """
+        self._add(key=key, value=value, title=title, descr=descr, comment=comment)
+
+    def _build(self) -> None:
+        """Build Type."""
 
-    add = BaseEnumType._add
+    def model_post_init(self, __context: Any) -> None:
+        """Run Build."""
+        self._build()
 
 
 class EnaType(AEnumType):
-
     """
     Enable (positive logic).
 
     >>> enable = EnaType()
     >>> enable
     EnaType()
     >>> enable.width
@@ -612,28 +629,27 @@
     EnumItem(1, 'ena', doc=Doc(title='enabled'))
 
     >>> enable = EnaType(default=1)
     >>> enable.default
     1
     """
 
-    keytype = BitType()
-    title = "Enable"
+    keytype: AScalarType = BitType()
+    title: str = "Enable"
 
-    def _build(self):
+    def _build(self) -> None:
         self._add(0, "dis", "disabled")
         self._add(1, "ena", "enabled")
 
     # def is_connectable(self, other):
     #     """Return True if connectable to `other`."""
     #     return (isinstance(other, BitType) and self.default == other.default) or super().is_connectable(other)
 
 
 class DisType(AEnumType):
-
     """
     Enable (positive logic).
 
     >>> disable = DisType()
     >>> disable
     DisType()
     >>> disable.width
@@ -646,24 +662,23 @@
     EnumItem(1, 'dis', doc=Doc(title='disabled'))
 
     >>> disable = DisType(default=1)
     >>> disable.default
     1
     """
 
-    keytype = BitType()
-    title = "Disable"
+    keytype: AScalarType = BitType()
+    title: str = "Disable"
 
-    def _build(self):
+    def _build(self) -> None:
         self._add(0, "ena", "enabled")
         self._add(1, "dis", "disabled")
 
 
 class BusyType(AEnumType):
-
     """
     Busy.
 
     >>> busy = BusyType()
     >>> busy
     BusyType()
     >>> busy.width
@@ -676,13 +691,13 @@
     EnumItem(1, 'busy', doc=Doc(title='Busy'))
 
     >>> busy = BusyType(default=1)
     >>> busy.default
     1
     """
 
-    keytype = BitType()
-    title = "Busy"
+    keytype: AScalarType = BitType()
+    title: str = "Busy"
 
-    def _build(self):
+    def _build(self) -> None:
         self._add(0, "idle", "Idle")
         self._add(1, "busy", "Busy")
```

### Comparing `ucdp-0.1.0/ucdp/types/orientation.py` & `ucdp-0.2.0/src/ucdp/orientation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -31,56 +31,56 @@
 Orient
 ===========
 
 A member in a structural type can have an orientation:
 
 * forward (`FWD`) from source to sink
 * backward (`BWD`) from sink to source
-* bi-directional (`BIDIR`) both directions
 
 >>> from tabulate import tabulate
->>> orientations = (FWD, BWD, BIDIR)
->>> overview = [(d, d.mode, d.suffix) for d in orientations]
->>> print(tabulate(overview, ("Orient", ".mode", ".suffix")))
-Orient      .mode  .suffix
---------  -------  ---------
-FWD             1
-BWD            -1
-BIDIR           0
+>>> import ucdp as u
+>>> orientations = (u.FWD, u.BWD)
+>>> overview = [(d, d.mode, d.name, d.suffix) for d in orientations]
+>>> print(tabulate(overview, ("Orient", ".mode", ".name", ".suffix")))
+Orient      .mode  .name    .suffix
+--------  -------  -------  ---------
+FWD             1  FWD
+BWD            -1  BWD
 
 Direction
 =========
 
 Ports have a direction:
 
 * input (`IN`)
 * output (`OUT`)
 * inout (`INOUT`)
+* input-monitor (`INM`)
+* output-monitor (`OUTM`)
 
 >>> from tabulate import tabulate
->>> directions = (IN, OUT, INOUT)
->>> overview = [(d, d.mode, d.suffix) for d in directions]
->>> print(tabulate(overview, ("Direction", ".mode", ".suffix")))
-Direction      .mode  .suffix
------------  -------  ---------
-IN                 1  _i
-OUT               -1  _o
-INOUT              0  _io
+>>> import ucdp as u
+>>> directions = (u.IN, u.OUT, u.INOUT)
+>>> overview = [(d, d.mode, d.name, d.suffix) for d in directions]
+>>> print(tabulate(overview, ("Direction", ".mode", ".name", ".suffix")))
+Direction      .mode  .name    .suffix
+-----------  -------  -------  ---------
+IN                 1  IN       _i
+OUT               -1  OUT      _o
+INOUT              0  INOUT    _io
 
 Common Features
 ===============
 
 You can calculate with :any:`Orientation` ...
 
 >>> FWD * FWD
 FWD
 >>> FWD * BWD
 BWD
->>> FWD * BIDIR
-BIDIR
 
 ... and :any:`Direction`
 
 >>> IN * FWD
 IN
 >>> IN * BWD
 OUT
@@ -88,22 +88,20 @@
 OUT
 >>> IN * BWD * BWD
 IN
 >>> OUT * FWD
 OUT
 >>> OUT * BWD
 IN
->>> IN * BIDIR
+>>> INOUT * FWD
 INOUT
->>> INOUT * BIDIR
+>>> INOUT * BWD
 INOUT
 >>> FWD * OUT
 BWD
->>> FWD * INOUT
-BIDIR
 
 :any:`Orientation` and :any:`Direction` are singletons. There is just one instance of each.
 
 >>> IN is IN
 True
 >>> IN is (IN * BWD * BWD)
 True
@@ -117,78 +115,91 @@
 >>> IN == FWD
 False
 
 API
 ===
 """
 
-from typing import Dict, Optional
+from typing import ClassVar, Optional, Union
 
-from attrs import define
+from .object import LightObject
 
-from ..attrs import ReusedFrozen, field
-
-
-@define(frozen=True, on_setattr=None, repr=False, auto_attribs=False)
-class AOrientation(ReusedFrozen):
 
+class AOrientation(LightObject):
     """Abstract Orientation."""
 
-    _NAMEMAP: Dict[int, str] = {}
+    _NAMEMAP: ClassVar[dict[int, str]] = {}
 
-    mode = field()
+    mode: int
     """
     Integer representation.
     """
 
-    # pylint: disable=protected-access
-    __name = field(init=False)
+    @property
+    def name(self):
+        """Name."""
+        return self._NAMEMAP[self.mode]
 
-    @__name.default
-    def _name_default(self):
+    def __str__(self):
         return self._NAMEMAP[self.mode]
 
     def __repr__(self):
-        return self.__name
+        return self._NAMEMAP[self.mode]
 
     def __mul__(self, other) -> "AOrientation":
         if isinstance(other, AOrientation):
-            return self.__class__(self.mode * other.mode)
+            return self.__class__(mode=self.mode * other.mode)
         return NotImplemented
 
     @property
     def suffix(self) -> str:
         """Suffix."""
         return ""
 
+    @classmethod
+    def cast(cls, value: Union["AOrientation", int]) -> "AOrientation":
+        """Cast `value`."""
+        if isinstance(value, cls):
+            return value
+        if isinstance(value, AOrientation):
+            return cls(mode=value.mode)
+        if isinstance(value, int) and value in cls._NAMEMAP.keys():
+            return cls(mode=value)
+        raise ValueError(f"Cannot cast {value}")
 
-class Orientation(AOrientation):
 
-    """Type Orientation."""
+class Orientation(AOrientation):
+    """
+    Type Orientation.
 
-    # pylint: disable=too-few-public-methods
+    >>> import ucdp as u
+    >>> u.Orientation.cast(1)
+    FWD
+    >>> u.Orientation.cast(u.FWD)
+    FWD
+    >>> u.Orientation.cast(u.IN)
+    FWD
+    """
 
-    _NAMEMAP = {
+    _NAMEMAP: ClassVar[dict[int, str]] = {
         1: "FWD",
         -1: "BWD",
-        0: "BIDIR",
     }
 
 
 class Direction(AOrientation):
-
     """Port Direction."""
 
-    _NAMEMAP = {
+    _NAMEMAP: ClassVar[dict[int, str]] = {
         1: "IN",
         -1: "OUT",
         0: "INOUT",
     }
 
-    _SUFFIXMAP = {
+    _SUFFIXMAP: ClassVar[dict[int, str]] = {
         1: "_i",
         -1: "_o",
         0: "_io",
     }
 
     @property
     def suffix(self) -> str:
@@ -204,72 +215,20 @@
         IN
         >>> Direction.from_name('ctrl_o')
         OUT
         >>> Direction.from_name('ctrl_io')
         INOUT
         >>> Direction.from_name('ctrl_s')
         >>> Direction.from_name('')
-        IN
         """
-        if not name:
-            return IN
         for mode, suffix in Direction._SUFFIXMAP.items():
             if name.endswith(suffix):
-                return Direction(mode)
+                return Direction(mode=mode)
         return None
 
 
-FWD = Orientation(1)
-BWD = Orientation(-1)
-BIDIR = Orientation(0)
-
-IN = Direction(1)
-OUT = Direction(-1)
-INOUT = Direction(0)
-
+FWD = Orientation(mode=1)
+BWD = Orientation(mode=-1)
 
-def convert_aorientation(value) -> AOrientation:
-    """
-    Convert Direction.
-
-    >>> convert_aorientation(FWD)
-    FWD
-    >>> convert_aorientation("test")
-    Traceback (most recent call last):
-      ...
-    ValueError: Invalid orientation 'test'. Valid are FWD, BWD, BIDIR, IN, OUT and INOUT
-    """
-    if value in (FWD, BWD, BIDIR, IN, OUT, INOUT):
-        return value
-    raise ValueError(f"Invalid orientation {value!r}. Valid are FWD, BWD, BIDIR, IN, OUT and INOUT")
-
-
-def convert_orientation(value) -> Orientation:
-    """
-    Convert Direction.
-
-    >>> convert_orientation(FWD)
-    FWD
-    >>> convert_orientation("test")
-    Traceback (most recent call last):
-      ...
-    ValueError: Invalid orientation 'test'. Valid are FWD, BWD and BIDIR
-    """
-    if value in (FWD, BWD, BIDIR):
-        return value
-    raise ValueError(f"Invalid orientation {value!r}. Valid are FWD, BWD and BIDIR")
-
-
-def convert_direction(value) -> Direction:
-    """
-    Convert Direction.
-
-    >>> convert_direction(IN)
-    IN
-    >>> convert_direction("test")
-    Traceback (most recent call last):
-      ...
-    ValueError: Invalid direction 'test'. Valid are IN, OUT and INOUT
-    """
-    if value in (IN, OUT, INOUT):
-        return value
-    raise ValueError(f"Invalid direction {value!r}. Valid are IN, OUT and INOUT")
+IN = Direction(mode=1)
+OUT = Direction(mode=-1)
+INOUT = Direction(mode=0)
```

### Comparing `ucdp-0.1.0/ucdp/types/scalar.py` & `ucdp-0.2.0/src/ucdp/typescalar.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,100 +18,111 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
-"""Scalar Types aka native Types."""
+"""
+Scalar Types.
+
+* :any:`IntegerType`
+* :any:`BitType`
+* :any:`BoolType`
+* :any:`RailType`
+* :any:`UintType`
+* :any:`SintType`
+"""
+
+from typing import Any, ClassVar
 
 from humannum import hex_
-from icdutil.slices import DOWN, Slice
 
-from ..attrs import ReusedFrozen, field, frozen
-from .base import AScalarType, AType, AVecType
+from .slices import DOWN, Slice
+from .typebase import AScalarType, AVecType
 
+INTEGER_WIDTH: int = 32
 
-@frozen
-class IntegerType(AScalarType, ReusedFrozen):
 
+class IntegerType(AScalarType):
     """
     Native Signed 32-Bit Integer.
 
     Keyword Args:
         default (int): Default Value. 0 by default.
 
     The width is fixed to 32.
 
     Documentation defaults are empty by default:
 
-    >>> import ucdp
-    >>> ucdp.IntegerType.title
-    >>> ucdp.IntegerType.descr
-    >>> ucdp.IntegerType.comment
+    >>> import ucdp as u
+    >>> u.IntegerType().title
+    >>> u.IntegerType().descr
+    >>> u.IntegerType().comment
 
     Example:
-
-    >>> example = ucdp.IntegerType()
+    >>> example = u.IntegerType()
     >>> example
     IntegerType()
     >>> example.width
     32
     >>> example.default
     0
 
     Another Example:
 
-    >>> example = ucdp.IntegerType(default=8)
+    >>> example = u.IntegerType(default=8)
     >>> example
     IntegerType(default=8)
     >>> example.width
     32
     >>> example.default
     8
 
     Selective Coverage Disable:
 
-    >>> example = ucdp.IntegerType()
+    >>> example = u.IntegerType()
     >>> example
     IntegerType()
 
     Range checking:
 
     >>> 5 in IntegerType()
     True
     >>> range(3, 10) in IntegerType()
     True
     >>> 2**32 in IntegerType()
     False
 
     Slicing:
 
-    >>> ucdp.IntegerType(default=31)['31:0']
+    >>> u.IntegerType(default=31)['31:0']
     IntegerType(default=31)
-    >>> ucdp.IntegerType(default=31)['3:1']
+    >>> u.IntegerType(default=31)['3:1']
     UintType(3, default=7)
-    >>> ucdp.IntegerType(default=31)['32:31']
+    >>> u.IntegerType(default=31)['32:31']
     Traceback (most recent call last):
         ...
     ValueError: Cannot slice bit(s) 32:31 from IntegerType(default=31) with dimension [31:0]
     """
 
-    width = 32
-    min_ = -1 * 2 ** (width - 1)
-    max_ = 2 ** (width - 1) - 1
+    width: ClassVar[int] = INTEGER_WIDTH  # type: ignore[misc]
+    min_: ClassVar[int] = -1 * 2 ** (width - 1)
+    max_: ClassVar[int] = 2 ** (width - 1) - 1
+
+    default: Any = 0
 
     def check(self, value, what="Value") -> int:
         """
         Check `value` for type.
 
         Values are limited to 32-bit signed [-2147483648, 2147483647].
 
-        >>> import ucdp
-        >>> example = ucdp.IntegerType()
+        >>> import ucdp as u
+        >>> example = u.IntegerType()
         >>> example.check(0)
         0
         >>> example.check(2147483647)
         2147483647
         >>> example.check(2147483648)
         Traceback (most recent call last):
           ...
@@ -128,109 +139,108 @@
             raise ValueError(f"{what} {value} is not a 32-bit signed integer with range [{self.min_}, {self.max_}]")
         return value
 
     def get_hex(self, value=None):
         """
         Return Hex Value.
 
-        >>> import ucdp
-        >>> ucdp.IntegerType(default=0x10FEC0DE).get_hex()
+        >>> import ucdp as u
+        >>> u.IntegerType(default=0x10FEC0DE).get_hex()
         Hex('0x10FEC0DE')
-        >>> ucdp.IntegerType(default=0x10FEC0DE).get_hex(value=0xBEEF)
+        >>> u.IntegerType(default=0x10FEC0DE).get_hex(value=0xBEEF)
         Hex('0x0000BEEF')
-        >>> ucdp.IntegerType().get_hex(value=9)
+        >>> u.IntegerType().get_hex(value=9)
         Hex('0x00000009')
         """
         if value is None:
             value = self.default
         self.check(value)
         value = int(value)
         wrap = 1 << 32
         value = (value + wrap) % wrap
         return hex_(value, width=32)
 
-    def is_connectable(self, other):
+    def is_connectable(self, other) -> bool:
         """
         Check For Valid Connection To `other`.
 
         Connections are only allowed to other :any:`IntegerType`.
         The default and isolation value have no influence.
 
         >>> IntegerType().is_connectable(IntegerType())
         True
         >>> IntegerType(default=1).is_connectable(IntegerType(default=2))
         True
         """
-        return isinstance(other, (SintType, IntegerType)) and int(other.width) == 32
+        return isinstance(other, (SintType, IntegerType)) and int(other.width) == INTEGER_WIDTH  # type: ignore[operator]
 
     def __getitem__(self, slice_):
         """Return Sliced Variant."""
         slice_ = Slice.cast(slice_, direction=DOWN)
-        if slice_.width == 32 and slice_.right == 0:
+        if slice_.width == INTEGER_WIDTH and slice_.right == 0:
             return self
-        if slice_.left < 31:
+        if slice_.left < (INTEGER_WIDTH - 1):
             return UintType(slice_.width, default=slice_.extract(self.default))
         raise ValueError(f"Cannot slice bit(s) {slice_!s} from {self} with dimension [31:0]")
 
 
-@frozen
-class BitType(AScalarType, ReusedFrozen):
-
+class BitType(AScalarType):
     """
     Native Single Bit.
 
     Keyword Args:
         default (int): Default Value. 0 by default.
 
     The width is fixed to 1.
 
     Example:
-
-    >>> import ucdp
-    >>> example = ucdp.BitType()
+    >>> import ucdp as u
+    >>> example = u.BitType()
     >>> example
     BitType()
     >>> example.width
     1
     >>> example.default
     0
 
     Another Example:
 
-    >>> example = ucdp.BitType(default=1)
+    >>> example = u.BitType(default=1)
     >>> example
     BitType(default=1)
     >>> example.width
     1
     >>> example.default
     1
 
     Slicing:
 
-    >>> ucdp.BitType(default=1)[0]
+    >>> u.BitType(default=1)[0]
     BitType(default=1)
-    >>> ucdp.BitType(default=1)[32:31]
+    >>> u.BitType(default=1)[32:31]
     Traceback (most recent call last):
         ...
     ValueError: Cannot slice bit(s) 32:31 from BitType(default=1)
     """
 
-    width = 1
-    min_ = 0
-    max_ = 1
+    width: ClassVar[int] = 1  # type: ignore[misc]
+    min_: ClassVar[int] = 0  # type: ignore[misc]
+    max_: ClassVar[int] = 1  # type: ignore[misc]
+
+    default: Any = 0
 
     @staticmethod
     def check(value, what="Value") -> int:
         """
         Check `value` for type.
 
         Values are limited to 0 and 1
 
-        >>> import ucdp
-        >>> example = ucdp.BitType()
+        >>> import ucdp as u
+        >>> example = u.BitType()
         >>> example.check(-1)
         Traceback (most recent call last):
           ...
         ValueError: Value -1 is not a single bit with range [0, 1]
         >>> example.check(0)
         0
         >>> example.check(1)
@@ -240,38 +250,37 @@
           ...
         ValueError: Value 2 is not a single bit with range [0, 1]
         >>> example.check(False)
         0
         >>> example.check(True)
         1
         """
-        # pylint: disable=arguments-differ
         value = int(value)
         if value not in (0, 1):
             raise ValueError(f"{what} {value} is not a single bit with range [0, 1]")
         return value
 
     def get_hex(self, value=None):
         """
         Return Hex Value.
 
-        >>> import ucdp
-        >>> ucdp.BitType().get_hex()
+        >>> import ucdp as u
+        >>> u.BitType().get_hex()
         Hex('0x0')
-        >>> ucdp.BitType(default=1).get_hex()
+        >>> u.BitType(default=1).get_hex()
         Hex('0x1')
-        >>> ucdp.BitType().get_hex(value=1)
+        >>> u.BitType().get_hex(value=1)
         Hex('0x1')
         """
         if value is None:
             value = self.default
         self.check(value)
         return hex_(value, width=1)
 
-    def is_connectable(self, other):
+    def is_connectable(self, other) -> bool:
         """
         Check For Valid Connection To `other`.
 
         Connections are only allowed to other :any:`BitType`.
         The default and isolation value have no influence.
 
         >>> BitType().is_connectable(BitType())
@@ -280,79 +289,74 @@
         True
 
         A connection to an :any:`UintType()` of width is forbidden (requires a cast).
 
         >>> BitType().is_connectable(UintType(2))
         False
         """
-        return isinstance(other, (BitType, UintType)) and int(other.width) == 1
+        return isinstance(other, (BitType, UintType)) and int(other.width) == 1  # type: ignore[operator]
 
     def __getitem__(self, slice_):
         slice_ = Slice.cast(slice_, direction=DOWN)
         if slice_.width == 1 and slice_.right == 0:
             return self
         raise ValueError(f"Cannot slice bit(s) {slice_!s} from {self}")
 
 
-@frozen
-class BoolType(AScalarType, ReusedFrozen):
-
+class BoolType(AScalarType):
     """
     Native Boolean.
 
     Keyword Args:
         default (int): Default Value. 0 by default.
-        iso (int): Isolation Value. Identical to default if omitted.
-        no_codecov: Exclude from toggle code coverage. Either `False`, `True` or a tuple of indicies.
 
     The width is fixed to 1.
 
     Example:
-
-    >>> import ucdp
-    >>> example = ucdp.BoolType()
+    >>> import ucdp as u
+    >>> example = u.BoolType()
     >>> example
     BoolType()
     >>> example.width
     1
     >>> example.default
     0
 
     Another Example:
 
-    >>> example = ucdp.BoolType(default=1)
+    >>> example = u.BoolType(default=True)
     >>> example
-    BoolType(default=1)
+    BoolType(default=True)
     >>> example.width
     1
     >>> example.default
-    1
+    True
 
     Slicing:
 
-    >>> ucdp.BoolType(default=1)[0]
-    BoolType(default=1)
-    >>> ucdp.BoolType()[32:31]
+    >>> u.BoolType(default=True)[0]
+    BoolType(default=True)
+    >>> u.BoolType()[32:31]
     Traceback (most recent call last):
         ...
     ValueError: Cannot slice bit(s) 32:31 from BoolType()
     """
 
-    default = field(default=0, kw_only=True)
-    width = 1
+    default: bool = False
+    width: ClassVar[int] = 1  # type: ignore[misc]
 
     @staticmethod
     def check(value, what="Value") -> bool:
         """
         Check `value` for type.
 
         Values are limited to 0 and 1
 
-        >>> import ucdp
-        >>> example = ucdp.BoolType()
+        >>> import ucdp as u
+        >>> example = u.BoolType()
         >>> example.check(-1)
         Traceback (most recent call last):
           ...
         ValueError: Value -1 is not a boolean
         >>> example.check(0)
         0
         >>> example.check(1)
@@ -362,46 +366,45 @@
           ...
         ValueError: Value 2 is not a boolean
         >>> example.check(False)
         0
         >>> example.check(True)
         1
         """
-        # pylint: disable=arguments-differ
         if value not in (False, True):
             raise ValueError(f"{what} {value} is not a boolean")
         return value
 
     def get_hex(self, value=None):
         """
         Return Hex Value.
 
-        >>> import ucdp
-        >>> ucdp.BoolType().get_hex()
+        >>> import ucdp as u
+        >>> u.BoolType().get_hex()
         Hex('0x0')
-        >>> ucdp.BoolType(default=1).get_hex()
+        >>> u.BoolType(default=True).get_hex()
         Hex('0x1')
-        >>> ucdp.BoolType().get_hex(value=1)
+        >>> u.BoolType().get_hex(value=True)
         Hex('0x1')
         """
         if value is None:
             value = self.default
         self.check(value)
         return hex_(value, width=1)
 
-    def is_connectable(self, other):
+    def is_connectable(self, other) -> bool:
         """
         Check For Valid Connection To `other`.
 
         Connections are only allowed to other :any:`BoolType`.
         The default and isolation value have no influence.
 
         >>> BoolType().is_connectable(BoolType())
         True
-        >>> BoolType(default=True).is_connectable(BoolType(default=0))
+        >>> BoolType(default=True).is_connectable(BoolType(default=False))
         True
 
         A connection to an :any:`UintType()` is forbidden (requires a cast).
 
         >>> BoolType().is_connectable(UintType(1))
         False
         """
@@ -410,69 +413,64 @@
     def __getitem__(self, slice_):
         slice_ = Slice.cast(slice_, direction=DOWN)
         if slice_.width == 1 and slice_.right == 0:
             return self
         raise ValueError(f"Cannot slice bit(s) {slice_!s} from {self}")
 
 
-@frozen
-class RailType(AScalarType, ReusedFrozen):
-
+class RailType(AScalarType):
     """
     Voltage Rail.
 
     Keyword Args:
         default (int): Default Value. 0 by default.
-        no_codecov: Exclude from toggle code coverage. Either `False`, `True` or a tuple of indicies.
 
     The width is fixed to 1.
 
     Example:
-
-    >>> import ucdp
-    >>> example = ucdp.RailType()
+    >>> import ucdp as u
+    >>> example = u.RailType()
     >>> example
     RailType()
     >>> example.width
     1
     >>> example.default
 
     Another Example:
 
-    >>> example = ucdp.RailType(default=1)
+    >>> example = u.RailType(default=1)
     >>> example
     RailType(default=1)
     >>> example.width
     1
     >>> example.default
     1
 
     Slicing:
 
-    >>> ucdp.RailType(default=1)[0]
+    >>> u.RailType(default=1)[0]
     RailType(default=1)
-    >>> ucdp.RailType(default=1)[32:31]
+    >>> u.RailType(default=1)[32:31]
     Traceback (most recent call last):
         ...
     ValueError: Cannot slice bit(s) 32:31 from RailType(default=1)
     """
 
-    default = field(default=None, kw_only=True)
-    iso = field(default=None, init=False)
-    width = 1
+    default: Any | None = None
+    width: ClassVar[int] = 1  # type: ignore[misc]
 
     @staticmethod
     def check(value, what="Value") -> int:
         """
         Check `value` for type.
 
         Values are limited to 0 and 1
 
-        >>> import ucdp
-        >>> example = ucdp.RailType()
+        >>> import ucdp as u
+        >>> example = u.RailType()
         >>> example.check(-1)
         Traceback (most recent call last):
           ...
         ValueError: Value -1 is not a single bit with range [0, 1]
         >>> example.check(0)
         0
         >>> example.check(1)
@@ -482,41 +480,40 @@
           ...
         ValueError: Value 2 is not a single bit with range [0, 1]
         >>> example.check(False)
         0
         >>> example.check(True)
         1
         """
-        # pylint: disable=arguments-differ
         value = int(value)
         if value not in (0, 1):
             raise ValueError(f"{what} {value} is not a single bit with range [0, 1]")
         return value
 
     def get_hex(self, value=None):
         """
         Return Hex Value.
 
-        >>> import ucdp
-        >>> ucdp.RailType().get_hex()
-        >>> ucdp.RailType(default=0).get_hex()
+        >>> import ucdp as u
+        >>> u.RailType().get_hex()
+        >>> u.RailType(default=0).get_hex()
         Hex('0x0')
-        >>> ucdp.RailType(default=1).get_hex()
+        >>> u.RailType(default=1).get_hex()
         Hex('0x1')
-        >>> ucdp.RailType().get_hex(value=1)
+        >>> u.RailType().get_hex(value=1)
         Hex('0x1')
         """
         if value is None:
             value = self.default
         if value is None:
             return None
         self.check(value)
         return hex_(value, width=1)
 
-    def is_connectable(self, other):
+    def is_connectable(self, other) -> bool:
         """
         Check For Valid Connection To `other`.
 
         Connections are only allowed to other :any:`RailType`.
         The default and isolation value have no influence.
 
         >>> RailType().is_connectable(RailType())
@@ -533,90 +530,91 @@
 
     # def cast(self, other):
     #     """
     #     How to cast an input of type `self` from a value of type `other`.
 
     #     `self = cast(other)`
     #     """
-    #     # pylint: disable=arguments-differ
     #     if isinstance(other, (BitType, UintType)) and other.width == 1:
     #         yield "", ""
     #     return NotImplemented
 
     def __getitem__(self, slice_):
         slice_ = Slice.cast(slice_, direction=DOWN)
         if slice_.width == 1 and slice_.right == 0:
             return self
         raise ValueError(f"Cannot slice bit(s) {slice_!s} from {self}")
 
 
-@frozen
 class UintType(AVecType):
-
     """
     Vector With Unsigned Interpretation.
 
     Args:
         width (int): Width in bits.
 
     Keyword Args:
         default (int): Default Value. 0 by default.
 
     Example:
-
-    >>> import ucdp
-    >>> example = ucdp.UintType(12)
+    >>> import ucdp as u
+    >>> example = u.UintType(12)
     >>> example
     UintType(12)
     >>> example.width
     12
     >>> example.default
     0
 
     Another Example:
 
-    >>> example = ucdp.UintType(16, default=8)
+    >>> example = u.UintType(16, default=8)
     >>> example
     UintType(16, default=8)
     >>> example.width
     16
     >>> example.default
     8
 
     Selective Coverage Disable:
 
-    >>> example = ucdp.UintType(32)
+    >>> example = u.UintType(32)
     >>> example
     UintType(32)
 
     Slicing:
 
-    >>> ucdp.UintType(16, default=31)[15:0]
+    >>> u.UintType(16, default=31)[15:0]
     UintType(16, default=31)
-    >>> ucdp.UintType(16, default=31)[3:1]
+    >>> u.UintType(16, default=31)[3:1]
     UintType(3, default=7)
-    >>> ucdp.UintType(16, default=31)[16:15]
+    >>> u.UintType(16, default=31)[16:15]
     Traceback (most recent call last):
         ...
     ValueError: Cannot slice bit(s) 16:15 from UintType(16, default=31)
     """
 
-    min_ = 0
+    min_: ClassVar[int] = 0
+
+    default: Any = 0
+
+    def __init__(self, width, **kwargs):
+        super().__init__(width=width, **kwargs)
 
     @property
     def max_(self):
         """Maximum Value."""
         return (2**self.width) - 1
 
     def check(self, value, what="Value") -> int:
         """
         Check `value` for type.
 
-        >>> import ucdp
-        >>> example = ucdp.UintType(8)
+        >>> import ucdp as u
+        >>> example = u.UintType(8)
         >>> example.check(0)
         0
         >>> example.check(255)
         255
         >>> example.check(256)
         Traceback (most recent call last):
           ...
@@ -632,28 +630,28 @@
             raise ValueError(f"{what} {value} is not a {self.width}-bit integer with range [0, {self.max_}]")
         return value
 
     def get_hex(self, value=None):
         """
         Return Hex Value.
 
-        >>> import ucdp
-        >>> ucdp.UintType(9).get_hex()
+        >>> import ucdp as u
+        >>> u.UintType(9).get_hex()
         Hex('0x000')
-        >>> ucdp.UintType(9, default=0xFE).get_hex()
+        >>> u.UintType(9, default=0xFE).get_hex()
         Hex('0x0FE')
-        >>> ucdp.UintType(9).get_hex(value=0xFE)
+        >>> u.UintType(9).get_hex(value=0xFE)
         Hex('0x0FE')
         """
         if value is None:
             value = self.default
         self.check(value)
         return hex_(value, width=self.width)
 
-    def is_connectable(self, other):
+    def is_connectable(self, other) -> bool:
         """
         Check For Valid Connection To `other`.
 
         Connections are only allowed to other :any:`UintType` of the same width.
         The default and isolation value have no influence.
 
         >>> UintType(8).is_connectable(UintType(8))
@@ -666,101 +664,98 @@
         A connection to an :any:`BitType()` is allowed, but :any:`SintType()` is forbidden (requires a cast).
 
         >>> UintType(1).is_connectable(BitType())
         True
         >>> UintType(1).is_connectable(SintType(1))
         False
         """
-        return isinstance(other, (UintType, BitType)) and self.width == other.width
+        return isinstance(other, (UintType, BitType)) and self.width == other.width  # type: ignore[operator]
 
     # def cast(self, other):
     #     """
     #     How to cast an input of type `self` from a value of type `other`.
 
     #     `self = cast(other)`
     #     """
-    #     # pylint: disable=arguments-differ
     #     if isinstance(other, (SintType, IntegerType)) and self.width == other.width:
     #         yield "", ""
     #     return NotImplemented
 
     def __getitem__(self, slice_):
         slice_ = Slice.cast(slice_, direction=DOWN)
         if slice_.width == self.width and slice_.right == self.right:
             return self
         if slice_ in self.slice_:
             return UintType(slice_.width, default=slice_.extract(self.default))
         raise ValueError(f"Cannot slice bit(s) {slice_!s} from {self}")
 
 
-@frozen
 class SintType(AVecType):
-
     """
     Vector With Unsigned Interpretation.
 
     Args:
         width (int): Width in bits.
 
     Keyword Args:
         default (int): Default Value. 0 by default.
         iso (int): Isolation Value. Identical to default if omitted.
-        no_codecov: Exclude from toggle code coverage. Either `False`, `True` or a tuple of indicies.
 
     Example:
-
-    >>> import ucdp
-    >>> example = ucdp.SintType(12)
+    >>> import ucdp as u
+    >>> example = u.SintType(12)
     >>> example
     SintType(12)
     >>> example.width
     12
     >>> example.default
     0
 
     Another Example:
 
-    >>> example = ucdp.SintType(16, default=8)
+    >>> example = u.SintType(16, default=8)
     >>> example
     SintType(16, default=8)
     >>> example.width
     16
     >>> example.default
     8
 
     Slicing:
 
-    >>> ucdp.SintType(16, default=31)[15:0]
+    >>> u.SintType(16, default=31)[15:0]
     SintType(16, default=31)
-    >>> ucdp.SintType(16, default=31)[15:8]
+    >>> u.SintType(16, default=31)[15:8]
     SintType(8)
-    >>> ucdp.SintType(16, default=31)[3:1]
+    >>> u.SintType(16, default=31)[3:1]
     UintType(3, default=7)
-    >>> ucdp.SintType(16, default=31)[16:15]
+    >>> u.SintType(16, default=31)[16:15]
     Traceback (most recent call last):
         ...
     ValueError: Cannot slice bit(s) 16:15 from SintType(16, default=31)
     """
 
+    default: Any = 0
+
     @property
     def min_(self):
         """Minimal Value."""
         return -1 * 2 ** (self.width - 1)
 
     @property
     def max_(self):
         """Maximum Value."""
         return 2 ** (self.width - 1) - 1
 
     def check(self, value, what="Value") -> int:
         """
         Check `value` for type.
 
-        >>> import ucdp
-        >>> example = ucdp.SintType(8)
+        >>> import ucdp as u
+        >>> example = u.SintType(8)
         >>> example.check(-128)
         -128
         >>> example.check(0)
         0
         >>> example.check(127)
         127
         >>> example.check(128)
@@ -781,33 +776,33 @@
             )
         return value
 
     def get_hex(self, value=None):
         """
         Return Hex Value.
 
-        >>> import ucdp
-        >>> ucdp.SintType(9).get_hex()
+        >>> import ucdp as u
+        >>> u.SintType(9).get_hex()
         Hex('0x000')
-        >>> ucdp.SintType(9, default=0xFE).get_hex()
+        >>> u.SintType(9, default=0xFE).get_hex()
         Hex('0x0FE')
-        >>> ucdp.SintType(9, default=-20).get_hex()
+        >>> u.SintType(9, default=-20).get_hex()
         Hex('0x1EC')
-        >>> ucdp.SintType(9).get_hex(value=0xFE)
+        >>> u.SintType(9).get_hex(value=0xFE)
         Hex('0x0FE')
         """
         if value is None:
             value = self.default
         self.check(value)
         width = int(self.width)
         wrap = 1 << width
         value = (value + wrap) % wrap
         return hex_(value, width=width)
 
-    def is_connectable(self, other):
+    def is_connectable(self, other) -> bool:
         """
         Check For Valid Connection To `other`.
 
         Connections are only allowed to other :any:`SintType` of the same width.
         The default and isolation value have no influence.
 
         >>> SintType(8).is_connectable(SintType(8))
@@ -820,67 +815,28 @@
         A connection to an :any:`BitType()` or :any:`UintType()` is forbidden (requires a cast).
 
         >>> SintType(1).is_connectable(BitType())
         False
         >>> SintType(1).is_connectable(UintType(1))
         False
         """
-        return isinstance(other, (SintType, IntegerType)) and self.width == other.width
+        return isinstance(other, (SintType, IntegerType)) and self.width == other.width  # type: ignore[operator]
 
     # def cast(self, other):
     #     """
     #     How to cast an input of type `self` from a value of type `other`.
 
     #     `self = cast(other)`
     #     """
-    #     # pylint: disable=arguments-differ
     #     if isinstance(other, (UintType, BitType)) and self.width == other.width:
     #         yield "", ""
     #     return NotImplemented
 
     def __getitem__(self, slice_):
         slice_ = Slice.cast(slice_, direction=DOWN)
         if slice_.width == self.width and slice_.right == self.right:
             return self
         if slice_ in self.slice_:
             if slice_.left == self.slice_.left:
                 return SintType(slice_.width, default=slice_.extract(self.default))
             return UintType(slice_.width, default=slice_.extract(self.default))
         raise ValueError(f"Cannot slice bit(s) {slice_!s} from {self}")
-
-
-@frozen
-class StringType(AType, ReusedFrozen):
-
-    """
-    Native String.
-
-    Example:
-
-    >>> import ucdp
-    >>> example = ucdp.StringType()
-    >>> example
-    StringType()
-    >>> example.bits
-    """
-
-    def is_connectable(self, other):
-        """
-        Check For Valid Connection To `other`.
-
-        Connections are only allowed to other :any:`StringType`.
-        The default and isolation value have no influence.
-
-        >>> StringType().is_connectable(StringType())
-        True
-
-        A connection to other types is forbidden.
-
-        >>> StringType().is_connectable(UintType(1))
-        False
-        """
-        return isinstance(other, StringType)
-
-    @property
-    def bits(self):
-        """Size in Bits."""
-        return None
```

### Comparing `ucdp-0.1.0/ucdp/types/struct.py` & `ucdp-0.2.0/src/ucdp/typestruct.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -24,56 +24,57 @@
 
 """
 Structure Types.
 
 A structure assembles multiple type, name, orientation pairs.
 
 * :any:`StructItem` - Struct item
-* :any:`AStructType` - Standard Struct
-* :any:`AGlobalStructType` - A public struct which fills up through all instances.
+* :any:`StructType` - Standard Struct
+* :any:`AAGlobalStructType` - A public struct which fills up through all instances.
 * :any:`DynamicStructType` - A public struct which fills up per instance.
 """
-from typing import Callable, Optional
 
-from ..attrs import NOTHING, ReusedFrozen, field, frozen
-from ..doc import Doc
-from ..nameutil import validate_name
-from ..util import AutoNum
-from .base import ACompositeType, AType
+from abc import abstractmethod
+from collections.abc import Callable
+from typing import Any
+
+from .consts import PAT_IDENTIFIER
+from .dict import Dict
+from .doc import Doc
+from .docutil import doc_from_type
+from .exceptions import LockError
+from .object import Field, Light, Object, PrivateField
 from .orientation import BWD, FWD, Orientation
+from .typebase import ACompositeType, BaseType
 
-_STRUCTNUM = AutoNum()
-
-
-@frozen
-class StructItem(ReusedFrozen):
 
+class StructItem(Object):
     """
-    Struct Item.
+    Struct NamedObject.
 
     Args:
         name (str): Name of struct member
         type_ (AType): Type of struct member
 
     Keyword Args:
         orient (Orient): Orientation of struct member. `FWD` by default
         doc (Doc): Documentation Container
         ifdef (str): IFDEF encapsulation
     """
 
-    name = field()
-    type_: AType = field()
-    orientation: Orientation = field(default=FWD)
-    doc: Doc = field(default=Doc())
-    ifdef: Optional[str] = field(default=None)
-
-    @name.validator
-    def _validate_name(self, attribute, value):
-        # pylint: disable=unused-argument
-        validate_name(value)
+    name: str = Field(pattern=PAT_IDENTIFIER)
+    type_: BaseType
+    orientation: Orientation = FWD
+    doc: Doc = Doc()
+    ifdef: str | None = None
+
+    _posargs: tuple[str, ...] = ("name", "type_")
+
+    def __init__(self, name, type_, **kwargs):
+        super().__init__(name=name, type_=type_, **kwargs)
 
     @property
     def title(self):
         """Alias to `doc.title`."""
         return self.doc.title
 
     @property
@@ -83,253 +84,322 @@
 
     @property
     def comment(self):
         """Alias to `doc.comment`."""
         return self.doc.comment
 
 
-@frozen
-class BaseStructType(dict, ACompositeType):
+StructFilter = Callable[[StructItem], bool]
 
-    """Base Type for all Structs."""
-
-    filter_: Callable[[StructItem], bool] = field(default=None, kw_only=True, repr=False)
-    _locked: bool = False
 
-    def __attrs_post_init__(self):
-        self._build()
+class BaseStructType(Dict, ACompositeType):
+    """Base Type for all Structs."""
 
-    def _build(self) -> None:
-        """Build Type."""
+    filter_: StructFilter | None = None
+    _items: dict[Any, Any] = PrivateField(default_factory=dict)
+    _locked: bool = PrivateField(default=False)
 
     def _add(
         self,
         name: str,
-        type_: AType,
+        type_: BaseType,
         orientation: Orientation = FWD,
-        title: Optional[str] = NOTHING,  # type: ignore
-        descr: Optional[str] = NOTHING,  # type: ignore
-        comment: Optional[str] = NOTHING,  # type: ignore
-        ifdef: Optional[str] = NOTHING,  # type: ignore
+        title: str | None = None,
+        descr: str | None = None,
+        comment: str | None = None,
+        ifdef: str | None = None,
     ) -> None:
         """
         Add member `name` with `type_` and `orientation`.
 
         Args:
-            name (str): Name
-            type_ (AType): Type
-            orientation (Orientation): Orientation
+            name: Name
+            type_: Type
+            orientation: Orientation
 
         Keyword Args:
-            title (str): Full Spoken Name.
-            descr (str): Documentation Description.
-            comment (str): Source Code Comment.
+            title: Full Spoken Name.
+            descr: Documentation Description.
+            comment: Source Code Comment.
+            ifdef: IFDEF encapsulation.
 
         :meta public:
         """
-        # pylint: disable=too-many-arguments
-        assert not self._locked, f"{self} is not public and forbidden to be modified."
-        if name not in self:
-            doc = Doc.from_type(type_, title, descr, comment)
-            structitem = StructItem(name, type_, orientation, doc, ifdef)
-            # pylint: disable=not-callable
+        if self._locked:
+            raise LockError(self)
+        items = self._items
+        if name not in items.keys():
+            doc = doc_from_type(type_, title=title, descr=descr, comment=comment)
+            structitem = StructItem(name, type_, orientation=orientation, doc=doc, ifdef=ifdef)
             if not self.filter_ or self.filter_(structitem):
-                self[name] = structitem
+                items[name] = structitem
         else:
             raise ValueError(f"name {name!r} already exists in {self} ({self[name]})")
 
-    def __iter__(self):
-        yield from self.values()
-
-    def is_connectable(self, other):
+    def is_connectable(self, other) -> bool:
         """Check For Valid Connection To `other`."""
-
         return (
             isinstance(other, BaseStructType)
             and len(self) == len(other)
-            and all(self._cmpitem(selfitem, otheritem) for selfitem, otheritem in zip(self, other))
+            and all(
+                self._cmpitem(selfitem, otheritem)
+                for selfitem, otheritem in zip(self.values(), other.values(), strict=False)
+            )
         )
 
     @staticmethod
     def _cmpitem(selfitem, otheritem):
         return (
             selfitem.name == otheritem.name
             and selfitem.type_.is_connectable(otheritem.type_)
             and selfitem.orientation == otheritem.orientation
             and selfitem.ifdef == otheritem.ifdef
         )
 
     @property
     def bits(self):
         """Size in Bits."""
-        return sum(item.type_.bits for item in self)
+        return sum(item.type_.bits for item in self.values())
 
+    @abstractmethod
+    def _build(self) -> None:
+        """Build Type."""
 
-@frozen
-class AStructType(BaseStructType, ReusedFrozen):
 
+class AStructType(BaseStructType, Light):
     """
-    Base class for all structural types, b    StructItem('data', UintType(8))
-    StructItem('valid', BitType())ehaves like a dictionary.
+    Base class for all structural types.
 
     The protected method `_build()` should be used to build the type.
 
     Definition of a struct:
 
-    >>> import ucdp
-    >>> class BusType(ucdp.AStructType):
-    ...     def _build(self):
-    ...         self._add('data', ucdp.UintType(8))
-    ...         self._add('valid', ucdp.BitType())
-    ...         self._add('accept', ucdp.BitType(), orientation=ucdp.BWD)
+    >>> import ucdp as u
+    >>> class BusType(u.AStructType):
+    ...     def _build(self) -> None:
+    ...         self._add('data', u.UintType(8))
+    ...         self._add('valid', u.BitType())
+    ...         self._add('accept', u.BitType(), orientation=u.BWD)
 
     Usage of a Struct:
 
     >>> bus = BusType()
     >>> bus
     BusType()
 
     The structs behave like a `dict`, with elements hashed by `name`.
     But different to a regular `dict`, it returns items on pure iteration:
 
-    >>> tuple(bus)
-    (StructItem('data', UintType(8)), StructItem('valid', BitType()), ...)
     >>> bus.keys()
     dict_keys(['data', 'valid', 'accept'])
     >>> bus.values()
     dict_values([StructItem('data', UintType(8)), StructItem('valid', BitType()), ...])
-    >>> for key, item in bus.items():
-    ...     print(key, item)
-    data StructItem('data', UintType(8))
-    valid StructItem('valid', BitType())
-    accept StructItem('accept', BitType(), orientation=BWD)
+    >>> bus.items()
+    dict_items([('data', StructItem('data', UintType(8))), ('valid', StructItem(...])
     >>> bus['valid']
     StructItem('valid', BitType())
+    >>> bus.bits
+    10
 
     Connections are only allowed to other :any:`AStructType` with the same key-value mapping.
     Default and isolation values are ignored.
 
     >>> BusType().is_connectable(BusType())
     True
 
-    >>> class Bus2Type(ucdp.AStructType):
-    ...     def _build(self):
-    ...         self._add('data', ucdp.UintType(8))
-    ...         self._add('valid', ucdp.BitType())
-    ...         self._add('accept', ucdp.BitType(), orientation=ucdp.FWD)
+    >>> class Bus2Type(u.AStructType):
+    ...     def _build(self) -> None:
+    ...         self._add('data', u.UintType(8))
+    ...         self._add('valid', u.BitType())
+    ...         self._add('accept', u.BitType(), orientation=u.FWD)
     >>> BusType().is_connectable(Bus2Type())
     False
 
-    >>> class Bus3Type(ucdp.AStructType):
-    ...     def _build(self):
-    ...         self._add('data', ucdp.UintType(8), title="title")
-    ...         self._add('valid', ucdp.BitType(default=1))
-    ...         self._add('accept', ucdp.BitType(), orientation=ucdp.BWD)
+    >>> class Bus3Type(u.AStructType):
+    ...     def _build(self) -> None:
+    ...         self._add('data', u.UintType(8), title="title")
+    ...         self._add('valid', u.BitType(default=1))
+    ...         self._add('accept', u.BitType(), orientation=u.BWD)
     >>> BusType().is_connectable(Bus3Type())
     True
 
     Struct members can be filtered.
     A struct member is added if the filter function returns `True` on a given :any:`StructItem` as argument.
 
     >>> def myfilter(structitem):
     ...     return "t" in structitem.name
-    >>> for item in BusType(filter_=myfilter): item
+    >>> for item in BusType(filter_=myfilter).values(): item
     StructItem('data', UintType(8))
     StructItem('accept', BitType(), orientation=BWD)
 
     There are also these predefined filters:
 
-    >>> for item in BusType(filter_=ucdp.fwdfilter): item
+    >>> for item in BusType(filter_=u.fwdfilter).values(): item
     StructItem('data', UintType(8))
     StructItem('valid', BitType())
 
-    >>> for item in BusType(filter_=ucdp.bwdfilter): item
+    >>> for item in BusType(filter_=u.bwdfilter).values(): item
     StructItem('accept', BitType(), orientation=BWD)
 
     This works also with the `new()` method:
 
-    >>> for item in BusType().new(filter_=ucdp.fwdfilter): item
+    >>> for item in BusType().new(filter_=u.fwdfilter).values(): item
     StructItem('data', UintType(8))
     StructItem('valid', BitType())
     """
 
-    def __attrs_post_init__(self):
+    def model_post_init(self, __context: Any) -> None:
+        """Run Build."""
         self._build()
-        object.__setattr__(self, "_locked", True)
+        self._locked = True
 
 
-@frozen
-class AGlobalStructType(BaseStructType, ReusedFrozen):
-
+class AGlobalStructType(BaseStructType, Light):
     """
     A singleton struct which can be filled outside `_build` and is **shared** between instances.
 
-    >>> import ucdp
-    >>> class BusType(ucdp.AGlobalStructType):
+    >>> import ucdp as u
+    >>> class BusType(u.AGlobalStructType):
     ...     pass
     >>> bus = BusType()
-    >>> bus.add('data', ucdp.UintType(8))
-    >>> bus.add('valid', ucdp.BitType())
+    >>> bus.add('data', u.UintType(8))
+    >>> bus.add('valid', u.BitType())
     >>> bus = BusType()
-    >>> bus.add('accept', ucdp.BitType(), orientation=ucdp.BWD)
+    >>> bus.add('accept', u.BitType(), orientation=u.BWD)
     >>> tuple(bus)
-    (StructItem('data', UintType(8)), StructItem('valid', BitType()), StructItem('accept', BitType(), orientation=BWD))
+    ('data', 'valid', 'accept')
 
     This is forbidden on normal struct:
 
-    >>> class BusType(ucdp.AStructType):
-    ...     pass
+    >>> class BusType(u.AStructType):
+    ...     def _build(self) -> None:
+    ...         pass
     >>> bus = BusType()
-    >>> bus._add('data', ucdp.UintType(8))
+    >>> bus._add('data', u.UintType(8))
     Traceback (most recent call last):
       ...
-    AssertionError: BusType() is not public and forbidden to be modified.
+    ucdp.exceptions.LockError: BusType() is already locked for modification.
     """
 
-    add = BaseStructType._add
+    def add(
+        self,
+        name: str,
+        type_: BaseType,
+        orientation: Orientation = FWD,
+        title: str | None = None,
+        descr: str | None = None,
+        comment: str | None = None,
+        ifdef: str | None = None,
+    ) -> None:
+        """
+        Add member `name` with `type_` and `orientation`.
 
+        Args:
+            name: Name
+            type_: Type
+            orientation: Orientation
 
-@frozen
-class DynamicStructType(BaseStructType):
+        Keyword Args:
+            title: Full Spoken Name.
+            descr: Documentation Description.
+            comment: Source Code Comment.
+            ifdef: IFDEF encapsulation.
+        """
+        self._add(
+            name,
+            type_,
+            orientation=orientation,
+            title=title,
+            descr=descr,
+            comment=comment,
+            ifdef=ifdef,
+        )
+
+    def _build(self) -> None:
+        """Build Type."""
+
+    def model_post_init(self, __context: Any) -> None:
+        """Run Build."""
+        if self.__class__ is AGlobalStructType:
+            raise TypeError("Can't instantiate abstract class AGlobalStructType. Please create a subclass.")
+        self._build()
 
+
+class DynamicStructType(BaseStructType):
     """
     A singleton struct which can be filled outside `_build` and is **not** shared between instances.
 
-    >>> import ucdp
-    >>> class BusType(ucdp.DynamicStructType):
+    >>> import ucdp as u
+    >>> class BusType(u.DynamicStructType):
     ...     pass
     >>> bus = BusType()
-    >>> bus.add('data', ucdp.UintType(8))
-    >>> bus.add('valid', ucdp.BitType())
+    >>> bus.add('data', u.UintType(8))
+    >>> bus.add('valid', u.BitType())
     >>> tuple(bus)
-    (StructItem('data', UintType(8)), StructItem('valid', BitType()))
+    ('data', 'valid')
     >>> bus = BusType()
-    >>> bus.add('accept', ucdp.BitType(), orientation=ucdp.BWD)
+    >>> bus.add('accept', u.BitType(), orientation=u.BWD)
     >>> tuple(bus)
-    (StructItem('accept', BitType(), orientation=BWD),)
+    ('accept',)
 
     This is forbidden on normal struct:
 
-    >>> class BusType(ucdp.AStructType):
-    ...     pass
+    >>> class BusType(u.AStructType):
+    ...     def _build(self) -> None:
+    ...         pass
     >>> bus = BusType()
-    >>> bus._add('data', ucdp.UintType(8))
+    >>> bus._add('data', u.UintType(8))
     Traceback (most recent call last):
       ...
-    AssertionError: BusType() is not public and forbidden to be modified.
+    ucdp.exceptions.LockError: BusType() is already locked for modification.
     """
 
-    idx = field(factory=_STRUCTNUM.get, init=False)
+    def add(
+        self,
+        name: str,
+        type_: BaseType,
+        orientation: Orientation = FWD,
+        title: str | None = None,
+        descr: str | None = None,
+        comment: str | None = None,
+        ifdef: str | None = None,
+    ) -> None:
+        """
+        Add member `name` with `type_` and `orientation`.
+
+        Args:
+            name: Name
+            type_: Type
+            orientation: Orientation
+
+        Keyword Args:
+            title: Full Spoken Name.
+            descr: Documentation Description.
+            comment: Source Code Comment.
+            ifdef: IFDEF encapsulation.
+        """
+        self._add(
+            name,
+            type_,
+            orientation=orientation,
+            title=title,
+            descr=descr,
+            comment=comment,
+            ifdef=ifdef,
+        )
 
-    add = BaseStructType._add
+    def _build(self) -> None:
+        """Build Type."""
 
-    _dynamic = True
+    def model_post_init(self, __context: Any) -> None:
+        """Run Build."""
+        self._build()
 
 
 def fwdfilter(structitem):
-    """Helper Function to filter for forward elements in structs."""
+    """Filter For Forward Elements In Structs."""
     return structitem.orientation == FWD
 
 
 def bwdfilter(structitem):
-    """Helper Function to filter for backward elements in structs."""
+    """Filter For Backward Elements In Structs."""
     return structitem.orientation == BWD
```

### Comparing `ucdp-0.1.0/ucdp/util.py` & `ucdp-0.2.0/src/ucdp/iterutil.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # MIT License
 #
-# Copyright (c) 2023 nbiotcloud
+# Copyright (c) 2024 nbiotcloud
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,56 +19,33 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 """
-Utilities
+Utilities.
 """
+
 import functools
 import re
-from typing import Any, Iterable, Tuple, Union
+from collections.abc import Iterable
 
 from matchor import matchs
 
 
-class AutoNum:
-
-    """
-    Auto Numbering.
-
-    >>> autonum = AutoNum()
-    >>> autonum.get()
-    0
-    >>> autonum.get()
-    1
-    """
-
-    # pylint: disable=too-few-public-methods
-
-    def __init__(self, start=0):
-        self.cnt = start
-
-    def get(self):
-        """Get Fresh Number."""
-        num = self.cnt
-        self.cnt += 1
-        return num
-
-
 @functools.lru_cache(maxsize=128)
 def _translate(seps):
     return re.compile(rf"[{seps}]\s*")
 
 
-Items = Union[Iterable[Any], str, None]
+Names = Iterable[str] | str
 
 
-def split(items, seps=";") -> Tuple[str, ...]:
+def split(items: Names, seps: str = ";") -> tuple[str, ...]:
     """
     Split items into tuple.
 
     >>> split(['abc', 'def'])
     ('abc', 'def')
     >>> split(('abc', 'def'))
     ('abc', 'def')
@@ -95,93 +72,64 @@
     if not items:
         items = []
     elif isinstance(items, str):
         items = [item.strip() for item in _translate(seps).split(items)]
     return tuple(items)
 
 
-def namefilter(names):
+def namefilter(namepats: Names):
     """
-    Create filter for names.
+    Create filter for namepats.
 
-    >>> import ucdp
-    >>> from collections import namedtuple
+    >>> import ucdp as u
     >>> def myfunc(items, filter_=None):
     ...     for item in items:
     ...         if not filter_ or filter_(item):
     ...             print(item)
-    >>> Item = namedtuple('Item', "name value")
 
-    >>> items = (Item('abc', 0), Item('cde', 1), Item('efg', 7))
+    >>> items = ('abc', 'cde', 'efg')
     >>> myfunc(items)
-    Item(name='abc', value=0)
-    Item(name='cde', value=1)
-    Item(name='efg', value=7)
-    >>> myfunc(items, filter_=ucdp.namefilter(''))
-    Item(name='abc', value=0)
-    Item(name='cde', value=1)
-    Item(name='efg', value=7)
-    >>> myfunc(items, filter_=ucdp.namefilter('cde; tuv'))
-    Item(name='cde', value=1)
-    >>> myfunc(items, filter_=ucdp.namefilter('*c*'))
-    Item(name='abc', value=0)
-    Item(name='cde', value=1)
-    >>> myfunc(items, filter_=ucdp.namefilter('!*c*'))
-    Item(name='efg', value=7)
-    >>> myfunc(items, filter_=ucdp.namefilter('*c*; !*e'))
-    Item(name='abc', value=0)
+    abc
+    cde
+    efg
+    >>> myfunc(items, filter_=u.namefilter(''))
+    abc
+    cde
+    efg
+    >>> myfunc(items, filter_=u.namefilter('cde; tuv'))
+    cde
+    >>> myfunc(items, filter_=u.namefilter('*c*'))
+    abc
+    cde
+    >>> myfunc(items, filter_=u.namefilter('!*c*'))
+    efg
+    >>> myfunc(items, filter_=u.namefilter('*c*; !*e'))
+    abc
 
     >>> items = ['abc', 'cde', 'efg']
-    >>> myfunc(items, filter_=ucdp.namefilter('*c*; !*e'))
+    >>> myfunc(items, filter_=u.namefilter('*c*; !*e'))
     abc
     """
+    _patterns: tuple[str, ...] = split(namepats)
+
+    inclist = [pat for pat in _patterns if not pat.startswith("!")]
+    exclist = [pat[1:] for pat in _patterns if pat.startswith("!")]
+
+    if inclist:
+        if exclist:
 
-    names = split(names)
+            def filter_(name: str):
+                return matchs(name, inclist) and not matchs(name, exclist)
+        else:
 
-    if names:
-        inclist = [name for name in names if not name.startswith("!")]
-        exclist = [name[1:] for name in names if name.startswith("!")]
-
-        def filter_(item):
-            if not isinstance(item, str):
-                item = item.name
-            if inclist:
-                if exclist:
-                    return matchs(item, inclist) and not matchs(item, exclist)
-                return matchs(item, inclist)
-            return not matchs(item, exclist)
+            def filter_(name: str):
+                return matchs(name, inclist)
+    elif exclist:
 
+        def filter_(name: str):
+            return not matchs(name, exclist)
     else:
 
-        def filter_(item):
-            # pylint: disable=unused-argument
+        def filter_(name: str):
             return True
 
     return filter_
-
-
-def opt(checker):
-    """
-    Optional.
-
-    Call ``checker`` only on values different from ``None``.
-
-    Assume this checker:
-
-    >>> def checker(value):
-    ...     if "a" in value:
-    ...         raise ValueError()
-    ...     return value
-
-    >>> checker(None)
-    Traceback (most recent call last):
-      ...
-    TypeError: argument of type 'NoneType' is not iterable
-    >>> opt(checker)(None)
-    """
-
-    def check(value):
-        if value is not None:
-            return checker(value)
-        return None
-
-    return check
```

