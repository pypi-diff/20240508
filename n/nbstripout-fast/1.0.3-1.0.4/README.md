# Comparing `tmp/nbstripout_fast-1.0.3.tar.gz` & `tmp/nbstripout_fast-1.0.4.tar.gz`

## Comparing `nbstripout_fast-1.0.3.tar` & `nbstripout_fast-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 nbstripout_fast-1.0.3/Cargo.toml
--rw-r--r--   0     1001      127       18 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/.gitattributes
--rw-r--r--   0     1001      127     1018 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/.github/workflows/test.yml
--rw-r--r--   0     1001      127     4115 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/.github/workflows/wheels.yml
--rw-r--r--   0     1001      127     3777 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/.gitignore
--rw-r--r--   0     1001      127      202 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/.pre-commit-hooks.yaml
--rw-r--r--   0     1001      127      945 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/CHANGELOG.md
--rw-r--r--   0     1001      127      406 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/CONTRIBUTING.md
--rw-r--r--   0     1001      127    16216 2024-01-01 18:17:54.000000 nbstripout_fast-1.0.3/Cargo.lock
--rw-r--r--   0     1001      127     1504 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/LICENSE.txt
--rw-r--r--   0     1001      127     4434 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/README.md
--rw-r--r--   0     1001      127      178 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/examples/.git-nbconfig.yaml
--rwxr-xr-x   0     1001      127     2014 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/examples/comparison.py
--rw-r--r--   0     1001      127     2704 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/examples/example.ipynb
--rw-r--r--   0     1001      127     1299 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/examples/example.stripped.ipynb
--rw-r--r--   0     1001      127     1479 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/src/lib.rs
--rw-r--r--   0     1001      127     9308 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/src/main.rs
--rw-r--r--   0     1001      127     7056 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/src/stripoutlib.rs
--rw-r--r--   0     1001      127     3863 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/tests/test_nbstripout_fast.py
--rw-r--r--   0     1001      127     1159 2024-01-01 18:17:32.000000 nbstripout_fast-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     5455 1970-01-01 00:00:00.000000 nbstripout_fast-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 nbstripout_fast-1.0.4/Cargo.toml
+-rw-r--r--   0     1001      127       18 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/.gitattributes
+-rw-r--r--   0     1001      127     1018 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/.github/workflows/test.yml
+-rw-r--r--   0     1001      127     4362 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/.github/workflows/wheels.yml
+-rw-r--r--   0     1001      127     3777 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/.gitignore
+-rw-r--r--   0     1001      127      202 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/.pre-commit-hooks.yaml
+-rw-r--r--   0     1001      127    10406 2024-05-08 21:13:26.000000 nbstripout_fast-1.0.4/=1.10.0
+-rw-r--r--   0     1001      127     1070 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/CHANGELOG.md
+-rw-r--r--   0     1001      127      406 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/CONTRIBUTING.md
+-rw-r--r--   0     1001      127    16891 2024-05-08 21:13:28.000000 nbstripout_fast-1.0.4/Cargo.lock
+-rw-r--r--   0     1001      127     1504 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/LICENSE.txt
+-rw-r--r--   0     1001      127     4434 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/README.md
+-rw-r--r--   0     1001      127      178 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/examples/.git-nbconfig.yaml
+-rwxr-xr-x   0     1001      127     2014 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/examples/comparison.py
+-rw-r--r--   0     1001      127     2704 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/examples/example.ipynb
+-rw-r--r--   0     1001      127     1299 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/examples/example.stripped.ipynb
+-rw-r--r--   0     1001      127     1479 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/src/lib.rs
+-rw-r--r--   0     1001      127     9358 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/src/main.rs
+-rw-r--r--   0     1001      127     7056 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/src/stripoutlib.rs
+-rw-r--r--   0     1001      127     3863 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/tests/test_nbstripout_fast.py
+-rw-r--r--   0     1001      127     1251 2024-05-08 21:13:06.000000 nbstripout_fast-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5557 1970-01-01 00:00:00.000000 nbstripout_fast-1.0.4/PKG-INFO
```

### Comparing `nbstripout_fast-1.0.3/Cargo.toml` & `nbstripout_fast-1.0.4/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nbstripout-fast"
-version = "1.0.3"
+version = "1.0.4"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nbstripout_fast"
 crate-type = ["cdylib", "rlib"]
