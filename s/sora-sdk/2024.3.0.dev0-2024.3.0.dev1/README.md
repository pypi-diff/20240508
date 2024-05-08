# Comparing `tmp/sora_sdk-2024.3.0.dev0.tar.gz` & `tmp/sora_sdk-2024.3.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sora_sdk-2024.3.0.dev0.tar", last modified: Wed May  1 06:30:54 2024, max compression
+gzip compressed data, was "sora_sdk-2024.3.0.dev1.tar", last modified: Wed May  8 07:02:27 2024, max compression
```

## Comparing `sora_sdk-2024.3.0.dev0.tar` & `sora_sdk-2024.3.0.dev1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-01 06:30:54.630010 sora_sdk-2024.3.0.dev0/
--rw-r--r--   0 runner     (501) staff       (20)    10174 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       33 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)    31624 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/NOTICE.md
--rw-r--r--   0 runner     (501) staff       (20)    17906 2024-05-01 06:30:54.629547 sora_sdk-2024.3.0.dev0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     5431 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/README.md
--rw-r--r--   0 runner     (501) staff       (20)    10395 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/pypath.py
--rw-r--r--   0 runner     (501) staff       (20)     3741 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)    29155 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/run.py
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-01 06:30:54.630094 sora_sdk-2024.3.0.dev0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1893 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-01 06:30:54.606643 sora_sdk-2024.3.0.dev0/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-01 06:30:54.610005 sora_sdk-2024.3.0.dev0/src/sora_sdk/
--rw-r--r--   0 runner     (501) staff       (20)     1180 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/src/sora_sdk/__init__.py
--rw-r--r--   0 runner     (501) staff       (20) 14367024 2024-05-01 06:30:47.000000 sora_sdk-2024.3.0.dev0/src/sora_sdk/sora_sdk_ext.cpython-38-darwin.so
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-01 06:30:54.628927 sora_sdk-2024.3.0.dev0/src/sora_sdk.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)    17906 2024-05-01 06:30:54.000000 sora_sdk-2024.3.0.dev0/src/sora_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      319 2024-05-01 06:30:54.000000 sora_sdk-2024.3.0.dev0/src/sora_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-01 06:30:54.000000 sora_sdk-2024.3.0.dev0/src/sora_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2024-05-01 06:30:54.000000 sora_sdk-2024.3.0.dev0/src/sora_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-01 06:30:54.628526 sora_sdk-2024.3.0.dev0/tests/
--rw-r--r--   0 runner     (501) staff       (20)      596 2024-05-01 06:28:12.000000 sora_sdk-2024.3.0.dev0/tests/test_recvonly.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 07:02:27.760016 sora_sdk-2024.3.0.dev1/
+-rw-r--r--   0 runner     (501) staff       (20)    10174 2024-05-08 06:58:54.000000 sora_sdk-2024.3.0.dev1/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       33 2024-05-08 06:58:54.000000 sora_sdk-2024.3.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)    31624 2024-05-08 06:58:54.000000 sora_sdk-2024.3.0.dev1/NOTICE.md
+-rw-r--r--   0 runner     (501) staff       (20)    17929 2024-05-08 07:02:27.759487 sora_sdk-2024.3.0.dev1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     5454 2024-05-08 06:58:54.000000 sora_sdk-2024.3.0.dev1/README.md
+-rw-r--r--   0 runner     (501) staff       (20)    10395 2024-05-08 06:58:54.000000 sora_sdk-2024.3.0.dev1/pypath.py
+-rw-r--r--   0 runner     (501) staff       (20)     3741 2024-05-08 06:58:54.000000 sora_sdk-2024.3.0.dev1/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)    29155 2024-05-08 06:58:54.000000 sora_sdk-2024.3.0.dev1/run.py
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-08 07:02:27.760107 sora_sdk-2024.3.0.dev1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1893 2024-05-08 06:58:54.000000 sora_sdk-2024.3.0.dev1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 07:02:27.734033 sora_sdk-2024.3.0.dev1/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 07:02:27.738238 sora_sdk-2024.3.0.dev1/src/sora_sdk/
+-rw-r--r--   0 runner     (501) staff       (20)     1180 2024-05-08 06:58:54.000000 sora_sdk-2024.3.0.dev1/src/sora_sdk/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20) 14367024 2024-05-08 07:02:19.000000 sora_sdk-2024.3.0.dev1/src/sora_sdk/sora_sdk_ext.cpython-38-darwin.so
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 07:02:27.758621 sora_sdk-2024.3.0.dev1/src/sora_sdk.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    17929 2024-05-08 07:02:27.000000 sora_sdk-2024.3.0.dev1/src/sora_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      319 2024-05-08 07:02:27.000000 sora_sdk-2024.3.0.dev1/src/sora_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-08 07:02:27.000000 sora_sdk-2024.3.0.dev1/src/sora_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        9 2024-05-08 07:02:27.000000 sora_sdk-2024.3.0.dev1/src/sora_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-08 07:02:27.757330 sora_sdk-2024.3.0.dev1/tests/
+-rw-r--r--   0 runner     (501) staff       (20)      596 2024-05-08 06:58:54.000000 sora_sdk-2024.3.0.dev1/tests/test_recvonly.py
```

### Comparing `sora_sdk-2024.3.0.dev0/LICENSE` & `sora_sdk-2024.3.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `sora_sdk-2024.3.0.dev0/NOTICE.md` & `sora_sdk-2024.3.0.dev1/NOTICE.md`

 * *Files identical despite different names*

