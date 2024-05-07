# Comparing `tmp/windows_capture-1.0.62.tar.gz` & `tmp/windows_capture-1.1.9.tar.gz`

## Comparing `windows_capture-1.0.62.tar` & `windows_capture-1.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      112 2024-01-05 07:54:56.000000 windows_capture-1.0.62/.github/FUNDING.yml
--rw-r--r--   0        0        0      465 2023-11-23 06:39:26.000000 windows_capture-1.0.62/.github/ISSUE_TEMPLATE/bug-report-🪲.md
--rw-r--r--   0        0        0      511 2023-11-23 06:39:26.000000 windows_capture-1.0.62/.github/ISSUE_TEMPLATE/feature-request-⭐.md
--rw-r--r--   0        0        0      514 2023-11-23 06:39:26.000000 windows_capture-1.0.62/.github/dependabot.yml
--rw-r--r--   0        0        0      393 2023-11-10 12:43:29.000000 windows_capture-1.0.62/.github/workflows/python.yml
--rw-r--r--   0        0        0      339 2023-10-28 21:42:42.000000 windows_capture-1.0.62/.github/workflows/rust.yml
--rw-r--r--   0        0        0        9 2023-10-28 21:42:42.000000 windows_capture-1.0.62/.gitignore
--rw-r--r--   0        0        0    12581 2024-03-02 12:47:16.000000 windows_capture-1.0.62/Cargo.lock
--rw-r--r--   0        0        0     1091 2023-10-28 21:42:42.000000 windows_capture-1.0.62/LICENCE
--rw-r--r--   0        0        0     5719 2024-03-02 14:55:26.000000 windows_capture-1.0.62/README.md
--rw-r--r--   0        0        0     3727 2024-03-02 14:55:32.000000 windows_capture-1.0.62/examples/basic.rs
--rw-r--r--   0        0        0       71 2023-11-09 15:15:27.000000 windows_capture-1.0.62/rust-toolchain.toml
--rw-r--r--   0        0        0      322 2024-03-02 08:19:32.000000 windows_capture-1.0.62/rustfmt.toml
--rw-r--r--   0        0        0    17161 2024-03-02 14:18:00.000000 windows_capture-1.0.62/src/capture.rs
--rw-r--r--   0        0        0     3137 2024-03-02 14:15:59.000000 windows_capture-1.0.62/src/d3d11.rs
--rw-r--r--   0        0        0    14087 2024-03-02 14:50:58.000000 windows_capture-1.0.62/src/encoder.rs
--rw-r--r--   0        0        0    14726 2024-03-02 14:35:40.000000 windows_capture-1.0.62/src/frame.rs
--rw-r--r--   0        0        0    16102 2024-03-02 14:15:44.000000 windows_capture-1.0.62/src/graphics_capture_api.rs
--rw-r--r--   0        0        0     5965 2024-03-02 14:58:19.000000 windows_capture-1.0.62/src/lib.rs
--rw-r--r--   0        0        0    15270 2024-03-02 14:15:20.000000 windows_capture-1.0.62/src/monitor.rs
--rw-r--r--   0        0        0     2499 2024-03-02 14:14:19.000000 windows_capture-1.0.62/src/settings.rs
--rw-r--r--   0        0        0     7494 2024-03-02 14:15:05.000000 windows_capture-1.0.62/src/window.rs
--rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 windows_capture-1.0.62/windows-capture-python/Cargo.toml
--rw-r--r--   0        0        0       19 2023-11-09 19:27:57.000000 windows_capture-1.0.62/windows-capture-python/.gitignore
--rw-r--r--   0        0        0     1091 2023-10-28 21:42:42.000000 windows_capture-1.0.62/windows-capture-python/LICENCE
--rw-r--r--   0        0        0     2929 2024-03-02 14:52:19.000000 windows_capture-1.0.62/windows-capture-python/README.md
--rw-r--r--   0        0        0    13305 2024-03-02 14:18:31.000000 windows_capture-1.0.62/windows-capture-python/src/lib.rs
--rw-r--r--   0        0        0     8749 2024-03-02 14:11:01.000000 windows_capture-1.0.62/windows-capture-python/windows_capture/__init__.py
--rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 windows_capture-1.0.62/Cargo.toml
--rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 windows_capture-1.0.62/pyproject.toml
--rw-r--r--   0        0        0     8749 2024-03-02 14:11:01.000000 windows_capture-1.0.62/windows_capture/__init__.py
--rw-r--r--   0        0        0     3892 1970-01-01 00:00:00.000000 windows_capture-1.0.62/PKG-INFO
+-rw-r--r--   0        0        0      112 2024-03-08 13:14:35.000000 windows_capture-1.1.9/.github/FUNDING.yml
+-rw-r--r--   0        0        0      465 2024-03-08 13:14:35.000000 windows_capture-1.1.9/.github/ISSUE_TEMPLATE/bug-report-🪲.md
+-rw-r--r--   0        0        0      511 2024-03-08 13:14:35.000000 windows_capture-1.1.9/.github/ISSUE_TEMPLATE/feature-request-⭐.md
+-rw-r--r--   0        0        0      514 2024-03-08 13:14:35.000000 windows_capture-1.1.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      393 2024-03-08 13:14:35.000000 windows_capture-1.1.9/.github/workflows/python.yml
+-rw-r--r--   0        0        0      339 2024-03-08 13:14:35.000000 windows_capture-1.1.9/.github/workflows/rust.yml
+-rw-r--r--   0        0        0        9 2024-03-08 13:14:35.000000 windows_capture-1.1.9/.gitignore
+-rw-r--r--   0        0        0    11420 2024-05-07 22:13:06.000000 windows_capture-1.1.9/Cargo.lock
+-rw-r--r--   0        0        0     1091 2024-03-08 13:14:35.000000 windows_capture-1.1.9/LICENCE
+-rw-r--r--   0        0        0     5682 2024-05-07 22:12:33.000000 windows_capture-1.1.9/README.md
+-rw-r--r--   0        0        0     3691 2024-05-04 16:54:51.000000 windows_capture-1.1.9/examples/basic.rs
+-rw-r--r--   0        0        0       71 2024-03-08 13:14:35.000000 windows_capture-1.1.9/rust-toolchain.toml
+-rw-r--r--   0        0        0      322 2024-03-08 13:14:35.000000 windows_capture-1.1.9/rustfmt.toml
+-rw-r--r--   0        0        0    17743 2024-05-07 22:11:29.000000 windows_capture-1.1.9/src/capture.rs
+-rw-r--r--   0        0        0     3234 2024-03-08 13:14:35.000000 windows_capture-1.1.9/src/d3d11.rs
+-rw-r--r--   0        0        0    22960 2024-04-21 17:14:40.000000 windows_capture-1.1.9/src/encoder.rs
+-rw-r--r--   0        0        0    14711 2024-05-04 17:06:29.000000 windows_capture-1.1.9/src/frame.rs
+-rw-r--r--   0        0        0    16102 2024-03-08 13:17:18.000000 windows_capture-1.1.9/src/graphics_capture_api.rs
+-rw-r--r--   0        0        0     6009 2024-05-07 22:12:33.000000 windows_capture-1.1.9/src/lib.rs
+-rw-r--r--   0        0        0    15349 2024-04-21 15:52:24.000000 windows_capture-1.1.9/src/monitor.rs
+-rw-r--r--   0        0        0     2030 2024-05-04 16:53:38.000000 windows_capture-1.1.9/src/settings.rs
+-rw-r--r--   0        0        0     7447 2024-04-21 15:52:15.000000 windows_capture-1.1.9/src/window.rs
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 windows_capture-1.1.9/windows-capture-python/Cargo.toml
+-rw-r--r--   0        0        0       19 2024-03-08 13:14:35.000000 windows_capture-1.1.9/windows-capture-python/.gitignore
+-rw-r--r--   0        0        0     1091 2024-03-08 13:14:35.000000 windows_capture-1.1.9/windows-capture-python/LICENCE
+-rw-r--r--   0        0        0     2929 2024-03-08 13:14:35.000000 windows_capture-1.1.9/windows-capture-python/README.md
+-rw-r--r--   0        0        0    14503 2024-05-04 16:57:40.000000 windows_capture-1.1.9/windows-capture-python/src/lib.rs
+-rw-r--r--   0        0        0     8749 2024-03-08 13:14:35.000000 windows_capture-1.1.9/windows-capture-python/windows_capture/__init__.py
+-rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 windows_capture-1.1.9/Cargo.toml
+-rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 windows_capture-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     8749 2024-03-08 13:14:35.000000 windows_capture-1.1.9/windows_capture/__init__.py
+-rw-r--r--   0        0        0     3891 1970-01-01 00:00:00.000000 windows_capture-1.1.9/PKG-INFO
```

### Comparing `windows_capture-1.0.62/.github/dependabot.yml` & `windows_capture-1.1.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `windows_capture-1.0.62/Cargo.lock` & `windows_capture-1.1.9/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -43,104 +43,104 @@
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets",
 ]
 
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -148,71 +148,71 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -222,64 +222,64 @@
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.52"
+version = "2.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
+checksum = "c993ed8ccba56ae856363b1845da7266a7cb78e1d146c8a32d54b45a8b831fc9"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.57"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
+checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.57"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
+checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -292,166 +292,140 @@
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "windows"
-version = "0.54.0"
+version = "0.56.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9252e5725dbed82865af151df558e754e4a3c2c30818359eb17465f1346a1b49"
+checksum = "1de69df01bdf1ead2f4ac895dc77c9351aefff65b2f3db429a343f9cbf05e132"
 dependencies = [
  "windows-core",
- "windows-targets 0.52.4",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-capture"
-version = "1.0.62"
+version = "1.1.9"
 dependencies = [
  "parking_lot",
  "rayon",
  "thiserror",
  "windows",
 ]
 
 [[package]]
 name = "windows-capture-python"
-version = "1.0.62"
+version = "1.1.9"
 dependencies = [
  "pyo3",
  "thiserror",
  "windows-capture",
 ]
 
 [[package]]
 name = "windows-core"
-version = "0.54.0"
+version = "0.56.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12661b9c89351d684a50a8a643ce5f608e20243b9fb84687800163429f161d65"
+checksum = "4698e52ed2d08f8658ab0c39512a7c00ee5fe2688c65f8c0a4f06750d729f2a6"
 dependencies = [
+ "windows-implement",
+ "windows-interface",
  "windows-result",
- "windows-targets 0.52.4",
+ "windows-targets",
 ]
 
 [[package]]
-name = "windows-result"
-version = "0.1.0"
+name = "windows-implement"
+version = "0.56.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd19df78e5168dfb0aedc343d1d1b8d422ab2db6756d2dc3fef75035402a3f64"
+checksum = "f6fc35f58ecd95a9b71c4f2329b911016e6bec66b3f2e6a4aad86bd2e99e2f9b"
 dependencies = [
- "windows-targets 0.52.4",
+ "proc-macro2",
+ "quote",
+ "syn",
 ]
 
 [[package]]
-name = "windows-targets"
-version = "0.48.5"
+name = "windows-interface"
+version = "0.56.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+checksum = "08990546bf4edef8f431fa6326e032865f27138718c587dc21bc0265bbcb57cc"
 dependencies = [
- "windows_aarch64_gnullvm 0.48.5",
- "windows_aarch64_msvc 0.48.5",
- "windows_i686_gnu 0.48.5",
- "windows_i686_msvc 0.48.5",
- "windows_x86_64_gnu 0.48.5",
- "windows_x86_64_gnullvm 0.48.5",
- "windows_x86_64_msvc 0.48.5",
+ "proc-macro2",
+ "quote",
+ "syn",
 ]
 
 [[package]]
-name = "windows-targets"
-version = "0.52.4"
+name = "windows-result"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "749f0da9cc72d82e600d8d2e44cadd0b9eedb9038f71a1c58556ac1c5791813b"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows-targets",
 ]
 
 [[package]]
-name = "windows_aarch64_gnullvm"
-version = "0.48.5"
+name = "windows-targets"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
+dependencies = [
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
+]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
-
-[[package]]
-name = "windows_aarch64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
-
-[[package]]
-name = "windows_i686_gnu"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
 
 [[package]]
-name = "windows_i686_msvc"
-version = "0.48.5"
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
-
-[[package]]
-name = "windows_x86_64_gnu"
-version = "0.52.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
-
-[[package]]
-name = "windows_x86_64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
```

