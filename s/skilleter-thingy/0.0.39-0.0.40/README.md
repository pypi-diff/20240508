# Comparing `tmp/skilleter_thingy-0.0.39.tar.gz` & `tmp/skilleter_thingy-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skilleter_thingy-0.0.39.tar", last modified: Wed May  8 12:52:29 2024, max compression
+gzip compressed data, was "skilleter_thingy-0.0.40.tar", last modified: Wed May  8 12:53:42 2024, max compression
```

## Comparing `skilleter_thingy-0.0.39.tar` & `skilleter_thingy-0.0.40.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:52:29.930164 skilleter_thingy-0.0.39/
--rw-rw-r--   0 jms       (1000) jms       (1000)    32422 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.39/LICENSE
--rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-05-08 12:52:29.926165 skilleter_thingy-0.0.39/PKG-INFO
--rw-rw-r--   0 jms       (1000) jms       (1000)     4510 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.39/README.md
--rw-rw-r--   0 jms       (1000) jms       (1000)     2855 2024-05-08 12:52:21.000000 skilleter_thingy-0.0.39/pyproject.toml
--rw-rw-r--   0 jms       (1000) jms       (1000)       38 2024-05-08 12:52:29.930164 skilleter_thingy-0.0.39/setup.cfg
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:52:29.926165 skilleter_thingy-0.0.39/src/
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:52:29.926165 skilleter_thingy-0.0.39/src/skilleter_thingy.egg-info/
--rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-05-08 12:52:29.000000 skilleter_thingy-0.0.39/src/skilleter_thingy.egg-info/PKG-INFO
--rw-rw-r--   0 jms       (1000) jms       (1000)      298 2024-05-08 12:52:29.000000 skilleter_thingy-0.0.39/src/skilleter_thingy.egg-info/SOURCES.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)        1 2024-05-08 12:52:29.000000 skilleter_thingy-0.0.39/src/skilleter_thingy.egg-info/dependency_links.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)     1971 2024-05-08 12:52:29.000000 skilleter_thingy-0.0.39/src/skilleter_thingy.egg-info/entry_points.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)       70 2024-05-08 12:52:29.000000 skilleter_thingy-0.0.39/src/skilleter_thingy.egg-info/requires.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)        7 2024-05-08 12:52:29.000000 skilleter_thingy-0.0.39/src/skilleter_thingy.egg-info/top_level.txt
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:53:42.827547 skilleter_thingy-0.0.40/
+-rw-rw-r--   0 jms       (1000) jms       (1000)    32422 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.40/LICENSE
+-rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-05-08 12:53:42.827547 skilleter_thingy-0.0.40/PKG-INFO
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4510 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.40/README.md
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2855 2024-05-08 12:53:19.000000 skilleter_thingy-0.0.40/pyproject.toml
+-rw-rw-r--   0 jms       (1000) jms       (1000)       38 2024-05-08 12:53:42.827547 skilleter_thingy-0.0.40/setup.cfg
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:53:42.823547 skilleter_thingy-0.0.40/src/
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-05-08 12:53:42.827547 skilleter_thingy-0.0.40/src/skilleter_thingy.egg-info/
+-rw-r--r--   0 jms       (1000) jms       (1000)     5210 2024-05-08 12:53:42.000000 skilleter_thingy-0.0.40/src/skilleter_thingy.egg-info/PKG-INFO
+-rw-rw-r--   0 jms       (1000) jms       (1000)      298 2024-05-08 12:53:42.000000 skilleter_thingy-0.0.40/src/skilleter_thingy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)        1 2024-05-08 12:53:42.000000 skilleter_thingy-0.0.40/src/skilleter_thingy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)     1971 2024-05-08 12:53:42.000000 skilleter_thingy-0.0.40/src/skilleter_thingy.egg-info/entry_points.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)       70 2024-05-08 12:53:42.000000 skilleter_thingy-0.0.40/src/skilleter_thingy.egg-info/requires.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)        7 2024-05-08 12:53:42.000000 skilleter_thingy-0.0.40/src/skilleter_thingy.egg-info/top_level.txt
```

### Comparing `skilleter_thingy-0.0.39/LICENSE` & `skilleter_thingy-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.39/PKG-INFO` & `skilleter_thingy-0.0.40/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skilleter_thingy
-Version: 0.0.39
+Version: 0.0.40
 Summary: A collection of useful utilities, mainly aimed at making Git more friendly
 Author-email: John Skilleter <john@skilleter.org.uk>
 Project-URL: Home, https://skilleter.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `skilleter_thingy-0.0.39/README.md` & `skilleter_thingy-0.0.40/README.md`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.39/pyproject.toml` & `skilleter_thingy-0.0.40/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "skilleter_thingy"
 
 # Version must be incremented to install updated Thingy
 
-version = "0.0.39"
+version = "0.0.40"
 
 authors = [
     {name="John Skilleter", email="john@skilleter.org.uk"},
 ]
 
 description = "A collection of useful utilities, mainly aimed at making Git more friendly"
```

### Comparing `skilleter_thingy-0.0.39/src/skilleter_thingy.egg-info/PKG-INFO` & `skilleter_thingy-0.0.40/src/skilleter_thingy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skilleter_thingy
-Version: 0.0.39
+Version: 0.0.40
 Summary: A collection of useful utilities, mainly aimed at making Git more friendly
 Author-email: John Skilleter <john@skilleter.org.uk>
 Project-URL: Home, https://skilleter.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `skilleter_thingy-0.0.39/src/skilleter_thingy.egg-info/entry_points.txt` & `skilleter_thingy-0.0.40/src/skilleter_thingy.egg-info/entry_points.txt`

 * *Files identical despite different names*