### Comparing `sora_sdk-2024.3.0.dev0/PKG-INFO` & `sora_sdk-2024.3.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sora_sdk
-Version: 2024.3.0.dev0
+Version: 2024.3.0.dev1
 Summary: WebRTC SFU Sora Python SDK
 Home-page: https://github.com/shiguredo/sora-python-sdk
 Author-email: "Shiguredo Inc." <contact+pypi@shiguredo.jp>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -241,15 +241,15 @@
 
 ## ドキュメント
 
 [Sora Python SDK](https://sora-python-sdk.shiguredo.jp/)
 
 ## サンプル集
 
-[examples](examples)を参照してください。
+[examples](examples) を参照してください。
 
 ## sora_sdk パッケージの追加
 
 ### pip
 
 ```console
 $ pip install sora_sdk
@@ -296,14 +296,15 @@
 - Intel VPL H.265 対応
   - [アダワープジャパン株式会社](https://adawarp.com/) 様
 
 ### 優先実装が可能な機能一覧
 
 **詳細は Discord やメールなどでお気軽にお問い合わせください**
 
+- Ubuntu 24.04 x86_64
 - Ubuntu 22.04 arm64
   - Python 3.10
   - NVIDIA Jetson JetPack SDK 6.0
 
 ## サポートについて
 
 ### Discord
```

### Comparing `sora_sdk-2024.3.0.dev0/README.md` & `sora_sdk-2024.3.0.dev1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 ## ドキュメント
 
 [Sora Python SDK](https://sora-python-sdk.shiguredo.jp/)
 
 ## サンプル集
 
-[examples](examples)を参照してください。
+[examples](examples) を参照してください。
 
 ## sora_sdk パッケージの追加
 
 ### pip
 
 ```console
 $ pip install sora_sdk
@@ -97,14 +97,15 @@
 - Intel VPL H.265 対応
   - [アダワープジャパン株式会社](https://adawarp.com/) 様
 
 ### 優先実装が可能な機能一覧
 
 **詳細は Discord やメールなどでお気軽にお問い合わせください**
 
+- Ubuntu 24.04 x86_64
 - Ubuntu 22.04 arm64
   - Python 3.10
   - NVIDIA Jetson JetPack SDK 6.0
 
 ## サポートについて
 
 ### Discord
```

### Comparing `sora_sdk-2024.3.0.dev0/pypath.py` & `sora_sdk-2024.3.0.dev1/pypath.py`

 * *Files identical despite different names*

### Comparing `sora_sdk-2024.3.0.dev0/pyproject.toml` & `sora_sdk-2024.3.0.dev1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "sora_sdk"
 authors = [{ name = "Shiguredo Inc.", email = "contact+pypi@shiguredo.jp" }]
-version = "2024.3.0.dev0"
+version = "2024.3.0.dev1"
 description = "WebRTC SFU Sora Python SDK"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
```

### Comparing `sora_sdk-2024.3.0.dev0/run.py` & `sora_sdk-2024.3.0.dev1/run.py`

 * *Files identical despite different names*

### Comparing `sora_sdk-2024.3.0.dev0/setup.py` & `sora_sdk-2024.3.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `sora_sdk-2024.3.0.dev0/src/sora_sdk/__init__.py` & `sora_sdk-2024.3.0.dev1/src/sora_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `sora_sdk-2024.3.0.dev0/src/sora_sdk/sora_sdk_ext.cpython-38-darwin.so` & `sora_sdk-2024.3.0.dev1/src/sora_sdk/sora_sdk_ext.cpython-38-darwin.so`

 * *Files 0% similar despite different names*

#### aarch64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit arm64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL|WEAK_DEFINES|BINDS_TO_WEAK|HAS_TLV_DESCRIPTORS>*

```diff
@@ -193,15 +193,15 @@
 00000c00: 0200 0000 1800 0000 9821 d500 da0e 0000  .........!......
 00000c10: d024 d600 b060 0300 0b00 0000 5000 0000  .$...`......P...
 00000c20: 0000 0000 0000 0000 0000 0000 e10b 0000  ................
 00000c30: e10b 0000 f902 0000 0000 0000 0000 0000  ................
 00000c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c50: 380f d600 6505 0000 0000 0000 0000 0000  8...e...........
 00000c60: 0000 0000 0000 0000 1b00 0000 1800 0000  ................
-00000c70: 8342 63ee eeb9 3a65 baac 3fc1 dbcf 6a0c  .Bc...:e..?...j.
+00000c70: b224 de98 2b83 34f9 b814 9299 b51c f572  .$..+.4........r
 00000c80: 3200 0000 2000 0000 0100 0000 0006 0d00  2... ...........
 00000c90: 0000 0e00 0100 0000 0300 0000 0007 f703  ................
 00000ca0: 2a00 0000 1000 0000 0000 0000 0000 0000  *...............
 00000cb0: 0c00 0000 6800 0000 1800 0000 0200 0000  ....h...........
 00000cc0: 0000 0200 0000 0100 2f53 7973 7465 6d2f  ......../System/
 00000cd0: 4c69 6272 6172 792f 4672 616d 6577 6f72  Library/Framewor
 00000ce0: 6b73 2f41 5646 6f75 6e64 6174 696f 6e2e  ks/AVFoundation.
@@ -3706,66 +3706,66 @@
 0000e790: 4bae 0094 e003 13aa a062 2b94 ff83 00d1  K........b+.....
 0000e7a0: fd7b 01a9 fd43 0091 a1c3 1fb8 e203 00f9  .{...C..........
 0000e7b0: 000c 40f9 2001 00b4 0800 40f9 0819 40f9  ..@. .....@...@.
 0000e7c0: a113 00d1 e203 0091 0001 3fd6 fd7b 41a9  ..........?..{A.
 0000e7d0: ff83 0091 c003 5fd6 5701 0094 ff83 03d1  ......_.W.......
 0000e7e0: e923 076d fc6f 08a9 fa67 09a9 f85f 0aa9  .#.m.o...g..._..
 0000e7f0: f657 0ba9 f44f 0ca9 fd7b 0da9 fd43 0391  .W...O...{...C..
-0000e800: 0840 201e f603 01aa f403 00aa f303 08aa  .@ .............
+0000e800: 0840 201e f503 01aa f403 00aa f303 08aa  .@ .............
 0000e810: 00e0 0291 e02f 00f9 2800 8052 e883 0139  ...../..(..R...9
-0000e820: 5c63 2b94 9996 40f9 990a 00b4 95a2 0491  \c+...@.........
-0000e830: f60b 00b4 88a6 40f9 197d 169b 00c1 221e  ......@..}....".
-0000e840: 285b 0090 0151 42fd 0008 611e 0008 611e  ([...QB...a...a.
-0000e850: 0008 611e 1700 789e 96e2 0391 5963 2b94  ..a...x.....Yc+.
-0000e860: 1700 178b f87e 8ad2 78bc b4f2 7893 d8f2  .....~..x...x...
-0000e870: 1804 e0f2 1a7d 8052 3b81 95d2 9b43 abf2  .....}.R;....C..
-0000e880: 9b6c c7f2 fbfb fff2 a802 40f9 1f01 19eb  .l........@.....
-0000e890: 8205 0054 4761 2b94 4005 0035 4963 2b94  ...TGa+.@..5Ic+.
-0000e8a0: 1f00 17eb 4a04 0054 4663 2b94 fc02 00cb  ....J..TFc+.....
-0000e8b0: 9f07 00f1 6b03 0054 4263 2b94 4463 2b94  ....k..TBc+.Dc+.
-0000e8c0: e000 00b4 1f04 00f1 eb00 0054 1f00 18eb  ...........T....
-0000e8d0: 2901 0054 0800 f092 0800 0014 0800 80d2  )..T............
-0000e8e0: 0600 0014 1f00 1beb 6200 0054 0800 f0d2  ........b..T....
-0000e8f0: 0700 0014 087c 1a9b 89fb 40d2 1f01 09eb  .....|....@.....
-0000e900: 6d00 0054 0200 f092 0200 0014 0201 1c8b  m..T............
-0000e910: e163 0191 e003 16aa 0063 2b94 2963 2b94  .c.......c+.)c+.
-0000e920: 2863 2b94 1f00 17eb 0bfb ff54 a802 40f9  (c+........T..@.
-0000e930: 1f01 19eb 6200 0054 1e61 2b94 a00c 0034  ....b..T.a+....4
-0000e940: 1c61 2b94 4003 0034 ff03 0139 c864 00d0  .a+.@..4...9.d..
-0000e950: 08d1 43f9 e807 00f9 0901 40f9 2905 0091  ..C.......@.)...
-0000e960: 0901 00f9 e003 0191 e123 0091 e803 13aa  .........#......
-0000e970: 7b00 0094 0c00 0014 ff03 0139 c864 00d0  {..........9.d..
-0000e980: 08d1 43f9 e807 00f9 0901 40f9 2905 0091  ..C.......@.)...
-0000e990: 0901 00f9 e003 0191 e123 0091 e803 13aa  .........#......
-0000e9a0: 6f00 0094 e023 0091 3c00 0014 37fb 7fd3  o....#..<...7...
-0000e9b0: 3f03 00f1 e0a2 9fda 5c63 2b94 f603 00aa  ?.......\c+.....
-0000e9c0: 989e 40f9 e103 18aa e203 17aa ad64 2b94  ..@..........d+.
-0000e9d0: 0107 198b 8896 40f9 0801 19cb 02f9 7fd3  ......@.........
-0000e9e0: e003 18aa aa64 2b94 8896 40f9 1701 19cb  .....d+...@.....
-0000e9f0: e003 15aa e103 17aa 2200 8052 e100 0094  ........"..R....
-0000ea00: 9796 00f9 0200 0090 42b0 3391 e003 16aa  ........B.3.....
-0000ea10: 0100 80d2 25b2 0094 e303 00aa 88a6 40f9  ....%.........@.
-0000ea20: 290b c89a e923 00f9 e883 04a9 0800 8252  )....#.........R
-0000ea30: 2800 a072 e86b 00b9 ff03 00b9 3400 8052  (..r.k......4..R
-0000ea40: e203 0191 e5a3 0191 e003 16aa 4100 8052  ............A..R
-0000ea50: 0400 80d2 0600 8052 2700 8052 d4ad 0094  .......R'..R....
-0000ea60: e007 00f9 90ad 0094 0180 40ad 0200 c03d  ..........@....=
-0000ea70: e287 00ad e003 833c f4a3 0139 e0a3 0191  .......<...9....
-0000ea80: e123 0091 e803 13aa 5c00 0094 e007 40f9  .#......\.....@.
-0000ea90: 8bad 0094 e043 0191 5ff1 ff97 e883 4139  .....C.._.....A9
-0000eaa0: 6800 0034 e02f 40f9 bd62 2b94 fd7b 4da9  h..4./@..b+..{M.
-0000eab0: f44f 4ca9 f657 4ba9 f85f 4aa9 fa67 49a9  .OL..WK.._J..gI.
-0000eac0: fc6f 48a9 e923 476d ff83 0391 c003 5fd6  .oH..#Gm......_.
-0000ead0: ff03 0139 c864 00d0 08d1 43f9 e807 00f9  ...9.d....C.....
-0000eae0: 0901 40f9 2905 0091 0901 00f9 e003 0191  ..@.)...........
-0000eaf0: e123 0091 e803 13aa 1900 0094 aaff ff17  .#..............
-0000eb00: 0b00 0014 0f00 0014 0900 0014 0d00 0014  ................
-0000eb10: f303 00aa e007 40f9 69ad 0094 0200 0014  ......@.i.......
-0000eb20: f303 00aa e043 0191 0300 0014 f303 00aa  .....C..........
-0000eb30: e023 0091 38f1 ff97 0300 0014 0100 0014  .#..8...........
+0000e820: 5c63 2b94 550a 00b4 88a6 40f9 197d 159b  \c+.U.....@..}..
+0000e830: 00c1 221e 285b 0090 0151 42fd 0008 611e  ..".([...QB...a.
+0000e840: 0008 611e 0008 611e 1600 789e 95e2 0391  ..a...a...x.....
+0000e850: 5c63 2b94 1600 168b f77e 8ad2 77bc b4f2  \c+......~..w...
+0000e860: 7793 d8f2 1704 e0f2 187d 8052 3a81 95d2  w........}.R:...
+0000e870: 9a43 abf2 9a6c c7f2 fafb fff2 8896 40f9  .C...l........@.
+0000e880: 1f01 19eb 8205 0054 4a61 2b94 4005 0035  .......TJa+.@..5
+0000e890: 4c63 2b94 1f00 16eb 4a04 0054 4963 2b94  Lc+.....J..TIc+.
+0000e8a0: db02 00cb 7f07 00f1 6b03 0054 4563 2b94  ........k..TEc+.
+0000e8b0: 4763 2b94 e000 00b4 1f04 00f1 eb00 0054  Gc+............T
+0000e8c0: 1f00 17eb 2901 0054 0800 f092 0800 0014  ....)..T........
+0000e8d0: 0800 80d2 0600 0014 1f00 1aeb 6200 0054  ............b..T
+0000e8e0: 0800 f0d2 0700 0014 087c 189b 69fb 40d2  .........|..i.@.
+0000e8f0: 1f01 09eb 6d00 0054 0200 f092 0200 0014  ....m..T........
+0000e900: 0201 1b8b e163 0191 e003 15aa 0363 2b94  .....c.......c+.
+0000e910: 2c63 2b94 2b63 2b94 1f00 16eb 0bfb ff54  ,c+.+c+........T
+0000e920: 8896 40f9 1f01 19eb 6200 0054 2161 2b94  ..@.....b..T!a+.
+0000e930: 400b 0034 1f61 2b94 e001 0034 ff03 0139  @..4.a+....4...9
+0000e940: c864 00d0 08d1 43f9 e807 00f9 0901 40f9  .d....C.......@.
+0000e950: 2905 0091 0901 00f9 e003 0191 e123 0091  )............#..
+0000e960: e803 13aa 7e00 0094 5700 0014 9996 40f9  ....~...W.....@.
+0000e970: d907 00b4 36fb 7fd3 3f03 00f1 c0a2 9fda  ....6...?.......
+0000e980: 6a63 2b94 f503 00aa 97a2 0491 989e 40f9  jc+...........@.
+0000e990: e103 18aa e203 16aa ba64 2b94 0107 198b  .........d+.....
+0000e9a0: 8896 40f9 0801 19cb 02f9 7fd3 e003 18aa  ..@.............
+0000e9b0: b764 2b94 8896 40f9 1601 19cb e003 17aa  .d+...@.........
+0000e9c0: e103 16aa 2200 8052 ee00 0094 9696 00f9  ...."..R........
+0000e9d0: 0200 0090 42b0 3391 e003 15aa 0100 80d2  ....B.3.........
+0000e9e0: 32b2 0094 e303 00aa 88a6 40f9 290b c89a  2.........@.)...
+0000e9f0: e923 00f9 e883 04a9 0800 8252 2800 a072  .#.........R(..r
+0000ea00: e86b 00b9 ff03 00b9 3400 8052 e203 0191  .k......4..R....
+0000ea10: e5a3 0191 e003 15aa 4100 8052 0400 80d2  ........A..R....
+0000ea20: 0600 8052 2700 8052 e1ad 0094 e007 00f9  ...R'..R........
+0000ea30: 9dad 0094 0180 40ad 0200 c03d e287 00ad  ......@....=....
+0000ea40: e003 833c f4a3 0139 e0a3 0191 e123 0091  ...<...9.....#..
+0000ea50: e803 13aa 6900 0094 e007 40f9 98ad 0094  ....i.....@.....
+0000ea60: e043 0191 1900 0014 ff03 0139 c864 00d0  .C.........9.d..
+0000ea70: 08d1 43f9 e807 00f9 0901 40f9 2905 0091  ..C.......@.)...
+0000ea80: 0901 00f9 e003 0191 e123 0091 e803 13aa  .........#......
+0000ea90: 3300 0094 0c00 0014 ff03 0139 c864 00d0  3..........9.d..
+0000eaa0: 08d1 43f9 e807 00f9 0901 40f9 2905 0091  ..C.......@.)...
+0000eab0: 0901 00f9 e003 0191 e123 0091 e803 13aa  .........#......
+0000eac0: 2700 0094 e023 0091 53f1 ff97 e883 4139  '....#..S.....A9
+0000ead0: 6800 0034 e02f 40f9 b162 2b94 fd7b 4da9  h..4./@..b+..{M.
+0000eae0: f44f 4ca9 f657 4ba9 f85f 4aa9 fa67 49a9  .OL..WK.._J..gI.
+0000eaf0: fc6f 48a9 e923 476d ff83 0391 c003 5fd6  .oH..#Gm......_.
+0000eb00: 0300 0014 0200 0014 0e00 0014 f303 00aa  ................
+0000eb10: e023 0091 0700 0014 f303 00aa e007 40f9  .#............@.
+0000eb20: 67ad 0094 0200 0014 f303 00aa e043 0191  g............C..
+0000eb30: 39f1 ff97 0400 0014 0200 0014 0100 0014  9...............
 0000eb40: f303 00aa e883 4139 6800 0034 e02f 40f9  ......A9h..4./@.
 0000eb50: 9362 2b94 e003 13aa b061 2b94 f657 bda9  .b+......a+..W..
 0000eb60: f44f 01a9 fd7b 02a9 fd83 0091 f403 01aa  .O...{..........
 0000eb70: f503 00aa f303 08aa 4000 8052 4161 2b94  ........@..RAa+.
 0000eb80: 6002 00f9 a802 4039 c964 00d0 29d9 43f9  `.....@9.d..).C.
 0000eb90: ca64 00d0 4acd 43f9 1f01 0071 4801 899a  .d..J.C....qH...
 0000eba0: 0901 40f9 2905 0091 0901 00f9 080c 00f9  ..@.)...........