```

### Comparing `nbstripout_fast-1.0.3/.github/workflows/test.yml` & `nbstripout_fast-1.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `nbstripout_fast-1.0.3/.github/workflows/wheels.yml` & `nbstripout_fast-1.0.4/.github/workflows/wheels.yml`

 * *Files 8% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
     - name: Set up rust cache
       uses: Swatinem/rust-cache@v2
 
     - name: Set up python
       uses: actions/setup-python@v4
       with:
-        python-version: '3.11'
+        python-version: '3.12'
 
     - name: install python dependencies
-      run: pip install -U setuptools wheel twine maturin build
+      run: pip install -U setuptools wheel twine maturin build pkginfo>=1.10.0
 
     - name: build sdist
       run: |
         python -m build --sdist -o wheelhouse
 
     - name: List and check sdist
       run: |
@@ -50,15 +50,15 @@
     name: >
       build ${{ matrix.python-version }} on ${{ matrix.platform || matrix.os }}
       ${{ (matrix.arch) || '' }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu, windows, macos]
-        python-version: ['cp311', 'cp310', 'cp39']
+        python-version: ['cp312', 'cp311', 'cp310', 'cp39']
         include:
           - os: ubuntu
             platform: linux
             pip_cache: ~/.cache/pip
           - os: windows
             ls: dir
             pip_cache: ~\AppData\Local\pip\Cache
@@ -67,15 +67,15 @@
     steps:
     - name: Check out the repo
       uses: actions/checkout@v3
 
     - name: Set up python
       uses: actions/setup-python@v4
       with:
-        python-version: '3.11'
+        python-version: '3.12'
 
     - if: matrix.os == 'macos' || matrix.os == 'windows'
       name: Set up rust toolchain
       uses: dtolnay/rust-toolchain@stable
 
     - if: matrix.os == 'macos' || matrix.os == 'windows'
       name: Set up rust cache
@@ -87,19 +87,20 @@
     - if: matrix.os == 'macos'
       name: Add aarch64-apple-darwin target
       run: rustup target add aarch64-apple-darwin
 
     - if: matrix.os == 'windows'
       name: Add i686-pc-windows-msvc target
       run: |
-        rustup toolchain install stable-i686-pc-windows-msvc
+        # Disable self-update on windows to prevent race condition; see https://github.com/rust-lang/rustup/issues/2441
+        rustup toolchain install stable-i686-pc-windows-msvc --no-self-update
         rustup target add i686-pc-windows-msvc
 
     - name: Build ${{ matrix.platform || matrix.os }} binaries
-      uses: pypa/cibuildwheel@v2.11.2
+      uses: pypa/cibuildwheel@v2.17.0
       env:
         CIBW_BUILD: '${{ matrix.python-version }}-*'
         # rust doesn't seem to be available for musl linux on i686
         CIBW_SKIP: '*-musllinux_i686'
         # we build for matrix.arch (only exists on macos), else 'auto'
         CIBW_ARCHS: ${{ matrix.arch || 'auto' }}
         CIBW_ENVIRONMENT: 'PATH="$HOME/.cargo/bin:$PATH" CARGO_TERM_COLOR="always"'
@@ -109,35 +110,39 @@
         CIBW_BEFORE_BUILD_LINUX: >
           curl https://sh.rustup.rs -sSf | sh -s -- --default-toolchain=stable --profile=minimal -y &&
           rustup show
         CIBW_BUILD_VERBOSITY: 1
 
     - name: List and check wheels
       run: |
