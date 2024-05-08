# Comparing `tmp/feather_tools-0.4.0.tar.gz` & `tmp/feather_tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feather_tools-0.4.0.tar", last modified: Wed May  8 17:18:17 2024, max compression
+gzip compressed data, was "feather_tools-0.5.0.tar", last modified: Wed May  8 17:26:28 2024, max compression
```

## Comparing `feather_tools-0.4.0.tar` & `feather_tools-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 17:18:17.655425 feather_tools-0.4.0/
--rw-r--r--   0 paepcke    (501) staff       (20)      256 2024-05-08 17:15:59.000000 feather_tools-0.4.0/MANIFEST.in
--rw-r--r--   0 paepcke    (501) staff       (20)     3610 2024-05-08 17:18:17.654557 feather_tools-0.4.0/PKG-INFO
--rw-r--r--   0 paepcke    (501) staff       (20)     3081 2024-05-08 17:15:59.000000 feather_tools-0.4.0/README.md
--rw-r--r--   0 paepcke    (501) staff       (20)      678 2024-05-08 17:18:03.000000 feather_tools-0.4.0/pyproject.toml
--rw-r--r--   0 paepcke    (501) staff       (20)       38 2024-05-08 17:18:17.655558 feather_tools-0.4.0/setup.cfg
-drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 17:18:17.646769 feather_tools-0.4.0/src/
-drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 17:18:17.648573 feather_tools-0.4.0/src/feather_tools/
--rw-r--r--   0 paepcke    (501) staff       (20)        0 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/__init__.py
--rw-r--r--   0 paepcke    (501) staff       (20)    21004 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/ftools_workhorse.py
-drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 17:18:17.653227 feather_tools-0.4.0/src/feather_tools/test/
--rw-r--r--   0 paepcke    (501) staff       (20)        0 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/test/__init__.py
--rwxr-xr-x   0 paepcke    (501) staff       (20)     6164 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/test/f2csv_copy.py
--rwxr-xr-x   0 paepcke    (501) staff       (20)     2727 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/test/fless_copy.py
--rwxr-xr-x   0 paepcke    (501) staff       (20)     2941 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/test/ftail_copy.py
--rwxr-xr-x   0 paepcke    (501) staff       (20)     2230 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/test/fwc_copy.py
--rw-r--r--   0 paepcke    (501) staff       (20)    27584 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/test/test_ftools_workhorse.py
-drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 17:18:17.653917 feather_tools-0.4.0/src/feather_tools.egg-info/
--rw-r--r--   0 paepcke    (501) staff       (20)     3610 2024-05-08 17:18:17.000000 feather_tools-0.4.0/src/feather_tools.egg-info/PKG-INFO
--rw-r--r--   0 paepcke    (501) staff       (20)      537 2024-05-08 17:18:17.000000 feather_tools-0.4.0/src/feather_tools.egg-info/SOURCES.txt
--rw-r--r--   0 paepcke    (501) staff       (20)        1 2024-05-08 17:18:17.000000 feather_tools-0.4.0/src/feather_tools.egg-info/dependency_links.txt
--rw-r--r--   0 paepcke    (501) staff       (20)       30 2024-05-08 17:18:17.000000 feather_tools-0.4.0/src/feather_tools.egg-info/requires.txt
--rw-r--r--   0 paepcke    (501) staff       (20)       14 2024-05-08 17:18:17.000000 feather_tools-0.4.0/src/feather_tools.egg-info/top_level.txt
+drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 17:26:28.469357 feather_tools-0.5.0/
+-rw-r--r--   0 paepcke    (501) staff       (20)      304 2024-05-08 17:24:35.000000 feather_tools-0.5.0/MANIFEST.in
+-rw-r--r--   0 paepcke    (501) staff       (20)     3610 2024-05-08 17:26:28.468510 feather_tools-0.5.0/PKG-INFO
+-rw-r--r--   0 paepcke    (501) staff       (20)     3081 2024-05-08 17:15:59.000000 feather_tools-0.5.0/README.md
+-rw-r--r--   0 paepcke    (501) staff       (20)      678 2024-05-08 17:24:48.000000 feather_tools-0.5.0/pyproject.toml
+-rw-r--r--   0 paepcke    (501) staff       (20)       38 2024-05-08 17:26:28.469522 feather_tools-0.5.0/setup.cfg
+drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 17:26:28.458757 feather_tools-0.5.0/src/
+drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 17:26:28.461758 feather_tools-0.5.0/src/feather_tools/
+-rw-r--r--   0 paepcke    (501) staff       (20)        0 2024-05-08 17:15:59.000000 feather_tools-0.5.0/src/feather_tools/__init__.py
+-rwxr-xr-x   0 paepcke    (501) staff       (20)     6164 2024-05-08 17:15:59.000000 feather_tools-0.5.0/src/feather_tools/f2csv
+-rwxr-xr-x   0 paepcke    (501) staff       (20)     2727 2024-05-08 17:15:59.000000 feather_tools-0.5.0/src/feather_tools/fless
+-rwxr-xr-x   0 paepcke    (501) staff       (20)     2941 2024-05-08 17:15:59.000000 feather_tools-0.5.0/src/feather_tools/ftail
+-rw-r--r--   0 paepcke    (501) staff       (20)    21004 2024-05-08 17:15:59.000000 feather_tools-0.5.0/src/feather_tools/ftools_workhorse.py
+-rwxr-xr-x   0 paepcke    (501) staff       (20)     2230 2024-05-08 17:15:59.000000 feather_tools-0.5.0/src/feather_tools/fwc
+drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 17:26:28.466842 feather_tools-0.5.0/src/feather_tools/test/
+-rw-r--r--   0 paepcke    (501) staff       (20)        0 2024-05-08 17:15:59.000000 feather_tools-0.5.0/src/feather_tools/test/__init__.py
+-rwxr-xr-x   0 paepcke    (501) staff       (20)     6164 2024-05-08 17:15:59.000000 feather_tools-0.5.0/src/feather_tools/test/f2csv_copy.py
+-rwxr-xr-x   0 paepcke    (501) staff       (20)     2727 2024-05-08 17:15:59.000000 feather_tools-0.5.0/src/feather_tools/test/fless_copy.py
+-rwxr-xr-x   0 paepcke    (501) staff       (20)     2941 2024-05-08 17:15:59.000000 feather_tools-0.5.0/src/feather_tools/test/ftail_copy.py
+-rwxr-xr-x   0 paepcke    (501) staff       (20)     2230 2024-05-08 17:15:59.000000 feather_tools-0.5.0/src/feather_tools/test/fwc_copy.py
+-rw-r--r--   0 paepcke    (501) staff       (20)     2698 2024-05-08 17:15:59.000000 feather_tools-0.5.0/src/feather_tools/test/simple_feather.feather
+-rw-r--r--   0 paepcke    (501) staff       (20)    27584 2024-05-08 17:15:59.000000 feather_tools-0.5.0/src/feather_tools/test/test_ftools_workhorse.py
+drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 17:26:28.467657 feather_tools-0.5.0/src/feather_tools.egg-info/
+-rw-r--r--   0 paepcke    (501) staff       (20)     3610 2024-05-08 17:26:28.000000 feather_tools-0.5.0/src/feather_tools.egg-info/PKG-INFO
+-rw-r--r--   0 paepcke    (501) staff       (20)      677 2024-05-08 17:26:28.000000 feather_tools-0.5.0/src/feather_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 paepcke    (501) staff       (20)        1 2024-05-08 17:26:28.000000 feather_tools-0.5.0/src/feather_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 paepcke    (501) staff       (20)       30 2024-05-08 17:26:28.000000 feather_tools-0.5.0/src/feather_tools.egg-info/requires.txt
+-rw-r--r--   0 paepcke    (501) staff       (20)       14 2024-05-08 17:26:28.000000 feather_tools-0.5.0/src/feather_tools.egg-info/top_level.txt
```

### Comparing `feather_tools-0.4.0/PKG-INFO` & `feather_tools-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feather_tools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Scripts to use for pyarrow feather files in a Linux terminal window
 Author-email: Andreas Paepcke <paepcke@cs.stanford.edu>
 Maintainer-email: Andreas Paepcke <paepcke@cs.stanford.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/paepcke/feather-tools
 Project-URL: Documentation, https://github.com/paepcke/feather-tools
 Requires-Python: >=3.11
