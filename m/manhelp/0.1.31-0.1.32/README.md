# Comparing `tmp/manhelp-0.1.31.tar.gz` & `tmp/manhelp-0.1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manhelp-0.1.31.tar", last modified: Wed May  8 08:17:43 2024, max compression
+gzip compressed data, was "manhelp-0.1.32.tar", last modified: Wed May  8 08:28:31 2024, max compression
```

## Comparing `manhelp-0.1.31.tar` & `manhelp-0.1.32.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 makbuk     (501) staff       (20)        0 2024-05-08 08:17:43.266809 manhelp-0.1.31/
--rw-r--r--   0 makbuk     (501) staff       (20)       35 2024-05-07 17:15:57.000000 manhelp-0.1.31/MANIFEST.in
--rw-r--r--   0 makbuk     (501) staff       (20)      492 2024-05-08 08:17:43.266277 manhelp-0.1.31/PKG-INFO
-drwxr-xr-x   0 makbuk     (501) staff       (20)        0 2024-05-08 08:17:43.244941 manhelp-0.1.31/iman/
--rw-r--r--   0 makbuk     (501) staff       (20)      316 2024-05-04 19:31:49.000000 manhelp-0.1.31/iman/__init__.py
-drwxr-xr-x   0 makbuk     (501) staff       (20)        0 2024-05-08 08:17:43.245807 manhelp-0.1.31/iman/data/
--rw-r--r--   0 makbuk     (501) staff       (20)  7715734 2024-05-04 19:28:40.000000 manhelp-0.1.31/iman/data/my-embeddings.pkl
--rw-r--r--   0 makbuk     (501) staff       (20)       66 2024-05-07 15:46:05.000000 manhelp-0.1.31/iman/main.py
--rw-r--r--   0 makbuk     (501) staff       (20)     1951 2024-05-07 15:32:07.000000 manhelp-0.1.31/iman/search.py
-drwxr-xr-x   0 makbuk     (501) staff       (20)        0 2024-05-08 08:17:43.265738 manhelp-0.1.31/manhelp.egg-info/
--rw-r--r--   0 makbuk     (501) staff       (20)      492 2024-05-08 08:17:43.000000 manhelp-0.1.31/manhelp.egg-info/PKG-INFO
--rw-r--r--   0 makbuk     (501) staff       (20)      304 2024-05-08 08:17:43.000000 manhelp-0.1.31/manhelp.egg-info/SOURCES.txt
--rw-r--r--   0 makbuk     (501) staff       (20)        1 2024-05-08 08:17:43.000000 manhelp-0.1.31/manhelp.egg-info/dependency_links.txt
--rw-r--r--   0 makbuk     (501) staff       (20)       39 2024-05-08 08:17:43.000000 manhelp-0.1.31/manhelp.egg-info/entry_points.txt
--rw-r--r--   0 makbuk     (501) staff       (20)       43 2024-05-08 08:17:43.000000 manhelp-0.1.31/manhelp.egg-info/requires.txt
--rw-r--r--   0 makbuk     (501) staff       (20)        5 2024-05-08 08:17:43.000000 manhelp-0.1.31/manhelp.egg-info/top_level.txt
--rw-r--r--   0 makbuk     (501) staff       (20)      857 2024-05-08 08:17:33.000000 manhelp-0.1.31/pyproject.toml
--rw-r--r--   0 makbuk     (501) staff       (20)       43 2024-05-08 07:26:04.000000 manhelp-0.1.31/requirements.txt
--rw-r--r--   0 makbuk     (501) staff       (20)       38 2024-05-08 08:17:43.266916 manhelp-0.1.31/setup.cfg
+drwxr-xr-x   0 makbuk     (501) staff       (20)        0 2024-05-08 08:28:31.903714 manhelp-0.1.32/
+-rw-r--r--   0 makbuk     (501) staff       (20)       35 2024-05-07 17:15:57.000000 manhelp-0.1.32/MANIFEST.in
+-rw-r--r--   0 makbuk     (501) staff       (20)      492 2024-05-08 08:28:31.902190 manhelp-0.1.32/PKG-INFO
+drwxr-xr-x   0 makbuk     (501) staff       (20)        0 2024-05-08 08:28:31.893956 manhelp-0.1.32/manhelp/
+-rw-r--r--   0 makbuk     (501) staff       (20)      322 2024-05-08 08:26:31.000000 manhelp-0.1.32/manhelp/__init__.py
+-rw-r--r--   0 makbuk     (501) staff       (20)       69 2024-05-08 08:26:25.000000 manhelp-0.1.32/manhelp/main.py
+-rw-r--r--   0 makbuk     (501) staff       (20)     1951 2024-05-08 08:26:33.000000 manhelp-0.1.32/manhelp/search.py
+drwxr-xr-x   0 makbuk     (501) staff       (20)        0 2024-05-08 08:28:31.901147 manhelp-0.1.32/manhelp.egg-info/
+-rw-r--r--   0 makbuk     (501) staff       (20)      492 2024-05-08 08:28:31.000000 manhelp-0.1.32/manhelp.egg-info/PKG-INFO
+-rw-r--r--   0 makbuk     (501) staff       (20)      285 2024-05-08 08:28:31.000000 manhelp-0.1.32/manhelp.egg-info/SOURCES.txt
+-rw-r--r--   0 makbuk     (501) staff       (20)        1 2024-05-08 08:28:31.000000 manhelp-0.1.32/manhelp.egg-info/dependency_links.txt
+-rw-r--r--   0 makbuk     (501) staff       (20)       42 2024-05-08 08:28:31.000000 manhelp-0.1.32/manhelp.egg-info/entry_points.txt
+-rw-r--r--   0 makbuk     (501) staff       (20)       43 2024-05-08 08:28:31.000000 manhelp-0.1.32/manhelp.egg-info/requires.txt
+-rw-r--r--   0 makbuk     (501) staff       (20)        8 2024-05-08 08:28:31.000000 manhelp-0.1.32/manhelp.egg-info/top_level.txt
+-rw-r--r--   0 makbuk     (501) staff       (20)      863 2024-05-08 08:27:58.000000 manhelp-0.1.32/pyproject.toml
+-rw-r--r--   0 makbuk     (501) staff       (20)       43 2024-05-08 07:26:04.000000 manhelp-0.1.32/requirements.txt
+-rw-r--r--   0 makbuk     (501) staff       (20)       38 2024-05-08 08:28:31.903922 manhelp-0.1.32/setup.cfg
```

### Comparing `manhelp-0.1.31/iman/search.py` & `manhelp-0.1.32/manhelp/search.py`

 * *Files identical despite different names*

### Comparing `manhelp-0.1.31/pyproject.toml` & `manhelp-0.1.32/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "manhelp"
-version = "0.1.31"
+version = "0.1.32"
 description = "manhelp provides an intuitive interface for finding Linux commands. It uses natural language processing to understand human language queries and returns the most relevant Linux commands. Ideal for both beginners who are learning Linux and experienced users who need a quick reference."
 authors = [
     {name = "me", email = "example@email.com"},
 ]
 
 license = { text = "MIT" }
 requires-python = ">=3.8"
@@ -24,12 +24,12 @@
 
 # [tool.setuptools.packages.find]
 # include = ["./iman"]  # ["*"] by default
 # exclude = ["./raw"]  # empty by default
 
 
 [tool.setuptools]
-packages = ["iman"]
+packages = ["manhelp"]
 
 
 [project.scripts]
-iman = "iman.main:app"
+iman = "manhelp.main:app"
```

