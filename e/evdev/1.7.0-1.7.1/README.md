# Comparing `tmp/evdev-1.7.0.tar.gz` & `tmp/evdev-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evdev-1.7.0.tar", last modified: Sun Feb 18 21:15:57 2024, max compression
+gzip compressed data, was "evdev-1.7.1.tar", last modified: Tue May  7 23:01:50 2024, max compression
```

## Comparing `evdev-1.7.0.tar` & `evdev-1.7.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-x---   0 gvalkov   (1000) gvalkov   (1000)        0 2024-02-18 21:15:57.517096 evdev-1.7.0/
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     1507 2024-02-18 18:46:50.000000 evdev-1.7.0/LICENSE
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)      200 2024-02-18 18:47:57.000000 evdev-1.7.0/MANIFEST.in
--rw-r--r--   0 gvalkov   (1000) gvalkov   (1000)     3238 2024-02-18 21:15:57.517096 evdev-1.7.0/PKG-INFO
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)      735 2024-02-18 21:12:00.000000 evdev-1.7.0/README.rst
-drwxr-x---   0 gvalkov   (1000) gvalkov   (1000)        0 2024-02-18 21:15:57.516096 evdev-1.7.0/evdev/
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)      549 2024-01-28 23:00:23.000000 evdev-1.7.0/evdev/__init__.py
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)    12566 2024-02-18 15:54:33.000000 evdev-1.7.0/evdev/device.py
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     2618 2024-01-28 23:03:56.000000 evdev-1.7.0/evdev/ecodes.py
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     3938 2024-01-28 23:04:01.000000 evdev-1.7.0/evdev/eventio.py
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     2865 2024-01-28 23:04:05.000000 evdev-1.7.0/evdev/eventio_async.py
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     5598 2024-01-28 23:04:08.000000 evdev-1.7.0/evdev/events.py
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     5517 2024-01-28 23:08:13.000000 evdev-1.7.0/evdev/evtest.py
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     4965 2024-01-28 23:04:14.000000 evdev-1.7.0/evdev/ff.py
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     2154 2024-01-28 23:03:18.000000 evdev-1.7.0/evdev/genecodes.py
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)    16357 2024-01-28 21:31:33.000000 evdev-1.7.0/evdev/input.c
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)    10538 2024-01-28 21:31:33.000000 evdev-1.7.0/evdev/uinput.c
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)    12572 2024-01-28 23:03:23.000000 evdev-1.7.0/evdev/uinput.py
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     4190 2024-01-28 23:03:45.000000 evdev-1.7.0/evdev/util.py
-drwxr-x---   0 gvalkov   (1000) gvalkov   (1000)        0 2024-02-18 21:15:57.517096 evdev-1.7.0/evdev.egg-info/
--rw-r--r--   0 gvalkov   (1000) gvalkov   (1000)     3238 2024-02-18 21:15:57.000000 evdev-1.7.0/evdev.egg-info/PKG-INFO
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)      464 2024-02-18 21:15:57.000000 evdev-1.7.0/evdev.egg-info/SOURCES.txt
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)        1 2024-02-18 21:15:57.000000 evdev-1.7.0/evdev.egg-info/dependency_links.txt
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)        6 2024-02-18 21:15:57.000000 evdev-1.7.0/evdev.egg-info/top_level.txt
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     1227 2024-02-18 21:15:40.000000 evdev-1.7.0/pyproject.toml
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)       38 2024-02-18 21:15:57.517096 evdev-1.7.0/setup.cfg
--rwxr-x---   0 gvalkov   (1000) gvalkov   (1000)     3349 2024-01-29 22:53:17.000000 evdev-1.7.0/setup.py
-drwxr-x---   0 gvalkov   (1000) gvalkov   (1000)        0 2024-02-18 21:15:57.517096 evdev-1.7.0/tests/
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)      760 2024-02-18 16:00:10.000000 evdev-1.7.0/tests/test_ecodes.py
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)      860 2024-01-28 23:08:13.000000 evdev-1.7.0/tests/test_events.py
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     3522 2024-01-28 23:08:13.000000 evdev-1.7.0/tests/test_uinput.py
--rw-r-----   0 gvalkov   (1000) gvalkov   (1000)      642 2024-01-28 23:08:13.000000 evdev-1.7.0/tests/test_util.py
+drwxr-x---   0 gvalkov   (1000) gvalkov   (1000)        0 2024-05-07 23:01:50.836833 evdev-1.7.1/
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     1507 2024-02-18 18:46:50.000000 evdev-1.7.1/LICENSE
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)      200 2024-02-18 18:47:57.000000 evdev-1.7.1/MANIFEST.in
+-rw-r--r--   0 gvalkov   (1000) gvalkov   (1000)     3519 2024-05-07 23:01:50.835832 evdev-1.7.1/PKG-INFO
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     1012 2024-05-07 23:00:13.000000 evdev-1.7.1/README.md
+drwxr-x---   0 gvalkov   (1000) gvalkov   (1000)        0 2024-05-07 23:01:50.835832 evdev-1.7.1/evdev/
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)      549 2024-01-28 23:00:23.000000 evdev-1.7.1/evdev/__init__.py
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)    12566 2024-02-18 15:54:33.000000 evdev-1.7.1/evdev/device.py
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     2618 2024-01-28 23:03:56.000000 evdev-1.7.1/evdev/ecodes.py
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     3938 2024-01-28 23:04:01.000000 evdev-1.7.1/evdev/eventio.py
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     2865 2024-01-28 23:04:05.000000 evdev-1.7.1/evdev/eventio_async.py
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     5598 2024-01-28 23:04:08.000000 evdev-1.7.1/evdev/events.py
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     5517 2024-01-28 23:08:13.000000 evdev-1.7.1/evdev/evtest.py
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     4965 2024-01-28 23:04:14.000000 evdev-1.7.1/evdev/ff.py
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     2154 2024-01-28 23:03:18.000000 evdev-1.7.1/evdev/genecodes.py
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)    16357 2024-01-28 21:31:33.000000 evdev-1.7.1/evdev/input.c
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)    10575 2024-05-07 22:20:05.000000 evdev-1.7.1/evdev/uinput.c
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)    13348 2024-05-07 22:20:05.000000 evdev-1.7.1/evdev/uinput.py
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     4190 2024-01-28 23:03:45.000000 evdev-1.7.1/evdev/util.py
+drwxr-x---   0 gvalkov   (1000) gvalkov   (1000)        0 2024-05-07 23:01:50.835832 evdev-1.7.1/evdev.egg-info/
+-rw-r--r--   0 gvalkov   (1000) gvalkov   (1000)     3519 2024-05-07 23:01:50.000000 evdev-1.7.1/evdev.egg-info/PKG-INFO
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)      463 2024-05-07 23:01:50.000000 evdev-1.7.1/evdev.egg-info/SOURCES.txt
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)        1 2024-05-07 23:01:50.000000 evdev-1.7.1/evdev.egg-info/dependency_links.txt
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)        6 2024-05-07 23:01:50.000000 evdev-1.7.1/evdev.egg-info/top_level.txt
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     1227 2024-05-07 23:01:20.000000 evdev-1.7.1/pyproject.toml
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)       38 2024-05-07 23:01:50.836833 evdev-1.7.1/setup.cfg
+-rwxr-x---   0 gvalkov   (1000) gvalkov   (1000)     3349 2024-01-29 22:53:17.000000 evdev-1.7.1/setup.py
+drwxr-x---   0 gvalkov   (1000) gvalkov   (1000)        0 2024-05-07 23:01:50.835832 evdev-1.7.1/tests/
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)      760 2024-02-18 16:00:10.000000 evdev-1.7.1/tests/test_ecodes.py
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)      860 2024-01-28 23:08:13.000000 evdev-1.7.1/tests/test_events.py
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)     3522 2024-01-28 23:08:13.000000 evdev-1.7.1/tests/test_uinput.py
+-rw-r-----   0 gvalkov   (1000) gvalkov   (1000)      642 2024-01-28 23:08:13.000000 evdev-1.7.1/tests/test_util.py
```

### Comparing `evdev-1.7.0/LICENSE` & `evdev-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/PKG-INFO` & `evdev-1.7.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6576 6465  : 2.1.Name: evde
-00000020: 760a 5665 7273 696f 6e3a 2031 2e37 2e30  v.Version: 1.7.0
+00000020: 760a 5665 7273 696f 6e3a 2031 2e37 2e31  v.Version: 1.7.1
 00000030: 0a53 756d 6d61 7279 3a20 4269 6e64 696e  .Summary: Bindin
 00000040: 6773 2074 6f20 7468 6520 4c69 6e75 7820  gs to the Linux 
 00000050: 696e 7075 7420 6861 6e64 6c69 6e67 2073  input handling s
 00000060: 7562 7379 7374 656d 0a41 7574 686f 722d  ubsystem.Author-
 00000070: 656d 6169 6c3a 2047 656f 7267 6920 5661  email: Georgi Va
 00000080: 6c6b 6f76 203c 6765 6f72 6769 2e74 2e76  lkov <georgi.t.v
 00000090: 616c 6b6f 7640 676d 6169 6c2e 636f 6d3e  alkov@gmail.com>
