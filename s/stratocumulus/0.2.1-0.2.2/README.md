# Comparing `tmp/stratocumulus-0.2.1.tar.gz` & `tmp/stratocumulus-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stratocumulus-0.2.1.tar", last modified: Tue Mar 21 21:40:24 2023, max compression
+gzip compressed data, was "stratocumulus-0.2.2.tar", last modified: Tue May  7 19:40:17 2024, max compression
```

## Comparing `stratocumulus-0.2.1.tar` & `stratocumulus-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-03-21 21:40:24.057580 stratocumulus-0.2.1/
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-03-21 21:40:24.036188 stratocumulus-0.2.1/.github/
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-03-21 21:40:24.039013 stratocumulus-0.2.1/.github/workflows/
--rw-r--r--   0 yangy197   (501) staff       (20)      703 2022-09-28 20:06:45.000000 stratocumulus-0.2.1/.github/workflows/test.yml
--rw-r--r--   0 yangy197   (501) staff       (20)     1532 2021-08-19 16:43:59.000000 stratocumulus-0.2.1/LICENSE
--rw-r--r--   0 yangy197   (501) staff       (20)       62 2021-08-19 16:43:59.000000 stratocumulus-0.2.1/MANIFEST.in
--rw-r--r--   0 yangy197   (501) staff       (20)     7137 2023-03-21 21:40:24.057002 stratocumulus-0.2.1/PKG-INFO
--rw-r--r--   0 yangy197   (501) staff       (20)     4433 2022-09-28 20:06:45.000000 stratocumulus-0.2.1/README.rst
--rw-r--r--   0 yangy197   (501) staff       (20)     1974 2023-03-21 21:30:56.000000 stratocumulus-0.2.1/pyproject.toml
--rw-r--r--   0 yangy197   (501) staff       (20)       38 2023-03-21 21:40:24.057763 stratocumulus-0.2.1/setup.cfg
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-03-21 21:40:24.041124 stratocumulus-0.2.1/strato/
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2021-11-10 17:34:26.000000 stratocumulus-0.2.1/strato/__init__.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1020 2022-09-28 20:06:45.000000 stratocumulus-0.2.1/strato/__main__.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-03-21 21:40:24.043467 stratocumulus-0.2.1/strato/backends/
--rw-r--r--   0 yangy197   (501) staff       (20)      133 2022-09-28 20:06:45.000000 stratocumulus-0.2.1/strato/backends/__init__.py
--rw-r--r--   0 yangy197   (501) staff       (20)     4524 2023-03-21 21:26:55.000000 stratocumulus-0.2.1/strato/backends/_aws.py
--rw-r--r--   0 yangy197   (501) staff       (20)     2531 2022-09-28 20:06:45.000000 stratocumulus-0.2.1/strato/backends/_gcp.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1856 2022-09-28 20:06:45.000000 stratocumulus-0.2.1/strato/backends/_local.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-03-21 21:40:24.047403 stratocumulus-0.2.1/strato/commands/
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2021-11-10 17:34:26.000000 stratocumulus-0.2.1/strato/commands/__init__.py
--rw-r--r--   0 yangy197   (501) staff       (20)     2719 2023-03-20 20:53:11.000000 stratocumulus-0.2.1/strato/commands/cp.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1360 2022-09-28 20:06:45.000000 stratocumulus-0.2.1/strato/commands/exists.py
--rw-r--r--   0 yangy197   (501) staff       (20)     2312 2022-09-28 20:06:45.000000 stratocumulus-0.2.1/strato/commands/rm.py
--rw-r--r--   0 yangy197   (501) staff       (20)     2457 2022-09-28 20:06:45.000000 stratocumulus-0.2.1/strato/commands/sync.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1135 2022-09-28 20:06:45.000000 stratocumulus-0.2.1/strato/commands/util.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-03-21 21:40:24.052619 stratocumulus-0.2.1/strato/tests/
--rw-r--r--   0 yangy197   (501) staff       (20)       72 2022-09-28 20:06:45.000000 stratocumulus-0.2.1/strato/tests/helpers.py
--rw-r--r--   0 yangy197   (501) staff       (20)      444 2022-09-28 20:06:45.000000 stratocumulus-0.2.1/strato/tests/test_backend.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1176 2023-03-20 20:53:11.000000 stratocumulus-0.2.1/strato/tests/test_cp.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1071 2022-09-28 20:06:45.000000 stratocumulus-0.2.1/strato/tests/test_rm.py
--rw-r--r--   0 yangy197   (501) staff       (20)      592 2022-09-28 20:06:45.000000 stratocumulus-0.2.1/strato/tests/test_sync.py
--rw-r--r--   0 yangy197   (501) staff       (20)      160 2023-03-21 21:40:23.000000 stratocumulus-0.2.1/strato/version.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-03-21 21:40:24.056232 stratocumulus-0.2.1/stratocumulus.egg-info/
--rw-r--r--   0 yangy197   (501) staff       (20)     7137 2023-03-21 21:40:23.000000 stratocumulus-0.2.1/stratocumulus.egg-info/PKG-INFO
--rw-r--r--   0 yangy197   (501) staff       (20)      727 2023-03-21 21:40:24.000000 stratocumulus-0.2.1/stratocumulus.egg-info/SOURCES.txt
--rw-r--r--   0 yangy197   (501) staff       (20)        1 2023-03-21 21:40:23.000000 stratocumulus-0.2.1/stratocumulus.egg-info/dependency_links.txt
--rw-r--r--   0 yangy197   (501) staff       (20)       48 2023-03-21 21:40:23.000000 stratocumulus-0.2.1/stratocumulus.egg-info/entry_points.txt
--rw-r--r--   0 yangy197   (501) staff       (20)       71 2023-03-21 21:40:23.000000 stratocumulus-0.2.1/stratocumulus.egg-info/requires.txt
--rw-r--r--   0 yangy197   (501) staff       (20)        7 2023-03-21 21:40:23.000000 stratocumulus-0.2.1/stratocumulus.egg-info/top_level.txt
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 19:40:17.983932 stratocumulus-0.2.2/
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 19:40:17.962378 stratocumulus-0.2.2/.github/
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 19:40:17.965266 stratocumulus-0.2.2/.github/workflows/
+-rw-r--r--   0 yangy197   (501) staff       (20)      703 2022-09-28 20:06:45.000000 stratocumulus-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0 yangy197   (501) staff       (20)     1532 2021-08-19 16:43:59.000000 stratocumulus-0.2.2/LICENSE
+-rw-r--r--   0 yangy197   (501) staff       (20)       62 2021-08-19 16:43:59.000000 stratocumulus-0.2.2/MANIFEST.in
+-rw-r--r--   0 yangy197   (501) staff       (20)     7259 2024-05-07 19:40:17.983068 stratocumulus-0.2.2/PKG-INFO
+-rw-r--r--   0 yangy197   (501) staff       (20)     4433 2022-09-28 20:06:45.000000 stratocumulus-0.2.2/README.rst
+-rw-r--r--   0 yangy197   (501) staff       (20)     1974 2023-03-21 21:30:56.000000 stratocumulus-0.2.2/pyproject.toml
+-rw-r--r--   0 yangy197   (501) staff       (20)       38 2024-05-07 19:40:17.984143 stratocumulus-0.2.2/setup.cfg
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 19:40:17.966706 stratocumulus-0.2.2/strato/
+-rw-r--r--   0 yangy197   (501) staff       (20)        0 2021-11-10 17:34:26.000000 stratocumulus-0.2.2/strato/__init__.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1020 2022-09-28 20:06:45.000000 stratocumulus-0.2.2/strato/__main__.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 19:40:17.968975 stratocumulus-0.2.2/strato/backends/
+-rw-r--r--   0 yangy197   (501) staff       (20)      133 2022-09-28 20:06:45.000000 stratocumulus-0.2.2/strato/backends/__init__.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     4524 2023-03-21 21:26:55.000000 stratocumulus-0.2.2/strato/backends/_aws.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     2531 2022-09-28 20:06:45.000000 stratocumulus-0.2.2/strato/backends/_gcp.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     2454 2024-05-07 19:27:02.000000 stratocumulus-0.2.2/strato/backends/_local.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 19:40:17.972671 stratocumulus-0.2.2/strato/commands/
+-rw-r--r--   0 yangy197   (501) staff       (20)        0 2021-11-10 17:34:26.000000 stratocumulus-0.2.2/strato/commands/__init__.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     2719 2023-03-20 20:53:11.000000 stratocumulus-0.2.2/strato/commands/cp.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1360 2022-09-28 20:06:45.000000 stratocumulus-0.2.2/strato/commands/exists.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     2312 2022-09-28 20:06:45.000000 stratocumulus-0.2.2/strato/commands/rm.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     2457 2022-09-28 20:06:45.000000 stratocumulus-0.2.2/strato/commands/sync.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1135 2022-09-28 20:06:45.000000 stratocumulus-0.2.2/strato/commands/util.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 19:40:17.976653 stratocumulus-0.2.2/strato/tests/
+-rw-r--r--   0 yangy197   (501) staff       (20)       72 2022-09-28 20:06:45.000000 stratocumulus-0.2.2/strato/tests/helpers.py
+-rw-r--r--   0 yangy197   (501) staff       (20)      444 2022-09-28 20:06:45.000000 stratocumulus-0.2.2/strato/tests/test_backend.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1271 2024-05-06 23:02:54.000000 stratocumulus-0.2.2/strato/tests/test_cp.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1071 2022-09-28 20:06:45.000000 stratocumulus-0.2.2/strato/tests/test_rm.py
+-rw-r--r--   0 yangy197   (501) staff       (20)      592 2022-09-28 20:06:45.000000 stratocumulus-0.2.2/strato/tests/test_sync.py
+-rw-r--r--   0 yangy197   (501) staff       (20)      411 2024-05-07 19:40:17.000000 stratocumulus-0.2.2/strato/version.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2024-05-07 19:40:17.981341 stratocumulus-0.2.2/stratocumulus.egg-info/
+-rw-r--r--   0 yangy197   (501) staff       (20)     7259 2024-05-07 19:40:17.000000 stratocumulus-0.2.2/stratocumulus.egg-info/PKG-INFO
+-rw-r--r--   0 yangy197   (501) staff       (20)      727 2024-05-07 19:40:17.000000 stratocumulus-0.2.2/stratocumulus.egg-info/SOURCES.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)        1 2024-05-07 19:40:17.000000 stratocumulus-0.2.2/stratocumulus.egg-info/dependency_links.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)       48 2024-05-07 19:40:17.000000 stratocumulus-0.2.2/stratocumulus.egg-info/entry_points.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)       71 2024-05-07 19:40:17.000000 stratocumulus-0.2.2/stratocumulus.egg-info/requires.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)        7 2024-05-07 19:40:17.000000 stratocumulus-0.2.2/stratocumulus.egg-info/top_level.txt
```

### Comparing `stratocumulus-0.2.1/.github/workflows/test.yml` & `stratocumulus-0.2.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.1/LICENSE` & `stratocumulus-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.1/PKG-INFO` & `stratocumulus-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stratocumulus
-Version: 0.2.1
+Version: 0.2.2
 Summary: File backend component of Cumulus
 Author-email: "Yiming Yang, Joshua Gould, Rimte Rocher, Bo Li" <cumulus-support@googlegroups.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, klarman-cell-observatory
         All rights reserved.
         