-        pip install twine
+        pip install twine pkginfo>=1.10.0
         ${{ matrix.ls || 'ls -lh' }} wheelhouse/
         twine check wheelhouse/*
 
     - name: Upload wheels
       uses: actions/upload-artifact@v2
       with:
         name: wheels
         path: ./wheelhouse/*.whl
 
   upload_to_pypi:
     name: Upload to PYPI
     runs-on: ubuntu-latest
     if: (github.event_name == 'release' && startsWith(github.ref, 'refs/tags')) || (github.event_name == 'workflow_dispatch')
     needs: [build_wheels, build_sdist]
+    environment:
+      name: pypi
+      url: https://pypi.org/p/nbstripout-fast
+    permissions:
+      id-token: write
     steps:
       - name: Retrieve wheels and sdist
         uses: actions/download-artifact@v3
 
       - name: List the build artifacts
         run: |
           ls -lAs wheels/
 
       - name: Upload to PyPI
-        uses: pypa/gh-action-pypi-publish@release/v1.5
+        uses: pypa/gh-action-pypi-publish@release/v1.8
         with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
           packages_dir: wheels/
```

### Comparing `nbstripout_fast-1.0.3/.gitignore` & `nbstripout_fast-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nbstripout_fast-1.0.3/CHANGELOG.md` & `nbstripout_fast-1.0.4/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## [1.0.4](https://github.com/deshaw/nbstripout-fast/compare/v1.0.3...v1.0.4) (2024-05-03)
+### Fixed
+- git worktree support
+
 ## [1.0.3](https://github.com/deshaw/nbstripout-fast/compare/v1.0.2...v1.0.3) (2024-01-01)
 ### Fixed
 - maxOS Support
 
 ## [1.0.2](https://github.com/deshaw/nbstripout-fast/compare/v1.0.1...v1.0.2) (2023-09-18)
 ### Fixed
 - Do not overwrite file if contents are identical [#9](https://github.com/deshaw/nbstripout-fast/issues/9)
```

### Comparing `nbstripout_fast-1.0.3/Cargo.lock` & `nbstripout_fast-1.0.4/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "atty"
 version = "0.2.14"
@@ -20,38 +20,44 @@
  "hermit-abi",
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clap"
 version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
 dependencies = [
  "atty",
- "bitflags",
+ "bitflags 1.3.2",
  "clap_derive",
  "clap_lex",
  "indexmap 1.9.3",
  "once_cell",
  "strsim",
  "termcolor",
  "textwrap",
@@ -102,17 +108,17 @@
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
@@ -139,71 +145,71 @@
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.1.0"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d530e1a18b1cb4c484e6e34556a0d948706958449fca0cab753d649f2bce3d1f"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
- "hashbrown 0.14.3",
+ "hashbrown 0.14.5",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "libc"
-version = "0.2.151"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "302d7ab3130588088d277783b1e2d2e10c9e9e4a16dd9050e6ec93fb3e7048f4"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
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
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "nbstripout-fast"
-version = "1.0.3"
+version = "1.0.4"
 dependencies = [
  "clap",
  "env_logger",
  "log",
  "pyo3",
  "serde",
  "serde_json",
@@ -220,27 +226,27 @@
 name = "os_str_bytes"
 version = "6.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2355d85b9a3786f481747ced0e0ff2ba35213a1f9bd406ed906554d7af805a1"
 
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
  "windows-targets",
 ]
@@ -267,17 +273,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.73"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dd5e8a1f1029c43224ad5898e50140c2aebb1705f19e67c918ebf5b9e797fe1"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.16.6"
@@ -335,98 +341,98 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.34"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22a37c9326af5ed140c86a46655b5278de879853be5573c01df185b6f49a580a"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.2"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "380b951a9c5e80ddfd6136919eef32310721aa4aacd4889a8d39124b026ab343"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.3"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f804c7828047e88b2d32e2d7fe5a105da8ee3264f01902f796c8e067dc2483f"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "ryu"
-version = "1.0.16"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.193"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25dd9975e68d0cb5aa1120c288333fc98731bd1dd12f561e468ea4728c042b89"
+checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.193"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43576ca501357b9b071ac53cdc7da8ef0cbd9493d8df094cd821777ea6e894d3"
+checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.44",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.109"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb0652c533506ad7a2e353cce269330d6afd8bdfb6d75e0ace5b35aacbd7b9e9"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
- "indexmap 2.1.0",
+ "indexmap 2.2.6",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_yaml"
@@ -438,17 +444,17 @@
  "ryu",
  "serde",
  "yaml-rust",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.2"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dccd0940a2dcdf68d092b8cbab7dc0ad8fa938bf95787e1b916b0e3d0e8e970"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
@@ -461,43 +467,43 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.44"
+version = "2.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92d27c2c202598d05175a6dd3af46824b7f747f8d8e9b14c623f19fa5069735d"
+checksum = "c993ed8ccba56ae856363b1845da7266a7cb78e1d146c8a32d54b45a8b831fc9"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.12"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c39fd04924ca3a864207c66fc2cd7d22d7c016007f9ce846cbb9326331930a"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "termcolor"
-version = "1.4.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff1bc3d3f05aff0403e8ac0d92ced918ec05b666a43f83297ccef5bea8a3d449"
+checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "textwrap"
-version = "0.16.0"
+version = "0.16.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
+checksum = "23d434d3f8967a09480fb04132ebe0a3e088c173e6d0ee7897abbdf4eab0f8b9"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
@@ -527,83 +533,99 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
 name = "windows-targets"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
+ "windows_i686_gnullvm",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.5"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "yaml-rust"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56c1936c4cc7a1c9ab21a1ebb602eb942ba868cbd44a99cb7cdc5892335e1c85"
 dependencies = [
```

### Comparing `nbstripout_fast-1.0.3/LICENSE.txt` & `nbstripout_fast-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nbstripout_fast-1.0.3/README.md` & `nbstripout_fast-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nbstripout_fast-1.0.3/examples/comparison.py` & `nbstripout_fast-1.0.4/examples/comparison.py`

 * *Files identical despite different names*

### Comparing `nbstripout_fast-1.0.3/examples/example.ipynb` & `nbstripout_fast-1.0.4/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `nbstripout_fast-1.0.3/examples/example.stripped.ipynb` & `nbstripout_fast-1.0.4/examples/example.stripped.ipynb`

 * *Files identical despite different names*

### Comparing `nbstripout_fast-1.0.3/src/lib.rs` & `nbstripout_fast-1.0.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nbstripout_fast-1.0.3/src/main.rs` & `nbstripout_fast-1.0.4/src/main.rs`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,16 @@
 // TODO: Maybe this should load relative to the file
 fn find_nbconfig() -> Result<Option<NBConfig>, String> {
     let mut dir = env::current_dir().map_err(|e| format!("Unable to read current dir {:?}", e))?;
     // Find .git. We don't want too many dependencies, so we do this a bit hacky
     loop {
         let git_dir = dir.as_path().join(".git");
         log::debug!("Looking for .git in {:?}", dir);
-        if git_dir.exists() && git_dir.is_dir() {
+        // We don't check if it is a dir as worktrees use a .git file
+        if git_dir.exists() {
             let nbconfig_path = dir.join(".git-nbconfig.yaml");
             if nbconfig_path.exists() && nbconfig_path.is_file() {
                 let f = std::fs::File::open(nbconfig_path)
                     .map_err(|e| format!("Could not open .git-nbconfig.yaml, {:?}", e))?;
                 let config = serde_yaml::from_reader::<std::fs::File, NBConfig>(f)
                     .map_err(|e| format!("Could not parse .git-nbconfig.yaml: {:?}", e))?;
                 log::debug!("{:?}", config);
```

### Comparing `nbstripout_fast-1.0.3/src/stripoutlib.rs` & `nbstripout_fast-1.0.4/src/stripoutlib.rs`

 * *Files identical despite different names*

### Comparing `nbstripout_fast-1.0.3/tests/test_nbstripout_fast.py` & `nbstripout_fast-1.0.4/tests/test_nbstripout_fast.py`

 * *Files identical despite different names*

### Comparing `nbstripout_fast-1.0.3/pyproject.toml` & `nbstripout_fast-1.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     "Development Status :: 5 - Production/Stable",
     "Environment :: Other Environment",
     "Framework :: IPython",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Version Control",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 [project.urls]
 homepage = "https://github.com/deshaw/nbstripout-fast"
```

### Comparing `nbstripout_fast-1.0.3/PKG-INFO` & `nbstripout_fast-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: nbstripout-fast
-Version: 1.0.3
+Version: 1.0.4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: nbformat ; extra == 'test'
 Requires-Dist: nbconvert ; extra == 'test'
```