@@ -148,56 +148,73 @@
 00000930: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
 00000940: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
 00000950: 5079 7468 6f6e 203a 3a20 496d 706c 656d  Python :: Implem
 00000960: 656e 7461 7469 6f6e 203a 3a20 4350 7974  entation :: CPyt
 00000970: 686f 6e0a 5265 7175 6972 6573 2d50 7974  hon.Requires-Pyt
 00000980: 686f 6e3a 203e 3d33 2e36 0a44 6573 6372  hon: >=3.6.Descr
 00000990: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
-000009a0: 7970 653a 2074 6578 742f 782d 7273 740a  ype: text/x-rst.
-000009b0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
-000009c0: 4345 4e53 450a 0a2a 6576 6465 762a 0a2d  CENSE..*evdev*.-
-000009d0: 2d2d 2d2d 2d2d 0a0a 5468 6973 2070 6163  ------..This pac
-000009e0: 6b61 6765 2070 726f 7669 6465 7320 6269  kage provides bi
-000009f0: 6e64 696e 6773 2074 6f20 7468 6520 6765  ndings to the ge
-00000a00: 6e65 7269 6320 696e 7075 7420 6576 656e  neric input even
-00000a10: 7420 696e 7465 7266 6163 6520 696e 0a4c  t interface in.L
-00000a20: 696e 7578 2e20 5468 6520 2a65 7664 6576  inux. The *evdev
-00000a30: 2a20 696e 7465 7266 6163 6520 7365 7276  * interface serv
-00000a40: 6573 2074 6865 2070 7572 706f 7365 206f  es the purpose o
-00000a50: 6620 7061 7373 696e 6720 6576 656e 7473  f passing events
-00000a60: 0a67 656e 6572 6174 6564 2069 6e20 7468  .generated in th
-00000a70: 6520 6b65 726e 656c 2064 6972 6563 746c  e kernel directl
-00000a80: 7920 746f 2075 7365 7273 7061 6365 2074  y to userspace t
-00000a90: 6872 6f75 6768 2063 6861 7261 6374 6572  hrough character
-00000aa0: 0a64 6576 6963 6573 2074 6861 7420 6172  .devices that ar
-00000ab0: 6520 7479 7069 6361 6c6c 7920 6c6f 6361  e typically loca
-00000ac0: 7465 6420 696e 2060 602f 6465 762f 696e  ted in ``/dev/in
-00000ad0: 7075 742f 6060 2e0a 0a54 6869 7320 7061  put/``...This pa
-00000ae0: 636b 6167 6520 616c 736f 2063 6f6d 6573  ckage also comes
-00000af0: 2077 6974 6820 6269 6e64 696e 6773 2074   with bindings t
-00000b00: 6f20 2a75 696e 7075 742a 2c20 7468 6520  o *uinput*, the 
-00000b10: 7573 6572 7370 6163 6520 696e 7075 740a  userspace input.
-00000b20: 7375 6273 7973 7465 6d2e 202a 5569 6e70  subsystem. *Uinp
-00000b30: 7574 2a20 616c 6c6f 7773 2075 7365 7273  ut* allows users
-00000b40: 7061 6365 2070 726f 6772 616d 7320 746f  pace programs to
-00000b50: 2063 7265 6174 6520 616e 6420 6861 6e64   create and hand
-00000b60: 6c65 0a69 6e70 7574 2064 6576 6963 6573  le.input devices
-00000b70: 2074 6861 7420 6361 6e20 696e 6a65 6374   that can inject
-00000b80: 2065 7665 6e74 7320 6469 7265 6374 6c79   events directly
-00000b90: 2069 6e74 6f20 7468 6520 696e 7075 740a   into the input.
-00000ba0: 7375 6273 7973 7465 6d2e 0a0a 446f 6375  subsystem...Docu
-00000bb0: 6d65 6e74 6174 696f 6e3a 0a20 2020 2068  mentation:.    h
-00000bc0: 7474 7073 3a2f 2f70 7974 686f 6e2d 6576  ttps://python-ev
-00000bd0: 6465 762e 7265 6164 7468 6564 6f63 732e  dev.readthedocs.
-00000be0: 696f 2f65 6e2f 6c61 7465 7374 2f0a 0a44  io/en/latest/..D
-00000bf0: 6576 656c 6f70 6d65 6e74 3a0a 2020 2020  evelopment:.    
-00000c00: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000c10: 6f6d 2f67 7661 6c6b 6f76 2f70 7974 686f  om/gvalkov/pytho
-00000c20: 6e2d 6576 6465 760a 0a50 6163 6b61 6765  n-evdev..Package
-00000c30: 3a0a 2020 2020 6874 7470 733a 2f2f 7079  :.    https://py
-00000c40: 7069 2e70 7974 686f 6e2e 6f72 672f 7079  pi.python.org/py
-00000c50: 7069 2f65 7664 6576 0a0a 4368 616e 6765  pi/evdev..Change
-00000c60: 6c6f 673a 0a20 2020 2068 7474 7073 3a2f  log:.    https:/
-00000c70: 2f70 7974 686f 6e2d 6576 6465 762e 7265  /python-evdev.re
-00000c80: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00000c90: 6c61 7465 7374 2f63 6861 6e67 656c 6f67  latest/changelog
-00000ca0: 2e68 746d 6c0a                           .html.
+000009a0: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
+000009b0: 776e 0a4c 6963 656e 7365 2d46 696c 653a  wn.License-File:
+000009c0: 204c 4943 454e 5345 0a0a 2320 6576 6465   LICENSE..# evde
+000009d0: 760a 0a3c 703e 0a20 2020 203c 6120 6872  v..<p>.    <a hr
+000009e0: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+000009f0: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
+00000a00: 2f65 7664 6576 223e 3c69 6d67 2061 6c74  /evdev"><img alt
+00000a10: 3d22 7079 7069 2076 6572 7369 6f6e 2220  ="pypi version" 
+00000a20: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000a30: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000a40: 2f76 2f65 7664 6576 2e73 7667 223e 3c2f  /v/evdev.svg"></
+00000a50: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00000a60: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000a70: 6f6d 2f67 7661 6c6b 6f76 2f70 7974 686f  om/gvalkov/pytho
+00000a80: 6e2d 6576 6465 762f 626c 6f62 2f6d 6169  n-evdev/blob/mai
+00000a90: 6e2f 4c49 4345 4e53 4522 3e3c 696d 6720  n/LICENSE"><img 
+00000aa0: 616c 743d 224c 6963 656e 7365 2220 7372  alt="License" sr
+00000ab0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000ac0: 6869 656c 6473 2e69 6f2f 7079 7069 2f6c  hields.io/pypi/l
+00000ad0: 2f65 7664 6576 223e 3c2f 613e 0a3c 2f70  /evdev"></a>.</p
+00000ae0: 3e0a 0a54 6869 7320 7061 636b 6167 6520  >..This package 
+00000af0: 7072 6f76 6964 6573 2062 696e 6469 6e67  provides binding
+00000b00: 7320 746f 2074 6865 2067 656e 6572 6963  s to the generic
+00000b10: 2069 6e70 7574 2065 7665 6e74 2069 6e74   input event int
+00000b20: 6572 6661 6365 2069 6e20 4c69 6e75 782e  erface in Linux.
+00000b30: 0a54 6865 202a 6576 6465 762a 2069 6e74  .The *evdev* int
+00000b40: 6572 6661 6365 2073 6572 7665 7320 7468  erface serves th
+00000b50: 6520 7075 7270 6f73 6520 6f66 2070 6173  e purpose of pas
+00000b60: 7369 6e67 2065 7665 6e74 7320 6765 6e65  sing events gene
+00000b70: 7261 7465 6420 696e 2074 6865 0a6b 6572  rated in the.ker
+00000b80: 6e65 6c20 6469 7265 6374 6c79 2074 6f20  nel directly to 
+00000b90: 7573 6572 7370 6163 6520 7468 726f 7567  userspace throug
+00000ba0: 6820 6368 6172 6163 7465 7220 6465 7669  h character devi
+00000bb0: 6365 7320 7468 6174 2061 7265 2074 7970  ces that are typ
+00000bc0: 6963 616c 6c79 0a6c 6f63 6174 6564 2069  ically.located i
+00000bd0: 6e20 602f 6465 762f 696e 7075 742f 602e  n `/dev/input/`.
+00000be0: 0a0a 5468 6973 2070 6163 6b61 6765 2061  ..This package a
+00000bf0: 6c73 6f20 636f 6d65 7320 7769 7468 2062  lso comes with b
+00000c00: 696e 6469 6e67 7320 746f 202a 7569 6e70  indings to *uinp
+00000c10: 7574 2a2c 2074 6865 2075 7365 7273 7061  ut*, the userspa
+00000c20: 6365 2069 6e70 7574 0a73 7562 7379 7374  ce input.subsyst
+00000c30: 656d 2e20 2a55 696e 7075 742a 2061 6c6c  em. *Uinput* all
+00000c40: 6f77 7320 7573 6572 7370 6163 6520 7072  ows userspace pr
+00000c50: 6f67 7261 6d73 2074 6f20 6372 6561 7465  ograms to create
+00000c60: 2061 6e64 2068 616e 646c 6520 696e 7075   and handle inpu
+00000c70: 7420 6465 7669 6365 730a 7468 6174 2063  t devices.that c
+00000c80: 616e 2069 6e6a 6563 7420 6576 656e 7473  an inject events
+00000c90: 2064 6972 6563 746c 7920 696e 746f 2074   directly into t
+00000ca0: 6865 2069 6e70 7574 2073 7562 7379 7374  he input subsyst
+00000cb0: 656d 2e0a 0a2a 2a2a 446f 6375 6d65 6e74  em...***Document
+00000cc0: 6174 696f 6e3a 2a2a 2a20 200a 6874 7470  ation:***  .http
+00000cd0: 733a 2f2f 7079 7468 6f6e 2d65 7664 6576  s://python-evdev
+00000ce0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000cf0: 656e 2f6c 6174 6573 742f 0a0a 2a2a 2a44  en/latest/..***D
+00000d00: 6576 656c 6f70 6d65 6e74 3a2a 2a2a 2020  evelopment:***  
+00000d10: 0a68 7474 7073 3a2f 2f67 6974 6875 622e  .https://github.
+00000d20: 636f 6d2f 6776 616c 6b6f 762f 7079 7468  com/gvalkov/pyth
+00000d30: 6f6e 2d65 7664 6576 0a0a 2a2a 2a50 6163  on-evdev..***Pac
+00000d40: 6b61 6765 3a2a 2a2a 2020 0a68 7474 7073  kage:***  .https
+00000d50: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
+00000d60: 7267 2f70 7970 692f 6576 6465 760a 0a2a  rg/pypi/evdev..*
+00000d70: 2a2a 4368 616e 6765 6c6f 673a 2a2a 2a20  **Changelog:*** 
+00000d80: 200a 6874 7470 733a 2f2f 7079 7468 6f6e   .https://python
+00000d90: 2d65 7664 6576 2e72 6561 6474 6865 646f  -evdev.readthedo
+00000da0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000db0: 6368 616e 6765 6c6f 672e 6874 6d6c 0a    changelog.html.
```

### Comparing `evdev-1.7.0/README.rst` & `evdev-1.7.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,64 @@
-00000000: 2a65 7664 6576 2a0a 2d2d 2d2d 2d2d 2d0a  *evdev*.-------.
-00000010: 0a54 6869 7320 7061 636b 6167 6520 7072  .This package pr
-00000020: 6f76 6964 6573 2062 696e 6469 6e67 7320  ovides bindings 
-00000030: 746f 2074 6865 2067 656e 6572 6963 2069  to the generic i
-00000040: 6e70 7574 2065 7665 6e74 2069 6e74 6572  nput event inter
-00000050: 6661 6365 2069 6e0a 4c69 6e75 782e 2054  face in.Linux. T
-00000060: 6865 202a 6576 6465 762a 2069 6e74 6572  he *evdev* inter
-00000070: 6661 6365 2073 6572 7665 7320 7468 6520  face serves the 
-00000080: 7075 7270 6f73 6520 6f66 2070 6173 7369  purpose of passi
-00000090: 6e67 2065 7665 6e74 730a 6765 6e65 7261  ng events.genera
-000000a0: 7465 6420 696e 2074 6865 206b 6572 6e65  ted in the kerne
-000000b0: 6c20 6469 7265 6374 6c79 2074 6f20 7573  l directly to us
-000000c0: 6572 7370 6163 6520 7468 726f 7567 6820  erspace through 
-000000d0: 6368 6172 6163 7465 720a 6465 7669 6365  character.device
-000000e0: 7320 7468 6174 2061 7265 2074 7970 6963  s that are typic
-000000f0: 616c 6c79 206c 6f63 6174 6564 2069 6e20  ally located in 
-00000100: 6060 2f64 6576 2f69 6e70 7574 2f60 602e  ``/dev/input/``.
-00000110: 0a0a 5468 6973 2070 6163 6b61 6765 2061  ..This package a
-00000120: 6c73 6f20 636f 6d65 7320 7769 7468 2062  lso comes with b
-00000130: 696e 6469 6e67 7320 746f 202a 7569 6e70  indings to *uinp
-00000140: 7574 2a2c 2074 6865 2075 7365 7273 7061  ut*, the userspa
-00000150: 6365 2069 6e70 7574 0a73 7562 7379 7374  ce input.subsyst
-00000160: 656d 2e20 2a55 696e 7075 742a 2061 6c6c  em. *Uinput* all
-00000170: 6f77 7320 7573 6572 7370 6163 6520 7072  ows userspace pr
-00000180: 6f67 7261 6d73 2074 6f20 6372 6561 7465  ograms to create
-00000190: 2061 6e64 2068 616e 646c 650a 696e 7075   and handle.inpu
-000001a0: 7420 6465 7669 6365 7320 7468 6174 2063  t devices that c
-000001b0: 616e 2069 6e6a 6563 7420 6576 656e 7473  an inject events
-000001c0: 2064 6972 6563 746c 7920 696e 746f 2074   directly into t
-000001d0: 6865 2069 6e70 7574 0a73 7562 7379 7374  he input.subsyst
-000001e0: 656d 2e0a 0a44 6f63 756d 656e 7461 7469  em...Documentati
-000001f0: 6f6e 3a0a 2020 2020 6874 7470 733a 2f2f  on:.    https://
-00000200: 7079 7468 6f6e 2d65 7664 6576 2e72 6561  python-evdev.rea
-00000210: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00000220: 6174 6573 742f 0a0a 4465 7665 6c6f 706d  atest/..Developm
-00000230: 656e 743a 0a20 2020 2068 7474 7073 3a2f  ent:.    https:/
-00000240: 2f67 6974 6875 622e 636f 6d2f 6776 616c  /github.com/gval
-00000250: 6b6f 762f 7079 7468 6f6e 2d65 7664 6576  kov/python-evdev
-00000260: 0a0a 5061 636b 6167 653a 0a20 2020 2068  ..Package:.    h
-00000270: 7474 7073 3a2f 2f70 7970 692e 7079 7468  ttps://pypi.pyth
-00000280: 6f6e 2e6f 7267 2f70 7970 692f 6576 6465  on.org/pypi/evde
-00000290: 760a 0a43 6861 6e67 656c 6f67 3a0a 2020  v..Changelog:.  
-000002a0: 2020 6874 7470 733a 2f2f 7079 7468 6f6e    https://python
-000002b0: 2d65 7664 6576 2e72 6561 6474 6865 646f  -evdev.readthedo
-000002c0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-000002d0: 6368 616e 6765 6c6f 672e 6874 6d6c 0a    changelog.html.
+00000000: 2320 6576 6465 760a 0a3c 703e 0a20 2020  # evdev..<p>.   
+00000010: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000020: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
+00000030: 672f 7079 7069 2f65 7664 6576 223e 3c69  g/pypi/evdev"><i
+00000040: 6d67 2061 6c74 3d22 7079 7069 2076 6572  mg alt="pypi ver
+00000050: 7369 6f6e 2220 7372 633d 2268 7474 7073  sion" src="https
+00000060: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000070: 6f2f 7079 7069 2f76 2f65 7664 6576 2e73  o/pypi/v/evdev.s
+00000080: 7667 223e 3c2f 613e 0a20 2020 203c 6120  vg"></a>.    <a 
+00000090: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+000000a0: 7468 7562 2e63 6f6d 2f67 7661 6c6b 6f76  thub.com/gvalkov
+000000b0: 2f70 7974 686f 6e2d 6576 6465 762f 626c  /python-evdev/bl
+000000c0: 6f62 2f6d 6169 6e2f 4c49 4345 4e53 4522  ob/main/LICENSE"
+000000d0: 3e3c 696d 6720 616c 743d 224c 6963 656e  ><img alt="Licen
+000000e0: 7365 2220 7372 633d 2268 7474 7073 3a2f  se" src="https:/
+000000f0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000100: 7079 7069 2f6c 2f65 7664 6576 223e 3c2f  pypi/l/evdev"></
+00000110: 613e 0a3c 2f70 3e0a 0a54 6869 7320 7061  a>.</p>..This pa
+00000120: 636b 6167 6520 7072 6f76 6964 6573 2062  ckage provides b
+00000130: 696e 6469 6e67 7320 746f 2074 6865 2067  indings to the g
+00000140: 656e 6572 6963 2069 6e70 7574 2065 7665  eneric input eve
+00000150: 6e74 2069 6e74 6572 6661 6365 2069 6e20  nt interface in 
+00000160: 4c69 6e75 782e 0a54 6865 202a 6576 6465  Linux..The *evde
+00000170: 762a 2069 6e74 6572 6661 6365 2073 6572  v* interface ser
+00000180: 7665 7320 7468 6520 7075 7270 6f73 6520  ves the purpose 
+00000190: 6f66 2070 6173 7369 6e67 2065 7665 6e74  of passing event
+000001a0: 7320 6765 6e65 7261 7465 6420 696e 2074  s generated in t
+000001b0: 6865 0a6b 6572 6e65 6c20 6469 7265 6374  he.kernel direct
+000001c0: 6c79 2074 6f20 7573 6572 7370 6163 6520  ly to userspace 
+000001d0: 7468 726f 7567 6820 6368 6172 6163 7465  through characte
+000001e0: 7220 6465 7669 6365 7320 7468 6174 2061  r devices that a
+000001f0: 7265 2074 7970 6963 616c 6c79 0a6c 6f63  re typically.loc
+00000200: 6174 6564 2069 6e20 602f 6465 762f 696e  ated in `/dev/in
+00000210: 7075 742f 602e 0a0a 5468 6973 2070 6163  put/`...This pac
+00000220: 6b61 6765 2061 6c73 6f20 636f 6d65 7320  kage also comes 
+00000230: 7769 7468 2062 696e 6469 6e67 7320 746f  with bindings to
+00000240: 202a 7569 6e70 7574 2a2c 2074 6865 2075   *uinput*, the u
+00000250: 7365 7273 7061 6365 2069 6e70 7574 0a73  serspace input.s
+00000260: 7562 7379 7374 656d 2e20 2a55 696e 7075  ubsystem. *Uinpu
+00000270: 742a 2061 6c6c 6f77 7320 7573 6572 7370  t* allows usersp
+00000280: 6163 6520 7072 6f67 7261 6d73 2074 6f20  ace programs to 
+00000290: 6372 6561 7465 2061 6e64 2068 616e 646c  create and handl
+000002a0: 6520 696e 7075 7420 6465 7669 6365 730a  e input devices.
+000002b0: 7468 6174 2063 616e 2069 6e6a 6563 7420  that can inject 
+000002c0: 6576 656e 7473 2064 6972 6563 746c 7920  events directly 
+000002d0: 696e 746f 2074 6865 2069 6e70 7574 2073  into the input s
+000002e0: 7562 7379 7374 656d 2e0a 0a2a 2a2a 446f  ubsystem...***Do
+000002f0: 6375 6d65 6e74 6174 696f 6e3a 2a2a 2a20  cumentation:*** 
+00000300: 200a 6874 7470 733a 2f2f 7079 7468 6f6e   .https://python
+00000310: 2d65 7664 6576 2e72 6561 6474 6865 646f  -evdev.readthedo
+00000320: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000330: 0a0a 2a2a 2a44 6576 656c 6f70 6d65 6e74  ..***Development
+00000340: 3a2a 2a2a 2020 0a68 7474 7073 3a2f 2f67  :***  .https://g
+00000350: 6974 6875 622e 636f 6d2f 6776 616c 6b6f  ithub.com/gvalko
+00000360: 762f 7079 7468 6f6e 2d65 7664 6576 0a0a  v/python-evdev..
+00000370: 2a2a 2a50 6163 6b61 6765 3a2a 2a2a 2020  ***Package:***  
+00000380: 0a68 7474 7073 3a2f 2f70 7970 692e 7079  .https://pypi.py
+00000390: 7468 6f6e 2e6f 7267 2f70 7970 692f 6576  thon.org/pypi/ev
+000003a0: 6465 760a 0a2a 2a2a 4368 616e 6765 6c6f  dev..***Changelo
+000003b0: 673a 2a2a 2a20 200a 6874 7470 733a 2f2f  g:***  .https://
+000003c0: 7079 7468 6f6e 2d65 7664 6576 2e72 6561  python-evdev.rea
+000003d0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000003e0: 6174 6573 742f 6368 616e 6765 6c6f 672e  atest/changelog.
+000003f0: 6874 6d6c                                html
```

### Comparing `evdev-1.7.0/evdev/__init__.py` & `evdev-1.7.1/evdev/__init__.py`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/evdev/device.py` & `evdev-1.7.1/evdev/device.py`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/evdev/ecodes.py` & `evdev-1.7.1/evdev/ecodes.py`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/evdev/eventio.py` & `evdev-1.7.1/evdev/eventio.py`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/evdev/eventio_async.py` & `evdev-1.7.1/evdev/eventio_async.py`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/evdev/events.py` & `evdev-1.7.1/evdev/events.py`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/evdev/evtest.py` & `evdev-1.7.1/evdev/evtest.py`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/evdev/ff.py` & `evdev-1.7.1/evdev/ff.py`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/evdev/genecodes.py` & `evdev-1.7.1/evdev/genecodes.py`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/evdev/input.c` & `evdev-1.7.1/evdev/input.c`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/evdev/uinput.c` & `evdev-1.7.1/evdev/uinput.c`

 * *Files 1% similar despite different names*

```diff
@@ -102,18 +102,20 @@
 {
     int fd;
     char sysname[64];
 
     int ret = PyArg_ParseTuple(args, "i", &fd);
     if (!ret) return NULL;
 
+    #ifdef UI_GET_SYSNAME
     if (ioctl(fd, UI_GET_SYSNAME(sizeof(sysname)), &sysname) < 0)
         goto on_err;
 
     return Py_BuildValue("s", &sysname);
+    #endif
 
     on_err:
         PyErr_SetFromErrno(PyExc_OSError);
         return NULL;
 }
 
 // Different kernel versions have different device setup methods. You can read