### Comparing `windows_capture-1.0.62/LICENCE` & `windows_capture-1.1.9/LICENCE`

 * *Files identical despite different names*

### Comparing `windows_capture-1.0.62/README.md` & `windows_capture-1.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 ## Installation
 
 Add this library to your `Cargo.toml`:
 
 ```toml
 [dependencies]
-windows-capture = "1.0.62"
+windows-capture = "1.1.9"
 ```
 or run this command
 
 ```
 cargo add windows-capture
 ```
 
@@ -44,15 +44,15 @@
 
 use windows_capture::{
     capture::GraphicsCaptureApiHandler,
     encoder::{VideoEncoder, VideoEncoderQuality, VideoEncoderType},
     frame::Frame,
     graphics_capture_api::InternalCaptureControl,
     monitor::Monitor,
-    settings::{ColorFormat, CursorCaptuerSettings, DrawBorderSettings, Settings},
+    settings::{ColorFormat, CursorCaptureSettings, DrawBorderSettings, Settings},
 };
 
 // This struct will be used to handle the capture events.
 struct Capture {
     // The video encoder that will be used to encode the frames.
     encoder: Option<VideoEncoder>,
     // To measure the time the capture has been running
@@ -129,24 +129,23 @@
 fn main() {
     // Gets The Foreground Window, Checkout The Docs For Other Capture Items
     let primary_monitor = Monitor::primary().expect("There is no primary monitor");
 
     let settings = Settings::new(
         // Item To Captue
         primary_monitor,
-        // Capture Cursor
-        CursorCaptuerSettings::Default,
-        // Draw Borders (None Means Default Api Configuration)
+        // Capture Cursor Settings
+        CursorCaptureSettings::Default,
+        // Draw Borders Settings
         DrawBorderSettings::Default,
         // The desired color format for the captured frame.
         ColorFormat::Rgba8,
         // Additional flags for the capture settings that will be passed to user defined `new` function.
         "Yea This Works".to_string(),
-    )
-    .unwrap();
+    );
 
     // Starts the capture and takes control of the current thread.
     // The errors from handler trait will end up here
     Capture::start(settings).expect("Screen Capture Failed");
 }
 ```
```

### Comparing `windows_capture-1.0.62/examples/basic.rs` & `windows_capture-1.1.9/examples/basic.rs`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 use windows_capture::{
     capture::GraphicsCaptureApiHandler,
     encoder::{VideoEncoder, VideoEncoderQuality, VideoEncoderType},
     frame::Frame,
     graphics_capture_api::InternalCaptureControl,
     monitor::Monitor,
-    settings::{ColorFormat, CursorCaptuerSettings, DrawBorderSettings, Settings},
+    settings::{ColorFormat, CursorCaptureSettings, DrawBorderSettings, Settings},
 };
 
 // This struct will be used to handle the capture events.
 struct Capture {
     // The video encoder that will be used to encode the frames.
     encoder: Option<VideoEncoder>,
     // To measure the time the capture has been running
@@ -90,22 +90,21 @@
 fn main() {
     // Gets The Foreground Window, Checkout The Docs For Other Capture Items
     let primary_monitor = Monitor::primary().expect("There is no primary monitor");
 
     let settings = Settings::new(
         // Item To Captue
         primary_monitor,
-        // Capture Cursor
-        CursorCaptuerSettings::Default,
-        // Draw Borders (None Means Default Api Configuration)
+        // Capture Cursor Settings
+        CursorCaptureSettings::Default,
+        // Draw Borders Settings
         DrawBorderSettings::Default,
         // The desired color format for the captured frame.
         ColorFormat::Rgba8,
         // Additional flags for the capture settings that will be passed to user defined `new` function.
         "Yea This Works".to_string(),
-    )
-    .unwrap();
+    );
 
     // Starts the capture and takes control of the current thread.
     // The errors from handler trait will end up here
     Capture::start(settings).expect("Screen Capture Failed");
 }
```

### Comparing `windows_capture-1.0.62/src/capture.rs` & `windows_capture-1.1.9/src/capture.rs`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     },
     thread::{self, JoinHandle},
 };
 
 use parking_lot::Mutex;
 use windows::{
     Foundation::AsyncActionCompletedHandler,
+    Graphics::Capture::GraphicsCaptureItem,
     Win32::{
         Foundation::{HANDLE, LPARAM, WPARAM},
         System::{
             Threading::{GetCurrentThreadId, GetThreadId},
             WinRT::{
                 CreateDispatcherQueueController, DispatcherQueueOptions, RoInitialize,
                 RoUninitialize, DQTAT_COM_NONE, DQTYPE_THREAD_CURRENT, RO_INIT_MULTITHREADED,
@@ -183,29 +184,31 @@
 
         Ok(())
     }
 }
 
 #[derive(thiserror::Error, Eq, PartialEq, Clone, Debug)]
 pub enum GraphicsCaptureApiError<E> {
-    #[error("Failed To Join Thread")]
+    #[error("Failed to join thread")]
     FailedToJoinThread,
-    #[error("Failed To Initialize WinRT")]
+    #[error("Failed to initialize WinRT")]
     FailedToInitWinRT,
-    #[error("Failed To Create Dispatcher Queue Controller")]
+    #[error("Failed to create dispatcher queue controller")]
     FailedToCreateDispatcherQueueController,
-    #[error("Failed To Shutdown Dispatcher Queue")]
+    #[error("Failed to shutdown dispatcher queue")]
     FailedToShutdownDispatcherQueue,
-    #[error("Failed To Set Dispatcher Queue Completed Handler")]
+    #[error("Failed to set dispatcher queue completed handler")]
     FailedToSetDispatcherQueueCompletedHandler,
-    #[error("Graphics Capture Error")]
+    #[error("Failed to convert item to GraphicsCaptureItem")]
+    ItemConvertFailed,
+    #[error("Graphics capture error")]
     GraphicsCaptureApiError(graphics_capture_api::Error),
-    #[error("New Handler Error")]
+    #[error("New handler error")]
     NewHandlerError(E),
-    #[error("Frame Handler Error")]
+    #[error("Frame handler error")]
     FrameHandlerError(E),
 }
 
 /// A trait representing a graphics capture handler.
 
 pub trait GraphicsCaptureApiHandler: Sized {
     /// The type of flags used to get the values from the settings.
@@ -219,15 +222,17 @@
     /// # Arguments
     ///
     /// * `settings` - The capture settings.
     ///
     /// # Returns
     ///
     /// Returns `Ok(())` if the capture was successful, otherwise returns an error of type `GraphicsCaptureApiError`.
-    fn start(settings: Settings<Self::Flags>) -> Result<(), GraphicsCaptureApiError<Self::Error>>
+    fn start<T: TryInto<GraphicsCaptureItem>>(
+        settings: Settings<Self::Flags, T>,
+    ) -> Result<(), GraphicsCaptureApiError<Self::Error>>
     where
         Self: Send + 'static,
         <Self as GraphicsCaptureApiHandler>::Flags: Send,
     {
         // Initialize WinRT
         unsafe {
             RoInitialize(RO_INIT_MULTITHREADED)
@@ -249,16 +254,22 @@
         let thread_id = unsafe { GetCurrentThreadId() };
 
         // Start capture
         let result = Arc::new(Mutex::new(None));
         let callback = Arc::new(Mutex::new(
             Self::new(settings.flags).map_err(GraphicsCaptureApiError::NewHandlerError)?,
         ));
+
+        let item = settings
+            .item
+            .try_into()
+            .map_err(|_| GraphicsCaptureApiError::ItemConvertFailed)?;
+
         let mut capture = GraphicsCaptureApi::new(
-            settings.item,
+            item,
             callback,
             settings.cursor_capture,
             settings.draw_border,
             settings.color_format,
             thread_id,
             result.clone(),
         )
@@ -267,15 +278,15 @@
             .start_capture()
             .map_err(GraphicsCaptureApiError::GraphicsCaptureApiError)?;
 
         // Message loop
         let mut message = MSG::default();
         unsafe {
             while GetMessageW(&mut message, None, 0, 0).as_bool() {
-                TranslateMessage(&message);
+                let _ = TranslateMessage(&message);
                 DispatchMessageW(&message);
             }
         }
 
         // Shutdown dispatcher queue
         let async_action = controller
             .ShutdownQueueAsync()
@@ -289,15 +300,15 @@
             ))
             .map_err(|_| GraphicsCaptureApiError::FailedToSetDispatcherQueueCompletedHandler)?;
 
         // Final message loop
         let mut message = MSG::default();
         unsafe {
             while GetMessageW(&mut message, None, 0, 0).as_bool() {
-                TranslateMessage(&message);
+                let _ = TranslateMessage(&message);
                 DispatchMessageW(&message);
             }
         }
 
         // Stop capture
         capture.stop_capture();
 
@@ -317,16 +328,16 @@
     /// # Arguments
     ///
     /// * `settings` - The capture settings.
     ///
     /// # Returns
     ///
     /// Returns `Ok(CaptureControl)` if the capture was successful, otherwise returns an error of type `GraphicsCaptureApiError`.
-    fn start_free_threaded(
-        settings: Settings<Self::Flags>,
+    fn start_free_threaded<T: TryInto<GraphicsCaptureItem> + Send + 'static>(
+        settings: Settings<Self::Flags, T>,
     ) -> Result<CaptureControl<Self, Self::Error>, GraphicsCaptureApiError<Self::Error>>
     where
         Self: Send + 'static,
         <Self as GraphicsCaptureApiHandler>::Flags: Send,
     {
         let (halt_sender, halt_receiver) = mpsc::channel::<Arc<AtomicBool>>();
         let (callback_sender, callback_receiver) = mpsc::channel::<Arc<Mutex<Self>>>();
@@ -355,16 +366,22 @@
                 let thread_id = unsafe { GetCurrentThreadId() };
 
                 // Start capture
                 let result = Arc::new(Mutex::new(None));
                 let callback = Arc::new(Mutex::new(
                     Self::new(settings.flags).map_err(GraphicsCaptureApiError::NewHandlerError)?,
                 ));
+
+                let item = settings
+                    .item
+                    .try_into()
+                    .map_err(|_| GraphicsCaptureApiError::ItemConvertFailed)?;
+
                 let mut capture = GraphicsCaptureApi::new(
-                    settings.item,
+                    item,
                     callback.clone(),
                     settings.cursor_capture,
                     settings.draw_border,
                     settings.color_format,
                     thread_id,
                     result.clone(),
                 )
@@ -380,15 +397,15 @@
                 // Send callback
                 callback_sender.send(callback).unwrap();
 
                 // Message loop
                 let mut message = MSG::default();
                 unsafe {
                     while GetMessageW(&mut message, None, 0, 0).as_bool() {
-                        TranslateMessage(&message);
+                        let _ = TranslateMessage(&message);
                         DispatchMessageW(&message);
                     }
                 }
 
                 // Shutdown dispatcher queue
                 let async_action = controller
                     .ShutdownQueueAsync()
@@ -405,15 +422,15 @@
                         GraphicsCaptureApiError::FailedToSetDispatcherQueueCompletedHandler
                     })?;
 
                 // Final message loop
                 let mut message = MSG::default();
                 unsafe {
                     while GetMessageW(&mut message, None, 0, 0).as_bool() {
-                        TranslateMessage(&message);
+                        let _ = TranslateMessage(&message);
                         DispatchMessageW(&message);
                     }
                 }
 
                 // Stop capture
                 capture.stop_capture();
```

