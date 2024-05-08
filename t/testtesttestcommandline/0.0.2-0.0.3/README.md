# Comparing `tmp/testtesttestcommandline-0.0.2.tar.gz` & `tmp/testtesttestcommandline-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testtesttestcommandline-0.0.2.tar", last modified: Wed May  8 15:33:32 2024, max compression
+gzip compressed data, was "testtesttestcommandline-0.0.3.tar", last modified: Wed May  8 15:34:48 2024, max compression
```

## Comparing `testtesttestcommandline-0.0.2.tar` & `testtesttestcommandline-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 minhthanh   (501) staff       (20)        0 2024-05-08 15:33:32.758577 testtesttestcommandline-0.0.2/
--rw-r--r--   0 minhthanh   (501) staff       (20)     1084 2024-04-07 15:58:08.000000 testtesttestcommandline-0.0.2/LICENSE
--rw-r--r--   0 minhthanh   (501) staff       (20)     4334 2024-05-08 15:33:32.758319 testtesttestcommandline-0.0.2/PKG-INFO
--rw-r--r--   0 minhthanh   (501) staff       (20)     2160 2024-04-07 16:15:36.000000 testtesttestcommandline-0.0.2/README.md
--rw-r--r--   0 minhthanh   (501) staff       (20)     1039 2024-05-08 15:33:01.000000 testtesttestcommandline-0.0.2/pyproject.toml
--rw-r--r--   0 minhthanh   (501) staff       (20)       38 2024-05-08 15:33:32.758623 testtesttestcommandline-0.0.2/setup.cfg
-drwxr-xr-x   0 minhthanh   (501) staff       (20)        0 2024-05-08 15:33:32.757965 testtesttestcommandline-0.0.2/testtesttestcommandline.egg-info/
--rw-r--r--   0 minhthanh   (501) staff       (20)     4334 2024-05-08 15:33:32.000000 testtesttestcommandline-0.0.2/testtesttestcommandline.egg-info/PKG-INFO
--rw-r--r--   0 minhthanh   (501) staff       (20)      316 2024-05-08 15:33:32.000000 testtesttestcommandline-0.0.2/testtesttestcommandline.egg-info/SOURCES.txt
--rw-r--r--   0 minhthanh   (501) staff       (20)        1 2024-05-08 15:33:32.000000 testtesttestcommandline-0.0.2/testtesttestcommandline.egg-info/dependency_links.txt
--rw-r--r--   0 minhthanh   (501) staff       (20)       46 2024-05-08 15:33:32.000000 testtesttestcommandline-0.0.2/testtesttestcommandline.egg-info/entry_points.txt
--rw-r--r--   0 minhthanh   (501) staff       (20)       12 2024-05-08 15:33:32.000000 testtesttestcommandline-0.0.2/testtesttestcommandline.egg-info/requires.txt
--rw-r--r--   0 minhthanh   (501) staff       (20)        7 2024-05-08 15:33:32.000000 testtesttestcommandline-0.0.2/testtesttestcommandline.egg-info/top_level.txt
+drwxr-xr-x   0 minhthanh   (501) staff       (20)        0 2024-05-08 15:34:48.372356 testtesttestcommandline-0.0.3/
+-rw-r--r--   0 minhthanh   (501) staff       (20)     1084 2024-04-07 15:58:08.000000 testtesttestcommandline-0.0.3/LICENSE
+-rw-r--r--   0 minhthanh   (501) staff       (20)     4336 2024-05-08 15:34:48.372116 testtesttestcommandline-0.0.3/PKG-INFO
+-rw-r--r--   0 minhthanh   (501) staff       (20)     2160 2024-04-07 16:15:36.000000 testtesttestcommandline-0.0.3/README.md
+-rw-r--r--   0 minhthanh   (501) staff       (20)     1041 2024-05-08 15:34:44.000000 testtesttestcommandline-0.0.3/pyproject.toml
+-rw-r--r--   0 minhthanh   (501) staff       (20)       38 2024-05-08 15:34:48.372407 testtesttestcommandline-0.0.3/setup.cfg
+drwxr-xr-x   0 minhthanh   (501) staff       (20)        0 2024-05-08 15:34:48.371787 testtesttestcommandline-0.0.3/testtesttestcommandline.egg-info/
+-rw-r--r--   0 minhthanh   (501) staff       (20)     4336 2024-05-08 15:34:48.000000 testtesttestcommandline-0.0.3/testtesttestcommandline.egg-info/PKG-INFO
+-rw-r--r--   0 minhthanh   (501) staff       (20)      316 2024-05-08 15:34:48.000000 testtesttestcommandline-0.0.3/testtesttestcommandline.egg-info/SOURCES.txt
+-rw-r--r--   0 minhthanh   (501) staff       (20)        1 2024-05-08 15:34:48.000000 testtesttestcommandline-0.0.3/testtesttestcommandline.egg-info/dependency_links.txt
+-rw-r--r--   0 minhthanh   (501) staff       (20)       46 2024-05-08 15:34:48.000000 testtesttestcommandline-0.0.3/testtesttestcommandline.egg-info/entry_points.txt
+-rw-r--r--   0 minhthanh   (501) staff       (20)       14 2024-05-08 15:34:48.000000 testtesttestcommandline-0.0.3/testtesttestcommandline.egg-info/requires.txt
+-rw-r--r--   0 minhthanh   (501) staff       (20)        7 2024-05-08 15:34:48.000000 testtesttestcommandline-0.0.3/testtesttestcommandline.egg-info/top_level.txt
```

### Comparing `testtesttestcommandline-0.0.2/LICENSE` & `testtesttestcommandline-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `testtesttestcommandline-0.0.2/PKG-INFO` & `testtesttestcommandline-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testtesttestcommandline
-Version: 0.0.2
+Version: 0.0.3
 Summary: A command-line tool to crack password-protected compressed files using brute force.
 Author-email: Minh Thanh <thanhdoantranminh@gmail.com>
 License: MIT License
         
         Copyright (c) 2017 - 2024 Doan Tran Minh Thanh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,15 +35,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: patoolib>=2
+Requires-Dist: patool>=2.2.0
 
 # CompressedCrack
 
 ![Banner](./assets/banner.png)
 
 CompressedCrack is a command-line tool that utilizes the brute-force method to crack any password-protected compressed file. It generates password combinations based on user-defined character sets and length range, and attempts to extract the archive using each generated password until the correct password is found.
```