```

### Comparing `evdev-1.7.0/evdev/uinput.py` & `evdev-1.7.1/evdev/uinput.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,15 +86,18 @@
         vendor=0x1,
         product=0x1,
         version=0x1,
         bustype=0x3,
         devnode="/dev/uinput",
         phys="py-evdev-uinput",
         input_props=None,
-        max_effects=ecodes.FF_MAX_EFFECTS,
+        # CentOS 7 has sufficiently old headers that FF_MAX_EFFECTS is not defined there,
+        # which causes the whole module to fail loading. Fallback on a hardcoded value of
+        # FF_MAX_EFFECTS if it is not defined in the ecodes.
+        max_effects=ecodes.ecodes.get("FF_MAX_EFFECTS", 96),
     ):
         """
         Arguments
         ---------
         events : dict
           Dictionary of event types mapping to lists of event codes. The
           event types and codes that the uinput device will be able to
@@ -326,19 +329,28 @@
                 break
         else:  # no break
             raise FileNotFoundError()
 
         # It is possible that there is some delay before /dev/input/event* shows
         # up on old systems that do not use devtmpfs, so if the device cannot be
         # found, wait for a short amount and then try again once.
-        try:
-            return device.InputDevice(device_path)
-        except FileNotFoundError:
-            time.sleep(0.1)
-            return device.InputDevice(device_path)
+        #
+        # Furthermore, even if devtmpfs is in use, it is possible that the device
+        # does show up immediately, but without the correct permissions that
+        # still need to be set by udev. Wait for up to two seconds for either the
+        # device to show up or the permissions to be set.
+        for attempt in range(19):
+            try:
+                return device.InputDevice(device_path)
+            except (FileNotFoundError, PermissionError):
+                time.sleep(0.1)
+
+        # Last attempt. If this fails, whatever exception the last attempt raises
+        # shall be the exception that this function raises.
+        return device.InputDevice(device_path)
 
     def _find_device_fallback(self):
         """
         Tries to find the device node when UI_GET_SYSNAME is not available or
         we're running on a system sufficiently exotic that we do not know how
         to interpret its return value.
         """
```

### Comparing `evdev-1.7.0/evdev/util.py` & `evdev-1.7.1/evdev/util.py`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/evdev.egg-info/PKG-INFO` & `evdev-1.7.1/evdev.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6576 6465  : 2.1.Name: evde
-00000020: 760a 5665 7273 696f 6e3a 2031 2e37 2e30  v.Version: 1.7.0
+00000020: 760a 5665 7273 696f 6e3a 2031 2e37 2e31  v.Version: 1.7.1
 00000030: 0a53 756d 6d61 7279 3a20 4269 6e64 696e  .Summary: Bindin
 00000040: 6773 2074 6f20 7468 6520 4c69 6e75 7820  gs to the Linux 
 00000050: 696e 7075 7420 6861 6e64 6c69 6e67 2073  input handling s
 00000060: 7562 7379 7374 656d 0a41 7574 686f 722d  ubsystem.Author-
 00000070: 656d 6169 6c3a 2047 656f 7267 6920 5661  email: Georgi Va
 00000080: 6c6b 6f76 203c 6765 6f72 6769 2e74 2e76  lkov <georgi.t.v
 00000090: 616c 6b6f 7640 676d 6169 6c2e 636f 6d3e  alkov@gmail.com>
@@ -148,56 +148,73 @@
 00000930: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
 00000940: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
 00000950: 5079 7468 6f6e 203a 3a20 496d 706c 656d  Python :: Implem
 00000960: 656e 7461 7469 6f6e 203a 3a20 4350 7974  entation :: CPyt
 00000970: 686f 6e0a 5265 7175 6972 6573 2d50 7974  hon.Requires-Pyt
 00000980: 686f 6e3a 203e 3d33 2e36 0a44 6573 6372  hon: >=3.6.Descr
 00000990: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
-000009a0: 7970 653a 2074 6578 742f 782d 7273 740a  ype: text/x-rst.
-000009b0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
-000009c0: 4345 4e53 450a 0a2a 6576 6465 762a 0a2d  CENSE..*evdev*.-
-000009d0: 2d2d 2d2d 2d2d 0a0a 5468 6973 2070 6163  ------..This pac
-000009e0: 6b61 6765 2070 726f 7669 6465 7320 6269  kage provides bi
-000009f0: 6e64 696e 6773 2074 6f20 7468 6520 6765  ndings to the ge
-00000a00: 6e65 7269 6320 696e 7075 7420 6576 656e  neric input even
-00000a10: 7420 696e 7465 7266 6163 6520 696e 0a4c  t interface in.L
-00000a20: 696e 7578 2e20 5468 6520 2a65 7664 6576  inux. The *evdev
-00000a30: 2a20 696e 7465 7266 6163 6520 7365 7276  * interface serv
-00000a40: 6573 2074 6865 2070 7572 706f 7365 206f  es the purpose o
-00000a50: 6620 7061 7373 696e 6720 6576 656e 7473  f passing events
-00000a60: 0a67 656e 6572 6174 6564 2069 6e20 7468  .generated in th
-00000a70: 6520 6b65 726e 656c 2064 6972 6563 746c  e kernel directl
-00000a80: 7920 746f 2075 7365 7273 7061 6365 2074  y to userspace t
-00000a90: 6872 6f75 6768 2063 6861 7261 6374 6572  hrough character
-00000aa0: 0a64 6576 6963 6573 2074 6861 7420 6172  .devices that ar
-00000ab0: 6520 7479 7069 6361 6c6c 7920 6c6f 6361  e typically loca
-00000ac0: 7465 6420 696e 2060 602f 6465 762f 696e  ted in ``/dev/in
-00000ad0: 7075 742f 6060 2e0a 0a54 6869 7320 7061  put/``...This pa
-00000ae0: 636b 6167 6520 616c 736f 2063 6f6d 6573  ckage also comes
-00000af0: 2077 6974 6820 6269 6e64 696e 6773 2074   with bindings t
-00000b00: 6f20 2a75 696e 7075 742a 2c20 7468 6520  o *uinput*, the 
-00000b10: 7573 6572 7370 6163 6520 696e 7075 740a  userspace input.
-00000b20: 7375 6273 7973 7465 6d2e 202a 5569 6e70  subsystem. *Uinp
-00000b30: 7574 2a20 616c 6c6f 7773 2075 7365 7273  ut* allows users
-00000b40: 7061 6365 2070 726f 6772 616d 7320 746f  pace programs to
-00000b50: 2063 7265 6174 6520 616e 6420 6861 6e64   create and hand
-00000b60: 6c65 0a69 6e70 7574 2064 6576 6963 6573  le.input devices
-00000b70: 2074 6861 7420 6361 6e20 696e 6a65 6374   that can inject
-00000b80: 2065 7665 6e74 7320 6469 7265 6374 6c79   events directly
-00000b90: 2069 6e74 6f20 7468 6520 696e 7075 740a   into the input.
-00000ba0: 7375 6273 7973 7465 6d2e 0a0a 446f 6375  subsystem...Docu
-00000bb0: 6d65 6e74 6174 696f 6e3a 0a20 2020 2068  mentation:.    h
-00000bc0: 7474 7073 3a2f 2f70 7974 686f 6e2d 6576  ttps://python-ev
-00000bd0: 6465 762e 7265 6164 7468 6564 6f63 732e  dev.readthedocs.
-00000be0: 696f 2f65 6e2f 6c61 7465 7374 2f0a 0a44  io/en/latest/..D
-00000bf0: 6576 656c 6f70 6d65 6e74 3a0a 2020 2020  evelopment:.    
-00000c00: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000c10: 6f6d 2f67 7661 6c6b 6f76 2f70 7974 686f  om/gvalkov/pytho
-00000c20: 6e2d 6576 6465 760a 0a50 6163 6b61 6765  n-evdev..Package
-00000c30: 3a0a 2020 2020 6874 7470 733a 2f2f 7079  :.    https://py
-00000c40: 7069 2e70 7974 686f 6e2e 6f72 672f 7079  pi.python.org/py
-00000c50: 7069 2f65 7664 6576 0a0a 4368 616e 6765  pi/evdev..Change
-00000c60: 6c6f 673a 0a20 2020 2068 7474 7073 3a2f  log:.    https:/
-00000c70: 2f70 7974 686f 6e2d 6576 6465 762e 7265  /python-evdev.re
-00000c80: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00000c90: 6c61 7465 7374 2f63 6861 6e67 656c 6f67  latest/changelog
-00000ca0: 2e68 746d 6c0a                           .html.
+000009a0: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
+000009b0: 776e 0a4c 6963 656e 7365 2d46 696c 653a  wn.License-File:
+000009c0: 204c 4943 454e 5345 0a0a 2320 6576 6465   LICENSE..# evde
+000009d0: 760a 0a3c 703e 0a20 2020 203c 6120 6872  v..<p>.    <a hr
+000009e0: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+000009f0: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
+00000a00: 2f65 7664 6576 223e 3c69 6d67 2061 6c74  /evdev"><img alt
+00000a10: 3d22 7079 7069 2076 6572 7369 6f6e 2220  ="pypi version" 
+00000a20: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000a30: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000a40: 2f76 2f65 7664 6576 2e73 7667 223e 3c2f  /v/evdev.svg"></
+00000a50: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00000a60: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000a70: 6f6d 2f67 7661 6c6b 6f76 2f70 7974 686f  om/gvalkov/pytho
+00000a80: 6e2d 6576 6465 762f 626c 6f62 2f6d 6169  n-evdev/blob/mai
+00000a90: 6e2f 4c49 4345 4e53 4522 3e3c 696d 6720  n/LICENSE"><img 
+00000aa0: 616c 743d 224c 6963 656e 7365 2220 7372  alt="License" sr
+00000ab0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000ac0: 6869 656c 6473 2e69 6f2f 7079 7069 2f6c  hields.io/pypi/l
+00000ad0: 2f65 7664 6576 223e 3c2f 613e 0a3c 2f70  /evdev"></a>.</p
+00000ae0: 3e0a 0a54 6869 7320 7061 636b 6167 6520  >..This package 
+00000af0: 7072 6f76 6964 6573 2062 696e 6469 6e67  provides binding
+00000b00: 7320 746f 2074 6865 2067 656e 6572 6963  s to the generic
+00000b10: 2069 6e70 7574 2065 7665 6e74 2069 6e74   input event int
+00000b20: 6572 6661 6365 2069 6e20 4c69 6e75 782e  erface in Linux.
+00000b30: 0a54 6865 202a 6576 6465 762a 2069 6e74  .The *evdev* int
+00000b40: 6572 6661 6365 2073 6572 7665 7320 7468  erface serves th
+00000b50: 6520 7075 7270 6f73 6520 6f66 2070 6173  e purpose of pas
+00000b60: 7369 6e67 2065 7665 6e74 7320 6765 6e65  sing events gene
+00000b70: 7261 7465 6420 696e 2074 6865 0a6b 6572  rated in the.ker
+00000b80: 6e65 6c20 6469 7265 6374 6c79 2074 6f20  nel directly to 
+00000b90: 7573 6572 7370 6163 6520 7468 726f 7567  userspace throug
+00000ba0: 6820 6368 6172 6163 7465 7220 6465 7669  h character devi
+00000bb0: 6365 7320 7468 6174 2061 7265 2074 7970  ces that are typ
+00000bc0: 6963 616c 6c79 0a6c 6f63 6174 6564 2069  ically.located i
+00000bd0: 6e20 602f 6465 762f 696e 7075 742f 602e  n `/dev/input/`.
+00000be0: 0a0a 5468 6973 2070 6163 6b61 6765 2061  ..This package a
+00000bf0: 6c73 6f20 636f 6d65 7320 7769 7468 2062  lso comes with b
+00000c00: 696e 6469 6e67 7320 746f 202a 7569 6e70  indings to *uinp
+00000c10: 7574 2a2c 2074 6865 2075 7365 7273 7061  ut*, the userspa
+00000c20: 6365 2069 6e70 7574 0a73 7562 7379 7374  ce input.subsyst
+00000c30: 656d 2e20 2a55 696e 7075 742a 2061 6c6c  em. *Uinput* all
+00000c40: 6f77 7320 7573 6572 7370 6163 6520 7072  ows userspace pr
+00000c50: 6f67 7261 6d73 2074 6f20 6372 6561 7465  ograms to create
+00000c60: 2061 6e64 2068 616e 646c 6520 696e 7075   and handle inpu
+00000c70: 7420 6465 7669 6365 730a 7468 6174 2063  t devices.that c
+00000c80: 616e 2069 6e6a 6563 7420 6576 656e 7473  an inject events
+00000c90: 2064 6972 6563 746c 7920 696e 746f 2074   directly into t
+00000ca0: 6865 2069 6e70 7574 2073 7562 7379 7374  he input subsyst
+00000cb0: 656d 2e0a 0a2a 2a2a 446f 6375 6d65 6e74  em...***Document
+00000cc0: 6174 696f 6e3a 2a2a 2a20 200a 6874 7470  ation:***  .http
+00000cd0: 733a 2f2f 7079 7468 6f6e 2d65 7664 6576  s://python-evdev
+00000ce0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000cf0: 656e 2f6c 6174 6573 742f 0a0a 2a2a 2a44  en/latest/..***D
+00000d00: 6576 656c 6f70 6d65 6e74 3a2a 2a2a 2020  evelopment:***  
+00000d10: 0a68 7474 7073 3a2f 2f67 6974 6875 622e  .https://github.
+00000d20: 636f 6d2f 6776 616c 6b6f 762f 7079 7468  com/gvalkov/pyth
+00000d30: 6f6e 2d65 7664 6576 0a0a 2a2a 2a50 6163  on-evdev..***Pac
+00000d40: 6b61 6765 3a2a 2a2a 2020 0a68 7474 7073  kage:***  .https
+00000d50: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
+00000d60: 7267 2f70 7970 692f 6576 6465 760a 0a2a  rg/pypi/evdev..*
+00000d70: 2a2a 4368 616e 6765 6c6f 673a 2a2a 2a20  **Changelog:*** 
+00000d80: 200a 6874 7470 733a 2f2f 7079 7468 6f6e   .https://python
+00000d90: 2d65 7664 6576 2e72 6561 6474 6865 646f  -evdev.readthedo
+00000da0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000db0: 6368 616e 6765 6c6f 672e 6874 6d6c 0a    changelog.html.
```

### Comparing `evdev-1.7.0/pyproject.toml` & `evdev-1.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "evdev"
-version = "1.7.0"
+version = "1.7.1"
 description = "Bindings to the Linux input handling subsystem"
 keywords = ["evdev", "input", "uinput"]
-readme = "README.rst"
+readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.6"
 authors = [
   { name="Georgi Valkov", email="georgi.t.valkov@gmail.com" },
 ]
 maintainers = [
   { name="Tobi", email="proxima@sezanzeb.de" },
@@ -35,17 +35,17 @@
 [tool.ruff]
 line-length = 120
 
 [tool.ruff.lint]
 ignore = ["E265", "E241", "F403", "F401", "E401", "E731"]
 
 [tool.bumpversion]
-current_version = "1.7.0"
+current_version = "1.7.1"
 commit = true
 tag = true
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 
 [[tool.bumpversion.files]]
-filename = "docs/conf.py"
+filename = "docs/conf.py"
```

### Comparing `evdev-1.7.0/setup.py` & `evdev-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/tests/test_ecodes.py` & `evdev-1.7.1/tests/test_ecodes.py`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/tests/test_events.py` & `evdev-1.7.1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/tests/test_uinput.py` & `evdev-1.7.1/tests/test_uinput.py`

 * *Files identical despite different names*

### Comparing `evdev-1.7.0/tests/test_util.py` & `evdev-1.7.1/tests/test_util.py`

 * *Files identical despite different names*