### Comparing `windows_capture-1.0.62/src/d3d11.rs` & `windows_capture-1.1.9/src/d3d11.rs`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-use windows::{
-    core::Interface,
-    Graphics::DirectX::Direct3D11::IDirect3DDevice,
-    Win32::{
-        Graphics::{
-            Direct3D::{
-                D3D_DRIVER_TYPE_HARDWARE, D3D_FEATURE_LEVEL, D3D_FEATURE_LEVEL_10_0,
-                D3D_FEATURE_LEVEL_10_1, D3D_FEATURE_LEVEL_11_0, D3D_FEATURE_LEVEL_11_1,
-                D3D_FEATURE_LEVEL_9_1, D3D_FEATURE_LEVEL_9_2, D3D_FEATURE_LEVEL_9_3,
-            },
-            Direct3D11::{
-                D3D11CreateDevice, ID3D11Device, ID3D11DeviceContext,
-                D3D11_CREATE_DEVICE_BGRA_SUPPORT, D3D11_SDK_VERSION,
-            },
-            Dxgi::IDXGIDevice,
-        },
-        System::WinRT::Direct3D11::CreateDirect3D11DeviceFromDXGIDevice,
-    },
-};
-
-#[derive(thiserror::Error, Eq, PartialEq, Clone, Debug)]
-pub enum Error {
-    #[error("Failed to create DirectX device with the recommended feature levels")]
-    FeatureLevelNotSatisfied,
-    #[error("Windows API Error: {0}")]
-    WindowsError(#[from] windows::core::Error),
-}
-
-/// Used To Send DirectX Device Across Threads
-pub struct SendDirectX<T>(pub T);
-
-impl<T> SendDirectX<T> {
-    /// Create A New `SendDirectX` Instance
-    ///
-    /// # Arguments
-    ///
-    /// * `device` - The DirectX Device
-    ///
-    /// # Returns
-    ///
-    /// Returns A New `SendDirectX` Instance
-    pub const fn new(device: T) -> Self {
-        Self(device)
-    }
-}
-
-#[allow(clippy::non_send_fields_in_send_ty)]
-unsafe impl<T> Send for SendDirectX<T> {}
-
-/// Create `ID3D11Device` and `ID3D11DeviceContext`
-pub fn create_d3d_device() -> Result<(ID3D11Device, ID3D11DeviceContext), Error> {
-    // Array of Direct3D feature levels.
-    // The feature levels are listed in descending order of capability.
-    // The highest feature level supported by the system is at index 0.
-    // The lowest feature level supported by the system is at the last index.
-    let feature_flags = [
-        D3D_FEATURE_LEVEL_11_1,
-        D3D_FEATURE_LEVEL_11_0,
-        D3D_FEATURE_LEVEL_10_1,
-        D3D_FEATURE_LEVEL_10_0,
-        D3D_FEATURE_LEVEL_9_3,
-        D3D_FEATURE_LEVEL_9_2,
-        D3D_FEATURE_LEVEL_9_1,
-    ];
-
-    let mut d3d_device = None;
-    let mut feature_level = D3D_FEATURE_LEVEL::default();
-    let mut d3d_device_context = None;
-    unsafe {
-        D3D11CreateDevice(
-            None,
-            D3D_DRIVER_TYPE_HARDWARE,
-            None,
-            D3D11_CREATE_DEVICE_BGRA_SUPPORT,
-            Some(&feature_flags),
-            D3D11_SDK_VERSION,
-            Some(&mut d3d_device),
-            Some(&mut feature_level),
-            Some(&mut d3d_device_context),
-        )?;
-    };
-
-    if feature_level != D3D_FEATURE_LEVEL_11_1 {
-        return Err(Error::FeatureLevelNotSatisfied);
-    }
-
-    Ok((d3d_device.unwrap(), d3d_device_context.unwrap()))
-}
-
-/// Create `IDirect3DDevice` From `ID3D11Device`
-pub fn create_direct3d_device(d3d_device: &ID3D11Device) -> Result<IDirect3DDevice, Error> {
-    let dxgi_device: IDXGIDevice = d3d_device.cast()?;
-    let inspectable = unsafe { CreateDirect3D11DeviceFromDXGIDevice(&dxgi_device)? };
-    let device: IDirect3DDevice = inspectable.cast()?;
-
-    Ok(device)
-}
+use windows::{
+    core::Interface,
+    Graphics::DirectX::Direct3D11::IDirect3DDevice,
+    Win32::{
+        Graphics::{
+            Direct3D::{
+                D3D_DRIVER_TYPE_HARDWARE, D3D_FEATURE_LEVEL, D3D_FEATURE_LEVEL_10_0,
+                D3D_FEATURE_LEVEL_10_1, D3D_FEATURE_LEVEL_11_0, D3D_FEATURE_LEVEL_11_1,
+                D3D_FEATURE_LEVEL_9_1, D3D_FEATURE_LEVEL_9_2, D3D_FEATURE_LEVEL_9_3,
+            },
+            Direct3D11::{
+                D3D11CreateDevice, ID3D11Device, ID3D11DeviceContext,
+                D3D11_CREATE_DEVICE_BGRA_SUPPORT, D3D11_SDK_VERSION,
+            },
+            Dxgi::IDXGIDevice,
+        },
+        System::WinRT::Direct3D11::CreateDirect3D11DeviceFromDXGIDevice,
+    },
+};
+
+#[derive(thiserror::Error, Eq, PartialEq, Clone, Debug)]
+pub enum Error {
+    #[error("Failed to create DirectX device with the recommended feature levels")]
+    FeatureLevelNotSatisfied,
+    #[error("Windows API Error: {0}")]
+    WindowsError(#[from] windows::core::Error),
+}
+
+/// Used To Send DirectX Device Across Threads
+pub struct SendDirectX<T>(pub T);
+
+impl<T> SendDirectX<T> {
+    /// Create A New `SendDirectX` Instance
+    ///
+    /// # Arguments
+    ///
+    /// * `device` - The DirectX Device
+    ///
+    /// # Returns
+    ///
+    /// Returns A New `SendDirectX` Instance
+    pub const fn new(device: T) -> Self {
+        Self(device)
+    }
+}
+
+#[allow(clippy::non_send_fields_in_send_ty)]
+unsafe impl<T> Send for SendDirectX<T> {}
+
+/// Create `ID3D11Device` and `ID3D11DeviceContext`
+pub fn create_d3d_device() -> Result<(ID3D11Device, ID3D11DeviceContext), Error> {
+    // Array of Direct3D feature levels.
+    // The feature levels are listed in descending order of capability.
+    // The highest feature level supported by the system is at index 0.
+    // The lowest feature level supported by the system is at the last index.
+    let feature_flags = [
+        D3D_FEATURE_LEVEL_11_1,
+        D3D_FEATURE_LEVEL_11_0,
+        D3D_FEATURE_LEVEL_10_1,
+        D3D_FEATURE_LEVEL_10_0,
+        D3D_FEATURE_LEVEL_9_3,
+        D3D_FEATURE_LEVEL_9_2,
+        D3D_FEATURE_LEVEL_9_1,
+    ];
+
+    let mut d3d_device = None;
+    let mut feature_level = D3D_FEATURE_LEVEL::default();
+    let mut d3d_device_context = None;
+    unsafe {
+        D3D11CreateDevice(
+            None,
+            D3D_DRIVER_TYPE_HARDWARE,
+            None,
+            D3D11_CREATE_DEVICE_BGRA_SUPPORT,
+            Some(&feature_flags),
+            D3D11_SDK_VERSION,
+            Some(&mut d3d_device),
+            Some(&mut feature_level),
+            Some(&mut d3d_device_context),
+        )?;
+    };
+
+    if feature_level != D3D_FEATURE_LEVEL_11_1 {
+        return Err(Error::FeatureLevelNotSatisfied);
+    }
+
+    Ok((d3d_device.unwrap(), d3d_device_context.unwrap()))
+}
+
+/// Create `IDirect3DDevice` From `ID3D11Device`
+pub fn create_direct3d_device(d3d_device: &ID3D11Device) -> Result<IDirect3DDevice, Error> {
+    let dxgi_device: IDXGIDevice = d3d_device.cast()?;
+    let inspectable = unsafe { CreateDirect3D11DeviceFromDXGIDevice(&dxgi_device)? };
+    let device: IDirect3DDevice = inspectable.cast()?;
+
+    Ok(device)
+}
```

### Comparing `windows_capture-1.0.62/src/encoder.rs` & `windows_capture-1.1.9/src/encoder.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use std::{
     fs::{self, File},
     path::Path,
+    slice,
     sync::{
         atomic::{self, AtomicBool},
         mpsc, Arc,
     },
     thread::{self, JoinHandle},
 };
 
@@ -23,17 +24,20 @@
         },
         MediaProperties::{
             MediaEncodingProfile, MediaEncodingSubtypes, VideoEncodingProperties,
             VideoEncodingQuality,
         },
         Transcoding::MediaTranscoder,
     },
