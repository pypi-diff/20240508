# Comparing `tmp/hugo-0.125.6.tar.gz` & `tmp/hugo-0.125.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugo-0.125.6.tar", last modified: Sun May  5 12:10:51 2024, max compression
+gzip compressed data, was "hugo-0.125.7.tar", last modified: Wed May  8 15:17:02 2024, max compression
```

## Comparing `hugo-0.125.6.tar` & `hugo-0.125.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:10:51.836034 hugo-0.125.6/
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-05 12:10:46.000000 hugo-0.125.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 12:10:46.000000 hugo-0.125.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 12:10:46.000000 hugo-0.125.6/LICENSE-hugo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-05 12:10:46.000000 hugo-0.125.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-05-05 12:10:51.836034 hugo-0.125.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-05-05 12:10:46.000000 hugo-0.125.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-05 12:10:46.000000 hugo-0.125.6/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:10:51.832034 hugo-0.125.6/hugo/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-05 12:10:46.000000 hugo-0.125.6/hugo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:10:51.836034 hugo-0.125.6/hugo/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-05 12:10:46.000000 hugo-0.125.6/hugo/binaries/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-05 12:10:46.000000 hugo-0.125.6/hugo/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:10:51.836034 hugo-0.125.6/hugo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-05-05 12:10:51.000000 hugo-0.125.6/hugo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-05 12:10:51.000000 hugo-0.125.6/hugo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 12:10:51.000000 hugo-0.125.6/hugo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-05 12:10:51.000000 hugo-0.125.6/hugo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-05 12:10:51.000000 hugo-0.125.6/hugo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-05 12:10:46.000000 hugo-0.125.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-05 12:10:51.836034 hugo-0.125.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-05-05 12:10:46.000000 hugo-0.125.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:17:02.687770 hugo-0.125.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-08 15:16:59.000000 hugo-0.125.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 15:16:59.000000 hugo-0.125.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 15:16:59.000000 hugo-0.125.7/LICENSE-hugo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-08 15:16:59.000000 hugo-0.125.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-05-08 15:17:02.687770 hugo-0.125.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-05-08 15:16:59.000000 hugo-0.125.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-08 15:16:59.000000 hugo-0.125.7/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:17:02.683769 hugo-0.125.7/hugo/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-08 15:16:59.000000 hugo-0.125.7/hugo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:17:02.683769 hugo-0.125.7/hugo/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 15:16:59.000000 hugo-0.125.7/hugo/binaries/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-08 15:16:59.000000 hugo-0.125.7/hugo/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:17:02.683769 hugo-0.125.7/hugo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-05-08 15:17:02.000000 hugo-0.125.7/hugo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-08 15:17:02.000000 hugo-0.125.7/hugo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:17:02.000000 hugo-0.125.7/hugo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 15:17:02.000000 hugo-0.125.7/hugo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 15:17:02.000000 hugo-0.125.7/hugo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-08 15:16:59.000000 hugo-0.125.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-08 15:17:02.687770 hugo-0.125.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-05-08 15:16:59.000000 hugo-0.125.7/setup.py
```

### Comparing `hugo-0.125.6/CODE_OF_CONDUCT.md` & `hugo-0.125.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hugo-0.125.6/LICENSE` & `hugo-0.125.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hugo-0.125.6/LICENSE-hugo.txt` & `hugo-0.125.7/LICENSE-hugo.txt`

 * *Files identical despite different names*

### Comparing `hugo-0.125.6/PKG-INFO` & `hugo-0.125.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugo
-Version: 0.125.6
+Version: 0.125.7
 Summary: Binaries for the Hugo static site generator, installable with pip
 Author-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 Maintainer-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/agriyakhetarpal/hugo-python-distributions
 Project-URL: Issues, https://github.com/agriyakhetarpal/hugo-python-distributions/issues
 Project-URL: Changelog, https://github.com/agriyakhetarpal/hugo-python-distributions/releases
```

### Comparing `hugo-0.125.6/README.md` & `hugo-0.125.7/README.md`

 * *Files identical despite different names*

### Comparing `hugo-0.125.6/SECURITY.md` & `hugo-0.125.7/SECURITY.md`

 * *Files identical despite different names*

### Comparing `hugo-0.125.6/hugo/cli.py` & `hugo-0.125.7/hugo/cli.py`

 * *Files identical despite different names*

### Comparing `hugo-0.125.6/hugo.egg-info/PKG-INFO` & `hugo-0.125.7/hugo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugo
-Version: 0.125.6
+Version: 0.125.7
 Summary: Binaries for the Hugo static site generator, installable with pip
 Author-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 Maintainer-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/agriyakhetarpal/hugo-python-distributions
 Project-URL: Issues, https://github.com/agriyakhetarpal/hugo-python-distributions/issues
 Project-URL: Changelog, https://github.com/agriyakhetarpal/hugo-python-distributions/releases
```

### Comparing `hugo-0.125.6/pyproject.toml` & `hugo-0.125.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hugo-0.125.6/setup.py` & `hugo-0.125.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import Command, Extension, setup
 from setuptools.command.build_ext import build_ext
 from setuptools.command.build_py import build_py
 from wheel.bdist_wheel import bdist_wheel
 
 # ------ Hugo build configuration and constants ------------------------------------
 
-HUGO_VERSION = "0.125.6"
+HUGO_VERSION = "0.125.7"
 # The Go toolchain will download the tarball into the hugo_cache/ directory.
 # We will point the build command to that location to build Hugo from source
 HUGO_CACHE_DIR = "hugo_cache"
 FILE_EXT = (
     ".exe" if (sys.platform == "win32" or os.environ.get("GOOS") == "windows") else ""
 )
 # The vendor name is used to set the vendorInfo variable in the Hugo binary
```

