# Comparing `tmp/bashgptz-0.1.tar.gz` & `tmp/bashgptz-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bashgptz-0.1.tar", last modified: Wed May  8 12:00:51 2024, max compression
+gzip compressed data, was "bashgptz-1.0.tar", last modified: Wed May  8 11:18:58 2024, max compression
```

## Comparing `bashgptz-0.1.tar` & `bashgptz-1.0.tar`

### file list

```diff
@@ -1,30 +1,28 @@
-drwxr-xr-x   0 petar      (501) staff       (20)        0 2024-05-08 12:00:51.419522 bashgptz-0.1/
--rw-r--r--   0 petar      (501) staff       (20)     1068 2024-05-06 14:50:14.000000 bashgptz-0.1/LICENSE.txt
--rw-r--r--   0 petar      (501) staff       (20)     4423 2024-05-08 12:00:51.419217 bashgptz-0.1/PKG-INFO
--rw-r--r--   0 petar      (501) staff       (20)     3907 2024-02-05 20:51:52.000000 bashgptz-0.1/README.md
--rw-r--r--   0 petar      (501) staff       (20)      848 2024-05-08 12:00:44.000000 bashgptz-0.1/pyproject.toml
--rw-r--r--   0 petar      (501) staff       (20)       38 2024-05-08 12:00:51.419588 bashgptz-0.1/setup.cfg
--rw-r--r--   0 petar      (501) staff       (20)      619 2024-05-08 11:04:38.000000 bashgptz-0.1/setup.py
-drwxr-xr-x   0 petar      (501) staff       (20)        0 2024-05-08 12:00:51.408287 bashgptz-0.1/src/
-drwxr-xr-x   0 petar      (501) staff       (20)        0 2024-05-08 12:00:51.417201 bashgptz-0.1/src/bashgpt/
--rw-r--r--   0 petar      (501) staff       (20)        0 2024-05-06 19:04:03.000000 bashgptz-0.1/src/bashgpt/__init__.py
--rw-r--r--   0 petar      (501) staff       (20)      397 2024-05-08 11:06:26.000000 bashgptz-0.1/src/bashgpt/chat.py
--rw-r--r--   0 petar      (501) staff       (20)     1673 2024-05-07 11:56:49.000000 bashgptz-0.1/src/bashgpt/db_and_key.py
--rw-r--r--   0 petar      (501) staff       (20)      536 2024-05-04 13:31:48.000000 bashgptz-0.1/src/bashgpt/defaults.json
--rw-r--r--   0 petar      (501) staff       (20)      642 2024-05-06 14:40:12.000000 bashgptz-0.1/src/bashgpt/extract_text.py
--rw-r--r--   0 petar      (501) staff       (20)     2554 2024-05-08 10:59:07.000000 bashgptz-0.1/src/bashgpt/get_file.py
--rw-r--r--   0 petar      (501) staff       (20)      269 2024-03-21 12:12:57.000000 bashgptz-0.1/src/bashgpt/load_defaults.py
--rwxr-xr-x   0 petar      (501) staff       (20)    29828 2024-05-08 11:13:15.000000 bashgptz-0.1/src/bashgpt/main.py
--rw-r--r--   0 petar      (501) staff       (20)     3146 2024-05-04 12:17:20.000000 bashgptz-0.1/src/bashgpt/models.json
--rw-r--r--   0 petar      (501) staff       (20)     3991 2024-05-04 12:08:13.000000 bashgptz-0.1/src/bashgpt/modes.json
--rw-r--r--   0 petar      (501) staff       (20)      292 2024-05-04 12:17:42.000000 bashgptz-0.1/src/bashgpt/modes_and_models.py
--rw-r--r--   0 petar      (501) staff       (20)      257 2024-05-06 13:16:21.000000 bashgptz-0.1/src/bashgpt/terminal_codes.py
--rw-r--r--   0 petar      (501) staff       (20)     1019 2024-05-08 11:06:11.000000 bashgptz-0.1/src/bashgpt/util_functions.py
--rw-r--r--   0 petar      (501) staff       (20)     1585 2024-05-08 11:03:50.000000 bashgptz-0.1/src/bashgpt/whisper.py
-drwxr-xr-x   0 petar      (501) staff       (20)        0 2024-05-08 12:00:51.418886 bashgptz-0.1/src/bashgptZ.egg-info/
--rw-r--r--   0 petar      (501) staff       (20)     4423 2024-05-08 12:00:51.000000 bashgptz-0.1/src/bashgptZ.egg-info/PKG-INFO
--rw-r--r--   0 petar      (501) staff       (20)      622 2024-05-08 12:00:51.000000 bashgptz-0.1/src/bashgptZ.egg-info/SOURCES.txt
--rw-r--r--   0 petar      (501) staff       (20)        1 2024-05-08 12:00:51.000000 bashgptz-0.1/src/bashgptZ.egg-info/dependency_links.txt
--rw-r--r--   0 petar      (501) staff       (20)       41 2024-05-08 12:00:51.000000 bashgptz-0.1/src/bashgptZ.egg-info/entry_points.txt
--rw-r--r--   0 petar      (501) staff       (20)       49 2024-05-08 12:00:51.000000 bashgptz-0.1/src/bashgptZ.egg-info/requires.txt
--rw-r--r--   0 petar      (501) staff       (20)        8 2024-05-08 12:00:51.000000 bashgptz-0.1/src/bashgptZ.egg-info/top_level.txt
+drwxr-xr-x   0 petar      (501) staff       (20)        0 2024-05-08 11:18:58.188717 bashgptz-1.0/
+-rw-r--r--   0 petar      (501) staff       (20)     1068 2024-05-06 14:50:14.000000 bashgptz-1.0/LICENSE.txt
+-rw-r--r--   0 petar      (501) staff       (20)     4428 2024-05-08 11:18:58.188321 bashgptz-1.0/PKG-INFO
+-rw-r--r--   0 petar      (501) staff       (20)     3907 2024-02-05 20:51:52.000000 bashgptz-1.0/README.md
+-rw-r--r--   0 petar      (501) staff       (20)      587 2024-05-08 11:15:23.000000 bashgptz-1.0/pyproject.toml
+-rw-r--r--   0 petar      (501) staff       (20)       38 2024-05-08 11:18:58.188800 bashgptz-1.0/setup.cfg
+-rw-r--r--   0 petar      (501) staff       (20)      619 2024-05-08 11:04:38.000000 bashgptz-1.0/setup.py
+drwxr-xr-x   0 petar      (501) staff       (20)        0 2024-05-08 11:18:58.178404 bashgptz-1.0/src/
+drwxr-xr-x   0 petar      (501) staff       (20)        0 2024-05-08 11:18:58.186282 bashgptz-1.0/src/bashgpt/
+-rw-r--r--   0 petar      (501) staff       (20)        0 2024-05-06 19:04:03.000000 bashgptz-1.0/src/bashgpt/__init__.py
+-rw-r--r--   0 petar      (501) staff       (20)      397 2024-05-08 11:06:26.000000 bashgptz-1.0/src/bashgpt/chat.py
+-rw-r--r--   0 petar      (501) staff       (20)     1673 2024-05-07 11:56:49.000000 bashgptz-1.0/src/bashgpt/db_and_key.py
+-rw-r--r--   0 petar      (501) staff       (20)      536 2024-05-04 13:31:48.000000 bashgptz-1.0/src/bashgpt/defaults.json
+-rw-r--r--   0 petar      (501) staff       (20)      642 2024-05-06 14:40:12.000000 bashgptz-1.0/src/bashgpt/extract_text.py
+-rw-r--r--   0 petar      (501) staff       (20)     2554 2024-05-08 10:59:07.000000 bashgptz-1.0/src/bashgpt/get_file.py
+-rw-r--r--   0 petar      (501) staff       (20)      269 2024-03-21 12:12:57.000000 bashgptz-1.0/src/bashgpt/load_defaults.py
+-rwxr-xr-x   0 petar      (501) staff       (20)    29828 2024-05-08 11:13:15.000000 bashgptz-1.0/src/bashgpt/main.py
+-rw-r--r--   0 petar      (501) staff       (20)     3146 2024-05-04 12:17:20.000000 bashgptz-1.0/src/bashgpt/models.json
+-rw-r--r--   0 petar      (501) staff       (20)     3991 2024-05-04 12:08:13.000000 bashgptz-1.0/src/bashgpt/modes.json
+-rw-r--r--   0 petar      (501) staff       (20)      292 2024-05-04 12:17:42.000000 bashgptz-1.0/src/bashgpt/modes_and_models.py
+-rw-r--r--   0 petar      (501) staff       (20)      257 2024-05-06 13:16:21.000000 bashgptz-1.0/src/bashgpt/terminal_codes.py
+-rw-r--r--   0 petar      (501) staff       (20)     1019 2024-05-08 11:06:11.000000 bashgptz-1.0/src/bashgpt/util_functions.py
+-rw-r--r--   0 petar      (501) staff       (20)     1585 2024-05-08 11:03:50.000000 bashgptz-1.0/src/bashgpt/whisper.py
+drwxr-xr-x   0 petar      (501) staff       (20)        0 2024-05-08 11:18:58.187812 bashgptz-1.0/src/bashgptZ.egg-info/
+-rw-r--r--   0 petar      (501) staff       (20)     4428 2024-05-08 11:18:58.000000 bashgptz-1.0/src/bashgptZ.egg-info/PKG-INFO
+-rw-r--r--   0 petar      (501) staff       (20)      548 2024-05-08 11:18:58.000000 bashgptz-1.0/src/bashgptZ.egg-info/SOURCES.txt
+-rw-r--r--   0 petar      (501) staff       (20)        1 2024-05-08 11:18:58.000000 bashgptz-1.0/src/bashgptZ.egg-info/dependency_links.txt
+-rw-r--r--   0 petar      (501) staff       (20)        8 2024-05-08 11:18:58.000000 bashgptz-1.0/src/bashgptZ.egg-info/top_level.txt
```

### Comparing `bashgptz-0.1/LICENSE.txt` & `bashgptz-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bashgptz-0.1/PKG-INFO` & `bashgptz-1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: bashgptZ
-Version: 0.1
-Project-URL: Homepage, https://github.com/yourusername/bashgpt
-Project-URL: Bug Tracker, https://github.com/yourusername/bashgpt/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: openai>=1.12.0
-Requires-Dist: anthropic>=0.19.1
-Requires-Dist: PyAudio>=0.2.13
-
 # BashGPT
 
 [!](https://user-images.githubusercontent.com/108212912/253288399-a2b2a520-84ea-458e-8d05-8c4771fd23e6.mov)
 
 ## Introduction
 **Why have all that pretty weak-ass html nonsense when you can just use God's given tool - the t e r m i n a l.**
```

### Comparing `bashgptz-0.1/README.md` & `bashgptz-1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: bashgptZ
+Version: 1.0
+Summary: A powerful and feature rich CLI chatbot interface.
+Author-email: ptrglbvc <petar0golubovic@gmail.com>
+Project-URL: Homepage, https://github.com/ptrglbvc/BashGPT
+Project-URL: Issues, https://github.com/ptrglbvc/BashGPT/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # BashGPT
 
 [!](https://user-images.githubusercontent.com/108212912/253288399-a2b2a520-84ea-458e-8d05-8c4771fd23e6.mov)
 
 ## Introduction
 **Why have all that pretty weak-ass html nonsense when you can just use God's given tool - the t e r m i n a l.**
```

### Comparing `bashgptz-0.1/setup.py` & `bashgptz-1.0/setup.py`

 * *Files identical despite different names*

### Comparing `bashgptz-0.1/src/bashgpt/db_and_key.py` & `bashgptz-1.0/src/bashgpt/db_and_key.py`

 * *Files identical despite different names*

### Comparing `bashgptz-0.1/src/bashgpt/defaults.json` & `bashgptz-1.0/src/bashgpt/defaults.json`

 * *Files identical despite different names*

### Comparing `bashgptz-0.1/src/bashgpt/extract_text.py` & `bashgptz-1.0/src/bashgpt/extract_text.py`

 * *Files identical despite different names*

### Comparing `bashgptz-0.1/src/bashgpt/get_file.py` & `bashgptz-1.0/src/bashgpt/get_file.py`

 * *Files identical despite different names*

### Comparing `bashgptz-0.1/src/bashgpt/main.py` & `bashgptz-1.0/src/bashgpt/main.py`

 * *Files identical despite different names*

### Comparing `bashgptz-0.1/src/bashgpt/models.json` & `bashgptz-1.0/src/bashgpt/models.json`

 * *Files identical despite different names*

### Comparing `bashgptz-0.1/src/bashgpt/modes.json` & `bashgptz-1.0/src/bashgpt/modes.json`

 * *Files identical despite different names*

### Comparing `bashgptz-0.1/src/bashgpt/util_functions.py` & `bashgptz-1.0/src/bashgpt/util_functions.py`

 * *Files identical despite different names*

### Comparing `bashgptz-0.1/src/bashgpt/whisper.py` & `bashgptz-1.0/src/bashgpt/whisper.py`

 * *Files identical despite different names*

### Comparing `bashgptz-0.1/src/bashgptZ.egg-info/PKG-INFO` & `bashgptz-1.0/src/bashgptZ.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: bashgptZ
-Version: 0.1
-Project-URL: Homepage, https://github.com/yourusername/bashgpt
-Project-URL: Bug Tracker, https://github.com/yourusername/bashgpt/issues
+Version: 1.0
+Summary: A powerful and feature rich CLI chatbot interface.
+Author-email: ptrglbvc <petar0golubovic@gmail.com>
+Project-URL: Homepage, https://github.com/ptrglbvc/BashGPT
+Project-URL: Issues, https://github.com/ptrglbvc/BashGPT/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: openai>=1.12.0
-Requires-Dist: anthropic>=0.19.1
-Requires-Dist: PyAudio>=0.2.13
 
 # BashGPT
 
 [!](https://user-images.githubusercontent.com/108212912/253288399-a2b2a520-84ea-458e-8d05-8c4771fd23e6.mov)
 
 ## Introduction
 **Why have all that pretty weak-ass html nonsense when you can just use God's given tool - the t e r m i n a l.**
```

### Comparing `bashgptz-0.1/src/bashgptZ.egg-info/SOURCES.txt` & `bashgptz-1.0/src/bashgptZ.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,10 +15,8 @@
 src/bashgpt/modes_and_models.py
 src/bashgpt/terminal_codes.py
 src/bashgpt/util_functions.py
 src/bashgpt/whisper.py
 src/bashgptZ.egg-info/PKG-INFO
 src/bashgptZ.egg-info/SOURCES.txt
 src/bashgptZ.egg-info/dependency_links.txt
-src/bashgptZ.egg-info/entry_points.txt
-src/bashgptZ.egg-info/requires.txt
 src/bashgptZ.egg-info/top_level.txt
```