+    Security::Cryptography::CryptographicBuffer,
     Storage::{
         FileAccessMode, StorageFile,
-        Streams::{Buffer, DataReader, InMemoryRandomAccessStream, InputStreamOptions},
+        Streams::{
+            Buffer, DataReader, IRandomAccessStream, InMemoryRandomAccessStream, InputStreamOptions,
+        },
     },
 };
 
 use crate::{
     d3d11::SendDirectX,
     frame::{Frame, ImageFormat},
     settings::ColorFormat,
@@ -137,15 +141,15 @@
 }
 
 #[derive(thiserror::Error, Debug)]
 pub enum VideoEncoderError {
     #[error("Windows API Error: {0}")]
     WindowsError(#[from] windows::core::Error),
     #[error("Frame send error")]
-    FrameSendError(#[from] mpsc::SendError<Option<(SendDirectX<IDirect3DSurface>, TimeSpan)>>),
+    FrameSendError(#[from] mpsc::SendError<Option<(VideoEncoderSource, TimeSpan)>>),
     #[error("IO Error: {0}")]
     IoError(#[from] std::io::Error),
 }
 
 unsafe impl Send for VideoEncoderError {}
 unsafe impl Sync for VideoEncoderError {}
 
@@ -167,18 +171,24 @@
     Pal = 5,
     Vga = 6,
     Qvga = 7,
     Uhd2160p = 8,
     Uhd4320p = 9,
 }
 
+/// The `VideoEncoderSource` struct represents all the types that can be send to the encoder.
+pub enum VideoEncoderSource {
+    DirectX(SendDirectX<IDirect3DSurface>),
+    Buffer((SendDirectX<*const u8>, usize)),
+}
+
 /// The `VideoEncoder` struct represents a video encoder that can be used to encode video frames and save them to a specified file path.
 pub struct VideoEncoder {
     first_timespan: Option<TimeSpan>,
-    frame_sender: mpsc::Sender<Option<(SendDirectX<IDirect3DSurface>, TimeSpan)>>,
+    frame_sender: mpsc::Sender<Option<(VideoEncoderSource, TimeSpan)>>,
     sample_requested: EventRegistrationToken,
     media_stream_source: MediaStreamSource,
     starting: EventRegistrationToken,
     transcode_thread: Option<JoinHandle<Result<(), VideoEncoderError>>>,
     frame_notify: Arc<(Mutex<bool>, Condvar)>,
     error_notify: Arc<AtomicBool>,
 }
@@ -231,15 +241,15 @@
         let video_stream_descriptor = VideoStreamDescriptor::Create(&video_encoding_properties)?;
 
         let media_stream_source =
             MediaStreamSource::CreateFromDescriptor(&video_stream_descriptor)?;
         media_stream_source.SetBufferTime(TimeSpan::default())?;
 
         let (frame_sender, frame_receiver) =
-            mpsc::channel::<Option<(SendDirectX<IDirect3DSurface>, TimeSpan)>>();
+            mpsc::channel::<Option<(VideoEncoderSource, TimeSpan)>>();
 
         let starting = media_stream_source.Starting(&TypedEventHandler::<
             MediaStreamSource,
             MediaStreamSourceStartingEventArgs,
         >::new(move |_, stream_start| {
             let stream_start = stream_start
                 .as_ref()
@@ -267,17 +277,30 @@
 
                 let frame = match frame_receiver.recv() {
                     Ok(frame) => frame,
                     Err(e) => panic!("Failed to receive frame from frame sender: {e}"),
                 };
 
                 match frame {
-                    Some((surface, timespan)) => {
-                        let sample =
-                            MediaStreamSample::CreateFromDirect3D11Surface(&surface.0, timespan)?;
+                    Some((source, timespan)) => {
+                        let sample = match source {
+                            VideoEncoderSource::DirectX(surface) => {
+                                MediaStreamSample::CreateFromDirect3D11Surface(
+                                    &surface.0, timespan,
+                                )?
+                            }
+                            VideoEncoderSource::Buffer(buffer_data) => {
+                                let buffer = buffer_data.0;
+                                let buffer =
+                                    unsafe { slice::from_raw_parts(buffer.0, buffer_data.1) };
+                                let buffer = CryptographicBuffer::CreateFromByteArray(buffer)?;
+                                MediaStreamSample::CreateFromBuffer(&buffer, timespan)?
+                            }
+                        };
+
                         sample_requested.Request()?.SetSample(&sample)?;
                     }
                     None => {
                         sample_requested.Request()?.SetSample(None)?;
                     }
                 }
 
@@ -336,14 +359,172 @@
             starting,
             transcode_thread: Some(transcode_thread),
             frame_notify,
             error_notify,
         })
     }
 
+    /// Creates a new `VideoEncoder` instance with the specified parameters.
+    ///
+    /// # Arguments
+    ///
+    /// * `encoder_type` - The type of video encoder to use.
+    /// * `encoder_quality` - The quality of the video encoder.
+    /// * `width` - The width of the video frames.
+    /// * `height` - The height of the video frames.
+    /// * `stream` - The stream where the encoded video will be saved.
+    ///
+    /// # Returns
+    ///
+    /// Returns a `Result` containing the `VideoEncoder` instance if successful, or a
+    /// `VideoEncoderError` if an error occurs.
+    pub fn new_from_stream<P: AsRef<Path>>(
+        encoder_type: VideoEncoderType,
+        encoder_quality: VideoEncoderQuality,
+        width: u32,
+        height: u32,
+        stream: IRandomAccessStream,
+    ) -> Result<Self, VideoEncoderError> {
+        let media_encoding_profile = match encoder_type {
+            VideoEncoderType::Avi => {
+                MediaEncodingProfile::CreateAvi(VideoEncodingQuality(encoder_quality as i32))?
+            }
+            VideoEncoderType::Hevc => {
+                MediaEncodingProfile::CreateHevc(VideoEncodingQuality(encoder_quality as i32))?
+            }
+            VideoEncoderType::Mp4 => {
+                MediaEncodingProfile::CreateMp4(VideoEncodingQuality(encoder_quality as i32))?
+            }
+            VideoEncoderType::Wmv => {
+                MediaEncodingProfile::CreateWmv(VideoEncodingQuality(encoder_quality as i32))?
+            }
+        };
+
+        let video_encoding_properties = VideoEncodingProperties::CreateUncompressed(
+            &MediaEncodingSubtypes::Bgra8()?,
+            width,
+            height,
+        )?;
+
+        let video_stream_descriptor = VideoStreamDescriptor::Create(&video_encoding_properties)?;
+
+        let media_stream_source =
+            MediaStreamSource::CreateFromDescriptor(&video_stream_descriptor)?;
+        media_stream_source.SetBufferTime(TimeSpan::default())?;
+
+        let (frame_sender, frame_receiver) =
+            mpsc::channel::<Option<(VideoEncoderSource, TimeSpan)>>();
+
+        let starting = media_stream_source.Starting(&TypedEventHandler::<
+            MediaStreamSource,
+            MediaStreamSourceStartingEventArgs,
+        >::new(move |_, stream_start| {
+            let stream_start = stream_start
+                .as_ref()
+                .expect("MediaStreamSource Starting parameter was None This Should Not Happen.");
+
+            stream_start
+                .Request()?
+                .SetActualStartPosition(TimeSpan { Duration: 0 })?;
+            Ok(())
+        }))?;
+
+        let frame_notify = Arc::new((Mutex::new(false), Condvar::new()));
+
+        let sample_requested = media_stream_source.SampleRequested(&TypedEventHandler::<
+            MediaStreamSource,
+            MediaStreamSourceSampleRequestedEventArgs,
+        >::new({
+            let frame_receiver = frame_receiver;
+            let frame_notify = frame_notify.clone();
+
+            move |_, sample_requested| {
+                let sample_requested = sample_requested.as_ref().expect(
+                    "MediaStreamSource SampleRequested parameter was None This Should Not Happen.",
+                );
+
+                let frame = match frame_receiver.recv() {
+                    Ok(frame) => frame,
+                    Err(e) => panic!("Failed to receive frame from frame sender: {e}"),
+                };
+
+                match frame {
+                    Some((source, timespan)) => {
+                        let sample = match source {
+                            VideoEncoderSource::DirectX(surface) => {
+                                MediaStreamSample::CreateFromDirect3D11Surface(
+                                    &surface.0, timespan,
+                                )?
+                            }
+                            VideoEncoderSource::Buffer(buffer_data) => {
+                                let buffer = buffer_data.0;
+                                let buffer =
+                                    unsafe { slice::from_raw_parts(buffer.0, buffer_data.1) };
+                                let buffer = CryptographicBuffer::CreateFromByteArray(buffer)?;
+                                MediaStreamSample::CreateFromBuffer(&buffer, timespan)?
+                            }
+                        };
+
+                        sample_requested.Request()?.SetSample(&sample)?;
+                    }
+                    None => {
+                        sample_requested.Request()?.SetSample(None)?;
+                    }
+                }
+
+                let (lock, cvar) = &*frame_notify;
+                *lock.lock() = true;
+                cvar.notify_one();
+
+                Ok(())
+            }
+        }))?;
+
+        let media_transcoder = MediaTranscoder::new()?;
+        media_transcoder.SetHardwareAccelerationEnabled(true)?;
+
+        let transcode = media_transcoder
+            .PrepareMediaStreamSourceTranscodeAsync(
+                &media_stream_source,
+                &stream,
+                &media_encoding_profile,
+            )?
+            .get()?;
+
+        let error_notify = Arc::new(AtomicBool::new(false));
+        let transcode_thread = thread::spawn({
+            let error_notify = error_notify.clone();
+
+            move || -> Result<(), VideoEncoderError> {
+                let result = transcode.TranscodeAsync();
+
+                if result.is_err() {
+                    error_notify.store(true, atomic::Ordering::Relaxed);
+                }
+
+                result?.get()?;
+
+                drop(media_transcoder);
+
+                Ok(())
+            }
+        });
+
+        Ok(Self {
+            first_timespan: None,
+            frame_sender,
+            sample_requested,
+            media_stream_source,
+            starting,
+            transcode_thread: Some(transcode_thread),
+            frame_notify,
+            error_notify,
+        })
+    }
+
     /// Sends a video frame to the video encoder for encoding.
     ///
     /// # Arguments
     ///
     /// * `frame` - A mutable reference to the `Frame` to be encoded.
     ///
     /// # Returns
@@ -357,18 +538,70 @@
             },
             None => {
                 let timespan = frame.timespan();
                 self.first_timespan = Some(timespan);
                 TimeSpan { Duration: 0 }
             }
         };
+        let surface = SendDirectX::new(unsafe { frame.as_raw_surface() });
+
+        self.frame_sender
+            .send(Some((VideoEncoderSource::DirectX(surface), timespan)))?;
+
+        let (lock, cvar) = &*self.frame_notify;
+        let mut processed = lock.lock();
+        if !*processed {
+            cvar.wait(&mut processed);
+        }
+        *processed = false;
+        drop(processed);
 
-        let surface = SendDirectX(unsafe { frame.as_raw_surface() });
+        if self.error_notify.load(atomic::Ordering::Relaxed) {
+            if let Some(transcode_thread) = self.transcode_thread.take() {
+                transcode_thread
+                    .join()
+                    .expect("Failed to join transcode thread")?;
+            }
+        }
+
+        Ok(())
+    }
+
+    /// Sends a video frame to the video encoder for encoding.
+    ///
+    /// # Arguments
+    ///
+    /// * `buffer` - A reference to the byte slice to be encoded Windows API expect this to be Bgra and bottom-top.
+    /// * `timespan` - The timespan that correlates to the frame buffer.
+    ///
+    /// # Returns
+    ///
+    /// Returns `Ok(())` if the frame is successfully sent for encoding, or a `VideoEncoderError`
+    /// if an error occurs.
+    pub fn send_frame_buffer(
+        &mut self,
+        buffer: &[u8],
+        timespan: i64,
+    ) -> Result<(), VideoEncoderError> {
+        let frame_timespan = timespan;
+        let timespan = match self.first_timespan {
+            Some(timespan) => TimeSpan {
+                Duration: frame_timespan - timespan.Duration,
+            },
+            None => {
+                let timespan = frame_timespan;
+                self.first_timespan = Some(TimeSpan { Duration: timespan });
+                TimeSpan { Duration: 0 }
+            }
+        };
 
-        self.frame_sender.send(Some((surface, timespan)))?;
+        self.frame_sender.send(Some((
+            VideoEncoderSource::Buffer((SendDirectX::new(buffer.as_ptr()), buffer.len())),
+            timespan,
+        )))?;
 
         let (lock, cvar) = &*self.frame_notify;
         let mut processed = lock.lock();
         if !*processed {
             cvar.wait(&mut processed);
         }
         *processed = false;
```

### Comparing `windows_capture-1.0.62/src/frame.rs` & `windows_capture-1.1.9/src/frame.rs`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     Bmp,
     JpegXr,
 }
 
 /// Represents a frame captured from a graphics capture item.
 ///
 /// # Example
-/// ```no_run
+/// ```ignore
 /// // Get frame from capture the session
 /// let mut buffer = frame.buffer()?;
 /// buffer.save_as_image("screenshot.png", ImageFormat::Png)?;
 /// ```
 pub struct Frame<'a> {
     d3d_device: &'a ID3D11Device,
     frame_surface: IDirect3DSurface,
@@ -357,15 +357,15 @@
         Ok(())
     }
 }
 
 /// Represents a frame buffer containing pixel data.
 ///
 /// # Example
-/// ```no_run
+/// ```ignore
 /// // Get frame from the capture session
 /// let mut buffer = frame.buffer()?;
 /// buffer.save_as_image("screenshot.png", ImageFormat::Png)?;
 /// ```
 pub struct FrameBuffer<'a> {
     raw_buffer: &'a mut [u8],
     buffer: &'a mut Vec<u8>,
@@ -441,24 +441,24 @@
     #[must_use]
     pub const fn has_padding(&self) -> bool {
         self.width * 4 != self.row_pitch
     }
 
     /// Get the raw pixel data with possible padding.
     #[must_use]