@@ -716831,20 +716831,20 @@
 00af01e0: 08a8 0201 8002 0cb0 0200 8c02 e401 0000  ................
 00af01f0: 0100 0000 0000 0000 ff9b 1501 0a20 04c8  ............. ..
 00af0200: 0101 24a8 0100 0001 0000 0000 0000 0000  ..$.............
 00af0210: ff9b 2101 1600 3800 0038 0894 0101 4024  ..!...8..8....@$
 00af0220: 0000 6408 9001 016c 2c00 0001 0000 0000  ..d....l,.......
 00af0230: 0000 0000 ffff 0120 0068 0000 680c 8003  ....... .h..h...
 00af0240: 0088 010c 8403 0094 01b0 0100 00c4 0238  ...............8
-00af0250: 9403 00fc 0234 0000 ffff 014b 00b8 0100  .....4.....K....
-00af0260: 00b8 0104 e406 00dc 0204 a806 00e4 0204  ................
-00af0270: b006 0088 0310 ac06 00b8 0310 d006 00dc  ................
-00af0280: 0304 e006 00e0 0334 0000 9404 10e0 0600  .......4........
-00af0290: dc04 28c4 0600 a005 10b4 0600 9006 10a4  ..(.............
-00af02a0: 0600 a006 6000 0000 ffff 010d 0070 0000  ....`........p..
+00af0250: 9403 00fc 0234 0000 ffff 014c 00ac 0100  .....4.....L....
+00af0260: 00ac 0104 e406 00d0 0204 ac06 00d8 0204  ................
+00af0270: dc06 00fc 0210 b006 00a4 0304 e006 00a8  ................
+00af0280: 0338 0000 e003 10e0 0600 a804 28cc 0600  .8..........(...
+00af0290: ec04 10bc 0600 a805 10a8 0600 d805 10a4  ................
+00af02a0: 0600 e805 9801 0000 ffff 010d 0070 0000  .............p..
 00af02b0: 7008 8801 0078 2400 0000 0000 ffff 010d  p....x$.........
 00af02c0: 0070 0000 700c 8c01 007c 2400 0000 0000  .p..p....|$.....
 00af02d0: ffff 0108 1808 6000 2048 0000 ffff 0114  ......`. H......
 00af02e0: 3c08 8002 0044 10d8 0100 6408 c001 006c  <....D....d....l
 00af02f0: a401 0000 ff9b 2901 1f3c 08c0 0100 4808  ......)..<....H.
 00af0300: b001 0064 08a8 0100 7408 a401 0184 010c  ...d....t.......
 00af0310: ac01 0090 017c 0000 0100 0000 0000 0000  .....|..........