```

### Comparing `feather_tools-0.4.0/README.md` & `feather_tools-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `feather_tools-0.4.0/pyproject.toml` & `feather_tools-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools >= 64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "feather_tools"
 description = "Scripts to use for pyarrow feather files in a Linux terminal window"
-version = "0.4.0"
+version = "0.5.0"
 readme  = "README.md"
 authors = [
   {name = "Andreas Paepcke", email = "paepcke@cs.stanford.edu"}
   ]
 maintainers = [
   {name = "Andreas Paepcke", email = "paepcke@cs.stanford.edu"}
   ]
```

### Comparing `feather_tools-0.4.0/src/feather_tools/ftools_workhorse.py` & `feather_tools-0.5.0/src/feather_tools/ftools_workhorse.py`

 * *Files identical despite different names*

### Comparing `feather_tools-0.4.0/src/feather_tools/test/f2csv_copy.py` & `feather_tools-0.5.0/src/feather_tools/f2csv`

 * *Files identical despite different names*

### Comparing `feather_tools-0.4.0/src/feather_tools/test/fless_copy.py` & `feather_tools-0.5.0/src/feather_tools/fless`

 * *Files identical despite different names*

### Comparing `feather_tools-0.4.0/src/feather_tools/test/ftail_copy.py` & `feather_tools-0.5.0/src/feather_tools/ftail`

 * *Files identical despite different names*