@@ -43,16 +43,19 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: s3fs
+Requires-Dist: importlib_metadata>=0.7; python_version < "3.8"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 ===================
 Stratocumulus
 ===================
 
 |PyPI| |Python| |License|
```

### Comparing `stratocumulus-0.2.1/README.rst` & `stratocumulus-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.1/pyproject.toml` & `stratocumulus-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.1/strato/__main__.py` & `stratocumulus-0.2.2/strato/__main__.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.1/strato/backends/_aws.py` & `stratocumulus-0.2.2/strato/backends/_aws.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.1/strato/backends/_gcp.py` & `stratocumulus-0.2.2/strato/backends/_gcp.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.1/strato/commands/cp.py` & `stratocumulus-0.2.2/strato/commands/cp.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.1/strato/commands/exists.py` & `stratocumulus-0.2.2/strato/commands/exists.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.1/strato/commands/rm.py` & `stratocumulus-0.2.2/strato/commands/rm.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.1/strato/commands/sync.py` & `stratocumulus-0.2.2/strato/commands/sync.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.1/strato/commands/util.py` & `stratocumulus-0.2.2/strato/commands/util.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.1/strato/tests/test_cp.py` & `stratocumulus-0.2.2/strato/tests/test_cp.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 @pytest.fixture(scope="module", params=[True, False])
 def trailing_slash(request):
     return request.param
 
 
 def test_cp_dir_aws(capsys, trailing_slash):
