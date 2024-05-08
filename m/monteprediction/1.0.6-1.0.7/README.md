# Comparing `tmp/monteprediction-1.0.6.tar.gz` & `tmp/monteprediction-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monteprediction-1.0.6.tar", last modified: Tue Apr 16 00:47:27 2024, max compression
+gzip compressed data, was "monteprediction-1.0.7.tar", last modified: Wed May  8 02:12:32 2024, max compression
```

## Comparing `monteprediction-1.0.6.tar` & `monteprediction-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:47:27.924768 monteprediction-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 00:47:17.000000 monteprediction-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-16 00:47:27.924768 monteprediction-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 00:47:17.000000 monteprediction-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:47:27.920768 monteprediction-1.0.6/monteprediction/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-16 00:47:17.000000 monteprediction-1.0.6/monteprediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 00:47:17.000000 monteprediction-1.0.6/monteprediction/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-16 00:47:17.000000 monteprediction-1.0.6/monteprediction/calendarutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-16 00:47:17.000000 monteprediction-1.0.6/monteprediction/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-16 00:47:17.000000 monteprediction-1.0.6/monteprediction/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-16 00:47:17.000000 monteprediction-1.0.6/monteprediction/truth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-16 00:47:17.000000 monteprediction-1.0.6/monteprediction/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:47:27.924768 monteprediction-1.0.6/monteprediction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-16 00:47:27.000000 monteprediction-1.0.6/monteprediction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-16 00:47:27.000000 monteprediction-1.0.6/monteprediction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 00:47:27.000000 monteprediction-1.0.6/monteprediction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 00:47:27.000000 monteprediction-1.0.6/monteprediction.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 00:47:27.000000 monteprediction-1.0.6/monteprediction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 00:47:27.000000 monteprediction-1.0.6/monteprediction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 00:47:27.924768 monteprediction-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-16 00:47:17.000000 monteprediction-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:47:27.924768 monteprediction-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-16 00:47:17.000000 monteprediction-1.0.6/tests/test_calendarutil.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-16 00:47:17.000000 monteprediction-1.0.6/tests/test_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:12:32.175104 monteprediction-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-08 02:12:19.000000 monteprediction-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-08 02:12:32.175104 monteprediction-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-08 02:12:19.000000 monteprediction-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:12:32.171104 monteprediction-1.0.7/monteprediction/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-08 02:12:19.000000 monteprediction-1.0.7/monteprediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-08 02:12:19.000000 monteprediction-1.0.7/monteprediction/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-08 02:12:19.000000 monteprediction-1.0.7/monteprediction/calendarutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-08 02:12:19.000000 monteprediction-1.0.7/monteprediction/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-08 02:12:19.000000 monteprediction-1.0.7/monteprediction/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-08 02:12:19.000000 monteprediction-1.0.7/monteprediction/truth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-08 02:12:19.000000 monteprediction-1.0.7/monteprediction/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:12:32.171104 monteprediction-1.0.7/monteprediction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-08 02:12:32.000000 monteprediction-1.0.7/monteprediction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-08 02:12:32.000000 monteprediction-1.0.7/monteprediction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 02:12:32.000000 monteprediction-1.0.7/monteprediction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 02:12:32.000000 monteprediction-1.0.7/monteprediction.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 02:12:32.000000 monteprediction-1.0.7/monteprediction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 02:12:32.000000 monteprediction-1.0.7/monteprediction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 02:12:32.175104 monteprediction-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-08 02:12:19.000000 monteprediction-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:12:32.171104 monteprediction-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-08 02:12:19.000000 monteprediction-1.0.7/tests/test_calendarutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-08 02:12:19.000000 monteprediction-1.0.7/tests/test_scoring.py
```

### Comparing `monteprediction-1.0.6/LICENSE` & `monteprediction-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.6/PKG-INFO` & `monteprediction-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monteprediction
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Weekly Monte Carlo Game
 Home-page: https://github.com/microprediction/monteprediction
 Author: microprediction
 Author-email: peter.cotton@microprediction.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `monteprediction-1.0.6/monteprediction/scoring.py` & `monteprediction-1.0.7/monteprediction/scoring.py`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.6/monteprediction/submission.py` & `monteprediction-1.0.7/monteprediction/submission.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,7 +34,8 @@
                 print(f"An error occurred: {e}")
 
             # Optional: wait before retrying
             time.sleep(1)  # Wait for 1 second before retrying
 
         else:
             print(f"Failed to send chunk {chunk_no} after {max_retries} attempts.")
+    return response
```

### Comparing `monteprediction-1.0.6/monteprediction/truth.py` & `monteprediction-1.0.7/monteprediction/truth.py`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.6/monteprediction/verification.py` & `monteprediction-1.0.7/monteprediction/verification.py`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.6/monteprediction.egg-info/PKG-INFO` & `monteprediction-1.0.7/monteprediction.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monteprediction
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Weekly Monte Carlo Game
 Home-page: https://github.com/microprediction/monteprediction
 Author: microprediction
 Author-email: peter.cotton@microprediction.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `monteprediction-1.0.6/setup.py` & `monteprediction-1.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="monteprediction",
-    version="1.0.6",
+    version="1.0.7",
     description="A Weekly Monte Carlo Game",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/microprediction/monteprediction",
     author="microprediction",
     author_email="peter.cotton@microprediction.com",
     license="MIT",
```

### Comparing `monteprediction-1.0.6/tests/test_calendarutil.py` & `monteprediction-1.0.7/tests/test_calendarutil.py`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.6/tests/test_scoring.py` & `monteprediction-1.0.7/tests/test_scoring.py`

 * *Files identical despite different names*