### Comparing `testtesttestcommandline-0.0.2/README.md` & `testtesttestcommandline-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `testtesttestcommandline-0.0.2/pyproject.toml` & `testtesttestcommandline-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "testtesttestcommandline"
-version = "0.0.2"
+version = "0.0.3"
 description = "A command-line tool to crack password-protected compressed files using brute force."
 readme = "README.md"
 authors = [{ name = "Minh Thanh", email = "thanhdoantranminh@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
@@ -16,15 +16,15 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.6",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
 ]
 keywords = ["brute force", "password cracking", "compressed files"]
-dependencies = ["patoolib>=2"]
+dependencies = ["patool>=2.2.0"]
 requires-python = ">=3.6"
 
 [project.urls]
 "Homepage" = "https://github.com/mnismt/CompressedCrack"
 "Bug Tracker" = "https://github.com/mnismt/CompressedCrack/issues"
 
 [project.scripts]
```

### Comparing `testtesttestcommandline-0.0.2/testtesttestcommandline.egg-info/PKG-INFO` & `testtesttestcommandline-0.0.3/testtesttestcommandline.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testtesttestcommandline
-Version: 0.0.2
+Version: 0.0.3
 Summary: A command-line tool to crack password-protected compressed files using brute force.
 Author-email: Minh Thanh <thanhdoantranminh@gmail.com>
 License: MIT License
         
         Copyright (c) 2017 - 2024 Doan Tran Minh Thanh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,15 +35,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: patoolib>=2
+Requires-Dist: patool>=2.2.0
 
 # CompressedCrack
 
 ![Banner](./assets/banner.png)
 
 CompressedCrack is a command-line tool that utilizes the brute-force method to crack any password-protected compressed file. It generates password combinations based on user-defined character sets and length range, and attempts to extract the archive using each generated password until the correct password is found.
```