@@ -890970,17 +890970,17 @@
 00d98590: 0000 0014 fade 0c02 0001 b39a 0002 0400  ................
 00d985a0: 0002 0002 0000 007a 0000 0058 0000 0000  .......z...X....
 00d985b0: 0000 0d99 00d9 8580 2002 000c 0000 0000  ........ .......
 00d985c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00d985d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00d985e0: 00ad f950 0000 0000 0000 0000 736f 7261  ...P........sora
 00d985f0: 5f73 646b 5f65 7874 2e63 7079 7468 6f6e  _sdk_ext.cpython
-00d98600: 2d33 382d 6461 7277 696e 2e73 6f00 a1f7  -38-darwin.so...
-00d98610: 7743 ff5d 4a26 3d37 0015 5cfb b526 0ddd  wC.]J&=7..\..&..
-00d98620: 0c08 bc60 ccc6 8956 8904 885b 130d 9eb8  ...`...V...[....
+00d98600: 2d33 382d 6461 7277 696e 2e73 6f00 7c55  -38-darwin.so.|U
+00d98610: d462 682f 2c7e e5b1 eba2 88bb d011 8e43  .bh/,~.........C
+00d98620: 5bc6 ba35 8115 bd00 b37e d7f4 3cb7 9eb8  [..5.....~..<...
 00d98630: 98f9 3981 cbff cabb eb57 563b c325 9e97  ..9......WV;.%..
 00d98640: 7d8e c084 3a43 afb3 0f48 5779 60d9 ad7f  }...:C...HWy`...
 00d98650: acb2 586f c6e9 66c0 04d7 d1d1 6b02 4f58  ..Xo..f.....k.OX
 00d98660: 05ff 7cb4 7c7a 85da bd8b 4889 2ca7 ad7f  ..|.|z....H.,...
 00d98670: acb2 586f c6e9 66c0 04d7 d1d1 6b02 4f58  ..Xo..f.....k.OX
 00d98680: 05ff 7cb4 7c7a 85da bd8b 4889 2ca7 ad7f  ..|.|z....H.,...
 00d98690: acb2 586f c6e9 66c0 04d7 d1d1 6b02 4f58  ..Xo..f.....k.OX