### Comparing `feather_tools-0.4.0/src/feather_tools/test/fwc_copy.py` & `feather_tools-0.5.0/src/feather_tools/fwc`

 * *Files identical despite different names*

### Comparing `feather_tools-0.4.0/src/feather_tools/test/test_ftools_workhorse.py` & `feather_tools-0.5.0/src/feather_tools/test/test_ftools_workhorse.py`

 * *Files identical despite different names*

### Comparing `feather_tools-0.4.0/src/feather_tools.egg-info/PKG-INFO` & `feather_tools-0.5.0/src/feather_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feather_tools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Scripts to use for pyarrow feather files in a Linux terminal window
 Author-email: Andreas Paepcke <paepcke@cs.stanford.edu>
 Maintainer-email: Andreas Paepcke <paepcke@cs.stanford.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/paepcke/feather-tools
 Project-URL: Documentation, https://github.com/paepcke/feather-tools
 Requires-Python: >=3.11
```

### Comparing `feather_tools-0.4.0/src/feather_tools.egg-info/SOURCES.txt` & `feather_tools-0.5.0/src/feather_tools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 MANIFEST.in
 README.md
 pyproject.toml
 src/feather_tools/__init__.py
+src/feather_tools/f2csv
+src/feather_tools/fless
+src/feather_tools/ftail
 src/feather_tools/ftools_workhorse.py
+src/feather_tools/fwc
 src/feather_tools.egg-info/PKG-INFO
 src/feather_tools.egg-info/SOURCES.txt
 src/feather_tools.egg-info/dependency_links.txt
 src/feather_tools.egg-info/requires.txt
 src/feather_tools.egg-info/top_level.txt
 src/feather_tools/test/__init__.py
 src/feather_tools/test/f2csv_copy.py
 src/feather_tools/test/fless_copy.py
 src/feather_tools/test/ftail_copy.py
 src/feather_tools/test/fwc_copy.py
+src/feather_tools/test/simple_feather.feather
 src/feather_tools/test/test_ftools_workhorse.py
```

