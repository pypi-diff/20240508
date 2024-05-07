# Comparing `tmp/laser_mind_client_meta-0.4.0.tar.gz` & `tmp/laser_mind_client_meta-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laser_mind_client_meta-0.4.0.tar", last modified: Tue Apr 30 12:36:02 2024, max compression
+gzip compressed data, was "laser_mind_client_meta-0.5.0.tar", last modified: Tue May  7 23:57:50 2024, max compression
```

## Comparing `laser_mind_client_meta-0.4.0.tar` & `laser_mind_client_meta-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 12:36:02.181168 laser_mind_client_meta-0.4.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1077 2024-04-30 12:18:34.000000 laser_mind_client_meta-0.4.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      475 2024-04-30 12:36:02.181168 laser_mind_client_meta-0.4.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       24 2024-04-30 12:18:34.000000 laser_mind_client_meta-0.4.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 12:36:02.177168 laser_mind_client_meta-0.4.0/laser_mind_client_meta/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       70 2024-04-30 12:18:34.000000 laser_mind_client_meta-0.4.0/laser_mind_client_meta/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      391 2024-04-30 12:18:34.000000 laser_mind_client_meta-0.4.0/laser_mind_client_meta/laser_mind_message_keys.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 12:36:02.177168 laser_mind_client_meta-0.4.0/laser_mind_client_meta.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      475 2024-04-30 12:36:02.000000 laser_mind_client_meta-0.4.0/laser_mind_client_meta.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      301 2024-04-30 12:36:02.000000 laser_mind_client_meta-0.4.0/laser_mind_client_meta.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-30 12:36:02.000000 laser_mind_client_meta-0.4.0/laser_mind_client_meta.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       23 2024-04-30 12:36:02.000000 laser_mind_client_meta-0.4.0/laser_mind_client_meta.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      605 2024-04-30 12:35:59.000000 laser_mind_client_meta-0.4.0/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-30 12:36:02.181168 laser_mind_client_meta-0.4.0/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:57:50.798461 laser_mind_client_meta-0.5.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-07 23:56:12.000000 laser_mind_client_meta-0.5.0/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      487 2024-05-07 23:57:50.798461 laser_mind_client_meta-0.5.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       24 2024-05-07 23:56:12.000000 laser_mind_client_meta-0.5.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:57:50.798461 laser_mind_client_meta-0.5.0/laser_mind_client_meta/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       70 2024-05-07 23:56:12.000000 laser_mind_client_meta-0.5.0/laser_mind_client_meta/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      391 2024-05-07 23:56:12.000000 laser_mind_client_meta-0.5.0/laser_mind_client_meta/laser_mind_message_keys.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:57:50.798461 laser_mind_client_meta-0.5.0/laser_mind_client_meta.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      487 2024-05-07 23:57:50.000000 laser_mind_client_meta-0.5.0/laser_mind_client_meta.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      301 2024-05-07 23:57:50.000000 laser_mind_client_meta-0.5.0/laser_mind_client_meta.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-07 23:57:50.000000 laser_mind_client_meta-0.5.0/laser_mind_client_meta.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       23 2024-05-07 23:57:50.000000 laser_mind_client_meta-0.5.0/laser_mind_client_meta.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      617 2024-05-07 23:57:46.000000 laser_mind_client_meta-0.5.0/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-07 23:57:50.798461 laser_mind_client_meta-0.5.0/setup.cfg
```

### Comparing `laser_mind_client_meta-0.4.0/pyproject.toml` & `laser_mind_client_meta-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "laser-mind-client-meta"
-version = "0.4.0"
+version = "0.5.0"
 description = "A meta data package for laser mind clients"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = []
-classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
+classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "Assaf Kalinski"
 email = "assaf@lightsolver.com"
 
 [project.urls]
 Homepage = "https://lightsolver.com"
```

