# Comparing `tmp/subdivision_hole_filler-0.0.1.tar.gz` & `tmp/subdivision_hole_filler-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subdivision_hole_filler-0.0.1.tar", last modified: Wed May  8 06:22:00 2024, max compression
+gzip compressed data, was "subdivision_hole_filler-1.0.0.tar", last modified: Wed May  8 07:46:18 2024, max compression
```

## Comparing `subdivision_hole_filler-0.0.1.tar` & `subdivision_hole_filler-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:22:00.185003 subdivision_hole_filler-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:22:00.177003 subdivision_hole_filler-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:22:00.181003 subdivision_hole_filler-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-08 06:21:47.000000 subdivision_hole_filler-0.0.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-08 06:21:47.000000 subdivision_hole_filler-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-08 06:21:47.000000 subdivision_hole_filler-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-08 06:21:47.000000 subdivision_hole_filler-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)   200849 2024-05-08 06:21:47.000000 subdivision_hole_filler-0.0.1/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-08 06:22:00.185003 subdivision_hole_filler-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-08 06:21:47.000000 subdivision_hole_filler-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-08 06:21:47.000000 subdivision_hole_filler-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 06:22:00.185003 subdivision_hole_filler-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:22:00.181003 subdivision_hole_filler-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:22:00.181003 subdivision_hole_filler-0.0.1/src/subdivision_hole_filler/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 06:21:47.000000 subdivision_hole_filler-0.0.1/src/subdivision_hole_filler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 06:22:00.000000 subdivision_hole_filler-0.0.1/src/subdivision_hole_filler/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-08 06:21:47.000000 subdivision_hole_filler-0.0.1/src/subdivision_hole_filler/hole_filler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:22:00.181003 subdivision_hole_filler-0.0.1/src/subdivision_hole_filler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-08 06:22:00.000000 subdivision_hole_filler-0.0.1/src/subdivision_hole_filler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-08 06:22:00.000000 subdivision_hole_filler-0.0.1/src/subdivision_hole_filler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 06:22:00.000000 subdivision_hole_filler-0.0.1/src/subdivision_hole_filler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 06:22:00.000000 subdivision_hole_filler-0.0.1/src/subdivision_hole_filler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 06:22:00.000000 subdivision_hole_filler-0.0.1/src/subdivision_hole_filler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:22:00.181003 subdivision_hole_filler-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-08 06:21:47.000000 subdivision_hole_filler-0.0.1/tests/test_6sided_hole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:18.574204 subdivision_hole_filler-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:18.570204 subdivision_hole_filler-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:18.574204 subdivision_hole_filler-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-08 07:46:09.000000 subdivision_hole_filler-1.0.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-08 07:46:09.000000 subdivision_hole_filler-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-08 07:46:09.000000 subdivision_hole_filler-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-08 07:46:09.000000 subdivision_hole_filler-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   200849 2024-05-08 07:46:09.000000 subdivision_hole_filler-1.0.0/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-08 07:46:18.574204 subdivision_hole_filler-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-08 07:46:09.000000 subdivision_hole_filler-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   106308 2024-05-08 07:46:09.000000 subdivision_hole_filler-1.0.0/iso.png
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-08 07:46:09.000000 subdivision_hole_filler-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 07:46:18.574204 subdivision_hole_filler-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    52038 2024-05-08 07:46:09.000000 subdivision_hole_filler-1.0.0/side.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:18.570204 subdivision_hole_filler-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:18.574204 subdivision_hole_filler-1.0.0/src/subdivision_hole_filler/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 07:46:09.000000 subdivision_hole_filler-1.0.0/src/subdivision_hole_filler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 07:46:18.000000 subdivision_hole_filler-1.0.0/src/subdivision_hole_filler/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-08 07:46:09.000000 subdivision_hole_filler-1.0.0/src/subdivision_hole_filler/hole_filler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:18.574204 subdivision_hole_filler-1.0.0/src/subdivision_hole_filler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-08 07:46:18.000000 subdivision_hole_filler-1.0.0/src/subdivision_hole_filler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-08 07:46:18.000000 subdivision_hole_filler-1.0.0/src/subdivision_hole_filler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:46:18.000000 subdivision_hole_filler-1.0.0/src/subdivision_hole_filler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 07:46:18.000000 subdivision_hole_filler-1.0.0/src/subdivision_hole_filler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 07:46:18.000000 subdivision_hole_filler-1.0.0/src/subdivision_hole_filler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:18.574204 subdivision_hole_filler-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-08 07:46:09.000000 subdivision_hole_filler-1.0.0/tests/test_6sided_hole.py
```

### Comparing `subdivision_hole_filler-0.0.1/.github/workflows/python-package.yml` & `subdivision_hole_filler-1.0.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-0.0.1/.github/workflows/python-publish.yml` & `subdivision_hole_filler-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-0.0.1/.gitignore` & `subdivision_hole_filler-1.0.0/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+_version.py
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `subdivision_hole_filler-0.0.1/LICENSE` & `subdivision_hole_filler-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-0.0.1/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf` & `subdivision_hole_filler-1.0.0/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-0.0.1/pyproject.toml` & `subdivision_hole_filler-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "subdivision-hole-filler"
 authors = [
   { name="HUANG Lihao", email="huang-lihao@outlook.com" },
 ]
-description = "A python package to fill N-sided holes using combined subdivision schemes."
+description = "A python package to fill N-sided holes using combined subdivision schemes, based on Catmull-Clark subdivison."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `subdivision_hole_filler-0.0.1/src/subdivision_hole_filler.egg-info/SOURCES.txt` & `subdivision_hole_filler-1.0.0/src/subdivision_hole_filler.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .gitignore
 LICENSE
 Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf
 README.md
+iso.png
 pyproject.toml
+side.png
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
 src/subdivision_hole_filler/__init__.py
 src/subdivision_hole_filler/_version.py
 src/subdivision_hole_filler/hole_filler.py
 src/subdivision_hole_filler.egg-info/PKG-INFO
 src/subdivision_hole_filler.egg-info/SOURCES.txt
```