@@ -890998,17 +890998,17 @@
 00d98750: 20c4 d5dc 3d0d 9f8d 556b bc56 bdbb db1c   ...=...Uk.V....
 00d98760: 94fd ba56 d2a6 8a28 0073 93d2 511e e50c  ...V...(.s..Q...
 00d98770: 8f85 91bd 5bd1 1074 d74c c229 c8ad 6c5b  ....[..t.L.)..l[
 00d98780: 3056 5c04 e3fa a472 76e7 23e7 eac9 35b7  0V\....rv.#...5.
 00d98790: da4b 16e3 3e81 8f51 16f8 6fa5 fd32 f291  .K..>..Q..o..2..
 00d987a0: ac9e c700 aebe a791 900c e1fb 0e1e 11fd  ................
 00d987b0: daf5 348a 5a9d 41b8 af64 5518 69cc e8bd  ..4.Z.A..dU.i...
-00d987c0: 16ad 3668 8be9 63e3 6f1d 006b 741c da1b  ..6h..c.o..kt...
-00d987d0: 5455 ad59 2599 f50e 6b8a d253 6f1a f18f  TU.Y%...k..So...
-00d987e0: 1760 c34d 5761 1d76 e123 ed25 fdc0 f58c  .`.MWa.v.#.%....
+00d987c0: 16ad 3668 8be9 63e3 6f1d 006b 741c d175  ..6h..c.o..kt..u
+00d987d0: 212d dad0 b729 d037 d0b5 9da0 cb3d f252  !-...).7.....=.R
+00d987e0: b183 7944 9912 544b 4adb dea9 387d f58c  ..yD..TKJ...8}..
 00d987f0: 557b 4299 ad33 70aa c27f e571 26b2 0598  U{B..3p....q&...
 00d98800: 1620 61d8 3ae9 45e6 45e3 35aa 1f32 1219  . a.:.E.E.5..2..
 00d98810: a5d8 0a29 f706 49fa dc05 cecf 2983 6c95  ...)..I.....).l.
 00d98820: a772 0141 ecd3 44b8 6934 4b71 030b f959  .r.A..D.i4Kq...Y
 00d98830: c3f9 702f 5642 975b 71b7 f669 b12b 1032  ..p/VB.[q..i.+.2
 00d98840: c074 f530 6c95 f9f4 b260 c711 adcc c728  .t.0l....`.....(
 00d98850: 7165 58b6 5b34 e9c6 6ebb 034e 4ca1 2726  qeX.[4..n..NL.'&
@@ -896570,17 +896570,17 @@
 00dae390: 334b 8ae0 310a 0581 de6d 95d6 7c81 ae87  3K..1....m..|...
 00dae3a0: 9aef dafd 5122 0cc7 2eb4 eee0 ed8d 9f40  ....Q".........@
 00dae3b0: e7b6 5519 f37c 5f29 8a73 2bb4 e4f5 4700  ..U..|_).s+...G.
 00dae3c0: 122b 89f7 dd8a 2db2 314b eed6 88df cb00  .+....-.1K......
 00dae3d0: 6354 c291 cf4c 41d1 effa bd06 33b8 5053  cT...LA.....3.PS
 00dae3e0: 8a35 32a1 d3f0 85fd aed9 e84f 90f2 fad6  .52........O....
 00dae3f0: 3a48 c002 19d6 e576 3271 5ac0 30ee aa2c  :H.....v2qZ.0..,
-00dae400: 0cc4 62d9 03cb 1aec b000 6aec eb87 2b24  ..b.......j...+$
-00dae410: 0a9a 39e0 d9c4 3c7d 83e4 792f dbba 5c7a  ..9...<}..y/..\z
-00dae420: 0647 c787 12de 94a7 decf 954f d8fc 60b1  .G.........O..`.
+00dae400: 0cc4 62d9 03cb 1aec b000 6aec eb87 4461  ..b.......j...Da
+00dae410: 4ede 5565 ff4f 5507 67d1 cd66 edd1 0538  N.Ue.OU.g..f...8
+00dae420: 30d3 a0e1 2bf5 38b7 60d6 14fe bd0e 60b1  0...+.8.`.....`.
 00dae430: b849 e6fc 08f0 9590 be83 def6 473c c945  .I..........G<.E
 00dae440: 851b 1a2f 1d32 8b34 de63 7278 3782 e206  .../.2.4.crx7...
 00dae450: dfd3 f722 a90a 9824 aa51 12d3 6dd4 b7a0  ..."...$.Q..m...
 00dae460: 8c73 89bc 5374 c78e 756c 75f4 42ec bcf3  .s..St..ulu.B...
 00dae470: 67b5 8aa4 c7ed a3fd 2ea7 23e5 b3f3 ee11  g.........#.....
 00dae480: fb6a 08c4 c124 69a1 8f9c 171f 3a8b 86f0  .j...$i.....:...
 00dae490: 3212 2a4b 5339 ec66 6e03 68ee be9f 34e4  2.*KS9.fn.h...4.
```

### Comparing `sora_sdk-2024.3.0.dev0/src/sora_sdk.egg-info/PKG-INFO` & `sora_sdk-2024.3.0.dev1/src/sora_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sora_sdk
-Version: 2024.3.0.dev0
+Version: 2024.3.0.dev1
 Summary: WebRTC SFU Sora Python SDK
 Home-page: https://github.com/shiguredo/sora-python-sdk
 Author-email: "Shiguredo Inc." <contact+pypi@shiguredo.jp>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -241,15 +241,15 @@
 
 ## ドキュメント
 
 [Sora Python SDK](https://sora-python-sdk.shiguredo.jp/)
 
 ## サンプル集
 
-[examples](examples)を参照してください。
+[examples](examples) を参照してください。
 
 ## sora_sdk パッケージの追加
 
 ### pip
 
 ```console
 $ pip install sora_sdk
@@ -296,14 +296,15 @@
 - Intel VPL H.265 対応
   - [アダワープジャパン株式会社](https://adawarp.com/) 様
 
 ### 優先実装が可能な機能一覧
 
 **詳細は Discord やメールなどでお気軽にお問い合わせください**
 
+- Ubuntu 24.04 x86_64
 - Ubuntu 22.04 arm64
   - Python 3.10
   - NVIDIA Jetson JetPack SDK 6.0
 
 ## サポートについて
 
 ### Discord
```

### Comparing `sora_sdk-2024.3.0.dev0/tests/test_recvonly.py` & `sora_sdk-2024.3.0.dev1/tests/test_recvonly.py`

 * *Files identical despite different names*