-    cp.main(["dir1", "s3://foo/bar" + "/" if trailing_slash else "", "-r", "--dryrun"])
+    cp.main(["dir1", "s3://foo/bar" + ("/" if trailing_slash else ""), "-r", "--dryrun"])
 
     assert (
         "aws s3 cp --only-show-errors --recursive dir1/ s3://foo/bar/dir1\n"
         == capsys.readouterr().out
     )
 
 
@@ -30,10 +30,14 @@
 
 def test_cp_dir_gcp(capsys):
     cp.main(["dir1", "gs://foo/bar", "-r", "--dryrun"])
     assert gsutil + " cp -r dir1 gs://foo/bar\n" == capsys.readouterr().out
 
 
 def test_cp_file_local(capsys):
-    # FIXME only the parent directory should be created
     cp.main(["file1", "/bar/foo", "--dryrun"])
-    assert "mkdir -p /bar/foo\ncp file1 /bar/foo\n" == capsys.readouterr().out
+    assert "cp file1 /bar/foo\n" == capsys.readouterr().out
+
+
+def test_cp_dir_local(capsys):
+    cp.main(["file1", "/bar/foo", "-r", "--dryrun"])
+    assert "mkdir -p /bar/foo\ncp -r file1 /bar/foo\n" == capsys.readouterr().out
```

### Comparing `stratocumulus-0.2.1/strato/tests/test_rm.py` & `stratocumulus-0.2.2/strato/tests/test_rm.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.1/strato/tests/test_sync.py` & `stratocumulus-0.2.2/strato/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `stratocumulus-0.2.1/stratocumulus.egg-info/PKG-INFO` & `stratocumulus-0.2.2/stratocumulus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stratocumulus
-Version: 0.2.1
+Version: 0.2.2
 Summary: File backend component of Cumulus
 Author-email: "Yiming Yang, Joshua Gould, Rimte Rocher, Bo Li" <cumulus-support@googlegroups.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, klarman-cell-observatory
         All rights reserved.
         
@@ -43,16 +43,19 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: s3fs
+Requires-Dist: importlib_metadata>=0.7; python_version < "3.8"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 ===================
 Stratocumulus
 ===================
 
 |PyPI| |Python| |License|
```

### Comparing `stratocumulus-0.2.1/stratocumulus.egg-info/SOURCES.txt` & `stratocumulus-0.2.2/stratocumulus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