-    pub fn as_raw_buffer(&'a mut self) -> &'a mut [u8] {
+    pub fn as_raw_buffer(&mut self) -> &mut [u8] {
         self.raw_buffer
     }
 
     /// Get the raw pixel data without padding.
     ///
     /// # Returns
     ///
     /// A mutable reference to the buffer containing pixel data without padding.
-    pub fn as_raw_nopadding_buffer(&'a mut self) -> Result<&'a mut [u8], Error> {
+    pub fn as_raw_nopadding_buffer(&mut self) -> Result<&mut [u8], Error> {
         if !self.has_padding() {
             return Ok(self.raw_buffer);
         }
 
         let frame_size = (self.width * self.height * 4) as usize;
         if self.buffer.capacity() < frame_size {
             self.buffer.resize(frame_size, 0);
@@ -489,15 +489,15 @@
     /// * `path` - The path where the image will be saved.
     /// * `format` - The image format to use for saving.
     ///
     /// # Returns
     ///
     /// An `Ok` result if the image is successfully saved, or an `Err` result if there was an error.
     pub fn save_as_image<T: AsRef<Path>>(
-        &'a mut self,
+        &mut self,
         path: T,
         format: ImageFormat,
     ) -> Result<(), Error> {
         let width = self.width;
         let height = self.height;
 
         let bytes = ImageEncoder::new(format, self.color_format).encode(
```

### Comparing `windows_capture-1.0.62/src/graphics_capture_api.rs` & `windows_capture-1.1.9/src/graphics_capture_api.rs`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     },
 };
 
 use crate::{
     capture::GraphicsCaptureApiHandler,
     d3d11::{self, create_d3d_device, create_direct3d_device, SendDirectX},
     frame::Frame,
-    settings::{ColorFormat, CursorCaptuerSettings, DrawBorderSettings},
+    settings::{ColorFormat, CursorCaptureSettings, DrawBorderSettings},
 };
 
 #[derive(thiserror::Error, Eq, PartialEq, Clone, Debug)]
 pub enum Error {
     #[error("Graphics capture API is not supported")]
     Unsupported,
     #[error("Graphics capture API toggling cursor capture is not supported")]
@@ -112,26 +112,26 @@
     /// Returns a `Result` containing the new `GraphicsCaptureApi` struct if successful, or an `Error` if an error occurred.
     pub fn new<
         T: GraphicsCaptureApiHandler<Error = E> + Send + 'static,
         E: Send + Sync + 'static,
     >(
         item: GraphicsCaptureItem,
         callback: Arc<Mutex<T>>,
-        cursor_capture: CursorCaptuerSettings,
+        cursor_capture: CursorCaptureSettings,
         draw_border: DrawBorderSettings,
         color_format: ColorFormat,
         thread_id: u32,
         result: Arc<Mutex<Option<E>>>,
     ) -> Result<Self, Error> {
         // Check support
         if !Self::is_supported()? {
             return Err(Error::Unsupported);
         }
 
-        if cursor_capture != CursorCaptuerSettings::Default
+        if cursor_capture != CursorCaptureSettings::Default
             && !Self::is_cursor_settings_supported()?
         {
             return Err(Error::CursorConfigUnsupported);
         }
 
         if draw_border != DrawBorderSettings::Default && !Self::is_border_settings_supported()? {
             return Err(Error::BorderConfigUnsupported);
@@ -289,20 +289,20 @@
                     };
                 }
 
                 Result::Ok(())
             }
         }))?;
 
-        if cursor_capture != CursorCaptuerSettings::Default {
+        if cursor_capture != CursorCaptureSettings::Default {
             if Self::is_cursor_settings_supported()? {
                 match cursor_capture {
-                    CursorCaptuerSettings::Default => (),
-                    CursorCaptuerSettings::WithCursor => session.SetIsCursorCaptureEnabled(true)?,
-                    CursorCaptuerSettings::WithoutCursor => {
+                    CursorCaptureSettings::Default => (),
+                    CursorCaptureSettings::WithCursor => session.SetIsCursorCaptureEnabled(true)?,
+                    CursorCaptureSettings::WithoutCursor => {
                         session.SetIsCursorCaptureEnabled(false)?
                     }
                 };
             } else {
                 return Err(Error::CursorConfigUnsupported);
             }
         }
```

### Comparing `windows_capture-1.0.62/src/lib.rs` & `windows_capture-1.1.9/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 //!
 //! ## Installation
 //!
 //! Add this library to your `Cargo.toml`:
 //!
 //! ```toml
 //! [dependencies]
-//! windows-capture = "1.0.62"
+//! windows-capture = "1.1.9"
 //! ```
 //! or run this command
 //!
 //! ```text
 //! cargo add windows-capture
 //! ```
 //!
@@ -40,15 +40,15 @@
 //!
 //! use windows_capture::{
 //!     capture::GraphicsCaptureApiHandler,
 //!     encoder::{VideoEncoder, VideoEncoderQuality, VideoEncoderType},
 //!     frame::Frame,
 //!     graphics_capture_api::InternalCaptureControl,
 //!     monitor::Monitor,
-//!     settings::{ColorFormat, CursorCaptuerSettings, DrawBorderSettings, Settings},
+//!     settings::{ColorFormat, CursorCaptureSettings, DrawBorderSettings, Settings},
 //! };
 //!
 //! // This struct will be used to handle the capture events.
 //! struct Capture {
 //!     // The video encoder that will be used to encode the frames.
 //!     encoder: Option<VideoEncoder>,
 //!     // To measure the time the capture has been running
@@ -124,31 +124,31 @@
 //!
 //! // Gets The Foreground Window, Checkout The Docs For Other Capture Items
 //! let primary_monitor = Monitor::primary().expect("There is no primary monitor");
 //!
 //! let settings = Settings::new(
 //!     // Item To Captue
 //!     primary_monitor,
-//!     // Capture Cursor
-//!     CursorCaptuerSettings::Default,
-//!     // Draw Borders (None Means Default Api Configuration)
+//!     // Capture Cursor Settings
+//!     CursorCaptureSettings::Default,
+//!     // Draw Borders Settings
 //!     DrawBorderSettings::Default,
 //!     // The desired color format for the captured frame.
 //!     ColorFormat::Rgba8,
 //!     // Additional flags for the capture settings that will be passed to user defined `new` function.
 //!     "Yea This Works".to_string(),
-//! )
-//! .unwrap();
+//! );
 //!
 //! // Starts the capture and takes control of the current thread.
 //! // The errors from handler trait will end up here
 //! Capture::start(settings).expect("Screen Capture Failed");
 //! ```
 #![warn(clippy::nursery)]
 #![warn(clippy::cargo)]
+#![allow(clippy::multiple_crate_versions)] // Should update as soon as possible
 
 /// Contains the main capture functionality, including the `WindowsCaptureHandler` trait and related types.
 pub mod capture;
 /// Internal module for Direct3D 11 related functionality.
 mod d3d11;
 /// Contains the encoder functionality for encoding captured frames.
 pub mod encoder;
```

### Comparing `windows_capture-1.0.62/src/monitor.rs` & `windows_capture-1.1.9/src/monitor.rs`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
                 rcWork: RECT::default(),
                 dwFlags: 0,
             },
             szDevice: [0; 32],
         };
         if unsafe {
             !GetMonitorInfoW(
-                self.as_raw_hmonitor(),
+                HMONITOR(self.as_raw_hmonitor()),
                 std::ptr::addr_of_mut!(monitor_info).cast(),
             )
             .as_bool()
         } {
             return Err(Error::FailedToGetMonitorInfo);
         }
 
@@ -238,15 +238,15 @@
                 rcWork: RECT::default(),
                 dwFlags: 0,
             },
             szDevice: [0; 32],
         };
         if unsafe {
             !GetMonitorInfoW(
-                self.as_raw_hmonitor(),
+                HMONITOR(self.as_raw_hmonitor()),
                 std::ptr::addr_of_mut!(monitor_info).cast(),
             )
             .as_bool()
         } {
             return Err(Error::FailedToGetMonitorInfo);
         }
 
@@ -276,15 +276,15 @@
                 rcWork: RECT::default(),
                 dwFlags: 0,
             },
             szDevice: [0; 32],
         };
         if unsafe {
             !GetMonitorInfoW(
-                self.as_raw_hmonitor(),
+                HMONITOR(self.as_raw_hmonitor()),
                 std::ptr::addr_of_mut!(monitor_info).cast(),
             )
             .as_bool()
         } {
             return Err(Error::FailedToGetMonitorInfo);
         }
 
@@ -418,24 +418,26 @@
         Ok(monitors)
     }
 
     /// Creates a `Monitor` instance from a raw HMONITOR.
     ///
     /// # Arguments
     ///
-    /// * `monitor` - The raw HMONITOR.
+    /// * `hmonitor` - The raw HMONITOR.
     #[must_use]
-    pub const fn from_raw_hmonitor(monitor: HMONITOR) -> Self {
-        Self { monitor }
+    pub const fn from_raw_hmonitor(monitor: isize) -> Self {
+        Self {
+            monitor: HMONITOR(monitor),
+        }
     }
 
     /// Returns the raw HMONITOR of the monitor.
     #[must_use]
-    pub const fn as_raw_hmonitor(&self) -> HMONITOR {
-        self.monitor
+    pub const fn as_raw_hmonitor(&self) -> isize {
+        self.monitor.0
     }
 
     // Callback Used For Enumerating All Monitors
     unsafe extern "system" fn enum_monitors_callback(
         monitor: HMONITOR,
         _: HDC,
         _: *mut RECT,
@@ -450,13 +452,13 @@
 }
 
 // Implements TryFrom For Monitor To Convert It To GraphicsCaptureItem
 impl TryFrom<Monitor> for GraphicsCaptureItem {
     type Error = Error;
 
     fn try_from(value: Monitor) -> Result<Self, Self::Error> {
-        let monitor = value.as_raw_hmonitor();
+        let monitor = HMONITOR(value.as_raw_hmonitor());
 
         let interop = windows::core::factory::<Self, IGraphicsCaptureItemInterop>()?;
         Ok(unsafe { interop.CreateForMonitor(monitor)? })
     }
 }
```

### Comparing `windows_capture-1.0.62/src/settings.rs` & `windows_capture-1.1.9/src/settings.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,83 +1,70 @@
 use windows::Graphics::Capture::GraphicsCaptureItem;
 
-#[derive(thiserror::Error, Eq, PartialEq, Clone, Debug)]
-pub enum Error {
-    #[error("Failed to convert item to GraphicsCaptureItem")]
-    ItemConvertFailed,
-}
-
 #[derive(Eq, PartialEq, Clone, Copy, Debug)]
 pub enum ColorFormat {
     Rgba16F = 10,
     Rgba8 = 28,
     Bgra8 = 87,
 }
 
 impl Default for ColorFormat {
     fn default() -> Self {
         Self::Rgba8
     }
 }
 
 #[derive(Eq, PartialEq, Clone, Debug)]
-pub enum CursorCaptuerSettings {
+pub enum CursorCaptureSettings {
     Default,
     WithCursor,
     WithoutCursor,
 }
 
 #[derive(Eq, PartialEq, Clone, Debug)]
 pub enum DrawBorderSettings {
     Default,
     WithBorder,
     WithoutBorder,
 }
 
 #[derive(Eq, PartialEq, Clone, Debug)]
 /// Represents the settings for screen capturing.
-pub struct Settings<Flags> {
+pub struct Settings<Flags, T: TryInto<GraphicsCaptureItem>> {
     /// The graphics capture item to capture.
-    pub item: GraphicsCaptureItem,
+    pub item: T,
     /// Specifies whether to capture the cursor.
-    pub cursor_capture: CursorCaptuerSettings,
+    pub cursor_capture: CursorCaptureSettings,
     /// Specifies whether to draw a border around the captured region.
     pub draw_border: DrawBorderSettings,
     /// The color format for the captured graphics.
     pub color_format: ColorFormat,
     /// Additional flags for capturing graphics.
     pub flags: Flags,
 }
 
-impl<Flags> Settings<Flags> {
+impl<Flags, T: TryInto<GraphicsCaptureItem>> Settings<Flags, T> {
     /// Create Capture Settings
     ///
     /// # Arguments
     ///
     /// * `item` - The graphics capture item.
     /// * `capture_cursor` - Whether to capture the cursor or not.
     /// * `draw_border` - Whether to draw a border around the captured region or not.
     /// * `color_format` - The desired color format for the captured frame.
     /// * `flags` - Additional flags for the capture settings that will be passed to user defined `new` function.
-    ///
-    /// # Returns
-    ///
-    /// Returns a `Result` containing the `Settings` if successful, or an `Error` if conversion to `GraphicsCaptureItem` fails.
-    pub fn new<T: TryInto<GraphicsCaptureItem>>(
+    pub const fn new(
         item: T,
-        cursor_capture: CursorCaptuerSettings,
+        cursor_capture: CursorCaptureSettings,
         draw_border: DrawBorderSettings,
         color_format: ColorFormat,
         flags: Flags,
-    ) -> Result<Self, Error> {
-        Ok(Self {
-            item: match item.try_into() {
-                Ok(item) => item,
-                Err(_) => return Err(Error::ItemConvertFailed),
-            },
+    ) -> Self {
+        Self {
+            item,
             cursor_capture,
             draw_border,
             color_format,
             flags,
-        })
+        }
     }
 }
```

### Comparing `windows_capture-1.0.62/src/window.rs` & `windows_capture-1.1.9/src/window.rs`

 * *Files 3% similar despite different names*

```diff
@@ -144,44 +144,40 @@
         let window = self.window;
 
         let monitor = unsafe { MonitorFromWindow(window, MONITOR_DEFAULTTONULL) };
 
         if monitor.is_invalid() {
             None
         } else {
-            Some(Monitor::from_raw_hmonitor(monitor))
+            Some(Monitor::from_raw_hmonitor(monitor.0))
         }
     }
 
     /// Checks if the window is a valid window.
     ///
-    /// # Arguments
-    ///
-    /// * `window` - The window handle to check.
-    ///
     /// # Returns
     ///
     /// Returns `true` if the window is valid, `false` otherwise.
     #[must_use]
-    pub fn is_window_valid(window: HWND) -> bool {
-        if !unsafe { IsWindowVisible(window).as_bool() } {
+    pub fn is_valid(&self) -> bool {
+        if !unsafe { IsWindowVisible(self.window).as_bool() } {
             return false;
         }
 
         let mut id = 0;
-        unsafe { GetWindowThreadProcessId(window, Some(&mut id)) };
+        unsafe { GetWindowThreadProcessId(self.window, Some(&mut id)) };
         if id == unsafe { GetCurrentProcessId() } {
             return false;
         }
 
         let mut rect = RECT::default();
-        let result = unsafe { GetClientRect(window, &mut rect) };
+        let result = unsafe { GetClientRect(self.window, &mut rect) };
         if result.is_ok() {
-            let styles = unsafe { GetWindowLongPtrW(window, GWL_STYLE) };
-            let ex_styles = unsafe { GetWindowLongPtrW(window, GWL_EXSTYLE) };
+            let styles = unsafe { GetWindowLongPtrW(self.window, GWL_STYLE) };
+            let ex_styles = unsafe { GetWindowLongPtrW(self.window, GWL_EXSTYLE) };
 
             if (ex_styles & isize::try_from(WS_EX_TOOLWINDOW.0).unwrap()) != 0 {
                 return false;
             }
             if (styles & isize::try_from(WS_CHILD.0).unwrap()) != 0 {
                 return false;
             }
@@ -212,42 +208,42 @@
         Ok(windows)
     }
 
     /// Creates a `Window` instance from a raw HWND.
     ///
     /// # Arguments
     ///
-    /// * `window` - The raw HWND.
+    /// * `hwnd` - The raw HWND.
     #[must_use]
-    pub const fn from_raw_hwnd(window: HWND) -> Self {
-        Self { window }
+    pub const fn from_raw_hwnd(hwnd: isize) -> Self {
+        Self { window: HWND(hwnd) }
     }
 
     /// Returns the raw HWND of the window.
     #[must_use]
-    pub const fn as_raw_hwnd(&self) -> HWND {
-        self.window
+    pub const fn as_raw_hwnd(&self) -> isize {
+        self.window.0
     }
 
     // Callback used for enumerating all windows.
     unsafe extern "system" fn enum_windows_callback(window: HWND, vec: LPARAM) -> BOOL {
         let windows = &mut *(vec.0 as *mut Vec<Self>);
 
-        if Self::is_window_valid(window) {
+        if Self::from_raw_hwnd(window.0).is_valid() {
             windows.push(Self { window });
         }
 
         TRUE
     }
 }
 
 // Implements TryFrom For Window To Convert It To GraphicsCaptureItem
 impl TryFrom<Window> for GraphicsCaptureItem {
     type Error = Error;
 
     fn try_from(value: Window) -> Result<Self, Self::Error> {
-        let window = value.as_raw_hwnd();
+        let window = HWND(value.as_raw_hwnd());
 
         let interop = windows::core::factory::<Self, IGraphicsCaptureItemInterop>()?;
         Ok(unsafe { interop.CreateForWindow(window)? })
     }
 }
```

### Comparing `windows_capture-1.0.62/windows-capture-python/Cargo.toml` & `windows_capture-1.1.9/windows-capture-python/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "windows-capture-python"
-version = "1.0.62"
+version = "1.1.9"
 authors = ["NiiightmareXD"]
 edition = "2021"
 description = "Fastest Windows Screen Capture Library For Python 🔥"
 readme = "README.md"
 repository = "https://github.com/NiiightmareXD/windows-capture/tree/main/windows-capture-python"
 license = "MIT"
 keywords = ["screen", "capture", "screenshot", "graphics", "windows"]
@@ -17,13 +17,15 @@
 ]
 
 [lib]
 name = "windows_capture"
 crate-type = ["cdylib"]
 
 [dependencies]
-pyo3 = { version = "0.20.3", features = [
+pyo3 = { version = "0.21.2", features = [
     "extension-module",
     "auto-initialize",
+    "abi3",
+    "abi3-py39",
 ] }
-thiserror = "1.0.57"
+thiserror = "1.0.60"
 windows-capture = { path = ".." }
```

### Comparing `windows_capture-1.0.62/windows-capture-python/LICENCE` & `windows_capture-1.1.9/windows-capture-python/LICENCE`

 * *Files identical despite different names*

### Comparing `windows_capture-1.0.62/windows-capture-python/README.md` & `windows_capture-1.1.9/windows-capture-python/README.md`

 * *Files identical despite different names*

### Comparing `windows_capture-1.0.62/windows-capture-python/src/lib.rs` & `windows_capture-1.1.9/windows-capture-python/src/lib.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,406 +1,419 @@
-#![warn(clippy::nursery)]
-#![warn(clippy::cargo)]
-#![allow(clippy::redundant_pub_crate)]
-
-use std::sync::Arc;
-
-use ::windows_capture::{
-    capture::{
-        CaptureControl, CaptureControlError, GraphicsCaptureApiError, GraphicsCaptureApiHandler,
-    },
-    frame::{self, Frame},
-    graphics_capture_api::InternalCaptureControl,
-    monitor::Monitor,
-    settings::{ColorFormat, CursorCaptuerSettings, DrawBorderSettings, Settings},
-    window::Window,
-};
-use pyo3::{exceptions::PyException, prelude::*, types::PyList};
-
-/// Fastest Windows Screen Capture Library For Python 🔥.
-#[pymodule]
-fn windows_capture(_py: Python, m: &PyModule) -> PyResult<()> {
-    m.add_class::<NativeWindowsCapture>()?;
-    m.add_class::<NativeCaptureControl>()?;
-    Ok(())
-}
-
-/// Internal Struct Used To Handle Free Threaded Start
-#[pyclass]
-pub struct NativeCaptureControl {
-    capture_control:
-        Option<CaptureControl<InnerNativeWindowsCapture, InnerNativeWindowsCaptureError>>,
-}
-
-impl NativeCaptureControl {
-    const fn new(
-        capture_control: CaptureControl<InnerNativeWindowsCapture, InnerNativeWindowsCaptureError>,
-    ) -> Self {
-        Self {
-            capture_control: Some(capture_control),
-        }
-    }
-}
-
-#[pymethods]
-impl NativeCaptureControl {
-    #[must_use]
-    pub fn is_finished(&self) -> bool {
-        self.capture_control
-            .as_ref()
-            .map_or(true, CaptureControl::is_finished)
-    }
-
-    pub fn wait(&mut self, py: Python) -> PyResult<()> {
-        // But Honestly WTF Is This? You Know How Much Time It Took Me To Debug This?
-        // Just Why? Who Decided This BS Threading Shit?
-        py.allow_threads(|| {
-            if let Some(capture_control) = self.capture_control.take() {
-                match capture_control.wait() {
-                    Ok(()) => (),
-                    Err(e) => {
-                        if let CaptureControlError::GraphicsCaptureApiError(
-                            GraphicsCaptureApiError::FrameHandlerError(
-                                InnerNativeWindowsCaptureError::PythonError(ref e),
-                            ),
-                        ) = e
-                        {
-                            return Err(PyException::new_err(format!(
-                                "Failed To Join The Capture Thread -> {e}",
-                            )));
-                        }
-
-                        return Err(PyException::new_err(format!(
-                            "Failed To Join The Capture Thread -> {e}",
-                        )));
-                    }
-                };
-            }
-
-            Ok(())
-        })?;
-
-        Ok(())
-    }
-
-    pub fn stop(&mut self, py: Python) -> PyResult<()> {
-        // But Honestly WTF Is This? You Know How Much Time It Took Me To Debug This?
-        // Just Why? Who TF Decided This BS Threading Shit?
-        py.allow_threads(|| {
-            if let Some(capture_control) = self.capture_control.take() {
-                match capture_control.stop() {
-                    Ok(()) => (),
-                    Err(e) => {
-                        if let CaptureControlError::GraphicsCaptureApiError(
-                            GraphicsCaptureApiError::FrameHandlerError(
-                                InnerNativeWindowsCaptureError::PythonError(ref e),
-                            ),
-                        ) = e
-                        {
-                            return Err(PyException::new_err(format!(
-                                "Failed To Stop The Capture Thread -> {e}",
-                            )));
-                        }
-
-                        return Err(PyException::new_err(format!(
-                            "Failed To Stop The Capture Thread -> {e}",
-                        )));
-                    }
-                };
-            }
-
-            Ok(())
-        })?;
-
-        Ok(())
-    }
-}
-
-/// Internal Struct Used For Windows Capture
-#[pyclass]
-pub struct NativeWindowsCapture {
-    on_frame_arrived_callback: Arc<PyObject>,
-    on_closed: Arc<PyObject>,
-    cursor_capture: CursorCaptuerSettings,
-    draw_border: DrawBorderSettings,
-    monitor_index: Option<usize>,
-    window_name: Option<String>,
-}
-
-#[pymethods]
-impl NativeWindowsCapture {
-    #[new]
-    pub fn new(
-        on_frame_arrived_callback: PyObject,
-        on_closed: PyObject,
-        cursor_capture: Option<bool>,
-        draw_border: Option<bool>,
-        mut monitor_index: Option<usize>,
-        window_name: Option<String>,
-    ) -> PyResult<Self> {
-        if window_name.is_some() && monitor_index.is_some() {
-            return Err(PyException::new_err(
-                "You Can't Specify Both The Monitor Index And The Window Name",
-            ));
-        }
-
-        if window_name.is_none() && monitor_index.is_none() {
-            monitor_index = Some(1);
-        }
-
-        let cursor_capture = match cursor_capture {
-            Some(true) => CursorCaptuerSettings::WithCursor,
-            Some(false) => CursorCaptuerSettings::WithoutCursor,
-            None => CursorCaptuerSettings::Default,
-        };
-
-        let draw_border = match draw_border {
-            Some(true) => DrawBorderSettings::WithBorder,
-            Some(false) => DrawBorderSettings::WithoutBorder,
-            None => DrawBorderSettings::Default,
-        };
-
-        Ok(Self {
-            on_frame_arrived_callback: Arc::new(on_frame_arrived_callback),
-            on_closed: Arc::new(on_closed),
-            cursor_capture,
-            draw_border,
-            monitor_index,
-            window_name,
-        })
-    }
-
-    /// Start Capture
-    pub fn start(&mut self) -> PyResult<()> {
-        let settings = if self.window_name.is_some() {
-            let window = match Window::from_contains_name(self.window_name.as_ref().unwrap()) {
-                Ok(window) => window,
-                Err(e) => {
-                    return Err(PyException::new_err(format!(
-                        "Failed To Find Window -> {e}"
-                    )));
-                }
-            };
-
-            match Settings::new(
-                window,
-                self.cursor_capture.clone(),
-                self.draw_border.clone(),
-                ColorFormat::Bgra8,
-                (
-                    self.on_frame_arrived_callback.clone(),
-                    self.on_closed.clone(),
-                ),
-            ) {
-                Ok(settings) => settings,
-                Err(e) => {
-                    return Err(PyException::new_err(format!(
-                        "Failed To Create Windows Capture Settings -> {e}"
-                    )));
-                }
-            }
-        } else {
-            let monitor = match Monitor::from_index(self.monitor_index.unwrap()) {
-                Ok(monitor) => monitor,
-                Err(e) => {
-                    return Err(PyException::new_err(format!(
-                        "Failed To Get Monitor From Index -> {e}"
-                    )));
-                }
-            };
-
-            match Settings::new(
-                monitor,
-                self.cursor_capture.clone(),
-                self.draw_border.clone(),
-                ColorFormat::Bgra8,
-                (
-                    self.on_frame_arrived_callback.clone(),
-                    self.on_closed.clone(),
-                ),
-            ) {
-                Ok(settings) => settings,
-                Err(e) => {
-                    return Err(PyException::new_err(format!(
-                        "Failed To Create Windows Capture Settings -> {e}"
-                    )));
-                }
-            }
-        };
-
-        match InnerNativeWindowsCapture::start(settings) {
-            Ok(()) => (),
-            Err(e) => {
-                if let GraphicsCaptureApiError::FrameHandlerError(
-                    InnerNativeWindowsCaptureError::PythonError(ref e),
-                ) = e
-                {
-                    return Err(PyException::new_err(format!(
-                        "Capture Session Threw An Exception -> {e}",
-                    )));
-                }
-
-                return Err(PyException::new_err(format!(
-                    "Capture Session Threw An Exception -> {e}",
-                )));
-            }
-        }
-
-        Ok(())
-    }
-
-    /// Start Capture On A Dedicated Thread
-    pub fn start_free_threaded(&mut self) -> PyResult<NativeCaptureControl> {
-        let settings = if self.window_name.is_some() {
-            let window = match Window::from_contains_name(self.window_name.as_ref().unwrap()) {
-                Ok(window) => window,
-                Err(e) => {
-                    return Err(PyException::new_err(format!(
-                        "Failed To Find Window -> {e}"
-                    )));
-                }
-            };
-
-            match Settings::new(
-                window,
-                self.cursor_capture.clone(),
-                self.draw_border.clone(),
-                ColorFormat::Bgra8,
-                (
-                    self.on_frame_arrived_callback.clone(),
-                    self.on_closed.clone(),
-                ),
-            ) {
-                Ok(settings) => settings,
-                Err(e) => {
-                    return Err(PyException::new_err(format!(
-                        "Failed To Create Windows Capture Settings -> {e}"
-                    )));
-                }
-            }
-        } else {
-            let monitor = match Monitor::from_index(self.monitor_index.unwrap()) {
-                Ok(monitor) => monitor,
-                Err(e) => {
-                    return Err(PyException::new_err(format!(
-                        "Failed To Get Monitor From Index -> {e}"
-                    )));
-                }
-            };
-
-            match Settings::new(
-                monitor,
-                self.cursor_capture.clone(),
-                self.draw_border.clone(),
-                ColorFormat::Bgra8,
-                (
-                    self.on_frame_arrived_callback.clone(),
-                    self.on_closed.clone(),
-                ),
-            ) {
-                Ok(settings) => settings,
-                Err(e) => {
-                    return Err(PyException::new_err(format!(
-                        "Failed To Create Windows Capture Settings -> {e}"
-                    )));
-                }
-            }
-        };
-
-        let capture_control = match InnerNativeWindowsCapture::start_free_threaded(settings) {
-            Ok(capture_control) => capture_control,
-            Err(e) => {
-                if let GraphicsCaptureApiError::FrameHandlerError(
-                    InnerNativeWindowsCaptureError::PythonError(ref e),
-                ) = e
-                {
-                    return Err(PyException::new_err(format!(
-                        "Capture Session Threw An Exception -> {e}",
-                    )));
-                }
-
-                return Err(PyException::new_err(format!(
-                    "Capture Session Threw An Exception -> {e}",
-                )));
-            }
-        };
-
-        let capture_control = NativeCaptureControl::new(capture_control);
-
-        Ok(capture_control)
-    }
-}
-
-struct InnerNativeWindowsCapture {
-    on_frame_arrived_callback: Arc<PyObject>,
-    on_closed: Arc<PyObject>,
-}
-
-#[derive(thiserror::Error, Debug)]
-pub enum InnerNativeWindowsCaptureError {
-    #[error("Python Callback Error")]
-    PythonError(pyo3::PyErr),
-    #[error("Frame Process Error")]
-    FrameProcessError(frame::Error),
-}
-
-impl GraphicsCaptureApiHandler for InnerNativeWindowsCapture {
-    type Flags = (Arc<PyObject>, Arc<PyObject>);
-    type Error = InnerNativeWindowsCaptureError;
-
-    fn new((on_frame_arrived_callback, on_closed): Self::Flags) -> Result<Self, Self::Error> {
-        Ok(Self {
-            on_frame_arrived_callback,
-            on_closed,
-        })
-    }
-
-    fn on_frame_arrived(
-        &mut self,
-        frame: &mut Frame,
-        capture_control: InternalCaptureControl,
-    ) -> Result<(), Self::Error> {
-        let width = frame.width();
-        let height = frame.height();
-        let mut buffer = frame
-            .buffer()
-            .map_err(InnerNativeWindowsCaptureError::FrameProcessError)?;
-        let buffer = buffer.as_raw_buffer();
-
-        Python::with_gil(|py| -> Result<(), Self::Error> {
-            py.check_signals()
-                .map_err(InnerNativeWindowsCaptureError::PythonError)?;
-
-            let stop_list = PyList::new(py, [false]);
-            self.on_frame_arrived_callback
-                .call1(
-                    py,
-                    (
-                        buffer.as_ptr() as isize,
-                        buffer.len(),
-                        width,
-                        height,
-                        stop_list,
-                    ),
-                )
-                .map_err(InnerNativeWindowsCaptureError::PythonError)?;
-
-            if stop_list[0]
-                .is_true()
-                .map_err(InnerNativeWindowsCaptureError::PythonError)?
-            {
-                capture_control.stop();
-            }
-
-            Ok(())
-        })?;
-
-        Ok(())
-    }
-
-    fn on_closed(&mut self) -> Result<(), Self::Error> {
-        Python::with_gil(|py| self.on_closed.call0(py))
-            .map_err(InnerNativeWindowsCaptureError::PythonError)?;
-
-        Ok(())
-    }
-}
+#![warn(clippy::nursery)]
+#![warn(clippy::cargo)]
+#![allow(clippy::redundant_pub_crate)]
+#![allow(clippy::multiple_crate_versions)] // Should update as soon as possible
+
+use std::sync::Arc;
+
+use ::windows_capture::{
+    capture::{
+        CaptureControl, CaptureControlError, GraphicsCaptureApiError, GraphicsCaptureApiHandler,
+    },
+    frame::{self, Frame},
+    graphics_capture_api::InternalCaptureControl,
+    monitor::Monitor,
+    settings::{ColorFormat, CursorCaptureSettings, DrawBorderSettings, Settings},
+    window::Window,
+};
+use pyo3::{exceptions::PyException, prelude::*, types::PyList};
+
+/// Fastest Windows Screen Capture Library For Python 🔥.
+#[pymodule]
+fn windows_capture(m: &Bound<'_, PyModule>) -> PyResult<()> {
+    m.add_class::<NativeWindowsCapture>()?;
+    m.add_class::<NativeCaptureControl>()?;
+    Ok(())
+}
+
+/// Internal Struct Used To Handle Free Threaded Start
+#[pyclass]
+pub struct NativeCaptureControl {
+    capture_control:
+        Option<CaptureControl<InnerNativeWindowsCapture, InnerNativeWindowsCaptureError>>,
+}
+
+impl NativeCaptureControl {
+    const fn new(
+        capture_control: CaptureControl<InnerNativeWindowsCapture, InnerNativeWindowsCaptureError>,
+    ) -> Self {
+        Self {
+            capture_control: Some(capture_control),
+        }
+    }
+}
+
+#[pymethods]
+impl NativeCaptureControl {
+    #[must_use]
+    pub fn is_finished(&self) -> bool {
+        self.capture_control
+            .as_ref()
+            .map_or(true, CaptureControl::is_finished)
+    }
+
+    pub fn wait(&mut self, py: Python) -> PyResult<()> {
+        // But Honestly WTF Is This? You Know How Much Time It Took Me To Debug This?
+        // Just Why? Who Decided This BS Threading Shit?
+        py.allow_threads(|| {
+            if let Some(capture_control) = self.capture_control.take() {
+                match capture_control.wait() {
+                    Ok(()) => (),
+                    Err(e) => {
+                        if let CaptureControlError::GraphicsCaptureApiError(
+                            GraphicsCaptureApiError::FrameHandlerError(
+                                InnerNativeWindowsCaptureError::PythonError(ref e),
+                            ),
+                        ) = e
+                        {
+                            return Err(PyException::new_err(format!(
+                                "Failed To Join The Capture Thread -> {e}",
+                            )));
+                        }
+
+                        return Err(PyException::new_err(format!(
+                            "Failed To Join The Capture Thread -> {e}",
+                        )));
+                    }
+                };
+            }
+
+            Ok(())
+        })?;
+
+        Ok(())
+    }
+
+    pub fn stop(&mut self, py: Python) -> PyResult<()> {
+        // But Honestly WTF Is This? You Know How Much Time It Took Me To Debug This?
+        // Just Why? Who TF Decided This BS Threading Shit?
+        py.allow_threads(|| {
+            if let Some(capture_control) = self.capture_control.take() {
+                match capture_control.stop() {
+                    Ok(()) => (),
+                    Err(e) => {
+                        if let CaptureControlError::GraphicsCaptureApiError(
+                            GraphicsCaptureApiError::FrameHandlerError(
+                                InnerNativeWindowsCaptureError::PythonError(ref e),
+                            ),
+                        ) = e
+                        {
+                            return Err(PyException::new_err(format!(
+                                "Failed To Stop The Capture Thread -> {e}",
+                            )));
+                        }
+
+                        return Err(PyException::new_err(format!(
+                            "Failed To Stop The Capture Thread -> {e}",
+                        )));
+                    }
+                };
+            }
+
+            Ok(())
+        })?;
+
+        Ok(())
+    }
+}
+
+/// Internal Struct Used For Windows Capture
+#[pyclass]
+pub struct NativeWindowsCapture {
+    on_frame_arrived_callback: Arc<PyObject>,
+    on_closed: Arc<PyObject>,
+    cursor_capture: CursorCaptureSettings,
+    draw_border: DrawBorderSettings,
+    monitor_index: Option<usize>,
+    window_name: Option<String>,
+}
+
+#[pymethods]
+impl NativeWindowsCapture {
+    #[new]
+    pub fn new(
+        on_frame_arrived_callback: PyObject,
+        on_closed: PyObject,
+        cursor_capture: Option<bool>,
+        draw_border: Option<bool>,
+        mut monitor_index: Option<usize>,
+        window_name: Option<String>,
+    ) -> PyResult<Self> {
+        if window_name.is_some() && monitor_index.is_some() {
+            return Err(PyException::new_err(
+                "You Can't Specify Both The Monitor Index And The Window Name",
+            ));
+        }
+
+        if window_name.is_none() && monitor_index.is_none() {
+            monitor_index = Some(1);
+        }
+
+        let cursor_capture = match cursor_capture {
+            Some(true) => CursorCaptureSettings::WithCursor,
+            Some(false) => CursorCaptureSettings::WithoutCursor,
+            None => CursorCaptureSettings::Default,
+        };
+
+        let draw_border = match draw_border {
+            Some(true) => DrawBorderSettings::WithBorder,
+            Some(false) => DrawBorderSettings::WithoutBorder,
+            None => DrawBorderSettings::Default,
+        };
+
+        Ok(Self {
+            on_frame_arrived_callback: Arc::new(on_frame_arrived_callback),
+            on_closed: Arc::new(on_closed),
+            cursor_capture,
+            draw_border,
+            monitor_index,
+            window_name,
+        })
+    }
+
+    /// Start Capture
+    pub fn start(&mut self) -> PyResult<()> {
+        if self.window_name.is_some() {
+            let window = match Window::from_contains_name(self.window_name.as_ref().unwrap()) {
+                Ok(window) => window,
+                Err(e) => {
+                    return Err(PyException::new_err(format!(
+                        "Failed To Find Window -> {e}"
+                    )));
+                }
+            };
+
+            let settings = Settings::new(
+                window,
+                self.cursor_capture.clone(),
+                self.draw_border.clone(),
+                ColorFormat::Bgra8,
+                (
+                    self.on_frame_arrived_callback.clone(),
+                    self.on_closed.clone(),
+                ),
+            );
+
+            match InnerNativeWindowsCapture::start(settings) {
+                Ok(()) => (),
+                Err(e) => {
+                    if let GraphicsCaptureApiError::FrameHandlerError(
+                        InnerNativeWindowsCaptureError::PythonError(ref e),
+                    ) = e
+                    {
+                        return Err(PyException::new_err(format!(
+                            "Capture Session Threw An Exception -> {e}",
+                        )));
+                    }
+
+                    return Err(PyException::new_err(format!(
+                        "Capture Session Threw An Exception -> {e}",
+                    )));
+                }
+            }
+        } else {
+            let monitor = match Monitor::from_index(self.monitor_index.unwrap()) {
+                Ok(monitor) => monitor,
+                Err(e) => {
+                    return Err(PyException::new_err(format!(
+                        "Failed To Get Monitor From Index -> {e}"
+                    )));
+                }
+            };
+
+            let settings = Settings::new(
+                monitor,
+                self.cursor_capture.clone(),
+                self.draw_border.clone(),
+                ColorFormat::Bgra8,
+                (
+                    self.on_frame_arrived_callback.clone(),
+                    self.on_closed.clone(),
+                ),
+            );
+
+            match InnerNativeWindowsCapture::start(settings) {
+                Ok(()) => (),
+                Err(e) => {
+                    if let GraphicsCaptureApiError::FrameHandlerError(
+                        InnerNativeWindowsCaptureError::PythonError(ref e),
+                    ) = e
+                    {
+                        return Err(PyException::new_err(format!(
+                            "Capture Session Threw An Exception -> {e}",
+                        )));
+                    }
+
+                    return Err(PyException::new_err(format!(
+                        "Capture Session Threw An Exception -> {e}",
+                    )));
+                }
+            }
+        };
+
+        Ok(())
+    }
+
+    /// Start Capture On A Dedicated Thread
+    pub fn start_free_threaded(&mut self) -> PyResult<NativeCaptureControl> {
+        let capture_control = if self.window_name.is_some() {
+            let window = match Window::from_contains_name(self.window_name.as_ref().unwrap()) {
+                Ok(window) => window,
+                Err(e) => {
+                    return Err(PyException::new_err(format!(
+                        "Failed To Find Window -> {e}"
+                    )));
+                }
+            };
+
+            let settings = Settings::new(
+                window,
+                self.cursor_capture.clone(),
+                self.draw_border.clone(),
+                ColorFormat::Bgra8,
+                (
+                    self.on_frame_arrived_callback.clone(),
+                    self.on_closed.clone(),
+                ),
+            );
+
+            let capture_control = match InnerNativeWindowsCapture::start_free_threaded(settings) {
+                Ok(capture_control) => capture_control,
+                Err(e) => {
+                    if let GraphicsCaptureApiError::FrameHandlerError(
+                        InnerNativeWindowsCaptureError::PythonError(ref e),
+                    ) = e
+                    {
+                        return Err(PyException::new_err(format!(
+                            "Capture Session Threw An Exception -> {e}",
+                        )));
+                    }
+
+                    return Err(PyException::new_err(format!(
+                        "Capture Session Threw An Exception -> {e}",
+                    )));
+                }
+            };
+
+            NativeCaptureControl::new(capture_control)
+        } else {
+            let monitor = match Monitor::from_index(self.monitor_index.unwrap()) {
+                Ok(monitor) => monitor,
+                Err(e) => {
+                    return Err(PyException::new_err(format!(
+                        "Failed To Get Monitor From Index -> {e}"
+                    )));
+                }
+            };
+
+            let settings = Settings::new(
+                monitor,
+                self.cursor_capture.clone(),
+                self.draw_border.clone(),
+                ColorFormat::Bgra8,
+                (
+                    self.on_frame_arrived_callback.clone(),
+                    self.on_closed.clone(),
+                ),
+            );
+
+            let capture_control = match InnerNativeWindowsCapture::start_free_threaded(settings) {
+                Ok(capture_control) => capture_control,
+                Err(e) => {
+                    if let GraphicsCaptureApiError::FrameHandlerError(
+                        InnerNativeWindowsCaptureError::PythonError(ref e),
+                    ) = e
+                    {
+                        return Err(PyException::new_err(format!(
+                            "Capture Session Threw An Exception -> {e}",
+                        )));
+                    }
+
+                    return Err(PyException::new_err(format!(
+                        "Capture Session Threw An Exception -> {e}",
+                    )));
+                }
+            };
+
+            NativeCaptureControl::new(capture_control)
+        };
+
+        Ok(capture_control)
+    }
+}
+
+struct InnerNativeWindowsCapture {
+    on_frame_arrived_callback: Arc<PyObject>,
+    on_closed: Arc<PyObject>,
+}
+
+#[derive(thiserror::Error, Debug)]
+pub enum InnerNativeWindowsCaptureError {
+    #[error("Python Callback Error")]
+    PythonError(pyo3::PyErr),
+    #[error("Frame Process Error")]
+    FrameProcessError(frame::Error),
+}
+
+impl GraphicsCaptureApiHandler for InnerNativeWindowsCapture {
+    type Flags = (Arc<PyObject>, Arc<PyObject>);
+    type Error = InnerNativeWindowsCaptureError;
+
+    fn new((on_frame_arrived_callback, on_closed): Self::Flags) -> Result<Self, Self::Error> {
+        Ok(Self {
+            on_frame_arrived_callback,
+            on_closed,
+        })
+    }
+
+    fn on_frame_arrived(
+        &mut self,
+        frame: &mut Frame,
+        capture_control: InternalCaptureControl,
+    ) -> Result<(), Self::Error> {
+        let width = frame.width();
+        let height = frame.height();
+        let mut buffer = frame
+            .buffer()
+            .map_err(InnerNativeWindowsCaptureError::FrameProcessError)?;
+        let buffer = buffer.as_raw_buffer();
+
+        Python::with_gil(|py| -> Result<(), Self::Error> {
+            py.check_signals()
+                .map_err(InnerNativeWindowsCaptureError::PythonError)?;
+
+            let stop_list = PyList::new_bound(py, [false]);
+            self.on_frame_arrived_callback
+                .call1(
+                    py,
+                    (
+                        buffer.as_ptr() as isize,
+                        buffer.len(),
+                        width,
+                        height,
+                        stop_list.clone(),
+                    ),
+                )
+                .map_err(InnerNativeWindowsCaptureError::PythonError)?;
+
+            if stop_list
+                .get_item(0)
+                .map_err(InnerNativeWindowsCaptureError::PythonError)?
+                .is_truthy()
+                .map_err(InnerNativeWindowsCaptureError::PythonError)?
+            {
+                capture_control.stop();
+            }
+
+            Ok(())
+        })?;
+
+        Ok(())
+    }
+
+    fn on_closed(&mut self) -> Result<(), Self::Error> {
+        Python::with_gil(|py| self.on_closed.call0(py))
+            .map_err(InnerNativeWindowsCaptureError::PythonError)?;
+
+        Ok(())
+    }
+}
```

### Comparing `windows_capture-1.0.62/windows-capture-python/windows_capture/__init__.py` & `windows_capture-1.1.9/windows-capture-python/windows_capture/__init__.py`

 * *Files identical despite different names*

### Comparing `windows_capture-1.0.62/Cargo.toml` & `windows_capture-1.1.9/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "windows-capture"
-version = "1.0.62"
+version = "1.1.9"
 authors = ["NiiightmareXD"]
 edition = "2021"
 description = "Fastest Windows Screen Capture Library For Rust 🔥"
 documentation = "https://docs.rs/windows-capture"
 readme = "README.md"
 repository = "https://github.com/NiiightmareXD/windows-capture"
 license = "MIT"
@@ -16,15 +16,15 @@
     "gui",
     "multimedia",
 ]
 resolver = "2"
 
 [dependencies]
 # Windows API
-windows = { version = "0.54.0", features = [
+windows = { version = "0.56.0", features = [
     "Win32_System_WinRT_Graphics_Capture",
     "Win32_Graphics_Direct3D11",
     "Win32_Foundation",
     "Graphics_Capture",
     "Win32_System_WinRT_Direct3D11",
     "Win32_System_Threading",
     "Win32_UI_WindowsAndMessaging",
@@ -38,24 +38,25 @@
     "Storage",
     "Graphics_Imaging",
     "Storage_Streams",
     "Foundation",
     "Media_MediaProperties",
     "Media_Core",
     "Media_Transcoding",
+    "Security_Cryptography",
 ] }
 
 # Mutex optimization
-parking_lot = "0.12.1"
+parking_lot = "0.12.2"
 
 # Multithreading
-rayon = "1.8.1"
+rayon = "1.10.0"
 
 # Error handling
-thiserror = "1.0.57"
+thiserror = "1.0.60"
 
 [package.metadata.docs.rs]
 default-target = "x86_64-pc-windows-msvc"
 targets = ["x86_64-pc-windows-msvc"]
 
 [[example]]
 name = "basic"
```

### Comparing `windows_capture-1.0.62/pyproject.toml` & `windows_capture-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.3,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "windows-capture"
-version = "1.0.62"
+version = "1.1.9"
 description = "Fastest Windows Screen Capture Library For Python 🔥"
 readme = "README.md"
 requires-python = ">=3.9"
 license = "MIT"
 authors = [{ name = "NiiightmareXD" }]
 keywords = ["screen", "capture", "screenshot", "graphics", "windows"]
 dependencies = ["numpy", "opencv-python"]
```

### Comparing `windows_capture-1.0.62/windows_capture/__init__.py` & `windows_capture-1.1.9/windows_capture/__init__.py`

 * *Files identical despite different names*

### Comparing `windows_capture-1.0.62/PKG-INFO` & `windows_capture-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: windows-capture
-Version: 1.0.62
+Version: 1.1.9
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: Topic :: Multimedia
```

