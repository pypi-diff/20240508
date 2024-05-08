# Comparing `tmp/lotgi-0.0.6.tar.gz` & `tmp/lotgi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lotgi-0.0.6.tar", last modified: Tue May  7 04:34:17 2024, max compression
+gzip compressed data, was "lotgi-0.0.7.tar", last modified: Wed May  8 02:51:43 2024, max compression
```

## Comparing `lotgi-0.0.6.tar` & `lotgi-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-07 04:34:17.182882 lotgi-0.0.6/
--rw-r--r--   0 alex       (501) staff       (20)      525 2024-05-07 04:34:17.182731 lotgi-0.0.6/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      705 2024-05-07 04:30:59.000000 lotgi-0.0.6/pyproject.toml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-07 04:34:17.180247 lotgi-0.0.6/python/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-07 04:34:17.181399 lotgi-0.0.6/python/lotgi/
--rw-r--r--   0 alex       (501) staff       (20)     7831 2024-05-07 04:30:28.000000 lotgi-0.0.6/python/lotgi/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)       61 2024-04-27 22:29:31.000000 lotgi-0.0.6/python/lotgi/__main__.py
--rw-r--r--   0 alex       (501) staff       (20)      706 2024-04-11 20:15:07.000000 lotgi-0.0.6/python/lotgi/_openai.py
--rw-r--r--   0 alex       (501) staff       (20)      383 2024-04-11 18:54:15.000000 lotgi-0.0.6/python/lotgi/logging.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-07 04:34:17.182145 lotgi-0.0.6/python/lotgi/models/
--rw-r--r--   0 alex       (501) staff       (20)     2203 2024-05-07 04:23:13.000000 lotgi-0.0.6/python/lotgi/models/rest.py
--rw-r--r--   0 alex       (501) staff       (20)     6014 2024-05-07 04:24:19.000000 lotgi-0.0.6/python/lotgi/rest_client.py
--rw-r--r--   0 alex       (501) staff       (20)     1316 2024-05-01 23:14:33.000000 lotgi-0.0.6/python/lotgi/tokens.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-07 04:34:17.182558 lotgi-0.0.6/python/lotgi.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      525 2024-05-07 04:34:17.000000 lotgi-0.0.6/python/lotgi.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      436 2024-05-07 04:34:17.000000 lotgi-0.0.6/python/lotgi.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-05-07 04:34:17.000000 lotgi-0.0.6/python/lotgi.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       36 2024-05-07 04:34:17.000000 lotgi-0.0.6/python/lotgi.egg-info/entry_points.txt
--rw-r--r--   0 alex       (501) staff       (20)       95 2024-05-07 04:34:17.000000 lotgi-0.0.6/python/lotgi.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       12 2024-05-07 04:34:17.000000 lotgi-0.0.6/python/lotgi.egg-info/top_level.txt
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-07 04:34:17.182283 lotgi-0.0.6/python/tests/
--rw-r--r--   0 alex       (501) staff       (20)       49 2024-04-08 18:16:29.000000 lotgi-0.0.6/python/tests/test_basic.py
--rw-r--r--   0 alex       (501) staff       (20)       38 2024-05-07 04:34:17.182910 lotgi-0.0.6/setup.cfg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-08 02:51:43.379283 lotgi-0.0.7/
+-rw-r--r--   0 alex       (501) staff       (20)      525 2024-05-08 02:51:43.379123 lotgi-0.0.7/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      705 2024-05-08 02:51:39.000000 lotgi-0.0.7/pyproject.toml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-08 02:51:43.376769 lotgi-0.0.7/python/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-08 02:51:43.377509 lotgi-0.0.7/python/lotgi/
+-rw-r--r--   0 alex       (501) staff       (20)     7831 2024-05-08 02:44:06.000000 lotgi-0.0.7/python/lotgi/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)       61 2024-04-27 22:29:31.000000 lotgi-0.0.7/python/lotgi/__main__.py
+-rw-r--r--   0 alex       (501) staff       (20)      706 2024-04-11 20:15:07.000000 lotgi-0.0.7/python/lotgi/_openai.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-08 02:51:43.378263 lotgi-0.0.7/python/lotgi/asyncio/
+-rw-r--r--   0 alex       (501) staff       (20)     1015 2024-05-07 20:29:22.000000 lotgi-0.0.7/python/lotgi/asyncio/rest_client.py
+-rw-r--r--   0 alex       (501) staff       (20)      383 2024-04-11 18:54:15.000000 lotgi-0.0.7/python/lotgi/logging.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-08 02:51:43.378506 lotgi-0.0.7/python/lotgi/models/
+-rw-r--r--   0 alex       (501) staff       (20)     2203 2024-05-07 04:23:13.000000 lotgi-0.0.7/python/lotgi/models/rest.py
+-rw-r--r--   0 alex       (501) staff       (20)     6156 2024-05-08 02:51:15.000000 lotgi-0.0.7/python/lotgi/rest_client.py
+-rw-r--r--   0 alex       (501) staff       (20)     1316 2024-05-01 23:14:33.000000 lotgi-0.0.7/python/lotgi/tokens.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-08 02:51:43.378938 lotgi-0.0.7/python/lotgi.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)      525 2024-05-08 02:51:43.000000 lotgi-0.0.7/python/lotgi.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      472 2024-05-08 02:51:43.000000 lotgi-0.0.7/python/lotgi.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-05-08 02:51:43.000000 lotgi-0.0.7/python/lotgi.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       36 2024-05-08 02:51:43.000000 lotgi-0.0.7/python/lotgi.egg-info/entry_points.txt
+-rw-r--r--   0 alex       (501) staff       (20)       95 2024-05-08 02:51:43.000000 lotgi-0.0.7/python/lotgi.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       12 2024-05-08 02:51:43.000000 lotgi-0.0.7/python/lotgi.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-08 02:51:43.378651 lotgi-0.0.7/python/tests/
+-rw-r--r--   0 alex       (501) staff       (20)       49 2024-04-08 18:16:29.000000 lotgi-0.0.7/python/tests/test_basic.py
+-rw-r--r--   0 alex       (501) staff       (20)       38 2024-05-08 02:51:43.379317 lotgi-0.0.7/setup.cfg
```

### Comparing `lotgi-0.0.6/PKG-INFO` & `lotgi-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lotgi
-Version: 0.0.6
+Version: 0.0.7
 Summary: For the love of the game
 Author-email: Alex Wu <alexanderwu@berkeley.edu>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: click>=7.0
```

### Comparing `lotgi-0.0.6/pyproject.toml` & `lotgi-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   "tabulate",
   "transformers",
   "openai",
   "tomli",
   "pandas",
   "shortuuid",
 ]
-version="0.0.6"
+version="0.0.7"
 
 
 [tool.setuptools.packages.find]
 where = ["python/"]
 
 [project.scripts]
 lotgi = "lotgi:cli"
```

### Comparing `lotgi-0.0.6/python/lotgi/__init__.py` & `lotgi-0.0.7/python/lotgi/__init__.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.6/python/lotgi/_openai.py` & `lotgi-0.0.7/python/lotgi/_openai.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.6/python/lotgi/models/rest.py` & `lotgi-0.0.7/python/lotgi/models/rest.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.6/python/lotgi/rest_client.py` & `lotgi-0.0.7/python/lotgi/rest_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,23 +78,28 @@
 
 
         if max_output_tokens is None:
             max_output_tokens = rest.DEFAULT_MAX_OUTPUT_TOKENS
         if regex  is None:
             regex = rest.DEFAULT_REGEX
 
+        if _autodetect_cloud_credentials:
+            huggingface_token = get_huggingface_credentials()
+        else:
+            huggingface_token = ""
+
         job_spec = rest.JobSpec(
             cloud_credentials=cloud_credentials,
             input_file=input_file,
             model=model,
             field=field,
             target_cost=target_cost,
             target_deadline=target_deadline,
             execution_tradeoff=execution_tradeoff,
-            huggingface_token=get_huggingface_credentials(),
+            huggingface_token=huggingface_token,
             max_output_tokens=max_output_tokens,
             regex=regex,
         )
 
 
         body = job_spec.dict()
```

### Comparing `lotgi-0.0.6/python/lotgi/tokens.py` & `lotgi-0.0.7/python/lotgi/tokens.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.6/python/lotgi.egg-info/PKG-INFO` & `lotgi-0.0.7/python/lotgi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lotgi
-Version: 0.0.6
+Version: 0.0.7
 Summary: For the love of the game
 Author-email: Alex Wu <alexanderwu@berkeley.edu>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: click>=7.0
```

